# Comparing `tmp/bondzai.bootstrap-framework-0.0.8.tar.gz` & `tmp/bondzai.bootstrap-framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.bootstrap-framework-0.0.8.tar", last modified: Wed Jul  5 12:40:50 2023, max compression
+gzip compressed data, was "bondzai.bootstrap-framework-0.0.9.tar", last modified: Mon Jul 10 17:59:32 2023, max compression
```

## Comparing `bondzai.bootstrap-framework-0.0.8.tar` & `bondzai.bootstrap-framework-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-05 12:40:50.981659 bondzai.bootstrap-framework-0.0.8/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-05 12:40:50.981807 bondzai.bootstrap-framework-0.0.8/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      141 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-05 12:40:50.976828 bondzai.bootstrap-framework-0.0.8/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-05 12:40:50.979543 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/
--rw-r--r--   0 theo       (501) staff       (20)      212 2023-07-05 12:40:42.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     2696 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/bootstrap.py
--rw-r--r--   0 theo       (501) staff       (20)    11284 2023-07-05 12:40:42.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_agent.py
--rw-r--r--   0 theo       (501) staff       (20)    14052 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_com.py
--rw-r--r--   0 theo       (501) staff       (20)     8285 2023-07-05 12:40:42.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_config.py
--rw-r--r--   0 theo       (501) staff       (20)     3008 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/file_handler.py
--rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/logger.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-05 12:40:50.981445 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      578 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       52 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-05 12:40:50.000000 bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-05 12:40:15.000000 bondzai.bootstrap-framework-0.0.8/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      755 2023-07-05 12:40:50.982367 bondzai.bootstrap-framework-0.0.8/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:32.883623 bondzai.bootstrap-framework-0.0.9/
+-rwxrwxrwx   0 root         (0) root         (0)      547 2023-07-10 17:56:54.000000 bondzai.bootstrap-framework-0.0.9/NOTICE
+-rwxrwxrwx   0 root         (0) root         (0)      578 2023-07-10 17:59:32.884132 bondzai.bootstrap-framework-0.0.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      141 2023-07-10 17:56:54.000000 bondzai.bootstrap-framework-0.0.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:32.349617 bondzai.bootstrap-framework-0.0.9/bondzai/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:32.655890 bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/
+-rwxrwxrwx   0 root         (0) root         (0)      212 2023-07-10 17:59:21.000000 bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2696 2023-07-10 17:56:54.000000 bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/bootstrap.py
+-rwxrwxrwx   0 root         (0) root         (0)    11284 2023-07-10 17:56:54.000000 bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/dvs_agent.py
+-rwxrwxrwx   0 root         (0) root         (0)    14052 2023-07-10 17:56:54.000000 bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/dvs_com.py
+-rwxrwxrwx   0 root         (0) root         (0)     8285 2023-07-10 17:56:54.000000 bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/dvs_config.py
+-rwxrwxrwx   0 root         (0) root         (0)     3008 2023-07-10 17:56:54.000000 bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/file_handler.py
+-rwxrwxrwx   0 root         (0) root         (0)      333 2023-07-10 17:56:54.000000 bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/logger.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:32.857707 bondzai.bootstrap-framework-0.0.9/bondzai.bootstrap_framework.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      578 2023-07-10 17:59:32.000000 bondzai.bootstrap-framework-0.0.9/bondzai.bootstrap_framework.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      700 2023-07-10 17:59:32.000000 bondzai.bootstrap-framework-0.0.9/bondzai.bootstrap_framework.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 17:59:32.000000 bondzai.bootstrap-framework-0.0.9/bondzai.bootstrap_framework.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-07-10 17:59:32.000000 bondzai.bootstrap-framework-0.0.9/bondzai.bootstrap_framework.egg-info/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-07-10 17:59:32.000000 bondzai.bootstrap-framework-0.0.9/bondzai.bootstrap_framework.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-10 17:59:32.000000 bondzai.bootstrap-framework-0.0.9/bondzai.bootstrap_framework.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 17:59:31.000000 bondzai.bootstrap-framework-0.0.9/bondzai.bootstrap_framework.egg-info/zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-07-10 17:56:54.000000 bondzai.bootstrap-framework-0.0.9/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      755 2023-07-10 17:59:32.888137 bondzai.bootstrap-framework-0.0.9/setup.cfg
```

### Comparing `bondzai.bootstrap-framework-0.0.8/NOTICE` & `bondzai.bootstrap-framework-0.0.9/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.8/PKG-INFO` & `bondzai.bootstrap-framework-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/bootstrap.py` & `bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_agent.py` & `bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/dvs_agent.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_com.py` & `bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/dvs_com.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/dvs_config.py` & `bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/dvs_config.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.8/bondzai/bootstrap_framework/file_handler.py` & `bondzai.bootstrap-framework-0.0.9/bondzai/bootstrap_framework/file_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/PKG-INFO` & `bondzai.bootstrap-framework-0.0.9/bondzai.bootstrap_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.bootstrap-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bondzai Bootstrap Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.bootstrap-framework-0.0.8/bondzai.bootstrap_framework.egg-info/SOURCES.txt` & `bondzai.bootstrap-framework-0.0.9/bondzai.bootstrap_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.bootstrap-framework-0.0.8/setup.cfg` & `bondzai.bootstrap-framework-0.0.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 package_dir = 
 	= .
 zip_safe = True
 include_package_data = True
 namespace_packages = 
 	bondzai
 install_requires = 
-	bondzai.davinsy-py==0.0.4
+	bondzai.davinsy-py==0.0.5
 	numpy==1.24.3
 	pyyaml==6.0
 
 [options.packages.find]
 where = .
 
 [egg_info]
```

