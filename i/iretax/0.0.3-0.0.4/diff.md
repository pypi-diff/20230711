# Comparing `tmp/iretax-0.0.3.tar.gz` & `tmp/iretax-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iretax-0.0.3.tar", last modified: Tue Jul 11 07:36:16 2023, max compression
+gzip compressed data, was "iretax-0.0.4.tar", last modified: Tue Jul 11 09:06:34 2023, max compression
```

## Comparing `iretax-0.0.3.tar` & `iretax-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 07:36:16.985349 iretax-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-07-10 16:57:31.000000 iretax-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    12292 2023-07-11 07:36:16.983346 iretax-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    11777 2023-07-11 07:31:01.000000 iretax-0.0.3/README.md
--rw-rw-rw-   0        0        0      601 2023-07-11 07:35:15.000000 iretax-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 07:36:16.986347 iretax-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 07:36:16.932428 iretax-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 07:36:16.973344 iretax-0.0.3/src/Iretax.egg-info/
--rw-rw-rw-   0        0        0    12292 2023-07-11 07:36:16.000000 iretax-0.0.3/src/Iretax.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-07-11 07:36:16.000000 iretax-0.0.3/src/Iretax.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 07:36:16.000000 iretax-0.0.3/src/Iretax.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 07:36:16.000000 iretax-0.0.3/src/Iretax.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 07:36:16.978346 iretax-0.0.3/src/iretax/
--rw-rw-rw-   0        0        0       92 2023-07-10 08:47:50.000000 iretax-0.0.3/src/iretax/__init__.py
--rw-rw-rw-   0        0        0     2918 2023-07-10 08:44:23.000000 iretax-0.0.3/src/iretax/rebate_calculator.py
--rw-rw-rw-   0        0        0     2172 2023-07-10 16:31:46.000000 iretax-0.0.3/src/iretax/tax_calculator.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:36:16.981345 iretax-0.0.3/tests/
--rw-rw-rw-   0        0        0     1105 2023-07-10 09:47:29.000000 iretax-0.0.3/tests/test_rebate_calculator.py
--rw-rw-rw-   0        0        0     1083 2023-07-10 16:36:53.000000 iretax-0.0.3/tests/test_tax_calculator.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:06:34.139211 iretax-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-07-10 16:57:31.000000 iretax-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    12253 2023-07-11 09:06:34.138205 iretax-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11738 2023-07-11 09:05:01.000000 iretax-0.0.4/README.md
+-rw-rw-rw-   0        0        0      601 2023-07-11 09:05:07.000000 iretax-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 09:06:34.139211 iretax-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 09:06:34.088010 iretax-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 09:06:34.125008 iretax-0.0.4/src/Iretax.egg-info/
+-rw-rw-rw-   0        0        0    12253 2023-07-11 09:06:34.000000 iretax-0.0.4/src/Iretax.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-07-11 09:06:34.000000 iretax-0.0.4/src/Iretax.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 09:06:34.000000 iretax-0.0.4/src/Iretax.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 09:06:34.000000 iretax-0.0.4/src/Iretax.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 09:06:34.132702 iretax-0.0.4/src/iretax/
+-rw-rw-rw-   0        0        0       92 2023-07-10 08:47:50.000000 iretax-0.0.4/src/iretax/__init__.py
+-rw-rw-rw-   0        0        0     2918 2023-07-10 08:44:23.000000 iretax-0.0.4/src/iretax/rebate_calculator.py
+-rw-rw-rw-   0        0        0     2172 2023-07-10 16:31:46.000000 iretax-0.0.4/src/iretax/tax_calculator.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:06:34.137209 iretax-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1105 2023-07-10 09:47:29.000000 iretax-0.0.4/tests/test_rebate_calculator.py
+-rw-rw-rw-   0        0        0     1083 2023-07-10 16:36:53.000000 iretax-0.0.4/tests/test_tax_calculator.py
```

### Comparing `iretax-0.0.3/LICENSE` & `iretax-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iretax-0.0.3/PKG-INFO` & `iretax-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iretax
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Tax Calculation and Rebate System
 Author-email: Shubham Goswami <goswamis@tcd.ie>
 Project-URL: Homepage, https://github.com/ShubhZ33/iretax
 Project-URL: Bug Tracker, https://github.com/ShubhZ33/iretax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 
 
 ## Installation
 
 The iretax package can be easily installed from TestPyPI by running the following command:
 
 ```shell
-pip install -i https://test.pypi.org/simple/iretax==0.0.2
+pip install iretax
 ```
 
 Usage
 =====
 
 Tax Calculator
 --------------
```

### Comparing `iretax-0.0.3/README.md` & `iretax-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 ## Installation
 
 The iretax package can be easily installed from TestPyPI by running the following command:
 
 ```shell
-pip install -i https://test.pypi.org/simple/iretax==0.0.2
+pip install iretax
 ```
 
 Usage
 =====
 
 Tax Calculator
 --------------
```

### Comparing `iretax-0.0.3/pyproject.toml` & `iretax-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iretax"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Shubham Goswami", email="goswamis@tcd.ie" },
 ]
 description = "A Tax Calculation and Rebate System"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `iretax-0.0.3/src/Iretax.egg-info/PKG-INFO` & `iretax-0.0.4/src/Iretax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iretax
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Tax Calculation and Rebate System
 Author-email: Shubham Goswami <goswamis@tcd.ie>
 Project-URL: Homepage, https://github.com/ShubhZ33/iretax
 Project-URL: Bug Tracker, https://github.com/ShubhZ33/iretax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 
 
 ## Installation
 
 The iretax package can be easily installed from TestPyPI by running the following command:
 
 ```shell
-pip install -i https://test.pypi.org/simple/iretax==0.0.2
+pip install iretax
 ```
 
 Usage
 =====
 
 Tax Calculator
 --------------
```

### Comparing `iretax-0.0.3/src/iretax/rebate_calculator.py` & `iretax-0.0.4/src/iretax/rebate_calculator.py`

 * *Files identical despite different names*

### Comparing `iretax-0.0.3/src/iretax/tax_calculator.py` & `iretax-0.0.4/src/iretax/tax_calculator.py`

 * *Files identical despite different names*

### Comparing `iretax-0.0.3/tests/test_rebate_calculator.py` & `iretax-0.0.4/tests/test_rebate_calculator.py`

 * *Files identical despite different names*

### Comparing `iretax-0.0.3/tests/test_tax_calculator.py` & `iretax-0.0.4/tests/test_tax_calculator.py`

 * *Files identical despite different names*

