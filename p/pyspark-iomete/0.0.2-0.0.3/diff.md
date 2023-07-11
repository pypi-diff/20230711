# Comparing `tmp/pyspark_iomete-0.0.2.tar.gz` & `tmp/pyspark_iomete-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_iomete-0.0.2.tar", last modified: Thu Feb 16 01:55:31 2023, max compression
+gzip compressed data, was "pyspark_iomete-0.0.3.tar", last modified: Tue Jul 11 15:35:50 2023, max compression
```

## Comparing `pyspark_iomete-0.0.2.tar` & `pyspark_iomete-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vusaldadalov   (501) staff       (20)        0 2023-02-16 01:55:31.774839 pyspark_iomete-0.0.2/
--rw-r--r--   0 vusaldadalov   (501) staff       (20)     2011 2023-02-16 01:55:31.774890 pyspark_iomete-0.0.2/PKG-INFO
--rw-r--r--   0 vusaldadalov   (501) staff       (20)     1146 2023-02-15 14:36:42.000000 pyspark_iomete-0.0.2/README.md
-drwxr-xr-x   0 vusaldadalov   (501) staff       (20)        0 2023-02-16 01:55:31.773968 pyspark_iomete-0.0.2/pyspark_iomete/
--rw-r--r--   0 vusaldadalov   (501) staff       (20)        0 2023-02-15 14:23:16.000000 pyspark_iomete-0.0.2/pyspark_iomete/__init__.py
--rw-r--r--   0 vusaldadalov   (501) staff       (20)      257 2023-02-15 14:11:07.000000 pyspark_iomete-0.0.2/pyspark_iomete/test_utils.py
--rw-r--r--   0 vusaldadalov   (501) staff       (20)      331 2023-02-15 14:10:10.000000 pyspark_iomete-0.0.2/pyspark_iomete/utils.py
-drwxr-xr-x   0 vusaldadalov   (501) staff       (20)        0 2023-02-16 01:55:31.774752 pyspark_iomete-0.0.2/pyspark_iomete.egg-info/
--rw-r--r--   0 vusaldadalov   (501) staff       (20)     2011 2023-02-16 01:55:31.000000 pyspark_iomete-0.0.2/pyspark_iomete.egg-info/PKG-INFO
--rw-r--r--   0 vusaldadalov   (501) staff       (20)      297 2023-02-16 01:55:31.000000 pyspark_iomete-0.0.2/pyspark_iomete.egg-info/SOURCES.txt
--rw-r--r--   0 vusaldadalov   (501) staff       (20)        1 2023-02-16 01:55:31.000000 pyspark_iomete-0.0.2/pyspark_iomete.egg-info/dependency_links.txt
--rw-r--r--   0 vusaldadalov   (501) staff       (20)       15 2023-02-16 01:55:31.000000 pyspark_iomete-0.0.2/pyspark_iomete.egg-info/requires.txt
--rw-r--r--   0 vusaldadalov   (501) staff       (20)       15 2023-02-16 01:55:31.000000 pyspark_iomete-0.0.2/pyspark_iomete.egg-info/top_level.txt
--rw-r--r--   0 vusaldadalov   (501) staff       (20)       38 2023-02-16 01:55:31.775040 pyspark_iomete-0.0.2/setup.cfg
--rw-r--r--   0 vusaldadalov   (501) staff       (20)     1388 2023-02-16 01:55:06.000000 pyspark_iomete-0.0.2/setup.py
+drwxr-xr-x   0 vusaldadalov   (501) staff       (20)        0 2023-07-11 15:35:50.930241 pyspark_iomete-0.0.3/
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)     2174 2023-07-11 15:35:50.930313 pyspark_iomete-0.0.3/PKG-INFO
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)     1309 2023-07-11 15:34:27.000000 pyspark_iomete-0.0.3/README.md
+drwxr-xr-x   0 vusaldadalov   (501) staff       (20)        0 2023-07-11 15:35:50.929371 pyspark_iomete-0.0.3/pyspark_iomete/
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)        0 2023-02-15 14:23:16.000000 pyspark_iomete-0.0.3/pyspark_iomete/__init__.py
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)      257 2023-02-15 14:11:07.000000 pyspark_iomete-0.0.3/pyspark_iomete/test_utils.py
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)      410 2023-07-11 15:31:33.000000 pyspark_iomete-0.0.3/pyspark_iomete/utils.py
+drwxr-xr-x   0 vusaldadalov   (501) staff       (20)        0 2023-07-11 15:35:50.930137 pyspark_iomete-0.0.3/pyspark_iomete.egg-info/
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)     2174 2023-07-11 15:35:50.000000 pyspark_iomete-0.0.3/pyspark_iomete.egg-info/PKG-INFO
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)      297 2023-07-11 15:35:50.000000 pyspark_iomete-0.0.3/pyspark_iomete.egg-info/SOURCES.txt
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)        1 2023-07-11 15:35:50.000000 pyspark_iomete-0.0.3/pyspark_iomete.egg-info/dependency_links.txt
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)       15 2023-07-11 15:35:50.000000 pyspark_iomete-0.0.3/pyspark_iomete.egg-info/requires.txt
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)       15 2023-07-11 15:35:50.000000 pyspark_iomete-0.0.3/pyspark_iomete.egg-info/top_level.txt
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)       38 2023-07-11 15:35:50.930509 pyspark_iomete-0.0.3/setup.cfg
+-rw-r--r--   0 vusaldadalov   (501) staff       (20)     1388 2023-07-11 15:32:06.000000 pyspark_iomete-0.0.3/setup.py
```

### Comparing `pyspark_iomete-0.0.2/PKG-INFO` & `pyspark_iomete-0.0.3/pyspark_iomete.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyspark_iomete
-Version: 0.0.2
+Name: pyspark-iomete
+Version: 0.0.3
 Summary: IOMETE's PySpark library that contains useful utilities for working with PySpark
 Home-page: https://github.com/iomete/pyspark-iomete
 Author: IOMETE
 Author-email: vusal@iomete.com
 License: Apache License 2.0
 Keywords: iomete,pyspark,utils
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,18 +42,21 @@
 
 Usage:
 ```python
 from pyspark_iomete.utils import get_spark_logger
 from pyspark.sql import SparkSession
 
 spark = SparkSession.builder.getOrCreate()
-logger = get_spark_logger(spark=spark)
 
-# or with a custom name
+# spark session and name will be used to create the logger
+# both are optional
 logger = get_spark_logger(spark=spark, name="my_custom_logger")
+
+# spark session will be retrieved using SparkSession.getActiveSession() and name will be set to the current file name
+logger = get_spark_logger()
 ```
 
 ## Test utility functions
 
 ### table_name_with_random_suffix
 
 This function is returning a table name with a random suffix. This is useful for testing purposes.
