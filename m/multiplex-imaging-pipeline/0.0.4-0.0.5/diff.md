# Comparing `tmp/multiplex-imaging-pipeline-0.0.4.tar.gz` & `tmp/multiplex-imaging-pipeline-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multiplex-imaging-pipeline-0.0.4.tar", last modified: Mon Jul 10 21:39:27 2023, max compression
+gzip compressed data, was "dist/multiplex-imaging-pipeline-0.0.5.tar", last modified: Tue Jul 11 13:48:19 2023, max compression
```

## Comparing `multiplex-imaging-pipeline-0.0.4.tar` & `multiplex-imaging-pipeline-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:39:27.009103 multiplex-imaging-pipeline-0.0.4/
--rw-r--r--   0 estorrs   (1048) users      (100)     1068 2022-05-03 13:51:26.000000 multiplex-imaging-pipeline-0.0.4/LICENSE
--rw-r--r--   0 estorrs   (1048) users      (100)    11200 2023-07-10 21:39:27.008103 multiplex-imaging-pipeline-0.0.4/PKG-INFO
--rw-r--r--   0 estorrs   (1048) users      (100)    10542 2023-07-10 20:30:49.000000 multiplex-imaging-pipeline-0.0.4/README.md
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:39:26.998103 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/
--rw-r--r--   0 estorrs   (1048) users      (100)        0 2022-05-03 13:56:19.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/__init__.py
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:39:27.007103 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/compute1/
--rw-r--r--   0 estorrs   (1048) users      (100)        0 2023-07-10 19:12:30.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/compute1/__init__.py
--rw-r--r--   0 estorrs   (1048) users      (100)     4886 2023-07-10 19:24:58.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/compute1/generate_run_commands.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10432 2023-07-07 15:00:12.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py
--rw-r--r--   0 estorrs   (1048) users      (100)    12125 2023-07-10 18:24:27.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/ome.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10283 2023-07-10 18:57:35.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/region_features.py
--rw-r--r--   0 estorrs   (1048) users      (100)     5319 2023-06-29 15:42:55.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/segmentation.py
--rw-r--r--   0 estorrs   (1048) users      (100)     8976 2023-07-10 18:14:03.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/spatial_features.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10291 2023-07-07 14:20:21.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/utils.py
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-10 21:39:27.005103 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/
--rw-r--r--   0 estorrs   (1048) users      (100)    11200 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 estorrs   (1048) users      (100)      739 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 estorrs   (1048) users      (100)        1 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       83 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 estorrs   (1048) users      (100)      148 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/requires.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       27 2023-07-10 21:39:26.000000 multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/top_level.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       38 2023-07-10 21:39:27.009103 multiplex-imaging-pipeline-0.0.4/setup.cfg
--rw-r--r--   0 estorrs   (1048) users      (100)     1637 2023-07-10 21:39:15.000000 multiplex-imaging-pipeline-0.0.4/setup.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 13:48:19.720121 multiplex-imaging-pipeline-0.0.5/
+-rw-r--r--   0 estorrs   (1048) users      (100)     1068 2022-05-03 13:51:26.000000 multiplex-imaging-pipeline-0.0.5/LICENSE
+-rw-r--r--   0 estorrs   (1048) users      (100)    11229 2023-07-11 13:48:19.719122 multiplex-imaging-pipeline-0.0.5/PKG-INFO
+-rw-r--r--   0 estorrs   (1048) users      (100)    10542 2023-07-10 20:30:49.000000 multiplex-imaging-pipeline-0.0.5/README.md
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 13:48:19.702121 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/
+-rw-r--r--   0 estorrs   (1048) users      (100)        0 2022-05-03 13:56:19.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/__init__.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 13:48:19.716122 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/compute1/
+-rw-r--r--   0 estorrs   (1048) users      (100)        0 2023-07-10 19:12:30.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/compute1/__init__.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     4886 2023-07-10 19:24:58.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/compute1/generate_run_commands.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10432 2023-07-07 15:00:12.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    12125 2023-07-10 18:24:27.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/ome.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10506 2023-07-11 13:24:23.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/region_features.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     5319 2023-06-29 15:42:55.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/segmentation.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     8976 2023-07-10 18:14:03.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/spatial_features.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10291 2023-07-07 14:20:21.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/utils.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 13:48:19.713122 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline.egg-info/
+-rw-r--r--   0 estorrs   (1048) users      (100)    11229 2023-07-11 13:48:18.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 estorrs   (1048) users      (100)      739 2023-07-11 13:48:18.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)        1 2023-07-11 13:48:18.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       83 2023-07-11 13:48:18.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)      164 2023-07-11 13:48:18.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline.egg-info/requires.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       27 2023-07-11 13:48:18.000000 multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       38 2023-07-11 13:48:19.721121 multiplex-imaging-pipeline-0.0.5/setup.cfg
+-rw-r--r--   0 estorrs   (1048) users      (100)     1705 2023-07-11 13:47:18.000000 multiplex-imaging-pipeline-0.0.5/setup.py
```

### Comparing `multiplex-imaging-pipeline-0.0.4/LICENSE` & `multiplex-imaging-pipeline-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.4/PKG-INFO` & `multiplex-imaging-pipeline-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: multiplex-imaging-pipeline
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for multiplex imaging analysis
 Home-page: https://github.com/estorrs/multiplex-imaging-analysis
 Author: Erik Storrs
 Author-email: estorrs@wustl.edu
 Keywords: multiplex imaging codex neighborhood analysis image segmentation visualization mibi codex phenocycler mihc hyperion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: segmentation
 License-File: LICENSE
 
 # multiplex-imaging-pipeline
 
 A pipeline for multiplex imaging analysis.
 
 Under active development
