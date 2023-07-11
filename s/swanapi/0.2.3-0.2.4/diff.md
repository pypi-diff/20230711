# Comparing `tmp/swanapi-0.2.3-py3-none-any.whl.zip` & `tmp/swanapi-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 17232 bytes, number of entries: 18
+Zip file size: 17399 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      157 b- defN 23-Jul-11 00:16 swanapi/__init__.py
 -rw-r--r--  2.0 unx     8931 b- defN 23-Jul-11 01:15 swanapi/base_inference.py
 -rw-r--r--  2.0 unx     1831 b- defN 23-Jul-11 00:57 swanapi/base_requests.py
 -rw-r--r--  2.0 unx      863 b- defN 23-Jul-09 17:55 swanapi/make_build.py
 -rw-r--r--  2.0 unx     2746 b- defN 23-Jul-11 03:40 swanapi/server.py
 -rw-r--r--  2.0 unx      562 b- defN 23-Jul-10 19:06 swanapi/swan_types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
 -rw-r--r--  2.0 unx     3953 b- defN 23-Jul-11 07:06 swanapi/docker_builder/config.py
--rw-r--r--  2.0 unx     3739 b- defN 23-Jul-11 07:27 swanapi/docker_builder/cuda_container.py
+-rw-r--r--  2.0 unx     4689 b- defN 23-Jul-11 13:47 swanapi/docker_builder/cuda_container.py
 -rw-r--r--  2.0 unx     3348 b- defN 23-Jul-09 18:53 swanapi/docker_builder/generate_dockerfile.py
 -rw-r--r--  2.0 unx     1901 b- defN 23-Jul-11 07:25 swanapi/docker_builder/runner.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 01:19 swanapi/utils/__init__.py
 -rw-r--r--  2.0 unx    15239 b- defN 23-Jul-11 00:31 swanapi/utils/utils.py
--rw-r--r--  2.0 unx      368 b- defN 23-Jul-11 07:27 swanapi-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 07:27 swanapi-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jul-11 07:27 swanapi-0.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 07:27 swanapi-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1481 b- defN 23-Jul-11 07:27 swanapi-0.2.3.dist-info/RECORD
-18 files, 45269 bytes uncompressed, 14792 bytes compressed:  67.3%
+-rw-r--r--  2.0 unx      368 b- defN 23-Jul-11 14:18 swanapi-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 14:18 swanapi-0.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-11 14:18 swanapi-0.2.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 14:18 swanapi-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1481 b- defN 23-Jul-11 14:18 swanapi-0.2.4.dist-info/RECORD
+18 files, 46219 bytes uncompressed, 14959 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: swanapi/utils/__init__.py
 Comment: 
 
 Filename: swanapi/utils/utils.py
 Comment: 
 
-Filename: swanapi-0.2.3.dist-info/METADATA
+Filename: swanapi-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.2.3.dist-info/WHEEL
+Filename: swanapi-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.2.3.dist-info/entry_points.txt
+Filename: swanapi-0.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.2.3.dist-info/top_level.txt
+Filename: swanapi-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.2.3.dist-info/RECORD
+Filename: swanapi-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swanapi/docker_builder/cuda_container.py

