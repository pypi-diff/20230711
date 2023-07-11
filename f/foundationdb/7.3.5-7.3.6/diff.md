# Comparing `tmp/foundationdb-7.3.5.tar.gz` & `tmp/foundationdb-7.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/foundationdb-7.3.5.tar", last modified: Sat Jun 17 22:43:56 2023, max compression
+gzip compressed data, was "dist/foundationdb-7.3.6.tar", last modified: Tue Jul 11 01:45:35 2023, max compression
```

## Comparing `foundationdb-7.3.5.tar` & `foundationdb-7.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-06-17 22:43:56.000000 foundationdb-7.3.5/
-drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-06-17 22:43:56.000000 foundationdb-7.3.5/fdb/
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1913 2023-06-17 17:07:30.000000 foundationdb-7.3.5/fdb/subspace_impl.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    30888 2023-06-17 17:07:30.000000 foundationdb-7.3.5/fdb/six.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)       25 2023-06-17 16:42:29.000000 foundationdb-7.3.5/fdb/apiversion.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    21791 2023-06-17 17:07:30.000000 foundationdb-7.3.5/fdb/tuple.py
--rwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    26547 2023-06-17 17:07:30.000000 foundationdb-7.3.5/fdb/directory_impl.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     4811 2023-06-17 17:07:30.000000 foundationdb-7.3.5/fdb/__init__.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     5842 2023-06-17 17:07:30.000000 foundationdb-7.3.5/fdb/tenant_management.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     2814 2023-06-17 17:07:30.000000 foundationdb-7.3.5/fdb/locality.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    38989 2023-06-17 16:44:43.000000 foundationdb-7.3.5/fdb/fdboptions.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    66069 2023-06-17 17:07:30.000000 foundationdb-7.3.5/fdb/impl.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)      252 2023-06-17 17:07:30.000000 foundationdb-7.3.5/README.rst
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1434 2023-06-17 22:43:56.000000 foundationdb-7.3.5/PKG-INFO
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1416 2023-06-17 16:42:29.000000 foundationdb-7.3.5/setup.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    11665 2023-06-17 16:42:29.000000 foundationdb-7.3.5/LICENSE
+drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-07-11 01:45:35.000000 foundationdb-7.3.6/
+drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-07-11 01:45:35.000000 foundationdb-7.3.6/fdb/
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1913 2023-06-17 17:07:30.000000 foundationdb-7.3.6/fdb/subspace_impl.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    30888 2023-06-17 17:07:30.000000 foundationdb-7.3.6/fdb/six.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)       25 2023-06-17 16:42:29.000000 foundationdb-7.3.6/fdb/apiversion.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    21791 2023-07-10 19:24:21.000000 foundationdb-7.3.6/fdb/tuple.py
+-rwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    26547 2023-06-17 17:07:30.000000 foundationdb-7.3.6/fdb/directory_impl.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     4811 2023-07-10 19:24:21.000000 foundationdb-7.3.6/fdb/__init__.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     5842 2023-06-17 17:07:30.000000 foundationdb-7.3.6/fdb/tenant_management.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     2814 2023-06-17 17:07:30.000000 foundationdb-7.3.6/fdb/locality.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    38989 2023-07-10 19:24:21.000000 foundationdb-7.3.6/fdb/fdboptions.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    66069 2023-07-10 19:24:21.000000 foundationdb-7.3.6/fdb/impl.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)      252 2023-06-17 17:07:30.000000 foundationdb-7.3.6/README.rst
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1434 2023-07-11 01:45:35.000000 foundationdb-7.3.6/PKG-INFO
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1416 2023-07-10 19:22:25.000000 foundationdb-7.3.6/setup.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    11665 2023-06-17 16:42:29.000000 foundationdb-7.3.6/LICENSE
```

### Comparing `foundationdb-7.3.5/fdb/subspace_impl.py` & `foundationdb-7.3.6/fdb/subspace_impl.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.5/fdb/six.py` & `foundationdb-7.3.6/fdb/six.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.5/fdb/tuple.py` & `foundationdb-7.3.6/fdb/tuple.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.5/fdb/directory_impl.py` & `foundationdb-7.3.6/fdb/directory_impl.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.5/fdb/__init__.py` & `foundationdb-7.3.6/fdb/__init__.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.5/fdb/tenant_management.py` & `foundationdb-7.3.6/fdb/tenant_management.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.5/fdb/locality.py` & `foundationdb-7.3.6/fdb/locality.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.5/fdb/fdboptions.py` & `foundationdb-7.3.6/fdb/fdboptions.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.5/fdb/impl.py` & `foundationdb-7.3.6/fdb/impl.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.5/PKG-INFO` & `foundationdb-7.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: foundationdb
-Version: 7.3.5
+Version: 7.3.6
 Summary: Python bindings for the FoundationDB database
 Home-page: https://www.foundationdb.org
 Author: FoundationDB
 Author-email: fdb-dist@apple.com
 License: UNKNOWN
 Description: Complete documentation of the FoundationDB Python API can be found at https://apple.github.io/foundationdb/api-python.html.
```

### Comparing `foundationdb-7.3.5/setup.py` & `foundationdb-7.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     with open("README.rst") as f:
         long_desc = f.read()
 except:
     long_desc = ""
 
 setup(name="foundationdb",
-      version="7.3.5",
+      version="7.3.6",
       author="FoundationDB",
       author_email="fdb-dist@apple.com",
       description="Python bindings for the FoundationDB database",
       url="https://www.foundationdb.org",
       packages=['fdb'],
       package_data={'fdb': ["fdb/*.py"]},
       long_description=long_desc,
```

### Comparing `foundationdb-7.3.5/LICENSE` & `foundationdb-7.3.6/LICENSE`

 * *Files identical despite different names*

