# Comparing `tmp/taichu-storage-0.0.6.tar.gz` & `tmp/taichu-storage-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-storage-0.0.6.tar", last modified: Tue Jul 11 10:35:00 2023, max compression
+gzip compressed data, was "taichu-storage-0.0.7.tar", last modified: Tue Jul 11 10:52:53 2023, max compression
```

## Comparing `taichu-storage-0.0.6.tar` & `taichu-storage-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 10:35:00.776042 taichu-storage-0.0.6/
--rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 10:35:00.775713 taichu-storage-0.0.6/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-07-11 10:35:00.776213 taichu-storage-0.0.6/setup.cfg
--rw-r--r--   0 wangkun    (501) staff       (20)      757 2023-07-11 10:34:53.000000 taichu-storage-0.0.6/setup.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 10:35:00.773570 taichu-storage-0.0.6/taichu_storage/
--rw-r--r--   0 wangkun    (501) staff       (20)     2597 2023-07-11 09:19:04.000000 taichu-storage-0.0.6/taichu_storage/__init__.py
--rw-r--r--   0 wangkun    (501) staff       (20)     5005 2023-07-11 09:39:29.000000 taichu-storage-0.0.6/taichu_storage/b3.py
--rw-r--r--   0 wangkun    (501) staff       (20)     3167 2023-07-11 09:19:04.000000 taichu-storage-0.0.6/taichu_storage/boto_client.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1116 2023-06-14 01:52:14.000000 taichu-storage-0.0.6/taichu_storage/env.py
--rw-r--r--   0 wangkun    (501) staff       (20)     2640 2023-07-11 01:58:58.000000 taichu-storage-0.0.6/taichu_storage/minio_client.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1643 2023-07-11 09:19:04.000000 taichu-storage-0.0.6/taichu_storage/obs.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 10:35:00.775211 taichu-storage-0.0.6/taichu_storage.egg-info/
--rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 10:35:00.000000 taichu-storage-0.0.6/taichu_storage.egg-info/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)      350 2023-07-11 10:35:00.000000 taichu-storage-0.0.6/taichu_storage.egg-info/SOURCES.txt
--rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-07-11 10:35:00.000000 taichu-storage-0.0.6/taichu_storage.egg-info/dependency_links.txt
--rw-r--r--   0 wangkun    (501) staff       (20)      104 2023-07-11 10:35:00.000000 taichu-storage-0.0.6/taichu_storage.egg-info/requires.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       15 2023-07-11 10:35:00.000000 taichu-storage-0.0.6/taichu_storage.egg-info/top_level.txt
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 10:52:53.477996 taichu-storage-0.0.7/
+-rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 10:52:53.476879 taichu-storage-0.0.7/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-07-11 10:52:53.478182 taichu-storage-0.0.7/setup.cfg
+-rw-r--r--   0 wangkun    (501) staff       (20)      757 2023-07-11 10:52:51.000000 taichu-storage-0.0.7/setup.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 10:52:53.469700 taichu-storage-0.0.7/taichu_storage/
+-rw-r--r--   0 wangkun    (501) staff       (20)     2597 2023-07-11 09:19:04.000000 taichu-storage-0.0.7/taichu_storage/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     5005 2023-07-11 09:39:29.000000 taichu-storage-0.0.7/taichu_storage/b3.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     3167 2023-07-11 09:19:04.000000 taichu-storage-0.0.7/taichu_storage/boto_client.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1116 2023-06-14 01:52:14.000000 taichu-storage-0.0.7/taichu_storage/env.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     2640 2023-07-11 01:58:58.000000 taichu-storage-0.0.7/taichu_storage/minio_client.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1643 2023-07-11 09:19:04.000000 taichu-storage-0.0.7/taichu_storage/obs.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 10:52:53.476061 taichu-storage-0.0.7/taichu_storage.egg-info/
+-rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 10:52:53.000000 taichu-storage-0.0.7/taichu_storage.egg-info/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      350 2023-07-11 10:52:53.000000 taichu-storage-0.0.7/taichu_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-07-11 10:52:53.000000 taichu-storage-0.0.7/taichu_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)      102 2023-07-11 10:52:53.000000 taichu-storage-0.0.7/taichu_storage.egg-info/requires.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       15 2023-07-11 10:52:53.000000 taichu-storage-0.0.7/taichu_storage.egg-info/top_level.txt
```

### Comparing `taichu-storage-0.0.6/setup.py` & `taichu-storage-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     long_description = 'storage sdks aggregation'
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='0.0.6',
+        version='0.0.7',
         description='storage sdks aggregation',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
```

### Comparing `taichu-storage-0.0.6/taichu_storage/__init__.py` & `taichu-storage-0.0.7/taichu_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.6/taichu_storage/b3.py` & `taichu-storage-0.0.7/taichu_storage/b3.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.6/taichu_storage/boto_client.py` & `taichu-storage-0.0.7/taichu_storage/boto_client.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.6/taichu_storage/env.py` & `taichu-storage-0.0.7/taichu_storage/env.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.6/taichu_storage/minio_client.py` & `taichu-storage-0.0.7/taichu_storage/minio_client.py`

 * *Files identical despite different names*

### Comparing `taichu-storage-0.0.6/taichu_storage/obs.py` & `taichu-storage-0.0.7/taichu_storage/obs.py`

 * *Files identical despite different names*

