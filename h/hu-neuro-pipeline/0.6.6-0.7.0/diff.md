# Comparing `tmp/hu-neuro-pipeline-0.6.6.tar.gz` & `tmp/hu-neuro-pipeline-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hu-neuro-pipeline-0.6.6.tar", last modified: Fri Jun 23 09:05:02 2023, max compression
+gzip compressed data, was "hu-neuro-pipeline-0.7.0.tar", last modified: Tue Jul 11 19:48:47 2023, max compression
```

## Comparing `hu-neuro-pipeline-0.6.6.tar` & `hu-neuro-pipeline-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.919692 hu-neuro-pipeline-0.6.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.915692 hu-neuro-pipeline-0.6.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.915692 hu-neuro-pipeline-0.6.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/.github/workflows/build_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-23 09:05:02.919692 hu-neuro-pipeline-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.915692 hu-neuro-pipeline-0.6.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    46302 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/docs/flowchart.odp
--rw-r--r--   0 runner    (1001) docker     (123)    30937 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/docs/inputs.md
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/docs/outputs.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.915692 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.919692 hu-neuro-pipeline-0.6.6/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/pipeline/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/averaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/boilerplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.919692 hu-neuro-pipeline-0.6.6/pipeline/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/datasets/ucap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/epoching.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/perm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/tfr.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:05:02.919692 hu-neuro-pipeline-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:48:47.432382 hu-neuro-pipeline-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:48:47.416382 hu-neuro-pipeline-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:48:47.416382 hu-neuro-pipeline-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/.github/workflows/build_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-11 19:48:47.432382 hu-neuro-pipeline-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:48:47.420382 hu-neuro-pipeline-0.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:48:47.424382 hu-neuro-pipeline-0.7.0/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    39318 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33724 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/_static/flowchart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   193157 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:48:47.424382 hu-neuro-pipeline-0.7.0/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/examples/ucap.Rmd
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/processing_group.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/processing_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/processing_participant.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/processing_tfr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:48:47.428382 hu-neuro-pipeline-0.7.0/doc/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/tables/averaging.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/tables/epoching.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/tables/inputs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/tables/outputs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/tables/performance.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/tables/perm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/tables/preprocessing.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/tables/tfr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/usage_inputs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/usage_outputs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/doc/usage_quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:48:47.428382 hu-neuro-pipeline-0.7.0/hu_neuro_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-11 19:48:47.000000 hu-neuro-pipeline-0.7.0/hu_neuro_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-11 19:48:47.000000 hu-neuro-pipeline-0.7.0/hu_neuro_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:48:47.000000 hu-neuro-pipeline-0.7.0/hu_neuro_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 19:48:47.000000 hu-neuro-pipeline-0.7.0/hu_neuro_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 19:48:47.000000 hu-neuro-pipeline-0.7.0/hu_neuro_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:48:47.432382 hu-neuro-pipeline-0.7.0/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 19:48:47.000000 hu-neuro-pipeline-0.7.0/pipeline/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/averaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/boilerplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:48:47.432382 hu-neuro-pipeline-0.7.0/pipeline/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/datasets/ucap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/epoching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/perm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pipeline/tfr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:48:47.432382 hu-neuro-pipeline-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-11 19:48:37.000000 hu-neuro-pipeline-0.7.0/setup.py
```

### Comparing `hu-neuro-pipeline-0.6.6/.github/workflows/build_publish.yml` & `hu-neuro-pipeline-0.7.0/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/LICENSE` & `hu-neuro-pipeline-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/PKG-INFO` & `hu-neuro-pipeline-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: hu-neuro-pipeline
-Version: 0.6.6
+Version: 0.7.0
 Summary: Single trial EEG pipeline at the Abdel Rahman Lab for Neurocognitive Psychology, Humboldt-Universität zu Berlin
 Home-page: https://github.com/alexenge/hu-neuro-pipeline
 Author: Alexander Enge
 Author-email: alexander.enge@hu-berlin.de
 Project-URL: Issue trackers, https://github.com/alexenge/hu-neuro-pipeline/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hu-neuro-pipeline
@@ -62,21 +63,15 @@
 
 ```r
 reticulate::py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
 ```
 
 ## 2. Usage
 
-[Pipeline inputs](docs/inputs.md) & [outputs](docs/outputs.md)
-
-<img src="https://i.imgur.com/WSj9t4b.png" width="400">
-
-## 3. Examples
-
-### 3.1 For Python users
+### 2.1 For Python users
 
 Here is a fairly minimal example for a (fictional) N400/P600 experiment with two experimental factors: `semantics` (e.g., related versus unrelated words) and emotional `context` (e.g., emotionally negative versus neutral).
 
 ```python
 from pipeline import group_pipeline
 
 trials, evokeds, config = group_pipeline(
@@ -103,15 +98,15 @@
 
 * The fact that log files contain additional trials from a semantic `'filler'` condition (which we want to skip because they don't have corresponding EEG triggers)
 
 * The *a priori* defined time windows and regions of interest for the N400 and P600 `components`
 
 * The log file columns (`average_by`) for which we want to obtain by-participant averaged waveforms (i.e., for all main and interaction effects)
 
-### 3.2 For R users
+### 2.2 For R users
 
 Here is the same example as above but for using the pipeline from R:
 
 ```R
 # Import Python module
 pipeline <- reticulate::import("pipeline")
 
