# Comparing `tmp/AutoThaliX-0.1.0.tar.gz` & `tmp/AutoThaliX-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoThaliX-0.1.0.tar", last modified: Sun Apr  9 08:12:44 2023, max compression
+gzip compressed data, was "AutoThaliX-0.2.0.tar", last modified: Tue Jul 11 08:15:56 2023, max compression
```

## Comparing `AutoThaliX-0.1.0.tar` & `AutoThaliX-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:12:44.509395 AutoThaliX-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:12:44.501395 AutoThaliX-0.1.0/AutoThaliX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-09 08:12:44.000000 AutoThaliX-0.1.0/AutoThaliX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-09 08:12:44.000000 AutoThaliX-0.1.0/AutoThaliX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:12:44.000000 AutoThaliX-0.1.0/AutoThaliX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-09 08:12:44.000000 AutoThaliX-0.1.0/AutoThaliX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 08:12:44.000000 AutoThaliX-0.1.0/AutoThaliX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-09 08:12:44.509395 AutoThaliX-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:12:44.505395 AutoThaliX-0.1.0/autothalix/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/autothalix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/autothalix/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/autothalix/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/autothalix/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:12:44.509395 AutoThaliX-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:12:44.509395 AutoThaliX-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/tests/test_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/tests/test_imp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/tests/test_lsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/tests/test_ocp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:15:56.283480 AutoThaliX-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:15:56.279480 AutoThaliX-0.2.0/AutoThaliX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-11 08:15:56.000000 AutoThaliX-0.2.0/AutoThaliX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 08:15:56.000000 AutoThaliX-0.2.0/AutoThaliX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:15:56.000000 AutoThaliX-0.2.0/AutoThaliX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 08:15:56.000000 AutoThaliX-0.2.0/AutoThaliX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 08:15:56.000000 AutoThaliX-0.2.0/AutoThaliX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-11 08:15:56.279480 AutoThaliX-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:15:56.279480 AutoThaliX-0.2.0/autothalix/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/autothalix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/autothalix/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14916 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/autothalix/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/autothalix/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 08:15:56.283480 AutoThaliX-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:15:56.279480 AutoThaliX-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/tests/test_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/tests/test_eis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/tests/test_imp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/tests/test_lsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-11 08:14:39.000000 AutoThaliX-0.2.0/tests/test_ocp.py
```

### Comparing `AutoThaliX-0.1.0/AutoThaliX.egg-info/PKG-INFO` & `AutoThaliX-0.2.0/AutoThaliX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThaliX
-Version: 0.1.0
+Version: 0.2.0
 Summary: A set of tools to work with tales potentiostats. Uses tales_remote
 Home-page: https://github.com/Arkady-A/autothalix
 Author: ArkadyA
 Author-email: arkadymirz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AutoThaliX-0.1.0/LICENSE` & `AutoThaliX-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.1.0/PKG-INFO` & `AutoThaliX-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThaliX
-Version: 0.1.0
+Version: 0.2.0
 Summary: A set of tools to work with tales potentiostats. Uses tales_remote
 Home-page: https://github.com/Arkady-A/autothalix
 Author: ArkadyA
 Author-email: arkadymirz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AutoThaliX-0.1.0/README.md` & `AutoThaliX-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.1.0/autothalix/measurements.py` & `AutoThaliX-0.2.0/autothalix/measurements.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,14 +102,28 @@
     def _start_measurements(self):
         pass
 
     @abstractmethod
     def _send_parameters(self):
         pass
 
+    @property
+    def potentiostat_mode(self):
+        return self._PotentiostatMode
+
+    @potentiostat_mode.setter
+    def potentiostat_mode(self, value: str):
+        mapping = {
+            'pseudogalvanostatic': PotentiostatMode.POTMODE_PSEUDOGALVANOSTATIC,
+            'galvanostatic': PotentiostatMode.POTMODE_GALVANOSTATIC,
+            'potentiostatic': PotentiostatMode.POTMODE_POTENTIOSTATIC,
+        }
+
+        self._PotentiostatMode = mapping[str.lower(value)]
+
 
 class CyclicVoltammetry(BaseMeasurement):
     """
     Cyclic Voltammetry measurement class. Inherits from BaseMeasurement class."""
     _measurement_name = 'cv'
     _measurement_full_name = 'Cyclic Voltammetry'
 
@@ -216,35 +230,74 @@
         self.wr_connection.setIEThirdEdgePotentialRelation(self.third_edge_potential_relation)
 
     def _start_measurements(self):
         self.wr_connection.checkIESetup()
         self.wr_connection.measureIE()
 
 
