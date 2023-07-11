# Comparing `tmp/polyswarm-api-3.3.2.tar.gz` & `tmp/polyswarm-api-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyswarm-api-3.3.2.tar", last modified: Tue Jun 20 20:09:43 2023, max compression
+gzip compressed data, was "polyswarm-api-3.4.0.tar", last modified: Tue Jul 11 20:22:10 2023, max compression
```

## Comparing `polyswarm-api-3.3.2.tar` & `polyswarm-api-3.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:09:43.832358 polyswarm-api-3.3.2/
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1616 2023-06-20 20:09:43.828359 polyswarm-api-3.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 20:09:43.832358 polyswarm-api-3.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:09:43.828359 polyswarm-api-3.3.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:09:43.828359 polyswarm-api-3.3.2/src/polyswarm_api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35276 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/api.py
--rw-rw-rw-   0 root         (0) root         (0)    20066 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    39808 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/resources.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:09:43.828359 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1616 2023-06-20 20:09:43.000000 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-20 20:09:43.000000 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:09:43.000000 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-20 20:09:43.000000 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-20 20:09:43.000000 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:22:10.436744 polyswarm-api-3.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-07-11 20:22:10.436744 polyswarm-api-3.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 20:22:10.436744 polyswarm-api-3.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:22:10.432744 polyswarm-api-3.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:22:10.436744 polyswarm-api-3.4.0/src/polyswarm_api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    35477 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20066 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    40300 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:22:10.436744 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-07-11 20:22:10.000000 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-11 20:22:10.000000 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 20:22:10.000000 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-11 20:22:10.000000 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 20:22:10.000000 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/top_level.txt
```

### Comparing `polyswarm-api-3.3.2/LICENSE` & `polyswarm-api-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.3.2/PKG-INFO` & `polyswarm-api-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm-api
-Version: 3.3.2
+Version: 3.4.0
 Summary: Client library to simplify interacting with the PolySwarm consumer API
 Home-page: https://github.com/polyswarm/polyswarm-api
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `polyswarm-api-3.3.2/README.md` & `polyswarm-api-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.3.2/setup.py` & `polyswarm-api-3.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The README.md will be used as the content for the PyPi package details page on the Python Package Index.
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 
 setup(
     name='polyswarm-api',
-    version='3.3.2',
+    version='3.4.0',
     description='Client library to simplify interacting with the PolySwarm consumer API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='PolySwarm Developers',
     author_email='info@polyswarm.io',
     url='https://github.com/polyswarm/polyswarm-api',
     license='MIT',
```

### Comparing `polyswarm-api-3.3.2/src/polyswarm_api/api.py` & `polyswarm-api-3.4.0/src/polyswarm_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -665,20 +665,20 @@
         """
         logger.info('Downloading %s into %s', instance_id, out_dir)
         artifact = resources.LocalArtifact.download_id(self, instance_id, folder=out_dir).result()
         artifact.handle.close()
 
         return artifact
 
-    def sandbox(self, instance_id, sandbox):
-        logger.info('Sandboxing %s in %s', instance_id, sandbox)
-        return resources.SandboxTask.create(self, artifact_id=instance_id, sandbox=sandbox).result()
+    def sandbox(self, instance_id, provider_slug, vm_slug):
+        logger.info('Sandboxing %s in provider %s vm %s', instance_id, provider_slug, vm_slug)
+        return resources.SandboxTask.create(self, artifact_id=instance_id, provider_slug=provider_slug, vm_slug=vm_slug).result()
 
-    def sandbox_file(self, artifact, sandbox, artifact_type=resources.ArtifactType.FILE, artifact_name=None):
-        logger.info('Sandboxing file in %s', sandbox)
+    def sandbox_file(self, artifact, provider_slug, vm_slug, artifact_type=resources.ArtifactType.FILE, artifact_name=None):
+        logger.info('Sandboxing file in provider %s vm %s', provider_slug, vm_slug)
         artifact_type = resources.ArtifactType.parse(artifact_type)
         # TODO This is a python 2.7 check if artifact is a file-like instance, consider changing
         #  to isinstance(artifact, io.IOBase) when deprecating 2.7 and implementing making LocalHandle
         #  inherit io.IOBase, although this will change the method delegation logic in the resource
         if hasattr(artifact, 'read') and hasattr(artifact.read, '__call__'):
             artifact = resources.LocalArtifact.from_handle(self, artifact, artifact_name=artifact_name or '',
                                                            artifact_type=artifact_type)
@@ -691,15 +691,16 @@
                                                                 artifact_name=artifact_name or artifact,
                                                                 artifact_type=artifact_type)
         if isinstance(artifact, resources.LocalArtifact):
             task = resources.SandboxTask.create_file(self,
                                                      artifact_name=artifact.artifact_name,
                                                      artifact_type=artifact.artifact_type.name,
                                                      community=self.community,
-                                                     sandbox=sandbox).result()
+                                                     provider_slug=provider_slug,
+                                                     vm_slug=vm_slug).result()
             task.upload_file(artifact)
             return resources.SandboxTask.update_file(self, id=task.id).result()
         else:
             raise exceptions.InvalidValueException(
                 'Artifacts should be a path to a file or a LocalArtifact instance')
 
     def sandbox_providers(self):
```

### Comparing `polyswarm-api-3.3.2/src/polyswarm_api/core.py` & `polyswarm-api-3.4.0/src/polyswarm_api/core.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.3.2/src/polyswarm_api/exceptions.py` & `polyswarm-api-3.4.0/src/polyswarm_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.3.2/src/polyswarm_api/resources.py` & `polyswarm-api-3.4.0/src/polyswarm_api/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1069,7 +1069,19 @@
         self.mimetype = content['mimetype']
         self.extended_type = content['extended_type']
         self.type = content['type']
 
 
 class SandboxProvider(core.BaseJsonResource):
     RESOURCE_ENDPOINT = "/sandbox/provider"
+
+    def __init__(self, content, api=None):
+        super(SandboxProvider, self).__init__(content, api=api)
+        self.slug = content['slug']
+        self.name = content['name']
+        self.tool = content['tool']
+        self.vms = content['vms']
+
+    @classmethod
+    def parse_result(cls, api, content, **kwargs):
+        logger.debug('Parsing resource %s', cls.__name__)
+        return [super(SandboxProvider, cls).parse_result(api, content[slug], **kwargs) for slug in content.keys()]
```

### Comparing `polyswarm-api-3.3.2/src/polyswarm_api/settings.py` & `polyswarm-api-3.4.0/src/polyswarm_api/settings.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.3.2/src/polyswarm_api.egg-info/PKG-INFO` & `polyswarm-api-3.4.0/src/polyswarm_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm-api
-Version: 3.3.2
+Version: 3.4.0
 Summary: Client library to simplify interacting with the PolySwarm consumer API
 Home-page: https://github.com/polyswarm/polyswarm-api
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