@@ -139,7 +134,13 @@
 )
 
 # Extract results
 trials <- res[[1]]
 evokeds <- res[[2]]
 config <- res[[3]]
 ```
+
+## 3. Processing details
+
+<img src="https://github.com/alexenge/hu-neuro-pipeline/blob/main/doc/_static/flowchart.svg" width="400">
+
+See the [documentation](https://hu-neuro-pipeline.readthedocs.io/en/latest/) for more details about how to use the pipeline and how it works under the hood.
```

### Comparing `hu-neuro-pipeline-0.6.6/README.md` & `hu-neuro-pipeline-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -45,21 +45,15 @@
 
 ```r
 reticulate::py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
 ```
 
 ## 2. Usage
 
-[Pipeline inputs](docs/inputs.md) & [outputs](docs/outputs.md)
-
-<img src="https://i.imgur.com/WSj9t4b.png" width="400">
-
-## 3. Examples
-
-### 3.1 For Python users
+### 2.1 For Python users
 
 Here is a fairly minimal example for a (fictional) N400/P600 experiment with two experimental factors: `semantics` (e.g., related versus unrelated words) and emotional `context` (e.g., emotionally negative versus neutral).
 
 ```python
 from pipeline import group_pipeline
 
 trials, evokeds, config = group_pipeline(
@@ -86,15 +80,15 @@
 
 * The fact that log files contain additional trials from a semantic `'filler'` condition (which we want to skip because they don't have corresponding EEG triggers)
 
 * The *a priori* defined time windows and regions of interest for the N400 and P600 `components`
 
 * The log file columns (`average_by`) for which we want to obtain by-participant averaged waveforms (i.e., for all main and interaction effects)
 
-### 3.2 For R users
+### 2.2 For R users
 
 Here is the same example as above but for using the pipeline from R:
 
 ```R
 # Import Python module
 pipeline <- reticulate::import("pipeline")
 
@@ -122,7 +116,13 @@
 )
 
 # Extract results
 trials <- res[[1]]
 evokeds <- res[[2]]
 config <- res[[3]]
 ```
+
+## 3. Processing details
+
+<img src="https://github.com/alexenge/hu-neuro-pipeline/blob/main/doc/_static/flowchart.svg" width="400">
+
+See the [documentation](https://hu-neuro-pipeline.readthedocs.io/en/latest/) for more details about how to use the pipeline and how it works under the hood.
```

### Comparing `hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/PKG-INFO` & `hu-neuro-pipeline-0.7.0/hu_neuro_pipeline.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: hu-neuro-pipeline
-Version: 0.6.6
+Version: 0.7.0
 Summary: Single trial EEG pipeline at the Abdel Rahman Lab for Neurocognitive Psychology, Humboldt-Universität zu Berlin
 Home-page: https://github.com/alexenge/hu-neuro-pipeline
 Author: Alexander Enge
 Author-email: alexander.enge@hu-berlin.de
 Project-URL: Issue trackers, https://github.com/alexenge/hu-neuro-pipeline/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hu-neuro-pipeline
@@ -62,21 +63,15 @@
 
 ```r
 reticulate::py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
 ```
 
 ## 2. Usage
 
-[Pipeline inputs](docs/inputs.md) & [outputs](docs/outputs.md)
-
-<img src="https://i.imgur.com/WSj9t4b.png" width="400">
-
-## 3. Examples
-
-### 3.1 For Python users
+### 2.1 For Python users
 
 Here is a fairly minimal example for a (fictional) N400/P600 experiment with two experimental factors: `semantics` (e.g., related versus unrelated words) and emotional `context` (e.g., emotionally negative versus neutral).
 
 ```python
 from pipeline import group_pipeline
 
 trials, evokeds, config = group_pipeline(
@@ -103,15 +98,15 @@
 
 * The fact that log files contain additional trials from a semantic `'filler'` condition (which we want to skip because they don't have corresponding EEG triggers)
 
 * The *a priori* defined time windows and regions of interest for the N400 and P600 `components`
 
 * The log file columns (`average_by`) for which we want to obtain by-participant averaged waveforms (i.e., for all main and interaction effects)
 
-### 3.2 For R users
+### 2.2 For R users
 
 Here is the same example as above but for using the pipeline from R:
 
 ```R
 # Import Python module
 pipeline <- reticulate::import("pipeline")
 
