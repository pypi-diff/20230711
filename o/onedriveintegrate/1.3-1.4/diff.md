# Comparing `tmp/onedriveintegrate-1.3.tar.gz` & `tmp/onedriveintegrate-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedriveintegrate-1.3.tar", last modified: Tue Jul 11 04:09:53 2023, max compression
+gzip compressed data, was "onedriveintegrate-1.4.tar", last modified: Tue Jul 11 05:46:00 2023, max compression
```

## Comparing `onedriveintegrate-1.3.tar` & `onedriveintegrate-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 04:09:53.673353 onedriveintegrate-1.3/
--rw-r--r--   0 william2399   (501) staff       (20)     2921 2023-07-11 04:09:53.672799 onedriveintegrate-1.3/PKG-INFO
--rw-r--r--   0 william2399   (501) staff       (20)     2742 2023-07-11 04:09:39.000000 onedriveintegrate-1.3/README.md
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 04:09:53.666751 onedriveintegrate-1.3/onedriveintegrate/
--rw-r--r--   0 william2399   (501) staff       (20)      101 2023-07-10 21:56:34.000000 onedriveintegrate-1.3/onedriveintegrate/__init__.py
--rw-r--r--   0 william2399   (501) staff       (20)     1798 2023-07-11 03:27:58.000000 onedriveintegrate-1.3/onedriveintegrate/ms_graph.py
--rw-r--r--   0 william2399   (501) staff       (20)     4299 2023-07-11 03:45:08.000000 onedriveintegrate-1.3/onedriveintegrate/onedrive_api.py
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 04:09:53.672127 onedriveintegrate-1.3/onedriveintegrate.egg-info/
--rw-r--r--   0 william2399   (501) staff       (20)     2921 2023-07-11 04:09:53.000000 onedriveintegrate-1.3/onedriveintegrate.egg-info/PKG-INFO
--rw-r--r--   0 william2399   (501) staff       (20)      316 2023-07-11 04:09:53.000000 onedriveintegrate-1.3/onedriveintegrate.egg-info/SOURCES.txt
--rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 04:09:53.000000 onedriveintegrate-1.3/onedriveintegrate.egg-info/dependency_links.txt
--rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 01:43:05.000000 onedriveintegrate-1.3/onedriveintegrate.egg-info/not-zip-safe
--rw-r--r--   0 william2399   (501) staff       (20)       18 2023-07-11 04:09:53.000000 onedriveintegrate-1.3/onedriveintegrate.egg-info/top_level.txt
--rw-r--r--   0 william2399   (501) staff       (20)       38 2023-07-11 04:09:53.673506 onedriveintegrate-1.3/setup.cfg
--rw-r--r--   0 william2399   (501) staff       (20)      512 2023-07-11 04:09:49.000000 onedriveintegrate-1.3/setup.py
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 05:46:00.273348 onedriveintegrate-1.4/
+-rw-r--r--   0 william2399   (501) staff       (20)     2895 2023-07-11 05:46:00.272886 onedriveintegrate-1.4/PKG-INFO
+-rw-r--r--   0 william2399   (501) staff       (20)     2716 2023-07-11 05:45:36.000000 onedriveintegrate-1.4/README.md
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 05:46:00.264935 onedriveintegrate-1.4/onedriveintegrate/
+-rw-r--r--   0 william2399   (501) staff       (20)      101 2023-07-10 21:56:34.000000 onedriveintegrate-1.4/onedriveintegrate/__init__.py
+-rw-r--r--   0 william2399   (501) staff       (20)     1798 2023-07-11 03:27:58.000000 onedriveintegrate-1.4/onedriveintegrate/ms_graph.py
+-rw-r--r--   0 william2399   (501) staff       (20)     4299 2023-07-11 03:45:08.000000 onedriveintegrate-1.4/onedriveintegrate/onedrive_api.py
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 05:46:00.272130 onedriveintegrate-1.4/onedriveintegrate.egg-info/
+-rw-r--r--   0 william2399   (501) staff       (20)     2895 2023-07-11 05:45:59.000000 onedriveintegrate-1.4/onedriveintegrate.egg-info/PKG-INFO
+-rw-r--r--   0 william2399   (501) staff       (20)      316 2023-07-11 05:46:00.000000 onedriveintegrate-1.4/onedriveintegrate.egg-info/SOURCES.txt
+-rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 05:45:59.000000 onedriveintegrate-1.4/onedriveintegrate.egg-info/dependency_links.txt
+-rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 01:43:05.000000 onedriveintegrate-1.4/onedriveintegrate.egg-info/not-zip-safe
+-rw-r--r--   0 william2399   (501) staff       (20)       18 2023-07-11 05:45:59.000000 onedriveintegrate-1.4/onedriveintegrate.egg-info/top_level.txt
+-rw-r--r--   0 william2399   (501) staff       (20)       38 2023-07-11 05:46:00.273494 onedriveintegrate-1.4/setup.cfg
+-rw-r--r--   0 william2399   (501) staff       (20)      512 2023-07-11 05:45:45.000000 onedriveintegrate-1.4/setup.py
```

### Comparing `onedriveintegrate-1.3/PKG-INFO` & `onedriveintegrate-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: onedriveintegrate
-Version: 1.3
+Version: 1.4
 Summary: Package for OneDrive File Management
 Author: William Guo
 License: MIT
 Description-Content-Type: text/markdown
 
 # OneDrive Integration Package
 ___
