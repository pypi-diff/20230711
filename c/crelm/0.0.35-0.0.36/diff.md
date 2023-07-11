# Comparing `tmp/crelm-0.0.35.tar.gz` & `tmp/crelm-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crelm-0.0.35.tar", max compression
+gzip compressed data, was "crelm-0.0.36.tar", max compression
```

## Comparing `crelm-0.0.35.tar` & `crelm-0.0.36.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1108 2023-05-03 17:25:38.782803 crelm-0.0.35/LICENSE
--rw-r--r--   0        0        0      600 2023-05-03 17:25:38.782803 crelm-0.0.35/README.md
--rw-r--r--   0        0        0      187 2023-05-03 17:25:38.782803 crelm-0.0.35/crelm/__init__.py
--rw-r--r--   0        0        0     3071 2023-05-14 14:20:50.777933 crelm-0.0.35/crelm/factory.py
--rw-r--r--   0        0        0      388 2023-05-13 18:12:40.800567 crelm-0.0.35/crelm/libcrelm.py
--rw-r--r--   0        0        0   107326 2023-05-03 17:25:38.784803 crelm-0.0.35/crelm/makeheaders.c
--rw-r--r--   0        0        0     1987 2023-05-03 17:25:38.784803 crelm-0.0.35/crelm/makeheaders_crelm.c
--rw-r--r--   0        0        0    15200 2023-06-15 19:32:10.157880 crelm-0.0.35/crelm/tube.py
--rw-r--r--   0        0        0      776 2023-06-15 19:37:49.788553 crelm-0.0.35/pyproject.toml
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 crelm-0.0.35/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:38.782803 crelm-0.0.36/LICENSE
+-rw-r--r--   0        0        0      600 2023-05-03 17:25:38.782803 crelm-0.0.36/README.md
+-rw-r--r--   0        0        0      187 2023-05-03 17:25:38.782803 crelm-0.0.36/crelm/__init__.py
+-rw-r--r--   0        0        0     3071 2023-05-14 14:20:50.777933 crelm-0.0.36/crelm/factory.py
+-rw-r--r--   0        0        0      388 2023-05-13 18:12:40.800567 crelm-0.0.36/crelm/libcrelm.py
+-rw-r--r--   0        0        0   107326 2023-05-03 17:25:38.784803 crelm-0.0.36/crelm/makeheaders.c
+-rw-r--r--   0        0        0     1987 2023-05-03 17:25:38.784803 crelm-0.0.36/crelm/makeheaders_crelm.c
+-rw-r--r--   0        0        0    15229 2023-07-11 16:31:02.092025 crelm-0.0.36/crelm/tube.py
+-rw-r--r--   0        0        0      776 2023-07-11 16:39:05.949566 crelm-0.0.36/pyproject.toml
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 crelm-0.0.36/PKG-INFO
```

### Comparing `crelm-0.0.35/LICENSE` & `crelm-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `crelm-0.0.35/README.md` & `crelm-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `crelm-0.0.35/crelm/factory.py` & `crelm-0.0.36/crelm/factory.py`

 * *Files identical despite different names*

### Comparing `crelm-0.0.35/crelm/makeheaders.c` & `crelm-0.0.36/crelm/makeheaders.c`

 * *Files identical despite different names*

### Comparing `crelm-0.0.35/crelm/makeheaders_crelm.c` & `crelm-0.0.36/crelm/makeheaders_crelm.c`

 * *Files identical despite different names*

### Comparing `crelm-0.0.35/crelm/tube.py` & `crelm-0.0.36/crelm/tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,16 +258,16 @@
                               library_dirs=[],
                               )
 
         try:
             self._lib_path = ffibuilder.compile(
                 tmpdir=self._gen_foldername,
                 verbose=self._verbose)
-        except:
-            print(f'{self._name}: Compilation failed')
+        except BaseException as arg:
+            print(f'{self._name}: Compilation failed ({arg})')
             return False
 
         if self._verbose:
             print(f'lib: {self._lib_path}')
 
         return True
```

### Comparing `crelm-0.0.35/pyproject.toml` & `crelm-0.0.36/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crelm"
-version = "0.0.35"
+version = "0.0.36"
 description = "Utility that automates turning simple C classes into Python objects"
 authors = [
   "WideOpenTech <foss@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `crelm-0.0.35/PKG-INFO` & `crelm-0.0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crelm
-Version: 0.0.35
+Version: 0.0.36
 Summary: Utility that automates turning simple C classes into Python objects
 Home-page: https://github.com/wideopensource/crelm
 Author: WideOpenTech
 Author-email: foss@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

