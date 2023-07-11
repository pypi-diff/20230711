# Comparing `tmp/onedrive-integration-1.2.tar.gz` & `tmp/onedrive-integration-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedrive-integration-1.2.tar", last modified: Tue Jul 11 01:09:54 2023, max compression
+gzip compressed data, was "onedrive-integration-1.3.tar", last modified: Tue Jul 11 01:12:24 2023, max compression
```

## Comparing `onedrive-integration-1.2.tar` & `onedrive-integration-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 01:09:54.762834 onedrive-integration-1.2/
--rw-r--r--   0 william2399   (501) staff       (20)     1454 2023-07-11 01:09:54.762345 onedrive-integration-1.2/PKG-INFO
--rw-r--r--   0 william2399   (501) staff       (20)     1272 2023-07-11 01:09:33.000000 onedrive-integration-1.2/README.md
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 01:09:54.754567 onedrive-integration-1.2/onedrive-integration/
--rw-r--r--   0 william2399   (501) staff       (20)      101 2023-07-10 21:56:34.000000 onedrive-integration-1.2/onedrive-integration/__init__.py
--rw-r--r--   0 william2399   (501) staff       (20)     1798 2023-07-11 00:16:53.000000 onedrive-integration-1.2/onedrive-integration/ms_graph.py
--rw-r--r--   0 william2399   (501) staff       (20)     2375 2023-07-10 21:54:31.000000 onedrive-integration-1.2/onedrive-integration/onedrive_api.py
-drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 01:09:54.761426 onedrive-integration-1.2/onedrive_integration.egg-info/
--rw-r--r--   0 william2399   (501) staff       (20)     1454 2023-07-11 01:09:54.000000 onedrive-integration-1.2/onedrive_integration.egg-info/PKG-INFO
--rw-r--r--   0 william2399   (501) staff       (20)      340 2023-07-11 01:09:54.000000 onedrive-integration-1.2/onedrive_integration.egg-info/SOURCES.txt
--rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 01:09:54.000000 onedrive-integration-1.2/onedrive_integration.egg-info/dependency_links.txt
--rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 00:39:33.000000 onedrive-integration-1.2/onedrive_integration.egg-info/not-zip-safe
--rw-r--r--   0 william2399   (501) staff       (20)       21 2023-07-11 01:09:54.000000 onedrive-integration-1.2/onedrive_integration.egg-info/top_level.txt
--rw-r--r--   0 william2399   (501) staff       (20)       38 2023-07-11 01:09:54.763043 onedrive-integration-1.2/setup.cfg
--rw-r--r--   0 william2399   (501) staff       (20)      518 2023-07-11 01:09:51.000000 onedrive-integration-1.2/setup.py
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 01:12:24.224674 onedrive-integration-1.3/
+-rw-r--r--   0 william2399   (501) staff       (20)     1422 2023-07-11 01:12:24.223887 onedrive-integration-1.3/PKG-INFO
+-rw-r--r--   0 william2399   (501) staff       (20)     1240 2023-07-11 01:11:26.000000 onedrive-integration-1.3/README.md
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 01:12:24.215995 onedrive-integration-1.3/onedrive-integration/
+-rw-r--r--   0 william2399   (501) staff       (20)      101 2023-07-10 21:56:34.000000 onedrive-integration-1.3/onedrive-integration/__init__.py
+-rw-r--r--   0 william2399   (501) staff       (20)     1798 2023-07-11 00:16:53.000000 onedrive-integration-1.3/onedrive-integration/ms_graph.py
+-rw-r--r--   0 william2399   (501) staff       (20)     2375 2023-07-10 21:54:31.000000 onedrive-integration-1.3/onedrive-integration/onedrive_api.py
+drwxr-xr-x   0 william2399   (501) staff       (20)        0 2023-07-11 01:12:24.222872 onedrive-integration-1.3/onedrive_integration.egg-info/
+-rw-r--r--   0 william2399   (501) staff       (20)     1422 2023-07-11 01:12:23.000000 onedrive-integration-1.3/onedrive_integration.egg-info/PKG-INFO
+-rw-r--r--   0 william2399   (501) staff       (20)      340 2023-07-11 01:12:24.000000 onedrive-integration-1.3/onedrive_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 01:12:23.000000 onedrive-integration-1.3/onedrive_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 william2399   (501) staff       (20)        1 2023-07-11 01:12:23.000000 onedrive-integration-1.3/onedrive_integration.egg-info/not-zip-safe
+-rw-r--r--   0 william2399   (501) staff       (20)       21 2023-07-11 01:12:23.000000 onedrive-integration-1.3/onedrive_integration.egg-info/top_level.txt
+-rw-r--r--   0 william2399   (501) staff       (20)       38 2023-07-11 01:12:24.225035 onedrive-integration-1.3/setup.cfg
+-rw-r--r--   0 william2399   (501) staff       (20)      518 2023-07-11 01:11:43.000000 onedrive-integration-1.3/setup.py
```

### Comparing `onedrive-integration-1.2/PKG-INFO` & `onedrive-integration-1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,33 @@
-Metadata-Version: 2.1
-Name: onedrive-integration
-Version: 1.2
-Summary: Package for OneDrive File Management
-Author: William Guo
-License: MIT
-Description-Content-Type: text/markdown
-
 # OneDrive Integration Package
 ___
 _onedrive-integration_ is a Python package for OneDrive functionality, featuring methods for OneDrive file management.
 
 ## Installation
 
 ## Usage / Getting started
 
 ## Helpful Resources
 
 Sources from Jie Jenn:
