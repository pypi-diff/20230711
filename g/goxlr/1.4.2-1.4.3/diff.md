# Comparing `tmp/goxlr-1.4.2.tar.gz` & `tmp/goxlr-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.4.2.tar", last modified: Tue Jul 11 14:12:13 2023, max compression
+gzip compressed data, was "goxlr-1.4.3.tar", last modified: Tue Jul 11 16:57:57 2023, max compression
```

## Comparing `goxlr-1.4.2.tar` & `goxlr-1.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:12:13.123291 goxlr-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-11 14:11:59.000000 goxlr-1.4.2/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 14:11:59.000000 goxlr-1.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 14:12:13.123291 goxlr-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-11 14:11:59.000000 goxlr-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:12:13.119291 goxlr-1.4.2/goxlr/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:12:13.123291 goxlr-1.4.2/goxlr/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/commands/goxlr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:12:13.123291 goxlr-1.4.2/goxlr/types/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/types/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-11 14:11:59.000000 goxlr-1.4.2/goxlr/types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:12:13.119291 goxlr-1.4.2/goxlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 14:12:13.000000 goxlr-1.4.2/goxlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 14:12:13.000000 goxlr-1.4.2/goxlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:12:13.000000 goxlr-1.4.2/goxlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 14:12:13.000000 goxlr-1.4.2/goxlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:12:13.000000 goxlr-1.4.2/goxlr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 14:11:59.000000 goxlr-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 14:12:13.123291 goxlr-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-11 14:11:59.000000 goxlr-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:57.344742 goxlr-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-11 16:57:45.000000 goxlr-1.4.3/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 16:57:45.000000 goxlr-1.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 16:57:57.344742 goxlr-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-11 16:57:45.000000 goxlr-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:57.340742 goxlr-1.4.3/goxlr/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:57.344742 goxlr-1.4.3/goxlr/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/commands/goxlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:57.344742 goxlr-1.4.3/goxlr/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/types/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-11 16:57:45.000000 goxlr-1.4.3/goxlr/types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:57:57.340742 goxlr-1.4.3/goxlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 16:57:57.000000 goxlr-1.4.3/goxlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 16:57:57.000000 goxlr-1.4.3/goxlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:57:57.000000 goxlr-1.4.3/goxlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 16:57:57.000000 goxlr-1.4.3/goxlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 16:57:57.000000 goxlr-1.4.3/goxlr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 16:57:45.000000 goxlr-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 16:57:57.344742 goxlr-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-11 16:57:45.000000 goxlr-1.4.3/setup.py
```

### Comparing `goxlr-1.4.2/LICENSE-3RD-PARTY.txt` & `goxlr-1.4.3/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.2/LICENSE.txt` & `goxlr-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.2/PKG-INFO` & `goxlr-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `goxlr-1.4.2/README.md` & `goxlr-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.2/goxlr/commands/daemon.py` & `goxlr-1.4.3/goxlr/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.2/goxlr/commands/goxlr.py` & `goxlr-1.4.3/goxlr/commands/goxlr.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.2/goxlr/commands/status.py` & `goxlr-1.4.3/goxlr/commands/status.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.2/goxlr/socket.py` & `goxlr-1.4.3/goxlr/socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
         :param update: Whether or not to update the status and mixers attributes
                        after receiving the patch.
 
         :return: The patch from the daemon.
         """
 
-        patches = await self.receive_patch()
+        patches = await Socket.receive_patch(self)
 
         if update:
             await self.update()
 
         return patches
 
     def select_mixer(self, serial: str = None):
```

### Comparing `goxlr-1.4.2/goxlr/types/enums.py` & `goxlr-1.4.3/goxlr/types/enums.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.2/goxlr/types/models.py` & `goxlr-1.4.3/goxlr/types/models.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.2/goxlr.egg-info/PKG-INFO` & `goxlr-1.4.3/goxlr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `goxlr-1.4.2/setup.py` & `goxlr-1.4.3/setup.py`

 * *Files identical despite different names*

