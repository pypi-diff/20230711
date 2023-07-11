# Comparing `tmp/igrafx_mining_sdk-2.24.1.tar.gz` & `tmp/igrafx_mining_sdk-2.24.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\igrafx_mining_sdk-2.24.1.tar", last modified: Tue Jul 11 08:00:53 2023, max compression
+gzip compressed data, was "dist\igrafx_mining_sdk-2.24.2.tar", last modified: Tue Jul 11 09:16:39 2023, max compression
```

## Comparing `igrafx_mining_sdk-2.24.1.tar` & `igrafx_mining_sdk-2.24.2.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 08:00:53.049801 igrafx_mining_sdk-2.24.1/
--rw-rw-rw-   0        0        0      318 2023-07-11 08:00:53.049801 igrafx_mining_sdk-2.24.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 08:00:53.026800 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/
--rw-rw-rw-   0        0        0     1752 2023-07-07 08:47:13.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/__init__.py
--rw-rw-rw-   0        0        0     6966 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/api_connector.py
--rw-rw-rw-   0        0        0    11537 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/column_mapping.py
--rw-rw-rw-   0        0        0     3153 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/datasource.py
--rw-rw-rw-   0        0        0     3418 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/graph.py
--rw-rw-rw-   0        0        0    10081 2023-06-23 09:37:29.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/project.py
--rw-rw-rw-   0        0        0     3077 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/workgroup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 08:00:53.040799 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk.egg-info/
--rw-rw-rw-   0        0        0      318 2023-07-11 08:00:52.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-07-11 08:00:52.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 08:00:52.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-11 08:00:52.000000 igrafx_mining_sdk-2.24.1/igrafx_mining_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 08:00:53.050800 igrafx_mining_sdk-2.24.1/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-07-11 07:59:48.000000 igrafx_mining_sdk-2.24.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 08:00:53.047800 igrafx_mining_sdk-2.24.1/tests/
--rw-rw-rw-   0        0        0     9022 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.1/tests/test_column_mapping.py
--rw-rw-rw-   0        0        0     3524 2023-06-26 13:02:16.000000 igrafx_mining_sdk-2.24.1/tests/test_datasource.py
--rw-rw-rw-   0        0        0     2046 2023-06-26 13:56:52.000000 igrafx_mining_sdk-2.24.1/tests/test_graph.py
--rw-rw-rw-   0        0        0     6791 2023-06-26 13:02:16.000000 igrafx_mining_sdk-2.24.1/tests/test_project.py
--rw-rw-rw-   0        0        0     1463 2023-06-26 13:02:16.000000 igrafx_mining_sdk-2.24.1/tests/test_workgroup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:16:39.925983 igrafx_mining_sdk-2.24.2/
+-rw-rw-rw-   0        0        0     1082 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.2/LICENSE
+-rw-rw-rw-   0        0        0      341 2023-07-11 09:16:39.925983 igrafx_mining_sdk-2.24.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3644 2023-07-03 09:05:26.000000 igrafx_mining_sdk-2.24.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 09:16:39.896982 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/
+-rw-rw-rw-   0        0        0     1754 2023-07-11 08:59:35.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/__init__.py
+-rw-rw-rw-   0        0        0     6966 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/api_connector.py
+-rw-rw-rw-   0        0        0    11537 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/column_mapping.py
+-rw-rw-rw-   0        0        0     3153 2023-07-11 08:50:57.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/datasource.py
+-rw-rw-rw-   0        0        0     3418 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/graph.py
+-rw-rw-rw-   0        0        0    10081 2023-07-11 08:51:40.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/project.py
+-rw-rw-rw-   0        0        0     3077 2023-07-11 08:51:10.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/workgroup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:16:39.917981 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/
+-rw-rw-rw-   0        0        0      341 2023-07-11 09:16:39.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-07-11 09:16:39.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 09:16:39.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-11 09:16:39.000000 igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      961 2023-07-11 08:43:20.000000 igrafx_mining_sdk-2.24.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 09:16:39.926979 igrafx_mining_sdk-2.24.2/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2023-07-11 09:16:37.000000 igrafx_mining_sdk-2.24.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:16:39.923991 igrafx_mining_sdk-2.24.2/tests/
+-rw-rw-rw-   0        0        0     9022 2023-06-20 10:15:54.000000 igrafx_mining_sdk-2.24.2/tests/test_column_mapping.py
+-rw-rw-rw-   0        0        0     3620 2023-07-11 09:10:27.000000 igrafx_mining_sdk-2.24.2/tests/test_datasource.py
+-rw-rw-rw-   0        0        0     2118 2023-07-11 09:10:27.000000 igrafx_mining_sdk-2.24.2/tests/test_graph.py
+-rw-rw-rw-   0        0        0     6863 2023-07-11 09:10:27.000000 igrafx_mining_sdk-2.24.2/tests/test_project.py
+-rw-rw-rw-   0        0        0     1553 2023-07-11 09:10:27.000000 igrafx_mining_sdk-2.24.2/tests/test_workgroup.py
```

### Comparing `igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/__init__.py` & `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
 
 from igrafx_mining_sdk.column_mapping import FileType, FileStructure, ColumnMapping, MetricAggregation, DimensionAggregation
 from igrafx_mining_sdk.datasource import Datasource
 from igrafx_mining_sdk.workgroup import Workgroup
 from igrafx_mining_sdk.project import Project
 from igrafx_mining_sdk.graph import Graph, GraphInstance
+
 import toml
 from pathlib import Path
 import importlib
 
 
 def extract_metadata():
     metadata = dict()
