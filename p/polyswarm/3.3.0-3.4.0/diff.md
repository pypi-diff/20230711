# Comparing `tmp/polyswarm-3.3.0.tar.gz` & `tmp/polyswarm-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyswarm-3.3.0.tar", last modified: Tue Jun 20 20:14:41 2023, max compression
+gzip compressed data, was "polyswarm-3.4.0.tar", last modified: Tue Jul 11 20:34:12 2023, max compression
```

## Comparing `polyswarm-3.3.0.tar` & `polyswarm-3.4.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.561974 polyswarm-3.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-20 20:13:59.000000 polyswarm-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2664 2023-06-20 20:14:41.561974 polyswarm-3.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-06-20 20:13:59.000000 polyswarm-3.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 20:14:41.561974 polyswarm-3.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-06-20 20:13:59.000000 polyswarm-3.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.557974 polyswarm-3.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.557974 polyswarm-3.3.0/src/polyswarm/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.561974 polyswarm-3.3.0/src/polyswarm/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/download.py
--rw-rw-rw-   0 root         (0) root         (0)     3734 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/engine.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/families.py
--rw-rw-rw-   0 root         (0) root         (0)     4528 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/historical.py
--rw-rw-rw-   0 root         (0) root         (0)     2430 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/links.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/live.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     6156 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/polyswarm.py
--rw-rw-rw-   0 root         (0) root         (0)     2163 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/rules.py
--rw-rw-rw-   0 root         (0) root         (0)     4000 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/sandbox.py
--rw-rw-rw-   0 root         (0) root         (0)     6349 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/scan.py
--rw-rw-rw-   0 root         (0) root         (0)     5916 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/search.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/tags.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.561974 polyswarm-3.3.0/src/polyswarm/formatters/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/formatters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/formatters/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2153 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/formatters/hashes.py
--rw-rw-rw-   0 root         (0) root         (0)     5722 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/formatters/json.py
--rw-rw-rw-   0 root         (0) root         (0)    24719 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/formatters/text.py
--rw-rw-rw-   0 root         (0) root         (0)    10475 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/polyswarm.py
--rw-rw-rw-   0 root         (0) root         (0)     3760 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.557974 polyswarm-3.3.0/src/polyswarm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2664 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1023 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:34:12.685487 polyswarm-3.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-11 20:33:49.000000 polyswarm-3.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-07-11 20:34:12.685487 polyswarm-3.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-11 20:33:49.000000 polyswarm-3.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 20:34:12.685487 polyswarm-3.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-07-11 20:33:49.000000 polyswarm-3.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:34:12.681487 polyswarm-3.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:34:12.681487 polyswarm-3.4.0/src/polyswarm/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:34:12.685487 polyswarm-3.4.0/src/polyswarm/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/families.py
+-rw-rw-rw-   0 root         (0) root         (0)     4528 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/historical.py
+-rw-rw-rw-   0 root         (0) root         (0)     2430 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/links.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/live.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     6156 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/polyswarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2163 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4182 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/sandbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     6349 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/scan.py
+-rw-rw-rw-   0 root         (0) root         (0)     5916 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/client/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:34:12.685487 polyswarm-3.4.0/src/polyswarm/formatters/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/formatters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/formatters/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2153 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/formatters/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     5722 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/formatters/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    25212 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/formatters/text.py
+-rw-rw-rw-   0 root         (0) root         (0)    10475 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/polyswarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     3760 2023-07-11 20:33:49.000000 polyswarm-3.4.0/src/polyswarm/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:34:12.681487 polyswarm-3.4.0/src/polyswarm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-07-11 20:34:12.000000 polyswarm-3.4.0/src/polyswarm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-07-11 20:34:12.000000 polyswarm-3.4.0/src/polyswarm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 20:34:12.000000 polyswarm-3.4.0/src/polyswarm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-11 20:34:12.000000 polyswarm-3.4.0/src/polyswarm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2023-07-11 20:34:12.000000 polyswarm-3.4.0/src/polyswarm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-11 20:34:12.000000 polyswarm-3.4.0/src/polyswarm.egg-info/top_level.txt
```

### Comparing `polyswarm-3.3.0/LICENSE` & `polyswarm-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/PKG-INFO` & `polyswarm-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm
-Version: 3.3.0
+Version: 3.4.0
 Summary: CLI for using the PolySwarm Customer APIs
 Home-page: https://github.com/polyswarm/polyswarm-cli
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `polyswarm-3.3.0/README.md` & `polyswarm-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/setup.py` & `polyswarm-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # The README.md will be used as the content for the PyPi package details page on the Python Package Index.
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 
 setup(
     name='polyswarm',
-    version='3.3.0',
+    version='3.4.0',
     description='CLI for using the PolySwarm Customer APIs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='PolySwarm Developers',
     author_email='info@polyswarm.io',
     url='https://github.com/polyswarm/polyswarm-cli',
     license='MIT',
     python_requires='>=3.5,<4',
     install_requires=[
-        'polyswarm-api~=3.3.2',
+        'polyswarm-api~=3.4.0',
         'click~=7.0',
         'colorama~=0.4.3',
         'future~=0.18.2',
         'click-log~=0.3.2',
         'pygments~=2.5.2',
     ],
     extras_require={
```

