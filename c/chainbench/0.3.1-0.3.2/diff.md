# Comparing `tmp/chainbench-0.3.1.tar.gz` & `tmp/chainbench-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.3.1.tar", max compression
+gzip compressed data, was "chainbench-0.3.2.tar", max compression
```

## Comparing `chainbench-0.3.1.tar` & `chainbench-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-07-10 07:23:02.669200 chainbench-0.3.1/LICENSE
--rw-r--r--   0        0        0     8428 2023-07-10 07:23:02.669200 chainbench-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/__main__.py
--rw-r--r--   0        0        0     8401 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/main.py
--rw-r--r--   0        0        0        0 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3597 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/avalanche/general.py
--rw-r--r--   0        0        0     2693 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/bsc/general.py
--rw-r--r--   0        0        0     2912 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/ethereum/general.py
--rw-r--r--   0        0        0      361 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/evm/get_logs.py
--rw-r--r--   0        0        0     4158 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0     1645 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0     1838 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/oasis/general.py
--rw-r--r--   0        0        0     2845 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/profile/polygon/general.py
--rw-r--r--   0        0        0      168 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     4705 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/test_data/base.py
--rw-r--r--   0        0        0      166 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/test_data/dummy.py
--rw-r--r--   0        0        0     2979 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/test_data/evm.py
--rw-r--r--   0        0        0        0 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/user/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/user/base.py
--rw-r--r--   0        0        0     2740 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/user/evm.py
--rw-r--r--   0        0        0        0 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/__init__.py
--rw-r--r--   0        0        0     3907 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/cli.py
--rw-r--r--   0        0        0     2511 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/event.py
--rw-r--r--   0        0        0     3436 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/monitor.py
--rw-r--r--   0        0        0     3463 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/notify.py
--rw-r--r--   0        0        0      279 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/rpc.py
--rw-r--r--   0        0        0      438 2023-07-10 07:23:02.669200 chainbench-0.3.1/chainbench/util/timer.py
--rw-r--r--   0        0        0      771 2023-07-10 07:23:02.673200 chainbench-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8941 1970-01-01 00:00:00.000000 chainbench-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 08:05:25.229816 chainbench-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8428 2023-07-11 08:05:25.229816 chainbench-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/__main__.py
+-rw-r--r--   0        0        0     8401 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/main.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3597 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     2693 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     2912 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      361 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0     4158 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0     1645 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0     1838 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0     2845 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0      168 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     4705 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/test_data/base.py
+-rw-r--r--   0        0        0      166 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/test_data/dummy.py
+-rw-r--r--   0        0        0     2979 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/user/base.py
+-rw-r--r--   0        0        0     2740 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/user/evm.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     3907 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/cli.py
+-rw-r--r--   0        0        0     2511 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/event.py
+-rw-r--r--   0        0        0     3436 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/monitor.py
+-rw-r--r--   0        0        0     3463 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/notify.py
+-rw-r--r--   0        0        0      279 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      438 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/timer.py
+-rw-r--r--   0        0        0      895 2023-07-11 08:05:25.233816 chainbench-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9033 1970-01-01 00:00:00.000000 chainbench-0.3.2/PKG-INFO
```

### Comparing `chainbench-0.3.1/LICENSE` & `chainbench-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/README.md` & `chainbench-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/main.py` & `chainbench-0.3.2/chainbench/main.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/profile/avalanche/general.py` & `chainbench-0.3.2/chainbench/profile/avalanche/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/profile/bsc/general.py` & `chainbench-0.3.2/chainbench/profile/bsc/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/profile/ethereum/general.py` & `chainbench-0.3.2/chainbench/profile/ethereum/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/profile/evm/heavy.py` & `chainbench-0.3.2/chainbench/profile/evm/heavy.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/profile/evm/light.py` & `chainbench-0.3.2/chainbench/profile/evm/light.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/profile/oasis/general.py` & `chainbench-0.3.2/chainbench/profile/oasis/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/profile/polygon/general.py` & `chainbench-0.3.2/chainbench/profile/polygon/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/test_data/base.py` & `chainbench-0.3.2/chainbench/test_data/base.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/test_data/evm.py` & `chainbench-0.3.2/chainbench/test_data/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/user/base.py` & `chainbench-0.3.2/chainbench/user/base.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/user/evm.py` & `chainbench-0.3.2/chainbench/user/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/util/cli.py` & `chainbench-0.3.2/chainbench/util/cli.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/util/event.py` & `chainbench-0.3.2/chainbench/util/event.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/util/monitor.py` & `chainbench-0.3.2/chainbench/util/monitor.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/chainbench/util/notify.py` & `chainbench-0.3.2/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.1/pyproject.toml` & `chainbench-0.3.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
-authors = ["Egor Molodik <egor.molodik@chainstack.com>"]
+authors = [
+    "Egor Molodik <egor.molodik@chainstack.com>",
+    "Erwin Wee <erwin.wee@chainstack.com>"
+]
+maintainers = ["Erwin Wee <erwin.wee@chainstack.com>"]
 readme = "README.md"
 packages = [{include = "chainbench"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-httpx = "^0.24.0"
+httpx = "0.24.0"
 locust = "^2.15.0"
 click = "^8.1.3"
 locust-plugins = "^3.3.0"
+httpcore = "0.17.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.2.0"
 pre-commit = "^3.2.2"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
```

### Comparing `chainbench-0.3.1/PKG-INFO` & `chainbench-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
+Maintainer: Erwin Wee
+Maintainer-email: erwin.wee@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: httpcore (==0.17.0)
+Requires-Dist: httpx (==0.24.0)
 Requires-Dist: locust (>=2.15.0,<3.0.0)
 Requires-Dist: locust-plugins (>=3.3.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 <img width="1200" alt="Labs" src="https://user-images.githubusercontent.com/99700157/213291931-5a822628-5b8a-4768-980d-65f324985d32.png">
 
 <p>
```

