# Comparing `tmp/disksurf-1.2.3.tar.gz` & `tmp/disksurf-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disksurf-1.2.3.tar", last modified: Thu Jun  1 10:01:17 2023, max compression
+gzip compressed data, was "disksurf-1.2.4.tar", last modified: Tue Jul 11 15:06:57 2023, max compression
```

## Comparing `disksurf-1.2.3.tar` & `disksurf-1.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-06-01 10:01:17.872152 disksurf-1.2.3/
--rw-r--r--   0 richardteague   (501) staff       (20)     1068 2023-03-27 18:30:47.000000 disksurf-1.2.3/LICENSE
--rw-r--r--   0 richardteague   (501) staff       (20)     3728 2023-06-01 10:01:17.872057 disksurf-1.2.3/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)     3297 2023-03-27 18:30:47.000000 disksurf-1.2.3/README.md
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-06-01 10:01:17.871364 disksurf-1.2.3/disksurf/
--rw-r--r--   0 richardteague   (501) staff       (20)      103 2023-03-27 18:30:47.000000 disksurf-1.2.3/disksurf/__init__.py
--rw-r--r--   0 richardteague   (501) staff       (20)    58364 2023-06-01 10:00:09.000000 disksurf-1.2.3/disksurf/observation.py
--rw-r--r--   0 richardteague   (501) staff       (20)    61353 2023-03-27 18:30:47.000000 disksurf-1.2.3/disksurf/surface.py
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-06-01 10:01:17.871905 disksurf-1.2.3/disksurf.egg-info/
--rw-r--r--   0 richardteague   (501) staff       (20)     3728 2023-06-01 10:01:17.000000 disksurf-1.2.3/disksurf.egg-info/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)      250 2023-06-01 10:01:17.000000 disksurf-1.2.3/disksurf.egg-info/SOURCES.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-06-01 10:01:17.000000 disksurf-1.2.3/disksurf.egg-info/dependency_links.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       57 2023-06-01 10:01:17.000000 disksurf-1.2.3/disksurf.egg-info/requires.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        9 2023-06-01 10:01:17.000000 disksurf-1.2.3/disksurf.egg-info/top_level.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-06-01 10:01:17.872182 disksurf-1.2.3/setup.cfg
--rw-r--r--   0 richardteague   (501) staff       (20)      842 2023-06-01 08:52:13.000000 disksurf-1.2.3/setup.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-07-11 15:06:57.958714 disksurf-1.2.4/
+-rw-r--r--   0 richardteague   (501) staff       (20)     1068 2023-03-27 18:30:47.000000 disksurf-1.2.4/LICENSE
+-rw-r--r--   0 richardteague   (501) staff       (20)     3728 2023-07-11 15:06:57.958613 disksurf-1.2.4/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)     3297 2023-03-27 18:30:47.000000 disksurf-1.2.4/README.md
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-07-11 15:06:57.957914 disksurf-1.2.4/disksurf/
+-rw-r--r--   0 richardteague   (501) staff       (20)      103 2023-03-27 18:30:47.000000 disksurf-1.2.4/disksurf/__init__.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    58429 2023-07-11 15:06:32.000000 disksurf-1.2.4/disksurf/observation.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    61353 2023-03-27 18:30:47.000000 disksurf-1.2.4/disksurf/surface.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-07-11 15:06:57.958477 disksurf-1.2.4/disksurf.egg-info/
+-rw-r--r--   0 richardteague   (501) staff       (20)     3728 2023-07-11 15:06:57.000000 disksurf-1.2.4/disksurf.egg-info/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)      250 2023-07-11 15:06:57.000000 disksurf-1.2.4/disksurf.egg-info/SOURCES.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-07-11 15:06:57.000000 disksurf-1.2.4/disksurf.egg-info/dependency_links.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       57 2023-07-11 15:06:57.000000 disksurf-1.2.4/disksurf.egg-info/requires.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        9 2023-07-11 15:06:57.000000 disksurf-1.2.4/disksurf.egg-info/top_level.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-07-11 15:06:57.958749 disksurf-1.2.4/setup.cfg
+-rw-r--r--   0 richardteague   (501) staff       (20)      842 2023-07-11 15:05:18.000000 disksurf-1.2.4/setup.py
```

### Comparing `disksurf-1.2.3/LICENSE` & `disksurf-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `disksurf-1.2.3/PKG-INFO` & `disksurf-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disksurf
-Version: 1.2.3
+Version: 1.2.4
 Summary: Infer and reproject a disk's 3D structure.
 Home-page: https://github.com/richteague/disksurf
 Author: Richard Teague
 Author-email: rteague@mit.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: disksurf Version: 1.2.3 Summary: Infer and
+Metadata-Version: 2.1 Name: disksurf Version: 1.2.4 Summary: Infer and
 reproject a disk's 3D structure. Home-page: https://github.com/richteague/
 disksurf Author: Richard Teague Author-email: rteague@mit.edu License: MIT
 Classifier: Programming Language :: Python :: 3.5 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # disksurf
                             [HD163296_zeroth.png]
                       [Documentation_Status] [DOI] [DOI]
```

