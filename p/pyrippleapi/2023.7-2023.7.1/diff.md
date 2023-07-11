# Comparing `tmp/pyrippleapi-2023.7.tar.gz` & `tmp/pyrippleapi-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrippleapi-2023.7.tar", last modified: Tue Jul 11 11:12:37 2023, max compression
+gzip compressed data, was "pyrippleapi-2023.7.1.tar", last modified: Tue Jul 11 12:20:23 2023, max compression
```

## Comparing `pyrippleapi-2023.7.tar` & `pyrippleapi-2023.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 11:12:37.161899 pyrippleapi-2023.7/
--rw-rw-rw-   0        0        0      416 2023-07-11 11:12:37.161899 pyrippleapi-2023.7/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2023.7/README.md
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2023.7/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-07-11 11:12:37.169902 pyrippleapi-2023.7/setup.cfg
--rw-rw-rw-   0        0        0      815 2023-07-11 10:50:28.000000 pyrippleapi-2023.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 11:12:37.099902 pyrippleapi-2023.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 11:12:37.118902 pyrippleapi-2023.7/src/pyrippleapi/
--rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2023.7/src/pyrippleapi/__init__.py
--rw-rw-rw-   0        0        0     2267 2023-07-11 11:07:23.000000 pyrippleapi-2023.7/src/pyrippleapi/api.py
--rw-rw-rw-   0        0        0      149 2023-07-11 11:06:07.000000 pyrippleapi-2023.7/src/pyrippleapi/exceptions.py
--rw-rw-rw-   0        0        0     5032 2023-07-11 11:11:06.000000 pyrippleapi-2023.7/src/pyrippleapi/generation_asset.py
-drwxrwxrwx   0        0        0        0 2023-07-11 11:12:37.159899 pyrippleapi-2023.7/src/pyrippleapi.egg-info/
--rw-rw-rw-   0        0        0      416 2023-07-11 11:12:37.000000 pyrippleapi-2023.7/src/pyrippleapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-07-11 11:12:37.000000 pyrippleapi-2023.7/src/pyrippleapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 11:12:37.000000 pyrippleapi-2023.7/src/pyrippleapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 11:12:37.000000 pyrippleapi-2023.7/src/pyrippleapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 11:12:37.000000 pyrippleapi-2023.7/src/pyrippleapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 12:20:23.386056 pyrippleapi-2023.7.1/
+-rw-rw-rw-   0        0        0      418 2023-07-11 12:20:23.386056 pyrippleapi-2023.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2023.7.1/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2023.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-11 12:20:23.395056 pyrippleapi-2023.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-07-11 12:19:20.000000 pyrippleapi-2023.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:20:23.326057 pyrippleapi-2023.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 12:20:23.346059 pyrippleapi-2023.7.1/src/pyrippleapi/
+-rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2023.7.1/src/pyrippleapi/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-07-11 12:19:13.000000 pyrippleapi-2023.7.1/src/pyrippleapi/api.py
+-rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2023.7.1/src/pyrippleapi/exceptions.py
+-rw-rw-rw-   0        0        0     5032 2023-07-11 11:11:06.000000 pyrippleapi-2023.7.1/src/pyrippleapi/generation_asset.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:20:23.384057 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-07-11 12:20:23.000000 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-07-11 12:20:23.000000 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 12:20:23.000000 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 12:20:23.000000 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-11 12:20:23.000000 pyrippleapi-2023.7.1/src/pyrippleapi.egg-info/top_level.txt
```

### Comparing `pyrippleapi-2023.7/setup.py` & `pyrippleapi-2023.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="pyrippleapi",
-    version="2023.7",
+    version="2023.7.1",
     description="Ripple energy api wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ryanbdclark/pyrippleapi",
     author="Ryan Clark",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

### Comparing `pyrippleapi-2023.7/src/pyrippleapi/api.py` & `pyrippleapi-2023.7.1/src/pyrippleapi/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-import aiohttp
 import logging
 from logging import Logger
 
+import aiohttp
+
 from .exceptions import (
-    RippleConnectionError
+    RippleAuthenticationError,
+    RippleConnectionError,
+    RippleDevicesError,
 )
 
 logger: Logger = logging.getLogger(__package__)
 
 
 class RippleAPI:
     """
@@ -70,8 +73,16 @@
 
         async with self.session.request(
             "GET", self._api_url + self._auth_token
         ) as response:
             if response.status != 200:
                 raise RippleConnectionError("Error sending request")
 
-            return await response.json()
+            response = await response.json()
+
+            if "error" in response:
+                raise RippleAuthenticationError("Invalid API Key")
+
+            if len(response["generation_assets"] < 1):
+                raise RippleDevicesError("No generation assets found")
+
+            return response
```

### Comparing `pyrippleapi-2023.7/src/pyrippleapi/generation_asset.py` & `pyrippleapi-2023.7.1/src/pyrippleapi/generation_asset.py`

 * *Files identical despite different names*