+class ElectrochemicalImpedanceSpectroscopy(BaseMeasurement):
+    """ Electrochemical Impedance Spectroscopy measurement class"""
+
+    _measurement_name = 'eis'
+    _measurement_full_name = 'Electrochemical Impedance Spectroscopy'
+
+    def __str__(self):
+        return self._measurement_name
+
+    def _send_parameters(self):
+        self.wr_connection.setPotentiostatMode(self.potentiostat_mode)
+        self.wr_connection.setAmplitude(self.amplitude)
+        self.wr_connection.setPotential(self.potential)
+        self.wr_connection.setLowerFrequencyLimit(self.lower_frequency_limit)
+        self.wr_connection.setStartFrequency(self.start_frequency)
+        self.wr_connection.setUpperFrequencyLimit(self.upper_frequency_limit)
+        self.wr_connection.setLowerNumberOfPeriods(self.lower_number_of_periods)
+        self.wr_connection.setLowerStepsPerDecade(self.lower_steps_per_decade)
+        self.wr_connection.setUpperNumberOfPeriods(self.upper_number_of_periods)
+        self.wr_connection.setUpperStepsPerDecade(self.upper_steps_per_decade)
+        self.wr_connection.setScanDirection(self.scan_direction)
+        self.wr_connection.setScanStrategy(self.scan_strategy)
+        self.wr_connection.setEISOutputPath(self.output_path)
+        self.wr_connection.setEISOutputFileName(self._output_filename)
+        self.wr_connection.setEISNaming(self.naming)
+    
+    @property
+    def parameters(self):
+        """Returns a list of mandatory parameters for IE measurement"""
+        return [
+            "potentiostat_mode",
+            "amplitude",
+            "potential",
+            "lower_frequency_limit",
+            "start_frequency",
+            "upper_frequency_limit",
+            "lower_number_of_periods",
+            "lower_steps_per_decade",
+            "upper_number_of_periods",
+            "upper_steps_per_decade",
+            "scan_direction",
+            "scan_strategy",
+            "output_path",
+            "naming",
+        ]
+
+    def _start_measurements(self):
+        self.wr_connection.enablePotentiostat()
+        self.wr_connection.measureEIS()    
+        self.wr_connection.disablePotentiostat()
+
+
 class BaseManualMeasurements(BaseMeasurement, ABC):
     """
     Base class for manual measurements
     """
 
     def __init__(self, wr_connection: ThalesRemoteScriptWrapper, measurement_id: str, **kwargs):
         super().__init__(wr_connection, measurement_id, **kwargs)
 
-    @property
-    def potentiostat_mode(self):
-        return self._PotentiostatMode
-
-    @potentiostat_mode.setter
-    def potentiostat_mode(self, value: str):
-        mapping = {
-            'pseudogalvanostatic': PotentiostatMode.POTMODE_PSEUDOGALVANOSTATIC,
-            'galvanostatic': PotentiostatMode.POTMODE_GALVANOSTATIC,
-            'potentiostatic': PotentiostatMode.POTMODE_POTENTIOSTATIC,
-        }
-
-        self._PotentiostatMode = mapping[str.lower(value)]
 
     def _save_data(self):
         logger.info(f"Saving {self.measurement_name} data to {self._output_filename}.csv")
         write_dict_to_csv(self.measured_data, os.path.join(self.output_path, self._output_filename + '.csv'))
 
     def run(self):
         super().run()
```

### Comparing `AutoThaliX-0.1.0/autothalix/utils.py` & `AutoThaliX-0.2.0/autothalix/utils.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.1.0/setup.py` & `AutoThaliX-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 install_requires = [req.strip() for req in requirements]
 
 setuptools.setup(
     name="AutoThaliX",
-    version="0.1.0",
+    version="0.2.0",
     author="ArkadyA",
     author_email="arkadymirz@gmail.com",
     description="A set of tools to work with tales potentiostats. Uses tales_remote",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Arkady-A/autothalix",
     packages=setuptools.find_packages(),
```

### Comparing `AutoThaliX-0.1.0/tests/test_cv.py` & `AutoThaliX-0.2.0/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.1.0/tests/test_imp.py` & `AutoThaliX-0.2.0/tests/test_imp.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.1.0/tests/test_lsv.py` & `AutoThaliX-0.2.0/tests/test_lsv.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.1.0/tests/test_ocp.py` & `AutoThaliX-0.2.0/tests/test_ocp.py`

 * *Files identical despite different names*

