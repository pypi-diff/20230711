# Comparing `tmp/velintegrator-1.0.tar.gz` & `tmp/velintegrator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velintegrator-1.0.tar", last modified: Wed Jul  5 09:03:33 2023, max compression
+gzip compressed data, was "velintegrator-1.0.1.tar", last modified: Tue Jul 11 13:08:30 2023, max compression
```

## Comparing `velintegrator-1.0.tar` & `velintegrator-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-05 09:03:33.660418 velintegrator-1.0/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-05 08:35:43.000000 velintegrator-1.0/MANIFEST.in
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      666 2023-07-05 09:03:33.660308 velintegrator-1.0/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      481 2023-07-05 08:50:48.000000 velintegrator-1.0/README.md
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-07-05 09:03:33.660452 velintegrator-1.0/setup.cfg
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      398 2023-07-05 09:03:26.000000 velintegrator-1.0/setup.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-05 09:03:33.659657 velintegrator-1.0/velintegrator/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-03 06:46:27.000000 velintegrator-1.0/velintegrator/__init__.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      949 2023-07-04 08:35:16.000000 velintegrator-1.0/velintegrator/handler.py
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     3608 2023-07-05 08:44:34.000000 velintegrator-1.0/velintegrator/sdk.py
-drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-05 09:03:33.660177 velintegrator-1.0/velintegrator.egg-info/
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      666 2023-07-05 09:03:33.000000 velintegrator-1.0/velintegrator.egg-info/PKG-INFO
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-07-05 09:03:33.000000 velintegrator-1.0/velintegrator.egg-info/SOURCES.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-07-05 09:03:33.000000 velintegrator-1.0/velintegrator.egg-info/dependency_links.txt
--rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-07-05 09:03:33.000000 velintegrator-1.0/velintegrator.egg-info/top_level.txt
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 13:08:30.671646 velintegrator-1.0.1/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       17 2023-07-11 12:42:19.000000 velintegrator-1.0.1/MANIFEST.in
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      668 2023-07-11 13:08:30.671515 velintegrator-1.0.1/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      481 2023-07-11 12:42:19.000000 velintegrator-1.0.1/README.md
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       38 2023-07-11 13:08:30.671685 velintegrator-1.0.1/setup.cfg
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      400 2023-07-11 13:08:17.000000 velintegrator-1.0.1/setup.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 13:08:30.670738 velintegrator-1.0.1/velintegrator/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 12:42:19.000000 velintegrator-1.0.1/velintegrator/__init__.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     1009 2023-07-11 12:45:44.000000 velintegrator-1.0.1/velintegrator/handler.py
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)     3608 2023-07-11 12:42:19.000000 velintegrator-1.0.1/velintegrator/sdk.py
+drwxr-xr-x   0 dachi_vadachkoria   (501) staff       (20)        0 2023-07-11 13:08:30.671364 velintegrator-1.0.1/velintegrator.egg-info/
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      668 2023-07-11 13:08:30.000000 velintegrator-1.0.1/velintegrator.egg-info/PKG-INFO
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)      260 2023-07-11 13:08:30.000000 velintegrator-1.0.1/velintegrator.egg-info/SOURCES.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)        1 2023-07-11 13:08:30.000000 velintegrator-1.0.1/velintegrator.egg-info/dependency_links.txt
+-rw-r--r--   0 dachi_vadachkoria   (501) staff       (20)       14 2023-07-11 13:08:30.000000 velintegrator-1.0.1/velintegrator.egg-info/top_level.txt
```

### Comparing `velintegrator-1.0/PKG-INFO` & `velintegrator-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velintegrator
-Version: 1.0
+Version: 1.0.1
 Summary: Veli Third Party Integrator
 Author: Dachi
 Author-email: dvadachkoria@veli.store
 Description-Content-Type: text/markdown
 
 Kafka Client for VELI.STORE
```

### Comparing `velintegrator-1.0/velintegrator/handler.py` & `velintegrator-1.0.1/velintegrator/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from velikafkaclient.decorators import tracing
 
 class BaseHandler:
 
     web_integrator = None
     ios_integrator = None
     android_integrator = None
     event_model = None
@@ -13,14 +14,15 @@
         self.event_name = event_name
         self.params_method = self.params_methods_mapper[event_name] if event_name in self.params_methods_mapper else \
             self.base_params_method
 
     def set_data(self, event_data, source):
         return self.event_model(**event_data)
 
+    @tracing
     async def send_data(self, event_data):
         event_data = event_data.dict()
         source = event_data.get('source')
         model = self.set_data(event_data, source)
         integrator_instances = {
             'web': self.web_integrator,
             'ios': self.ios_integrator,
```

### Comparing `velintegrator-1.0/velintegrator/sdk.py` & `velintegrator-1.0.1/velintegrator/sdk.py`

 * *Files identical despite different names*

### Comparing `velintegrator-1.0/velintegrator.egg-info/PKG-INFO` & `velintegrator-1.0.1/velintegrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velintegrator
-Version: 1.0
+Version: 1.0.1
 Summary: Veli Third Party Integrator
 Author: Dachi
 Author-email: dvadachkoria@veli.store
 Description-Content-Type: text/markdown
 
 Kafka Client for VELI.STORE
```

