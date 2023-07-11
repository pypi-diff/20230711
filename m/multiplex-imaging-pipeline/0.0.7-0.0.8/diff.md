# Comparing `tmp/multiplex-imaging-pipeline-0.0.7.tar.gz` & `tmp/multiplex-imaging-pipeline-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multiplex-imaging-pipeline-0.0.7.tar", last modified: Tue Jul 11 14:29:13 2023, max compression
+gzip compressed data, was "dist/multiplex-imaging-pipeline-0.0.8.tar", last modified: Tue Jul 11 16:59:28 2023, max compression
```

## Comparing `multiplex-imaging-pipeline-0.0.7.tar` & `multiplex-imaging-pipeline-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:29:13.038886 multiplex-imaging-pipeline-0.0.7/
--rw-r--r--   0 estorrs   (1048) users      (100)     1068 2022-05-03 13:51:26.000000 multiplex-imaging-pipeline-0.0.7/LICENSE
--rw-r--r--   0 estorrs   (1048) users      (100)    11229 2023-07-11 14:29:13.037886 multiplex-imaging-pipeline-0.0.7/PKG-INFO
--rw-r--r--   0 estorrs   (1048) users      (100)    10542 2023-07-10 20:30:49.000000 multiplex-imaging-pipeline-0.0.7/README.md
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:29:13.025886 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/
--rw-r--r--   0 estorrs   (1048) users      (100)        0 2022-05-03 13:56:19.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/__init__.py
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:29:13.036886 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/compute1/
--rw-r--r--   0 estorrs   (1048) users      (100)        0 2023-07-10 19:12:30.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/compute1/__init__.py
--rw-r--r--   0 estorrs   (1048) users      (100)     4886 2023-07-10 19:24:58.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/compute1/generate_run_commands.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10739 2023-07-11 14:28:47.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py
--rw-r--r--   0 estorrs   (1048) users      (100)    12125 2023-07-10 18:24:27.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/ome.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10506 2023-07-11 13:24:23.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/region_features.py
--rw-r--r--   0 estorrs   (1048) users      (100)     5319 2023-06-29 15:42:55.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/segmentation.py
--rw-r--r--   0 estorrs   (1048) users      (100)     8976 2023-07-10 18:14:03.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/spatial_features.py
--rw-r--r--   0 estorrs   (1048) users      (100)    10291 2023-07-07 14:20:21.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/utils.py
-drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 14:29:13.033886 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/
--rw-r--r--   0 estorrs   (1048) users      (100)    11229 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 estorrs   (1048) users      (100)      739 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 estorrs   (1048) users      (100)        1 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       83 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 estorrs   (1048) users      (100)      164 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/requires.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       27 2023-07-11 14:29:12.000000 multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/top_level.txt
--rw-r--r--   0 estorrs   (1048) users      (100)       38 2023-07-11 14:29:13.038886 multiplex-imaging-pipeline-0.0.7/setup.cfg
--rw-r--r--   0 estorrs   (1048) users      (100)     1705 2023-07-11 14:29:04.000000 multiplex-imaging-pipeline-0.0.7/setup.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 16:59:28.194263 multiplex-imaging-pipeline-0.0.8/
+-rw-r--r--   0 estorrs   (1048) users      (100)     1068 2022-05-03 13:51:26.000000 multiplex-imaging-pipeline-0.0.8/LICENSE
+-rw-r--r--   0 estorrs   (1048) users      (100)    12238 2023-07-11 16:59:28.193263 multiplex-imaging-pipeline-0.0.8/PKG-INFO
+-rw-r--r--   0 estorrs   (1048) users      (100)    11551 2023-07-11 14:29:34.000000 multiplex-imaging-pipeline-0.0.8/README.md
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 16:59:28.179263 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/
+-rw-r--r--   0 estorrs   (1048) users      (100)        0 2022-05-03 13:56:19.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/__init__.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 16:59:28.192263 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/compute1/
+-rw-r--r--   0 estorrs   (1048) users      (100)        0 2023-07-10 19:12:30.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/compute1/__init__.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     4886 2023-07-10 19:24:58.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/compute1/generate_run_commands.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10739 2023-07-11 14:28:47.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    12125 2023-07-10 18:24:27.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/ome.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10679 2023-07-11 14:34:02.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/region_features.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     5319 2023-06-29 15:42:55.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/segmentation.py
+-rw-r--r--   0 estorrs   (1048) users      (100)     8976 2023-07-10 18:14:03.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/spatial_features.py
+-rw-r--r--   0 estorrs   (1048) users      (100)    10291 2023-07-07 14:20:21.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/utils.py
+drwxr-xr-x   0 estorrs   (1048) users      (100)        0 2023-07-11 16:59:28.189263 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline.egg-info/
+-rw-r--r--   0 estorrs   (1048) users      (100)    12238 2023-07-11 16:59:28.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 estorrs   (1048) users      (100)      739 2023-07-11 16:59:28.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)        1 2023-07-11 16:59:28.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       83 2023-07-11 16:59:28.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)      164 2023-07-11 16:59:28.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline.egg-info/requires.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       27 2023-07-11 16:59:28.000000 multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 estorrs   (1048) users      (100)       38 2023-07-11 16:59:28.194263 multiplex-imaging-pipeline-0.0.8/setup.cfg
+-rw-r--r--   0 estorrs   (1048) users      (100)     1705 2023-07-11 16:58:29.000000 multiplex-imaging-pipeline-0.0.8/setup.py
```

### Comparing `multiplex-imaging-pipeline-0.0.7/LICENSE` & `multiplex-imaging-pipeline-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.7/PKG-INFO` & `multiplex-imaging-pipeline-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplex-imaging-pipeline
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for multiplex imaging analysis
 Home-page: https://github.com/estorrs/multiplex-imaging-analysis
 Author: Erik Storrs
 Author-email: estorrs@wustl.edu
 Keywords: multiplex imaging codex neighborhood analysis image segmentation visualization mibi codex phenocycler mihc hyperion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -20,28 +20,38 @@
 A pipeline for multiplex imaging analysis.
 
 Under active development
 
 
 ## Installation
 