```

### Comparing `igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/api_connector.py` & `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/api_connector.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/column_mapping.py` & `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/column_mapping.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/datasource.py` & `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/datasource.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/graph.py` & `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/graph.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/project.py` & `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/project.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.1/igrafx_mining_sdk/workgroup.py` & `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk/workgroup.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.1/igrafx_mining_sdk.egg-info/SOURCES.txt` & `igrafx_mining_sdk-2.24.2/igrafx_mining_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+LICENSE
+README.md
+pyproject.toml
 setup.py
 igrafx_mining_sdk/__init__.py
 igrafx_mining_sdk/api_connector.py
 igrafx_mining_sdk/column_mapping.py
 igrafx_mining_sdk/datasource.py
 igrafx_mining_sdk/graph.py
 igrafx_mining_sdk/project.py
```

### Comparing `igrafx_mining_sdk-2.24.1/setup.py` & `igrafx_mining_sdk-2.24.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 import toml
 import re
 
 # Parse pyproject.toml file
-with open('../pyproject.toml', 'r') as f:
+with open('./pyproject.toml', 'r') as f:
     pyproject_data = toml.load(f)
 
 # Extract package information
 package_infos = {
     "__author__": pyproject_data['tool']['poetry']['authors'][0].split('<')[0].rstrip(),
     "__version__": pyproject_data['tool']['poetry']['version'],
     "__doc__": pyproject_data['tool']['poetry']['description'],
@@ -20,10 +20,10 @@
 setup(
     name="igrafx_mining_sdk",
     version=package_infos['__version__'],
     description=package_infos['__doc__'],
     url="https://www.logpickr.com/fr/accueil.html",
     author=package_infos['__author__'],
     author_email=package_infos['__email__'],
-    packages=["igrafx_mining_sdk"],
+    packages=find_packages(),    #["igrafx_mining_sdk"],
     licence="Apache License 2.0"
 )
```

### Comparing `igrafx_mining_sdk-2.24.1/tests/test_column_mapping.py` & `igrafx_mining_sdk-2.24.2/tests/test_column_mapping.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.24.1/tests/test_datasource.py` & `igrafx_mining_sdk-2.24.2/tests/test_datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # MIT License, Copyright 2023 iGrafx
 # https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
+from pathlib import Path
 import pytest
-from igrafx_mining_sdk import Project
+from igrafx_mining_sdk.project import Project
 from igrafx_mining_sdk.datasource import Datasource
 from igrafx_mining_sdk.workgroup import Workgroup
 from dotenv import load_dotenv
 import os
 
 # Load environment variables from .env file
-load_dotenv()
+dotenv_path = Path(__file__).parent.parent / '.env'
+load_dotenv(dotenv_path)
 
 NAME = os.environ.get('NAME')
 TYPE = os.environ.get('TYPE')
 HOST = os.environ.get('HOST')
 PORT = os.environ.get('PORT')
 
 wg_id = os.environ.get('WG_ID')
```

### Comparing `igrafx_mining_sdk-2.24.1/tests/test_graph.py` & `igrafx_mining_sdk-2.24.2/tests/test_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # MIT License, Copyright 2023 iGrafx
 # https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
 
 from pathlib import Path
 import pytest
-from igrafx_mining_sdk import Project
+from igrafx_mining_sdk.project import Project
 from igrafx_mining_sdk.workgroup import Workgroup
 from igrafx_mining_sdk.graph import Graph
 from dotenv import load_dotenv
 import os
 
 # Load environment variables from .env file
-load_dotenv()
+dotenv_path = Path(__file__).parent.parent / '.env'
+load_dotenv(dotenv_path)
 
 wg_id = os.environ.get('WG_ID')
 wg_key = os.environ.get('WG_KEY')
 wg_url = os.environ.get('WG_URL')
 wg_auth = os.environ.get('WG_AUTH')
 project_id = os.environ.get('PROJECT_ID')
```

### Comparing `igrafx_mining_sdk-2.24.1/tests/test_project.py` & `igrafx_mining_sdk-2.24.2/tests/test_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # MIT License, Copyright 2023 iGrafx
 # https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
 
 from pathlib import Path
-from igrafx_mining_sdk import Project, FileStructure, FileType
-from igrafx_mining_sdk.column_mapping import Column, ColumnType, ColumnMapping
+from igrafx_mining_sdk.project import Project, FileStructure
+from igrafx_mining_sdk.column_mapping import Column, ColumnType, ColumnMapping, FileType
 from igrafx_mining_sdk.datasource import Datasource
 from igrafx_mining_sdk.workgroup import Workgroup
 import pytest
 from dotenv import load_dotenv
 import os
 
 # Load environment variables from .env file
-load_dotenv()
+dotenv_path = Path(__file__).parent.parent / '.env'
+load_dotenv(dotenv_path)
 
 wg_id = os.environ.get('WG_ID')
 wg_key = os.environ.get('WG_KEY')
 wg_url = os.environ.get('WG_URL')
 wg_auth = os.environ.get('WG_AUTH')
 project_id = os.environ.get('PROJECT_ID')
```

### Comparing `igrafx_mining_sdk-2.24.1/tests/test_workgroup.py` & `igrafx_mining_sdk-2.24.2/tests/test_workgroup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # MIT License, Copyright 2023 iGrafx
 # https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
+from pathlib import Path
 
 import pytest
 from igrafx_mining_sdk.workgroup import Workgroup
 from dotenv import load_dotenv
 import os
 
 # Load environment variables from .env file
-load_dotenv()
+dotenv_path = Path(__file__).parent.parent / '.env'
+load_dotenv(dotenv_path)
 
 wg_id = os.environ.get('WG_ID')
 wg_key = os.environ.get('WG_KEY')
 wg_url = os.environ.get('WG_URL')
 wg_auth = os.environ.get('WG_AUTH')
 project_id = os.environ.get('PROJECT_ID')
```

