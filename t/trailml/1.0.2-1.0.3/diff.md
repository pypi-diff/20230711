# Comparing `tmp/trailml-1.0.2.tar.gz` & `tmp/trailml-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailml-1.0.2.tar", last modified: Wed Jul  5 14:04:05 2023, max compression
+gzip compressed data, was "trailml-1.0.3.tar", last modified: Tue Jul 11 18:31:37 2023, max compression
```

## Comparing `trailml-1.0.2.tar` & `trailml-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.047338 trailml-1.0.2/
--rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-07-05 14:04:05.047181 trailml-1.0.2/PKG-INFO
--rw-r--r--   0 nikolaus   (501) staff       (20)      832 2023-05-29 16:34:46.000000 trailml-1.0.2/README.md
--rw-r--r--   0 nikolaus   (501) staff       (20)      665 2023-07-05 14:02:41.000000 trailml-1.0.2/pyproject.toml
--rw-r--r--   0 nikolaus   (501) staff       (20)       38 2023-07-05 14:04:05.047392 trailml-1.0.2/setup.cfg
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.043511 trailml-1.0.2/src/
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.044316 trailml-1.0.2/src/trail/
--rw-r--r--   0 nikolaus   (501) staff       (20)       44 2023-05-29 16:34:46.000000 trailml-1.0.2/src/trail/__init__.py
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.045110 trailml-1.0.2/src/trail/libconfig/
--rw-r--r--   0 nikolaus   (501) staff       (20)      194 2023-07-05 12:36:48.000000 trailml-1.0.2/src/trail/libconfig/__init__.py
--rw-r--r--   0 nikolaus   (501) staff       (20)      467 2023-05-30 16:59:12.000000 trailml-1.0.2/src/trail/libconfig/config.py
--rw-r--r--   0 nikolaus   (501) staff       (20)    10765 2023-07-05 13:35:09.000000 trailml-1.0.2/src/trail/trail.py
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.046086 trailml-1.0.2/src/trail/userconfig/
--rw-r--r--   0 nikolaus   (501) staff       (20)      650 2023-05-29 16:34:46.000000 trailml-1.0.2/src/trail/userconfig/__init__.py
--rw-r--r--   0 nikolaus   (501) staff       (20)     3074 2023-05-29 16:34:46.000000 trailml-1.0.2/src/trail/userconfig/config.py
--rw-r--r--   0 nikolaus   (501) staff       (20)      859 2023-05-29 16:34:46.000000 trailml-1.0.2/src/trail/userconfig/exceptions.py
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.046964 trailml-1.0.2/src/trailml.egg-info/
--rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-07-05 14:04:05.000000 trailml-1.0.2/src/trailml.egg-info/PKG-INFO
--rw-r--r--   0 nikolaus   (501) staff       (20)      400 2023-07-05 14:04:05.000000 trailml-1.0.2/src/trailml.egg-info/SOURCES.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)        1 2023-07-05 14:04:05.000000 trailml-1.0.2/src/trailml.egg-info/dependency_links.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)       62 2023-07-05 14:04:05.000000 trailml-1.0.2/src/trailml.egg-info/requires.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)        6 2023-07-05 14:04:05.000000 trailml-1.0.2/src/trailml.egg-info/top_level.txt
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-11 18:31:37.028933 trailml-1.0.3/
+-rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-07-11 18:31:37.028742 trailml-1.0.3/PKG-INFO
+-rw-r--r--   0 nikolaus   (501) staff       (20)      832 2023-05-29 16:34:46.000000 trailml-1.0.3/README.md
+-rw-r--r--   0 nikolaus   (501) staff       (20)      665 2023-07-11 18:26:02.000000 trailml-1.0.3/pyproject.toml
+-rw-r--r--   0 nikolaus   (501) staff       (20)       38 2023-07-11 18:31:37.028989 trailml-1.0.3/setup.cfg
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-11 18:31:37.024964 trailml-1.0.3/src/
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-11 18:31:37.025660 trailml-1.0.3/src/trail/
+-rw-r--r--   0 nikolaus   (501) staff       (20)       44 2023-05-29 16:34:46.000000 trailml-1.0.3/src/trail/__init__.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-11 18:31:37.026487 trailml-1.0.3/src/trail/libconfig/
+-rw-r--r--   0 nikolaus   (501) staff       (20)      194 2023-07-05 12:36:48.000000 trailml-1.0.3/src/trail/libconfig/__init__.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)      467 2023-05-30 16:59:12.000000 trailml-1.0.3/src/trail/libconfig/config.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)    10939 2023-07-11 18:24:16.000000 trailml-1.0.3/src/trail/trail.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-11 18:31:37.027348 trailml-1.0.3/src/trail/userconfig/
+-rw-r--r--   0 nikolaus   (501) staff       (20)      650 2023-05-29 16:34:46.000000 trailml-1.0.3/src/trail/userconfig/__init__.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)     3074 2023-05-29 16:34:46.000000 trailml-1.0.3/src/trail/userconfig/config.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)      859 2023-05-29 16:34:46.000000 trailml-1.0.3/src/trail/userconfig/exceptions.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-11 18:31:37.028501 trailml-1.0.3/src/trailml.egg-info/
+-rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-07-11 18:31:37.000000 trailml-1.0.3/src/trailml.egg-info/PKG-INFO
+-rw-r--r--   0 nikolaus   (501) staff       (20)      400 2023-07-11 18:31:37.000000 trailml-1.0.3/src/trailml.egg-info/SOURCES.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)        1 2023-07-11 18:31:37.000000 trailml-1.0.3/src/trailml.egg-info/dependency_links.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)       62 2023-07-11 18:31:37.000000 trailml-1.0.3/src/trailml.egg-info/requires.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)        6 2023-07-11 18:31:37.000000 trailml-1.0.3/src/trailml.egg-info/top_level.txt
```

### Comparing `trailml-1.0.2/PKG-INFO` & `trailml-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailml
-Version: 1.0.2
+Version: 1.0.3
 Summary: Trail ML library
 Author-email: Trail ML <python@trail-ml.com>
 Project-URL: Homepage, https://trail-ml.com
 Project-URL: Bug Tracker, https://github.com/trail-ml/bugtracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trailml-1.0.2/README.md` & `trailml-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `trailml-1.0.2/pyproject.toml` & `trailml-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trailml"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Trail ML", email="python@trail-ml.com" },
 ]
 description = "Trail ML library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `trailml-1.0.2/src/trail/trail.py` & `trailml-1.0.3/src/trail/trail.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,25 @@
             $parentExperimentId: String!,
             $title: String!,
             $comments: String!,
             $instanceRunParameters: GenericScalar!,
             $instanceRunMetrics: GenericScalar!,
             $instanceRunComplete: Boolean!
             $hypothesis: String,
