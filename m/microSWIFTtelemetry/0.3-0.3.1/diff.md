# Comparing `tmp/microSWIFTtelemetry-0.3.tar.gz` & `tmp/microSWIFTtelemetry-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microSWIFTtelemetry-0.3.tar", last modified: Tue Jul 11 00:05:52 2023, max compression
+gzip compressed data, was "microSWIFTtelemetry-0.3.1.tar", last modified: Tue Jul 11 00:23:58 2023, max compression
```

## Comparing `microSWIFTtelemetry-0.3.tar` & `microSWIFTtelemetry-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:05:52.420707 microSWIFTtelemetry-0.3/
--rw-r--r--   0 jacob      (501) staff       (20)     1068 2022-11-06 06:16:28.000000 microSWIFTtelemetry-0.3/LICENSE
--rw-r--r--   0 jacob      (501) staff       (20)     1360 2023-07-11 00:05:52.420550 microSWIFTtelemetry-0.3/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     3636 2022-12-22 16:21:15.000000 microSWIFTtelemetry-0.3/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:05:52.418555 microSWIFTtelemetry-0.3/microSWIFTtelemetry/
--rw-r--r--   0 jacob      (501) staff       (20)      137 2022-12-04 19:59:27.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/__init__.py
--rw-r--r--   0 jacob      (501) staff       (20)     9144 2023-07-10 23:17:39.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/pull_telemetry.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:05:52.420170 microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/
--rw-r--r--   0 jacob      (501) staff       (20)       78 2022-12-04 20:17:51.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/__init__.py
--rw-r--r--   0 jacob      (501) staff       (20)     4301 2023-07-10 23:28:55.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/compile_sbd.py
--rw-r--r--   0 jacob      (501) staff       (20)     3012 2023-07-08 00:22:46.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/definitions.py
--rw-r--r--   0 jacob      (501) staff       (20)     6227 2023-07-10 22:55:49.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/read_sbd.py
--rw-r--r--   0 jacob      (501) staff       (20)     2387 2023-07-10 23:48:51.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry/version.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:05:52.419058 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1360 2023-07-11 00:05:52.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      506 2023-07-11 00:05:52.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-11 00:05:52.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       31 2023-07-11 00:05:52.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)       20 2023-07-11 00:05:52.000000 microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)      145 2022-11-06 01:29:54.000000 microSWIFTtelemetry-0.3/pyproject.toml
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-11 00:05:52.420751 microSWIFTtelemetry-0.3/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1373 2022-11-06 20:48:39.000000 microSWIFTtelemetry-0.3/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:23:58.374210 microSWIFTtelemetry-0.3.1/
+-rw-r--r--   0 jacob      (501) staff       (20)     1068 2022-11-06 06:16:28.000000 microSWIFTtelemetry-0.3.1/LICENSE
+-rw-r--r--   0 jacob      (501) staff       (20)     1362 2023-07-11 00:23:58.374073 microSWIFTtelemetry-0.3.1/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     3636 2022-12-22 16:21:15.000000 microSWIFTtelemetry-0.3.1/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:23:58.372474 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/
+-rw-r--r--   0 jacob      (501) staff       (20)      137 2022-12-04 19:59:27.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/__init__.py
+-rw-r--r--   0 jacob      (501) staff       (20)     9144 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/pull_telemetry.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:23:58.373864 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/
+-rw-r--r--   0 jacob      (501) staff       (20)       78 2022-12-04 20:17:51.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/__init__.py
+-rw-r--r--   0 jacob      (501) staff       (20)     4301 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/compile_sbd.py
+-rw-r--r--   0 jacob      (501) staff       (20)     3012 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/definitions.py
+-rw-r--r--   0 jacob      (501) staff       (20)     6227 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/read_sbd.py
+-rw-r--r--   0 jacob      (501) staff       (20)     2386 2023-07-11 00:23:33.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/version.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:23:58.372999 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1362 2023-07-11 00:23:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      506 2023-07-11 00:23:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-11 00:23:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       31 2023-07-11 00:23:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       20 2023-07-11 00:23:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)      145 2022-11-06 01:29:54.000000 microSWIFTtelemetry-0.3.1/pyproject.toml
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-11 00:23:58.374249 microSWIFTtelemetry-0.3.1/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1373 2022-11-06 20:48:39.000000 microSWIFTtelemetry-0.3.1/setup.py
```

### Comparing `microSWIFTtelemetry-0.3/LICENSE` & `microSWIFTtelemetry-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3/PKG-INFO` & `microSWIFTtelemetry-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microSWIFTtelemetry
-Version: 0.3
+Version: 0.3.1
 Summary: microSWIFTtelemetry: Python-based functionality for pulling telemetry from the microSWIFT wave buoy.
 Home-page: https://github.com/SASlabgroup/microSWIFTtelemetry
 Download-URL: 
 Author: Jacob Davis
 Author-email: davisjr@uw.edu
 Maintainer: Jacob Davis
 Maintainer-email: davisjr@uw.edu
```

### Comparing `microSWIFTtelemetry-0.3/README.md` & `microSWIFTtelemetry-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3/microSWIFTtelemetry/pull_telemetry.py` & `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/pull_telemetry.py`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/compile_sbd.py` & `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/compile_sbd.py`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/definitions.py` & `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/definitions.py`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3/microSWIFTtelemetry/sbd/read_sbd.py` & `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/read_sbd.py`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3/microSWIFTtelemetry/version.py` & `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import absolute_import, division, print_function
 from os.path import join as pjoin
 
 # Format expected by setup.py and doc/source/conf.py: string of form "X.Y.Z"
 _version_major = 0
 _version_minor = 3
-_version_micro = ''  # use '' for first of series, number for 1 and above
+_version_micro = 1  # use '' for first of series, number for 1 and above
 # _version_extra = 'dev'
 _version_extra = ''  # TODO: Uncomment this for full releases
 
 # Construct full version string from these.
 _ver = [_version_major, _version_minor]
 if _version_micro:
     _ver.append(_version_micro)
```

### Comparing `microSWIFTtelemetry-0.3/microSWIFTtelemetry.egg-info/PKG-INFO` & `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microSWIFTtelemetry
-Version: 0.3
+Version: 0.3.1
 Summary: microSWIFTtelemetry: Python-based functionality for pulling telemetry from the microSWIFT wave buoy.
 Home-page: https://github.com/SASlabgroup/microSWIFTtelemetry
 Download-URL: 
 Author: Jacob Davis
 Author-email: davisjr@uw.edu
 Maintainer: Jacob Davis
 Maintainer-email: davisjr@uw.edu
```

### Comparing `microSWIFTtelemetry-0.3/setup.py` & `microSWIFTtelemetry-0.3.1/setup.py`

 * *Files identical despite different names*