```

### Comparing `multiplex-imaging-pipeline-0.0.4/README.md` & `multiplex-imaging-pipeline-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/compute1/generate_run_commands.py` & `multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/compute1/generate_run_commands.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py` & `multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/ome.py` & `multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/ome.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/region_features.py` & `multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/region_features.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
 def get_region_features(
         adata_fp, ome_fp, mask_fp=None,
         mask_markers=None, min_area=10000, sigma=1., default_threshold=2.):
     a = sc.read_h5ad(adata_fp)
     channel_to_img = utils.extract_ome_tiff(ome_fp)
     channel_to_img = {utils.R_CHANNEL_MAPPING.get(k, k):v for k, v in channel_to_img.items()}
-    channel_to_img_scaled = {c:img / img.std() for c, img in channel_to_img.items()}
+    # channel_to_img_scaled = {c:img / img.std() for c, img in channel_to_img.items()}
 
     if mask_fp is not None:
         mask = tifffile.imread(mask_fp)
     else:
         logging.info(f'no mask detected, generating mask from {mask_markers}')
         channels = [c.replace('_fraction', '') for c in a.var.index.to_list()]
         channel_to_thresh = {c:thresh for c, thresh in zip(channels, a.uns['thresholds'])
@@ -215,32 +215,36 @@
     labeled_dict, _ = get_morphology_masks(labeled)
 
     type_to_table = {}
     for k, img in labeled_dict.items():
         logging.info(f'generating region features for {k}')
         df_meta = get_regionprops_df(img)
 
+        logging.info(f'generating cell fractions')
         df_fracs = calculate_annotation_fractions(a, img, 'cell_type')
         df_fracs.columns = [f'cell_type_fraction_{c}' for c in df_fracs.columns]
 
+        logging.info(f'generating marker intensities')
         df_marker_intensities = calculate_marker_intensities(channel_to_img, img)
         df_marker_intensities.columns = [f'marker_intensity_{c}'
                                          for c in df_marker_intensities.columns]
         
+        logging.info(f'generating marker intensities scaled')
         df_marker_intensities_scaled = calculate_marker_intensities(channel_to_img_scaled, img)
         df_marker_intensities_scaled.columns = [f'marker_intensity_scaled_{c}'
                                          for c in df_marker_intensities_scaled.columns]
 
         combined = pd.merge(
             df_meta, df_fracs, left_index=True, right_index=True, how='left')
         combined = pd.merge(
             combined, df_marker_intensities, left_index=True, right_index=True, how='left')
         combined = pd.merge(
             combined, df_marker_intensities_scaled, left_index=True, right_index=True, how='left')
         
+        logging.info(f'generating marker fractions')
         if 'thresholds' in a.uns and a.uns['thresholds'] is not None:
             df_marker_fracs = calculate_marker_fractions(channel_to_img, a, img)
             df_marker_fracs.columns = [f'marker_fraction_{c}'
                                     for c in df_marker_fracs.columns]
             combined = pd.merge(
                 combined, df_marker_fracs, left_index=True, right_index=True, how='left')
```

### Comparing `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/segmentation.py` & `multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/segmentation.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/spatial_features.py` & `multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/spatial_features.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline/utils.py` & `multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/PKG-INFO` & `multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: multiplex-imaging-pipeline
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for multiplex imaging analysis
 Home-page: https://github.com/estorrs/multiplex-imaging-analysis
 Author: Erik Storrs
 Author-email: estorrs@wustl.edu
 Keywords: multiplex imaging codex neighborhood analysis image segmentation visualization mibi codex phenocycler mihc hyperion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: segmentation
 License-File: LICENSE
 
 # multiplex-imaging-pipeline
 
 A pipeline for multiplex imaging analysis.
 
 Under active development
```

### Comparing `multiplex-imaging-pipeline-0.0.4/multiplex_imaging_pipeline.egg-info/SOURCES.txt` & `multiplex-imaging-pipeline-0.0.5/multiplex_imaging_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.4/setup.py` & `multiplex-imaging-pipeline-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     # $ pip install multiplex-imaging-pipeline
     name='multiplex-imaging-pipeline',
-    version='0.0.4',
+    version='0.0.5',
     description='A Python library for multiplex imaging analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/estorrs/multiplex-imaging-analysis',
     author='Erik Storrs',
     author_email='estorrs@wustl.edu',
     classifiers=[
@@ -39,16 +39,20 @@
         'tifffile',
         'ome-types',
         'scikit-image',
         'scikit-learn',
         'imagecodecs>=2022.7.27',
         'torch',
         'torchvision',
-        'deepcell',
     ],
+    extras_require={
+        'segmentation': [
+            'deepcell'
+        ],
+    },
     include_package_data=True,
 
     entry_points={
         'console_scripts': [
             'mip=multiplex_imaging_pipeline.multiplex_imaging_pipeline:main',
         ],
     },
```

