# Comparing `tmp/sky130-hdl21-4.0.0.tar.gz` & `tmp/sky130-hdl21-4.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sky130-hdl21-4.0.0.tar", last modified: Tue Jul 11 20:26:33 2023, max compression
+gzip compressed data, was "sky130-hdl21-4.0.0rc0.tar", last modified: Tue Jul 11 16:55:35 2023, max compression
```

## Comparing `sky130-hdl21-4.0.0.tar` & `sky130-hdl21-4.0.0rc0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 20:26:33.560955 sky130-hdl21-4.0.0/
--rw-r--r--   0 dan        (501) staff       (20)    20705 2023-07-11 20:26:33.560737 sky130-hdl21-4.0.0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)    20433 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-11 20:26:33.560999 sky130-hdl21-4.0.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      912 2023-07-11 20:22:36.000000 sky130-hdl21-4.0.0/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 20:26:33.556661 sky130-hdl21-4.0.0/sky130_hdl21/
--rw-r--r--   0 dan        (501) staff       (20)      333 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 20:26:33.559089 sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/
--rw-r--r--   0 dan        (501) staff       (20)      153 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    54089 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/high_density.py
--rw-r--r--   0 dan        (501) staff       (20)    46922 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/high_speed.py
--rw-r--r--   0 dan        (501) staff       (20)    44111 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/low_leakage.py
--rw-r--r--   0 dan        (501) staff       (20)    88672 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/low_power.py
--rw-r--r--   0 dan        (501) staff       (20)    47203 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/low_speed.py
--rw-r--r--   0 dan        (501) staff       (20)    47898 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/medium_speed.py
--rw-r--r--   0 dan        (501) staff       (20)    15550 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/pdk_data.py
--rw-r--r--   0 dan        (501) staff       (20)    13463 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/pdk_logic.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 20:26:33.560447 sky130-hdl21-4.0.0/sky130_hdl21/primitives/
--rw-r--r--   0 dan        (501) staff       (20)       26 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/primitives/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    14933 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/primitives/prim_dicts.py
--rw-r--r--   0 dan        (501) staff       (20)     7888 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/primitives/primitives.py
--rw-r--r--   0 dan        (501) staff       (20)     7191 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/test_netlists.py
--rw-r--r--   0 dan        (501) staff       (20)    13614 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/test_pdk.py
--rw-r--r--   0 dan        (501) staff       (20)    21806 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0/sky130_hdl21/test_site_sims.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 20:26:33.557458 sky130-hdl21-4.0.0/sky130_hdl21.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)    20705 2023-07-11 20:26:33.000000 sky130-hdl21-4.0.0/sky130_hdl21.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      759 2023-07-11 20:26:33.000000 sky130-hdl21-4.0.0/sky130_hdl21.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-11 20:26:33.000000 sky130-hdl21-4.0.0/sky130_hdl21.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       58 2023-07-11 20:26:33.000000 sky130-hdl21-4.0.0/sky130_hdl21.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       13 2023-07-11 20:26:33.000000 sky130-hdl21-4.0.0/sky130_hdl21.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:55:35.860919 sky130-hdl21-4.0.0rc0/
+-rw-r--r--   0 dan        (501) staff       (20)    20708 2023-07-11 16:55:35.860704 sky130-hdl21-4.0.0rc0/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)    20433 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-11 16:55:35.860964 sky130-hdl21-4.0.0rc0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      915 2023-07-11 16:52:30.000000 sky130-hdl21-4.0.0rc0/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:55:35.858046 sky130-hdl21-4.0.0rc0/sky130_hdl21/
+-rw-r--r--   0 dan        (501) staff       (20)      333 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:55:35.859992 sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/
+-rw-r--r--   0 dan        (501) staff       (20)      153 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    54089 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/high_density.py
+-rw-r--r--   0 dan        (501) staff       (20)    46922 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/high_speed.py
+-rw-r--r--   0 dan        (501) staff       (20)    44111 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/low_leakage.py
+-rw-r--r--   0 dan        (501) staff       (20)    88672 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/low_power.py
+-rw-r--r--   0 dan        (501) staff       (20)    47203 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/low_speed.py
+-rw-r--r--   0 dan        (501) staff       (20)    47898 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/medium_speed.py
+-rw-r--r--   0 dan        (501) staff       (20)    15550 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/pdk_data.py
+-rw-r--r--   0 dan        (501) staff       (20)    13463 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/pdk_logic.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:55:35.860468 sky130-hdl21-4.0.0rc0/sky130_hdl21/primitives/
+-rw-r--r--   0 dan        (501) staff       (20)       26 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/primitives/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    14933 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/primitives/prim_dicts.py
+-rw-r--r--   0 dan        (501) staff       (20)     7888 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/primitives/primitives.py
+-rw-r--r--   0 dan        (501) staff       (20)     7191 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/test_netlists.py
+-rw-r--r--   0 dan        (501) staff       (20)    13614 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/test_pdk.py
+-rw-r--r--   0 dan        (501) staff       (20)    21806 2023-07-11 14:50:48.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21/test_site_sims.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:55:35.858778 sky130-hdl21-4.0.0rc0/sky130_hdl21.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)    20708 2023-07-11 16:55:35.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      759 2023-07-11 16:55:35.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-11 16:55:35.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       61 2023-07-11 16:55:35.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       13 2023-07-11 16:55:35.000000 sky130-hdl21-4.0.0rc0/sky130_hdl21.egg-info/top_level.txt
```

### Comparing `sky130-hdl21-4.0.0/PKG-INFO` & `sky130-hdl21-4.0.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sky130-hdl21
-Version: 4.0.0
+Version: 4.0.0rc0
 Summary: SkyWater 130nm PDK Package for Hdl21
 Home-page: https://github.com/dan-fritchman/Hdl21
 Author: Dan Fritchman, Thomas Pluck
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `sky130-hdl21-4.0.0/readme.md` & `sky130-hdl21-4.0.0rc0/readme.md`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/setup.py` & `sky130-hdl21-4.0.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "readme.md").read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "4.0.0"
+_VLSIR_VERSION = "4.0.0rc0"
 
 setup(
     name="sky130-hdl21",
     version=_VLSIR_VERSION,
     description="SkyWater 130nm PDK Package for Hdl21",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/high_density.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/high_density.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/high_speed.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/high_speed.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/low_leakage.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/low_leakage.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/low_power.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/low_power.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/low_speed.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/low_speed.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/digital_cells/medium_speed.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/digital_cells/medium_speed.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/pdk_data.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/pdk_data.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/pdk_logic.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/pdk_logic.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/primitives/prim_dicts.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/primitives/prim_dicts.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/primitives/primitives.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/primitives/primitives.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/test_netlists.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/test_netlists.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/test_pdk.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/test_pdk.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21/test_site_sims.py` & `sky130-hdl21-4.0.0rc0/sky130_hdl21/test_site_sims.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21.egg-info/PKG-INFO` & `sky130-hdl21-4.0.0rc0/sky130_hdl21.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sky130-hdl21
-Version: 4.0.0
+Version: 4.0.0rc0
 Summary: SkyWater 130nm PDK Package for Hdl21
 Home-page: https://github.com/dan-fritchman/Hdl21
 Author: Dan Fritchman, Thomas Pluck
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `sky130-hdl21-4.0.0/sky130_hdl21.egg-info/SOURCES.txt` & `sky130-hdl21-4.0.0rc0/sky130_hdl21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

