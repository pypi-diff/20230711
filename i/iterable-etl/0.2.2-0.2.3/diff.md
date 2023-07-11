# Comparing `tmp/iterable_etl-0.2.2.tar.gz` & `tmp/iterable_etl-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterable_etl-0.2.2.tar", last modified: Tue Jun 27 21:54:18 2023, max compression
+gzip compressed data, was "iterable_etl-0.2.3.tar", last modified: Tue Jul 11 20:15:30 2023, max compression
```

## Comparing `iterable_etl-0.2.2.tar` & `iterable_etl-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:54:18.182479 iterable_etl-0.2.2/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 iterable_etl-0.2.2/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2027 2023-06-27 21:54:18.182479 iterable_etl-0.2.2/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1519 2023-06-14 17:30:32.000000 iterable_etl-0.2.2/README_PUBLIC.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:54:18.182479 iterable_etl-0.2.2/iterable_etl/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-27 21:54:11.000000 iterable_etl-0.2.2/iterable_etl/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      155 2023-06-14 17:33:42.000000 iterable_etl-0.2.2/iterable_etl/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1233 2023-06-27 19:27:08.000000 iterable_etl-0.2.2/iterable_etl/iterable_etl.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:54:18.182479 iterable_etl-0.2.2/iterable_etl/libs/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 iterable_etl-0.2.2/iterable_etl/libs/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      729 2023-06-27 18:55:02.000000 iterable_etl-0.2.2/iterable_etl/libs/cnst.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1900 2023-06-22 19:06:27.000000 iterable_etl-0.2.2/iterable_etl/libs/dbg.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1214 2023-06-27 21:46:45.000000 iterable_etl-0.2.2/iterable_etl/libs/network.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1403 2023-06-21 19:49:44.000000 iterable_etl-0.2.2/iterable_etl/libs/spark.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      928 2023-06-14 17:33:42.000000 iterable_etl-0.2.2/iterable_etl/libs/transform.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:54:18.182479 iterable_etl-0.2.2/iterable_etl/tables/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 iterable_etl-0.2.2/iterable_etl/tables/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      843 2023-06-14 17:39:05.000000 iterable_etl-0.2.2/iterable_etl/tables/campaign_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1370 2023-06-14 17:39:18.000000 iterable_etl-0.2.2/iterable_etl/tables/campaign_list_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1723 2023-06-14 17:39:50.000000 iterable_etl-0.2.2/iterable_etl/tables/campaign_metrics.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      769 2023-06-14 17:40:00.000000 iterable_etl-0.2.2/iterable_etl/tables/list.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2279 2023-06-27 18:55:02.000000 iterable_etl-0.2.2/iterable_etl/tables/list_user_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1772 2023-06-27 21:53:50.000000 iterable_etl-0.2.2/iterable_etl/tables/user_history.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:54:18.182479 iterable_etl-0.2.2/iterable_etl.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2027 2023-06-27 21:54:18.000000 iterable_etl-0.2.2/iterable_etl.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      753 2023-06-27 21:54:18.000000 iterable_etl-0.2.2/iterable_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-27 21:54:18.000000 iterable_etl-0.2.2/iterable_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-27 21:54:18.000000 iterable_etl-0.2.2/iterable_etl.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-27 21:54:18.000000 iterable_etl-0.2.2/iterable_etl.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      426 2023-06-27 21:54:18.186479 iterable_etl-0.2.2/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1050 2023-06-27 21:54:11.000000 iterable_etl-0.2.2/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-27 21:54:18.182479 iterable_etl-0.2.2/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 iterable_etl-0.2.2/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-11 20:15:30.284474 iterable_etl-0.2.3/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 iterable_etl-0.2.3/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2037 2023-07-11 20:15:30.284474 iterable_etl-0.2.3/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1530 2023-07-11 20:09:32.000000 iterable_etl-0.2.3/README_PUBLIC.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-11 20:15:30.280474 iterable_etl-0.2.3/iterable_etl/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      207 2023-07-11 20:15:16.000000 iterable_etl-0.2.3/iterable_etl/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      155 2023-06-14 17:33:42.000000 iterable_etl-0.2.3/iterable_etl/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1233 2023-06-27 19:27:08.000000 iterable_etl-0.2.3/iterable_etl/iterable_etl.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-11 20:15:30.280474 iterable_etl-0.2.3/iterable_etl/libs/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 iterable_etl-0.2.3/iterable_etl/libs/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      729 2023-06-27 18:55:02.000000 iterable_etl-0.2.3/iterable_etl/libs/cnst.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1900 2023-06-22 19:06:27.000000 iterable_etl-0.2.3/iterable_etl/libs/dbg.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1214 2023-06-27 21:46:45.000000 iterable_etl-0.2.3/iterable_etl/libs/network.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1403 2023-06-21 19:49:44.000000 iterable_etl-0.2.3/iterable_etl/libs/spark.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      928 2023-06-14 17:33:42.000000 iterable_etl-0.2.3/iterable_etl/libs/transform.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-11 20:15:30.284474 iterable_etl-0.2.3/iterable_etl/tables/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 iterable_etl-0.2.3/iterable_etl/tables/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      843 2023-06-14 17:39:05.000000 iterable_etl-0.2.3/iterable_etl/tables/campaign_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1370 2023-06-14 17:39:18.000000 iterable_etl-0.2.3/iterable_etl/tables/campaign_list_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1723 2023-06-14 17:39:50.000000 iterable_etl-0.2.3/iterable_etl/tables/campaign_metrics.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      769 2023-06-14 17:40:00.000000 iterable_etl-0.2.3/iterable_etl/tables/list.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2279 2023-07-11 20:14:12.000000 iterable_etl-0.2.3/iterable_etl/tables/list_user_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1772 2023-07-11 20:14:12.000000 iterable_etl-0.2.3/iterable_etl/tables/user_history.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-11 20:15:30.280474 iterable_etl-0.2.3/iterable_etl.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2037 2023-07-11 20:15:30.000000 iterable_etl-0.2.3/iterable_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      753 2023-07-11 20:15:30.000000 iterable_etl-0.2.3/iterable_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-07-11 20:15:30.000000 iterable_etl-0.2.3/iterable_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-07-11 20:15:30.000000 iterable_etl-0.2.3/iterable_etl.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-07-11 20:15:30.000000 iterable_etl-0.2.3/iterable_etl.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      426 2023-07-11 20:15:30.284474 iterable_etl-0.2.3/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1049 2023-07-11 20:15:16.000000 iterable_etl-0.2.3/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-11 20:15:30.284474 iterable_etl-0.2.3/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 iterable_etl-0.2.3/tests/__init__.py
```

### Comparing `iterable_etl-0.2.2/PKG-INFO` & `iterable_etl-0.2.3/iterable_etl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: iterable_etl
-Version: 0.2.2
+Name: iterable-etl
+Version: 0.2.3
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# `iterable_etl`
+# `iterable_etl` DEPRECATED
 
 > Replicate data from iterable in databricks
 
 [![pypi](https://img.shields.io/pypi/v/iterable_etl?style=for-the-badge)](https://pypi.org/project/iterable_etl/)
 
 ## Usage
```

### Comparing `iterable_etl-0.2.2/README_PUBLIC.md` & `iterable_etl-0.2.3/README_PUBLIC.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# `iterable_etl`
+# `iterable_etl` DEPRECATED
 
 > Replicate data from iterable in databricks
 
 [![pypi](https://img.shields.io/pypi/v/iterable_etl?style=for-the-badge)](https://pypi.org/project/iterable_etl/)
 
 ## Usage
```

### Comparing `iterable_etl-0.2.2/iterable_etl/iterable_etl.py` & `iterable_etl-0.2.3/iterable_etl/iterable_etl.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/libs/cnst.py` & `iterable_etl-0.2.3/iterable_etl/libs/cnst.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/libs/dbg.py` & `iterable_etl-0.2.3/iterable_etl/libs/dbg.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/libs/network.py` & `iterable_etl-0.2.3/iterable_etl/libs/network.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/libs/spark.py` & `iterable_etl-0.2.3/iterable_etl/libs/spark.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/libs/transform.py` & `iterable_etl-0.2.3/iterable_etl/libs/transform.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/tables/campaign_history.py` & `iterable_etl-0.2.3/iterable_etl/tables/campaign_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/tables/campaign_list_history.py` & `iterable_etl-0.2.3/iterable_etl/tables/campaign_list_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/tables/campaign_metrics.py` & `iterable_etl-0.2.3/iterable_etl/tables/campaign_metrics.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/tables/list.py` & `iterable_etl-0.2.3/iterable_etl/tables/list.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/tables/list_user_history.py` & `iterable_etl-0.2.3/iterable_etl/tables/list_user_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/iterable_etl/tables/user_history.py` & `iterable_etl-0.2.3/iterable_etl/tables/user_history.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """user_history"""
 
-from typing import Dict
 from datetime import datetime
+from typing import Dict
 
 from pandas import DataFrame as PandasDF
 
 from iterable_etl.libs.cnst import get_headers, urls
 from iterable_etl.libs.dbg import print_dataframe_head, write_dataframe_to_csv
 from iterable_etl.libs.network import get_data_csv
 from iterable_etl.libs.transform import csv_to_dataframe
```

### Comparing `iterable_etl-0.2.2/iterable_etl.egg-info/PKG-INFO` & `iterable_etl-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: iterable-etl
-Version: 0.2.2
+Name: iterable_etl
+Version: 0.2.3
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# `iterable_etl`
+# `iterable_etl` DEPRECATED
 
 > Replicate data from iterable in databricks
 
 [![pypi](https://img.shields.io/pypi/v/iterable_etl?style=for-the-badge)](https://pypi.org/project/iterable_etl/)
 
 ## Usage
```

### Comparing `iterable_etl-0.2.2/iterable_etl.egg-info/SOURCES.txt` & `iterable_etl-0.2.3/iterable_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.2.2/setup.py` & `iterable_etl-0.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="iterable_etl",
-    version="0.2.2",
+    version="0.2.3",
     description="Replicate iterable data in databricks",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 7 - Inactive",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
     license="UNLICENSED",
     packages=find_packages(include=["iterable_etl", "iterable_etl.*"]),
     url="https://github.com/neofinancial/iterable_etl",
```

