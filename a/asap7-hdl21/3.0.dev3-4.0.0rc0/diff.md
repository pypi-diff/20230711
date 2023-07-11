# Comparing `tmp/asap7-hdl21-3.0.dev3.tar.gz` & `tmp/asap7-hdl21-4.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asap7-hdl21-3.0.dev3.tar", last modified: Tue Jan 17 23:17:47 2023, max compression
+gzip compressed data, was "asap7-hdl21-4.0.0rc0.tar", last modified: Tue Jul 11 16:55:22 2023, max compression
```

## Comparing `asap7-hdl21-3.0.dev3.tar` & `asap7-hdl21-4.0.0rc0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:47.047925 asap7-hdl21-3.0.dev3/
--rw-r--r--   0 dan        (501) staff       (20)      254 2023-01-17 23:17:47.047717 asap7-hdl21-3.0.dev3/PKG-INFO
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:47.046262 asap7-hdl21-3.0.dev3/asap7/
--rw-r--r--   0 dan        (501) staff       (20)      315 2022-11-26 00:08:30.000000 asap7-hdl21-3.0.dev3/asap7/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     3985 2022-11-26 00:08:30.000000 asap7-hdl21-3.0.dev3/asap7/pdk.py
--rw-r--r--   0 dan        (501) staff       (20)      180 2022-11-26 00:08:30.000000 asap7-hdl21-3.0.dev3/asap7/test_pdk.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:47.047390 asap7-hdl21-3.0.dev3/asap7_hdl21.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      254 2023-01-17 23:17:46.000000 asap7-hdl21-3.0.dev3/asap7_hdl21.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      241 2023-01-17 23:17:47.000000 asap7-hdl21-3.0.dev3/asap7_hdl21.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-01-17 23:17:46.000000 asap7-hdl21-3.0.dev3/asap7_hdl21.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       61 2023-01-17 23:17:46.000000 asap7-hdl21-3.0.dev3/asap7_hdl21.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)        6 2023-01-17 23:17:46.000000 asap7-hdl21-3.0.dev3/asap7_hdl21.egg-info/top_level.txt
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-05-03 17:59:57.000000 asap7-hdl21-3.0.dev3/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-01-17 23:17:47.047979 asap7-hdl21-3.0.dev3/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      895 2023-01-17 23:14:01.000000 asap7-hdl21-3.0.dev3/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:55:22.273883 asap7-hdl21-4.0.0rc0/
+-rw-r--r--   0 dan        (501) staff       (20)      250 2023-07-11 16:55:22.273702 asap7-hdl21-4.0.0rc0/PKG-INFO
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:55:22.272774 asap7-hdl21-4.0.0rc0/asap7_hdl21/
+-rw-r--r--   0 dan        (501) staff       (20)      315 2023-07-11 14:50:48.000000 asap7-hdl21-4.0.0rc0/asap7_hdl21/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     3985 2023-07-11 14:50:48.000000 asap7-hdl21-4.0.0rc0/asap7_hdl21/pdk.py
+-rw-r--r--   0 dan        (501) staff       (20)      180 2023-07-11 14:50:48.000000 asap7-hdl21-4.0.0rc0/asap7_hdl21/test_pdk.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:55:22.273493 asap7-hdl21-4.0.0rc0/asap7_hdl21.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      250 2023-07-11 16:55:22.000000 asap7-hdl21-4.0.0rc0/asap7_hdl21.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      259 2023-07-11 16:55:22.000000 asap7-hdl21-4.0.0rc0/asap7_hdl21.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-11 16:55:22.000000 asap7-hdl21-4.0.0rc0/asap7_hdl21.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       61 2023-07-11 16:55:22.000000 asap7-hdl21-4.0.0rc0/asap7_hdl21.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       12 2023-07-11 16:55:22.000000 asap7-hdl21-4.0.0rc0/asap7_hdl21.egg-info/top_level.txt
+-rw-r--r--   0 dan        (501) staff       (20)        0 2022-05-03 17:59:57.000000 asap7-hdl21-4.0.0rc0/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-11 16:55:22.273925 asap7-hdl21-4.0.0rc0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      891 2023-07-11 16:53:58.000000 asap7-hdl21-4.0.0rc0/setup.py
```

### Comparing `asap7-hdl21-3.0.dev3/asap7/pdk.py` & `asap7-hdl21-4.0.0rc0/asap7_hdl21/pdk.py`

 * *Files identical despite different names*

### Comparing `asap7-hdl21-3.0.dev3/setup.py` & `asap7-hdl21-4.0.0rc0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "readme.md").read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "3.0.dev3"
+_VLSIR_VERSION = "4.0.0rc0"
 
 setup(
     name="asap7-hdl21",
     version=_VLSIR_VERSION,
     description="ASAP7 PDK Package for Hdl21",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dan-fritchman/Hdl21",
     author="Dan Fritchman",
     packages=find_packages(),
-    python_requires=">=3.8, <4",
+    python_requires=">=3.7",
     install_requires=[f"hdl21=={_VLSIR_VERSION}"],
     extras_require={"dev": ["pytest==7.1", "coverage", "pytest-cov", "twine"]},
 )
```

