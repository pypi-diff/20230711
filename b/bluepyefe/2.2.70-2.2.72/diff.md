# Comparing `tmp/bluepyefe-2.2.70.tar.gz` & `tmp/bluepyefe-2.2.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepyefe-2.2.70.tar", last modified: Mon Jul  3 11:05:39 2023, max compression
+gzip compressed data, was "bluepyefe-2.2.72.tar", last modified: Tue Jul 11 06:59:05 2023, max compression
```

## Comparing `bluepyefe-2.2.70.tar` & `bluepyefe-2.2.72.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:05:39.577031 bluepyefe-2.2.70/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-03 11:05:39.577031 bluepyefe-2.2.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:05:39.577031 bluepyefe-2.2.70/bluepyefe/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 11:05:39.577031 bluepyefe-2.2.70/bluepyefe/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/auto_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:05:39.577031 bluepyefe-2.2.70/bluepyefe/ecode/
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/DeHyperPol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/HyperDePol.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/SpikeRec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/negCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/posCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/sAHP.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/sineSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/ecode/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:05:39.577031 bluepyefe-2.2.70/bluepyefe/igorpy/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/igorpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/nwbreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/rheobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/bluepyefe/translate_legacy_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:05:39.577031 bluepyefe-2.2.70/bluepyefe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-03 11:05:39.000000 bluepyefe-2.2.70/bluepyefe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-03 11:05:39.000000 bluepyefe-2.2.70/bluepyefe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:05:39.000000 bluepyefe-2.2.70/bluepyefe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 11:05:39.000000 bluepyefe-2.2.70/bluepyefe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 11:05:39.000000 bluepyefe-2.2.70/bluepyefe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:05:39.577031 bluepyefe-2.2.70/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 11:05:39.577031 bluepyefe-2.2.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-07-03 11:05:37.000000 bluepyefe-2.2.70/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:59:05.832747 bluepyefe-2.2.72/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-11 06:59:05.832747 bluepyefe-2.2.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:59:05.832747 bluepyefe-2.2.72/bluepyefe/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 06:59:05.832747 bluepyefe-2.2.72/bluepyefe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/auto_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:59:05.832747 bluepyefe-2.2.72/bluepyefe/ecode/
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/DeHyperPol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/HyperDePol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/SpikeRec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/negCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/posCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/sAHP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/sineSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/ecode/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:59:05.832747 bluepyefe-2.2.72/bluepyefe/igorpy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/igorpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/nwbreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/rheobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/bluepyefe/translate_legacy_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:59:05.832747 bluepyefe-2.2.72/bluepyefe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-11 06:59:05.000000 bluepyefe-2.2.72/bluepyefe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-11 06:59:05.000000 bluepyefe-2.2.72/bluepyefe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:59:05.000000 bluepyefe-2.2.72/bluepyefe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 06:59:05.000000 bluepyefe-2.2.72/bluepyefe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 06:59:05.000000 bluepyefe-2.2.72/bluepyefe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:59:05.832747 bluepyefe-2.2.72/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 06:59:05.832747 bluepyefe-2.2.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-07-11 06:59:02.000000 bluepyefe-2.2.72/versioneer.py
```

### Comparing `bluepyefe-2.2.70/LICENSE.txt` & `bluepyefe-2.2.72/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/PKG-INFO` & `bluepyefe-2.2.72/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.70
+Version: 2.2.72
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.70/README.rst` & `bluepyefe-2.2.72/README.rst`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/__init__.py` & `bluepyefe-2.2.72/bluepyefe/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/auto_targets.py` & `bluepyefe-2.2.72/bluepyefe/auto_targets.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/cell.py` & `bluepyefe-2.2.72/bluepyefe/cell.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/DeHyperPol.py` & `bluepyefe-2.2.72/bluepyefe/ecode/DeHyperPol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/HyperDePol.py` & `bluepyefe-2.2.72/bluepyefe/ecode/HyperDePol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/SpikeRec.py` & `bluepyefe-2.2.72/bluepyefe/ecode/SpikeRec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/__init__.py` & `bluepyefe-2.2.72/bluepyefe/ecode/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/negCheops.py` & `bluepyefe-2.2.72/bluepyefe/ecode/negCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/posCheops.py` & `bluepyefe-2.2.72/bluepyefe/ecode/posCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/ramp.py` & `bluepyefe-2.2.72/bluepyefe/ecode/ramp.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/sAHP.py` & `bluepyefe-2.2.72/bluepyefe/ecode/sAHP.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/sineSpec.py` & `bluepyefe-2.2.72/bluepyefe/ecode/sineSpec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/step.py` & `bluepyefe-2.2.72/bluepyefe/ecode/step.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/ecode/tools.py` & `bluepyefe-2.2.72/bluepyefe/ecode/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/extract.py` & `bluepyefe-2.2.72/bluepyefe/extract.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/igorpy/__init__.py` & `bluepyefe-2.2.72/bluepyefe/igorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/nwbreader.py` & `bluepyefe-2.2.72/bluepyefe/nwbreader.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/plotting.py` & `bluepyefe-2.2.72/bluepyefe/plotting.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/protocol.py` & `bluepyefe-2.2.72/bluepyefe/protocol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/reader.py` & `bluepyefe-2.2.72/bluepyefe/reader.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/recording.py` & `bluepyefe-2.2.72/bluepyefe/recording.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/rheobase.py` & `bluepyefe-2.2.72/bluepyefe/rheobase.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/target.py` & `bluepyefe-2.2.72/bluepyefe/target.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/tools.py` & `bluepyefe-2.2.72/bluepyefe/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe/translate_legacy_config.py` & `bluepyefe-2.2.72/bluepyefe/translate_legacy_config.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/bluepyefe.egg-info/PKG-INFO` & `bluepyefe-2.2.72/bluepyefe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.70
+Version: 2.2.72
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.70/bluepyefe.egg-info/SOURCES.txt` & `bluepyefe-2.2.72/bluepyefe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/examples/__init__.py` & `bluepyefe-2.2.72/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/setup.py` & `bluepyefe-2.2.72/setup.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.70/versioneer.py` & `bluepyefe-2.2.72/versioneer.py`

 * *Files identical despite different names*

