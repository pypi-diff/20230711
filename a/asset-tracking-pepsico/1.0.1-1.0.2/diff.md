# Comparing `tmp/asset_tracking_pepsico-1.0.1.tar.gz` & `tmp/asset_tracking_pepsico-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_tracking_pepsico-1.0.1.tar", last modified: Wed Jul  5 13:01:09 2023, max compression
+gzip compressed data, was "asset_tracking_pepsico-1.0.2.tar", last modified: Tue Jul 11 10:51:07 2023, max compression
```

## Comparing `asset_tracking_pepsico-1.0.1.tar` & `asset_tracking_pepsico-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-05 13:01:09.093556 asset_tracking_pepsico-1.0.1/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-1.0.1/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-05 13:01:09.092982 asset_tracking_pepsico-1.0.1/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-1.0.1/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-05 13:01:09.087053 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6746 2023-05-31 12:41:32.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/asset_tracking_devicelogs.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     4855 2023-07-05 12:58:56.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/asset_tracking_ingest.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-05 13:01:09.091971 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/dto/
--rw-r--r--   0 jatintalati   (501) staff       (20)     6503 2023-07-05 12:58:56.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/dto/PostgresSchema.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     1332 2023-07-03 06:34:17.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-05 13:01:09.091198 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-05 13:01:09.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-07-05 13:01:09.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-07-05 13:01:09.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       35 2023-07-05 13:01:09.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-07-05 13:01:09.000000 asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      748 2023-07-05 12:59:49.000000 asset_tracking_pepsico-1.0.1/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-07-05 13:01:09.093729 asset_tracking_pepsico-1.0.1/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 10:51:07.833849 asset_tracking_pepsico-1.0.2/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 asset_tracking_pepsico-1.0.2/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-11 10:51:07.833459 asset_tracking_pepsico-1.0.2/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1015 2023-05-31 14:48:14.000000 asset_tracking_pepsico-1.0.2/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 10:51:07.828903 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6750 2023-07-11 10:47:36.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/asset_tracking_devicelogs.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     4877 2023-07-11 10:45:08.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/asset_tracking_ingest.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 10:51:07.832953 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/dto/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     6794 2023-07-11 10:46:24.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/dto/PostgresSchema.py
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1332 2023-07-03 06:34:17.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 10:51:07.832435 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1593 2023-07-11 10:51:07.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      442 2023-07-11 10:51:07.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-07-11 10:51:07.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       35 2023-07-11 10:51:07.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       23 2023-07-11 10:51:07.000000 asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      748 2023-07-11 10:48:26.000000 asset_tracking_pepsico-1.0.2/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-07-11 10:51:07.834030 asset_tracking_pepsico-1.0.2/setup.cfg
```

### Comparing `asset_tracking_pepsico-1.0.1/LICENSE` & `asset_tracking_pepsico-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.1/PKG-INFO` & `asset_tracking_pepsico-1.0.2/asset_tracking_pepsico.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: asset_tracking_pepsico
-Version: 1.0.1
+Name: asset-tracking-pepsico
+Version: 1.0.2
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-1.0.1/README.md` & `asset_tracking_pepsico-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/asset_tracking_devicelogs.py` & `asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/asset_tracking_devicelogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                 else:
                     speed = None
                     properties_dict = self.extract_extra_properties(row)
                 lat_long_acc = row['Accuracy']
                 ts = row['Timestamp']
                 lat, long = float(row['Latitude']), float(row['Longitude'])
 
-                schema = PostgresSchemaDto(schema_version=schema_version, asset_id=gpid, asset_type=asset_type,
-                                           datasource=data_source, asset_latitude=lat, asset_longitude=long, speed=speed,
+                schema = PostgresSchemaDto(schema_version=schema_version, object_id=gpid, object_type=asset_type,
+                                           datasource=data_source, object_latitude=lat, object_longitude=long, speed=speed,
                                            lat_long_acc=lat_long_acc, event_type=event, created_ts=ts,
                                            properties_dict=str(properties_dict))
                 schema_list.append(schema)
             return schema_list
         except:
             traceback.print_exc()
```

### Comparing `asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/asset_tracking_ingest.py` & `asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/asset_tracking_ingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,20 +97,20 @@
 
                 properties_dict = {
                     'Employee_Name': emp_name,
                     'AppNamespace': item['AppNamespace'],
                     'AppVersion': item['AppVersion'],
                     'OsVersion': item['OsVersion'],
                     'Transition': transition,
-                    'Route': route,
                     'Version': version,
                     'EventId': item['EventId'],
                     'Description': event_desc
                 }
 
                 schema = PostgresSchemaDto(schema_version=schema_version, object_id=object_id, object_type=object_type, event_type=event,
                                            location_hint=loc_desc, location_id=loc_id, object_latitude=lat, object_longitude=long,
-                                           created_ts=times, lat_long_acc=acc, datasource=data_source, properties_dict=str(properties_dict))
+                                           created_ts=times, lat_long_acc=acc, datasource=data_source,
+                                           properties_dict=str(properties_dict), routeid=route)
                 schema_list.append(schema)
             return schema_list
         except:
             traceback.print_exc()