@@ -139,7 +134,13 @@
 )
 
 # Extract results
 trials <- res[[1]]
 evokeds <- res[[2]]
 config <- res[[3]]
 ```
+
+## 3. Processing details
+
+<img src="https://github.com/alexenge/hu-neuro-pipeline/blob/main/doc/_static/flowchart.svg" width="400">
+
+See the [documentation](https://hu-neuro-pipeline.readthedocs.io/en/latest/) for more details about how to use the pipeline and how it works under the hood.
```

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/__init__.py` & `hu-neuro-pipeline-0.7.0/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/averaging.py` & `hu-neuro-pipeline-0.7.0/pipeline/averaging.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/boilerplate.py` & `hu-neuro-pipeline-0.7.0/pipeline/boilerplate.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/datasets/ucap.py` & `hu-neuro-pipeline-0.7.0/pipeline/datasets/ucap.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/epoching.py` & `hu-neuro-pipeline-0.7.0/pipeline/epoching.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/group.py` & `hu-neuro-pipeline-0.7.0/pipeline/group.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,44 +51,24 @@
     perm_tmin=0.0,
     perm_tmax=1.0,
     perm_channels=None,
     perm_fmin=None,
     perm_fmax=None,
     n_jobs=1
 ):
-    """Processes EEG data for all participants of an experiment.
+    """Process EEG data for a group of participants.
 
-    For each participant, the raw data is read and cleaned using standard steps
-    (downsampling, bad channel interpolation, ocular correction, frequency
-    domain filtering). Epochs are created around the `triggers`. Bad epochs are
-    removed based on peak-to-peak amplitude. Single trial mean ERP amplitudes
-    for ERP `components` of interest are computed and matched to the single
-    trial behavioral data from the `log_files`.
-
-    Optionally, this last step is repeated on a time-frequency representation
-    (TFR) of the data obtained via Morlet wavelet convolution.
-
-    The result is a single trial data frame which can be used for fitting
-    linear mixed-effects models on the mean ERP amplitudes (and power).
-
-    Additionally, by-participant condition averages (`evokeds`) for the ERPs
-    (and power) are computed to facilitate plotting. Optionally, these can also
-    be tested for condition differences in an exploratory fashion using
-    cluster-based permutation tests.
-
-    For details about the pipeline, see Frömer et al. (2018)[1].
+    Performs preprocessing and computes single trial mean amplitudes for ERP
+    components of interest as well as by-participant averaged waveforms.
+    Optionally, performs time-frequency analysis and/or cluster-based
+    permutation tests.
 
     Parameters & returns
     --------------------
-    See the README[2] in the GitHub repository for the pipeline.
-
-    Notes
-    -----
-    [1] https://doi.org/10.3389/fnins.2018.00048
-    [2] https://github.com/alexenge/hu-neuro-pipeline/blob/dev/README.md
+    See `Usage <../usage.html>`_ for the pipeline input arguments and outputs.
     """
 
     # Convert input types
     tfr_freqs = list(tfr_freqs)
     tfr_cycles = list(tfr_cycles)
 
     # Backup input arguments for re-use
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/io.py` & `hu-neuro-pipeline-0.7.0/pipeline/io.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/participant.py` & `hu-neuro-pipeline-0.7.0/pipeline/participant.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,42 +51,22 @@
     trials_dir=None,
     evokeds_dir=None,
     chanlocs_dir=None,
     tfr_dir=None,
     report_dir=None,
     to_df=True,
 ):
-    """Processes EEG data for a single participant.
+    """Process EEG data for a single participant.
 
-    The raw data is read and cleaned using standard steps (downsampling, bad
-    channel interpolation, ocular correction, frequency domain filtering).
-    Epochs are created around the `triggers`. Bad epochs are removed based on
-    peak-to-peak amplitude. Single trial mean ERP amplitudes for ERP
-    `components` of interest are computed and matched to the single trial
-    behavioral data from the `log_file`.
-
-    Optionally, this last step is repeated on a time-frequency representation
-    (TFR) of the data obtained via Morlet wavelet convolution.
-
-    The result is a single trial data frame which can be used for fitting
-    linear mixed-effects models on the mean ERP amplitudes (and power).
-
-    Additionally, condition averages (`evokeds`) for the ERPs (and power) are
-    computed to facilitate plotting.
-
-    For details about the pipeline, see Frömer et al. (2018)[1].
+    Performs preprocessing and computes single trial mean amplitudes for ERP
+    components of interest as well as averaged waveforms.
 
     Parameters & returns
     --------------------
-    See the README[2] in the GitHub repository for the pipeline.
-
-    Notes
-    -----
-    [1] https://doi.org/10.3389/fnins.2018.00048
-    [2] https://github.com/alexenge/hu-neuro-pipeline/blob/dev/README.md
+    See `Usage <../usage.html>`_ for the pipeline input arguments and outputs.
     """
 
     # Backup input arguments for re-use
     config = locals()
 
     # Read raw data
     raw, participant_id = read_raw(vhdr_file)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/perm.py` & `hu-neuro-pipeline-0.7.0/pipeline/perm.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/preprocessing.py` & `hu-neuro-pipeline-0.7.0/pipeline/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/report.py` & `hu-neuro-pipeline-0.7.0/pipeline/report.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/pipeline/tfr.py` & `hu-neuro-pipeline-0.7.0/pipeline/tfr.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.6/setup.py` & `hu-neuro-pipeline-0.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         project_urls={
             'Issue trackers': 'https://github.com/alexenge/hu-neuro-pipeline/issues',
         },
         classifiers=[
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
         ],
         packages=package_tree('pipeline'),
         install_requires=[
             'chardet',
             'joblib',
```

