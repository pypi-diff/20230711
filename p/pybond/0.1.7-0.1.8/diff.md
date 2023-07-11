# Comparing `tmp/pybond-0.1.7.tar.gz` & `tmp/pybond-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybond-0.1.7.tar", max compression
+gzip compressed data, was "pybond-0.1.8.tar", max compression
```

## Comparing `pybond-0.1.7.tar` & `pybond-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3030 2023-05-15 00:09:42.242843 pybond-0.1.7/README.md
--rw-r--r--   0        0        0      385 2023-01-23 06:22:02.588103 pybond-0.1.7/pybond/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-14 22:59:40.370502 pybond-0.1.7/pybond/assertions.py
--rw-r--r--   0        0        0     5791 2023-05-15 00:09:42.147226 pybond-0.1.7/pybond/james.py
--rw-r--r--   0        0        0      633 2023-05-15 00:09:42.003420 pybond-0.1.7/pybond/memory.py
--rw-r--r--   0        0        0      400 2023-05-15 00:09:42.003950 pybond-0.1.7/pybond/types.py
--rw-r--r--   0        0        0     2017 2023-05-13 04:49:52.047150 pybond-0.1.7/pybond/util.py
--rw-r--r--   0        0        0      984 2023-05-15 00:09:42.243064 pybond-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 pybond-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3030 2023-07-11 19:28:18.644826 pybond-0.1.8/README.md
+-rw-r--r--   0        0        0      385 2023-01-23 06:22:02.588103 pybond-0.1.8/pybond/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-14 22:59:40.370502 pybond-0.1.8/pybond/assertions.py
+-rw-r--r--   0        0        0     5781 2023-07-11 19:28:18.645132 pybond-0.1.8/pybond/james.py
+-rw-r--r--   0        0        0      633 2023-05-15 00:58:17.181063 pybond-0.1.8/pybond/memory.py
+-rw-r--r--   0        0        0      400 2023-05-15 16:32:17.555194 pybond-0.1.8/pybond/types.py
+-rw-r--r--   0        0        0     2017 2023-05-15 16:32:17.555907 pybond-0.1.8/pybond/util.py
+-rw-r--r--   0        0        0      984 2023-07-11 19:28:18.645444 pybond-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 pybond-0.1.8/PKG-INFO
```

### Comparing `pybond-0.1.7/README.md` & `pybond-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 [clojure `bond` library](https://github.com/circleci/bond/).
 
 ## Installation
 
 pip
 
 ```bash
-pip install pybond==0.1.7
+pip install pybond==0.1.8
 ```
 
 requirements.txt
 
 ```python
-pybond==0.1.7
+pybond==0.1.8
 ```
 
 pyproject.toml
 
 ```toml
-pybond = "0.1.7"
+pybond = "0.1.8"
 ```
 
 ## Example usage
 
 Let's say you wanted to test the functions in this module:
 
 ```python
```

### Comparing `pybond-0.1.7/pybond/assertions.py` & `pybond-0.1.8/pybond/assertions.py`

 * *Files identical despite different names*

### Comparing `pybond-0.1.7/pybond/james.py` & `pybond-0.1.8/pybond/james.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,9 +185,9 @@
     ```
     import my_module
     with spy([my_module, "test_function"]):
         my_module.test_function("abc")
         function_calls = calls(my_module.test_function)
     ```
     """
-    with stub(*[(m, n, deepcopy(getattr(m, n))) for m, n in targets]):
+    with stub(*[(m, n, getattr(m, n)) for m, n in targets]):
         yield
```

### Comparing `pybond-0.1.7/pybond/memory.py` & `pybond-0.1.8/pybond/memory.py`

 * *Files identical despite different names*

### Comparing `pybond-0.1.7/pybond/util.py` & `pybond-0.1.8/pybond/util.py`

 * *Files identical despite different names*

### Comparing `pybond-0.1.7/pyproject.toml` & `pybond-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybond"
-version = "0.1.7"
+version = "0.1.8"
 description = "pybond is a spying and stubbing library inspired by the clojure bond library."
 authors = ["Guillaume Pelletier <guigui.p@gmail.com>"]
 license = "Eclipse Public License - v 1.0"
 readme = "README.md"
 homepage = "https://github.com/epgui/pybond"
 repository = "https://github.com/epgui/pybond"
 keywords = [
```

### Comparing `pybond-0.1.7/PKG-INFO` & `pybond-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybond
-Version: 0.1.7
+Version: 0.1.8
 Summary: pybond is a spying and stubbing library inspired by the clojure bond library.
 Home-page: https://github.com/epgui/pybond
 License: Eclipse Public License - v 1.0
 Keywords: bond,monkeypatch,spy,stub,clojure,functional programming
 Author: Guillaume Pelletier
 Author-email: guigui.p@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -30,27 +30,27 @@
 [clojure `bond` library](https://github.com/circleci/bond/).
 
 ## Installation
 
 pip
 
 ```bash
-pip install pybond==0.1.7
+pip install pybond==0.1.8
 ```
 
 requirements.txt
 
 ```python
-pybond==0.1.7
+pybond==0.1.8
 ```
 
 pyproject.toml
 
 ```toml
-pybond = "0.1.7"
+pybond = "0.1.8"
 ```
 
 ## Example usage
 
 Let's say you wanted to test the functions in this module:
 
 ```python
```

