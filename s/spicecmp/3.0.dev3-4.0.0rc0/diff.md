# Comparing `tmp/spicecmp-3.0.dev3.tar.gz` & `tmp/spicecmp-4.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicecmp-3.0.dev3.tar", last modified: Tue Jan 17 23:18:12 2023, max compression
+gzip compressed data, was "spicecmp-4.0.0rc0.tar", last modified: Tue Jul 11 16:58:17 2023, max compression
```

## Comparing `spicecmp-3.0.dev3.tar` & `spicecmp-4.0.0rc0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:18:12.531322 spicecmp-3.0.dev3/
--rw-r--r--   0 dan        (501) staff       (20)     2842 2022-06-15 18:46:18.000000 spicecmp-3.0.dev3/.gitignore
--rw-r--r--   0 dan        (501) staff       (20)     5243 2023-01-17 23:18:12.531118 spicecmp-3.0.dev3/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     4962 2022-06-15 18:46:46.000000 spicecmp-3.0.dev3/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-01-17 23:18:12.531375 spicecmp-3.0.dev3/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1066 2023-01-17 23:14:16.000000 spicecmp-3.0.dev3/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:18:12.529058 spicecmp-3.0.dev3/spicecmp/
--rw-r--r--   0 dan        (501) staff       (20)      276 2022-07-19 02:39:52.000000 spicecmp-3.0.dev3/spicecmp/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    10416 2022-11-04 17:57:06.000000 spicecmp-3.0.dev3/spicecmp/benches.py
--rw-r--r--   0 dan        (501) staff       (20)     3773 2022-11-04 17:57:06.000000 spicecmp-3.0.dev3/spicecmp/compare_me.py
--rw-r--r--   0 dan        (501) staff       (20)     3334 2022-11-04 17:57:06.000000 spicecmp-3.0.dev3/spicecmp/compare_meas.py
--rw-r--r--   0 dan        (501) staff       (20)      170 2022-11-04 17:57:06.000000 spicecmp-3.0.dev3/spicecmp/corner.py
--rw-r--r--   0 dan        (501) staff       (20)      133 2022-11-04 17:57:06.000000 spicecmp-3.0.dev3/spicecmp/errormode.py
--rw-r--r--   0 dan        (501) staff       (20)      747 2022-11-04 17:57:06.000000 spicecmp-3.0.dev3/spicecmp/mos.py
--rw-r--r--   0 dan        (501) staff       (20)     2517 2022-11-04 17:57:06.000000 spicecmp-3.0.dev3/spicecmp/pdk.py
--rw-r--r--   0 dan        (501) staff       (20)      873 2022-11-04 17:57:06.000000 spicecmp-3.0.dev3/spicecmp/pdk_sim_combo.py
--rw-r--r--   0 dan        (501) staff       (20)      904 2022-11-04 17:57:06.000000 spicecmp-3.0.dev3/spicecmp/simulator.py
--rw-r--r--   0 dan        (501) staff       (20)     1856 2022-11-04 17:57:06.000000 spicecmp-3.0.dev3/spicecmp/testcase.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:18:12.530137 spicecmp-3.0.dev3/spicecmp.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     5243 2023-01-17 23:18:12.000000 spicecmp-3.0.dev3/spicecmp.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      460 2023-01-17 23:18:12.000000 spicecmp-3.0.dev3/spicecmp.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-01-17 23:18:12.000000 spicecmp-3.0.dev3/spicecmp.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)      117 2023-01-17 23:18:12.000000 spicecmp-3.0.dev3/spicecmp.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       15 2023-01-17 23:18:12.000000 spicecmp-3.0.dev3/spicecmp.egg-info/top_level.txt
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:18:12.530601 spicecmp-3.0.dev3/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-06-15 18:46:18.000000 spicecmp-3.0.dev3/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)       92 2022-07-19 02:39:52.000000 spicecmp-3.0.dev3/tests/test_spicecmp.py
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

