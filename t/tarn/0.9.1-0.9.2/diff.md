# Comparing `tmp/tarn-0.9.1.tar.gz` & `tmp/tarn-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.9.1.tar", last modified: Wed Jul  5 09:33:43 2023, max compression
+gzip compressed data, was "tarn-0.9.2.tar", last modified: Tue Jul 11 08:56:38 2023, max compression
```

## Comparing `tarn-0.9.1.tar` & `tarn-0.9.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:33:43.922975 tarn-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-05 09:33:41.000000 tarn-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 09:33:41.000000 tarn-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-05 09:33:43.918975 tarn-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-05 09:33:41.000000 tarn-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-05 09:33:41.000000 tarn-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-05 09:33:41.000000 tarn-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:33:43.922975 tarn-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-05 09:33:41.000000 tarn-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:33:43.914975 tarn-0.9.1/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:33:43.918975 tarn-0.9.1/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:33:43.918975 tarn-0.9.1/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:33:43.918975 tarn-0.9.1/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/location/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/location/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:33:43.918975 tarn-0.9.1/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:33:43.918975 tarn-0.9.1/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:33:43.918975 tarn-0.9.1/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:33:43.918975 tarn-0.9.1/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/tools/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-05 09:33:41.000000 tarn-0.9.1/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:33:43.914975 tarn-0.9.1/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-05 09:33:43.000000 tarn-0.9.1/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-05 09:33:43.000000 tarn-0.9.1/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:33:43.000000 tarn-0.9.1/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-05 09:33:43.000000 tarn-0.9.1/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-05 09:33:43.000000 tarn-0.9.1/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-11 08:56:33.000000 tarn-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 08:56:33.000000 tarn-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 08:56:38.443924 tarn-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-11 08:56:33.000000 tarn-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-11 08:56:33.000000 tarn-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 08:56:33.000000 tarn-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 08:56:38.443924 tarn-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-11 08:56:33.000000 tarn-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.439924 tarn-0.9.2/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.439924 tarn-0.9.2/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.443924 tarn-0.9.2/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/tools/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-11 08:56:33.000000 tarn-0.9.2/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:56:38.439924 tarn-0.9.2/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 08:56:38.000000 tarn-0.9.2/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-11 08:56:38.000000 tarn-0.9.2/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:56:38.000000 tarn-0.9.2/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 08:56:38.000000 tarn-0.9.2/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 08:56:38.000000 tarn-0.9.2/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.9.1/LICENSE` & `tarn-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/PKG-INFO` & `tarn-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.9.1
+Version: 0.9.2
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.1.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.2.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.9.1/README.md` & `tarn-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/pyproject.toml` & `tarn-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/setup.py` & `tarn-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/cache/storage.py` & `tarn-0.9.2/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/compat.py` & `tarn-0.9.2/tarn/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/config.py` & `tarn-0.9.2/tarn/config.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/digest.py` & `tarn-0.9.2/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/interface.py` & `tarn-0.9.2/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/local/storage.py` & `tarn-0.9.2/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/location/disk_dict.py` & `tarn-0.9.2/tarn/location/disk_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from contextlib import contextmanager
 from pathlib import Path
 from typing import ContextManager, Iterable, Optional, Tuple, Union
 
 from ..compat import Self, copy_file, remove_file, rmtree
 from ..config import load_config, root_params
 from ..digest import key_to_relative
-from ..exceptions import StorageCorruption
+from ..exceptions import CollisionError, StorageCorruption
 from ..interface import Key, Keys, MaybeLabels, MaybeValue, PathOrStr, Value
 from ..tools import Locker, SizeTracker, UsageTracker
 from ..tools.labels import LabelsStorage
 from ..utils import adjust_permissions, create_folders, get_size, match_buffers, match_files
 from .interface import Meta, Writable
 
 logger = logging.getLogger(__name__)
@@ -202,12 +202,15 @@
 
 
 def _is_pathlike(x):
     return isinstance(x, (os.PathLike, str))
 
 
 def _match(value, file, key):