```

### Comparing `pyspark_iomete-0.0.2/README.md` & `pyspark_iomete-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -20,18 +20,21 @@
 
 Usage:
 ```python
 from pyspark_iomete.utils import get_spark_logger
 from pyspark.sql import SparkSession
 
 spark = SparkSession.builder.getOrCreate()
-logger = get_spark_logger(spark=spark)
 
-# or with a custom name
+# spark session and name will be used to create the logger
+# both are optional
 logger = get_spark_logger(spark=spark, name="my_custom_logger")
+
+# spark session will be retrieved using SparkSession.getActiveSession() and name will be set to the current file name
+logger = get_spark_logger()
 ```
 
 ## Test utility functions
 
 ### table_name_with_random_suffix
 
 This function is returning a table name with a random suffix. This is useful for testing purposes.
```

### Comparing `pyspark_iomete-0.0.2/pyspark_iomete.egg-info/PKG-INFO` & `pyspark_iomete-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyspark-iomete
-Version: 0.0.2
+Name: pyspark_iomete
+Version: 0.0.3
 Summary: IOMETE's PySpark library that contains useful utilities for working with PySpark
 Home-page: https://github.com/iomete/pyspark-iomete
 Author: IOMETE
 Author-email: vusal@iomete.com
 License: Apache License 2.0
 Keywords: iomete,pyspark,utils
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,18 +42,21 @@
 
 Usage:
 ```python
 from pyspark_iomete.utils import get_spark_logger
 from pyspark.sql import SparkSession
 
 spark = SparkSession.builder.getOrCreate()
-logger = get_spark_logger(spark=spark)
 
-# or with a custom name
+# spark session and name will be used to create the logger
+# both are optional
 logger = get_spark_logger(spark=spark, name="my_custom_logger")
+
+# spark session will be retrieved using SparkSession.getActiveSession() and name will be set to the current file name
+logger = get_spark_logger()
 ```
 
 ## Test utility functions
 
 ### table_name_with_random_suffix
 
 This function is returning a table name with a random suffix. This is useful for testing purposes.
```

### Comparing `pyspark_iomete-0.0.2/setup.py` & `pyspark_iomete-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from distutils.core import setup
 
 package_name = "pyspark_iomete"
-package_version = "0.0.2"
+package_version = "0.0.3"
 
 description = """IOMETE's PySpark library that contains useful utilities for working with PySpark"""
 
 # pull long description from README
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), "r", encoding="utf8") as f:
     long_description = f.read()
```

