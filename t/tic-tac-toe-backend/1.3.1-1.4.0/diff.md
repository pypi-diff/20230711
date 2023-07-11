# Comparing `tmp/tic-tac-toe-backend-1.3.1.tar.gz` & `tmp/tic-tac-toe-backend-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tic-tac-toe-backend-1.3.1.tar", last modified: Sat Jul  8 01:51:48 2023, max compression
+gzip compressed data, was "tic-tac-toe-backend-1.4.0.tar", last modified: Tue Jul 11 01:45:25 2023, max compression
```

## Comparing `tic-tac-toe-backend-1.3.1.tar` & `tic-tac-toe-backend-1.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:51:48.010048 tic-tac-toe-backend-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-08 01:51:48.010048 tic-tac-toe-backend-1.3.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1530 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:51:48.010048 tic-tac-toe-backend-1.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1182 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:51:48.006048 tic-tac-toe-backend-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:51:48.010048 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-08 01:51:47.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-08 01:51:47.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:51:47.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-08 01:51:47.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 01:51:47.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:51:48.010048 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:51:48.010048 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:51:48.010048 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      474 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/operations/get_.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      481 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/operations/get_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/operations/put_games.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:51:48.010048 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2969 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/shared/move.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/shared/moveparameter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/shared/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5163 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:51:48.010048 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-08 01:51:37.000000 tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:45:25.148671 tic-tac-toe-backend-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-11 01:45:25.148671 tic-tac-toe-backend-1.4.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1530 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 01:45:25.148671 tic-tac-toe-backend-1.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1182 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:45:25.144671 tic-tac-toe-backend-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:45:25.144671 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-11 01:45:25.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-11 01:45:25.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 01:45:25.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 01:45:25.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 01:45:25.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:45:25.148671 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:45:25.148671 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:45:25.148671 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      474 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/operations/get_.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      481 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/operations/get_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/operations/put_games.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:45:25.148671 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2969 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/shared/move.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/shared/moveparameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/shared/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5163 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:45:25.148671 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-11 01:45:11.000000 tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/utils/utils.py
```

### Comparing `tic-tac-toe-backend-1.3.1/LICENSE.md` & `tic-tac-toe-backend-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.3.1/PKG-INFO` & `tic-tac-toe-backend-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tic-tac-toe-backend
-Version: 1.3.1
+Version: 1.4.0
 Summary: Tic Tac Toe Backend Python Client SDK
 Home-page: UNKNOWN
 Author: Shain Lafazan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `tic-tac-toe-backend-1.3.1/README.md` & `tic-tac-toe-backend-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.3.1/setup.py` & `tic-tac-toe-backend-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="tic-tac-toe-backend",
-    version="1.3.1",
+    version="1.4.0",
     author="Shain Lafazan",
     description="Tic Tac Toe Backend Python Client SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
```

### Comparing `tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backend.egg-info/PKG-INFO` & `tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backend.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tic-tac-toe-backend
-Version: 1.3.1
+Version: 1.4.0
 Summary: Tic Tac Toe Backend Python Client SDK
 Home-page: UNKNOWN
 Author: Shain Lafazan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backend.egg-info/SOURCES.txt` & `tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/shared/__init__.py` & `tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/models/shared/move.py` & `tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/models/shared/move.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/sdk.py` & `tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/sdk.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/sdkconfiguration.py` & `tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/sdkconfiguration.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 class SDKConfiguration:
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.0'
-    sdk_version: str = '1.3.1'
-    gen_version: str = '2.58.2'
+    sdk_version: str = '1.4.0'
+    gen_version: str = '2.61.0'
 
     def get_server_details(self) -> tuple[str, dict[str, str]]:
         if self.server_url:
             return self.server_url.removesuffix('/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/utils/retries.py` & `tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/utils/retries.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.3.1/src/tic_tac_toe_backends/utils/utils.py` & `tic-tac-toe-backend-1.4.0/src/tic_tac_toe_backends/utils/utils.py`

 * *Files identical despite different names*

