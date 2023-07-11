# Comparing `tmp/bondzai.davinsy-py-0.0.5.tar.gz` & `tmp/bondzai.davinsy-py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.davinsy-py-0.0.5.tar", last modified: Mon Jul 10 17:59:10 2023, max compression
+gzip compressed data, was "bondzai.davinsy-py-0.0.6.tar", last modified: Tue Jul 11 18:21:52 2023, max compression
```

## Comparing `bondzai.davinsy-py-0.0.5.tar` & `bondzai.davinsy-py-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:10.537632 bondzai.davinsy-py-0.0.5/
--rwxrwxrwx   0 root         (0) root         (0)      547 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/NOTICE
--rwxrwxrwx   0 root         (0) root         (0)      491 2023-07-10 17:59:10.538632 bondzai.davinsy-py-0.0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:09.990473 bondzai.davinsy-py-0.0.5/bondzai/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:10.324985 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/
--rwxrwxrwx   0 root         (0) root         (0)       24 2023-07-10 17:58:59.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3989 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/davinsy.py
--rwxrwxrwx   0 root         (0) root         (0)     6693 2023-07-10 17:58:59.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/enums.py
--rwxrwxrwx   0 root         (0) root         (0)      333 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/logger.py
--rwxrwxrwx   0 root         (0) root         (0)    21765 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/model.py
--rwxrwxrwx   0 root         (0) root         (0)    24433 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/operations.py
--rwxrwxrwx   0 root         (0) root         (0)     3346 2023-07-10 17:58:59.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/preproc.py
--rwxrwxrwx   0 root         (0) root         (0)     1034 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:10.513627 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      491 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      591 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)       26 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 17:59:09.000000 bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-07-10 17:56:52.000000 bondzai.davinsy-py-0.0.5/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      700 2023-07-10 17:59:10.543147 bondzai.davinsy-py-0.0.5/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:21:52.695822 bondzai.davinsy-py-0.0.6/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      491 2023-07-11 18:21:52.696174 bondzai.davinsy-py-0.0.6/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)       72 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:21:52.679568 bondzai.davinsy-py-0.0.6/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:21:52.689847 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/
+-rw-r--r--   0 theo       (501) staff       (20)       24 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     3989 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/davinsy.py
+-rw-r--r--   0 theo       (501) staff       (20)     7213 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/enums.py
+-rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/logger.py
+-rw-r--r--   0 theo       (501) staff       (20)    21765 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/model.py
+-rw-r--r--   0 theo       (501) staff       (20)    24433 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/operations.py
+-rw-r--r--   0 theo       (501) staff       (20)     3346 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/preproc.py
+-rw-r--r--   0 theo       (501) staff       (20)     1034 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/utils.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:21:52.695258 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      491 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      591 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       26 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-11 18:21:52.698365 bondzai.davinsy-py-0.0.6/setup.cfg
```

### Comparing `bondzai.davinsy-py-0.0.5/NOTICE` & `bondzai.davinsy-py-0.0.6/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/davinsy.py` & `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/davinsy.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/enums.py` & `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -259,7 +259,28 @@
     KPI_SIZE_BYTE = 17
     KPI_SIZE_KBYTE = 18
     KPI_QI = 19
     KPI_OTHER_FLOAT = 20
     KPI_TRAINING_NET_LAYERS = 21
 
 
+class RUNCommandParameter(Enum):
+    RUN_PARAM_BREAK = 0x0100
+    RUN_PARAM_APPS = 0x0200
+    RUN_PARAM_OPS = 0x0300
+
+
+class MALCommandParameter(Enum):
+    MAL_PARAM_NB_THREADS = 0x0100
+    MAL_PARAM_DATA_SOURCES = 0x0200
+    MAL_PARAM_LIFE_CYCLE = 0x0300
+    MAL_PARAM_NVM_FILE = 0x8100
+    MAL_PARAM_CLEAR_NVM = 0x8200
+    MAL_PARAM_MONITORING = 0x2000
+
+
+class BLDCommandParameter(Enum):
+    BLD_PARAM_LINUX_LIB_NAMES = 0x8000
+    BLD_PARAM_LINUX_PYTHON_SCRIPT_NAME = 0x8001
+    BLD_PARAM_CORTEXM_INIT_DONE = 0x8002
+
+
```

### Comparing `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/model.py` & `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/model.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/operations.py` & `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/operations.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/preproc.py` & `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/preproc.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.5/bondzai/davinsy_py/utils.py` & `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.5/bondzai.davinsy_py.egg-info/SOURCES.txt` & `bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.5/setup.cfg` & `bondzai.davinsy-py-0.0.6/setup.cfg`

 * *Files identical despite different names*

