# Comparing `tmp/easy-kubeflow-0.0.8.tar.gz` & `tmp/easy-kubeflow-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy-kubeflow-0.0.8.tar", last modified: Wed Jun 14 04:37:48 2023, max compression
+gzip compressed data, was "dist/easy-kubeflow-0.0.9.tar", last modified: Tue Jul 11 05:26:02 2023, max compression
```

## Comparing `easy-kubeflow-0.0.8.tar` & `easy-kubeflow-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/
--rw-r--r--   0 lwb        (501) staff       (20)      492 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/PKG-INFO
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/
--rw-r--r--   0 lwb        (501) staff       (20)      492 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/PKG-INFO
--rw-r--r--   0 lwb        (501) staff       (20)      476 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/SOURCES.txt
--rw-r--r--   0 lwb        (501) staff       (20)       52 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/requires.txt
--rw-r--r--   0 lwb        (501) staff       (20)       14 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/top_level.txt
--rw-r--r--   0 lwb        (501) staff       (20)        1 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow.egg-info/dependency_links.txt
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow/
--rw-r--r--   0 lwb        (501) staff       (20)      122 2021-12-16 02:31:39.000000 easy-kubeflow-0.0.8/easy_kubeflow/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow/pipelines/
--rw-r--r--   0 lwb        (501) staff       (20)       69 2021-12-16 02:30:40.000000 easy-kubeflow-0.0.8/easy_kubeflow/pipelines/__init__.py
--rw-r--r--   0 lwb        (501) staff       (20)    21815 2023-06-14 03:54:58.000000 easy-kubeflow-0.0.8/easy_kubeflow/pipelines/pipelines_util.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow/utils/
--rw-r--r--   0 lwb        (501) staff       (20)     1140 2021-12-16 02:29:02.000000 easy-kubeflow-0.0.8/easy_kubeflow/utils/log_util.py
--rw-r--r--   0 lwb        (501) staff       (20)       31 2021-12-16 02:30:25.000000 easy-kubeflow-0.0.8/easy_kubeflow/utils/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow/examples/
--rw-r--r--   0 lwb        (501) staff       (20)        0 2021-12-16 08:21:23.000000 easy-kubeflow-0.0.8/easy_kubeflow/examples/__init__.py
-drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/easy_kubeflow/_docker/
--rw-r--r--   0 lwb        (501) staff       (20)       36 2021-12-16 02:30:53.000000 easy-kubeflow-0.0.8/easy_kubeflow/_docker/__init__.py
--rw-r--r--   0 lwb        (501) staff       (20)    22930 2022-12-05 06:17:57.000000 easy-kubeflow-0.0.8/easy_kubeflow/_docker/docker_util.py
--rw-r--r--   0 lwb        (501) staff       (20)     7231 2023-02-27 10:44:37.000000 easy-kubeflow-0.0.8/README.md
--rw-r--r--   0 lwb        (501) staff       (20)      836 2023-06-14 04:37:35.000000 easy-kubeflow-0.0.8/setup.py
--rw-r--r--   0 lwb        (501) staff       (20)       38 2023-06-14 04:37:48.000000 easy-kubeflow-0.0.8/setup.cfg
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/
+-rw-r--r--   0 lwb        (501) staff       (20)      492 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/PKG-INFO
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow.egg-info/
+-rw-r--r--   0 lwb        (501) staff       (20)      492 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow.egg-info/PKG-INFO
+-rw-r--r--   0 lwb        (501) staff       (20)      476 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow.egg-info/SOURCES.txt
+-rw-r--r--   0 lwb        (501) staff       (20)       52 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow.egg-info/requires.txt
+-rw-r--r--   0 lwb        (501) staff       (20)       14 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow.egg-info/top_level.txt
+-rw-r--r--   0 lwb        (501) staff       (20)        1 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow.egg-info/dependency_links.txt
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow/
+-rw-r--r--   0 lwb        (501) staff       (20)      122 2021-12-16 02:31:39.000000 easy-kubeflow-0.0.9/easy_kubeflow/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow/pipelines/
+-rw-r--r--   0 lwb        (501) staff       (20)       69 2021-12-16 02:30:40.000000 easy-kubeflow-0.0.9/easy_kubeflow/pipelines/__init__.py
+-rw-r--r--   0 lwb        (501) staff       (20)    22851 2023-07-11 05:25:51.000000 easy-kubeflow-0.0.9/easy_kubeflow/pipelines/pipelines_util.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow/utils/
+-rw-r--r--   0 lwb        (501) staff       (20)     1140 2021-12-16 02:29:02.000000 easy-kubeflow-0.0.9/easy_kubeflow/utils/log_util.py
+-rw-r--r--   0 lwb        (501) staff       (20)       31 2021-12-16 02:30:25.000000 easy-kubeflow-0.0.9/easy_kubeflow/utils/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow/examples/
+-rw-r--r--   0 lwb        (501) staff       (20)        0 2021-12-16 08:21:23.000000 easy-kubeflow-0.0.9/easy_kubeflow/examples/__init__.py
+drwxr-xr-x   0 lwb        (501) staff       (20)        0 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/easy_kubeflow/_docker/
+-rw-r--r--   0 lwb        (501) staff       (20)       36 2021-12-16 02:30:53.000000 easy-kubeflow-0.0.9/easy_kubeflow/_docker/__init__.py
+-rw-r--r--   0 lwb        (501) staff       (20)    22930 2022-12-05 06:17:57.000000 easy-kubeflow-0.0.9/easy_kubeflow/_docker/docker_util.py
+-rw-r--r--   0 lwb        (501) staff       (20)     7231 2023-02-27 10:44:37.000000 easy-kubeflow-0.0.9/README.md
+-rw-r--r--   0 lwb        (501) staff       (20)      836 2023-07-11 05:25:51.000000 easy-kubeflow-0.0.9/setup.py
+-rw-r--r--   0 lwb        (501) staff       (20)       38 2023-07-11 05:26:02.000000 easy-kubeflow-0.0.9/setup.cfg
```

### Comparing `easy-kubeflow-0.0.8/easy_kubeflow/pipelines/pipelines_util.py` & `easy-kubeflow-0.0.9/easy_kubeflow/pipelines/pipelines_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -342,14 +342,30 @@
         ) \
             .container \
             .add_volume_mount(
             k8s_client.V1VolumeMount(
                 mount_path=self.nfs_path,
                 name=self.uuid + '-pv')
         )
