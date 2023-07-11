# Comparing `tmp/onedriveintegrate-1.2.tar.gz` & `tmp/onedriveintegrate-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedriveintegrate-1.2.tar", last modified: Tue Jul 11 04:06:10 2023, max compression
+gzip compressed data, was "onedriveintegrate-1.3.tar", last modified: Tue Jul 11 04:09:53 2023, max compression
```

## Comparing `onedriveintegrate-1.2.tar` & `onedriveintegrate-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 04:06:10.351458 onedriveintegrate-1.2/
--rw-r--r--   0 william2399   (501) staff       (20)     2784 2023-07-11 04:06:10.350993 onedriveintegrate-1.2/PKG-INFO
--rw-r--r--   0 william2399   (501) staff       (20)     2605 2023-07-11 04:05:05.000000 onedriveintegrate-1.2/README.md
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 04:06:10.324034 onedriveintegrate-1.2/onedriveintegrate/
--rw-r--r--   0 william2399   (501) staff       (20)      101 2023-07-10 21:56:34.000000 onedriveintegrate-1.2/onedriveintegrate/__init__.py
--rw-r--r--   0 william2399   (501) staff       (20)     1798 2023-07-11 03:27:58.000000 onedriveintegrate-1.2/onedriveintegrate/ms_graph.py
--rw-r--r--   0 william2399   (501) staff       (20)     4299 2023-07-11 03:45:08.000000 onedriveintegrate-1.2/onedriveintegrate/onedrive_api.py
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 04:06:10.350240 onedriveintegrate-1.2/onedriveintegrate.egg-info/
--rw-r--r--   0 william2399   (501) staff       (20)     2784 2023-07-11 04:06:10.000000 onedriveintegrate-1.2/onedriveintegrate.egg-info/PKG-INFO
--rw-r--r--   0 william2399   (501) staff       (20)      316 2023-07-11 04:06:10.000000 onedriveintegrate-1.2/onedriveintegrate.egg-info/SOURCES.txt
--rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 04:06:10.000000 onedriveintegrate-1.2/onedriveintegrate.egg-info/dependency_links.txt
--rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 01:43:05.000000 onedriveintegrate-1.2/onedriveintegrate.egg-info/not-zip-safe
--rw-r--r--   0 william2399   (501) staff       (20)       18 2023-07-11 04:06:10.000000 onedriveintegrate-1.2/onedriveintegrate.egg-info/top_level.txt
--rw-r--r--   0 william2399   (501) staff       (20)       38 2023-07-11 04:06:10.351611 onedriveintegrate-1.2/setup.cfg
--rw-r--r--   0 william2399   (501) staff       (20)      512 2023-07-11 04:06:00.000000 onedriveintegrate-1.2/setup.py
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 04:09:53.673353 onedriveintegrate-1.3/
+-rw-r--r--   0 william2399   (501) staff       (20)     2921 2023-07-11 04:09:53.672799 onedriveintegrate-1.3/PKG-INFO
+-rw-r--r--   0 william2399   (501) staff       (20)     2742 2023-07-11 04:09:39.000000 onedriveintegrate-1.3/README.md
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 04:09:53.666751 onedriveintegrate-1.3/onedriveintegrate/
+-rw-r--r--   0 william2399   (501) staff       (20)      101 2023-07-10 21:56:34.000000 onedriveintegrate-1.3/onedriveintegrate/__init__.py
+-rw-r--r--   0 william2399   (501) staff       (20)     1798 2023-07-11 03:27:58.000000 onedriveintegrate-1.3/onedriveintegrate/ms_graph.py
+-rw-r--r--   0 william2399   (501) staff       (20)     4299 2023-07-11 03:45:08.000000 onedriveintegrate-1.3/onedriveintegrate/onedrive_api.py
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 04:09:53.672127 onedriveintegrate-1.3/onedriveintegrate.egg-info/
+-rw-r--r--   0 william2399   (501) staff       (20)     2921 2023-07-11 04:09:53.000000 onedriveintegrate-1.3/onedriveintegrate.egg-info/PKG-INFO
+-rw-r--r--   0 william2399   (501) staff       (20)      316 2023-07-11 04:09:53.000000 onedriveintegrate-1.3/onedriveintegrate.egg-info/SOURCES.txt
+-rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 04:09:53.000000 onedriveintegrate-1.3/onedriveintegrate.egg-info/dependency_links.txt
+-rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 01:43:05.000000 onedriveintegrate-1.3/onedriveintegrate.egg-info/not-zip-safe
+-rw-r--r--   0 william2399   (501) staff       (20)       18 2023-07-11 04:09:53.000000 onedriveintegrate-1.3/onedriveintegrate.egg-info/top_level.txt
+-rw-r--r--   0 william2399   (501) staff       (20)       38 2023-07-11 04:09:53.673506 onedriveintegrate-1.3/setup.cfg
+-rw-r--r--   0 william2399   (501) staff       (20)      512 2023-07-11 04:09:49.000000 onedriveintegrate-1.3/setup.py
```

### Comparing `onedriveintegrate-1.2/PKG-INFO` & `onedriveintegrate-1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedriveintegrate
-Version: 1.2
+Version: 1.3
 Summary: Package for OneDrive File Management
 Author: William Guo
 License: MIT
 Description-Content-Type: text/markdown
 
 # OneDrive Integration Package
 ___
