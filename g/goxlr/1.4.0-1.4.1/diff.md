# Comparing `tmp/goxlr-1.4.0.tar.gz` & `tmp/goxlr-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.4.0.tar", last modified: Mon Jul 10 22:34:16 2023, max compression
+gzip compressed data, was "goxlr-1.4.1.tar", last modified: Tue Jul 11 12:56:42 2023, max compression
```

## Comparing `goxlr-1.4.0.tar` & `goxlr-1.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:34:16.078720 goxlr-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-10 22:34:06.000000 goxlr-1.4.0/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 22:34:06.000000 goxlr-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-10 22:34:16.078720 goxlr-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-10 22:34:06.000000 goxlr-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:34:16.078720 goxlr-1.4.0/goxlr/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:34:16.078720 goxlr-1.4.0/goxlr/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/commands/goxlr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:34:16.078720 goxlr-1.4.0/goxlr/types/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/types/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-10 22:34:06.000000 goxlr-1.4.0/goxlr/types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:34:16.078720 goxlr-1.4.0/goxlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-10 22:34:16.000000 goxlr-1.4.0/goxlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-10 22:34:16.000000 goxlr-1.4.0/goxlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:34:16.000000 goxlr-1.4.0/goxlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 22:34:16.000000 goxlr-1.4.0/goxlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 22:34:16.000000 goxlr-1.4.0/goxlr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 22:34:06.000000 goxlr-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 22:34:16.078720 goxlr-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-10 22:34:06.000000 goxlr-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:42.517770 goxlr-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-11 12:56:31.000000 goxlr-1.4.1/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 12:56:31.000000 goxlr-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 12:56:42.517770 goxlr-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-11 12:56:31.000000 goxlr-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:42.517770 goxlr-1.4.1/goxlr/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:42.517770 goxlr-1.4.1/goxlr/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/commands/goxlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:42.517770 goxlr-1.4.1/goxlr/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/types/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-11 12:56:31.000000 goxlr-1.4.1/goxlr/types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:42.517770 goxlr-1.4.1/goxlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-11 12:56:42.000000 goxlr-1.4.1/goxlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 12:56:42.000000 goxlr-1.4.1/goxlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:56:42.000000 goxlr-1.4.1/goxlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 12:56:42.000000 goxlr-1.4.1/goxlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 12:56:42.000000 goxlr-1.4.1/goxlr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 12:56:31.000000 goxlr-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 12:56:42.517770 goxlr-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-11 12:56:31.000000 goxlr-1.4.1/setup.py
```

### Comparing `goxlr-1.4.0/LICENSE-3RD-PARTY.txt` & `goxlr-1.4.1/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.0/LICENSE.txt` & `goxlr-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.0/PKG-INFO` & `goxlr-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python wrapper for the GoXLR Utility API.
-Home-page: https://github.com/samcarsonx/goxlr
+Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE-3RD-PARTY.txt
 License-File: LICENSE.txt
```

### Comparing `goxlr-1.4.0/README.md` & `goxlr-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.0/goxlr/commands/daemon.py` & `goxlr-1.4.1/goxlr/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.0/goxlr/commands/goxlr.py` & `goxlr-1.4.1/goxlr/commands/goxlr.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.0/goxlr/commands/status.py` & `goxlr-1.4.1/goxlr/commands/status.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.0/goxlr/socket.py` & `goxlr-1.4.1/goxlr/socket.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.0/goxlr/types/enums.py` & `goxlr-1.4.1/goxlr/types/enums.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.0/goxlr/types/models.py` & `goxlr-1.4.1/goxlr/types/models.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.0/goxlr.egg-info/PKG-INFO` & `goxlr-1.4.1/goxlr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python wrapper for the GoXLR Utility API.
-Home-page: https://github.com/samcarsonx/goxlr
+Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE-3RD-PARTY.txt
 License-File: LICENSE.txt
```

### Comparing `goxlr-1.4.0/setup.py` & `goxlr-1.4.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 setup(
     name="goxlr",
     version=verstr,
     description="A Python wrapper for the GoXLR Utility API.",
-    url="https://github.com/samcarsonx/goxlr",
+    url="https://github.com/samcarsonx/goxlr-py",
     author="Sam Carson",
     author_email="sam@samcarson.co.uk",
     license="MIT",
     packages=find_packages(),
     install_requires=["asyncio", "websockets"],
     python_requires=">=3.10",
     long_description=open("README.md").read(),
```

