# Comparing `tmp/yaccounts-1.1.6.tar.gz` & `tmp/yaccounts-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaccounts-1.1.6.tar", last modified: Mon Jul 10 22:37:10 2023, max compression
+gzip compressed data, was "yaccounts-1.1.7.tar", last modified: Tue Jul 11 04:09:10 2023, max compression
```

## Comparing `yaccounts-1.1.6.tar` & `yaccounts-1.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:37:10.310799 yaccounts-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 22:37:10.310799 yaccounts-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 22:37:10.310799 yaccounts-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 22:36:48.000000 yaccounts-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:37:10.310799 yaccounts-1.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-10 22:36:48.000000 yaccounts-1.1.6/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:37:10.310799 yaccounts-1.1.6/yaccounts/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/operating_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/workbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/worksheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:37:10.310799 yaccounts-1.1.6/yaccounts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 22:37:10.000000 yaccounts-1.1.6/yaccounts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-10 22:37:10.000000 yaccounts-1.1.6/yaccounts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:37:10.000000 yaccounts-1.1.6/yaccounts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 22:37:10.000000 yaccounts-1.1.6/yaccounts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 22:37:10.000000 yaccounts-1.1.6/yaccounts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:09:10.365062 yaccounts-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 04:09:10.365062 yaccounts-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:09:10.365062 yaccounts-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 04:08:48.000000 yaccounts-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:09:10.365062 yaccounts-1.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-11 04:08:48.000000 yaccounts-1.1.7/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:09:10.365062 yaccounts-1.1.7/yaccounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/operating_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/workbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/worksheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:09:10.365062 yaccounts-1.1.7/yaccounts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 04:09:10.000000 yaccounts-1.1.7/yaccounts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-11 04:09:10.000000 yaccounts-1.1.7/yaccounts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:09:10.000000 yaccounts-1.1.7/yaccounts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 04:09:10.000000 yaccounts-1.1.7/yaccounts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 04:09:10.000000 yaccounts-1.1.7/yaccounts.egg-info/top_level.txt
```

### Comparing `yaccounts-1.1.6/test/test.py` & `yaccounts-1.1.7/test/test.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.6/yaccounts/config.py` & `yaccounts-1.1.7/yaccounts/config.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.6/yaccounts/operating_unit.py` & `yaccounts-1.1.7/yaccounts/operating_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         worksheet,
         operating_unit,
         year,
         name=None,
         budgeted_account=None,
     ) -> None:
         self.worksheet = worksheet
-        self.operating_unit = operating_unit
+        self.operating_unit = str(operating_unit)
         self.name = name
         self.year = year
 
         if budgeted_account is None:
             self.budgeted_account = operating_unit.startswith("R")
         else:
             self.budgeted_account = budgeted_account
```

### Comparing `yaccounts-1.1.6/yaccounts/workbook.py` & `yaccounts-1.1.7/yaccounts/workbook.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.6/yaccounts/worksheet.py` & `yaccounts-1.1.7/yaccounts/worksheet.py`

 * *Files identical despite different names*