-* [Upload Files to One Drive using Microsoft Graph API in Python] (https://www.youtube.com/watch?v=Ok8O_QnrSBI)
-* [Download Files from OneDrive Using Microsoft Graph API in Python] (https://www.youtube.com/watch?v=w6YeOkikVFI)
-* [Source Code for ms_graph.py] (https://learndataanalysis.org/ms_graph-py-source-code/)
+* [Upload Files to One Drive using Microsoft Graph API in Python](https://www.youtube.com/watch?v=Ok8O_QnrSBI)
+* [Download Files from OneDrive Using Microsoft Graph API in Python](https://www.youtube.com/watch?v=w6YeOkikVFI)
+* [Source Code for ms_graph.py](https://learndataanalysis.org/ms_graph-py-source-code/)
 
 Microsoft Graph API:
-* [Microsoft Graph Explorer] (https://developer.microsoft.com/en-us/graph/graph-explorer)
-* [Microsoft Azure Portal] (https://azure.microsoft.com/en-us/get-started/azure-portal)
-* [Overview of Microsoft Graph - Documentation] (https://learn.microsoft.com/en-us/graph/overview?view=graph-rest-1.0)
-
-Sources on PyPi:
-* [Build a Python Module and Share it with Pip Install] (https://www.youtube.com/watch?v=FkmtmYFTlYE)
-* [PyPi.org] (https://pypi.org/)
-
-Sources on Markdown:
-* [Make a README] (https://www.makeareadme.com/)
-* [How to write a good README] (https://dev.to/merlos/how-to-write-a-good-readme-bog)
+* [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
+* [Microsoft Azure Portal](https://azure.microsoft.com/en-us/get-started/azure-portal)
+* [Overview of Microsoft Graph - Documentation](https://learn.microsoft.com/en-us/graph/overview?view=graph-rest-1.0)
+
+PyPi:
+* [Build a Python Module and Share it with Pip Install](https://www.youtube.com/watch?v=FkmtmYFTlYE)
+* [PyPi.org](https://pypi.org/)
+
+Markdown:
+* [Make a README](https://www.makeareadme.com/)
+* [How to write a good README](https://dev.to/merlos/how-to-write-a-good-readme-bog)
 
 ## Acknowledgements
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `onedrive-integration-1.2/README.md` & `onedrive-integration-1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,41 @@
+Metadata-Version: 2.1
+Name: onedrive-integration
+Version: 1.3
+Summary: Package for OneDrive File Management
+Author: William Guo
+License: MIT
+Description-Content-Type: text/markdown
+
 # OneDrive Integration Package
 ___
 _onedrive-integration_ is a Python package for OneDrive functionality, featuring methods for OneDrive file management.
 
 ## Installation
 
 ## Usage / Getting started
 
 ## Helpful Resources
 
 Sources from Jie Jenn:
-* [Upload Files to One Drive using Microsoft Graph API in Python] (https://www.youtube.com/watch?v=Ok8O_QnrSBI)
-* [Download Files from OneDrive Using Microsoft Graph API in Python] (https://www.youtube.com/watch?v=w6YeOkikVFI)
-* [Source Code for ms_graph.py] (https://learndataanalysis.org/ms_graph-py-source-code/)
+* [Upload Files to One Drive using Microsoft Graph API in Python](https://www.youtube.com/watch?v=Ok8O_QnrSBI)
+* [Download Files from OneDrive Using Microsoft Graph API in Python](https://www.youtube.com/watch?v=w6YeOkikVFI)
+* [Source Code for ms_graph.py](https://learndataanalysis.org/ms_graph-py-source-code/)
 
 Microsoft Graph API:
-* [Microsoft Graph Explorer] (https://developer.microsoft.com/en-us/graph/graph-explorer)
-* [Microsoft Azure Portal] (https://azure.microsoft.com/en-us/get-started/azure-portal)
-* [Overview of Microsoft Graph - Documentation] (https://learn.microsoft.com/en-us/graph/overview?view=graph-rest-1.0)
-
-Sources on PyPi:
-* [Build a Python Module and Share it with Pip Install] (https://www.youtube.com/watch?v=FkmtmYFTlYE)
-* [PyPi.org] (https://pypi.org/)
-
-Sources on Markdown:
-* [Make a README] (https://www.makeareadme.com/)
-* [How to write a good README] (https://dev.to/merlos/how-to-write-a-good-readme-bog)
+* [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
+* [Microsoft Azure Portal](https://azure.microsoft.com/en-us/get-started/azure-portal)
+* [Overview of Microsoft Graph - Documentation](https://learn.microsoft.com/en-us/graph/overview?view=graph-rest-1.0)
+
+PyPi:
+* [Build a Python Module and Share it with Pip Install](https://www.youtube.com/watch?v=FkmtmYFTlYE)
+* [PyPi.org](https://pypi.org/)
+
+Markdown:
+* [Make a README](https://www.makeareadme.com/)
+* [How to write a good README](https://dev.to/merlos/how-to-write-a-good-readme-bog)
 
 ## Acknowledgements
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `onedrive-integration-1.2/onedrive-integration/ms_graph.py` & `onedrive-integration-1.3/onedrive-integration/ms_graph.py`

 * *Files identical despite different names*

### Comparing `onedrive-integration-1.2/onedrive-integration/onedrive_api.py` & `onedrive-integration-1.3/onedrive-integration/onedrive_api.py`

 * *Files identical despite different names*

### Comparing `onedrive-integration-1.2/onedrive_integration.egg-info/PKG-INFO` & `onedrive-integration-1.3/onedrive_integration.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedrive-integration
-Version: 1.2
+Version: 1.3
 Summary: Package for OneDrive File Management
 Author: William Guo
 License: MIT
 Description-Content-Type: text/markdown
 
 # OneDrive Integration Package
 ___
@@ -13,29 +13,29 @@
 ## Installation
 
 ## Usage / Getting started
 
 ## Helpful Resources
 
 Sources from Jie Jenn:
-* [Upload Files to One Drive using Microsoft Graph API in Python] (https://www.youtube.com/watch?v=Ok8O_QnrSBI)
-* [Download Files from OneDrive Using Microsoft Graph API in Python] (https://www.youtube.com/watch?v=w6YeOkikVFI)
-* [Source Code for ms_graph.py] (https://learndataanalysis.org/ms_graph-py-source-code/)
+* [Upload Files to One Drive using Microsoft Graph API in Python](https://www.youtube.com/watch?v=Ok8O_QnrSBI)
+* [Download Files from OneDrive Using Microsoft Graph API in Python](https://www.youtube.com/watch?v=w6YeOkikVFI)
+* [Source Code for ms_graph.py](https://learndataanalysis.org/ms_graph-py-source-code/)
 
 Microsoft Graph API:
-* [Microsoft Graph Explorer] (https://developer.microsoft.com/en-us/graph/graph-explorer)
-* [Microsoft Azure Portal] (https://azure.microsoft.com/en-us/get-started/azure-portal)
-* [Overview of Microsoft Graph - Documentation] (https://learn.microsoft.com/en-us/graph/overview?view=graph-rest-1.0)
-
-Sources on PyPi:
-* [Build a Python Module and Share it with Pip Install] (https://www.youtube.com/watch?v=FkmtmYFTlYE)
-* [PyPi.org] (https://pypi.org/)
-
-Sources on Markdown:
-* [Make a README] (https://www.makeareadme.com/)
-* [How to write a good README] (https://dev.to/merlos/how-to-write-a-good-readme-bog)
+* [Microsoft Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer)
+* [Microsoft Azure Portal](https://azure.microsoft.com/en-us/get-started/azure-portal)
+* [Overview of Microsoft Graph - Documentation](https://learn.microsoft.com/en-us/graph/overview?view=graph-rest-1.0)
+
+PyPi:
+* [Build a Python Module and Share it with Pip Install](https://www.youtube.com/watch?v=FkmtmYFTlYE)
+* [PyPi.org](https://pypi.org/)
+
+Markdown:
+* [Make a README](https://www.makeareadme.com/)
+* [How to write a good README](https://dev.to/merlos/how-to-write-a-good-readme-bog)
 
 ## Acknowledgements
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `onedrive-integration-1.2/setup.py` & `onedrive-integration-1.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Read contents of README.md file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
       name='onedrive-integration',
-      version='1.2',
+      version='1.3',
       long_description=long_description,
       long_description_content_type='text/markdown',
       description='Package for OneDrive File Management',
       author='William Guo',
       license='MIT',
       packages=['onedrive-integration'],
       zip_safe=False
```

