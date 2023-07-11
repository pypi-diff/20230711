# Comparing `tmp/findmyorder-1.5.9.tar.gz` & `tmp/findmyorder-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.5.9.tar", max compression
+gzip compressed data, was "findmyorder-1.6.0.tar", max compression
```

## Comparing `findmyorder-1.5.9.tar` & `findmyorder-1.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-08 13:56:29.259122 findmyorder-1.5.9/LICENSE
--rw-r--r--   0        0        0     3046 2023-07-08 13:56:29.259122 findmyorder-1.5.9/README.md
--rw-r--r--   0        0        0      113 2023-07-08 13:56:30.059133 findmyorder-1.5.9/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-07-08 13:56:29.259122 findmyorder-1.5.9/findmyorder/config.py
--rw-r--r--   0        0        0     2495 2023-07-08 13:56:29.259122 findmyorder-1.5.9/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5779 2023-07-08 13:56:29.259122 findmyorder-1.5.9/findmyorder/main.py
--rw-r--r--   0        0        0     2349 2023-07-08 13:56:30.055133 findmyorder-1.5.9/pyproject.toml
--rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 findmyorder-1.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-11 19:37:13.897006 findmyorder-1.6.0/LICENSE
+-rw-r--r--   0        0        0     3049 2023-07-11 19:37:13.897006 findmyorder-1.6.0/README.md
+-rw-r--r--   0        0        0      113 2023-07-11 19:37:14.641029 findmyorder-1.6.0/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-07-11 19:37:13.897006 findmyorder-1.6.0/findmyorder/config.py
+-rw-r--r--   0        0        0     2533 2023-07-11 19:37:13.897006 findmyorder-1.6.0/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5875 2023-07-11 19:37:13.897006 findmyorder-1.6.0/findmyorder/main.py
+-rw-r--r--   0        0        0     2380 2023-07-11 19:37:14.641029 findmyorder-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3922 1970-01-01 00:00:00.000000 findmyorder-1.6.0/PKG-INFO
```

### Comparing `findmyorder-1.5.9/LICENSE` & `findmyorder-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.9/README.md` & `findmyorder-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/v/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/dm/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://github.com/mraniki/findmyorder"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/findmyorder/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
-   <a href="https://talkyuniverse.readthedocs.io/projects/fyndmyorder/"><img src="https://readthedocs.org/projects/talkytrend/badge/?version=latest&style=for-the-badge"></a><br>
+   <a href="https://talky.readthedocs.io/projects/findmyorder/index.html"><img src="https://readthedocs.org/projects/findmyorder/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-findmyorder-main"><img src="https://codebeat.co/badges/9b113098-d22d-498d-9c61-eb1e96c1311a"/></a><br>
    <a href="https://codecov.io/gh/mraniki/findmyorder"><img src="https://codecov.io/gh/mraniki/findmyorder/branch/main/graph/badge.svg?token=4838MSZNCC"/> </a><br>
     </td>
      <td align="left"> 
         Find My order,<br>
        a parsing package to find trading order
      </td>
```

#### html2text {}

```diff
@@ -14,15 +14,15 @@
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/findmyorder?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/github/actions/workflow/status/
 mraniki/findmyorder/                                        Find My order,
 %F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-  a parsing package
 the-badge&logo=GitHub&logoColor=white]                      to find trading
