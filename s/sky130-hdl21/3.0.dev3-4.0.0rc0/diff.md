# Comparing `tmp/sky130-hdl21-3.0.dev3.tar.gz` & `tmp/sky130-hdl21-4.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sky130-hdl21-3.0.dev3.tar", last modified: Tue Jan 17 23:17:59 2023, max compression
+gzip compressed data, was "sky130-hdl21-4.0.0rc0.tar", last modified: Tue Jul 11 16:55:35 2023, max compression
```

## Comparing `sky130-hdl21-3.0.dev3.tar` & `sky130-hdl21-4.0.0rc0.tar`

### file list

```diff
@@ -1,15 +1,30 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:59.254263 sky130-hdl21-3.0.dev3/
--rw-r--r--   0 dan        (501) staff       (20)      264 2023-01-17 23:17:59.254080 sky130-hdl21-3.0.dev3/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-05-03 17:59:57.000000 sky130-hdl21-3.0.dev3/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-01-17 23:17:59.254310 sky130-hdl21-3.0.dev3/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      905 2023-01-17 23:14:01.000000 sky130-hdl21-3.0.dev3/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:59.253048 sky130-hdl21-3.0.dev3/sky130/
--rw-r--r--   0 dan        (501) staff       (20)      315 2022-11-26 00:08:30.000000 sky130-hdl21-3.0.dev3/sky130/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     5480 2022-11-26 00:08:30.000000 sky130-hdl21-3.0.dev3/sky130/pdk.py
--rw-r--r--   0 dan        (501) staff       (20)     1984 2022-11-26 00:08:30.000000 sky130-hdl21-3.0.dev3/sky130/test_pdk.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:59.253875 sky130-hdl21-3.0.dev3/sky130_hdl21.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      264 2023-01-17 23:17:59.000000 sky130-hdl21-3.0.dev3/sky130_hdl21.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      249 2023-01-17 23:17:59.000000 sky130-hdl21-3.0.dev3/sky130_hdl21.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-01-17 23:17:59.000000 sky130-hdl21-3.0.dev3/sky130_hdl21.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       61 2023-01-17 23:17:59.000000 sky130-hdl21-3.0.dev3/sky130_hdl21.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)        7 2023-01-17 23:17:59.000000 sky130-hdl21-3.0.dev3/sky130_hdl21.egg-info/top_level.txt
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

### Comparing `sky130-hdl21-3.0.dev3/setup.py` & `sky130-hdl21-4.0.0rc0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "readme.md").read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "3.0.dev3"
+_VLSIR_VERSION = "4.0.0rc0"
 
 setup(
     name="sky130-hdl21",
     version=_VLSIR_VERSION,
     description="SkyWater 130nm PDK Package for Hdl21",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dan-fritchman/Hdl21",
-    author="Dan Fritchman",
+    author="Dan Fritchman, Thomas Pluck",
     packages=find_packages(),
-    python_requires=">=3.8, <4",
+    python_requires=">=3.7",
     install_requires=[f"hdl21=={_VLSIR_VERSION}"],
     extras_require={"dev": ["pytest==7.1", "coverage", "pytest-cov", "twine"]},
 )
```