```diff
@@ -1,8 +1,23 @@
 from pynvml import *
+import platform
+
+
+def platform_detect():
+    platform_system = platform.system().lower()
+    # if "macos" in platform_system:
+    #     return "macos"
+    if "windows" in platform_system:
+        return "windows"
+    elif "wsl" in platform_system:
+        return "wsl"
+    elif "linux" in platform_system:
+        return "linux"
+    else:
+        raise ValueError("不支持的操作系统")
 
 
 class NVDetection():
     def __init__(self):
         try:
             nvmlInit()
         except NVMLError:
@@ -44,23 +59,34 @@
     def __init__(self, nv_info: NVDetection):
         self.nv_info = nv_info
         self.nv_driver_version = self.nv_info.get_nv_driver_version()
         self.cuda_version = self.nv_info.get_cuda_version()[0][:4]
         self.cuda_base_image_tag = self.get_cuda_base_image_tag()
 
     def get_gpu_command(self):
-        commond = f"""
+        platform_system = platform_detect()
+
+        if platform_system == "wsl":
+            commond = f"""
 distribution=$(. /etc/os-release;echo $ID$VERSION_ID)
 curl -s -L https://nvidia.github.io/nvidia-docker/gpgkey | sudo apt-key add -
 curl -s -L https://nvidia.github.io/nvidia-docker/$distribution/nvidia-docker.list | sudo tee /etc/apt/sources.list.d/nvidia-docker.list
 sudo apt-get update && sudo apt-get install -y nvidia-container-toolkit
-sudo systemctl restart docker
+sudo service restart docker
 docker pull {self.cuda_base_image_tag}
         """
-
+        else:
+            commond = f"""
+distribution=$(. /etc/os-release;echo $ID$VERSION_ID)
+curl -s -L https://nvidia.github.io/nvidia-docker/gpgkey | sudo apt-key add -
+curl -s -L https://nvidia.github.io/nvidia-docker/$distribution/nvidia-docker.list | sudo tee /etc/apt/sources.list.d/nvidia-docker.list
+sudo apt-get update && sudo apt-get install -y nvidia-container-toolkit
+sudo systemctl restart docker
+docker pull {self.cuda_base_image_tag}
+                    """
         return commond
 
     def get_cuda_base_image_tag(self):
         if self.cuda_version == "1100":
             cuda_base_image = "nvidia/cuda:11.0.3-base-ubuntu20.04"
         elif self.cuda_version == "1100":
             cuda_base_image = "nvidia/cuda:11.0.3-base-ubuntu20.04"
```

## Comparing `swanapi-0.2.3.dist-info/RECORD` & `swanapi-0.2.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 swanapi/base_inference.py,sha256=QlWvZI1rpff8pdcMLQ-AKDBHbAIKulXDXJd2I6TAnJw,8931
 swanapi/base_requests.py,sha256=kpGxsP26WgZG7SroPCoDZl_7fjsgHmXOSFHGKbCnozc,1831
 swanapi/make_build.py,sha256=P4WsA52pftJyNLrU986UKkYPY88VLzRMgQJ6s_UUTY0,863
 swanapi/server.py,sha256=AuVDQd_AJbBejrYT5MY5R0NIM64_9QWMCUhqzfUH0Vw,2746
 swanapi/swan_types.py,sha256=6rjoLVOqyahSQXilAVtMVS4e50MNeCMEBinPu3jR_JE,562
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swanapi/docker_builder/config.py,sha256=oMHdFbV8zGzlsIfMjPT1PimM1t6LLnkEIuKxEpjiANM,3953
-swanapi/docker_builder/cuda_container.py,sha256=M0nMeGXwhKCQ1XdqaBNVO3tshEs6d4pwY8HkcXC3FpM,3739
+swanapi/docker_builder/cuda_container.py,sha256=HBVrWfq7_SkUrC_L9D9oCCCDHChuw-GV09AasrCDGlE,4689
 swanapi/docker_builder/generate_dockerfile.py,sha256=bbd2u94MgyZq883WrTtk936TM-6eUYTuc1ZqgVdgM90,3348
 swanapi/docker_builder/runner.py,sha256=rHLlSWqyJkXfWbSIBJGTWfiqtzsOdXYQZrHR0OoUAh8,1901
 swanapi/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swanapi/utils/utils.py,sha256=jx9anz_ty9T1FAJRAT8eLlsKoCOGha4CsPzKa2plK50,15239
-swanapi-0.2.3.dist-info/METADATA,sha256=kUaOrop9Pnmzvf6mAI02y8BSlMoJgI6ORSoKYeBcxl4,368
-swanapi-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.2.3.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
-swanapi-0.2.3.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.2.3.dist-info/RECORD,,
+swanapi-0.2.4.dist-info/METADATA,sha256=RG26okDn3ifK611GQf6mkWLJ4g9daXQHESAGejOP4xg,368
+swanapi-0.2.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.2.4.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
+swanapi-0.2.4.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.2.4.dist-info/RECORD,,
```