-[https://readthedocs.org/projects/talkytrend/badge/         order
+[https://readthedocs.org/projects/findmyorder/badge/        order
 ?version=latest&style=for-the-badge]
 [https://codebeat.co/badges/9b113098-d22d-498d-9c61-
 eb1e96c1311a]
 [https://codecov.io/gh/mraniki/findmyorder/branch/main/
 graph/badge.svg?token=4838MSZNCC]
 ** How to use it **
```

### Comparing `findmyorder-1.5.9/findmyorder/config.py` & `findmyorder-1.6.0/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.9/findmyorder/default_settings.toml` & `findmyorder-1.6.0/findmyorder/default_settings.toml`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 instrument_mapping = true
 mapping = [
     { id = "GOLD", alt = "XAUUSD" },
     { id = "SILVER", alt = "XAGUSD" },
     { id = "BTC", alt = "WBTC" },
     { id = "ETH", alt = "WETH" },
 ]
-
+ignore_instrument = "US500 USTEC DOGE"
 
 
 [testing]
 VALUE = "On Testing"
 findmyorder_enabled = true
 action_identifier = "BUY SELL LONG SHORT"
 actions = [
```

### Comparing `findmyorder-1.5.9/findmyorder/main.py` & `findmyorder-1.6.0/findmyorder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,24 +93,27 @@
             return e
 
     async def get_order(
         self,
         msg: str,
     ):
         """get an order."""
-        if await self.search(msg):
-            order = await self.identify_order(msg)
-            if isinstance(order, dict):
-                order["timestamp"] = datetime.utcnow().strftime(
-                    "%Y-%m-%dT%H:%M:%SZ")
-            print(settings.instrument_mapping)
-            if settings.instrument_mapping:
-                await self.replace_instrument(order)
-            return order
-        return None
+        if not await self.search(msg):
+            return None
+        order = await self.identify_order(msg)
+        if isinstance(order, dict):
+            order["timestamp"] = datetime.utcnow().strftime(
+                "%Y-%m-%dT%H:%M:%SZ")
+        print(settings.instrument_mapping)
+        if settings.instrument_mapping:
+            await self.replace_instrument(order)
+        if order["instrument"] in settings.ignore_instrument:
+            """ ignoring instrument"""
+            return
+        return order
 
     async def replace_instrument(self, order):
         """ replace instrument by an alternative instrument """
         instrument = order["instrument"]
         for item in settings.mapping:
             if item["id"] == instrument:
                 order["instrument"] = item["alt"]
```

### Comparing `findmyorder-1.5.9/pyproject.toml` & `findmyorder-1.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.5.9"
+version = "1.6.0"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -43,16 +43,16 @@
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.0.0"
 sphinx_bootstrap_theme = "^0.8.1"
 sphinx-autoapi = "^2.1.1"
 sphinx-copybutton= "^0.5.2"
 myst-parser = "^2.0.0"
 sphinx-notfound-page = "^0.8.3"
-seed_intersphinx_mapping = "^1.2.1"
-
+sphinxext-remoteliteralinclude = "^0.4.0"
+sphinx-togglebutton = "*"
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
```

### Comparing `findmyorder-1.5.9/PKG-INFO` & `findmyorder-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.5.9
+Version: 1.6.0
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,15 @@
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/v/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/dm/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://github.com/mraniki/findmyorder"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/findmyorder/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
-   <a href="https://talkyuniverse.readthedocs.io/projects/fyndmyorder/"><img src="https://readthedocs.org/projects/talkytrend/badge/?version=latest&style=for-the-badge"></a><br>
+   <a href="https://talky.readthedocs.io/projects/findmyorder/index.html"><img src="https://readthedocs.org/projects/findmyorder/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-findmyorder-main"><img src="https://codebeat.co/badges/9b113098-d22d-498d-9c61-eb1e96c1311a"/></a><br>
    <a href="https://codecov.io/gh/mraniki/findmyorder"><img src="https://codecov.io/gh/mraniki/findmyorder/branch/main/graph/badge.svg?token=4838MSZNCC"/> </a><br>
     </td>
      <td align="left"> 
         Find My order,<br>
        a parsing package to find trading order
      </td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.5.9 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.6.0 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist:
@@ -26,15 +26,15 @@
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/findmyorder?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/github/actions/workflow/status/
 mraniki/findmyorder/                                        Find My order,
 %F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-  a parsing package
 the-badge&logo=GitHub&logoColor=white]                      to find trading
-[https://readthedocs.org/projects/talkytrend/badge/         order
+[https://readthedocs.org/projects/findmyorder/badge/        order
 ?version=latest&style=for-the-badge]
 [https://codebeat.co/badges/9b113098-d22d-498d-9c61-
 eb1e96c1311a]
 [https://codecov.io/gh/mraniki/findmyorder/branch/main/
 graph/badge.svg?token=4838MSZNCC]
 ** How to use it **
```

