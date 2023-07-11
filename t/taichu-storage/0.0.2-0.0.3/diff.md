# Comparing `tmp/taichu-storage-0.0.2.tar.gz` & `tmp/taichu-storage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-storage-0.0.2.tar", last modified: Tue Jul 11 02:00:49 2023, max compression
+gzip compressed data, was "taichu-storage-0.0.3.tar", last modified: Tue Jul 11 02:44:38 2023, max compression
```

## Comparing `taichu-storage-0.0.2.tar` & `taichu-storage-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:00:49.770481 taichu-storage-0.0.2/
--rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 02:00:49.770224 taichu-storage-0.0.2/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-07-11 02:00:49.770574 taichu-storage-0.0.2/setup.cfg
--rw-r--r--   0 wangkun    (501) staff       (20)      730 2023-07-10 11:04:28.000000 taichu-storage-0.0.2/setup.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:00:49.768615 taichu-storage-0.0.2/taichu_storage/
--rw-r--r--   0 wangkun    (501) staff       (20)     2559 2023-07-11 01:58:58.000000 taichu-storage-0.0.2/taichu_storage/__init__.py
--rw-r--r--   0 wangkun    (501) staff       (20)     2171 2023-07-11 02:00:34.000000 taichu-storage-0.0.2/taichu_storage/b1.py
--rw-r--r--   0 wangkun    (501) staff       (20)     4717 2023-07-11 01:58:58.000000 taichu-storage-0.0.2/taichu_storage/b3.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1116 2023-06-14 01:52:14.000000 taichu-storage-0.0.2/taichu_storage/env.py
--rw-r--r--   0 wangkun    (501) staff       (20)     2640 2023-07-11 01:58:58.000000 taichu-storage-0.0.2/taichu_storage/minio_client.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1322 2023-07-11 01:58:58.000000 taichu-storage-0.0.2/taichu_storage/obs.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:00:49.769914 taichu-storage-0.0.2/taichu_storage.egg-info/
--rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 02:00:49.000000 taichu-storage-0.0.2/taichu_storage.egg-info/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)      341 2023-07-11 02:00:49.000000 taichu-storage-0.0.2/taichu_storage.egg-info/SOURCES.txt
--rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-07-11 02:00:49.000000 taichu-storage-0.0.2/taichu_storage.egg-info/dependency_links.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       37 2023-07-11 02:00:49.000000 taichu-storage-0.0.2/taichu_storage.egg-info/requires.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       15 2023-07-11 02:00:49.000000 taichu-storage-0.0.2/taichu_storage.egg-info/top_level.txt
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:44:38.655778 taichu-storage-0.0.3/
+-rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 02:44:38.655528 taichu-storage-0.0.3/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-07-11 02:44:38.655872 taichu-storage-0.0.3/setup.cfg
+-rw-r--r--   0 wangkun    (501) staff       (20)      757 2023-07-11 02:43:30.000000 taichu-storage-0.0.3/setup.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:44:38.653362 taichu-storage-0.0.3/taichu_storage/
+-rw-r--r--   0 wangkun    (501) staff       (20)     2559 2023-07-11 01:58:58.000000 taichu-storage-0.0.3/taichu_storage/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     2171 2023-07-11 02:00:34.000000 taichu-storage-0.0.3/taichu_storage/b1.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     4717 2023-07-11 01:58:58.000000 taichu-storage-0.0.3/taichu_storage/b3.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1116 2023-06-14 01:52:14.000000 taichu-storage-0.0.3/taichu_storage/env.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     2640 2023-07-11 01:58:58.000000 taichu-storage-0.0.3/taichu_storage/minio_client.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1322 2023-07-11 01:58:58.000000 taichu-storage-0.0.3/taichu_storage/obs.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 02:44:38.655178 taichu-storage-0.0.3/taichu_storage.egg-info/
+-rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 02:44:38.000000 taichu-storage-0.0.3/taichu_storage.egg-info/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      341 2023-07-11 02:44:38.000000 taichu-storage-0.0.3/taichu_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-07-11 02:44:38.000000 taichu-storage-0.0.3/taichu_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)      104 2023-07-11 02:44:38.000000 taichu-storage-0.0.3/taichu_storage.egg-info/requires.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       15 2023-07-11 02:44:38.000000 taichu-storage-0.0.3/taichu_storage.egg-info/top_level.txt
```

### Comparing `taichu-storage-0.0.2/setup.py` & `taichu-storage-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 if __name__ == '__main__':
     name = 'taichu-storage'
 
-    requirements = ['boto==2.49.0', 'esdk-obs-python==3.22.2']
+    with open('requirements.txt', 'r') as f:
+        requirements = f.read().splitlines()
 
     long_description = 'storage sdks aggregation'
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='0.0.2',
+        version='0.0.3',
         description='storage sdks aggregation',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
```

### Comparing `taichu-storage-0.0.2/taichu_storage/__init__.py` & `taichu-storage-0.0.3/taichu_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.2/taichu_storage/b1.py` & `taichu-storage-0.0.3/taichu_storage/b1.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.2/taichu_storage/b3.py` & `taichu-storage-0.0.3/taichu_storage/b3.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.2/taichu_storage/env.py` & `taichu-storage-0.0.3/taichu_storage/env.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.2/taichu_storage/minio_client.py` & `taichu-storage-0.0.3/taichu_storage/minio_client.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.2/taichu_storage/obs.py` & `taichu-storage-0.0.3/taichu_storage/obs.py`

 * *Files identical despite different names*