### Comparing `polyswarm-3.3.0/src/polyswarm/__main__.py` & `polyswarm-3.4.0/src/polyswarm/__main__.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/download.py` & `polyswarm-3.4.0/src/polyswarm/client/download.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/engine.py` & `polyswarm-3.4.0/src/polyswarm/client/engine.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/families.py` & `polyswarm-3.4.0/src/polyswarm/client/families.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/historical.py` & `polyswarm-3.4.0/src/polyswarm/client/historical.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/links.py` & `polyswarm-3.4.0/src/polyswarm/client/links.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/live.py` & `polyswarm-3.4.0/src/polyswarm/client/live.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/metadata.py` & `polyswarm-3.4.0/src/polyswarm/client/metadata.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/polyswarm.py` & `polyswarm-3.4.0/src/polyswarm/client/polyswarm.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/rules.py` & `polyswarm-3.4.0/src/polyswarm/client/rules.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/sandbox.py` & `polyswarm-3.4.0/src/polyswarm/client/sandbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,40 +11,42 @@
 
 @click.group(short_help='Interact with the Polyswarm sandbox system.')
 def sandbox():
     pass
 
 
 @sandbox.command('instance', short_help='Submit an existing artifact by id to be sandboxed.')
-@click.argument('sandbox', type=click.STRING)
+@click.argument('provider_slug', type=click.STRING)
 @click.argument('artifact-id', nargs=-1, callback=utils.validate_id)
+@click.option('--vm_slug', 'vm_slug', type=click.STRING)
 @click.pass_context
-def submit(ctx, sandbox, artifact_id):
+def submit(ctx, provider_slug, artifact_id, vm_slug):
     """
     Submit an artifact by artifact id to be sandboxed.
     """
     api = ctx.obj['api']
     output = ctx.obj['output']
 
-    for tasks in api.sandbox_instances(artifact_id, sandbox=sandbox):
+    for tasks in api.sandbox_instances(artifact_id, provider_slug=provider_slug, vm_slug=vm_slug):
         output.sandbox_task(tasks)
 
 
 @sandbox.command('file', short_help='Submit a local file to be sandboxed.')
 @click.argument('sandbox', type=click.STRING)
 @click.argument('path', type=click.Path(exists=True), required=True)
+@click.option('--vm_slug', 'vm_slug', type=click.STRING)
 @click.pass_context
-def file(ctx, path, sandbox):
+def file(ctx, path, sandbox, vm_slug):
     """
     Submit a local file to be sandboxed.
     """
     api = ctx.obj['api']
     output = ctx.obj['output']
 
-    output.sandbox_task(api.sandbox_file(path, sandbox))
+    output.sandbox_task(api.sandbox_file(path, sandbox, vm_slug))
 
 
 @sandbox.command('providers', short_help='List the names of available sandboxes.')
 @click.pass_context
 def sandbox_list(ctx):
     """
     List the names of available sandbox providers.
```

### Comparing `polyswarm-3.3.0/src/polyswarm/client/scan.py` & `polyswarm-3.4.0/src/polyswarm/client/scan.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/search.py` & `polyswarm-3.4.0/src/polyswarm/client/search.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/tags.py` & `polyswarm-3.4.0/src/polyswarm/client/tags.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/client/utils.py` & `polyswarm-3.4.0/src/polyswarm/client/utils.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/formatters/base.py` & `polyswarm-3.4.0/src/polyswarm/formatters/base.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/formatters/hashes.py` & `polyswarm-3.4.0/src/polyswarm/formatters/hashes.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/formatters/json.py` & `polyswarm-3.4.0/src/polyswarm/formatters/json.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/formatters/text.py` & `polyswarm-3.4.0/src/polyswarm/formatters/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,17 +335,25 @@
                 output.append('%s: Updated at %s' % (tool, pretty_print_datetime(metadata['updated'])))
         self._close_group()
 
         return self._output(output, write)
 
     def sandbox_providers(self, result, write=True):
         output = []
-        output.append(self._white('============================= Providers ============================='))
-        for provider in result.json['result']:
+        for provider in result.json['result'].values():
+            output.append(self._white('============================= Provider ============================='))
+            output.append(self._blue('slug: {}'.format(provider['slug'])))
             output.append(self._white('name: {}'.format(provider['name'])))
+            output.append(self._white('tool: {}'.format(provider['tool'])))
+            self._open_group()
+            for vm in provider['vms'].values():
+                output.append(self._white('============================= VM ============================='))
+                for k, v in vm.items():
+                    output.append(self._white('{}: {}'.format(k, v)))
+            self._close_group()
         return self._output(output, write)
     
     def sandbox_task(self, task, write=True):
         output = []
         output.append(self._white('============================= Sandbox Task ============================='))
         output.append(self._blue('id: {}'.format(task.id)))
         output.append(self._blue('sha256: {}'.format(task.sha256)))
```

### Comparing `polyswarm-3.3.0/src/polyswarm/polyswarm.py` & `polyswarm-3.4.0/src/polyswarm/polyswarm.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm/utils.py` & `polyswarm-3.4.0/src/polyswarm/utils.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.3.0/src/polyswarm.egg-info/PKG-INFO` & `polyswarm-3.4.0/src/polyswarm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm
-Version: 3.3.0
+Version: 3.4.0
 Summary: CLI for using the PolySwarm Customer APIs
 Home-page: https://github.com/polyswarm/polyswarm-cli
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `polyswarm-3.3.0/src/polyswarm.egg-info/SOURCES.txt` & `polyswarm-3.4.0/src/polyswarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