-_onedriveintegrate_ is a Python package for OneDrive functionality, featuring methods for OneDrive file management and interacting Microsoft
-OneDrive API.
+_onedriveintegrate_ is a Python package for OneDrive functionality, featuring methods for OneDrive file management.
 
 List of relevant operations:
 * Authenticate users using Microsoft Graph API
 * Write files to a folder
 * Read files from the drive
 * List contents of a folder
 * Search for files based on text/id
@@ -22,14 +21,15 @@
 ___
 Use a simple [pip](https://pip.pypa.io/en/stable/) command to install _onedriveintegrate_: 
 ```bash
 pip install onedriveintegrate
 ```
 
 ## Usage / Getting started
+___
 ```python
 from onedriveintegrate.onedrive_api import OneDriveAPI
 from onedriveintegrate.ms_graph import generate_access_token, GRAPH_API_ENDPOINT
 
 # User's Client ID
 client_ID = 'XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX'
 
@@ -52,15 +52,15 @@
 
 # 4) Search item based on search text/id, results storted in output_file
 onedrive_query.search_text(search_txt, output_file)
 onedrive_query.search_id(file_id OR folder_id, output_file)
 ```
 
 ## Helpful Resources
-
+___
 Sources from Jie Jenn:
 * [Upload Files to One Drive using Microsoft Graph API in Python](https://www.youtube.com/watch?v=Ok8O_QnrSBI)
 * [Download Files from OneDrive Using Microsoft Graph API in Python](https://www.youtube.com/watch?v=w6YeOkikVFI)
 * [Source Code for ms_graph.py](https://learndataanalysis.org/ms_graph-py-source-code/)
 
 Microsoft Graph API:
 * [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
@@ -73,13 +73,13 @@
 * [PyPi.org](https://pypi.org/)
 
 Markdown:
 * [Make a README](https://www.makeareadme.com/)
 * [How to write a good README](https://dev.to/merlos/how-to-write-a-good-readme-bog)
 
 ## Acknowledgements
-
+___
 This package makes use of Jie Jenn's ms_graph.py for the user authentication process.
 
 ## License
-
+___
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `onedriveintegrate-1.3/README.md` & `onedriveintegrate-1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # OneDrive Integration Package
 ___
-_onedriveintegrate_ is a Python package for OneDrive functionality, featuring methods for OneDrive file management and interacting Microsoft
-OneDrive API.
+_onedriveintegrate_ is a Python package for OneDrive functionality, featuring methods for OneDrive file management.
 
 List of relevant operations:
 * Authenticate users using Microsoft Graph API
 * Write files to a folder
 * Read files from the drive
 * List contents of a folder
 * Search for files based on text/id
@@ -14,14 +13,15 @@
 ___
 Use a simple [pip](https://pip.pypa.io/en/stable/) command to install _onedriveintegrate_: 
 ```bash
 pip install onedriveintegrate
 ```
 
 ## Usage / Getting started
+___
 ```python
 from onedriveintegrate.onedrive_api import OneDriveAPI
 from onedriveintegrate.ms_graph import generate_access_token, GRAPH_API_ENDPOINT
 
 # User's Client ID
 client_ID = 'XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX'
 
@@ -44,15 +44,15 @@
 
 # 4) Search item based on search text/id, results storted in output_file
 onedrive_query.search_text(search_txt, output_file)
 onedrive_query.search_id(file_id OR folder_id, output_file)
 ```
 
 ## Helpful Resources
-
+___
 Sources from Jie Jenn:
 * [Upload Files to One Drive using Microsoft Graph API in Python](https://www.youtube.com/watch?v=Ok8O_QnrSBI)
 * [Download Files from OneDrive Using Microsoft Graph API in Python](https://www.youtube.com/watch?v=w6YeOkikVFI)
 * [Source Code for ms_graph.py](https://learndataanalysis.org/ms_graph-py-source-code/)
 
 Microsoft Graph API:
 * [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
@@ -65,13 +65,13 @@
 * [PyPi.org](https://pypi.org/)
 
 Markdown:
 * [Make a README](https://www.makeareadme.com/)
 * [How to write a good README](https://dev.to/merlos/how-to-write-a-good-readme-bog)
 
 ## Acknowledgements
-
+___
 This package makes use of Jie Jenn's ms_graph.py for the user authentication process.
 
 ## License
-
+___
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `onedriveintegrate-1.3/onedriveintegrate/ms_graph.py` & `onedriveintegrate-1.4/onedriveintegrate/ms_graph.py`

 * *Files identical despite different names*

### Comparing `onedriveintegrate-1.3/onedriveintegrate/onedrive_api.py` & `onedriveintegrate-1.4/onedriveintegrate/onedrive_api.py`

 * *Files identical despite different names*

### Comparing `onedriveintegrate-1.3/onedriveintegrate.egg-info/PKG-INFO` & `onedriveintegrate-1.4/onedriveintegrate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: onedriveintegrate
-Version: 1.3
+Version: 1.4
 Summary: Package for OneDrive File Management
 Author: William Guo
 License: MIT
 Description-Content-Type: text/markdown
 
 # OneDrive Integration Package
 ___
-_onedriveintegrate_ is a Python package for OneDrive functionality, featuring methods for OneDrive file management and interacting Microsoft
-OneDrive API.
+_onedriveintegrate_ is a Python package for OneDrive functionality, featuring methods for OneDrive file management.
 
 List of relevant operations:
 * Authenticate users using Microsoft Graph API
 * Write files to a folder
 * Read files from the drive
 * List contents of a folder
 * Search for files based on text/id
@@ -22,14 +21,15 @@
 ___
 Use a simple [pip](https://pip.pypa.io/en/stable/) command to install _onedriveintegrate_: 
 ```bash
 pip install onedriveintegrate
 ```
 
 ## Usage / Getting started
+___
 ```python
 from onedriveintegrate.onedrive_api import OneDriveAPI
 from onedriveintegrate.ms_graph import generate_access_token, GRAPH_API_ENDPOINT
 
 # User's Client ID
 client_ID = 'XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX'
 
@@ -52,15 +52,15 @@
 
 # 4) Search item based on search text/id, results storted in output_file
 onedrive_query.search_text(search_txt, output_file)
 onedrive_query.search_id(file_id OR folder_id, output_file)
 ```
 
 ## Helpful Resources
-
+___
 Sources from Jie Jenn:
 * [Upload Files to One Drive using Microsoft Graph API in Python](https://www.youtube.com/watch?v=Ok8O_QnrSBI)
 * [Download Files from OneDrive Using Microsoft Graph API in Python](https://www.youtube.com/watch?v=w6YeOkikVFI)
 * [Source Code for ms_graph.py](https://learndataanalysis.org/ms_graph-py-source-code/)
 
 Microsoft Graph API:
 * [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
@@ -73,13 +73,13 @@
 * [PyPi.org](https://pypi.org/)
 
 Markdown:
 * [Make a README](https://www.makeareadme.com/)
 * [How to write a good README](https://dev.to/merlos/how-to-write-a-good-readme-bog)
 
 ## Acknowledgements
-
+___
 This package makes use of Jie Jenn's ms_graph.py for the user authentication process.
 
 ## License
-
+___
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `onedriveintegrate-1.3/setup.py` & `onedriveintegrate-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Read contents of README.md file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
       name='onedriveintegrate',
-      version='1.3',
+      version='1.4',
       long_description=long_description,
       long_description_content_type='text/markdown',
       description='Package for OneDrive File Management',
       author='William Guo',
       license='MIT',
       packages=['onedriveintegrate'],
       zip_safe=False
```

