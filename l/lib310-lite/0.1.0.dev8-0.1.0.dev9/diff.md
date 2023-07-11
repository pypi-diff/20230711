# Comparing `tmp/lib310_lite-0.1.0.dev8.tar.gz` & `tmp/lib310_lite-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.1.0.dev8.tar", max compression
+gzip compressed data, was "lib310_lite-0.1.0.dev9.tar", max compression
```

## Comparing `lib310_lite-0.1.0.dev8.tar` & `lib310_lite-0.1.0.dev9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev8/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev8/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev8/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev8/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0    13844 2023-07-11 10:06:50.728620 lib310_lite-0.1.0.dev8/lib310_lite/laser/laser.py
--rw-r--r--   0        0        0      798 2023-07-11 10:06:50.730846 lib310_lite-0.1.0.dev8/pyproject.toml
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev8/setup.py
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev9/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev9/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev9/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev9/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0    13840 2023-07-11 10:11:35.990937 lib310_lite-0.1.0.dev9/lib310_lite/laser/laser.py
+-rw-r--r--   0        0        0      798 2023-07-11 10:12:00.861480 lib310_lite-0.1.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev9/setup.py
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev9/PKG-INFO
```

### Comparing `lib310_lite-0.1.0.dev8/lib310_lite/bigquery/client.py` & `lib310_lite-0.1.0.dev9/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev8/lib310_lite/bigquery/constants.py` & `lib310_lite-0.1.0.dev9/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev8/lib310_lite/laser/laser.py` & `lib310_lite-0.1.0.dev9/lib310_lite/laser/laser.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
         :return:
         """
         cnx = None
         cursor = None
         result = None
         try:
             # cnx = MySQLdb.connect(**self.db_config)
-            cnx = self.connection_pool.get_connection()
+            cnx = self.connection_pool.connection()
             cursor = cnx.cursor(cursorclass=MySQLdb.cursors.DictCursor)
             query = "SELECT {} FROM {} WHERE row_id IN ({})".format(self.COLUMNS, self.MAIN_TABLE_NAME, ','.join(map(str, index_list)))
             cursor.execute(query)
             result = cursor.fetchall()
         except Exception as e:
             result = None
             print(e)
```

### Comparing `lib310_lite-0.1.0.dev8/pyproject.toml` & `lib310_lite-0.1.0.dev9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.1.0.dev8"
+version = "0.1.0.dev9"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.1.0.dev8/setup.py` & `lib310_lite-0.1.0.dev9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'mysqlclient>=2.0.0',
  'numpy<1.23.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.1.0.dev8',
+    'version': '0.1.0.dev9',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.1.0.dev8/PKG-INFO` & `lib310_lite-0.1.0.dev9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```

