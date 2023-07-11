# Comparing `tmp/shaku-database-1.1.3.tar.gz` & `tmp/shaku-database-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.1.3.tar", last modified: Mon Jul 10 06:31:13 2023, max compression
+gzip compressed data, was "shaku-database-1.1.4.tar", last modified: Tue Jul 11 09:00:53 2023, max compression
```

## Comparing `shaku-database-1.1.3.tar` & `shaku-database-1.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.218353 shaku-database-1.1.3/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.3/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-10 06:31:13.218112 shaku-database-1.1.3/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.3/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.215652 shaku-database-1.1.3/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.3/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.216021 shaku-database-1.1.3/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.3/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.3/database/bigquery/bq_sql_parser.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.3/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.216296 shaku-database-1.1.3/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.3/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.3/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.216429 shaku-database-1.1.3/gdrive_gcs_toolkit/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.3/gdrive_gcs_toolkit/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.216738 shaku-database-1.1.3/gdrive_gcs_toolkit/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.3/gdrive_gcs_toolkit/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.3/gdrive_gcs_toolkit/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.217135 shaku-database-1.1.3/gdrive_gcs_toolkit/google_shared_drive/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.3/gdrive_gcs_toolkit/google_shared_drive/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)    11601 2023-07-10 06:30:13.000000 shaku-database-1.1.3/gdrive_gcs_toolkit/google_shared_drive/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-10 06:31:13.218396 shaku-database-1.1.3/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-10 06:30:17.000000 shaku-database-1.1.3/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-10 06:31:13.217898 shaku-database-1.1.3/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-10 06:31:13.000000 shaku-database-1.1.3/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      600 2023-07-10 06:31:13.000000 shaku-database-1.1.3/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-10 06:31:13.000000 shaku-database-1.1.3/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-10 06:31:13.000000 shaku-database-1.1.3/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-10 06:31:13.000000 shaku-database-1.1.3/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.799610 shaku-database-1.1.4/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.4/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-11 09:00:53.799417 shaku-database-1.1.4/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.4/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.796421 shaku-database-1.1.4/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.4/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.796924 shaku-database-1.1.4/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.4/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.4/database/bigquery/bq_sql_parser.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.4/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.797312 shaku-database-1.1.4/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.4/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.4/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.797679 shaku-database-1.1.4/gdrive_gcs_toolkit/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.4/gdrive_gcs_toolkit/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.797927 shaku-database-1.1.4/gdrive_gcs_toolkit/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.4/gdrive_gcs_toolkit/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.4/gdrive_gcs_toolkit/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.798367 shaku-database-1.1.4/gdrive_gcs_toolkit/google_shared_drive/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.4/gdrive_gcs_toolkit/google_shared_drive/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)    11601 2023-07-10 06:30:13.000000 shaku-database-1.1.4/gdrive_gcs_toolkit/google_shared_drive/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-11 09:00:53.799652 shaku-database-1.1.4/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-11 09:00:26.000000 shaku-database-1.1.4/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.799229 shaku-database-1.1.4/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-11 09:00:53.000000 shaku-database-1.1.4/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      600 2023-07-11 09:00:53.000000 shaku-database-1.1.4/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-11 09:00:53.000000 shaku-database-1.1.4/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-11 09:00:53.000000 shaku-database-1.1.4/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-11 09:00:53.000000 shaku-database-1.1.4/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.1.3/LICENSE` & `shaku-database-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.3/PKG-INFO` & `shaku-database-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.3
+Version: 1.1.4
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.3/README.md` & `shaku-database-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.3/database/bigquery/bq_sql_parser.py` & `shaku-database-1.1.4/database/bigquery/bq_sql_parser.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.3/database/bigquery/util.py` & `shaku-database-1.1.4/database/bigquery/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.3/database/cloud_sql/crud.py` & `shaku-database-1.1.4/database/cloud_sql/crud.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.3/gdrive_gcs_toolkit/cloud_storage/util.py` & `shaku-database-1.1.4/gdrive_gcs_toolkit/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.3/gdrive_gcs_toolkit/google_shared_drive/util.py` & `shaku-database-1.1.4/gdrive_gcs_toolkit/google_shared_drive/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.3/setup.py` & `shaku-database-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 EX_INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else ""
                        for s in requirements.split("\n")}
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 setup(
     name="shaku-database",
-    version="1.1.3",
+    version="1.1.4",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.1.3/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.1.4/shaku_database.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.3
+Version: 1.1.4
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.3/shaku_database.egg-info/SOURCES.txt` & `shaku-database-1.1.4/shaku_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.3/shaku_database.egg-info/requires.txt` & `shaku-database-1.1.4/shaku_database.egg-info/requires.txt`

 * *Files identical despite different names*