-    if _is_pathlike(value):
-        match_files(value, file)
-    else:
-        with open(file, 'rb') as dst:
-            match_buffers(value, dst, context=key.hex())
+    try:
+        if _is_pathlike(value):
+            match_files(value, file)
+        else:
+            with open(file, 'rb') as dst:
+                match_buffers(value, dst, context=key.hex())
+    except ValueError as e:
+        raise CollisionError(f"Written value and the new one doesn't match: {key}") from e
```

### Comparing `tarn-0.9.1/tarn/location/fanout.py` & `tarn-0.9.2/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/location/interface.py` & `tarn-0.9.2/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/location/levels.py` & `tarn-0.9.2/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/location/nginx.py` & `tarn-0.9.2/tarn/location/nginx.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/location/redis.py` & `tarn-0.9.2/tarn/location/redis.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from contextlib import contextmanager
 from datetime import datetime
 from typing import Any, ContextManager, Iterable, Optional, Tuple, Union
 
 from redis import Redis
 
 from ..digest import value_to_buffer
+from ..exceptions import CollisionError, StorageCorruption
 from ..interface import Key, Keys, MaybeLabels, Meta, Value
 from .interface import Writable
 
 
 class RedisLocation(Writable):
     def __init__(self, redis: Union[Redis, str], prefix: str = ''):
         if isinstance(redis, str):
@@ -22,52 +23,58 @@
     def contents(self) -> Iterable[Tuple[Key, Any, Meta]]:
         for raw_key in self.redis.scan_iter(match=self.prefix + b'*'):
             key = raw_key[len(self.prefix):]
             yield key, self, RedisMeta(key=key, location=self)
 
     @contextmanager
     def read(self, key: Key, return_labels: bool) -> ContextManager:
-        content_key = self.prefix + key
-        content = self.redis.get(content_key)
-        if content is None:
-            yield
-            return
-        self.update_usage_date(key)
-        if return_labels:
-            labels = self.get_labels(key)
-            with value_to_buffer(self.redis.get(content_key)) as buffer:
-                yield buffer, labels
+        try:
+            content_key = self.prefix + key
+            content = self.redis.get(content_key)
+            if content is None:
+                yield
                 return
-        with value_to_buffer(self.redis.get(content_key)) as buffer:
-            yield buffer
+            self.update_usage_date(key)
+            if return_labels:
+                labels = self.get_labels(key)
+                with value_to_buffer(self.redis.get(content_key)) as buffer:
+                    yield buffer, labels
+                    return
+            with value_to_buffer(self.redis.get(content_key)) as buffer:
+                yield buffer
+        except StorageCorruption:
+            self.delete(key)
     
     def read_batch(self, keys: Keys) -> Iterable[Optional[Tuple[Key, Tuple[Value, MaybeLabels]]]]:
         for key in keys:
             with self.read(key, True) as value:
                 yield key, value
                 
     @contextmanager
     def write(self, key: Key, value: Value, labels: MaybeLabels) -> ContextManager:
-        content_key = self.prefix + key
-        with value_to_buffer(value) as value:
-            content = self.redis.get(content_key)
-            if content is None:
-                self.redis.set(content_key, value.read())
+        try:
+            content_key = self.prefix + key
+            with value_to_buffer(value) as value:
+                content = self.redis.get(content_key)
+                if content is None:
+                    self.redis.set(content_key, value.read())
+                    self.update_labels(key, labels)
+                    self.update_usage_date(key)
+                    with value_to_buffer(self.redis.get(content_key)) as buffer:
+                        yield buffer
+                        return
+                old_content = self.redis.get(content_key)
+                if old_content != value.read():
+                    raise CollisionError(f"Written value and the new one doesn't match: {key}")
                 self.update_labels(key, labels)
                 self.update_usage_date(key)
                 with value_to_buffer(self.redis.get(content_key)) as buffer:
                     yield buffer