### Comparing `spicecmp-3.0.dev3/.gitignore` & `spicecmp-4.0.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `spicecmp-3.0.dev3/PKG-INFO` & `spicecmp-4.0.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: spicecmp
-Version: 3.0.dev3
+Version: 4.0.0rc0
 Summary: Spice Models and Results Comparisons
 Home-page: https://github.com/Vlsir/Vlsir
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
-Requires-Python: >=3.8, <4
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 
 # SpiceCmp 
 
 A Python library for making comparisons between Spice-class simulators.
```

### Comparing `spicecmp-3.0.dev3/readme.md` & `spicecmp-4.0.0rc0/readme.md`

 * *Files identical despite different names*

### Comparing `spicecmp-3.0.dev3/setup.py` & `spicecmp-4.0.0rc0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 
 """
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 import pathlib
 
-here = pathlib.Path(__file__).parent.resolve()
-
 # Get the long description from the README file
-long_description = (here / "readme.md").read_text(encoding="utf-8")
+here = pathlib.Path(__file__).parent.resolve()
+readme = here / "readme.md"
+long_description = "" if not readme.exists() else readme.read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "3.0.dev3"
+_VLSIR_VERSION = "4.0.0rc0"
 
 setup(
     name="spicecmp",
     version=_VLSIR_VERSION,
     description="Spice Models and Results Comparisons",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Vlsir/Vlsir",
     author="Dan Fritchman",
     author_email="dan@fritch.mn",
     packages=find_packages(),
-    python_requires=">=3.8, <4",
+    python_requires=">=3.7, <3.12",
     install_requires=[
-        "pandas",
+        "pandas~=1.3",
         f"hdl21=={_VLSIR_VERSION}",
         f"vlsir=={_VLSIR_VERSION}",
         f"vlsirtools=={_VLSIR_VERSION}",
     ],
     extras_require={
         "dev": ["pytest==7.1", "coverage", "pytest-cov", "black==22.6", "twine"]
     },
```

### Comparing `spicecmp-3.0.dev3/spicecmp/benches.py` & `spicecmp-4.0.0rc0/spicecmp/benches.py`

 * *Files identical despite different names*

### Comparing `spicecmp-3.0.dev3/spicecmp/compare_me.py` & `spicecmp-4.0.0rc0/spicecmp/compare_me.py`

 * *Files identical despite different names*

### Comparing `spicecmp-3.0.dev3/spicecmp/compare_meas.py` & `spicecmp-4.0.0rc0/spicecmp/compare_meas.py`

 * *Files identical despite different names*

### Comparing `spicecmp-3.0.dev3/spicecmp/mos.py` & `spicecmp-4.0.0rc0/spicecmp/mos.py`

 * *Files identical despite different names*

### Comparing `spicecmp-3.0.dev3/spicecmp/pdk.py` & `spicecmp-4.0.0rc0/spicecmp/pdk.py`

 * *Files identical despite different names*

### Comparing `spicecmp-3.0.dev3/spicecmp/pdk_sim_combo.py` & `spicecmp-4.0.0rc0/spicecmp/pdk_sim_combo.py`

 * *Files identical despite different names*

### Comparing `spicecmp-3.0.dev3/spicecmp/simulator.py` & `spicecmp-4.0.0rc0/spicecmp/simulator.py`

 * *Files identical despite different names*

### Comparing `spicecmp-3.0.dev3/spicecmp/testcase.py` & `spicecmp-4.0.0rc0/spicecmp/testcase.py`

 * *Files identical despite different names*

### Comparing `spicecmp-3.0.dev3/spicecmp.egg-info/PKG-INFO` & `spicecmp-4.0.0rc0/spicecmp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: spicecmp
-Version: 3.0.dev3
+Version: 4.0.0rc0
 Summary: Spice Models and Results Comparisons
 Home-page: https://github.com/Vlsir/Vlsir
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
-Requires-Python: >=3.8, <4
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 
 # SpiceCmp 
 
 A Python library for making comparisons between Spice-class simulators.
```