### Comparing `disksurf-1.2.3/README.md` & `disksurf-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `disksurf-1.2.3/disksurf/observation.py` & `disksurf-1.2.4/disksurf/observation.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,14 +629,15 @@
             min_Inu = -1e10
         min_difference = -self.estimate_RMS()
 
         # Minimum distance between the peaks. 
 
         detect_peaks_kw = detect_peaks_kwargs or {}
         distance = detect_peaks_kw.pop('distance', 0.5 * self.bmaj / self.dpix)
+        distance = max(distance, 1.0)
 
         # Loop through each channel, then each vertical pixel column to extract
         # the peaks.
 
         _surface = []
         for c_idx in range(data.shape[0]):
 
@@ -673,16 +674,16 @@
                                                   distance=distance,
                                                   height=min_difference)
                         
                         # Fail if there are more than four peaks. 
 
                         if len(y_idx) != 4:
                             raise ValueError("More than four peaks detected.")
-
-                        y_idx = np.mean([y_idx[1:], y_idx[:-1]], axis=0)
+                        
+                        y_idx = np.nanmean([y_idx[1:], y_idx[:-1]], axis=0)
                         y_idx = y_idx.astype('int')[[0, -1]]
 
                     else:
                         y_idx, props = find_peaks(x=cut,
                                                   distance=distance,
                                                   height=min_Inu)
                         y_idx = y_idx[np.argsort(props['peak_heights'])]
```

### Comparing `disksurf-1.2.3/disksurf/surface.py` & `disksurf-1.2.4/disksurf/surface.py`

 * *Files identical despite different names*

### Comparing `disksurf-1.2.3/disksurf.egg-info/PKG-INFO` & `disksurf-1.2.4/disksurf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disksurf
-Version: 1.2.3
+Version: 1.2.4
 Summary: Infer and reproject a disk's 3D structure.
 Home-page: https://github.com/richteague/disksurf
 Author: Richard Teague
 Author-email: rteague@mit.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: disksurf Version: 1.2.3 Summary: Infer and
+Metadata-Version: 2.1 Name: disksurf Version: 1.2.4 Summary: Infer and
 reproject a disk's 3D structure. Home-page: https://github.com/richteague/
 disksurf Author: Richard Teague Author-email: rteague@mit.edu License: MIT
 Classifier: Programming Language :: Python :: 3.5 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # disksurf
                             [HD163296_zeroth.png]
                       [Documentation_Status] [DOI] [DOI]
```

### Comparing `disksurf-1.2.3/setup.py` & `disksurf-1.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="disksurf",
-    version="1.2.3",
+    version="1.2.4",
     author="Richard Teague",
     author_email="rteague@mit.edu",
     description=("Infer and reproject a disk's 3D structure."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/richteague/disksurf",
     packages=["disksurf"],
```

