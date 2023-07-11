# Comparing `tmp/spicecmp-4.0.0.tar.gz` & `tmp/spicecmp-4.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicecmp-4.0.0.tar", last modified: Tue Jul 11 20:26:59 2023, max compression
+gzip compressed data, was "spicecmp-4.0.0rc0.tar", last modified: Tue Jul 11 16:58:17 2023, max compression
```

## Comparing `spicecmp-4.0.0.tar` & `spicecmp-4.0.0rc0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 20:26:59.683423 spicecmp-4.0.0/
--rw-r--r--   0 dan        (501) staff       (20)     2842 2023-06-26 21:21:08.000000 spicecmp-4.0.0/.gitignore
--rw-r--r--   0 dan        (501) staff       (20)     5243 2023-07-11 20:26:59.683243 spicecmp-4.0.0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     4962 2023-06-26 21:21:08.000000 spicecmp-4.0.0/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-11 20:26:59.683464 spicecmp-4.0.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1115 2023-07-11 20:23:32.000000 spicecmp-4.0.0/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 20:26:59.682058 spicecmp-4.0.0/spicecmp/
--rw-r--r--   0 dan        (501) staff       (20)      276 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    10416 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/benches.py
--rw-r--r--   0 dan        (501) staff       (20)     3773 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/compare_me.py
--rw-r--r--   0 dan        (501) staff       (20)     3334 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/compare_meas.py
--rw-r--r--   0 dan        (501) staff       (20)      170 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/corner.py
--rw-r--r--   0 dan        (501) staff       (20)      133 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/errormode.py
--rw-r--r--   0 dan        (501) staff       (20)      747 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/mos.py
--rw-r--r--   0 dan        (501) staff       (20)     2517 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/pdk.py
--rw-r--r--   0 dan        (501) staff       (20)      873 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/pdk_sim_combo.py
--rw-r--r--   0 dan        (501) staff       (20)      904 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/simulator.py
--rw-r--r--   0 dan        (501) staff       (20)     1856 2023-06-26 21:21:08.000000 spicecmp-4.0.0/spicecmp/testcase.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 20:26:59.682774 spicecmp-4.0.0/spicecmp.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     5243 2023-07-11 20:26:59.000000 spicecmp-4.0.0/spicecmp.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      460 2023-07-11 20:26:59.000000 spicecmp-4.0.0/spicecmp.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-11 20:26:59.000000 spicecmp-4.0.0/spicecmp.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)      113 2023-07-11 20:26:59.000000 spicecmp-4.0.0/spicecmp.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       15 2023-07-11 20:26:59.000000 spicecmp-4.0.0/spicecmp.egg-info/top_level.txt
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 20:26:59.683032 spicecmp-4.0.0/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2023-06-26 21:21:08.000000 spicecmp-4.0.0/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)       92 2023-06-26 21:21:08.000000 spicecmp-4.0.0/tests/test_spicecmp.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:58:17.276863 spicecmp-4.0.0rc0/
+-rw-r--r--   0 dan        (501) staff       (20)     2842 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/.gitignore
+-rw-r--r--   0 dan        (501) staff       (20)     5246 2023-07-11 16:58:17.276624 spicecmp-4.0.0rc0/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     4962 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-11 16:58:17.276911 spicecmp-4.0.0rc0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     1118 2023-07-11 16:44:54.000000 spicecmp-4.0.0rc0/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:58:17.274826 spicecmp-4.0.0rc0/spicecmp/
+-rw-r--r--   0 dan        (501) staff       (20)      276 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    10416 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/benches.py
+-rw-r--r--   0 dan        (501) staff       (20)     3773 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/compare_me.py
+-rw-r--r--   0 dan        (501) staff       (20)     3334 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/compare_meas.py
+-rw-r--r--   0 dan        (501) staff       (20)      170 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/corner.py
+-rw-r--r--   0 dan        (501) staff       (20)      133 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/errormode.py
+-rw-r--r--   0 dan        (501) staff       (20)      747 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/mos.py
+-rw-r--r--   0 dan        (501) staff       (20)     2517 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/pdk.py
+-rw-r--r--   0 dan        (501) staff       (20)      873 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/pdk_sim_combo.py
+-rw-r--r--   0 dan        (501) staff       (20)      904 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/simulator.py
+-rw-r--r--   0 dan        (501) staff       (20)     1856 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/spicecmp/testcase.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:58:17.275879 spicecmp-4.0.0rc0/spicecmp.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     5246 2023-07-11 16:58:17.000000 spicecmp-4.0.0rc0/spicecmp.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      460 2023-07-11 16:58:17.000000 spicecmp-4.0.0rc0/spicecmp.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-11 16:58:17.000000 spicecmp-4.0.0rc0/spicecmp.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)      122 2023-07-11 16:58:17.000000 spicecmp-4.0.0rc0/spicecmp.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       15 2023-07-11 16:58:17.000000 spicecmp-4.0.0rc0/spicecmp.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:58:17.276127 spicecmp-4.0.0rc0/tests/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/tests/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)       92 2023-06-26 21:21:08.000000 spicecmp-4.0.0rc0/tests/test_spicecmp.py
```

### Comparing `spicecmp-4.0.0/.gitignore` & `spicecmp-4.0.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `spicecmp-4.0.0/PKG-INFO` & `spicecmp-4.0.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicecmp
-Version: 4.0.0
+Version: 4.0.0rc0
 Summary: Spice Models and Results Comparisons
 Home-page: https://github.com/Vlsir/Vlsir
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spicecmp-4.0.0/readme.md` & `spicecmp-4.0.0rc0/readme.md`

 * *Files identical despite different names*