+
+        # add shm for pytorch multiple worker use
+        self.op.add_volume(
+            k8s_client.V1Volume(name='dshm',
+                                empty_dir=k8s_client.V1EmptyDirVolumeSource(
+                                    medium='Memory'
+                                )
+                                )
+        ) \
+            .container \
+            .add_volume_mount(
+            k8s_client.V1VolumeMount(
+                mount_path='/dev/shm',
+                name='dshm'
+            )
+        )
         _logger.info("Nfs server master host is: %s" % self.nfs_master_host)
         _logger.info("Nfs server mount path: %s" % self.nfs_path)
 
     def _node_selecter(self, strategies: Optional[list] = None):
         """
         add pod's node select strategies
         :param strategies: strategy list
@@ -524,14 +540,30 @@
         ) \
             .container \
             .add_volume_mount(
             k8s_client.V1VolumeMount(
                 mount_path=self.nfs_path,
                 name=self.uuid + '-pv')
         )
+
+        # add shm for pytorch multiple worker use
+        self.op.add_volume(
+            k8s_client.V1Volume(name='dshm',
+                                empty_dir=k8s_client.V1EmptyDirVolumeSource(
+                                    medium='Memory'
+                                )
+                                )
+        ) \
+            .container \
+            .add_volume_mount(
+            k8s_client.V1VolumeMount(
+                mount_path='/dev/shm',
+                name='dshm'
+            )
+        )
         _logger.info("Nfs server master host is: %s" % self.nfs_master_host)
         _logger.info("Nfs server mount path: %s" % self.nfs_path)
 
     def _node_selecter(self, strategies: Optional[list] = None):
         """
         add pod's node select strategies
         :param strategies: strategy list
```

### Comparing `easy-kubeflow-0.0.8/easy_kubeflow/utils/log_util.py` & `easy-kubeflow-0.0.9/easy_kubeflow/utils/log_util.py`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.0.8/easy_kubeflow/_docker/docker_util.py` & `easy-kubeflow-0.0.9/easy_kubeflow/_docker/docker_util.py`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.0.8/README.md` & `easy-kubeflow-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `easy-kubeflow-0.0.8/setup.py` & `easy-kubeflow-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = None
 
 setuptools.setup(
     name="easy-kubeflow",  # Replace with your own name
-    version="0.0.8",
+    version="0.0.9",
     author="CrazyBean",
     author_email="liuweibin@stonewise.cn",
     description="sdk help users for a better use of kubeflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://service.stonewise.cn:8029/liuweibin/easy-kubeflow.git",
     install_requires=[
```