```

### Comparing `asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/dto/PostgresSchema.py` & `asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/dto/PostgresSchema.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     heading: Optional[float] = None
     speed: Optional[float] = None
     speed_accuracy: Optional[float] = None
     course: Optional[float] = None
     course_accuracy: Optional[float] = None
     datasource: Optional[str] = None
     properties_dict: Optional[str] = None
+    routeid: Optional[str] = None
 
 
 class PostgresSchemaDto:
     schema_version: Optional[float] = None
     object_type: Optional[str] = None
     object_id: Optional[str] = None
     event_type: Optional[str] = None
@@ -38,19 +39,20 @@
     heading: Optional[float] = None
     speed: Optional[float] = None
     speed_accuracy: Optional[float] = None
     course: Optional[float] = None
     course_accuracy: Optional[float] = None
     datasource: Optional[str] = None
     properties_dict: Optional[str] = None
+    routeid: Optional[str] = None
 
     def __init__(self, schema_version=None, object_type=None, object_id=None, event_type=None, location_hint=None, location_id=None,
                  object_latitude=None, object_longitude=None, lat_long_acc=None, created_ts=None, altitude=None, heading=None,
                  speed=None, speed_accuracy=None, course=None, course_accuracy=None,
-                 datasource=None, properties_dict=None):
+                 datasource=None, properties_dict=None, routeid=None):
         self.schema_version = schema_version
         self.object_type = object_type
         self.object_id = object_id
         self.event_type = event_type
         self.location_hint = location_hint
         self.location_id = location_id
         self.object_latitude = object_latitude
@@ -61,14 +63,15 @@
         self.heading = heading
         self.speed = speed
         self.speed_accuracy = speed_accuracy
         self.course = course
         self.course_accuracy = course_accuracy
         self.datasource = datasource
         self.properties_dict = properties_dict
+        self.routeid = routeid
 
     # Getter methods
     def get_schema_version(self):
         return self.schema_version
 
     def get_object_type(self):
         return self.object_type
@@ -117,14 +120,17 @@
 
     def get_datasource(self):
         return self.datasource
 
     def get_properties_dict(self):
         return self.properties_dict
 
+    def get_routeid(self):
+        return self.routeid
+
     # Setter methods
     def set_schema_version(self, value):
         self.schema_version = value
 
     def set_object_type(self, value):
         self.object_type = value
 
@@ -172,14 +178,17 @@
 
     def set_datasource(self, value):
         self.datasource = value
 
     def set_properties_dict(self, value):
         self.properties_dict = value
 
+    def set_routeid(self, value):
+        self.routeid = value
+
     def __dict__(self):
         return {
             'schema_version': self.schema_version,
             'object_type': self.object_type,
             'object_id': self.object_id,
             'event_type': self.event_type,
             'location_hint': self.location_hint,
@@ -191,15 +200,16 @@
             'altitude': self.altitude,
             'heading': self.heading,
             'speed': self.speed,
             'speed_accuracy': self.speed_accuracy,
             'course': self.course,
             'course_accuracy': self.course_accuracy,
             'datasource': self.datasource,
-            'properties_dict': self.properties_dict
+            'properties_dict': self.properties_dict,
+            'routeid': self.routeid
         }
 
     def __str__(self):
         return f"{self.schema_version}, \'{self.object_type}\', \'{self.object_id}\', \'{self.event_type}\', \'{self.location_hint}\', " \
                f"\'{self.location_id}\', {self.object_latitude}, {self.object_longitude}, {self.lat_long_acc}, \'{self.created_ts}\', " \
                f"{self.altitude}, {self.heading}, {self.speed}, {self.speed_accuracy}, {self.course}, {self.course_accuracy}, " \
-               f"\'{self.datasource}\', \'{self.properties_dict}\'"
+               f"\'{self.datasource}\', \'{self.properties_dict}\', \'{self.routeid}\'"
```

### Comparing `asset_tracking_pepsico-1.0.1/asset_tracking_pepsico/utilities.py` & `asset_tracking_pepsico-1.0.2/asset_tracking_pepsico/utilities.py`

 * *Files identical despite different names*

### Comparing `asset_tracking_pepsico-1.0.1/asset_tracking_pepsico.egg-info/PKG-INFO` & `asset_tracking_pepsico-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: asset-tracking-pepsico
-Version: 1.0.1
+Name: asset_tracking_pepsico
+Version: 1.0.2
 Summary: An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: asset,tracking,pepsico,location,latitude,longitude,store,events
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `asset_tracking_pepsico-1.0.1/pyproject.toml` & `asset_tracking_pepsico-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_tracking_pepsico"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "An asset tracking package where the device logs can be read and the location information can be extracted from the log file provided in the parameters."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["asset", "tracking", "pepsico", "location", "latitude", "longitude", "store", "events"]
```

