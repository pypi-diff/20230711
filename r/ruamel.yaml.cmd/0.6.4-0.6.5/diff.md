# Comparing `tmp/ruamel.yaml.cmd-0.6.4.tar.gz` & `tmp/ruamel.yaml.cmd-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruamel.yaml.cmd-0.6.4.tar", last modified: Mon Jul 10 20:43:08 2023, max compression
+gzip compressed data, was "ruamel.yaml.cmd-0.6.5.tar", last modified: Tue Jul 11 18:51:22 2023, max compression
```

## Comparing `ruamel.yaml.cmd-0.6.4.tar` & `ruamel.yaml.cmd-0.6.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-07-10 20:43:08.511385 ruamel.yaml.cmd-0.6.4/
--rw-r--r--   0 anthon    (1000) users      (500)     1121 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/LICENSE
--rw-r--r--   0 anthon    (1000) users      (500)     2446 2023-07-10 20:43:08.511247 ruamel.yaml.cmd-0.6.4/PKG-INFO
--rw-r--r--   0 anthon    (1000) users      (500)     1844 2022-01-12 10:48:58.000000 ruamel.yaml.cmd-0.6.4/README.rst
--rw-r--r--   0 anthon    (1000) users      (500)    10649 2023-06-13 21:15:26.000000 ruamel.yaml.cmd-0.6.4/__init__.py
--rw-r--r--   0 anthon    (1000) users      (500)    39519 2023-06-13 21:15:28.000000 ruamel.yaml.cmd-0.6.4/__main__.py
--rw-r--r--   0 anthon    (1000) users      (500)     1734 2023-06-17 05:52:40.000000 ruamel.yaml.cmd-0.6.4/analyse.py
--rw-r--r--   0 anthon    (1000) users      (500)     3986 2023-06-17 05:55:05.000000 ruamel.yaml.cmd-0.6.4/generate.py
--rw-r--r--   0 anthon    (1000) users      (500)       97 2023-06-08 05:34:02.000000 ruamel.yaml.cmd-0.6.4/pyproject.toml
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-07-10 20:43:08.511078 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/
--rw-r--r--   0 anthon    (1000) users      (500)     2446 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/PKG-INFO
--rw-r--r--   0 anthon    (1000) users      (500)      415 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/SOURCES.txt
--rw-r--r--   0 anthon    (1000) users      (500)        1 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/dependency_links.txt
--rw-r--r--   0 anthon    (1000) users      (500)       55 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/entry_points.txt
--rw-r--r--   0 anthon    (1000) users      (500)        1 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/not-zip-safe
--rw-r--r--   0 anthon    (1000) users      (500)      100 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/requires.txt
--rw-r--r--   0 anthon    (1000) users      (500)        7 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/top_level.txt
--rw-r--r--   0 anthon    (1000) users      (500)       38 2023-07-10 20:43:08.511424 ruamel.yaml.cmd-0.6.4/setup.cfg
--rw-rw-r--   0 anthon    (1000) users      (500)    33384 2023-06-08 05:34:02.000000 ruamel.yaml.cmd-0.6.4/setup.py
--rw-r--r--   0 anthon    (1000) users      (500)     1358 2021-10-31 20:02:23.000000 ruamel.yaml.cmd-0.6.4/simpleresolver.py
--rw-r--r--   0 anthon    (1000) users      (500)    45147 2023-07-10 20:30:58.000000 ruamel.yaml.cmd-0.6.4/yaml_cmd.py
+drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-07-11 18:51:22.405215 ruamel.yaml.cmd-0.6.5/
+-rw-r--r--   0 anthon    (1000) users      (500)     1121 2023-07-11 18:51:22.000000 ruamel.yaml.cmd-0.6.5/LICENSE
+-rw-r--r--   0 anthon    (1000) users      (500)     2446 2023-07-11 18:51:22.405074 ruamel.yaml.cmd-0.6.5/PKG-INFO
+-rw-r--r--   0 anthon    (1000) users      (500)     1844 2022-01-12 10:48:58.000000 ruamel.yaml.cmd-0.6.5/README.rst
+-rw-r--r--   0 anthon    (1000) users      (500)    10649 2023-07-11 18:50:18.000000 ruamel.yaml.cmd-0.6.5/__init__.py
+-rw-r--r--   0 anthon    (1000) users      (500)    39519 2023-06-13 21:15:28.000000 ruamel.yaml.cmd-0.6.5/__main__.py
+-rw-r--r--   0 anthon    (1000) users      (500)     1734 2023-06-17 05:52:40.000000 ruamel.yaml.cmd-0.6.5/analyse.py
+-rw-r--r--   0 anthon    (1000) users      (500)     3986 2023-06-17 05:55:05.000000 ruamel.yaml.cmd-0.6.5/generate.py
+-rw-r--r--   0 anthon    (1000) users      (500)       97 2023-06-08 05:34:02.000000 ruamel.yaml.cmd-0.6.5/pyproject.toml
+drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-07-11 18:51:22.404903 ruamel.yaml.cmd-0.6.5/ruamel.yaml.cmd.egg-info/
+-rw-r--r--   0 anthon    (1000) users      (500)     2446 2023-07-11 18:51:22.000000 ruamel.yaml.cmd-0.6.5/ruamel.yaml.cmd.egg-info/PKG-INFO
+-rw-r--r--   0 anthon    (1000) users      (500)      415 2023-07-11 18:51:22.000000 ruamel.yaml.cmd-0.6.5/ruamel.yaml.cmd.egg-info/SOURCES.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        1 2023-07-11 18:51:22.000000 ruamel.yaml.cmd-0.6.5/ruamel.yaml.cmd.egg-info/dependency_links.txt
+-rw-r--r--   0 anthon    (1000) users      (500)       55 2023-07-11 18:51:22.000000 ruamel.yaml.cmd-0.6.5/ruamel.yaml.cmd.egg-info/entry_points.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        1 2023-07-11 18:51:22.000000 ruamel.yaml.cmd-0.6.5/ruamel.yaml.cmd.egg-info/not-zip-safe
+-rw-r--r--   0 anthon    (1000) users      (500)      100 2023-07-11 18:51:22.000000 ruamel.yaml.cmd-0.6.5/ruamel.yaml.cmd.egg-info/requires.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        7 2023-07-11 18:51:22.000000 ruamel.yaml.cmd-0.6.5/ruamel.yaml.cmd.egg-info/top_level.txt
+-rw-r--r--   0 anthon    (1000) users      (500)       38 2023-07-11 18:51:22.405250 ruamel.yaml.cmd-0.6.5/setup.cfg
+-rw-rw-r--   0 anthon    (1000) users      (500)    33384 2023-06-08 05:34:02.000000 ruamel.yaml.cmd-0.6.5/setup.py
+-rw-r--r--   0 anthon    (1000) users      (500)     1358 2021-10-31 20:02:23.000000 ruamel.yaml.cmd-0.6.5/simpleresolver.py
+-rw-r--r--   0 anthon    (1000) users      (500)    45299 2023-07-11 18:50:00.000000 ruamel.yaml.cmd-0.6.5/yaml_cmd.py
```

### Comparing `ruamel.yaml.cmd-0.6.4/LICENSE` & `ruamel.yaml.cmd-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ruamel.yaml.cmd-0.6.4/PKG-INFO` & `ruamel.yaml.cmd-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruamel.yaml.cmd
-Version: 0.6.4
+Version: 0.6.5
 Summary: commandline utility to manipulate YAML files
 Home-page: https://sourceforge.net/p/ruamel-yaml-cmd/code/ci/default/tree
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ruamel.yaml.cmd-0.6.4/README.rst` & `ruamel.yaml.cmd-0.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `ruamel.yaml.cmd-0.6.4/__init__.py` & `ruamel.yaml.cmd-0.6.5/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 from __future__ import print_function, absolute_import, division, unicode_literals
 
 _package_data = dict(
     full_package_name='ruamel.yaml.cmd',
-    version_info=(0, 6, 4),
-    __version__='0.6.4',
-    version_timestamp='2023-06-08 07:34:21',
+    version_info=(0, 6, 5),
+    __version__='0.6.5',
+    version_timestamp='2023-07-11 20:50:18',
     author='Anthon van der Neut',
     author_email='a.van.der.neut@ruamel.eu',
     description='commandline utility to manipulate YAML files',
     entry_points='yaml',
     license='MIT',
     since=2015,
     nested=True,
```