-                    return
-            old_content = self.redis.get(content_key)
-            if old_content != value.read():
-                raise ValueError(f"Written value and the new one doesn't match: {key}")
-            self.update_labels(key, labels)
-            self.update_usage_date(key)
-            with value_to_buffer(self.redis.get(content_key)) as buffer:
-                yield buffer
+        except StorageCorruption:
+            self.delete(key)
 
     def get_labels(self, key: Key) -> MaybeLabels:
         labels_key = b'labels' + self.prefix + key
         labels_bytes = self.redis.get(labels_key)
         if labels_bytes is None:
             return
         return list(json.loads(labels_bytes))
```

### Comparing `tarn-0.9.1/tarn/location/s3.py` & `tarn-0.9.2/tarn/location/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from contextlib import contextmanager
 from datetime import datetime
 from io import SEEK_CUR, SEEK_END, SEEK_SET
 from typing import Any, BinaryIO, ContextManager, Iterable, Mapping, Optional, Tuple, Union
 
 from botocore.exceptions import ClientError
 
+from tarn.exceptions import CollisionError
+
 from ..compat import S3Client
 from ..digest import key_to_relative, value_to_buffer
+from ..exceptions import CollisionError, StorageCorruption
 from ..interface import Key, Keys, MaybeLabels, Meta, Value
 from ..utils import match_buffers
 from .interface import Writable
 
 
 class S3(Writable):
     def __init__(self, s3_client: S3Client, bucket_name: str):
@@ -27,55 +30,64 @@
                 for obj in response['Contents']:
                     path = obj['Key']
                     key = self._path_to_key(path)
                     yield key, self, S3Meta(path=path, location=self)
 
     @contextmanager
     def read(self, key: Key, return_labels: bool) -> ContextManager[Union[None, Value, Tuple[Value, MaybeLabels]]]:
-        path = self._key_to_path(key)
         try:
-            if return_labels:
-                self.update_usage_date(path)
-                yield self._get_buffer(path), self.get_labels(path)
-            else:
-                self.update_usage_date(path)
-                yield self._get_buffer(path)
-
-        except ClientError as e:
-            if e.response['Error']['Code'] == "404" or e.response['Error']['Code'] == "NoSuchKey":  # file doesn't exist
-                yield
-            else:
-                raise
+            path = self._key_to_path(key)
+            try:
+                if return_labels:
+                    self.update_usage_date(path)
+                    yield self._get_buffer(path), self.get_labels(path)
+                else:
+                    self.update_usage_date(path)
+                    yield self._get_buffer(path)
+
+            except ClientError as e:
+                if e.response['Error']['Code'] == "404" or e.response['Error']['Code'] == "NoSuchKey":  # file doesn't exist
+                    yield
+                else:
+                    raise
+        except StorageCorruption:
+            self.delete(key)
 
     def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, Union[Value, MaybeLabels]]]:
         for key in keys:
             with self.read(key, True) as value:
                 yield key, value
 
     @contextmanager
     def write(self, key: Key, value: Value, labels: MaybeLabels) -> ContextManager:
-        path = self._key_to_path(key)
-        with value_to_buffer(value) as value:
-            try:
-                self.s3.get_object(Bucket=self.bucket, Key=path)
-                obj_body = self.s3.get_object(Bucket=self.bucket, Key=path).get('Body')
-                match_buffers(value, obj_body, context=key.hex())
-                self.update_labels(path, labels)
-                self.update_usage_date(path)
-                yield self._get_buffer(path)
-                return
-            except ClientError as e:
-                if e.response['Error']['Code'] == "404" or e.response['Error']['Code'] == "NoSuchKey":
-                    self.s3.upload_fileobj(Bucket=self.bucket, Key=path, Fileobj=value)
+        try:
+            path = self._key_to_path(key)
+            with value_to_buffer(value) as value:
+                try:
+                    self.s3.get_object(Bucket=self.bucket, Key=path)
+                    obj_body = self.s3.get_object(Bucket=self.bucket, Key=path).get('Body')
+                    try:
+                        match_buffers(value, obj_body, context=key.hex())
+                    except ValueError as e:
+                        raise CollisionError(f"Written value and the new one doesn't match: {key}") from e
                     self.update_labels(path, labels)
                     self.update_usage_date(path)
                     yield self._get_buffer(path)
                     return
