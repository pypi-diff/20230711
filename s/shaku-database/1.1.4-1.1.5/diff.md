# Comparing `tmp/shaku-database-1.1.4.tar.gz` & `tmp/shaku-database-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.1.4.tar", last modified: Tue Jul 11 09:00:53 2023, max compression
+gzip compressed data, was "shaku-database-1.1.5.tar", last modified: Tue Jul 11 09:10:42 2023, max compression
```

## Comparing `shaku-database-1.1.4.tar` & `shaku-database-1.1.5.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.799610 shaku-database-1.1.4/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.4/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-11 09:00:53.799417 shaku-database-1.1.4/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.4/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.796421 shaku-database-1.1.4/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.4/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.796924 shaku-database-1.1.4/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.4/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.4/database/bigquery/bq_sql_parser.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.4/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.797312 shaku-database-1.1.4/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.4/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.4/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.797679 shaku-database-1.1.4/gdrive_gcs_toolkit/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.4/gdrive_gcs_toolkit/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.797927 shaku-database-1.1.4/gdrive_gcs_toolkit/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.4/gdrive_gcs_toolkit/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.4/gdrive_gcs_toolkit/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.798367 shaku-database-1.1.4/gdrive_gcs_toolkit/google_shared_drive/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.4/gdrive_gcs_toolkit/google_shared_drive/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)    11601 2023-07-10 06:30:13.000000 shaku-database-1.1.4/gdrive_gcs_toolkit/google_shared_drive/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-11 09:00:53.799652 shaku-database-1.1.4/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-11 09:00:26.000000 shaku-database-1.1.4/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:00:53.799229 shaku-database-1.1.4/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-11 09:00:53.000000 shaku-database-1.1.4/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      600 2023-07-11 09:00:53.000000 shaku-database-1.1.4/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-11 09:00:53.000000 shaku-database-1.1.4/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-11 09:00:53.000000 shaku-database-1.1.4/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-11 09:00:53.000000 shaku-database-1.1.4/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.467533 shaku-database-1.1.5/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.5/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-11 09:10:42.467350 shaku-database-1.1.5/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.5/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.464006 shaku-database-1.1.5/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.5/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.464536 shaku-database-1.1.5/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.5/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.5/database/bigquery/bq_sql_parser.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.5/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.465004 shaku-database-1.1.5/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.5/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.5/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.465467 shaku-database-1.1.5/database/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:09:30.000000 shaku-database-1.1.5/database/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1580 2023-07-11 09:00:21.000000 shaku-database-1.1.5/database/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.465708 shaku-database-1.1.5/gdrive_gcs_toolkit/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.5/gdrive_gcs_toolkit/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.465937 shaku-database-1.1.5/gdrive_gcs_toolkit/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.5/gdrive_gcs_toolkit/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.5/gdrive_gcs_toolkit/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.466328 shaku-database-1.1.5/gdrive_gcs_toolkit/google_shared_drive/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.5/gdrive_gcs_toolkit/google_shared_drive/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)    11601 2023-07-10 06:30:13.000000 shaku-database-1.1.5/gdrive_gcs_toolkit/google_shared_drive/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-11 09:10:42.467573 shaku-database-1.1.5/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-11 09:10:11.000000 shaku-database-1.1.5/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.467173 shaku-database-1.1.5/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-11 09:10:42.000000 shaku-database-1.1.5/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      666 2023-07-11 09:10:42.000000 shaku-database-1.1.5/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-11 09:10:42.000000 shaku-database-1.1.5/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-11 09:10:42.000000 shaku-database-1.1.5/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-11 09:10:42.000000 shaku-database-1.1.5/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.1.4/LICENSE` & `shaku-database-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.4/PKG-INFO` & `shaku-database-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.4
+Version: 1.1.5
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.4/README.md` & `shaku-database-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.4/database/bigquery/bq_sql_parser.py` & `shaku-database-1.1.5/database/bigquery/bq_sql_parser.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.4/database/bigquery/util.py` & `shaku-database-1.1.5/database/bigquery/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.4/database/cloud_sql/crud.py` & `shaku-database-1.1.5/database/cloud_sql/crud.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.4/gdrive_gcs_toolkit/cloud_storage/util.py` & `shaku-database-1.1.5/gdrive_gcs_toolkit/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.4/gdrive_gcs_toolkit/google_shared_drive/util.py` & `shaku-database-1.1.5/gdrive_gcs_toolkit/google_shared_drive/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.4/setup.py` & `shaku-database-1.1.5/setup.py`

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
-    version="1.1.4",
+    version="1.1.5",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.1.4/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.1.5/shaku_database.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.4
+Version: 1.1.5
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.4/shaku_database.egg-info/SOURCES.txt` & `shaku-database-1.1.5/shaku_database.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 setup.py
 database/__init__.py
 database/bigquery/__init__.py
 database/bigquery/bq_sql_parser.py
 database/bigquery/util.py
 database/cloud_sql/__init__.py
 database/cloud_sql/crud.py
+database/cloud_storage/__init__.py
+database/cloud_storage/util.py
 gdrive_gcs_toolkit/__init__.py
 gdrive_gcs_toolkit/cloud_storage/__init__.py
 gdrive_gcs_toolkit/cloud_storage/util.py
 gdrive_gcs_toolkit/google_shared_drive/__init__.py
 gdrive_gcs_toolkit/google_shared_drive/util.py
 shaku_database.egg-info/PKG-INFO
 shaku_database.egg-info/SOURCES.txt
```

### Comparing `shaku-database-1.1.4/shaku_database.egg-info/requires.txt` & `shaku-database-1.1.5/shaku_database.egg-info/requires.txt`

 * *Files identical despite different names*

