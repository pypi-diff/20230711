# Comparing `tmp/micropython-dftds-0.0.1.tar.gz` & `tmp/micropython-dftds-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-dftds-0.0.1.tar", last modified: Thu Jul  6 23:24:32 2023, max compression
+gzip compressed data, was "micropython-dftds-0.0.2.tar", last modified: Tue Jul 11 20:48:57 2023, max compression
```

## Comparing `micropython-dftds-0.0.1.tar` & `micropython-dftds-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:24:32.134913 micropython-dftds-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-06 23:24:32.134913 micropython-dftds-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-06 23:24:22.000000 micropython-dftds-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:24:32.130913 micropython-dftds-0.0.1/dftds/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 23:24:22.000000 micropython-dftds-0.0.1/dftds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 23:24:22.000000 micropython-dftds-0.0.1/dftds/kvalue_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 23:24:22.000000 micropython-dftds-0.0.1/dftds/kvalue_repository_flash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-06 23:24:22.000000 micropython-dftds-0.0.1/dftds/tds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:24:32.134913 micropython-dftds-0.0.1/micropython_dftds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-06 23:24:32.000000 micropython-dftds-0.0.1/micropython_dftds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-06 23:24:32.000000 micropython-dftds-0.0.1/micropython_dftds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:24:32.000000 micropython-dftds-0.0.1/micropython_dftds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 23:24:32.000000 micropython-dftds-0.0.1/micropython_dftds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 23:24:32.134913 micropython-dftds-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-06 23:24:22.000000 micropython-dftds-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:24:32.134913 micropython-dftds-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-06 23:24:22.000000 micropython-dftds-0.0.1/tests/test_k_value_repository_flash.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-06 23:24:22.000000 micropython-dftds-0.0.1/tests/test_tds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:57.294635 micropython-dftds-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-11 20:48:57.294635 micropython-dftds-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-11 20:48:47.000000 micropython-dftds-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:57.294635 micropython-dftds-0.0.2/dftds/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 20:48:47.000000 micropython-dftds-0.0.2/dftds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 20:48:47.000000 micropython-dftds-0.0.2/dftds/kvalue_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-11 20:48:47.000000 micropython-dftds-0.0.2/dftds/kvalue_repository_flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-11 20:48:47.000000 micropython-dftds-0.0.2/dftds/tds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:57.294635 micropython-dftds-0.0.2/micropython_dftds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-11 20:48:57.000000 micropython-dftds-0.0.2/micropython_dftds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 20:48:57.000000 micropython-dftds-0.0.2/micropython_dftds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:48:57.000000 micropython-dftds-0.0.2/micropython_dftds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 20:48:57.000000 micropython-dftds-0.0.2/micropython_dftds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:48:57.294635 micropython-dftds-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-11 20:48:47.000000 micropython-dftds-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:48:57.294635 micropython-dftds-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-11 20:48:47.000000 micropython-dftds-0.0.2/tests/test_k_value_repository_flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-11 20:48:47.000000 micropython-dftds-0.0.2/tests/test_tds.py
```

### Comparing `micropython-dftds-0.0.1/dftds/kvalue_repository_flash.py` & `micropython-dftds-0.0.2/dftds/kvalue_repository_flash.py`

 * *Files identical despite different names*

### Comparing `micropython-dftds-0.0.1/dftds/tds.py` & `micropython-dftds-0.0.2/dftds/tds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This project was created with the purpose to implement an equivalent of github.com/DFRobot/GravityTDS with micropython.
 """
 import machine
 import ujson
+import time
 
 from dftds.kvalue_repository import KValueRepository
 
 
 TDS_FACTOR = 0.5
 
 class GravityTDS:
@@ -61,16 +62,21 @@
         except OSError as e:
             print(f"error trying to create file: {e}")
 
     def update(self):
         """
         update retrieve a sample from the sensor and calculate the TDS
         """
-        analog_value = self.sensor.read_u16()
-        self.voltage = analog_value/self.adc_range*self.aref
+        analog_values = []
+        for i in range(0, 10):
+            analog_value = self.sensor.read_u16()
+            analog_values.append(analog_value)
+            time.sleep(0.01)
+        avg_analog_value = sum(analog_values)/len(analog_values)
+        self.voltage = avg_analog_value/self.adc_range*self.aref
         ec_value = calculate_ec(self.voltage, self.k_value)
         # temperature compensation
         ec_value_25 = ec_value / (1.0+0.02*(self.temperature-25.0))
         self.tds_value = ec_value_25 * TDS_FACTOR
         return self.tds_value
```

### Comparing `micropython-dftds-0.0.1/setup.py` & `micropython-dftds-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='micropython-dftds',
-    version='0.0.1',
+    version='0.0.2',
     description='MicroPython library for the TDS meter sensor',
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/WendelHime/micropython-dftds',
     project_urls={
         'github': 'https://github.com/WendelHime/micropython-dftds',
     },
```

### Comparing `micropython-dftds-0.0.1/tests/test_k_value_repository_flash.py` & `micropython-dftds-0.0.2/tests/test_k_value_repository_flash.py`

 * *Files identical despite different names*