-                else:
-                    raise
+                except ClientError as e:
+                    if e.response['Error']['Code'] == "404" or e.response['Error']['Code'] == "NoSuchKey":
+                        self.s3.upload_fileobj(Bucket=self.bucket, Key=path, Fileobj=value)
+                        self.update_labels(path, labels)
+                        self.update_usage_date(path)
+                        yield self._get_buffer(path)
+                        return
+                    else:
+                        raise
+        except StorageCorruption:
+            self.delete(key)
 
     def delete(self, key: Key):
         path = self._key_to_path(key)
         self.s3.delete_object(Bucket=self.bucket, Key=path)
 
     def update_labels(self, path: str, labels: MaybeLabels):
         if labels is not None:
```

### Comparing `tarn-0.9.1/tarn/location/scp.py` & `tarn-0.9.2/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/pickler/compat.py` & `tarn-0.9.2/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/pickler/interface.py` & `tarn-0.9.2/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/pool/hash_key.py` & `tarn-0.9.2/tarn/pool/hash_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/pool/pickle_key.py` & `tarn-0.9.2/tarn/pool/pickle_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import logging
-from io import BytesIO
 import os
+from io import BytesIO
 from pathlib import Path
 from typing import Any, NamedTuple, Optional, Sequence, Type, Union
 
 from ..compat import HashAlgorithm
-from ..exceptions import DeserializationError, ReadError, StorageCorruption, WriteError
+from ..exceptions import CollisionError, DeserializationError, ReadError, StorageCorruption, WriteError
 from ..interface import Key, MaybeLabels, PathOrStr, Value
 from ..location import Level, Location
 from ..pickler import PREVIOUS_VERSIONS, dumps
 from ..serializers import Serializer, SerializerError
 from ..utils import value_to_buffer
 from .hash_key import HashKeyStorage, LocationsLike, resolve_location
 
@@ -67,20 +67,23 @@
 
         digest = key.digest
         logger.info('Serializing %s', digest)
         mapping = dict(self.serializer.save(value, lambda v: self.storage.write(v, labels=labels).hex()))
 
         # we want a reproducible mapping each time
         logger.info('Saving to index %s', digest)
-        with self.index.write(digest, BytesIO(json.dumps(mapping, sort_keys=True).encode()), labels=None) as written:
-            if written is None:
-                if error:
-                    raise WriteError('The index could not be written to any storage')
-                return None
-
+        try:
+            with self.index.write(digest, BytesIO(json.dumps(mapping, sort_keys=True).encode()), labels=None) as written:
+                if written is None:
+                    if error:
+                        raise WriteError('The index could not be written to any storage')
+                    return None
+        except CollisionError as e:
+            with self.index.read(digest, return_labels=False) as v:
+                raise CollisionError(f'Old mapping: {v.read()}. New mapping: {mapping}') from e
         return digest
 
     def _read_for_digest(self, digest):
         with self.index.read(digest, False) as index:
             if index is None:
                 return None, False
```

### Comparing `tarn-0.9.1/tarn/serializers.py` & `tarn-0.9.2/tarn/serializers.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/tools/labels.py` & `tarn-0.9.2/tarn/tools/labels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/tools/locker.py` & `tarn-0.9.2/tarn/tools/locker.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/tools/size.py` & `tarn-0.9.2/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/tools/usage.py` & `tarn-0.9.2/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn/utils.py` & `tarn-0.9.2/tarn/utils.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.1/tarn.egg-info/PKG-INFO` & `tarn-0.9.2/tarn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.9.1
+Version: 0.9.2
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.1.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.2.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.9.1/tarn.egg-info/SOURCES.txt` & `tarn-0.9.2/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

