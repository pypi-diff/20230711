# Comparing `tmp/swanapi-0.2.0-py3-none-any.whl.zip` & `tmp/swanapi-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,19 @@
-Zip file size: 10878 bytes, number of entries: 15
+Zip file size: 15835 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      157 b- defN 23-Jul-11 00:16 swanapi/__init__.py
 -rw-r--r--  2.0 unx     8931 b- defN 23-Jul-11 01:15 swanapi/base_inference.py
 -rw-r--r--  2.0 unx     1831 b- defN 23-Jul-11 00:57 swanapi/base_requests.py
 -rw-r--r--  2.0 unx      863 b- defN 23-Jul-09 17:55 swanapi/make_build.py
 -rw-r--r--  2.0 unx     2769 b- defN 23-Jul-11 00:45 swanapi/server.py
 -rw-r--r--  2.0 unx      562 b- defN 23-Jul-10 19:06 swanapi/swan_types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
 -rw-r--r--  2.0 unx     3889 b- defN 23-Jul-09 18:35 swanapi/docker_builder/config.py
 -rw-r--r--  2.0 unx     3348 b- defN 23-Jul-09 18:53 swanapi/docker_builder/generate_dockerfile.py
 -rw-r--r--  2.0 unx     1419 b- defN 23-Jul-09 18:39 swanapi/docker_builder/runner.py
--rw-r--r--  2.0 unx      340 b- defN 23-Jul-11 01:16 swanapi-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 01:16 swanapi-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jul-11 01:16 swanapi-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 01:16 swanapi-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1225 b- defN 23-Jul-11 01:16 swanapi-0.2.0.dist-info/RECORD
-15 files, 25484 bytes uncompressed, 8840 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 01:19 swanapi/utils/__init__.py
+-rw-r--r--  2.0 unx    15239 b- defN 23-Jul-11 00:31 swanapi/utils/utils.py
+-rw-r--r--  2.0 unx      340 b- defN 23-Jul-11 01:19 swanapi-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 01:19 swanapi-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-11 01:19 swanapi-0.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 01:19 swanapi-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1384 b- defN 23-Jul-11 01:19 swanapi-0.2.1.dist-info/RECORD
+17 files, 40882 bytes uncompressed, 13551 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -24,23 +24,29 @@
 
 Filename: swanapi/docker_builder/generate_dockerfile.py
 Comment: 
 
 Filename: swanapi/docker_builder/runner.py
 Comment: 
 
-Filename: swanapi-0.2.0.dist-info/METADATA
+Filename: swanapi/utils/__init__.py
 Comment: 
 
-Filename: swanapi-0.2.0.dist-info/WHEEL
+Filename: swanapi/utils/utils.py
 Comment: 
 
-Filename: swanapi-0.2.0.dist-info/entry_points.txt
+Filename: swanapi-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.2.0.dist-info/top_level.txt
+Filename: swanapi-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.2.0.dist-info/RECORD
+Filename: swanapi-0.2.1.dist-info/entry_points.txt
+Comment: 
+
+Filename: swanapi-0.2.1.dist-info/top_level.txt
+Comment: 
+
+Filename: swanapi-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `swanapi-0.2.0.dist-info/RECORD` & `swanapi-0.2.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -4,12 +4,14 @@
 swanapi/make_build.py,sha256=P4WsA52pftJyNLrU986UKkYPY88VLzRMgQJ6s_UUTY0,863
 swanapi/server.py,sha256=eLtrZmN0RU9RP9Yzh7z33lqkzaZerylNHAVhYXxkr4E,2769
 swanapi/swan_types.py,sha256=6rjoLVOqyahSQXilAVtMVS4e50MNeCMEBinPu3jR_JE,562
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swanapi/docker_builder/config.py,sha256=CspWGMAyxZz_rd2JecCrsC4nL75Zh3o7XGAXMVHa32o,3889
 swanapi/docker_builder/generate_dockerfile.py,sha256=bbd2u94MgyZq883WrTtk936TM-6eUYTuc1ZqgVdgM90,3348
 swanapi/docker_builder/runner.py,sha256=uDToZ5UfgshahcnKbu8Eb7enLLry2pVHn7e2bJB56vk,1419
-swanapi-0.2.0.dist-info/METADATA,sha256=7m2ryE58-cufMAIClPhrkiNxQw7gEBJvvY1avCS92EE,340
-swanapi-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.2.0.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
-swanapi-0.2.0.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.2.0.dist-info/RECORD,,
+swanapi/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+swanapi/utils/utils.py,sha256=jx9anz_ty9T1FAJRAT8eLlsKoCOGha4CsPzKa2plK50,15239
+swanapi-0.2.1.dist-info/METADATA,sha256=8tapJs7f6UhkO3VOqSjhI2pRDoR1okRjIDqAebc-A7s,340
+swanapi-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.2.1.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
+swanapi-0.2.1.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.2.1.dist-info/RECORD,,
```

