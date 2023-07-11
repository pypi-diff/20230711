# Comparing `tmp/napari-stpt-0.1.0.5.tar.gz` & `tmp/napari-stpt-0.1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-stpt-0.1.0.5.tar", last modified: Mon Jul 10 11:51:53 2023, max compression
+gzip compressed data, was "napari-stpt-0.1.0.6.tar", last modified: Tue Jul 11 11:36:39 2023, max compression
```

## Comparing `napari-stpt-0.1.0.5.tar` & `napari-stpt-0.1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 11:51:53.629359 napari-stpt-0.1.0.5/
--rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.5/LICENSE
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-07-10 11:51:53.627359 napari-stpt-0.1.0.5/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.1.0.5/README.md
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 11:51:53.566359 napari-stpt-0.1.0.5/napari_stpt/
--rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.5/napari_stpt/__init__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.1.0.5/napari_stpt/__main__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)   147412 2023-07-10 11:01:58.000000 napari-stpt-0.1.0.5/napari_stpt/napari_stpt.py
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 11:51:53.625359 napari-stpt-0.1.0.5/napari_stpt.egg-info/
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)      313 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/SOURCES.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/dependency_links.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/entry_points.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)      116 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/requires.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2023-07-10 11:51:53.000000 napari-stpt-0.1.0.5/napari_stpt.egg-info/top_level.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2023-07-10 11:51:53.629359 napari-stpt-0.1.0.5/setup.cfg
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1343 2023-07-10 11:51:44.000000 napari-stpt-0.1.0.5/setup.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-11 11:36:39.661655 napari-stpt-0.1.0.6/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.6/LICENSE
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-07-11 11:36:39.660655 napari-stpt-0.1.0.6/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.1.0.6/README.md
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-11 11:36:39.640655 napari-stpt-0.1.0.6/napari_stpt/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.6/napari_stpt/__init__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.1.0.6/napari_stpt/__main__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)   147543 2023-07-11 06:07:39.000000 napari-stpt-0.1.0.6/napari_stpt/napari_stpt.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-11 11:36:39.657655 napari-stpt-0.1.0.6/napari_stpt.egg-info/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-07-11 11:36:39.000000 napari-stpt-0.1.0.6/napari_stpt.egg-info/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      313 2023-07-11 11:36:39.000000 napari-stpt-0.1.0.6/napari_stpt.egg-info/SOURCES.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-07-11 11:36:39.000000 napari-stpt-0.1.0.6/napari_stpt.egg-info/dependency_links.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2023-07-11 11:36:39.000000 napari-stpt-0.1.0.6/napari_stpt.egg-info/entry_points.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      116 2023-07-11 11:36:39.000000 napari-stpt-0.1.0.6/napari_stpt.egg-info/requires.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2023-07-11 11:36:39.000000 napari-stpt-0.1.0.6/napari_stpt.egg-info/top_level.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2023-07-11 11:36:39.662655 napari-stpt-0.1.0.6/setup.cfg
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     1343 2023-07-11 11:35:59.000000 napari-stpt-0.1.0.6/setup.py
```

### Comparing `napari-stpt-0.1.0.5/LICENSE` & `napari-stpt-0.1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.0.5/PKG-INFO` & `napari-stpt-0.1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.1.0.5
+Version: 0.1.0.6
 Summary: napari viewer which can read stpt images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.1.0.5/README.md` & `napari-stpt-0.1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.0.5/napari_stpt/napari_stpt.py` & `napari-stpt-0.1.0.6/napari_stpt/napari_stpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,42 +358,43 @@
                 pass
             
             if verbose:
                 print(f"reference_size: {reference_size}")
     
             
         # Remove previous volumes
-        try:
-            if not load_in_reference:
-                self.viewer.layers.remove('C1')
-            del self.aligned_1
-            self.aligned_1 = None
-        except Exception:
-            pass
-        try:
-            if not load_in_reference:
-                self.viewer.layers.remove('C2')
-            del self.aligned_2
-            self.aligned_2 = None
-        except Exception:
-            pass
-        try:
-            if not load_in_reference:
-                self.viewer.layers.remove('C3')
-            del self.aligned_3
-            self.aligned_3 = None
-        except Exception:
-            pass
-        try:
-            if not load_in_reference:
-                self.viewer.layers.remove('C4')
-            del self.aligned_4
-            self.aligned_4 = None
-        except Exception:
-            pass
+        if False:
+            try:
+                if not load_in_reference:
+                    self.viewer.layers.remove('C1')
+                del self.aligned_1
+                self.aligned_1 = None
+            except Exception:
+                pass
+            try:
+                if not load_in_reference:
+                    self.viewer.layers.remove('C2')
+                del self.aligned_2
+                self.aligned_2 = None
+            except Exception:
+                pass
+            try:
+                if not load_in_reference:
+                    self.viewer.layers.remove('C3')
+                del self.aligned_3
+                self.aligned_3 = None
+            except Exception:
+                pass
+            try:
+                if not load_in_reference:
+                    self.viewer.layers.remove('C4')
+                del self.aligned_4
+                self.aligned_4 = None
+            except Exception:
+                pass
 
         # Clear memory
         gc.collect()
 
         
         
         for folder in self.image_folders:
```

### Comparing `napari-stpt-0.1.0.5/napari_stpt.egg-info/PKG-INFO` & `napari-stpt-0.1.0.6/napari_stpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.1.0.5
+Version: 0.1.0.6
 Summary: napari viewer which can read stpt images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.1.0.5/setup.py` & `napari-stpt-0.1.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # this grabs the requirements from requirements.txt
 #REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 # This call to setup() does all the work
 setup(
     name="napari-stpt",
-    version="0.1.0.5",
+    version="0.1.0.6",
     description="napari viewer which can read stpt images as zarr files",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/TristanWhitmarsh/napari-stpt",
     author="Tristan Whitmarsh",
     author_email="tw401@cam.ac.uk",
     license="GNU",
```

