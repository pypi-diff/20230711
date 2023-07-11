# Comparing `tmp/dheeobs-0.1.0.tar.gz` & `tmp/dheeobs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dheeobs-0.1.0.tar", last modified: Tue Jun 13 16:35:51 2023, max compression
+gzip compressed data, was "dheeobs-0.1.1.tar", last modified: Tue Jul 11 16:46:57 2023, max compression
```

## Comparing `dheeobs-0.1.0.tar` & `dheeobs-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:35:51.153230 dheeobs-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-13 16:35:51.153230 dheeobs-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-06-02 15:28:40.000000 dheeobs-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:35:51.153230 dheeobs-0.1.0/dheeobs/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-13 16:35:13.000000 dheeobs-0.1.0/dheeobs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-06-13 16:35:13.000000 dheeobs-0.1.0/dheeobs/dhee_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-06-13 16:35:13.000000 dheeobs-0.1.0/dheeobs/dhee_loghandler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:35:51.153230 dheeobs-0.1.0/dheeobs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-13 16:35:51.000000 dheeobs-0.1.0/dheeobs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-13 16:35:51.000000 dheeobs-0.1.0/dheeobs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 16:35:51.000000 dheeobs-0.1.0/dheeobs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-13 16:35:51.000000 dheeobs-0.1.0/dheeobs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 16:35:51.000000 dheeobs-0.1.0/dheeobs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 16:35:51.153230 dheeobs-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-13 16:21:18.000000 dheeobs-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:46:57.045670 dheeobs-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-11 16:46:57.045670 dheeobs-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-06-02 15:28:40.000000 dheeobs-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:46:57.044670 dheeobs-0.1.1/dheeobs/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-11 16:46:04.000000 dheeobs-0.1.1/dheeobs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-11 16:46:04.000000 dheeobs-0.1.1/dheeobs/dhee_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4129 2023-07-11 16:46:04.000000 dheeobs-0.1.1/dheeobs/dhee_loghandler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:46:57.045670 dheeobs-0.1.1/dheeobs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-11 16:46:56.000000 dheeobs-0.1.1/dheeobs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-11 16:46:56.000000 dheeobs-0.1.1/dheeobs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 16:46:56.000000 dheeobs-0.1.1/dheeobs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-11 16:46:56.000000 dheeobs-0.1.1/dheeobs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-11 16:46:56.000000 dheeobs-0.1.1/dheeobs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 16:46:57.045670 dheeobs-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-11 16:45:10.000000 dheeobs-0.1.1/setup.py
```

### Comparing `dheeobs-0.1.0/dheeobs/dhee_logger.py` & `dheeobs-0.1.1/dheeobs/dhee_logger.py`

 * *Files identical despite different names*

### Comparing `dheeobs-0.1.0/dheeobs/dhee_loghandler.py` & `dheeobs-0.1.1/dheeobs/dhee_loghandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,57 +35,65 @@
         """
         Post Logs to InfluxDB Server
         :param record: logging record object
         :return:
         """
         message = self.format(record)
         level = record.levelname
-        log_location = record.filename + "::" + record.funcName + "::" + str(record.lineno)  # Eg., dhee_loghandler.py::post_logs_to_influxdb::45
+        log_location = record.filename + "::" + record.funcName + "::" + str(
+            record.lineno)  # Eg., dhee_loghandler.py::post_logs_to_influxdb::45
 
-        if hasattr(self,'glueContext') and self.glueContext is not None:
-            args =  self.get_commandline_args()
+        if hasattr(self, 'glueContext') and self.glueContext is not None:
+            args = self.get_commandline_args()
         else:
             args = {'INFLUXDB_URL': os.getenv('INFLUXDB_URL'), 'INFLUXDB_ORG': os.getenv('INFLUXDB_ORG'),
                     'INFLUXDB_BUCKET': os.getenv('INFLUXDB_BUCKET'), 'INFLUXDB_TOKEN': os.getenv('INFLUXDB_TOKEN'),
-                    'MEASUREMENT_NAME': os.getenv('MEASUREMENT_NAME')}
+                    'MEASUREMENT_NAME': os.getenv('MEASUREMENT_NAME'), 'PIPELINE_ID': os.getenv('PIPELINE_ID'),
+                    'JOB_RUN_ID': os.getenv('JOB_RUN_ID')}
 
         timestamp = int(datetime.now(timezone.utc).timestamp() * 1000000000)
         url = args['INFLUXDB_URL'] + "/api/v2/write?org=" + args['INFLUXDB_ORG'] + "&bucket=" + args[
             'INFLUXDB_BUCKET'] + "&precision=ns"
         headers = {
             'Authorization': 'Token ' + args['INFLUXDB_TOKEN'],
             'Content-Type': 'text/plain; charset=utf-8'
         }
-        payload = args['MEASUREMENT_NAME'] + ",level=" + level + " message=\"" + message + "\",location=\"" + log_location +"\" " + str(timestamp)
+
+        if 'PIPELINE_ID' not in args:
+            payload = args['MEASUREMENT_NAME'] + ",level=" + level + " message=\"" + message + "\",location=\"" + log_location +"\" " + str(timestamp)
+        else:
+            content = message.split("#")
+            payload = args['MEASUREMENT_NAME'] + ",pipelineId=" + args['PIPELINE_ID'] + ",job_run_id=\"" + args[
+                      'JOB_RUN_ID'] + "\",expectation_type=\"" + content[
+                      0] + "\",column_name=\"" + content[1] + "\",validation_status=\"" + content[2] + "\" values=\"" + content[
+                      3] + "\" " + str(timestamp)
         response = requests.request("POST", url, headers=headers, data=payload)
         response.raise_for_status()
 
     def post_logs_to_cloudwatch(self, record: logging.LogRecord):
         """
         Post Logs to Cloudwatch from AWS Glue Job
         :param record: logging record object
         :return:
         """
-        if hasattr(self,'glueContext') and self.glueContext is not None and "get_logger" in dir(self.glueContext):
+        if hasattr(self, 'glueContext') and self.glueContext is not None and "get_logger" in dir(self.glueContext):
             glue_logger = self.glueContext.get_logger()
             message = self.format(record)
             if record.levelname == "WARNING":
                 glue_logger.warn(message)
             elif record.levelname == "ERROR":
                 glue_logger.error(message)
             elif record.levelname == "DEBUG":
                 glue_logger.debug(message)
             else:
                 glue_logger.info(message)
 
-
     def get_commandline_args(self):
         """
         To get Command Line arguments to setup integration endpoint configuration
         :return:
         """
         arguments_dict = {}
         for index, argument in enumerate(sys.argv):
             if argument.startswith("--"):
                 arguments_dict[argument[2:]] = sys.argv[index + 1]
         return arguments_dict
-
```

