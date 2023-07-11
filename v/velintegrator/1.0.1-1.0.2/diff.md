# Comparing `tmp/velintegrator-1.0.1.tar.gz` & `tmp/velintegrator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velintegrator-1.0.1.tar", last modified: Tue Jul 11 13:08:30 2023, max compression
+gzip compressed data, was "velintegrator-1.0.2.tar", last modified: Tue Jul 11 14:05:07 2023, max compression
```

## Comparing `velintegrator-1.0.1.tar` & `velintegrator-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 13:08:30.671646 velintegrator-1.0.1/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.0.1/MANIFEST.in
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      668 2023-07-11 13:08:30.671515 velintegrator-1.0.1/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      481 2023-07-11 12:42:19.000000 velintegrator-1.0.1/README.md
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-07-11 13:08:30.671685 velintegrator-1.0.1/setup.cfg
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2023-07-11 13:08:17.000000 velintegrator-1.0.1/setup.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 13:08:30.670738 velintegrator-1.0.1/velintegrator/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.0.1/velintegrator/__init__.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     1009 2023-07-11 12:45:44.000000 velintegrator-1.0.1/velintegrator/handler.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     3608 2023-07-11 12:42:19.000000 velintegrator-1.0.1/velintegrator/sdk.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 13:08:30.671364 velintegrator-1.0.1/velintegrator.egg-info/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      668 2023-07-11 13:08:30.000000 velintegrator-1.0.1/velintegrator.egg-info/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-07-11 13:08:30.000000 velintegrator-1.0.1/velintegrator.egg-info/SOURCES.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-07-11 13:08:30.000000 velintegrator-1.0.1/velintegrator.egg-info/dependency_links.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-07-11 13:08:30.000000 velintegrator-1.0.1/velintegrator.egg-info/top_level.txt
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 14:05:07.115619 velintegrator-1.0.2/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.0.2/MANIFEST.in
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-11 14:05:07.115498 velintegrator-1.0.2/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      742 2023-07-11 14:04:48.000000 velintegrator-1.0.2/README.md
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-07-11 14:05:07.115652 velintegrator-1.0.2/setup.cfg
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2023-07-11 14:03:39.000000 velintegrator-1.0.2/setup.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 14:05:07.114825 velintegrator-1.0.2/velintegrator/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.0.2/velintegrator/__init__.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     1031 2023-07-11 14:03:25.000000 velintegrator-1.0.2/velintegrator/handler.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     3608 2023-07-11 12:42:19.000000 velintegrator-1.0.2/velintegrator/sdk.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 14:05:07.115366 velintegrator-1.0.2/velintegrator.egg-info/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      929 2023-07-11 14:05:07.000000 velintegrator-1.0.2/velintegrator.egg-info/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-07-11 14:05:07.000000 velintegrator-1.0.2/velintegrator.egg-info/SOURCES.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-07-11 14:05:07.000000 velintegrator-1.0.2/velintegrator.egg-info/dependency_links.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-07-11 14:05:07.000000 velintegrator-1.0.2/velintegrator.egg-info/top_level.txt
```

### Comparing `velintegrator-1.0.1/velintegrator/handler.py` & `velintegrator-1.0.2/velintegrator/handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from velikafkaclient.decorators import tracing
 
-class BaseHandler:
 
+class BaseHandler:
     web_integrator = None
     ios_integrator = None
     android_integrator = None
     event_model = None
     params_methods_mapper = {}
     base_params_method = None
     params_method = None
+    tracing_id = None
 
     def __init__(self, event_name):
         self.event_name = event_name
         self.params_method = self.params_methods_mapper[event_name] if event_name in self.params_methods_mapper else \
             self.base_params_method
 
     def set_data(self, event_data, source):
```

### Comparing `velintegrator-1.0.1/velintegrator/sdk.py` & `velintegrator-1.0.2/velintegrator/sdk.py`

 * *Files identical despite different names*

