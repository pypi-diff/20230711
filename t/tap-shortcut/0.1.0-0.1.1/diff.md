# Comparing `tmp/tap_shortcut-0.1.0.tar.gz` & `tmp/tap_shortcut-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_shortcut-0.1.0.tar", max compression
+gzip compressed data, was "tap_shortcut-0.1.1.tar", max compression
```

## Comparing `tap_shortcut-0.1.0.tar` & `tap_shortcut-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-07-07 17:21:40.227947 tap_shortcut-0.1.0/LICENSE
--rw-r--r--   0        0        0     2571 2023-07-07 17:21:40.227947 tap_shortcut-0.1.0/README.md
--rw-r--r--   0        0        0     2194 2023-07-07 17:22:03.543925 tap_shortcut-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-07-07 17:21:40.231947 tap_shortcut-0.1.0/tap_shortcut/__init__.py
--rw-r--r--   0        0        0     1063 2023-07-07 17:21:40.231947 tap_shortcut-0.1.0/tap_shortcut/client.py
--rw-r--r--   0        0        0     2247 2023-07-07 17:21:40.231947 tap_shortcut-0.1.0/tap_shortcut/streams.py
--rw-r--r--   0        0        0     3634 2023-07-07 17:21:40.231947 tap_shortcut-0.1.0/tap_shortcut/tap.py
--rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 tap_shortcut-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 19:49:53.235587 tap_shortcut-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2571 2023-07-11 19:49:53.235587 tap_shortcut-0.1.1/README.md
+-rw-r--r--   0        0        0     2194 2023-07-11 19:50:14.820091 tap_shortcut-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-07-11 19:49:53.235587 tap_shortcut-0.1.1/tap_shortcut/__init__.py
+-rw-r--r--   0        0        0     1063 2023-07-11 19:49:53.235587 tap_shortcut-0.1.1/tap_shortcut/client.py
+-rw-r--r--   0        0        0     2247 2023-07-11 19:49:53.235587 tap_shortcut-0.1.1/tap_shortcut/streams.py
+-rw-r--r--   0        0        0     3634 2023-07-11 19:49:53.235587 tap_shortcut-0.1.1/tap_shortcut/tap.py
+-rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 tap_shortcut-0.1.1/PKG-INFO
```

### Comparing `tap_shortcut-0.1.0/LICENSE` & `tap_shortcut-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.1.0/README.md` & `tap_shortcut-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.1.0/pyproject.toml` & `tap_shortcut-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-shortcut"
-version = "0.1.0"
+version = "0.1.1"
 description = "`tap-shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Shortcut",
 ]
@@ -12,15 +12,15 @@
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-shortcut"
 repository = "https://github.com/edgarrmondragon/tap-shortcut"
 documentation = "https://github.com/edgarrmondragon/tap-shortcut#readme"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "0.29.0"
+singer-sdk = "0.30.0"
 toolz = "0.12.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
 [tool.isort]
 profile = "black"
```

### Comparing `tap_shortcut-0.1.0/tap_shortcut/client.py` & `tap_shortcut-0.1.1/tap_shortcut/client.py`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.1.0/tap_shortcut/streams.py` & `tap_shortcut-0.1.1/tap_shortcut/streams.py`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.1.0/tap_shortcut/tap.py` & `tap_shortcut-0.1.1/tap_shortcut/tap.py`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.1.0/PKG-INFO` & `tap_shortcut-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tap-shortcut
-Version: 0.1.0
+Version: 0.1.1
 Summary: `tap-shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-shortcut
 License: Apache-2.0
 Keywords: ELT,singer.io,Shortcut
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: singer-sdk (==0.29.0)
+Requires-Dist: singer-sdk (==0.30.0)
 Requires-Dist: toolz (==0.12.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-shortcut#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-shortcut
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: tap-shortcut Version: 0.1.0 Summary: `tap-shortcut`
+Metadata-Version: 2.1 Name: tap-shortcut Version: 0.1.1 Summary: `tap-shortcut`
 is a Singer tap for Shortcut, built with the Meltano SDK for Singer Taps. Home-
 page: https://github.com/edgarrmondragon/tap-shortcut License: Apache-2.0
 Keywords: ELT,singer.io,Shortcut Author: Edgar RamÃ­rez-MondragÃ³n Author-
 email: edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: singer-sdk (==0.29.0) Requires-Dist: toolz (==0.12.0) Project-URL:
+Dist: singer-sdk (==0.30.0) Requires-Dist: toolz (==0.12.0) Project-URL:
 Documentation, https://github.com/edgarrmondragon/tap-shortcut#readme Project-
 URL: Repository, https://github.com/edgarrmondragon/tap-shortcut Description-
 Content-Type: text/markdown
                                 # tap-shortcut
                        [pre-commit.ci_status] [License]
       Singer tap for Shortcut. Built with the [Meltano Tap SDK](https://
                        sdk.meltano.com) for Singer Taps.
```