-            $metricsHistoryEntries: [MetricsHistoryInput]
+            $metricsHistoryEntries: [MetricsHistoryInput],
+            $gitCommitHash: String
         ) {
             addExperiment(
                 projectId: $projectId,
                 parentExperimentId: $parentExperimentId,
                 title: $title,
                 comments: $comments,
                 hypothesis: $hypothesis
                 metricsHistory: $metricsHistoryEntries
+                gitCommitHash: $gitCommitHash
                 instanceRuns: {
                     comment: "",
                     parameters: $instanceRunParameters,
                     metrics: $instanceRunMetrics,
                     isComplete: $instanceRunComplete
                 }
             ) {
@@ -118,15 +120,14 @@
         self.artifacts = []
         self.default_handler = signal.getsignal(signal.SIGINT)
         self.is_complete = True
         self.hypothesis = ""
 
     def signal_handler(self, signum, frame):
         self.is_complete = False
-        self.__exit__
         print("Latest run is logged.")
         raise KeyboardInterrupt()
 
     def __enter__(self):
         if mlflow.active_run() is None:
             raise Exception('No active mlflow run found!')
         signal.signal(signal.SIGINT, self.signal_handler)  # type: ignore
@@ -225,24 +226,26 @@
                     'parentExperimentId': self.parent_experiment_id,
                     'title': self.experiment_title,
                     'comments': '',
                     'instanceRunParameters': converted_params,
                     'instanceRunMetrics': run.data.metrics,
                     'instanceRunComplete': self.is_complete,
                     'hypothesis': self.hypothesis,
+                    'gitCommitHash': run.data.tags.get("mlflow.source.git.commit", ""),
                     'metricsHistoryEntries': self.get_metric_history_data(
                         run_id=run_id
                     ),
                 },
             )
 
             experiment_id = result['addExperiment']['experiment']['id']
             self.project_config.update_parent_experiment_id(experiment_id)
             self.parent_experiment_id = experiment_id
-        except TransportQueryError:
+        except TransportQueryError as e:
+            print(e)
             print(
                 'Error uploading experiment data to Trail. Please contact us '
                 'if the problem persists.',
                 file=sys.stderr
             )
 
     def _upload_artifacts(self, run: Run):
```

### Comparing `trailml-1.0.2/src/trail/userconfig/__init__.py` & `trailml-1.0.3/src/trail/userconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `trailml-1.0.2/src/trail/userconfig/config.py` & `trailml-1.0.3/src/trail/userconfig/config.py`

 * *Files identical despite different names*

### Comparing `trailml-1.0.2/src/trail/userconfig/exceptions.py` & `trailml-1.0.3/src/trail/userconfig/exceptions.py`

 * *Files identical despite different names*

### Comparing `trailml-1.0.2/src/trailml.egg-info/PKG-INFO` & `trailml-1.0.3/src/trailml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailml
-Version: 1.0.2
+Version: 1.0.3
 Summary: Trail ML library
 Author-email: Trail ML <python@trail-ml.com>
 Project-URL: Homepage, https://trail-ml.com
 Project-URL: Bug Tracker, https://github.com/trail-ml/bugtracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

