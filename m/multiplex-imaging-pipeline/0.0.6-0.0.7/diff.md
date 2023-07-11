# Comparing `tmp/multiplex-imaging-pipeline-0.0.6.tar.gz` & `tmp/multiplex-imaging-pipeline-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multiplex-imaging-pipeline-0.0.6.tar", last modified: Tue Jul 11 14:14:45 2023, max compression
+gzip compressed data, was "dist/multiplex-imaging-pipeline-0.0.7.tar", last modified: Tue Jul 11 14:29:13 2023, max compression
```

## Comparing `multiplex-imaging-pipeline-0.0.6.tar` & `multiplex-imaging-pipeline-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:14:45.924450 multiplex-imaging-pipeline-0.0.6/
--rw-r--r--   0 estorrs   (1048) users      (100)     1068 2022-05-03 13:51:26.000000 multiplex-imaging-pipeline-0.0.6/LICENSE
--rw-r--r--   0 estorrs   (1048) users      (100)    11229 2023-07-11 14:14:45.922450 multiplex-imaging-pipeline-0.0.6/PKG-INFO
--rw-r--r--   0 estorrs   (1048) users      (100)    10542 2023-07-10 20:30:49.000000 multiplex-imaging-pipeline-0.0.6/README.md
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:14:45.909450 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/
--rw-r--r--   0 estorrs   (1048) users      (100)        0 2022-05-03 13:56:19.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/__init__.py
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:14:45.920450 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/compute1/
--rw-r--r--   0 estorrs   (1048) users      (100)        0 2023-07-10 19:12:30.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/compute1/__init__.py
--rw-r--r--   0 estorrs   (1048) users      (100)     4886 2023-07-10 19:24:58.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/compute1/generate_run_commands.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10712 2023-07-11 14:12:29.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py
--rw-r--r--   0 estorrs   (1048) users      (100)    12125 2023-07-10 18:24:27.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/ome.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10506 2023-07-11 13:24:23.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/region_features.py
--rw-r--r--   0 estorrs   (1048) users      (100)     5319 2023-06-29 15:42:55.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/segmentation.py
--rw-r--r--   0 estorrs   (1048) users      (100)     8976 2023-07-10 18:14:03.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/spatial_features.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10291 2023-07-07 14:20:21.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/utils.py
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:14:45.917450 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline.egg-info/
--rw-r--r--   0 estorrs   (1048) users      (100)    11229 2023-07-11 14:14:45.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 estorrs   (1048) users      (100)      739 2023-07-11 14:14:45.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 estorrs   (1048) users      (100)        1 2023-07-11 14:14:45.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       83 2023-07-11 14:14:45.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 estorrs   (1048) users      (100)      164 2023-07-11 14:14:45.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline.egg-info/requires.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       27 2023-07-11 14:14:45.000000 multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline.egg-info/top_level.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       38 2023-07-11 14:14:45.924450 multiplex-imaging-pipeline-0.0.6/setup.cfg
--rw-r--r--   0 estorrs   (1048) users      (100)     1705 2023-07-11 14:14:35.000000 multiplex-imaging-pipeline-0.0.6/setup.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:29:13.038886 multiplex-imaging-pipeline-0.0.7/
+-rw-r--r--   0 estorrs   (1048) users      (100)     1068 2022-05-03 13:51:26.000000 multiplex-imaging-pipeline-0.0.7/LICENSE
+-rw-r--r--   0 estorrs   (1048) users      (100)    11229 2023-07-11 14:29:13.037886 multiplex-imaging-pipeline-0.0.7/PKG-INFO
+-rw-r--r--   0 estorrs   (1048) users      (100)    10542 2023-07-10 20:30:49.000000 multiplex-imaging-pipeline-0.0.7/README.md
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:29:13.025886 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/
+-rw-r--r--   0 estorrs   (1048) users      (100)        0 2022-05-03 13:56:19.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/__init__.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:29:13.036886 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/compute1/
+-rw-r--r--   0 estorrs   (1048) users      (100)        0 2023-07-10 19:12:30.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/compute1/__init__.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     4886 2023-07-10 19:24:58.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/compute1/generate_run_commands.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10739 2023-07-11 14:28:47.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    12125 2023-07-10 18:24:27.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/ome.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10506 2023-07-11 13:24:23.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/region_features.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     5319 2023-06-29 15:42:55.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/segmentation.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     8976 2023-07-10 18:14:03.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/spatial_features.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10291 2023-07-07 14:20:21.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/utils.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:29:13.033886 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/
+-rw-r--r--   0 estorrs   (1048) users      (100)    11229 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 estorrs   (1048) users      (100)      739 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)        1 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       83 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)      164 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/requires.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       27 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       38 2023-07-11 14:29:13.038886 multiplex-imaging-pipeline-0.0.7/setup.cfg
+-rw-r--r--   0 estorrs   (1048) users      (100)     1705 2023-07-11 14:29:04.000000 multiplex-imaging-pipeline-0.0.7/setup.py
```

### Comparing `multiplex-imaging-pipeline-0.0.6/LICENSE` & `multiplex-imaging-pipeline-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.6/PKG-INFO` & `multiplex-imaging-pipeline-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplex-imaging-pipeline
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for multiplex imaging analysis
 Home-page: https://github.com/estorrs/multiplex-imaging-analysis
 Author: Erik Storrs
 Author-email: estorrs@wustl.edu
 Keywords: multiplex imaging codex neighborhood analysis image segmentation visualization mibi codex phenocycler mihc hyperion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `multiplex-imaging-pipeline-0.0.6/README.md` & `multiplex-imaging-pipeline-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/compute1/generate_run_commands.py` & `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/compute1/generate_run_commands.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py` & `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 ##############
 ## make-ome ##
 ##############
 parser.add_argument('--input-tif', type=str,
     help='Used in make-ome mode. Either directory of stitched tif files that will be combined into a single ome.tiff file, a multichannel .tif (for original codex platform), or a .qptiff (phenocycler platform).')
 
-parser.add_argument('--output-filepath', type=str,
+parser.add_argument('--output-filepath', type=str, default='output.ome.tiff',
     help='Location to write ome.tiff file')
 
 parser.add_argument('--platform', type=str,
     choices=['codex', 'phenocycler', 'raw'], default='phenocycler',
     help='Which platform produced the input images. phenocycler assumes a .qptiff from the akoya phenocycler platform. codex assumes a multichannel .tif output by the original akoya codex platform. raw will save a directory of .tifs together into a multiplex image.')
 
 parser.add_argument('--bbox', type=str,
```

### Comparing `multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/ome.py` & `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/ome.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/region_features.py` & `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/region_features.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/segmentation.py` & `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/segmentation.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/spatial_features.py` & `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/spatial_features.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline/utils.py` & `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline.egg-info/PKG-INFO` & `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplex-imaging-pipeline
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for multiplex imaging analysis
 Home-page: https://github.com/estorrs/multiplex-imaging-analysis
 Author: Erik Storrs
 Author-email: estorrs@wustl.edu
 Keywords: multiplex imaging codex neighborhood analysis image segmentation visualization mibi codex phenocycler mihc hyperion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `multiplex-imaging-pipeline-0.0.6/multiplex_imaging_pipeline.egg-info/SOURCES.txt` & `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.6/setup.py` & `multiplex-imaging-pipeline-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     # $ pip install multiplex-imaging-pipeline
     name='multiplex-imaging-pipeline',
-    version='0.0.6',
+    version='0.0.7',
     description='A Python library for multiplex imaging analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/estorrs/multiplex-imaging-analysis',
     author='Erik Storrs',
     author_email='estorrs@wustl.edu',
     classifiers=[
```