### Comparing `spicecmp-4.0.0/setup.py` & `spicecmp-4.0.0rc0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pathlib
 
 # Get the long description from the README file
 here = pathlib.Path(__file__).parent.resolve()
 readme = here / "readme.md"
 long_description = "" if not readme.exists() else readme.read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "4.0.0"
+_VLSIR_VERSION = "4.0.0rc0"
 
 setup(
     name="spicecmp",
     version=_VLSIR_VERSION,
     description="Spice Models and Results Comparisons",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `spicecmp-4.0.0/spicecmp/benches.py` & `spicecmp-4.0.0rc0/spicecmp/benches.py`

 * *Files identical despite different names*

### Comparing `spicecmp-4.0.0/spicecmp/compare_me.py` & `spicecmp-4.0.0rc0/spicecmp/compare_me.py`

 * *Files identical despite different names*

### Comparing `spicecmp-4.0.0/spicecmp/compare_meas.py` & `spicecmp-4.0.0rc0/spicecmp/compare_meas.py`

 * *Files identical despite different names*

### Comparing `spicecmp-4.0.0/spicecmp/mos.py` & `spicecmp-4.0.0rc0/spicecmp/mos.py`

 * *Files identical despite different names*

### Comparing `spicecmp-4.0.0/spicecmp/pdk.py` & `spicecmp-4.0.0rc0/spicecmp/pdk.py`

 * *Files identical despite different names*

### Comparing `spicecmp-4.0.0/spicecmp/pdk_sim_combo.py` & `spicecmp-4.0.0rc0/spicecmp/pdk_sim_combo.py`

 * *Files identical despite different names*

### Comparing `spicecmp-4.0.0/spicecmp/simulator.py` & `spicecmp-4.0.0rc0/spicecmp/simulator.py`

 * *Files identical despite different names*

### Comparing `spicecmp-4.0.0/spicecmp/testcase.py` & `spicecmp-4.0.0rc0/spicecmp/testcase.py`

 * *Files identical despite different names*

### Comparing `spicecmp-4.0.0/spicecmp.egg-info/PKG-INFO` & `spicecmp-4.0.0rc0/spicecmp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicecmp
-Version: 4.0.0
+Version: 4.0.0rc0
 Summary: Spice Models and Results Comparisons
 Home-page: https://github.com/Vlsir/Vlsir
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