### Comparing `ruamel.yaml.cmd-0.6.4/__main__.py` & `ruamel.yaml.cmd-0.6.5/__main__.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml.cmd-0.6.4/analyse.py` & `ruamel.yaml.cmd-0.6.5/analyse.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml.cmd-0.6.4/generate.py` & `ruamel.yaml.cmd-0.6.5/generate.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/PKG-INFO` & `ruamel.yaml.cmd-0.6.5/ruamel.yaml.cmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruamel.yaml.cmd
-Version: 0.6.4
+Version: 0.6.5
 Summary: commandline utility to manipulate YAML files
 Home-page: https://sourceforge.net/p/ruamel-yaml-cmd/code/ci/default/tree
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ruamel.yaml.cmd-0.6.4/setup.py` & `ruamel.yaml.cmd-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml.cmd-0.6.4/simpleresolver.py` & `ruamel.yaml.cmd-0.6.5/simpleresolver.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml.cmd-0.6.4/yaml_cmd.py` & `ruamel.yaml.cmd-0.6.5/yaml_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,27 +508,33 @@
         # print('dfs', dfs)
         yaml.default_flow_style = dfs
         yaml.dump_all(docs, sys.stdout)
         return 1 if errors else 0
 
     @staticmethod
     def json_load(inp):
-        import orjson
+        try:
+            import orjson as json
+        except ImportError:
+            import json
 
-        return orjson.loads(inp)
+        return json.loads(inp)
 
     def _from_line_json(self, inp):
         """parse line json (i.e. one json document per line) and convert to
            list of loaded constructs"""
         # yaml = ruamel.yaml.YAML(type='safe')
-        import ujson
+        try:
+            import orjson as json
+        except ImportError:
+            import json
 
         data = []
         for line in inp.splitlines():
-            data.append(ujson.loads(line))
+            data.append(json.loads(line))
         return data
 
     def pickle(self):
         import pickle
 
         # import dill as pickle
         data = []
```

