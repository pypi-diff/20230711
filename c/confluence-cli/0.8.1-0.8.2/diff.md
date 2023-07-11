# Comparing `tmp/confluence_cli-0.8.1.tar.gz` & `tmp/confluence_cli-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluence_cli-0.8.1.tar", max compression
+gzip compressed data, was "confluence_cli-0.8.2.tar", max compression
```

## Comparing `confluence_cli-0.8.1.tar` & `confluence_cli-0.8.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2022-12-03 16:21:12.562517 confluence_cli-0.8.1/LICENSE.txt
--rw-r--r--   0        0        0      939 2022-12-12 18:03:51.829619 confluence_cli-0.8.1/README.md
--rw-r--r--   0        0        0      233 2022-12-03 16:21:12.318517 confluence_cli-0.8.1/confluence_cli/cli/__init__.py
--rw-r--r--   0        0        0     1860 2022-12-03 16:21:12.310517 confluence_cli-0.8.1/confluence_cli/cli/comala_api.py
--rw-r--r--   0        0        0     7219 2023-01-30 19:37:24.723228 confluence_cli-0.8.1/confluence_cli/cli/confluence_async.py
--rw-r--r--   0        0        0     1230 2022-12-12 17:53:44.181742 confluence_cli-0.8.1/confluence_cli/cli/confluence_limited.py
--rw-r--r--   0        0        0    13393 2022-12-12 21:17:59.128698 confluence_cli-0.8.1/confluence_cli/cli/confluence_wrapper.py
--rw-r--r--   0        0        0     8059 2023-01-30 14:53:18.184682 confluence_cli-0.8.1/confluence_cli/cli/paginators.py
--rw-r--r--   0        0        0     3509 2023-01-30 13:48:54.049440 confluence_cli-0.8.1/confluence_cli/cli/types.py
--rw-r--r--   0        0        0     2577 2023-07-08 20:52:47.543022 confluence_cli-0.8.1/confluence_cli/cli/utils.py
--rw-r--r--   0        0        0      817 2023-07-11 14:29:55.502003 confluence_cli-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 confluence_cli-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-12-03 16:21:12.562517 confluence_cli-0.8.2/LICENSE.txt
+-rw-r--r--   0        0        0      939 2022-12-12 18:03:51.829619 confluence_cli-0.8.2/README.md
+-rw-r--r--   0        0        0      233 2022-12-03 16:21:12.318517 confluence_cli-0.8.2/confluence_cli/cli/__init__.py
+-rw-r--r--   0        0        0     1860 2022-12-03 16:21:12.310517 confluence_cli-0.8.2/confluence_cli/cli/comala_api.py
+-rw-r--r--   0        0        0     7219 2023-01-30 19:37:24.723228 confluence_cli-0.8.2/confluence_cli/cli/confluence_async.py
+-rw-r--r--   0        0        0     1230 2022-12-12 17:53:44.181742 confluence_cli-0.8.2/confluence_cli/cli/confluence_limited.py
+-rw-r--r--   0        0        0    13393 2022-12-12 21:17:59.128698 confluence_cli-0.8.2/confluence_cli/cli/confluence_wrapper.py
+-rw-r--r--   0        0        0     8059 2023-01-30 14:53:18.184682 confluence_cli-0.8.2/confluence_cli/cli/paginators.py
+-rw-r--r--   0        0        0     3509 2023-01-30 13:48:54.049440 confluence_cli-0.8.2/confluence_cli/cli/types.py
+-rw-r--r--   0        0        0     2577 2023-07-08 20:52:47.543022 confluence_cli-0.8.2/confluence_cli/cli/utils.py
+-rw-r--r--   0        0        0      815 2023-07-11 14:35:29.142344 confluence_cli-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 confluence_cli-0.8.2/PKG-INFO
```

### Comparing `confluence_cli-0.8.1/LICENSE.txt` & `confluence_cli-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.1/README.md` & `confluence_cli-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.1/confluence_cli/cli/comala_api.py` & `confluence_cli-0.8.2/confluence_cli/cli/comala_api.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.1/confluence_cli/cli/confluence_async.py` & `confluence_cli-0.8.2/confluence_cli/cli/confluence_async.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.1/confluence_cli/cli/confluence_limited.py` & `confluence_cli-0.8.2/confluence_cli/cli/confluence_limited.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.1/confluence_cli/cli/confluence_wrapper.py` & `confluence_cli-0.8.2/confluence_cli/cli/confluence_wrapper.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.1/confluence_cli/cli/paginators.py` & `confluence_cli-0.8.2/confluence_cli/cli/paginators.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.1/confluence_cli/cli/types.py` & `confluence_cli-0.8.2/confluence_cli/cli/types.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.1/confluence_cli/cli/utils.py` & `confluence_cli-0.8.2/confluence_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.1/pyproject.toml` & `confluence_cli-0.8.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,24 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "confluence-cli"
-version = "0.8.1"
+version = "0.8.2"
 description = "Just another Atlassian Confluence API cli extension"
 authors = ["J. Andres Guerrero <juguerre@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "confluence_cli/cli"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0 <3.9"
-requests = "~2.28.1"
+requests = "^2.28"
 atlassian-python-api = "3.23.0"
 click = "^8.1.3"
 click-completion = "^0.5.2"
 tqdm = "^4.64.1"
 coloredlogs = "^15.0.1"
 urllib3 = "^1.26.13"
 python-decouple = "^3.6"
```

### Comparing `confluence_cli-0.8.1/PKG-INFO` & `confluence_cli-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confluence-cli
-Version: 0.8.1
+Version: 0.8.2
 Summary: Just another Atlassian Confluence API cli extension
 License: MIT
 Author: J. Andres Guerrero
 Author-email: juguerre@gmail.com
 Requires-Python: >=3.8.0,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-completion (>=0.5.2,<0.6.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: python-box (>=6.1.0,<7.0.0)
 Requires-Dist: python-decouple (>=3.6,<4.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.28.1,<2.29.0)
+Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.13,<2.0.0)
 Description-Content-Type: text/markdown
 
 # confluence-cli
 
 confluence-cli is a convenient wrapper module for python atlassian confluence original package.
```

