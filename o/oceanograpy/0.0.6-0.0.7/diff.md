# Comparing `tmp/oceanograpy-0.0.6.tar.gz` & `tmp/oceanograpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanograpy-0.0.6.tar", last modified: Tue Jul 11 20:53:49 2023, max compression
+gzip compressed data, was "oceanograpy-0.0.7.tar", last modified: Tue Jul 11 20:56:04 2023, max compression
```

## Comparing `oceanograpy-0.0.6.tar` & `oceanograpy-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 20:53:49.391430 oceanograpy-0.0.6/
--rw-rw-rw-   0        0        0    35823 2023-07-07 18:08:28.000000 oceanograpy-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      782 2023-07-11 20:53:49.390411 oceanograpy-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-08 03:43:29.000000 oceanograpy-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 20:53:49.379413 oceanograpy-0.0.6/oceanograpy/
--rw-rw-rw-   0        0        0      228 2023-07-11 20:51:36.000000 oceanograpy-0.0.6/oceanograpy/__init__.py
--rw-rw-rw-   0        0        0    24735 2023-07-11 18:15:27.000000 oceanograpy-0.0.6/oceanograpy/adcp_plot_tools.py
--rw-rw-rw-   0        0        0     2434 2023-07-11 20:22:37.000000 oceanograpy-0.0.6/oceanograpy/example.py
--rw-rw-rw-   0        0        0     2820 2023-07-11 20:50:48.000000 oceanograpy-0.0.6/oceanograpy/frma.py
--rw-rw-rw-   0        0        0     5339 2023-07-10 23:50:52.000000 oceanograpy-0.0.6/oceanograpy/matplotlib_dhi.py
--rw-rw-rw-   0        0        0     4375 2023-07-08 03:16:35.000000 oceanograpy-0.0.6/oceanograpy/processing_tools.py
--rw-rw-rw-   0        0        0    24857 2023-07-08 03:22:23.000000 oceanograpy-0.0.6/oceanograpy/seabird_ctd.py
--rw-rw-rw-   0        0        0    67612 2023-07-08 17:53:37.000000 oceanograpy-0.0.6/oceanograpy/workhorse_adcp.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:53:49.389413 oceanograpy-0.0.6/oceanograpy.egg-info/
--rw-rw-rw-   0        0        0      782 2023-07-11 20:53:49.000000 oceanograpy-0.0.6/oceanograpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-11 20:53:49.000000 oceanograpy-0.0.6/oceanograpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 20:53:49.000000 oceanograpy-0.0.6/oceanograpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 20:53:49.000000 oceanograpy-0.0.6/oceanograpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2023-07-08 00:06:28.000000 oceanograpy-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 20:53:49.392411 oceanograpy-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-07-11 20:52:58.000000 oceanograpy-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:56:04.241185 oceanograpy-0.0.7/
+-rw-rw-rw-   0        0        0    35823 2023-07-07 18:08:28.000000 oceanograpy-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      782 2023-07-11 20:56:04.240185 oceanograpy-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-08 03:43:29.000000 oceanograpy-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 20:56:04.218187 oceanograpy-0.0.7/oceanograpy/
+-rw-rw-rw-   0        0        0      202 2023-07-11 20:55:23.000000 oceanograpy-0.0.7/oceanograpy/__init__.py
+-rw-rw-rw-   0        0        0    24735 2023-07-11 18:15:27.000000 oceanograpy-0.0.7/oceanograpy/adcp_plot_tools.py
+-rw-rw-rw-   0        0        0     2434 2023-07-11 20:22:37.000000 oceanograpy-0.0.7/oceanograpy/example.py
+-rw-rw-rw-   0        0        0     2820 2023-07-11 20:50:48.000000 oceanograpy-0.0.7/oceanograpy/frma.py
+-rw-rw-rw-   0        0        0     5339 2023-07-10 23:50:52.000000 oceanograpy-0.0.7/oceanograpy/matplotlib_dhi.py
+-rw-rw-rw-   0        0        0     4375 2023-07-08 03:16:35.000000 oceanograpy-0.0.7/oceanograpy/processing_tools.py
+-rw-rw-rw-   0        0        0    24857 2023-07-08 03:22:23.000000 oceanograpy-0.0.7/oceanograpy/seabird_ctd.py
+-rw-rw-rw-   0        0        0    67612 2023-07-08 17:53:37.000000 oceanograpy-0.0.7/oceanograpy/workhorse_adcp.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:56:04.239186 oceanograpy-0.0.7/oceanograpy.egg-info/
+-rw-rw-rw-   0        0        0      782 2023-07-11 20:56:04.000000 oceanograpy-0.0.7/oceanograpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-11 20:56:04.000000 oceanograpy-0.0.7/oceanograpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 20:56:04.000000 oceanograpy-0.0.7/oceanograpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-11 20:56:04.000000 oceanograpy-0.0.7/oceanograpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2023-07-08 00:06:28.000000 oceanograpy-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 20:56:04.241185 oceanograpy-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-07-11 20:55:57.000000 oceanograpy-0.0.7/setup.py
```

### Comparing `oceanograpy-0.0.6/LICENSE` & `oceanograpy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.6/PKG-INFO` & `oceanograpy-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanograpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Toolbox for importing and plotting ADCP and CTD data
 Home-page:  
 Author: Andy Banks
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oceanograpy-0.0.6/oceanograpy/adcp_plot_tools.py` & `oceanograpy-0.0.7/oceanograpy/adcp_plot_tools.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.6/oceanograpy/example.py` & `oceanograpy-0.0.7/oceanograpy/example.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.6/oceanograpy/frma.py` & `oceanograpy-0.0.7/oceanograpy/frma.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.6/oceanograpy/matplotlib_dhi.py` & `oceanograpy-0.0.7/oceanograpy/matplotlib_dhi.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.6/oceanograpy/processing_tools.py` & `oceanograpy-0.0.7/oceanograpy/processing_tools.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.6/oceanograpy/seabird_ctd.py` & `oceanograpy-0.0.7/oceanograpy/seabird_ctd.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.6/oceanograpy/workhorse_adcp.py` & `oceanograpy-0.0.7/oceanograpy/workhorse_adcp.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.6/oceanograpy.egg-info/PKG-INFO` & `oceanograpy-0.0.7/oceanograpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanograpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Toolbox for importing and plotting ADCP and CTD data
 Home-page:  
 Author: Andy Banks
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oceanograpy-0.0.6/setup.py` & `oceanograpy-0.0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="oceanograpy",
-    version="0.0.6",
+    version="0.0.7",
     author="Andy Banks",
     author_email="",
     description="Toolbox for importing and plotting ADCP and CTD data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=" ",
     packages=["oceanograpy"],
```

