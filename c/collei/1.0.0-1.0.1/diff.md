# Comparing `tmp/collei-1.0.0.tar.gz` & `tmp/collei-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collei-1.0.0.tar", max compression
+gzip compressed data, was "collei-1.0.1.tar", max compression
```

## Comparing `collei-1.0.0.tar` & `collei-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1086 2023-07-01 17:03:03.878769 collei-1.0.0/LICENSE
--rw-r--r--   0        0        0      893 2023-07-06 13:51:46.340984 collei-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      689 2023-07-06 13:51:27.424093 collei-1.0.0/README.md
--rw-r--r--   0        0        0      335 2023-07-06 06:43:30.608088 collei-1.0.0/src/collei/__init__.py
--rw-r--r--   0        0        0      412 2023-07-06 06:43:43.225123 collei-1.0.0/src/collei/clients.py
--rw-r--r--   0        0        0        6 2023-07-06 06:42:51.138083 collei-1.0.0/src/collei/managers/__init__.py
--rw-r--r--   0        0        0      433 2023-07-06 06:42:20.980352 collei-1.0.0/src/collei/managers/nsfw.py
--rw-r--r--   0        0        0      426 2023-07-06 06:42:23.243536 collei-1.0.0/src/collei/managers/sfw.py
--rw-r--r--   0        0        0        6 2023-07-06 06:43:22.637155 collei-1.0.0/src/collei/models/__init__.py
--rw-r--r--   0        0        0        6 2023-07-06 06:43:19.639228 collei-1.0.0/src/collei/models/enums/__init__.py
--rw-r--r--   0        0        0        6 2023-07-06 06:42:47.792143 collei-1.0.0/src/collei/models/enums/categories/__init__.py
--rw-r--r--   0        0        0      168 2023-07-06 06:42:35.909192 collei-1.0.0/src/collei/models/enums/categories/nsfw.py
--rw-r--r--   0        0        0      714 2023-07-06 06:42:42.136063 collei-1.0.0/src/collei/models/enums/categories/sfw.py
--rw-r--r--   0        0        0       61 2023-07-06 06:43:28.650121 collei-1.0.0/src/collei/models/images.py
--rw-r--r--   0        0        0     1510 1970-01-01 00:00:00.000000 collei-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-01 17:03:03.878769 collei-1.0.1/LICENSE
+-rw-r--r--   0        0        0      901 2023-07-11 17:28:32.309193 collei-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      697 2023-07-07 12:08:21.322476 collei-1.0.1/README.md
+-rw-r--r--   0        0        0      328 2023-07-07 12:06:37.580405 collei-1.0.1/src/collei/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-07 12:06:36.062224 collei-1.0.1/src/collei/client.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:42:51.138083 collei-1.0.1/src/collei/manager/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-07 12:06:31.508657 collei-1.0.1/src/collei/manager/nsfw.py
+-rw-r--r--   0        0        0      423 2023-07-07 12:06:31.513657 collei-1.0.1/src/collei/manager/sfw.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:43:22.637155 collei-1.0.1/src/collei/model/__init__.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:43:19.639228 collei-1.0.1/src/collei/model/enums/__init__.py
+-rw-r--r--   0        0        0        6 2023-07-06 06:42:47.792143 collei-1.0.1/src/collei/model/enums/categories/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-06 06:42:35.909192 collei-1.0.1/src/collei/model/enums/categories/nsfw.py
+-rw-r--r--   0        0        0      714 2023-07-06 06:42:42.136063 collei-1.0.1/src/collei/model/enums/categories/sfw.py
+-rw-r--r--   0        0        0       61 2023-07-07 12:05:39.842835 collei-1.0.1/src/collei/model/image.py
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 collei-1.0.1/PKG-INFO
```

### Comparing `collei-1.0.0/LICENSE` & `collei-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `collei-1.0.0/pyproject.toml` & `collei-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "collei"
-version = "1.0.0"
+version = "1.0.1"
 description = "🍂 An unofficial Waifu.pics API wrapper for Python"
 license = "MIT"
 authors = ["elaresai <elaresai@gmail.com>"]
 maintainers = ["elaresai <elaresai@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/elaresai/collei"
 repository = "https://github.com/elaresai/collei"
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.9",
 
     "Topic :: Software Development :: Libraries",
 ]
 packages = [{ include = "collei", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.8.0,<3.12"
 attrs = "^23.1.0"
 requests = "^2.31.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `collei-1.0.0/README.md` & `collei-1.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # collei