+Basic installation (will run all modes except `segment-ome`).
+
 ```bash
 pip install multiplex-imaging-pipeline
 ```
 
+To preform segmentation, [deepcell](https://github.com/vanvalenlab/deepcell-tf) dependencies need to be installed via the command below. If you need to run segmentation we **highly** suggest installing into a fresh virtual environment. Installing deepcell tends to throw errors on a lot of machines, if this is the case for you we provide a [docker](https://github.com/estorrs/multiplex-imaging-pipeline/tree/main#docker) image that can run all `multiplex-imaging-pipeline` functionality. 
+
+```bash
+pip install multiplex-imaging-pipeline[segmentation]
+```
+
 ## Usage
 
 ### ome.tiff generation
 
 ome.tiff files can be created with the `make-ome` command.
 
 ```bash
 mip make-ome --input-tif INPUT_TIF --platform PLATFORM --bbox BBOX --output-filepath OUTPUT_FILEPATH
 ```
 
+See --input-tif and --platform for details on what types of input formats are expected.
+
 #### Arguments
 + --input-tif
   + Input tif or directory of tifs to be converted into HTAN compatible ome.tiff format. If --platform is "phenocycler", then a file with a .qptiff extension output by the phenocycler platform is expected. If --platform is "codex", then a multichannel imagej .tif output by the first-generation codex machine is expected. If --platform is "raw" then a directory of tifs is expected, where the images will be combined into a multichannel .ome.tiff and the channel names will be named based on the files (for example if one of the files is named protein1.tif, then that channel in the ome.tiff will be named protein1).
 
 + --platform
   + Can be one of ["phenocycler", "codex", "raw"]. For Akoya images, use "phenocycler" for their new platform (.qptiff file extension), and use "codex" for the first-generation machine (multichannel imagej .tif file). To convert a directory of single channel .tif files into a multichannel ome.tiff, use "raw". See --input-tif for more details. Default is "phenocycler".
 
@@ -203,16 +213,22 @@
 
 ## Docker
 
 ```bash
 docker pull estorrs/multiplex-imaging-pipeline:0.0.1
 ```
 
-Example of ome.tiff generation with docker.
+Note that you'll need to map input and output data folders with the -v flag when running the docker container.
 
-Note that you'll need to map input and output data folders with the -v flag.
+###### Example of ome.tiff generation with docker.
 
 ```bash
 docker run -v /path/to/input/dir:/inputs -v /path/to/output/dir:/outputs estorrs/multiplex-imaging-pipeline:0.0.1 mip make-ome --input-tif /inputs/file.qptiff --platform phenocycler --output-filepath /outputs/output.ome.tiff
 ```
 
+###### Example of ome.tiff cell segmentation with docker.
+
+```bash
+docker run -v /path/to/input/dir:/inputs -v /path/to/output/dir:/outputs estorrs/multiplex-imaging-pipeline:0.0.1 mip segment-ome --input-tif /inputs/file.ome.tiff --output-prefix output
+```
+
```

### Comparing `multiplex-imaging-pipeline-0.0.7/README.md` & `multiplex-imaging-pipeline-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,38 @@
 A pipeline for multiplex imaging analysis.
 
 Under active development
 
 
 ## Installation
 
+Basic installation (will run all modes except `segment-ome`).
+
 ```bash
 pip install multiplex-imaging-pipeline
 ```
 
+To preform segmentation, [deepcell](https://github.com/vanvalenlab/deepcell-tf) dependencies need to be installed via the command below. If you need to run segmentation we **highly** suggest installing into a fresh virtual environment. Installing deepcell tends to throw errors on a lot of machines, if this is the case for you we provide a [docker](https://github.com/estorrs/multiplex-imaging-pipeline/tree/main#docker) image that can run all `multiplex-imaging-pipeline` functionality. 
+
+```bash
+pip install multiplex-imaging-pipeline[segmentation]
+```
+
 ## Usage
 
 ### ome.tiff generation
 
 ome.tiff files can be created with the `make-ome` command.
 
 ```bash
 mip make-ome --input-tif INPUT_TIF --platform PLATFORM --bbox BBOX --output-filepath OUTPUT_FILEPATH
 ```
 
+See --input-tif and --platform for details on what types of input formats are expected.
+
 #### Arguments
 + --input-tif
   + Input tif or directory of tifs to be converted into HTAN compatible ome.tiff format. If --platform is "phenocycler", then a file with a .qptiff extension output by the phenocycler platform is expected. If --platform is "codex", then a multichannel imagej .tif output by the first-generation codex machine is expected. If --platform is "raw" then a directory of tifs is expected, where the images will be combined into a multichannel .ome.tiff and the channel names will be named based on the files (for example if one of the files is named protein1.tif, then that channel in the ome.tiff will be named protein1).
 
 + --platform
   + Can be one of ["phenocycler", "codex", "raw"]. For Akoya images, use "phenocycler" for their new platform (.qptiff file extension), and use "codex" for the first-generation machine (multichannel imagej .tif file). To convert a directory of single channel .tif files into a multichannel ome.tiff, use "raw". See --input-tif for more details. Default is "phenocycler".
 
@@ -186,16 +196,22 @@
 
 ## Docker
 
 ```bash
 docker pull estorrs/multiplex-imaging-pipeline:0.0.1
 ```
 
-Example of ome.tiff generation with docker.
+Note that you'll need to map input and output data folders with the -v flag when running the docker container.
 
-Note that you'll need to map input and output data folders with the -v flag.
+###### Example of ome.tiff generation with docker.
 
 ```bash
 docker run -v /path/to/input/dir:/inputs -v /path/to/output/dir:/outputs estorrs/multiplex-imaging-pipeline:0.0.1 mip make-ome --input-tif /inputs/file.qptiff --platform phenocycler --output-filepath /outputs/output.ome.tiff
 ```
 
+###### Example of ome.tiff cell segmentation with docker.
+
+```bash
+docker run -v /path/to/input/dir:/inputs -v /path/to/output/dir:/outputs estorrs/multiplex-imaging-pipeline:0.0.1 mip segment-ome --input-tif /inputs/file.ome.tiff --output-prefix output
+```
+
```

### Comparing `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/compute1/generate_run_commands.py` & `multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/compute1/generate_run_commands.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py` & `multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/multiplex_imaging_pipeline.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/ome.py` & `multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/ome.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/region_features.py` & `multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/region_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,18 +118,21 @@
             data.append([counts.get(cat, 0) / f.shape[0] for cat in pool])
         else:
             data.append([np.nan] * len(pool))
     df = pd.DataFrame(data=data, columns=pool, index=list(range(1, labeled.max() + 1, 1)))
     return df
         
 
-def calculate_marker_intensities(channel_to_img, labeled):
+def calculate_marker_intensities(channel_to_img, labeled, scale=False):
     data, labels = [], []
     channels = sorted(set(channel_to_img.keys()))
-    stacked = np.concatenate([np.expand_dims(channel_to_img[c], -1) for c in channels], axis=-1)
+    if scale:
+        stacked = np.concatenate([np.expand_dims(channel_to_img[c] / channel_to_img[c].std(), -1) for c in channels], axis=-1)
+    else:
+        stacked = np.concatenate([np.expand_dims(channel_to_img[c], -1) for c in channels], axis=-1)
     props = regionprops(labeled, intensity_image=stacked)
     for prop in props:
         labels.append(prop.label)
         data.append(prop.intensity_mean.tolist())
    
     df = pd.DataFrame(data=data, columns=channels, index=labels)
     return df
@@ -225,15 +228,15 @@
 
         logging.info(f'generating marker intensities')
         df_marker_intensities = calculate_marker_intensities(channel_to_img, img)
         df_marker_intensities.columns = [f'marker_intensity_{c}'
                                          for c in df_marker_intensities.columns]
         
         logging.info(f'generating marker intensities scaled')
-        df_marker_intensities_scaled = calculate_marker_intensities(channel_to_img_scaled, img)
+        df_marker_intensities_scaled = calculate_marker_intensities(channel_to_img, img, scale=True)
         df_marker_intensities_scaled.columns = [f'marker_intensity_scaled_{c}'
                                          for c in df_marker_intensities_scaled.columns]
 
         combined = pd.merge(
             df_meta, df_fracs, left_index=True, right_index=True, how='left')
         combined = pd.merge(
             combined, df_marker_intensities, left_index=True, right_index=True, how='left')
```

### Comparing `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/segmentation.py` & `multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/segmentation.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/spatial_features.py` & `multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/spatial_features.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline/utils.py` & `multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/PKG-INFO` & `multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiplex-imaging-pipeline
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for multiplex imaging analysis
 Home-page: https://github.com/estorrs/multiplex-imaging-analysis
 Author: Erik Storrs
 Author-email: estorrs@wustl.edu
 Keywords: multiplex imaging codex neighborhood analysis image segmentation visualization mibi codex phenocycler mihc hyperion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -20,28 +20,38 @@
 A pipeline for multiplex imaging analysis.
 
 Under active development
 
 
 ## Installation
 
+Basic installation (will run all modes except `segment-ome`).
+
 ```bash
 pip install multiplex-imaging-pipeline
 ```
 
+To preform segmentation, [deepcell](https://github.com/vanvalenlab/deepcell-tf) dependencies need to be installed via the command below. If you need to run segmentation we **highly** suggest installing into a fresh virtual environment. Installing deepcell tends to throw errors on a lot of machines, if this is the case for you we provide a [docker](https://github.com/estorrs/multiplex-imaging-pipeline/tree/main#docker) image that can run all `multiplex-imaging-pipeline` functionality. 
+
+```bash
+pip install multiplex-imaging-pipeline[segmentation]
+```
+
 ## Usage
 
 ### ome.tiff generation
 
 ome.tiff files can be created with the `make-ome` command.
 
 ```bash
 mip make-ome --input-tif INPUT_TIF --platform PLATFORM --bbox BBOX --output-filepath OUTPUT_FILEPATH
 ```
 
+See --input-tif and --platform for details on what types of input formats are expected.
+
 #### Arguments
 + --input-tif
   + Input tif or directory of tifs to be converted into HTAN compatible ome.tiff format. If --platform is "phenocycler", then a file with a .qptiff extension output by the phenocycler platform is expected. If --platform is "codex", then a multichannel imagej .tif output by the first-generation codex machine is expected. If --platform is "raw" then a directory of tifs is expected, where the images will be combined into a multichannel .ome.tiff and the channel names will be named based on the files (for example if one of the files is named protein1.tif, then that channel in the ome.tiff will be named protein1).
 
 + --platform
   + Can be one of ["phenocycler", "codex", "raw"]. For Akoya images, use "phenocycler" for their new platform (.qptiff file extension), and use "codex" for the first-generation machine (multichannel imagej .tif file). To convert a directory of single channel .tif files into a multichannel ome.tiff, use "raw". See --input-tif for more details. Default is "phenocycler".
 
@@ -203,16 +213,22 @@
 
 ## Docker
 
 ```bash
 docker pull estorrs/multiplex-imaging-pipeline:0.0.1
 ```
 
-Example of ome.tiff generation with docker.
+Note that you'll need to map input and output data folders with the -v flag when running the docker container.
 
-Note that you'll need to map input and output data folders with the -v flag.
+###### Example of ome.tiff generation with docker.
 
 ```bash
 docker run -v /path/to/input/dir:/inputs -v /path/to/output/dir:/outputs estorrs/multiplex-imaging-pipeline:0.0.1 mip make-ome --input-tif /inputs/file.qptiff --platform phenocycler --output-filepath /outputs/output.ome.tiff
 ```
 
+###### Example of ome.tiff cell segmentation with docker.
+
+```bash
+docker run -v /path/to/input/dir:/inputs -v /path/to/output/dir:/outputs estorrs/multiplex-imaging-pipeline:0.0.1 mip segment-ome --input-tif /inputs/file.ome.tiff --output-prefix output
+```
+
```

### Comparing `multiplex-imaging-pipeline-0.0.7/multiplex_imaging_pipeline.egg-info/SOURCES.txt` & `multiplex-imaging-pipeline-0.0.8/multiplex_imaging_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiplex-imaging-pipeline-0.0.7/setup.py` & `multiplex-imaging-pipeline-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     # $ pip install multiplex-imaging-pipeline
     name='multiplex-imaging-pipeline',
-    version='0.0.7',
+    version='0.0.8',
     description='A Python library for multiplex imaging analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/estorrs/multiplex-imaging-analysis',
     author='Erik Storrs',
     author_email='estorrs@wustl.edu',
     classifiers=[
```

