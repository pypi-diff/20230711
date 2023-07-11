# Comparing `tmp/flowchem-test-0.1a3.tar.gz` & `tmp/flowchem-test-0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchem-test-0.1a3.tar", last modified: Fri Nov 25 13:29:55 2022, max compression
+gzip compressed data, was "flowchem-test-0.1b1.tar", last modified: Tue Jul 11 16:28:33 2023, max compression
```

## Comparing `flowchem-test-0.1a3.tar` & `flowchem-test-0.1b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 13:29:55.254618 flowchem-test-0.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2022-11-25 13:29:42.000000 flowchem-test-0.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      726 2022-11-25 13:29:55.254618 flowchem-test-0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      181 2022-11-25 13:29:42.000000 flowchem-test-0.1a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2022-11-25 13:29:42.000000 flowchem-test-0.1a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-25 13:29:55.254618 flowchem-test-0.1a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 13:29:55.250618 flowchem-test-0.1a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 13:29:55.250618 flowchem-test-0.1a3/src/flowchem_test/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-11-25 13:29:42.000000 flowchem-test-0.1a3/src/flowchem_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2022-11-25 13:29:42.000000 flowchem-test-0.1a3/src/flowchem_test/fakedevice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-25 13:29:42.000000 flowchem-test-0.1a3/src/flowchem_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      365 2022-11-25 13:29:42.000000 flowchem-test-0.1a3/src/flowchem_test/test_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-25 13:29:55.254618 flowchem-test-0.1a3/src/flowchem_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2022-11-25 13:29:55.000000 flowchem-test-0.1a3/src/flowchem_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2022-11-25 13:29:55.000000 flowchem-test-0.1a3/src/flowchem_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-25 13:29:55.000000 flowchem-test-0.1a3/src/flowchem_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-11-25 13:29:55.000000 flowchem-test-0.1a3/src/flowchem_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-11-25 13:29:55.000000 flowchem-test-0.1a3/src/flowchem_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-11-25 13:29:55.000000 flowchem-test-0.1a3/src/flowchem_test.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:28:33.782167 flowchem-test-0.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-11 16:28:24.000000 flowchem-test-0.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-11 16:28:33.782167 flowchem-test-0.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 16:28:24.000000 flowchem-test-0.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-11 16:28:24.000000 flowchem-test-0.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:28:33.782167 flowchem-test-0.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:28:33.778167 flowchem-test-0.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:28:33.782167 flowchem-test-0.1b1/src/flowchem_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:28:24.000000 flowchem-test-0.1b1/src/flowchem_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-11 16:28:24.000000 flowchem-test-0.1b1/src/flowchem_test/fakedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:28:24.000000 flowchem-test-0.1b1/src/flowchem_test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-11 16:28:24.000000 flowchem-test-0.1b1/src/flowchem_test/test_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:28:33.782167 flowchem-test-0.1b1/src/flowchem_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-11 16:28:33.000000 flowchem-test-0.1b1/src/flowchem_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 16:28:33.000000 flowchem-test-0.1b1/src/flowchem_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:28:33.000000 flowchem-test-0.1b1/src/flowchem_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-11 16:28:33.000000 flowchem-test-0.1b1/src/flowchem_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 16:28:33.000000 flowchem-test-0.1b1/src/flowchem_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 16:28:33.000000 flowchem-test-0.1b1/src/flowchem_test.egg-info/top_level.txt
```

### Comparing `flowchem-test-0.1a3/LICENSE` & `flowchem-test-0.1b1/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,5 @@
-Copyright 2022
-
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `flowchem-test-0.1a3/PKG-INFO` & `flowchem-test-0.1b1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: flowchem-test
-Version: 0.1a3
+Version: 0.1b1
 Summary: Add support for test devices in flowchem.
 Author-email: Dario Cambié <2422614+dcambie@users.noreply.github.com>
 Maintainer-email: Dario Cambié <2422614+dcambie@users.noreply.github.com>
 License: MIT
 Project-URL: repository, https://github.com/cambiegroup/flowchem-test
 Keywords: chemistry,automation,laboratory,testing
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-flowchem-test
-==================
+# flowchem-test
 
 Add test-devices to [flowchem](https://github.com/cambiegroup/flowchem) and serves as an example of how to add support
 to new devices via plugins.
```

### Comparing `flowchem-test-0.1a3/src/flowchem_test/fakedevice.py` & `flowchem-test-0.1b1/src/flowchem_test/fakedevice.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """Fake device for testing purposes. No parameters needed."""
 from collections.abc import Iterable
 
 from flowchem.components.base_component import FlowchemComponent
-from flowchem.devices.flowchem_device import DeviceInfo, Person
+from flowchem.devices.flowchem_device import DeviceInfo
 from flowchem.devices.flowchem_device import FlowchemDevice
+from flowchem.utils.people import dario
 
 from .test_component import TestComponent
 
 
-__all__ = ["FakeDevice"]
-
-dario = Person(name="Dario Cambiè", email="2422614+dcambie@users.noreply.github.com")
-
-
 class FakeDevice(FlowchemDevice):
-
     metadata = DeviceInfo(
         authors=[dario],
         maintainers=[dario],
         manufacturer="virtual-device",
         model="FakeDevice",
         serial_number=42,
         version="v1.0",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flowchem-test-0.1a3/src/flowchem_test.egg-info/PKG-INFO` & `flowchem-test-0.1b1/src/flowchem_test.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: flowchem-test
-Version: 0.1a3
+Version: 0.1b1
 Summary: Add support for test devices in flowchem.
 Author-email: Dario Cambié <2422614+dcambie@users.noreply.github.com>
 Maintainer-email: Dario Cambié <2422614+dcambie@users.noreply.github.com>
 License: MIT
 Project-URL: repository, https://github.com/cambiegroup/flowchem-test
 Keywords: chemistry,automation,laboratory,testing
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-flowchem-test
-==================
+# flowchem-test
 
 Add test-devices to [flowchem](https://github.com/cambiegroup/flowchem) and serves as an example of how to add support
 to new devices via plugins.
```