-🍂 An unofficial [*Waifu.pics*](https://waifu.pics) API wrapper for Python
+
+🍂 An unofficial [_Waifu.pics API_](https://waifu.pics) wrapper for Python
 
 # 📦 Packages
+
 ## 🐍 PyPi
+
 ```sh
 pip install collei
 ```
+
 # 🔎 Examples
-[*examples/basic.py*](https://github.com/elaresai/xycu/blob/main/examples/basic.py)
-```py
-"""basic.py"""
 
-from collei import Client, SfwCategory
+[_examples/basic.py_](https://github.com/elaresai/collei/blob/main/examples/basic.py)
+
+```py
+import collei
 
-client = Client()
+client = collei.Client()
 
-print(client.sfw.get(SfwCategory.HUG))
-print(client.sfw.get(SfwCategory.KISS))
-print(client.sfw.get(SfwCategory.LICK))
-print(client.sfw.get(SfwCategory.BITE))
+print(client.sfw.get(collei.SfwCategory.HUG))
+print(client.sfw.get(collei.SfwCategory.KISS))
+print(client.sfw.get(collei.SfwCategory.LICK))
+print(client.sfw.get(collei.SfwCategory.BITE))
 ```
 
 # ✨ Links
-[🐍 *PyPi*](https://pypi.org/project/collei/)\
-[🏠 *Homepage*](https://github.com/elaresai/collei)\
-[🐱 *Repository*](https://github.com/elaresai/collei)
+
+[🐍 _PyPI_](https://pypi.org/project/collei/)\
+[🏠 _Homepage_](https://github.com/elaresai/collei)\
+[🐱 _Repository_](https://github.com/elaresai/collei)
```

### Comparing `collei-1.0.0/src/collei/models/enums/categories/sfw.py` & `collei-1.0.1/src/collei/model/enums/categories/sfw.py`

 * *Files identical despite different names*

### Comparing `collei-1.0.0/PKG-INFO` & `collei-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 Metadata-Version: 2.1
 Name: collei
-Version: 1.0.0
+Version: 1.0.1
 Summary: 🍂 An unofficial Waifu.pics API wrapper for Python
 Home-page: https://github.com/elaresai/collei
 License: MIT
 Author: elaresai
 Author-email: elaresai@gmail.com
 Maintainer: elaresai
 Maintainer-email: elaresai@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8.0,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/elaresai/collei
 Description-Content-Type: text/markdown
 
 # collei
-🍂 An unofficial [*Waifu.pics*](https://waifu.pics) API wrapper for Python
+
+🍂 An unofficial [_Waifu.pics API_](https://waifu.pics) wrapper for Python
 
 # 📦 Packages
+
 ## 🐍 PyPi
+
 ```sh
 pip install collei
 ```
+
 # 🔎 Examples
-[*examples/basic.py*](https://github.com/elaresai/xycu/blob/main/examples/basic.py)
-```py
-"""basic.py"""
 
-from collei import Client, SfwCategory
+[_examples/basic.py_](https://github.com/elaresai/collei/blob/main/examples/basic.py)
 
-client = Client()
+```py
+import collei
+
+client = collei.Client()
 
-print(client.sfw.get(SfwCategory.HUG))
-print(client.sfw.get(SfwCategory.KISS))
-print(client.sfw.get(SfwCategory.LICK))
-print(client.sfw.get(SfwCategory.BITE))
+print(client.sfw.get(collei.SfwCategory.HUG))
+print(client.sfw.get(collei.SfwCategory.KISS))
+print(client.sfw.get(collei.SfwCategory.LICK))
+print(client.sfw.get(collei.SfwCategory.BITE))
 ```
 
 # ✨ Links
-[🐍 *PyPi*](https://pypi.org/project/collei/)\
-[🏠 *Homepage*](https://github.com/elaresai/collei)\
-[🐱 *Repository*](https://github.com/elaresai/collei)
+
+[🐍 _PyPI_](https://pypi.org/project/collei/)\
+[🏠 _Homepage_](https://github.com/elaresai/collei)\
+[🐱 _Repository_](https://github.com/elaresai/collei)
```

