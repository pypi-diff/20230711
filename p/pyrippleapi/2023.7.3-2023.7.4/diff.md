# Comparing `tmp/pyrippleapi-2023.7.3.tar.gz` & `tmp/pyrippleapi-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrippleapi-2023.7.3.tar", last modified: Tue Jul 11 13:50:54 2023, max compression
+gzip compressed data, was "pyrippleapi-2023.7.4.tar", last modified: Tue Jul 11 14:33:36 2023, max compression
```

## Comparing `pyrippleapi-2023.7.3.tar` & `pyrippleapi-2023.7.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 13:50:54.002374 pyrippleapi-2023.7.3/
--rw-rw-rw-   0        0        0      418 2023-07-11 13:50:54.002374 pyrippleapi-2023.7.3/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2023.7.3/README.md
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2023.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-07-11 13:50:54.005376 pyrippleapi-2023.7.3/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-07-11 13:50:12.000000 pyrippleapi-2023.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:50:53.952379 pyrippleapi-2023.7.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 13:50:53.976376 pyrippleapi-2023.7.3/src/pyrippleapi/
--rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2023.7.3/src/pyrippleapi/__init__.py
--rw-rw-rw-   0        0        0     2597 2023-07-11 12:39:48.000000 pyrippleapi-2023.7.3/src/pyrippleapi/api.py
--rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2023.7.3/src/pyrippleapi/exceptions.py
--rw-rw-rw-   0        0        0     5738 2023-07-11 13:50:05.000000 pyrippleapi-2023.7.3/src/pyrippleapi/generation_asset.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:50:54.000375 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/
--rw-rw-rw-   0        0        0      418 2023-07-11 13:50:53.000000 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-07-11 13:50:53.000000 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 13:50:53.000000 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 13:50:53.000000 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 13:50:53.000000 pyrippleapi-2023.7.3/src/pyrippleapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 14:33:36.328366 pyrippleapi-2023.7.4/
+-rw-rw-rw-   0        0        0      418 2023-07-11 14:33:36.329366 pyrippleapi-2023.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-11 09:09:37.000000 pyrippleapi-2023.7.4/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyrippleapi-2023.7.4/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-11 14:33:36.331368 pyrippleapi-2023.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-07-11 14:32:34.000000 pyrippleapi-2023.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:33:36.276368 pyrippleapi-2023.7.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 14:33:36.302368 pyrippleapi-2023.7.4/src/pyrippleapi/
+-rw-rw-rw-   0        0        0        0 2023-07-11 09:10:36.000000 pyrippleapi-2023.7.4/src/pyrippleapi/__init__.py
+-rw-rw-rw-   0        0        0     3076 2023-07-11 14:32:19.000000 pyrippleapi-2023.7.4/src/pyrippleapi/api.py
+-rw-rw-rw-   0        0        0      336 2023-07-11 12:16:29.000000 pyrippleapi-2023.7.4/src/pyrippleapi/exceptions.py
+-rw-rw-rw-   0        0        0     5738 2023-07-11 13:50:05.000000 pyrippleapi-2023.7.4/src/pyrippleapi/generation_asset.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:33:36.326369 pyrippleapi-2023.7.4/src/pyrippleapi.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-07-11 14:33:36.000000 pyrippleapi-2023.7.4/src/pyrippleapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-07-11 14:33:36.000000 pyrippleapi-2023.7.4/src/pyrippleapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:33:36.000000 pyrippleapi-2023.7.4/src/pyrippleapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 14:33:36.000000 pyrippleapi-2023.7.4/src/pyrippleapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-11 14:33:36.000000 pyrippleapi-2023.7.4/src/pyrippleapi.egg-info/top_level.txt
```

### Comparing `pyrippleapi-2023.7.3/setup.py` & `pyrippleapi-2023.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="pyrippleapi",
-    version="2023.7.3",
+    version="2023.7.4",
     description="Ripple energy api wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ryanbdclark/pyrippleapi",
     author="Ryan Clark",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

### Comparing `pyrippleapi-2023.7.3/src/pyrippleapi/api.py` & `pyrippleapi-2023.7.4/src/pyrippleapi/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -67,22 +67,29 @@
         Method for calling the Ripple API
 
         Returns
         ------
         dict: Dictionary containing the response
         """
 
+        headers = {
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Accept-Language": "en-GB,en;q=0.9,en-US;q=0.8",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.67",
+        }
+
         async with self.session.request(
-            "GET", self._api_url + self._auth_token
+            "GET", self._api_url + self._auth_token, headers=headers
         ) as response:
             if response.status != 200:
                 raise RippleConnectionError("Error sending request")
 
             response = await response.json()
 
             if "error" in response:
                 raise RippleAuthenticationError("Invalid API Key")
 
-            if len(response["generation_assets"])<1:
+            if len(response["generation_assets"]) < 1:
                 raise RippleDevicesError("No generation assets found")
 
             return response
```

### Comparing `pyrippleapi-2023.7.3/src/pyrippleapi/generation_asset.py` & `pyrippleapi-2023.7.4/src/pyrippleapi/generation_asset.py`

 * *Files identical despite different names*

