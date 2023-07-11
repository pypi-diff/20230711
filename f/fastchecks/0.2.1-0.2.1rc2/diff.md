# Comparing `tmp/fastchecks-0.2.1.tar.gz` & `tmp/fastchecks-0.2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchecks-0.2.1.tar", max compression
+gzip compressed data, was "fastchecks-0.2.1rc2.tar", max compression
```

## Comparing `fastchecks-0.2.1.tar` & `fastchecks-0.2.1rc2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-07-11 10:41:01.033771 fastchecks-0.2.1/LICENSE
--rw-r--r--   0        0        0     5034 2023-07-11 12:00:38.559491 fastchecks-0.2.1/README.md
--rw-r--r--   0        0        0      569 2023-07-11 10:41:01.034019 fastchecks-0.2.1/fastchecks/NOTICE
--rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.2.1/fastchecks/__init__.py
--rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.2.1/fastchecks/check.py
--rw-r--r--   0        0        0    12259 2023-07-11 12:00:38.514751 fastchecks-0.2.1/fastchecks/cli.py
--rw-r--r--   0        0        0     3165 2023-07-11 12:00:38.515268 fastchecks-0.2.1/fastchecks/conf.py
--rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.2.1/fastchecks/log.py
--rw-r--r--   0        0        0      892 2023-07-11 10:41:00.994931 fastchecks-0.2.1/fastchecks/meta.py
--rw-r--r--   0        0        0     6992 2023-07-11 11:36:08.255245 fastchecks-0.2.1/fastchecks/runner.py
--rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.2.1/fastchecks/sockets/__init__.py
--rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.2.1/fastchecks/sockets/postgres/__init__.py
--rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.2.1/fastchecks/sockets/postgres/schema/down.sql
--rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.2.1/fastchecks/sockets/postgres/schema/up.sql
--rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.2.1/fastchecks/types.py
--rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.2.1/fastchecks/util.py
--rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.2.1/fastchecks/vutil.py
--rw-r--r--   0        0        0     1974 2023-07-11 12:04:53.497078 fastchecks-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5705 1970-01-01 00:00:00.000000 fastchecks-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 10:41:01.033771 fastchecks-0.2.1rc2/LICENSE
+-rw-r--r--   0        0        0     5033 2023-07-11 11:48:52.604708 fastchecks-0.2.1rc2/README.md
+-rw-r--r--   0        0        0      569 2023-07-11 10:41:01.034019 fastchecks-0.2.1rc2/fastchecks/NOTICE
+-rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.2.1rc2/fastchecks/__init__.py
+-rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.2.1rc2/fastchecks/check.py
+-rw-r--r--   0        0        0    12259 2023-07-11 11:48:52.605005 fastchecks-0.2.1rc2/fastchecks/cli.py
+-rw-r--r--   0        0        0     3165 2023-07-11 11:48:52.605178 fastchecks-0.2.1rc2/fastchecks/conf.py
+-rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.2.1rc2/fastchecks/log.py
+-rw-r--r--   0        0        0      892 2023-07-11 10:41:00.994931 fastchecks-0.2.1rc2/fastchecks/meta.py
+-rw-r--r--   0        0        0     6992 2023-07-11 11:36:08.255245 fastchecks-0.2.1rc2/fastchecks/runner.py
+-rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.2.1rc2/fastchecks/sockets/__init__.py
+-rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.2.1rc2/fastchecks/sockets/postgres/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/down.sql
+-rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/up.sql
+-rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.2.1rc2/fastchecks/types.py
+-rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.2.1rc2/fastchecks/util.py
+-rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.2.1rc2/fastchecks/vutil.py
+-rw-r--r--   0        0        0     1978 2023-07-11 11:49:32.742553 fastchecks-0.2.1rc2/pyproject.toml
+-rw-r--r--   0        0        0     5707 1970-01-01 00:00:00.000000 fastchecks-0.2.1rc2/PKG-INFO
```

### Comparing `fastchecks-0.2.1/LICENSE` & `fastchecks-0.2.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/README.md` & `fastchecks-0.2.1rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,23 +39,23 @@
 * Further type checking with Pydantic (v2).
 * Further static analysis with pyflakes.
 
 
 
 ## Install
 
-### Via pip
+### With pip
 
 ```shell
 # You need to run this with a Python 3.11 environment -- You can manage different python versions for instance with `pyenv`
 pip install -U fastchecks
 ```
 
 
-### or via source
+### From source
 
 You need to have [python poetry](https://python-poetry.org/docs/) installed. Then:
 
 ```shell
 # clone this repository
 _reponame="fastchecks";
 _branch="main";
```

### Comparing `fastchecks-0.2.1/fastchecks/NOTICE` & `fastchecks-0.2.1rc2/fastchecks/NOTICE`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/__init__.py` & `fastchecks-0.2.1rc2/fastchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/check.py` & `fastchecks-0.2.1rc2/fastchecks/check.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/cli.py` & `fastchecks-0.2.1rc2/fastchecks/cli.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/conf.py` & `fastchecks-0.2.1rc2/fastchecks/conf.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/log.py` & `fastchecks-0.2.1rc2/fastchecks/log.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/meta.py` & `fastchecks-0.2.1rc2/fastchecks/meta.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/runner.py` & `fastchecks-0.2.1rc2/fastchecks/runner.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/sockets/__init__.py` & `fastchecks-0.2.1rc2/fastchecks/sockets/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/sockets/postgres/__init__.py` & `fastchecks-0.2.1rc2/fastchecks/sockets/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/sockets/postgres/schema/down.sql` & `fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/down.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/sockets/postgres/schema/up.sql` & `fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/up.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/types.py` & `fastchecks-0.2.1rc2/fastchecks/types.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/util.py` & `fastchecks-0.2.1rc2/fastchecks/util.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/fastchecks/vutil.py` & `fastchecks-0.2.1rc2/fastchecks/vutil.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1/pyproject.toml` & `fastchecks-0.2.1rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastchecks"
-version = "0.2.1"
+version = "0.2.1-rc2"
 description = "🚥 Fast website monitoring backend service"
 authors = ["Dr. Juan Miguel Cejuela <i@juanmi.rocks>"]
 readme = "README.md"
 repository = "https://github.com/juanmirocks/fastchecks"
 packages = [{ include = "fastchecks" }]
```

### Comparing `fastchecks-0.2.1/PKG-INFO` & `fastchecks-0.2.1rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastchecks
-Version: 0.2.1
+Version: 0.2.1rc2
 Summary: 🚥 Fast website monitoring backend service
 Home-page: https://github.com/juanmirocks/fastchecks
 Author: Dr. Juan Miguel Cejuela
 Author-email: i@juanmi.rocks
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -57,23 +57,23 @@
 * Further type checking with Pydantic (v2).
 * Further static analysis with pyflakes.
 
 
 
 ## Install
 
-### Via pip
+### With pip
 
 ```shell
 # You need to run this with a Python 3.11 environment -- You can manage different python versions for instance with `pyenv`
 pip install -U fastchecks
 ```
 
 
-### or via source
+### From source
 
 You need to have [python poetry](https://python-poetry.org/docs/) installed. Then:
 
 ```shell
 # clone this repository
 _reponame="fastchecks";
 _branch="main";
```