@@ -62,14 +62,15 @@
 * [Download Files from OneDrive Using Microsoft Graph API in Python](https://www.youtube.com/watch?v=w6YeOkikVFI)
 * [Source Code for ms_graph.py](https://learndataanalysis.org/ms_graph-py-source-code/)
 
 Microsoft Graph API:
 * [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
 * [Microsoft Azure Portal](https://azure.microsoft.com/en-us/get-started/azure-portal)
 * [Overview of Microsoft Graph - Documentation](https://learn.microsoft.com/en-us/graph/overview?view=graph-rest-1.0)
+* [How to Upload Files to OneDrive](https://learn.microsoft.com/en-us/training/modules/msgraph-access-file-data/4-upload-files-onedrive)
 
 PyPi:
 * [Build a Python Module and Share it with Pip Install](https://www.youtube.com/watch?v=FkmtmYFTlYE)
 * [PyPi.org](https://pypi.org/)
 
 Markdown:
 * [Make a README](https://www.makeareadme.com/)
```

### Comparing `onedriveintegrate-1.2/README.md` & `onedriveintegrate-1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 * [Download Files from OneDrive Using Microsoft Graph API in Python](https://www.youtube.com/watch?v=w6YeOkikVFI)
 * [Source Code for ms_graph.py](https://learndataanalysis.org/ms_graph-py-source-code/)
 
 Microsoft Graph API:
 * [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
 * [Microsoft Azure Portal](https://azure.microsoft.com/en-us/get-started/azure-portal)
 * [Overview of Microsoft Graph - Documentation](https://learn.microsoft.com/en-us/graph/overview?view=graph-rest-1.0)
+* [How to Upload Files to OneDrive](https://learn.microsoft.com/en-us/training/modules/msgraph-access-file-data/4-upload-files-onedrive)
 
 PyPi:
 * [Build a Python Module and Share it with Pip Install](https://www.youtube.com/watch?v=FkmtmYFTlYE)
 * [PyPi.org](https://pypi.org/)
 
 Markdown:
 * [Make a README](https://www.makeareadme.com/)
```

### Comparing `onedriveintegrate-1.2/onedriveintegrate/ms_graph.py` & `onedriveintegrate-1.3/onedriveintegrate/ms_graph.py`

 * *Files identical despite different names*

### Comparing `onedriveintegrate-1.2/onedriveintegrate/onedrive_api.py` & `onedriveintegrate-1.3/onedriveintegrate/onedrive_api.py`

 * *Files identical despite different names*

### Comparing `onedriveintegrate-1.2/onedriveintegrate.egg-info/PKG-INFO` & `onedriveintegrate-1.3/onedriveintegrate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedriveintegrate
-Version: 1.2
+Version: 1.3
 Summary: Package for OneDrive File Management
 Author: William Guo
 License: MIT
 Description-Content-Type: text/markdown
 
 # OneDrive Integration Package
 ___
@@ -62,14 +62,15 @@
 * [Download Files from OneDrive Using Microsoft Graph API in Python](https://www.youtube.com/watch?v=w6YeOkikVFI)
 * [Source Code for ms_graph.py](https://learndataanalysis.org/ms_graph-py-source-code/)
 
 Microsoft Graph API:
 * [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
 * [Microsoft Azure Portal](https://azure.microsoft.com/en-us/get-started/azure-portal)
 * [Overview of Microsoft Graph - Documentation](https://learn.microsoft.com/en-us/graph/overview?view=graph-rest-1.0)
+* [How to Upload Files to OneDrive](https://learn.microsoft.com/en-us/training/modules/msgraph-access-file-data/4-upload-files-onedrive)
 
 PyPi:
 * [Build a Python Module and Share it with Pip Install](https://www.youtube.com/watch?v=FkmtmYFTlYE)
 * [PyPi.org](https://pypi.org/)
 
 Markdown:
 * [Make a README](https://www.makeareadme.com/)
```

### Comparing `onedriveintegrate-1.2/setup.py` & `onedriveintegrate-1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Read contents of README.md file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
       name='onedriveintegrate',
-      version='1.2',
+      version='1.3',
       long_description=long_description,
       long_description_content_type='text/markdown',
       description='Package for OneDrive File Management',
       author='William Guo',
       license='MIT',
       packages=['onedriveintegrate'],
       zip_safe=False
```

