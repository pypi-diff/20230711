# Comparing `tmp/vlsirtools-3.0.dev3.tar.gz` & `tmp/vlsirtools-4.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlsirtools-3.0.dev3.tar", last modified: Tue Jan 17 23:17:19 2023, max compression
+gzip compressed data, was "vlsirtools-4.0.0rc0.tar", last modified: Tue Jul 11 16:48:18 2023, max compression
```

## Comparing `vlsirtools-3.0.dev3.tar` & `vlsirtools-4.0.0rc0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:19.928967 vlsirtools-3.0.dev3/
--rw-r--r--   0 dan        (501) staff       (20)     2772 2022-12-19 18:57:12.000000 vlsirtools-3.0.dev3/.gitignore
--rw-r--r--   0 dan        (501) staff       (20)     1521 2022-06-15 18:46:18.000000 vlsirtools-3.0.dev3/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)     3099 2023-01-17 23:17:19.928770 vlsirtools-3.0.dev3/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2794 2022-12-19 18:57:12.000000 vlsirtools-3.0.dev3/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-01-17 23:17:19.929014 vlsirtools-3.0.dev3/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1102 2023-01-17 23:14:16.000000 vlsirtools-3.0.dev3/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:19.921878 vlsirtools-3.0.dev3/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-06-13 20:36:42.000000 vlsirtools-3.0.dev3/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    20330 2023-01-17 23:14:13.000000 vlsirtools-3.0.dev3/tests/test_vlsirtools.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:19.922454 vlsirtools-3.0.dev3/vlsirtools/
--rw-r--r--   0 dan        (501) staff       (20)      149 2022-07-19 02:39:52.000000 vlsirtools-3.0.dev3/vlsirtools/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:19.925505 vlsirtools-3.0.dev3/vlsirtools/netlist/
--rw-r--r--   0 dan        (501) staff       (20)     3291 2022-11-03 17:38:34.000000 vlsirtools-3.0.dev3/vlsirtools/netlist/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    20856 2022-11-04 17:51:25.000000 vlsirtools-3.0.dev3/vlsirtools/netlist/base.py
--rw-r--r--   0 dan        (501) staff       (20)     9225 2022-12-19 18:57:12.000000 vlsirtools-3.0.dev3/vlsirtools/netlist/spectre.py
--rw-r--r--   0 dan        (501) staff       (20)     2112 2022-11-03 17:38:34.000000 vlsirtools-3.0.dev3/vlsirtools/netlist/spectre_spice_shared.py
--rw-r--r--   0 dan        (501) staff       (20)    18024 2022-12-06 02:10:08.000000 vlsirtools-3.0.dev3/vlsirtools/netlist/spice.py
--rw-r--r--   0 dan        (501) staff       (20)    10559 2022-11-03 17:38:34.000000 vlsirtools-3.0.dev3/vlsirtools/netlist/verilog.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:19.925785 vlsirtools-3.0.dev3/vlsirtools/spectre/
--rw-r--r--   0 dan        (501) staff       (20)      122 2022-07-19 02:39:52.000000 vlsirtools-3.0.dev3/vlsirtools/spectre/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:19.928192 vlsirtools-3.0.dev3/vlsirtools/spice/
--rw-r--r--   0 dan        (501) staff       (20)       84 2022-11-03 17:38:34.000000 vlsirtools-3.0.dev3/vlsirtools/spice/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     6180 2022-11-03 17:38:34.000000 vlsirtools-3.0.dev3/vlsirtools/spice/base.py
--rw-r--r--   0 dan        (501) staff       (20)    18589 2022-12-06 02:10:08.000000 vlsirtools-3.0.dev3/vlsirtools/spice/ngspice.py
--rw-r--r--   0 dan        (501) staff       (20)     7030 2022-12-19 18:57:12.000000 vlsirtools-3.0.dev3/vlsirtools/spice/sim_data.py
--rw-r--r--   0 dan        (501) staff       (20)    15986 2022-11-03 17:38:34.000000 vlsirtools-3.0.dev3/vlsirtools/spice/spectre.py
--rw-r--r--   0 dan        (501) staff       (20)     5673 2022-12-19 18:57:12.000000 vlsirtools-3.0.dev3/vlsirtools/spice/spice.py
--rw-r--r--   0 dan        (501) staff       (20)    14854 2022-12-19 18:57:12.000000 vlsirtools-3.0.dev3/vlsirtools/spice/xyce.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:19.928367 vlsirtools-3.0.dev3/vlsirtools/xyce/
--rw-r--r--   0 dan        (501) staff       (20)      113 2022-07-19 02:39:52.000000 vlsirtools-3.0.dev3/vlsirtools/xyce/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:19.923315 vlsirtools-3.0.dev3/vlsirtools.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     3099 2023-01-17 23:17:19.000000 vlsirtools-3.0.dev3/vlsirtools.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      710 2023-01-17 23:17:19.000000 vlsirtools-3.0.dev3/vlsirtools.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-01-17 23:17:19.000000 vlsirtools-3.0.dev3/vlsirtools.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       94 2023-01-17 23:17:19.000000 vlsirtools-3.0.dev3/vlsirtools.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       17 2023-01-17 23:17:19.000000 vlsirtools-3.0.dev3/vlsirtools.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:18.748022 vlsirtools-4.0.0rc0/
+-rw-r--r--   0 dan        (501) staff       (20)     2772 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/.gitignore
+-rw-r--r--   0 dan        (501) staff       (20)     1521 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)     2676 2023-07-11 16:48:18.747828 vlsirtools-4.0.0rc0/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2368 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-11 16:48:18.748065 vlsirtools-4.0.0rc0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     1152 2023-07-11 16:44:54.000000 vlsirtools-4.0.0rc0/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:18.743748 vlsirtools-4.0.0rc0/tests/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2022-06-13 20:36:42.000000 vlsirtools-4.0.0rc0/tests/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     3790 2023-06-28 18:09:23.000000 vlsirtools-4.0.0rc0/tests/test_primitives.py
+-rw-r--r--   0 dan        (501) staff       (20)    21524 2023-06-28 18:09:23.000000 vlsirtools-4.0.0rc0/tests/test_vlsirtools.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:18.744450 vlsirtools-4.0.0rc0/vlsirtools/
+-rw-r--r--   0 dan        (501) staff       (20)      596 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:18.746309 vlsirtools-4.0.0rc0/vlsirtools/netlist/
+-rw-r--r--   0 dan        (501) staff       (20)     3571 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/netlist/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    31903 2023-06-28 18:09:27.000000 vlsirtools-4.0.0rc0/vlsirtools/netlist/base.py
+-rw-r--r--   0 dan        (501) staff       (20)    14534 2023-06-28 18:09:27.000000 vlsirtools-4.0.0rc0/vlsirtools/netlist/spectre.py
+-rw-r--r--   0 dan        (501) staff       (20)     2112 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/netlist/spectre_spice_shared.py
+-rw-r--r--   0 dan        (501) staff       (20)    26324 2023-06-28 18:09:27.000000 vlsirtools-4.0.0rc0/vlsirtools/netlist/spice.py
+-rw-r--r--   0 dan        (501) staff       (20)    10660 2023-06-28 18:09:27.000000 vlsirtools-4.0.0rc0/vlsirtools/netlist/verilog.py
+-rw-r--r--   0 dan        (501) staff       (20)    16639 2023-06-28 18:09:23.000000 vlsirtools-4.0.0rc0/vlsirtools/primitives.py
+-rw-r--r--   0 dan        (501) staff       (20)     6456 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/pytest.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:18.746456 vlsirtools-4.0.0rc0/vlsirtools/spectre/
+-rw-r--r--   0 dan        (501) staff       (20)      122 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/spectre/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:18.747428 vlsirtools-4.0.0rc0/vlsirtools/spice/
+-rw-r--r--   0 dan        (501) staff       (20)       84 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/spice/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     4907 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/spice/base.py
+-rw-r--r--   0 dan        (501) staff       (20)    12654 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/spice/ngspice.py
+-rw-r--r--   0 dan        (501) staff       (20)     7030 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/spice/sim_data.py
+-rw-r--r--   0 dan        (501) staff       (20)    11256 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/spice/spectre.py
+-rw-r--r--   0 dan        (501) staff       (20)     5412 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/spice/spice.py
+-rw-r--r--   0 dan        (501) staff       (20)    14053 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/spice/xyce.py
+-rw-r--r--   0 dan        (501) staff       (20)     3459 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/spicetype.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:18.747579 vlsirtools-4.0.0rc0/vlsirtools/xyce/
+-rw-r--r--   0 dan        (501) staff       (20)      113 2023-06-26 21:21:08.000000 vlsirtools-4.0.0rc0/vlsirtools/xyce/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:48:18.745434 vlsirtools-4.0.0rc0/vlsirtools.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     2676 2023-07-11 16:48:18.000000 vlsirtools-4.0.0rc0/vlsirtools.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      805 2023-07-11 16:48:18.000000 vlsirtools-4.0.0rc0/vlsirtools.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-11 16:48:18.000000 vlsirtools-4.0.0rc0/vlsirtools.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       97 2023-07-11 16:48:18.000000 vlsirtools-4.0.0rc0/vlsirtools.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       17 2023-07-11 16:48:18.000000 vlsirtools-4.0.0rc0/vlsirtools.egg-info/top_level.txt
```

### Comparing `vlsirtools-3.0.dev3/.gitignore` & `vlsirtools-4.0.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `vlsirtools-3.0.dev3/LICENSE` & `vlsirtools-4.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `vlsirtools-3.0.dev3/PKG-INFO` & `vlsirtools-4.0.0rc0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: vlsirtools
-Version: 3.0.dev3
+Version: 4.0.0rc0
 Summary: Tools for the Vlsir IC Design Schema
 Home-page: https://github.com/Vlsir/Vlsir
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # Vlsir Tools 
 
@@ -28,47 +28,34 @@
     """Enumerated, Internally-Defined Spice-Class Simulators"""
 
     SPECTRE = "spectre"
     XYCE = "xyce"
     NGSPICE = "ngspice"
 ```
 
-The primary entry-point for simulation is `vlsirtools.spice.sim`. 
+The primary entry-point for simulation is `vlsirtools.spice.sim`. By default, `sim` runs your chosen simulator in parallel over the list of `SimInputs` provided as `inp`.
 
 ```python
 def sim(
     inp: OneOrMore[vsp.SimInput], opts: Optional[SimOptions] = None
 ) -> OneOrMore[SimResultUnion]:
 ```
 
 The `sim` function takes as input one or more `vlsir.spice.SimInput`s and a set of simulation options (`vlsirtools.spice.SimOptions`), and returns one of two result-types depending on its input `options`.
 
-
 ```python
 class ResultFormat(Enum):
     """Enumerated Result Formats"""
 
     SIM_DATA = "sim_data" 
     VLSIR_PROTO = "vlsir_proto" 
 ```
 
 The `VLSIR_PROTO` result-format returns a `vlsir.spice.SimResult` object, which is a protobuf-encoded representation of the simulation results. The `SIM_DATA` format instead uses the types defined in `vlsirtools.spice.sim_data`, a python-native combination of dataclasses and numpy arrays. The former is generally more convenient for sharing with other programs, and the latter for further in-Python processing. 
 
-Simulations can be invoked asynchronously by instead invoking `vlsirtools.spice.sim_async`. 
-Its interface is identical to `vlsirtools.spice.sim`, but for returning an `Awaitable`. 
-
-```python
-async def sim_async(
-    inp: OneOrMore[vsp.SimInput], opts: Optional[SimOptions] = None
-) -> Awaitable[OneOrMore[SimResultUnion]]:
-```
-
-Asynchronously invoking simulation is particularly valuable for large batches of simulations, 
-e.g. for "corner" or other parametric variations, as the simulator invocations can be run in parallel.
-
 ### Simulator and Analysis Support
 
 Each spice-class simulator includes its own netlist syntax and opinions about the specification for analyses. 
 The `vlsir.spice` schema  
 
 | Analysis             | Spectre            | Xyce               | NgSpice     |
 | -------------------- | ------------------ | ------------------ | ------------------ |
```

### Comparing `vlsirtools-3.0.dev3/readme.md` & `vlsirtools-4.0.0rc0/vlsirtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: vlsirtools
+Version: 4.0.0rc0
+Summary: Tools for the Vlsir IC Design Schema
+Home-page: https://github.com/Vlsir/Vlsir
+Author: Dan Fritchman
+Author-email: dan@fritch.mn
+Requires-Python: >=3.7, <3.12
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 
 # Vlsir Tools 
 
 Python-based tools and utilites for working with the Vlsir IC design schema. 
 
 ## Netlisting 
 
@@ -16,47 +28,34 @@
     """Enumerated, Internally-Defined Spice-Class Simulators"""
 
     SPECTRE = "spectre"
     XYCE = "xyce"
     NGSPICE = "ngspice"
 ```
 
-The primary entry-point for simulation is `vlsirtools.spice.sim`. 
+The primary entry-point for simulation is `vlsirtools.spice.sim`. By default, `sim` runs your chosen simulator in parallel over the list of `SimInputs` provided as `inp`.
 
 ```python
 def sim(
     inp: OneOrMore[vsp.SimInput], opts: Optional[SimOptions] = None
 ) -> OneOrMore[SimResultUnion]:
 ```
 
 The `sim` function takes as input one or more `vlsir.spice.SimInput`s and a set of simulation options (`vlsirtools.spice.SimOptions`), and returns one of two result-types depending on its input `options`.
 
-
 ```python
 class ResultFormat(Enum):
     """Enumerated Result Formats"""
 
     SIM_DATA = "sim_data" 
     VLSIR_PROTO = "vlsir_proto" 
 ```
 
 The `VLSIR_PROTO` result-format returns a `vlsir.spice.SimResult` object, which is a protobuf-encoded representation of the simulation results. The `SIM_DATA` format instead uses the types defined in `vlsirtools.spice.sim_data`, a python-native combination of dataclasses and numpy arrays. The former is generally more convenient for sharing with other programs, and the latter for further in-Python processing. 
 
-Simulations can be invoked asynchronously by instead invoking `vlsirtools.spice.sim_async`. 
-Its interface is identical to `vlsirtools.spice.sim`, but for returning an `Awaitable`. 
-
-```python
-async def sim_async(
-    inp: OneOrMore[vsp.SimInput], opts: Optional[SimOptions] = None
-) -> Awaitable[OneOrMore[SimResultUnion]]:
-```
-
-Asynchronously invoking simulation is particularly valuable for large batches of simulations, 
-e.g. for "corner" or other parametric variations, as the simulator invocations can be run in parallel.
-
 ### Simulator and Analysis Support
 
 Each spice-class simulator includes its own netlist syntax and opinions about the specification for analyses. 
 The `vlsir.spice` schema  
 
 | Analysis             | Spectre            | Xyce               | NgSpice     |
 | -------------------- | ------------------ | ------------------ | ------------------ |
```

### Comparing `vlsirtools-3.0.dev3/setup.py` & `vlsirtools-4.0.0rc0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 
 """
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 import pathlib
 
-here = pathlib.Path(__file__).parent.resolve()
-
 # Get the long description from the README file
-long_description = (here / "readme.md").read_text(encoding="utf-8")
+here = pathlib.Path(__file__).parent.resolve()
+readme = here / "readme.md"
+long_description = "" if not readme.exists() else readme.read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "3.0.dev3"
+_VLSIR_VERSION = "4.0.0rc0"
 
 setup(
     name="vlsirtools",
     version=_VLSIR_VERSION,
     description="Tools for the Vlsir IC Design Schema",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Vlsir/Vlsir",
     author="Dan Fritchman",
     author_email="dan@fritch.mn",
     packages=find_packages(),
-    python_requires=">=3.7, <4",
+    python_requires=">=3.7, <3.12",
     install_requires=[
         f"vlsir=={_VLSIR_VERSION}",  # VLSIR Core Python Bindings
-        "numpy==1.21.5",  # For `sim_data` simulation results
-        "pandas",  # For CSV reading
+        "numpy~=1.21",  # For `sim_data` simulation results
+        "pandas~=1.3",  # For CSV reading
     ],
     extras_require={
         "dev": ["pytest==7.1", "coverage", "pytest-cov", "black==22.6", "twine"]
     },
 )
```

### Comparing `vlsirtools-3.0.dev3/tests/test_vlsirtools.py` & `vlsirtools-4.0.0rc0/tests/test_vlsirtools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 # Vlsir Python Tools
 Unit Tests
 """
 
+import numpy as np
 import pytest
 from io import StringIO
-from pathlib import Path
 from typing import Dict, List, Optional
 
 import vlsir.utils_pb2 as vutils
 from vlsir.utils_pb2 import Reference, QualifiedName, ParamValue, Param
 import vlsir.circuit_pb2 as vckt
 from vlsir.circuit_pb2 import (
     Module,
@@ -138,16 +138,26 @@
     def default_conns() -> Dict:
         # Shorthand for connections between node "vvv" and "VSS", used for many instances below.
         return _connections(
             p=ConnectionTarget(sig="vvv"),
             n=ConnectionTarget(sig="VSS"),
         )
 
+    # Create ExternalModules for a few model-based device-types
+    mos1 = vlsirtools.primitives.mos(name="mos1", domain="mymodels")
+    d1 = vlsirtools.primitives.diode(name="d1", domain="mymodels")
+    bjt1 = vlsirtools.primitives.bipolar(name="bjt1", domain="mymodels")
+    t1 = vlsirtools.primitives.tline(name="t1", domain="mymodels")
+
+    def _eref(emod: vckt.ExternalModule) -> Reference:
+        return Reference(external=emod.name)
+
     pkg = Package(
         domain="vlsir.tests.test_netlist1",
+        ext_modules=[mos1, d1, bjt1, t1],
         modules=[
             Module(
                 name="mid",
                 parameters=_params(
                     r=ParamValue(double=1e3),
                     l=ParamValue(double=1e-9),
                     c=ParamValue(double=1e-15),
@@ -186,46 +196,52 @@
                     ),
                     Instance(
                         name="i",
                         module=_prim("isource"),
                         connections=default_conns(),
                         parameters=_params(dc=ParamValue(double=1e-6)),
                     ),
+                    # Model-based instances
                     Instance(
                         name="m",
-                        module=_prim("mos"),
+                        module=_eref(mos1),
                         connections=_connections(
                             d=ConnectionTarget(sig="VSS"),
                             g=ConnectionTarget(sig="VSS"),
                             s=ConnectionTarget(sig="VSS"),
                             b=ConnectionTarget(sig="VSS"),
                         ),
-                        parameters=_params(
-                            modelname=ParamValue(string="some_model_name")
-                        ),
+                        parameters=[],
                     ),
                     Instance(
                         name="q",
-                        module=_prim("bipolar"),
+                        module=_eref(bjt1),
                         connections=_connections(
                             c=ConnectionTarget(sig="VSS"),
                             b=ConnectionTarget(sig="VSS"),
                             e=ConnectionTarget(sig="VSS"),
                         ),
-                        parameters=_params(
-                            modelname=ParamValue(string="some_model_name")
-                        ),
+                        parameters=[],
                     ),
                     Instance(
                         name="d",
-                        module=_prim("diode"),
+                        module=_eref(d1),
                         connections=default_conns(),
-                        parameters=_params(
-                            modelname=ParamValue(string="some_model_name")
+                        parameters=[],
+                    ),
+                    Instance(
+                        name="t",
+                        module=_eref(t1),
+                        connections=_connections(
+                            p1p=ConnectionTarget(sig="VSS"),
+                            p1n=ConnectionTarget(sig="VSS"),
+                            p2p=ConnectionTarget(sig="VSS"),
+                            p2n=ConnectionTarget(sig="VSS"),
                         ),
+                        parameters=[],
                     ),
                 ],
             ),
             Module(
                 name="top",
                 ports=[
                     Port(direction="NONE", signal="VSS"),
@@ -416,14 +432,15 @@
 
     # Run it, requesting in-memory `SimData` results.
     sd_results = sim(
         inp=inp,
         opts=SimOptions(
             simulator=simulator,
             fmt=ResultFormat.SIM_DATA,
+            rundir="./scratch",
         ),
     )
 
     # Check a handful of things about what comes back
     assert isinstance(sd_results, sd.SimResult)
     if AnalysisType.OP not in skip:
         assert isinstance(sd_results[AnalysisType.OP], sd.OpResult)
@@ -446,57 +463,93 @@
     )
     assert isinstance(proto_results, vsp.SimResult)
 
     # And return the `sim_data` version for any further inspection.
     return sd_results
 
 
-@pytest.mark.skipif(
-    not vlsirtools.spectre.available(),
-    reason="No spectre installation on path",
-)
+@pytest.mark.spectre
 def test_spectre1():
     """Test an empty-input call to the `vlsir.spice.Sim` interface to `spectre`."""
     dummy_sim_tests(SupportedSimulators.SPECTRE)
 
 
-@pytest.mark.skipif(
-    not vlsirtools.xyce.available(),
-    reason="No Xyce installation on path",
-)
+@pytest.mark.xyce
 def test_xyce1():
     """Test an empty-input call to the `vlsir.spice.Sim` interface to `xyce`."""
     dummy_sim_tests(SupportedSimulators.XYCE)
 
 
-@pytest.mark.skipif(
-    not vlsirtools.spice.ngspice.available(),
-    reason="No ngspice installation on path",
-)
+@pytest.mark.ngspice
 def test_ngspice1():
     """Test an empty-input call to the `vlsir.spice.Sim` interface to `ngspice`."""
-    dummy_sim_tests(SupportedSimulators.NGSPICE, skip=[AnalysisType.DC])
+
+    res = dummy_sim_tests(
+        SupportedSimulators.NGSPICE,
+        skip=[
+            AnalysisType.DC
+        ],  ## Skip the DC sweep; ngspice doesn't support this kinda sweep
+    )
+
+    # Check that the AC frequency vector came back as expected
+    # A follow-on from https://github.com/Vlsir/Vlsir/issues/66
+    freqs = np.array(
+        [
+            1.00000000e03,
+            1.25892541e03,
+            1.58489319e03,
+            1.99526231e03,
+            2.51188643e03,
+            3.16227766e03,
+            3.98107171e03,
+            5.01187234e03,
+            6.30957344e03,
+            7.94328235e03,
+            1.00000000e04,
+            1.25892541e04,
+            1.58489319e04,
+            1.99526231e04,
+            2.51188643e04,
+            3.16227766e04,
+            3.98107171e04,
+            5.01187234e04,
+            6.30957344e04,
+            7.94328235e04,
+            1.00000000e05,
+            1.25892541e05,
+            1.58489319e05,
+            1.99526231e05,
+            2.51188643e05,
+            3.16227766e05,
+            3.98107171e05,
+            5.01187234e05,
+            6.30957344e05,
+            7.94328235e05,
+            1.00000000e06,
+        ]
+    )
+    ac_result = res[AnalysisType.AC]
+    assert np.allclose(ac_result.freq, freqs)
 
 
+@pytest.mark.xyce
 def test_xyce_import():
     # Just test importing from the `vlsirtools.xyce` path
     # FIXME: probably deprecate this
     from vlsirtools.xyce import sim
 
 
+@pytest.mark.spectre
 def test_spectre_import():
     # Just test importing from the `vlsirtools.spectre` path
     # FIXME: probably deprecate this
     from vlsirtools.spectre import sim
 
 
-@pytest.mark.skipif(
-    not vlsirtools.spice.ngspice.available(),
-    reason="No ngspice installation on path",
-)
+@pytest.mark.ngspice
 def test_noise1():
     """Test the Noise analysis"""
 
     # A very complicated testbench: a voltage source and resistor in parallel.
     pkg = vckt.Package(
         domain="vlsirtools.tests.test_noise1",
         modules=[
@@ -573,15 +626,7 @@
     )
     vlsirtools.spice.sim(
         sim_input,
         opts=SimOptions(
             simulator=SupportedSimulators.NGSPICE, fmt=ResultFormat.SIM_DATA
         ),
     )
-
-
-@pytest.mark.xfail(reason="#41 https://github.com/Vlsir/Vlsir/issues/41")
-def test_theres_a_simulator_available():
-    """Test that there is at least one simulator available for testing.
-    This is... debatable whether we wanna do it? A good idea, but tough to set up e.g. on CI servers.
-    And basically impossible for anything with a paid license."""
-    assert vlsirtools.spice.default() is not None
```

### Comparing `vlsirtools-3.0.dev3/vlsirtools/netlist/__init__.py` & `vlsirtools-4.0.0rc0/vlsirtools/netlist/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     Includes string-value conversion."""
 
     VERILOG = "verilog"
     SPECTRE = "spectre"
 
     # Spice Dialects
     SPICE = "spice"
-    HSPICE = "hspice"
     NGSPICE = "ngspice"
     XYCE = "xyce"
+    HSPICE = "hspice"
     CDL = "cdl"
 
     @staticmethod
     def get(spec: "NetlistFormatSpec") -> "NetlistFormat":
         """Get the format specified by `spec`, in either enum or string terms.
         Only does real work in the case when `spec` is a string, otherwise returns it unchanged."""
         if isinstance(spec, (NetlistFormat, str)):
@@ -72,17 +72,21 @@
     indent: str = 2 * " "  # Indentation. Defaults to two spaces.
     width: int = 80  # Line-width. Defaults to 80.
 
 
 # Type-alias for specifying format, either in enum or string terms
 NetlistFormatSpec = Union[NetlistFormat, str]
 
+## FIXME: add more `Netlistable`s
+##Netlistable = Union[vlsir.circuit.Package]
+Netlistable = vlsir.circuit.Package
+
 
 def netlist(
-    pkg: vlsir.circuit.Package,
+    pkg: Netlistable,  ## FIXME: rename
     dest: IO,
     fmt: NetlistFormatSpec = "spectre",
     opts: Optional[NetlistOptions] = None,
 ) -> None:
     """Netlist proto-Package `pkg` to destination `dest`.
 
     Example usages:
@@ -105,15 +109,20 @@
     Format-specifier `fmt` may be any of the `NetlistFormatSpec` enumerated values
     or their string equivalents.
     """
 
     if opts is not None:
         raise NotImplementedError("NetlistOptions not yet implemented.")  # FIXME!
 
+    # If `fmt` is a string, turn it into an enum
     fmt_enum = NetlistFormat.get(fmt)
+
+    # Get the corresponding `Netlister` class and instantiate it
     netlister_cls = fmt_enum.netlister()
-    netlister = netlister_cls(pkg, dest)
-    netlister.netlist()
+    netlister = netlister_cls(dest=dest)
+
+    # Write the netlist
+    return netlister.write_package(pkg)
 
 
 # Set our exported content for star-imports
 __all__ = ["netlist", "NetlistFormat", "NetlistFormatSpec"]
```

### Comparing `vlsirtools-3.0.dev3/vlsirtools/netlist/spectre.py` & `vlsirtools-4.0.0rc0/vlsirtools/netlist/verilog.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,245 +1,280 @@
 """
-# Spectre-Format Netlister
+# Verilog-Format Netlister 
 """
-
-# Std-Lib Imports
-from typing import Union, List
-
 # Local Imports
 import vlsir
+import vlsir.circuit_pb2 as vckt
 
 # Import the base-class
-from .spectre_spice_shared import SpectreSpiceShared
-from .base import Netlister, ResolvedModule, ResolvedParams, SpicePrefix
-
-
-def map_primitive(rmodule: ResolvedModule, paramvals: ResolvedParams) -> str:
-    """Map a primitive into Spectre's supported names and parameters.
-    Returns the "apparent module name" for instances of the primitive.
-    Argument `paramvals` is often modified along the way.
-
-    Note spectre syntax is such that the "apparent module name" can be either of:
-    (a) a fixed name per spice-prefix, for basic types (r, c, l, etc), or
-    (b) the *model* name for model-based devices, (mos, bjt, diode, etc)"""
-
-    # For voltage sources, add spectre's "type" parameter, and potentially rename several parameters
-    if rmodule.spice_prefix == SpicePrefix.VSOURCE:
-        vname = rmodule.module_name
-        vtypes = dict(
-            vdc="dc",
-            vpulse="pulse",
-            vsin="sine",
-        )
-        if vname not in vtypes:
-            msg = f"Invalid or unsupported voltage-source type {vname}"
-            raise ValueError(msg)
-        paramvals.set("type", vtypes[vname])
-
-        if vname == "vpulse":
-            # For pulse sources, need to rename most parameters
-            paramvals.rename("v1", "val0")
-            paramvals.rename("v2", "val1")
-            paramvals.rename("td", "delay")
-            paramvals.rename("tr", "rise")
-            paramvals.rename("tf", "fall")
-            paramvals.rename("tpw", "width")
-            paramvals.rename("tper", "period")
-        elif vname == "vdc":
-            if "ac" in paramvals:
-                paramvals.rename("ac", "mag")
-
-    # Mapping from spice-prefix to spectre-name for fixed-name types
-    basics = {
-        SpicePrefix.RESISTOR: "resistor",
-        SpicePrefix.CAPACITOR: "capacitor",
-        SpicePrefix.INDUCTOR: "inductor",
-        SpicePrefix.VSOURCE: "vsource",
-        SpicePrefix.ISOURCE: "isource",
-        SpicePrefix.VCVS: "vcvs",
-        SpicePrefix.VCCS: "vccs",
-        SpicePrefix.CCCS: "cccs",
-        SpicePrefix.CCVS: "ccvs",
-    }
-    if rmodule.spice_prefix in basics:
-        return basics[rmodule.spice_prefix]
-
-    # Other primitive-types get an "apparent module name" equal to their *model* name.
-    model_based = {
-        SpicePrefix.MOS,
-        SpicePrefix.BIPOLAR,
-        SpicePrefix.DIODE,
-        SpicePrefix.TLINE,
-    }
-    if rmodule.spice_prefix in model_based:
-        # Get the model-name from its instance parameters
-        return paramvals.pop("modelname")
-
-    # Otherwise, unclear what this is or how we got here.
-    raise RuntimeError(f"Unsupported or Invalid Primitive {rmodule}")
+from .base import Netlister, ResolvedModule, ResolvedParams
 
 
-class SpectreNetlister(SpectreSpiceShared):
-    """Spectre-Format Netlister"""
+class VerilogNetlister(Netlister):
+    """
+    # Structural Verilog Netlister
+    """
 
     @property
     def enum(self):
         """Get our entry in the `NetlistFormat` enumeration"""
         from . import NetlistFormat
 
-        return NetlistFormat.SPECTRE
+        return NetlistFormat.VERILOG
 
-    def write_module_definition(self, module: vlsir.circuit.Module) -> None:
-        """Create a Spectre-format definition for proto-Module `module`"""
+    def write_module_definition(self, module: vckt.Module) -> None:
+        """Create a Verilog module definition for proto-Module `module`"""
 
         # Create the module name
         module_name = self.get_module_name(module)
         # Check for double-definition
         if module_name in self.module_names:
             raise RuntimeError(f"Module {module_name} doubly defined")
         # Add to our visited lists
         self.module_names.add(module_name)
         self.pmodules[module.name] = module
 
-        # Collect and index vlsir.circuit.Signals in this Module by name.
+        # Collect and index vckt.Signals in this Module by name.
         self.collect_signals_by_name(module)
 
-        # Create the sub-circuit definition header
-        self.writeln(f"subckt {module_name} ")
-        self.indent += 1
+        # Create the module header
+        self.writeln(f"module {module_name}")
+
+        # Write its parameters, if defined
+        self.write_param_declarations(module)
 
         if module.ports:  # Create its ports
-            self.writeln(
-                "+ "
-                + " ".join([self.format_port_decl(pport) for pport in module.ports])
-                + " "
-            )
+            # Don't forget, a trailing comma after the last one is fatal to high-tech Verilog parsers!
+            self.writeln("( ")
+            self.indent += 1
+            for num, pport in enumerate(module.ports):
+                comma = "" if num == len(module.ports) - 1 else ","
+                self.writeln(self.format_port_decl(pport) + comma)
+            self.indent -= 1
+            self.writeln("); ")
         else:
-            self.writeln("+ // No ports ")
+            self.writeln("( ) ;  // No ports ")
+
+        self.writeln("")  # Blank line to end "header" facets
+        self.indent += 1
+
+        # Write the internal signal declarations
+        self.write_internal_signal_declarations()
 
-        # Create its parameters, if defined
-        if module.parameters:
-            formatted = [self.format_param_decl(pparam) for pparam in module.parameters]
-            formatted = " ".join(formatted)
-            self.writeln("parameters " + formatted + " ")
+        if module.instances:  # Create its instances
+            self.writeln("")
+            self.writeln("// Instance Declarations")
+            for pinst in module.instances:
+                self.write_instance(pinst)
         else:
-            self.writeln("+ // No parameters ")
+            self.writeln("// No Instances")
 
-        self.writeln("")  # End "header" facets
-        # Note nothing need be done for internal signals;
-        # spice and spectre create these "out of thin air"
-
-        # Create its instances
-        for pinst in module.instances:
-            self.write_instance(pinst)
-        self.writeln("")
+        # Write any netlist-literal content
+        self.write_literals(module.literals)
 
-        # Close up the sub-circuit
+        # Close up the module
         self.indent -= 1
-        self.writeln("ends \n")
+        self.writeln("")  # Blank before `endmodule`
+        self.writeln(f"endmodule // {module_name} \n\n")
 
-    def write_instance(self, pinst: vlsir.circuit.Instance) -> None:
-        """Create and return a netlist-string for Instance `pinst`"""
+    def write_internal_signal_declarations(self) -> None:
+        if not self.internal_signals_by_name:
+            return self.writeln("// No Signal Declarations")
+
+        self.writeln("// Signal Declarations")
+        for psig in self.internal_signals_by_name.values():
+            self.writeln(self.format_signal_decl(psig) + "; ")
+
+    def write_param_declarations(self, module: vlsir.circuit.Module) -> None:
+        """Write the parameter declarations for Module `module`."""
+
+        if not len(module.parameters):  # No parameters
+            # Note we check `len` because `module.parameters` is a protobuf thing, and *who knows* how it converts to `bool`.
+            return self.writeln("// No parameters ")
+
+        # Get all the formatted parameter-strings
+        formatted = [self.format_param_decl(param) for param in module.parameters]
+        # Add the commas to all *BUT THE LAST*. Like JSON, Verilog demands it, or fails.
+        formatted = [d + "," for d in formatted[:-1]] + [formatted[-1]]
 
-        # Initial resolution phase.
-        # Start by getting the Module or ExternalModule definition
+        # Write them all to our destination
+        self.writeln("#( ")
+        self.indent += 1
+        [self.writeln(f) for f in formatted]
+        self.indent -= 1
+        self.writeln(") \n")
+
+    def write_instance(self, pinst: vckt.Instance) -> None:
+        """Format and write Instance `pinst`"""
+
+        # Get its Module or ExternalModule definition
         rmodule = self.resolve_reference(pinst.module)
+        if not isinstance(rmodule, ResolvedModule):
+            # Spice-level primitives and models are generally not available in Verilog runtimes,
+            # and hence generate errors here if attempted in netlisting.
+            raise RuntimeError(f"Invalid module for Verilog: {rmodule}")
+        module, module_name = rmodule.module, rmodule.module_name
 
         # Resolve its parameter values
-        resolved_instance_parameters = self.get_instance_params(pinst, rmodule.module)
+        resolved_instance_parameters = self.get_instance_params(pinst, module)
 
-        module, module_name = rmodule.module, rmodule.module_name
-        if rmodule.spice_prefix == SpicePrefix.SUBCKT:
-            module_name = rmodule.module_name
-        else:  # Primitive element. Look up spectre-format module-name
-            module_name = map_primitive(rmodule, resolved_instance_parameters)
+        # Write the module-name
+        self.writeln(module_name)
+
+        # Write its parameter-values
+        self.write_instance_params(resolved_instance_parameters)
 
-        # Create the instance name
-        self.writeln(pinst.name + "")
+        # Write the instance name
+        self.writeln(pinst.name)
 
-        if module.ports:
-            self.writeln("+ // Ports: ")
+        if module.ports:  # Write connections, by-name, in-order
+            self.writeln("( ")
+            self.indent += 1
             # Get `module`'s port-order
             port_order = [pport.signal for pport in module.ports]
-            # And write the Instance ports, in that order
-            pconns = []
             connection_targets = {
                 connection.portname: connection.target
                 for connection in pinst.connections
             }
-            for pname in port_order:
-                pconn = connection_targets.get(pname, None)
-                if pconn is None:
+            # And write the Instance ports, in that order
+            for num, pname in enumerate(port_order):
+                ptarget = connection_targets.get(pname, None)
+                if ptarget is None:
                     raise RuntimeError(f"Unconnected Port {pname} on {pinst.name}")
-                pconns.append(pconn)
-            self.writeln(
-                "+ ( "
-                + " ".join([self.format_connection_target(pconn) for pconn in pconns])
-                + " )"
-            )
+                # Again a trailing comma after the last one is fatal!
+                comma = "" if num == len(port_order) - 1 else ","
+                self.writeln(
+                    f".{pname}({self.format_connection_target(ptarget)}){comma} "
+                )
+            # Close up the ports
+            self.indent -= 1
+            self.writeln("); ")
         else:
-            self.writeln("+ // No ports ")
-
-        # Write the module-name
-        self.writeln("+  " + module_name + " ")
+            self.writeln("// No ports ")
 
-        # Write the instance parameters
-        self.write_instance_params(resolved_instance_parameters)
-
-        # And add a post-instance blank line
-        self.writeln("")
+        self.writeln("")  # Post-Instance blank line
 
     def write_instance_params(self, pvals: ResolvedParams) -> None:
         """Write Instance parameters `pvals`"""
         if not pvals:
-            return self.writeln("+ // No parameters ")
-        # Write its parameter-values
-        formatted = " ".join([f"{pname}={pval}" for pname, pval in pvals.items()])
-        self.writeln("+  " + formatted + " ")
+            return self.writeln("// No parameters ")
 
-    def format_concat(self, pconc: vlsir.circuit.Concat) -> str:
-        """Format the Concatenation of several other Connections"""
-        out = ""
-        for part in pconc.parts:
-            out += self.format_connection_target(part) + " "
-        return out
-
-    def format_port_decl(self, pport: vlsir.circuit.Port) -> str:
-        """Get a netlist `Port` definition"""
-        # In Spectre, as well as most spice, this syntax is the same as referring to the Port.
-        return self.format_port_ref(pport)
+        # Write the parameter-values
+        self.writeln("#( ")
+        self.indent += 1
+        # ANSI-style params: .NAME(VALUE)
+        formatted = ", ".join([f".{pname}({pval})" for pname, pval in pvals.items()])
+        self.writeln(formatted)
+        self.indent -= 1
+        self.writeln(") ")
 
-    def format_port_ref(self, pport: vlsir.circuit.Port) -> str:
-        """Get a netlist `Port` reference"""
-        return self.format_signal_ref(self.get_signal(pport.signal))
+    @classmethod
+    def format_param_type(cls, pparam: vlsir.Param) -> str:
+        """Verilog type-string for `Parameter` `param`."""
+        ptype = pparam.WhichOneof("value")
+        if ptype == "integer":
+            return "longint"
+        if ptype == "double":
+            return "real"
+        if ptype == "string":
+            return "string"
+        raise ValueError
 
     @classmethod
-    def format_signal_ref(cls, psig: vlsir.circuit.Signal) -> str:
-        """Get a netlist definition for Signal `psig`"""
-        if psig.width < 1:
-            raise RuntimeError
-        if psig.width == 1:  # width==1, i.e. a scalar signal
-            return psig.name
-        # Vector/ multi "bit" Signal. Creates several spice signals.
-        return " ".join(
-            [f"{psig.name}{cls.format_bus_bit(k)}" for k in reversed(range(psig.width))]
-        )
+    def format_param_decl(cls, param: vlsir.Param) -> str:
+        """Format a parameter-declaration"""
+        rv = f"parameter {param.name}"
+        # FIXME: whether to include datatype
+        # dtype = cls.format_param_type(param)
+        default = cls.get_param_default(param)
+        if default is not None:
+            rv += f" = {default}"
+        return rv
+
+    def format_concat(self, pconc: vckt.Concat) -> str:
+        """Format the Concatenation of several other Connections"""
+        # Verilog { a, b, c } concatenation format
+        parts = [self.format_connection_target(part) for part in pconc.parts]
+        return "{" + ", ".join(parts) + "}"
+
+    def format_port_decl(self, pport: vckt.Port) -> str:
+        """Format a `Port` declaration"""
+
+        # First retrieve and check the validity of its direction
+        port_type_to_str = {
+            vckt.Port.Direction.Value("INPUT"): "input",
+            vckt.Port.Direction.Value("OUTPUT"): "output",
+            vckt.Port.Direction.Value("INOUT"): "inout",
+            vckt.Port.Direction.Value("NONE"): "NO_DIRECTION",
+        }
+        dir_ = port_type_to_str.get(pport.direction, None)
+        if dir_ is None:
+            msg = f"Invalid Verilog netlisting for unknown Port direction {pport.direction}"
+            raise RuntimeError(msg)
+        if dir_ == "NO_DIRECTION":
+            msg = f"Invalid Verilog netlisting for undirected Port {pport}"
+            raise RuntimeError(msg)
+
+        return dir_ + " " + self.format_signal_decl(self.get_signal(pport.signal))
+
+    def format_signal_decl(self, psig: vckt.Signal) -> str:
+        """Format a `Signal` declaration"""
+        rv = "wire"
+        if psig.width > 1:
+            rv += f" [{psig.width-1}:0]"
+        rv += f" {psig.name}"
+        return rv
+
+    def format_port_ref(self, pport: vckt.Port) -> str:
+        """Format a reference to a `Port`.
+        Unlike declarations, this just requires the name of its `Signal`."""
+        return self.format_signal_ref(self.get_signal(pport.signal))
 
     @classmethod
-    def format_signal_slice(cls, pslice: vlsir.circuit.Slice) -> str:
-        """Get a netlist definition for Signal-Slice `pslice`"""
-        base = pslice.signal
-        indices = list(reversed(range(pslice.bot, pslice.top + 1)))
-        if not len(indices):
-            raise RuntimeError(f"Attempting to netlist empty slice {pslice}")
-        return " ".join([f"{base}{cls.format_bus_bit(k)}" for k in indices])
+    def format_signal_ref(cls, psig: vckt.Signal) -> str:
+        """Format a reference to a `Signal`.
+        Unlike declarations, this just requires its name."""
+        return psig.name
 
     @classmethod
-    def format_bus_bit(cls, index: Union[int, str]) -> str:
-        """Format-specific string-representation of a bus bit-index"""
-        # Spectre netlisting uses an underscore prefix, e.g. `bus_0`
-        return "_" + str(index)
+    def format_signal_slice(cls, pslice: vckt.Slice) -> str:
+        """Format Signal-Slice `pslice`"""
+        if pslice.top == pslice.bot:  # Single-bit slice
+            return f"{pslice.signal}[{pslice.top}]"
+        return f"{pslice.signal}[{pslice.top}:{pslice.bot}]"  # Multi-bit slice
 
     def write_comment(self, comment: str) -> None:
-        """While Spectre *can* do a bunch of other comment-styles,
-        the canonical one is generally the C-style line comment beginning with `//`."""
-        self.writeln(f"// {comment}")
+        """Verilog uses C-style line comments, beginning with `//`"""
+        self.write(f"// {comment}\n")
+
+    @classmethod
+    def format_prefix(cls, pre: vlsir.SIPrefix) -> str:
+        """Format a `SIPrefix` to a string"""
+        # Verilog does not have the SI prefixes built in. Always write the exponent value.
+        map = {
+            # Single-character aliases, supported by every SPICE we know
+            vlsir.SIPrefix.YOCTO: "e-24",
+            vlsir.SIPrefix.ZEPTO: "e-21",
+            vlsir.SIPrefix.ATTO: "e-18",
+            vlsir.SIPrefix.FEMTO: "e-15",
+            vlsir.SIPrefix.PICO: "e-12",
+            vlsir.SIPrefix.NANO: "e-9",
+            vlsir.SIPrefix.MICRO: "e-6",
+            vlsir.SIPrefix.MILLI: "e-3",
+            vlsir.SIPrefix.CENTI: "e-2",
+            vlsir.SIPrefix.DECI: "e-1",
+            vlsir.SIPrefix.UNIT: "",
+            vlsir.SIPrefix.DECA: "e1",
+            vlsir.SIPrefix.HECTO: "e2",
+            vlsir.SIPrefix.KILO: "e3",
+            vlsir.SIPrefix.MEGA: "e6",
+            vlsir.SIPrefix.GIGA: "e9",
+            vlsir.SIPrefix.TERA: "e12",
+            vlsir.SIPrefix.PETA: "e15",
+            vlsir.SIPrefix.EXA: "e17",
+            vlsir.SIPrefix.ZETTA: "e18",
+            vlsir.SIPrefix.YOTTA: "e19",
+        }
+        if pre not in map:
+            raise ValueError(f"Invalid or Unsupported SIPrefix {pre}")
+
+        return map[pre]
```

### Comparing `vlsirtools-3.0.dev3/vlsirtools/netlist/spectre_spice_shared.py` & `vlsirtools-4.0.0rc0/vlsirtools/netlist/spectre_spice_shared.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-3.0.dev3/vlsirtools/netlist/spice.py` & `vlsirtools-4.0.0rc0/vlsirtools/netlist/spice.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,22 +29,31 @@
 
 "Spice" netlisting therefore requires a small family of "Spice Dialects", 
 heavily re-using a central `SpiceNetlister` class, but requiring simulator-specific implementation details. 
 
 """
 
 # Std-Lib Imports
-from typing import Dict, Union
+from typing import Union
 
 # Local Imports
 import vlsir
+import vlsir.circuit_pb2 as vckt
+import vlsir.spice_pb2 as vsp
 
 # Import the base-class
 from .spectre_spice_shared import SpectreSpiceShared
-from .base import Netlister, ResolvedModule, ResolvedParams, SpicePrefix, ModuleLike
+from .base import (
+    ResolvedModule,
+    ResolvedParams,
+    SpiceType,
+    ModuleLike,
+    SpiceBuiltin,
+    SpiceModelRef,
+)
 
 
 class SpiceNetlister(SpectreSpiceShared):
     """
     # "Generic" Spice Netlister
     and base-class for Spice dialects.
 
@@ -60,32 +69,32 @@
     @property
     def enum(self):
         """Get our entry in the `NetlistFormat` enumeration"""
         from . import NetlistFormat
 
         return NetlistFormat.SPICE
 
-    def write_module_definition(self, module: vlsir.circuit.Module) -> None:
+    def write_module_definition(self, module: vckt.Module) -> None:
         """Write the `SUBCKT` definition for `Module` `module`."""
 
         # Create the module name
         module_name = self.get_module_name(module)
         # Check for double-definition
         if module_name in self.module_names:
             raise RuntimeError(f"Module {module_name} doubly defined")
 
-        # Collect and index vlsir.circuit.Signals in this Module by name.
+        # Collect and index vckt.Signals in this Module by name.
         self.collect_signals_by_name(module)
 
         # Add to our visited lists
         self.module_names.add(module_name)
         self.pmodules[module.name] = module
 
         # Create the sub-circuit definition header
-        self.write(f".SUBCKT {module_name} \n")
+        self.writeln(f".SUBCKT {module_name}")
 
         # Create its ports, if any are defined
         if module.ports:
             self.write_port_declarations(module)
         else:
             self.write_comment("No ports")
 
@@ -98,149 +107,191 @@
         # End the `subckt` header-content with a blank line
         self.write("\n")
 
         # Create its instances
         for pinst in module.instances:
             self.write_instance(pinst)
 
+        # Write any netlist-literal content
+        self.write_literals(module.literals)
+
         # And close up the sub-circuit
         self.write(".ENDS\n\n")
 
-    def write_port_declarations(self, module: vlsir.circuit.Module) -> None:
+    def write_port_declarations(self, module: vckt.Module) -> None:
         """Write the port declarations for Module `module`."""
         self.write("+ ")
         for pport in module.ports:
             self.write(self.format_port_decl(pport) + " ")
         self.write("\n")
 
-    def write_param_declarations(self, module: vlsir.circuit.Module) -> None:
+    def write_param_declarations(self, module: vckt.Module) -> None:
         """Write the parameter declarations for Module `module`.
-        Parameter declaration format: `name1=val1 name2=val2 name3=val3 \n`"""
+        Parameter declaration format: `name1=val1 name2=val2 name3=val3`"""
         self.write("+ ")
         for pparam in module.parameters:
             self.write(self.format_param_decl(pparam))
         self.write("\n")
 
     def write_instance_name(
-        self, pinst: vlsir.circuit.Instance, rmodule: ResolvedModule
+        self,
+        pinst: vckt.Instance,
+        spice_type: SpiceType = SpiceType.SUBCKT,
     ) -> None:
         """Write the instance-name line for `pinst`, including the SPICE-dictated primitive-prefix."""
-        self.write(f"{rmodule.spice_prefix.value}{pinst.name} \n")
+        self.writeln(f"{spice_type.value}{pinst.name}")
 
-    def write_instance(self, pinst: vlsir.circuit.Instance) -> None:
+    def write_instance(self, pinst: vckt.Instance) -> None:
         """Create and return a netlist-string for Instance `pinst`"""
 
-        # Get its Module or ExternalModule definition,
-        resolved = self.resolve_reference(pinst.module)
+        # Resolve what kinda thing we are to instantiate
+        ref = self.resolve_reference(pinst.module)
 
-        # And dispatch to `subckt` or `primitive` writers
-        if resolved.spice_prefix == SpicePrefix.SUBCKT:
-            return self.write_subckt_instance(pinst, resolved)
-
-        if resolved.spice_prefix == SpicePrefix.VSOURCE:
-            # Voltage sources get weird, and vary between dialiects. Farm them out to a dedicated method.
-            return self.write_voltage_source_instance(pinst, resolved)
-
-        # Everything else falls into the `primitive` category
-        return self.write_primitive_instance(pinst, resolved)
+        # And dispatch to our writers
+        if isinstance(ref, ResolvedModule):
+            return self.write_subckt_instance(pinst, ref)
+
+        if isinstance(ref, SpiceModelRef):
+            return self.write_model_instance(pinst, ref)
+
+        if isinstance(ref, SpiceBuiltin):
+            if ref.spice_type == SpiceType.VSOURCE:
+                # Voltage sources get weird, and vary between dialiects. Farm them out to a dedicated method.
+                return self.write_voltage_source_instance(pinst, ref)
+
+            # Everything else falls into the `primitive` category
+            return self.write_primitive_instance(pinst, ref)
+
+        raise RuntimeError(f"Unrecognized reference type {ref}")
+
+    def write_model_instance(self, pinst: vckt.Instance, ref: SpiceModelRef) -> None:
+        """# Write a `.model` instance.
+        While sub-classes may modify this behavior, the default is to produce netlist-content
+        very similar to that of `write_subckt_instance`, hence the sharing via `write_instance_inner`."""
+
+        return self.write_instance_inner(
+            pinst=pinst,
+            module=ref.module,
+            module_name=ref.model_name,
+            spice_type=ref.spice_type,
+        )
 
     def write_subckt_instance(
-        self, pinst: vlsir.circuit.Instance, rmodule: ResolvedModule
+        self, pinst: vckt.Instance, rmodule: ResolvedModule
+    ) -> None:
+        """# Write a subcircuit instance.
+        While sub-classes may modify this behavior, the default is to produce netlist-content
+        very similar to that of `write_model_instance`, hence the sharing via `write_instance_inner`."""
+
+        return self.write_instance_inner(
+            pinst=pinst,
+            module=rmodule.module,
+            module_name=rmodule.module_name,
+            spice_type=SpiceType.SUBCKT,
+        )
+
+    def write_instance_inner(
+        self,
+        pinst: vckt.Instance,
+        module: ModuleLike,
+        module_name: str,
+        spice_type: SpiceType,
     ) -> None:
-        """Write sub-circuit-instance `pinst` of `rmodule`."""
+        """Inner implementation of `write_subckt_instance` and `write_model_instance`"""
 
         # Write the instance name
-        self.write_instance_name(pinst, rmodule)
+        self.write_instance_name(pinst, spice_type=spice_type)
 
         # Write its port-connections
-        self.write_instance_conns(pinst, rmodule.module)
+        self.write_instance_conns(pinst, module)
 
         # Write the sub-circuit name
-        self.write("+ " + rmodule.module_name + " \n")
+        self.writeln("+ " + module_name)
 
         # Write its parameter values
-        resolved_param_values = self.get_instance_params(pinst, rmodule.module)
+        resolved_param_values = self.get_instance_params(pinst, module)
         self.write_instance_params(resolved_param_values)
 
         # Add a blank after each instance
         self.write("\n")
+        ...
 
-    def write_primitive_instance(
-        self, pinst: vlsir.circuit.Instance, rmodule: ResolvedModule
-    ) -> None:
+    def write_primitive_instance(self, pinst: vckt.Instance, ref: SpiceBuiltin) -> None:
         """Write primitive-instance `pinst` of `rmodule`.
         Note spice's primitive instances often differn syntactically from sub-circuit instances,
         in that they can have positional (only) parameters."""
 
         # Write the instance name
-        self.write_instance_name(pinst, rmodule)
+        self.write_instance_name(pinst, ref.spice_type)
 
         # Write its port-connections
-        self.write_instance_conns(pinst, rmodule.module)
+        self.write_instance_conns(pinst, ref.module)
 
         # Resolve its parameter-values to spice-strings
-        resolved_param_values = self.get_instance_params(pinst, rmodule.module)
+        resolved_param_values = self.get_instance_params(pinst, ref.module)
 
         # Write special and/or positional parameters
-        if rmodule.spice_prefix == SpicePrefix.RESISTOR:
+        if ref.spice_type == SpiceType.RESISTOR:
             positional_keys = ["r"]
-        elif rmodule.spice_prefix == SpicePrefix.CAPACITOR:
+        elif ref.spice_type == SpiceType.CAPACITOR:
             positional_keys = ["c"]
-        elif rmodule.spice_prefix == SpicePrefix.INDUCTOR:
+        elif ref.spice_type == SpiceType.INDUCTOR:
             positional_keys = ["l"]
-        elif rmodule.spice_prefix == SpicePrefix.ISOURCE:
+        elif ref.spice_type == SpiceType.ISOURCE:
             positional_keys = ["dc"]
-        elif rmodule.spice_prefix in (
-            SpicePrefix.VCVS,
-            SpicePrefix.VCCS,
-            SpicePrefix.CCCS,
-            SpicePrefix.CCVS,
-        ):
+        elif ref.spice_type in {
+            SpiceType.VCVS,
+            SpiceType.VCCS,
+            SpiceType.CCCS,
+            SpiceType.CCVS,
+        }:
             positional_keys = ["gain"]
-        elif rmodule.spice_prefix in (
-            SpicePrefix.MOS,
-            SpicePrefix.BIPOLAR,
-            SpicePrefix.DIODE,
-            SpicePrefix.TLINE,
-        ):
-            positional_keys = ["modelname"]
+        elif ref.spice_type in {
+            SpiceType.MOS,
+            SpiceType.BIPOLAR,
+            SpiceType.DIODE,
+            SpiceType.TLINE,
+        }:
+            raise RuntimeError(f"Internal error: {ref} should be netlisted as a model")
+        elif ref.spice_type == SpiceType.SUBCKT:
+            raise RuntimeError(f"Internal error: {ref} should be netlisted as a subckt")
         else:
-            positional_keys = []
+            raise RuntimeError(f"Unrecognized primitive type {ref.spice_type}")
 
         # Pop all positional parameters ("pp") from `resolved_param_values`
         pp = resolved_param_values.pop_many(positional_keys)
 
         # Write the positional parameters, in the order specified by `positional_keys`
-        self.write("+ " + " ".join([pp[pkey] for pkey in positional_keys]) + " \n")
+        self.writeln("+ " + " ".join([pp[pkey] for pkey in positional_keys]))
 
         # Now! Write its subckt-style by-name parameter values
         self.write_instance_params(resolved_param_values)
 
         # Add a blank after each instance
         self.write("\n")
 
     def write_voltage_source_instance(
         self,
-        pinst: vlsir.circuit.Instance,
-        rmodule: ResolvedModule,
+        pinst: vckt.Instance,
+        ref: SpiceBuiltin,
     ) -> None:
         """Write a voltage-source instance `pinst`.
         Throws an Exception if `rmodule` is not a known voltage-source type."""
 
         # Resolve its parameter values
-        resolved_param_values = self.get_instance_params(pinst, rmodule.module)
+        resolved_param_values = self.get_instance_params(pinst, ref.module)
 
         # Write the instance name
-        self.write_instance_name(pinst, rmodule)
+        self.write_instance_name(pinst, ref.spice_type)
 
         # Write its port-connections
-        self.write_instance_conns(pinst, rmodule.module)
+        self.write_instance_conns(pinst, ref.module)
 
         # Handle each of the voltage-source cases
-        name = rmodule.module.name.name
+        name = ref.module.name.name
         if name == "vdc":
             dc = resolved_param_values.pop("dc")
             self.write(f"+ dc {self.format_expression(dc)} \n")
             ac = resolved_param_values.pop("ac")
             self.write(f"+ ac {self.format_expression(ac)} \n")
 
         elif name == "vpulse":
@@ -266,17 +317,15 @@
 
         # Now! Write its subckt-style by-name parameter values
         self.write_instance_params(resolved_param_values)
 
         # Add a blank after each instance
         self.write("\n")
 
-    def write_instance_conns(
-        self, pinst: vlsir.circuit.Instance, module: ModuleLike
-    ) -> None:
+    def write_instance_conns(self, pinst: vckt.Instance, module: ModuleLike) -> None:
         """Write the port-connections for Instance `pinst`"""
 
         # Write a quick comment for port-less modules
         if not module.ports:
             self.write("+ ")
             return self.write_comment("No ports")
 
@@ -312,45 +361,45 @@
 
         # And write them
         for (pname, pval) in pvals.items():
             self.write(f"{pname}={self.format_expression(pval)} ")
 
         self.write("\n")
 
-    def format_concat(self, pconc: vlsir.circuit.Concat) -> str:
+    def format_concat(self, pconc: vckt.Concat) -> str:
         """Format the Concatenation of several other Connections"""
         out = ""
         for part in pconc.parts:
             out += self.format_connection_target(part) + " "
         return out
 
-    def format_port_decl(self, pport: vlsir.circuit.Port) -> str:
+    def format_port_decl(self, pport: vckt.Port) -> str:
         """Get a netlist `Port` definition"""
         signal = self.get_signal(pport.signal)
         return self.format_signal_ref(signal)
 
-    def format_port_ref(self, pport: vlsir.circuit.Port) -> str:
+    def format_port_ref(self, pport: vckt.Port) -> str:
         """Get a netlist `Port` reference"""
         signal = self.get_signal(pport.signal)
         return self.format_signal_ref(signal)
 
     @classmethod
-    def format_signal_ref(cls, psig: vlsir.circuit.Signal) -> str:
+    def format_signal_ref(cls, psig: vckt.Signal) -> str:
         """Get a netlist definition for Signal `psig`"""
         if psig.width < 1:
             raise RuntimeError
         if psig.width == 1:  # width==1, i.e. a scalar signal
             return psig.name
         # Vector/ multi "bit" Signal. Creates several spice signals.
         return " ".join(
             [f"{psig.name}{cls.format_bus_bit(k)}" for k in reversed(range(psig.width))]
         )
 
     @classmethod
-    def format_signal_slice(cls, pslice: vlsir.circuit.Slice) -> str:
+    def format_signal_slice(cls, pslice: vckt.Slice) -> str:
         """Get a netlist definition for Signal-Slice `pslice`"""
         base = pslice.signal
         indices = list(reversed(range(pslice.bot, pslice.top + 1)))
         if not len(indices):
             raise RuntimeError(f"Attempting to netlist empty slice {pslice}")
         return " ".join([f"{base}{cls.format_bus_bit(k)}" for k in indices])
 
@@ -402,15 +451,15 @@
     @property
     def enum(self):
         """Get our entry in the `NetlistFormat` enumeration"""
         from . import NetlistFormat
 
         return NetlistFormat.XYCE
 
-    def write_param_declarations(self, module: vlsir.circuit.Module) -> None:
+    def write_param_declarations(self, module: vckt.Module) -> None:
         """Write the parameter declarations for Module `module`.
         Parameter declaration format:
         .SUBCKT <name> <ports>
         + PARAMS: name1=val1 name2=val2 name3=val3 \n
         """
         self.write("+ PARAMS: ")  # <= Xyce-specific
         for pparam in module.parameters:
@@ -445,28 +494,207 @@
         So, just use it all the time."""
         self.write(f"; {comment}\n")
 
     def format_expression(self, expr: str) -> str:
         # Xyce expressions are wrapped in curly braces.
         return f"{{{expr}}}"
 
+    @classmethod
+    def format_sim_dut(cls, module_name: str) -> str:
+        """# Format the top-level DUT instance for module name `module_name`."""
+        return f"xtop 0 {module_name} ; Top-Level DUT \n"
+
+    def write_include(self, inc: vsp.Include) -> None:
+        """# Write an `Include`"""
+        self.writeln(f".include '{inc.path}'")
+
+    def write_lib_include(self, lib: vsp.LibInclude) -> None:
+        """# Write a `LibInclude`"""
+        self.writeln(f".lib {lib.path} {lib.section}")
+
+    def write_save(self, save: vsp.Save) -> None:
+        # FIXME!
+        raise NotImplementedError(f"Unimplemented control card {save} for {self}")
+
+    def write_meas(self, meas: vsp.Meas) -> None:
+        """# Write a measurement."""
+        line = f".meas {meas.analysis_type} {meas.name} {meas.expr} \n"
+        self.writeln(line)
+
+    def write_sim_param(self, param: vlsir.Param) -> None:
+        """# Write a simulation parameter."""
+        line = f".param {param.name}={self.get_param_value(param.value)} \n"
+        self.writeln(line)
+
+    def write_sim_option(self, opt: vsp.SimOptions) -> None:
+        # FIXME: make this just `Param` instead
+        raise NotImplementedError
+
+    def write_ac(self, an: vsp.AcInput) -> None:
+        """# Write an AC analysis."""
+        raise NotImplementedError
+
+    def write_dc(self, an: vsp.DcInput) -> None:
+        """# Write a DC analysis."""
+        raise NotImplementedError
+
+    def write_op(self, an: vsp.OpInput) -> None:
+        """# Write an operating point analysis."""
+        raise NotImplementedError
+
+    def write_tran(self, an: vsp.TranInput) -> None:
+        """# Write a transient analysis."""
+        raise NotImplementedError
+
+    def write_noise(self, an: vsp.NoiseInput) -> None:
+        """# Write a noise analysis."""
+        raise NotImplementedError
+
 
 class NgspiceNetlister(SpiceNetlister):
     """
     Ngspice-Format Netlister
     Should be identical to the base Spice netlister
     """
 
     @property
     def enum(self):
         """Get our entry in the `NetlistFormat` enumeration"""
         from . import NetlistFormat
 
         return NetlistFormat.NGSPICE
 
+    @classmethod
+    def format_sim_dut(cls, module_name: str) -> str:
+        """# Format the top-level DUT instance for module name `module_name`."""
+        return f"xtop 0 {module_name} // Top-Level DUT \n\n"
+
+    def write_include(self, inc: vsp.Include) -> None:
+        return self.writeln(f'.include "{inc.path}"')
+
+    def write_lib_include(self, lib: vsp.LibInclude) -> None:
+        txt = f'.lib "{lib.path}" {lib.section}'
+        return self.writeln(txt)
+
+    def write_save(self, save: vsp.Save) -> None:
+        # FIXME!
+        raise NotImplementedError(f"Unimplemented Save {save} for {self}")
+
+    def write_meas(self, meas: vsp.Meas) -> None:
+        txt = f".meas {meas.analysis_type} {meas.name} {meas.expr}"
+        return self.writeln(txt)
+
+    def write_sim_param(self, param: vlsir.Param) -> None:
+        txt = f".param {param.name}={self.get_param_value(param.value)}"
+        return self.writeln(txt)
+
+    def write_sim_option(self, opt: vsp.SimOptions) -> None:
+        # FIXME: make this just `Param` instead
+        return self.writeln(f".option {opt.name} = {self.get_param_value(opt.value)}\n")
+
+    def write_ac(self, an: vsp.AcInput) -> None:
+        """# Write an AC analysis."""
+
+        if not an.analysis_name:
+            raise RuntimeError(f"Analysis name required for {an}")
+        if len(an.ctrls):
+            raise NotImplementedError  # FIXME!
+
+        # Unpack the analysis / sweep content
+        fstart = an.fstart
+        if fstart <= 0:
+            raise ValueError(f"Invalid `fstart` {fstart}")
+        fstop = an.fstop
+        if fstop <= 0:
+            raise ValueError(f"Invalid `fstop` {fstop}")
+        npts = an.npts
+        if npts <= 0:
+            raise ValueError(f"Invalid `npts` {npts}")
+
+        # Write the analysis command
+        line = f".ac dec {npts} {fstart} {fstop}\n\n"
+        self.writeln(line)
+
+    def write_dc(self, an: vsp.DcInput) -> None:
+        """# Write a DC analysis."""
+
+        if not an.analysis_name:
+            raise RuntimeError(f"Analysis name required for {an}")
+        if len(an.ctrls):
+            raise NotImplementedError  # FIXME!
+
+        # Write the analysis command
+        param = an.indep_name
+        ## Interpret the sweep
+        sweep_type = an.sweep.WhichOneof("tp")
+        if sweep_type == "linear":
+            sweep = an.sweep.linear
+            line = (
+                f".dc param start={sweep.start} stop={sweep.stop} step={sweep.step}\n\n"
+            )
+            self.writeln(line)
+        elif sweep_type == "points":
+            raise ValueError("NG Spice does not support a DC point sweep")
+            sweep = an.sweep.points
+            line = f".dc values=[{sweep.points}]\n\n"
+            self.writeln(line)
+        elif sweep_type == "log":
+            raise NotImplementedError
+        else:
+            raise ValueError("Invalid sweep type")
+
+    def write_op(self, an: vsp.OpInput) -> None:
+        """# Write an operating point analysis."""
+
+        if not an.analysis_name:
+            raise RuntimeError(f"Analysis name required for {an}")
+        if len(an.ctrls):
+            raise NotImplementedError  # FIXME!
+
+        self.writeln(f".op\n")
+
+    def write_tran(self, an: vsp.TranInput) -> None:
+        """# Write a transient analysis."""
+        if not an.analysis_name:
+            raise RuntimeError(f"Analysis name required for {an}")
+        if len(an.ctrls):
+            raise NotImplementedError
+        if len(an.ic):
+            raise NotImplementedError
+
+        self.writeln(f".tran {an.tstep} {an.tstop}\n")
+
+    def write_noise(self, an: vsp.NoiseInput) -> None:
+        """# Write a noise analysis."""
+
+        if not an.analysis_name:
+            raise RuntimeError(f"Analysis name required for {an}")
+        if len(an.ctrls):
+            raise NotImplementedError
+
+        self.writeln(f".save all")
+
+        # NgSpice's syntax for a hierarchical reference to a net is (apparently) `v(v.<dot-separated-path>)`
+        # and similarly a source is `v.<dot-separated-path>`.
+        #
+        # In response to "where on earth did you find this?" @avi wrote:
+        # "this isn't really documented anywhere. I figured this out on a hunch from the syntax for saving transistor parameters, which is something like @m.path_to_transistor[param_name]"
+        #
+        if an.output_n:  # Differential output spec
+            noise_output = f"v(v.xtop.{an.output_p}, v.xtop.{an.output_n})"
+        else:
+            noise_output = f"v(v.xtop.{an.output_p})"
+
+        # NOTE: the `noise_input_source` being a *voltage* source is functionally encoded here,
+        # particularly by the "v" prepended to its name.
+        # Should we ever support current source noise inputs, we'll need to change this.
+        noise_input_source = f"v.xtop.v{an.input_source}"
+        noise_sweep = f"dec {an.npts} {an.fstart} {an.fstop}"
+        self.writeln(f".noise {noise_output} {noise_input_source} {noise_sweep}\n")
+
 
 class CdlNetlister(SpiceNetlister):
     """FIXME: CDL-Format Netlister"""
 
     def __init__(self, *_, **__):
         raise NotImplementedError
```

### Comparing `vlsirtools-3.0.dev3/vlsirtools/spice/base.py` & `vlsirtools-4.0.0rc0/vlsirtools/spice/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ 
 # Simulator State Base-Class 
 """
 
 # Std-Lib Imports
-import asyncio, os, tempfile
-from typing import Optional, Awaitable, List, IO
+import subprocess, os, tempfile
+from typing import Optional, List, IO
 from pathlib import Path
 
 # Local/ Project Dependencies
 import vlsir.spice_pb2 as vsp
 import vlsir.circuit_pb2 as vckt
 from . import SimResultUnion, SupportedSimulators, SimOptions, ResultFormat
 
@@ -38,108 +38,81 @@
     """
 
     @classmethod
     def enum(cls) -> SupportedSimulators:
         raise NotImplementedError
 
     @classmethod
-    async def sim(
+    def sim(
         cls, inp: vsp.SimInput, opts: Optional[SimOptions] = None
-    ) -> Awaitable[SimResultUnion]:
+    ) -> SimResultUnion:
         """Sim-invoking class method.
         Creates an instance of `cls` as a context manager, run in its simulation directory.
         This should be invoked by typical implementations of a free-standing `sim` function."""
 
         if opts is None:  # Create the default `SimOptions`
             opts = SimOptions(simulator=cls.enum())
 
         # Create the simulation-class instance, and execute its main `run` method
         sim = cls(inp=inp, opts=opts)
         try:
             sim.setup()
-            results = await sim.run()
+            results = sim.run()
         finally:
             sim.cleanup()
 
         # FIXME: we shouldn't need this `isinstance`; get Xyce to return `sd.SimResult` and decide whether to convert here
         if opts.fmt == ResultFormat.VLSIR_PROTO and not isinstance(
             results, vsp.SimResult
         ):
             return results.to_proto()
         return results
 
-    def run(self) -> Awaitable[SimResultUnion]:
+    def run(self) -> SimResultUnion:
         raise NotImplementedError("`Sim` subclasses must implement `run`")
 
     def __init__(self, inp: vsp.SimInput, opts: SimOptions) -> None:
         self.inp = inp
         self.opts = opts
         self.rundir = opts.rundir
         self.tmpdir: Optional[tempfile.TemporaryDirectory] = None
-        self.top: Optional[vckt.Module] = None
-        self.subprocesses: List[asyncio.Process] = []
+        self.subprocesses: List[subprocess.Process] = []
 
     def setup(self):
         """Perform simulation setup, including the simulation directory and top-level Module validation."""
 
         # Set up the simulation directory
         if self.rundir is not None:  # User-specified `rundir`
             self.tmpdir = None
             self.rundir = Path(self.rundir).absolute()
             if not self.rundir.exists():
                 os.makedirs(self.rundir)
         else:  # Create a new temp directory
             self.tmpdir = tempfile.TemporaryDirectory()
             self.rundir = Path(self.tmpdir.name).absolute()
 
-        # Ensure that we have a valid top-level module
-        self.validate_top()
-
     def cleanup(self):
         """On completion, clean up after ourselves."""
         if self.tmpdir is not None:
             self.tmpdir.cleanup()
 
-    def validate_top(self) -> None:
-        """Ensure that the `top` module exists,
-        and adheres to the "Spice top-level" port-interface: a single port for ground / VSS / node-zero.
-        Sets the `self.top` attribute when successful, or raises a `RuntimeError` when not."""
-
-        if not self.inp.top:
-            raise RuntimeError(f"No top-level module specified")
-
-        found = False
-        for module in self.inp.pkg.modules:
-            if module.name == self.inp.top:
-                found = True
-                self.top = module
-                if len(module.ports) != 1:
-                    msg = f"`vlsir.SimInput` top-level module {self.inp.top} must have *one* (VSS) port - has {len(module.ports)} ports [{module.ports}]"
-                    raise RuntimeError(msg)
-                break
-
-        if not found:
-            names = [m.name for m in self.inp.pkg.modules]
-            msg = f"Top-level module `{self.inp.top}` not found among Modules {names}"
-            raise RuntimeError(msg)
-
-    async def run_subprocess(self, cmd: str) -> Awaitable[None]:
-        """Asynchronously run a shell subprocess invoking command `cmd`.
+    def run_subprocess(self, cmd: str) -> None:
+        """Run a shell subprocess invoking command `cmd`.
         All subprocesses are run in `self.rundir`, and tracked in the list `self.subprocesses`."""
 
-        proc = await asyncio.create_subprocess_shell(
+        proc = subprocess.Popen(
             cmd,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
             cwd=str(self.rundir),
         )
         self.subprocesses.append(proc)
-        stdout, stderr = await proc.communicate()
+        stdout, stderr = proc.communicate()
 
-        # The async subprocess module does not raise Python exceptions: check the return code instead.
+        # The subprocess module does not raise Python exceptions: check the return code instead.
         if proc.returncode != 0:
             from . import SimError
 
             raise SimError(sim=self, stdout=stdout, stderr=stderr)
         return None
 
     def open(self, name: str, mode: str = "r") -> IO:
```

### Comparing `vlsirtools-3.0.dev3/vlsirtools/spice/sim_data.py` & `vlsirtools-4.0.0rc0/vlsirtools/spice/sim_data.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-3.0.dev3/vlsirtools/spice/spectre.py` & `vlsirtools-4.0.0rc0/vlsirtools/spice/xyce.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,441 +1,399 @@
 """
-Spectre Implementation of `vlsir.spice.Sim`
+Xyce Implementation of `vsp.Sim`
 """
 
 # Std-Lib Imports
-import subprocess, re, shutil, glob
+import subprocess, random, shutil
+import concurrent.futures
+from glob import glob
+from os import PathLike
+from typing import IO, Dict, Union
+import shlex
+
 import numpy as np
-from typing import Tuple, Any, Mapping, Optional, IO, Dict, Awaitable
-from dataclasses import dataclass
-from warnings import warn
-from enum import Enum
+import pandas as pd
 
 # Local/ Project Dependencies
 import vlsir.spice_pb2 as vsp
-from ..netlist import netlist
-from ..netlist.spectre import SpectreNetlister
+from ..netlist import XyceNetlister
 from .base import Sim
-from .sim_data import TranResult, OpResult, SimResult, AcResult, DcResult
-from .spice import (
-    SupportedSimulators,
-    sim,
-    sim_async,  # Not directly used here, but "re-exported"
+from .sim_data import (
+    TranResult,
+    OpResult,
+    SimResult,
+    AcResult,
+    DcResult,
+    AnalysisResult,
 )
+from .spice import SupportedSimulators, sim
+
 
 # Module-level configuration. Over-writeable by sufficiently motivated users.
-SPECTRE_EXECUTABLE = "spectre"  # The simulator executable invoked. If over-ridden, likely for sake of a specific path or version.
+XYCE_EXECUTABLE = "Xyce"  # The simulator executable invoked. If over-ridden, likely for sake of a specific path or version.
 
 
 def available() -> bool:
-    return SpectreSim.available()
+    return XyceSim.available()
 
 
-class SpectreSim(Sim):
+class XyceSim(Sim):
     """
-    State and execution logic for a Spectre-call to `vsp.Sim`.
+    State and execution logic for a Xyce-call to `vsp.Sim`.
+
+    Xyce can, in principle, run multiple analyses per process,
+    but seems to commonly confuse outputs or disallow saving them
+    from multiple analyses.
+
+    Execution therefore instead occurs one Xyce-process per analysis.
+    Results from each analysis-process are collated into a single `SimResult`.
     """
 
     @staticmethod
     def available() -> bool:
-        """Boolean indication of whether the current running environment includes the simulator executable."""
-        if shutil.which(SPECTRE_EXECUTABLE) is None:
+        """Boolean indication of whether the current running environment includes the simulator executable on its path."""
+
+        if shutil.which(XYCE_EXECUTABLE) is None:
             return False
         try:
             # And if it's set, check that we can get its version without croaking.
-            # This can often happen because of an inaccessible license server, or just a badly-linked installation.
             subprocess.run(
-                f"{SPECTRE_EXECUTABLE} -V",  # Yes, "version" gets a capital "V" for this program (ascii shrug)
+                f"{XYCE_EXECUTABLE} -v",  # Get the version,
                 shell=True,
                 check=True,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 timeout=10,
             )
         except Exception:
             # Indicate "not available" for any Exception. Usually this will be a `subprocess.CalledProcessError`.
             return False
         return True  # Otherwise, installation looks good.
 
     @classmethod
     def enum(cls) -> SupportedSimulators:
-        return SupportedSimulators.SPECTRE
+        return SupportedSimulators.XYCE
 
-    async def run(self) -> Awaitable[SimResult]:
+    def run(self) -> SimResult:
         """Run the specified `SimInput` in directory `self.rundir`, returning its results."""
 
-        netlist_file = self.open("netlist.scs", "w")
-        netlist_file.write("// Test Netlist \n\n")
-        netlist_file.write("simulator lang=spectre \n\n")
-        netlist_file.write("global 0\n\n")
-        netlist(pkg=self.inp.pkg, dest=netlist_file, fmt="spectre")
+        # Write the DUT netlist
+        self.write_dut_netlist()
+
+        # Run each analysis as a concurrent subprocess
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            an_results = list(executor.map(self.analysis, self.inp.an))
+        return SimResult(an_results)
+
+    def write_dut_netlist(self) -> None:
+        """# Write the DUT part (really, everything but Analyses) of the netlist.
+
+        Xyce is weird in that we can't reliably get multi-analysis sims to work,
+        so we write the DUT, copy it to a new file for each analysis, and then carry on modifying that.
+
+        This function largely parallels `Netlister.write_sim_input()`,
+        but skips the analysis-specific parts."""
+
+        netlist_file = self.open("dut", "w")
+        netlister = XyceNetlister(dest=netlist_file)
+
+        # Do our fake version of `write_sim_input`
+
+        # Write the header
+        netlister.write_sim_header(self.inp)
+
+        # Write the circuit-definitions package
+        netlister.write_package(pkg=self.inp.pkg)
 
         # Write the top-level instance
-        top_name = SpectreNetlister.get_module_name(self.top)
-        netlist_file.write(f"xtop 0 {top_name} // Top-Level DUT \n\n")
+        netlister.write_sim_dut(self.inp)
 
-        if self.inp.opts:
-            raise NotImplementedError(f"SimInput Options")
+        # Write sim options
+        netlister.write_sim_options(self.inp.opts)
 
         # Write each control element
-        self.write_control_elements(netlist_file)
+        netlister.write_control_elements(self.inp.ctrls)
 
-        # Write each analysis
-        for an in self.inp.an:
-            self.netlist_analysis(an, netlist_file)
-
-        netlist_file.flush()
-        netlist_file.close()
-
-        # Run the simulation
-        await self.run_spectre_process()
-
-        # Parse output data
-        data = parse_nutbin(self.open("netlist.raw", "rb"))
-        an_type_dispatch = dict(
-            ac=self.parse_ac, dc=self.parse_dc, op=self.parse_op, tran=self.parse_tran
-        )
-        results = []
-        for an in self.inp.an:
-            an_type = an.WhichOneof("an")
-            inner = getattr(an, an_type)
-            if an_type not in an_type_dispatch:
-                msg = f"Invalid or Unsupported analysis {an} with type {an_type}"
-                raise RuntimeError(msg)
-            func = an_type_dispatch[an_type]
-            if inner.analysis_name not in data:
-                msg = f"Cannot read results for analysis {an}"
-                raise RuntimeError(msg)
-            inner_data = data[inner.analysis_name]
-            an_results = func(inner, inner_data)
-            results.append(an_results)
-
-        return SimResult(an=results)
-
-    def write_control_elements(self, netlist_file: IO) -> None:
-        """Write control elements to the netlist"""
-        for ctrl in self.inp.ctrls:
-            inner = ctrl.WhichOneof("ctrl")
-            if inner == "include":
-                netlist_file.write(f'include "{ctrl.include.path}" \n')
-            elif inner == "lib":
-                txt = f'include "{ctrl.lib.path}" section={ctrl.lib.section} \n'
-                netlist_file.write(txt)
-            elif inner == "literal":
-                netlist_file.write(ctrl.literal + "\n")
-            elif inner == "param":
-                # txt = f"parameters {ctrl.param.name}={str(ctrl.param.value)} \n"
-                txt = f"parameters  {ctrl.param.name}={SpectreNetlister.get_param_value(ctrl.param.value)} \n"
-                netlist_file.write(txt)
-            elif inner == "meas":
-                # Measurements are written in Spice syntax; wrap them in "simulator lang".
-                netlist_file.write(f"simulator lang=spice \n")
-                txt = f".meas {ctrl.meas.analysis_type} {ctrl.meas.name} {ctrl.meas.expr} \n"
-                netlist_file.write(txt)
-                netlist_file.write(f"simulator lang=spectre \n")
-            elif inner in ("save"):
-                raise NotImplementedError(
-                    f"Unimplemented control card {ctrl} for {self}"
-                )  # FIXME!
-            else:
-                raise RuntimeError(f"Unknown control type: {inner}")
+        # Skip this part!
+        # # Write each analysis
+        # for an in self.inp.an:
+        #     netlister.write_analysis(an)
 
-    def netlist_analysis(self, an: vsp.Analysis, netlist_file: IO) -> None:
-        """Netlist an `Analysis`, largely dispatching its content to a type-specific method."""
+        # And ensure all output makes it to `self.dest`
+        netlister.flush()
 
+    def analysis(self, an: vsp.Analysis) -> AnalysisResult:
+        """Execute a `vsp.Analysis`, returning its `AnalysisResult`"""
+
+        # `Analysis` is a Union (protobuf `oneof`) of the analysis-types.
+        # Unwrap it, and dispatch based on the type.
         inner = an.WhichOneof("an")
-        inner_dispatch = dict(
-            ac=self.netlist_ac,
-            dc=self.netlist_dc,
-            op=self.netlist_op,
-            tran=self.netlist_tran,
-        )
-        inner_dispatch[inner](getattr(an, inner), netlist_file)
 
-    def netlist_ac(self, an: vsp.AcInput, netlist_file: IO) -> None:
+        if inner == "op":
+            return self.op(an.op)
+        if inner == "dc":
+            return self.dc(an.dc)
+        if inner == "ac":
+            return self.ac(an.ac)
+        if inner == "tran":
+            return self.tran(an.tran)
+        if inner in ("sweep", "monte", "custom"):
+            raise NotImplementedError(f"{inner} not implemented")
+        raise RuntimeError(f"Unknown analysis type: {inner}")
+
+    def ac(self, an: vsp.AcInput) -> vsp.AcResult:
         """Run an AC analysis."""
 
+        # Unpack the `AcInput`
         if not an.analysis_name:
             raise RuntimeError(f"Analysis name required for {an}")
+        analysis_name = an.analysis_name
         if len(an.ctrls):
             raise NotImplementedError  # FIXME!
 
-        # Unpack the analysis / sweep content
+        # Copy and append to the existing DUT netlist
+        netlist = self.copy_dut_netlist(f"{analysis_name}.sp")
+
+        # Write the analysis command
+        npts = an.npts
         fstart = an.fstart
-        if fstart <= 0:
-            raise ValueError(f"Invalid `fstart` {fstart}")
         fstop = an.fstop
-        if fstop <= 0:
-            raise ValueError(f"Invalid `fstop` {fstop}")
-        npts = an.npts
-        if npts <= 0:
-            raise ValueError(f"Invalid `npts` {npts}")
+        netlist.write(f".ac DEC {npts} {fstart} {fstop} \n\n")
 
-        # Write the analysis command
-        line = f"{an.analysis_name} ac start={fstart} stop={fstop} dec={npts}\n\n"
-        netlist_file.write(line)
+        # FIXME: always saving everything, no matter what
+        # Note `csv` output-formatting is encoded here
+        netlist.write(".print ac format=csv v(*) i(*) \n\n")
+
+        # And don't forget - the thing SPICE can't live without - END!
+        netlist.write(".end \n\n")
+        netlist.flush()
+
+        # Do the real work, running the simulation
+        self.run_xyce_process(analysis_name)
+
+        # Read the results from CSV
+        with self.open(f"{analysis_name}.sp.FD.csv", "r") as csv_handle:
+            csv_data = read_csv(csv_handle)
+
+        # Separate Frequency vector
+        freq: np.ndarray = csv_data.pop("FREQ")
+        data: Dict[str, np.ndarray] = {}
+
+        # Pull together separate real/imaginary parts into complex numbers
+        keys = list(csv_data.keys())
+        for re, im in zip(keys[::2], keys[1::2]):
+            # Check that node-names match, or fail.
+            # Peel out "Re(" and "Im(" from the beginning, and a trailing ")" from the end.
+            if re[3:-1] != im[3:-1]:
+                raise RuntimeError(f"Unmatched complex number: {re}, {im}")
+            name = re[3:-1]
+            data[name] = np.array(
+                [complex(r, i) for r, i in zip(csv_data[re], csv_data[im])]
+            )
 
-    def netlist_dc(self, an: vsp.DcInput, netlist_file: IO) -> None:
-        """Netlist a DC analysis."""
+        # Parse any scalar measurement results
+        measurements = self.parse_measurements(analysis_name)
 
+        # And arrange them in an `AcResult`
+        return AcResult(
+            analysis_name=an.analysis_name,
+            freq=freq,
+            data=data,
+            measurements=measurements,
+        )
+
+    def dc(self, an: vsp.DcInput) -> DcResult:
+        """Run a DC analysis."""
+
+        # Unpack the `DcInput`
         if not an.analysis_name:
             raise RuntimeError(f"Analysis name required for {an}")
+        analysis_name = an.analysis_name
         if len(an.ctrls):
             raise NotImplementedError  # FIXME!
 
+        # Copy and append to the existing DUT netlist
+        netlist = self.copy_dut_netlist(f"{analysis_name}.sp")
+
         # Write the analysis command
         param = an.indep_name
         ## Interpret the sweep
         sweep_type = an.sweep.WhichOneof("tp")
         if sweep_type == "linear":
             sweep = an.sweep.linear
-            line = f"{an.analysis_name} dc param={param} start={sweep.start} stop={sweep.stop} step={sweep.step}\n\n"
-            netlist_file.write(line)
+            netlist.write(
+                f".dc LIN {param} {sweep.start} {sweep.stop} {sweep.step}\n\n"
+            )
+        elif sweep_type == "log":
+            sweep = an.sweep.log
+            netlist.write(
+                f".dc DEC {param} {sweep.start} {sweep.stop} {sweep.npts}\n\n"
+            )
         elif sweep_type == "points":
             sweep = an.sweep.points
-            line = f"{an.analysis_name} dc values=[{sweep.points}]\n\n"
-            netlist_file.write(line)
-        elif sweep_type == "log":
-            raise NotImplementedError
+            netlist.write(
+                f".dc {param} LIST {' '.join([str(pt) for pt in sweep.points])}\n\n"
+            )
         else:
             raise ValueError("Invalid sweep type")
 
-    def netlist_op(self, an: vsp.OpInput, netlist_file: IO) -> None:
-        """Netlist a single point DC analysis"""
+        # FIXME: always saving everything, no matter what
+        # Note `csv` output-formatting is encoded here
+        netlist.write(".print dc format=csv v(*) i(*) \n\n")
 
-        if not an.analysis_name:
-            raise RuntimeError(f"Analysis name required for {an}")
-        if len(an.ctrls):
-            raise NotImplementedError  # FIXME!
+        # And don't forget - the thing SPICE can't live without - END!
+        netlist.write(".end \n\n")
+        netlist.flush()
 
-        netlist_file.write(f"{an.analysis_name} dc oppoint=rawfile\n\n")
+        # Do the real work, running the simulation
+        self.run_xyce_process(analysis_name)
 
-    def netlist_tran(self, an: vsp.TranInput, netlist_file: IO) -> None:
-        if not an.analysis_name:
-            raise RuntimeError(f"Analysis name required for {an}")
-        if len(an.ctrls):
-            raise NotImplementedError
-        if len(an.ic):
-            raise NotImplementedError
-
-        netlist_file.write(f"{an.analysis_name} tran stop={an.tstop} \n\n")
+        # Read the results from CSV
+        with self.open(f"{analysis_name}.sp.csv", "r") as csv_handle:
+            csv_data = read_csv(csv_handle)
 
-    def parse_ac(self, an: vsp.AcInput, nutbin: "NutBinAnalysis") -> AcResult:
-        # FIXME: the `mt0` and friends file names collide with tran, if they are used in the same Sim!
-        measurements = self.get_measurements("*.mt*")
-
-        # Pop the frequence vector out of the data
-        freq = nutbin.data.pop("freq")
-        # Nutbin format stores the frequency vector as complex numbers, along with all the complex-valued signal data.
-        # Grab the real parts of the frequencies, and ensure that they don't (somehow) have nonzero imaginary parts.
-        if np.any(freq.imag):
-            raise RuntimeError(f"Imaginary parts of frequencies in {freq}")
-        freq = freq.real
+        # Parse any scalar measurement results
+        measurements = self.parse_measurements(analysis_name)
 
-        return AcResult(
-            analysis_name=an.analysis_name,
-            freq=freq,
-            data=nutbin.data,
-            measurements=measurements,
-        )
-
-    def parse_dc(self, an: vsp.DcInput, nutbin: "NutBinAnalysis") -> DcResult:
-        measurements = self.get_measurements("*.ms*")
+        # And arrange them in an `OpResult`
         return DcResult(
             analysis_name=an.analysis_name,
             indep_name=an.indep_name,
-            data=nutbin.data,
+            data=csv_data,
             measurements=measurements,
         )
 
-    def parse_op(self, an: vsp.OpInput, nutbin: "NutBinAnalysis") -> OpResult:
-        return OpResult(
-            analysis_name=an.analysis_name,
-            data={k: v[0] for k, v in nutbin.data.items()},
-        )
-
-    def parse_tran(self, an: vsp.TranInput, nutbin: "NutBinAnalysis") -> TranResult:
-        """Extract the results for Analysis `an` from `data`."""
-        measurements = self.get_measurements("*.mt*")
-        return TranResult(
-            analysis_name=an.analysis_name, data=nutbin.data, measurements=measurements
-        )
+    def op(self, an: vsp.OpInput) -> OpResult:
+        """Run an operating-point analysis.
+        Xyce describes the `.op` analysis as "partially supported".
+        Here the `vsp.Op` analysis is mapped to DC, with a dummy sweep."""
 
-    def get_measurements(self, filepat: str) -> Dict[str, float]:
-        """Get the measurements at files matching (glob) `filepat`.
-        Returns only a single files-worth of measurements, and issues a warning if more than one such file exists.
-        Returns an empty dictionary if no matching files are found."""
-        meas_files = list(self.glob(filepat))
-        if not meas_files:
-            return dict()
-        if len(meas_files) > 1:
-            msg = f"Unsupported: more than one measurement-file generated. Only the first will be read"
-            warn(msg)
-        return parse_mt0(self.open(meas_files[0], "r"))
-
-    def run_spectre_process(self) -> Awaitable[None]:
-        """Run a Spectre sub-process, executing the simulation"""
-        # Note the `nutbin` output format is dictated here
-        cmd = f"{SPECTRE_EXECUTABLE} -E -format nutbin netlist.scs"
-        return self.run_subprocess(cmd)
+        # Unpack the `OpInput`
+        if not an.analysis_name:
+            raise RuntimeError(f"Analysis name required for {an}")
+        analysis_name = an.analysis_name
+        if len(an.ctrls):
+            raise NotImplementedError  # FIXME!
 
+        # Copy and append to the existing DUT netlist
+        netlist = self.copy_dut_netlist(f"{analysis_name}.sp")
 
-class FromStr:
-    """Mix-in for creating `Enum`s from string values."""
+        # Create the dummy parameter, and "sweep" a single value of it
+        dummy_param = f"_dummy_{random.randint(0,65536)}_"
+        netlist.write(f".param {dummy_param}=1 \n\n")
 
-    @classmethod
-    def from_str(cls, s: str) -> "FromStr":
-        reversed = {v.value: v for v in cls}
-        if s not in reversed:
-            msg = f"Invalid `{cls.__name__}`: `{s}`"
-            raise ValueError(msg)
-        return reversed[s]
+        # Write the analysis command
+        netlist.write(f".dc {dummy_param} 1 1 1 \n\n")
 
+        # FIXME: always saving everything, no matter what
+        # Note `csv` output-formatting is encoded here
+        netlist.write(".print dc format=csv v(*) i(*) \n\n")
 
-class NumType(FromStr, Enum):
-    """# Numeric Datatypes
-    Values equal the strings used in NutBin data files."""
+        # And don't forget - the thing SPICE can't live without - END!
+        netlist.write(".end \n\n")
+        netlist.flush()
 
-    REAL = "real"
-    COMPLEX = "complex"
+        # Do the real work, running the simulation
+        self.run_xyce_process(analysis_name)
 
+        # Read the results from CSV
+        with self.open(f"{analysis_name}.sp.csv", "r") as csv_handle:
+            csv_data = read_csv(csv_handle)
 
-class Units(FromStr, Enum):
-    """# Unit Types
-    Values equal the strings used in NutBin data files."""
+        # Each value in `csv_data` will be a single-element list.
+        # Pull those single elements out.
+        data = {k: v[0] for k, v in csv_data.items()}
 
-    DUMMY = "dummy"
-    SWEEP = "sweep"
-    SECONDS = "s"
-    VOLTS = "V"
-    AMPS = "A"
-    HERTZ = "Hz"
-    CELSIUS = "C"
+        # And arrange them in an `OpResult`
+        return OpResult(
+            analysis_name=an.analysis_name,
+            data=data,
+        )
 
+    def tran(self, an: vsp.TranInput) -> vsp.TranResult:
+        """Run a transient analysis."""
 
-@dataclass
-class VarSpec:
-    """Variable Spec"""
+        # Extract fields from our `TranInput`
+        if not an.analysis_name:
+            raise RuntimeError(f"Analysis name required for {an}")
+        analysis_name = an.analysis_name
 
-    name: str
-    units: Units
+        # Why not make tstop/tstep required?
+        if not an.tstop or not an.tstep:
+            raise ValueError("tstop and tstep must be defined")
+        tstop = an.tstop
+        tstep = an.tstep
+        if len(an.ic):
+            raise NotImplementedError
+        if len(an.ctrls):
+            raise NotImplementedError
 
+        # Copy and append to the existing DUT netlist
+        netlist = self.copy_dut_netlist(f"{analysis_name}.sp")
 
-@dataclass
-class NutBinAnalysis:
-    """Analysis result from a NutBin file."""
+        # Write the analysis command
+        netlist.write(f".tran {tstep} {tstop} \n\n")
 
-    analysis_name: str  # Analysis name
-    numtype: NumType  # Numeric type in `data` field
-    data: Mapping[str, np.ndarray]  # Signal name => data
-    units: Mapping[str, Units]  # Signal name => units
+        # FIXME: always saving everything, no matter what
+        # Note `csv` output-formatting is encoded here
+        netlist.write(".print tran format=csv v(*) i(*) \n\n")
 
+        # And don't forget - the thing SPICE can't live without - END!
+        netlist.write(".end \n\n")
+        netlist.flush()
 
-def parse_nutbin(f: IO) -> Mapping[str, NutBinAnalysis]:
-    """Parse a `nutbin` format set of simulation results.
-    Returns results as a dictionary from `analysis_name` to `NutBinAnalysis`.
-    Note this is paired with the simulator invocation commands, which include `format=nutbin`."""
+        # Do the real work, running the simulation
+        self.run_xyce_process(analysis_name)
 
-    # Parse per-file header info
-    # First 2 lines are ascii one line statements
-    _title = f.readline()  # Title, ignored
-    _date = f.readline()  # Run date, ignored
+        # Parse and organize our results
+        # First pull them in from CSV
+        with self.open(f"{analysis_name}.sp.csv", "r") as csv_handle:
+            csv_data = read_csv(csv_handle)
 
-    # And parse the rest of the file per-analysis
-    rv = {}
-    while f:
-        plotname = f.readline().decode("ascii")  # Simulation name
-        if len(plotname) == 0:
-            break
-        an = parse_nutbin_analysis(f, plotname)
-        rv[an.analysis_name] = an
-    return rv
+        # Parse any scalar measurement results
+        measurements = self.parse_measurements(analysis_name)
 
+        # And organize them into a `TranResult`
+        return TranResult(
+            analysis_name=an.analysis_name, data=csv_data, measurements=measurements
+        )
 
-def parse_nutbin_analysis(f: IO, plotname: str) -> NutBinAnalysis:
-    """Parse a `NutBinAnalysis` from an open nutbin-format file `f`."""
+    def run_xyce_process(self, name: str) -> None:
+        """Run a `Xyce` sub-process executing the simulation."""
+        return self.run_subprocess(cmd=shlex.split(f"{XYCE_EXECUTABLE} {name}.sp"))
+
+    def parse_measurements(self, analysis_name: str) -> Dict[str, float]:
+        # FIXME: the *input* should really be dictating whether we have measurements.
+        # For now, we just search for any matching filenames via `glob`
+        meas_glob = glob(f"*{analysis_name}*.m*0")
+        if len(meas_glob) > 1:
+            raise RuntimeError(f"Unsupported multiple measurement results for {self}")
+        if len(meas_glob) == 1:
+            measurements = parse_meas(self.open(meas_glob[0], "r"))
+            return {k.lower(): v for k, v in measurements.items()}
+        # No measurement-file, return an empty result
+        return {}
+
+    def copy_dut_netlist(self, path: str) -> IO:
+        """Copy the `DUT` part of the netlist to file `path`,
+        in our working directory, and return a file-handle to it."""
+        shutil.copy(self.path("dut"), self.path(path))
+        return self.open(path, "a")
+
+
+def read_csv(handle: Union[IO, PathLike]) -> Dict[str, np.ndarray]:
+    """Read CSV from file-handle `handle` into a dictionary of {header: array}s."""
 
-    # Next 4 lines are also ascii one line statements
-    # Parse the `Flags` field, which primarily includes the numeric datatype
-    flags = f.readline().decode("ascii")
-    flags = flags.split()
-    if len(flags) != 2 or flags[0] != "Flags:":
-        raise ValueError(f"Invalid flags {flags}")
-    numtype = NumType.from_str(flags[1])
-    nptypes = {NumType.REAL: float, NumType.COMPLEX: complex}
-    nptype = nptypes[numtype]
-
-    # Parse the number of variables and points
-    num_vars_line = f.readline()  # No. Variables:   [nvar]
-    num_pts_line = f.readline()  # No. Points:      [npts]
-    sim_name = plotname.split("`")[-1].split("'")[0]
-
-    # Find the number of variables and number of points
-    num_vars = int(
-        re.match(
-            r"No. Variables:\s+(?P<num_vars>\d+)\n",
-            num_vars_line.decode("ascii"),
-        ).group("num_vars")
-    )
-    num_pts = int(
-        re.match(
-            r"No. Points:\s+(?P<num_pts>\d+)\n",
-            num_pts_line.decode("ascii"),
-        ).group("num_pts")
-    )
-
-    # Decode the variables spec, looks like the following
-    # Variables: [Variable idx] [Variable name] [units] [optional_flags]
-    var_line = f.readline().decode("ascii")
-    var_specs = [_read_var_spec(var_line[10:])]
-    for i in range(num_vars - 1):
-        var_specs.append(_read_var_spec(f.readline().decode("ascii")))
-
-    # Read the binary data, should look like the following:
-    # Binary: \n[Binary data]
-    binary_line = f.readline().decode("ascii")
-    assert binary_line == "Binary:\n"
-    # Data is big endian
-    bin_data = np.fromfile(
-        f, dtype=np.dtype(nptype).newbyteorder(">"), count=num_vars * num_pts
-    )
-    data = {}
-    units = {}
-    for i, var in enumerate(var_specs):
-        data[var.name] = bin_data[i::num_vars]
-        units[var.name] = var.units
-
-    return NutBinAnalysis(
-        analysis_name=sim_name,
-        numtype=numtype,
-        data=data,
-        units=units,
-    )
-
-
-def _read_var_spec(line: str) -> VarSpec:
-    """Read a Variable spec line from the input
-    and return the name and the units."""
-    m = re.match(
-        r"\s+(?P<idx>\d+)\s+(?P<name>\S+)\s+(?P<units>\S+)(?P<rest>.*)\n", line
-    )
-    return VarSpec(name=m.group("name"), units=Units.from_str(m.group("units")))
-
-
-def parse_mt0(file: IO) -> Dict[str, float]:
-    """Parse an (open) "mt0-format" measurement-file into a set of {name: value} pairs."""
-
-    file.readline()  # Header
-    file.readline()  # Netlist Title
-    keys = file.readline()  # Measurement Names Line
-    keys = keys.split()
-    values = file.readline()  # Measurement Values Line
+    df = pd.read_csv(handle)
+    return {n: np.array(c) for n, c in df.items()}
 
-    def convert(s: str) -> float:
-        """Convert a string to a float, converting failing cases to `NaN`"""
-        try:
-            return float(s)
-        except:
-            return float("NaN")
 
-    values = [convert(s) for s in values.split()]
-    return dict(zip(keys, values))
+def parse_meas(file: IO) -> Dict[str, float]:
+    """Parse an (open) measurement-file to a {name: value} dictionary."""
+    rv = {}
+    for line in file.readlines():
+        contents = line.split()
+        if len(contents) != 3 or contents[1] != "=":
+            raise RuntimeError(f"Invalid line in Xyce measurements: {line}")
+        name, val = contents[0], float(contents[2])
+        rv[name] = val
+    return rv
```

### Comparing `vlsirtools-3.0.dev3/vlsirtools/spice/spice.py` & `vlsirtools-4.0.0rc0/vlsirtools/pytest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,166 +1,196 @@
-""" 
-# Spice-Class Simulator Interface 
 """
+# VlsirTools Pytest Utilities 
 
-# Std-Lib Imports
-import asyncio, os, subprocess
-from typing import Union, Optional, Sequence, Awaitable, TypeVar
-from enum import Enum
-from textwrap import dedent
-from dataclasses import dataclass, field
+Primarily adds and parses the command-line options for enabling and disabling `vlsirtools.spice` simulators. 
+To use these utilities, add the following to your `conftest.py`:
 
-# Local/ Project Dependencies
-import vlsir.spice_pb2 as vsp
-from vlsir.spice_pb2 import *  # Not used here intentionally, but "re-exported"
-from . import sim_data as sd
+```python
+from vlsirtools.pytest import (
+    pytest_configure,
+    pytest_addoption,
+    pytest_collection_modifyitems,
+)
+```
+
+See VlsirTools' own `conftest.py` for an example.  
+With these functions included, by those names, in `conftest.py`, invocations of `pytest` can use: 
+
+* The `--simulator_test_mode` command-line option 
+  * Values are `required`, `if_available`, or `disabled`
+* Markers for each supported simulator
+  * `spectre`, `xyce`, and `ngspice` are currently supported
+* Command-line options for each supported simulator, to override `simulator_test_mode`
+
+
+Examples: 
+
+```
+pytest --simulator_test_mode disabled       # Disables all simulation tests
+pytest --simulator_test_mode required       # Requires all simulation tests
+pytest --simulator_test_mode if_available   # Runs tests on available simulators
+
+pytest --simulator_test_mode if_available --ngspice required  # Requires ngspice, tests all others available 
+pytest --simulator_test_mode required --xyce disabled         # Disables xyce, requires all others
+pytest --simulator_test_mode disabled --spectre required      # Requires spectre, disables all others
+```
 
+"""
 
-class ResultFormat(Enum):
-    """Enumerated Result Formats"""
 
-    SIM_DATA = "sim_data"  # Types defined in the `sim_data` module
-    VLSIR_PROTO = "vlsir_proto"  # `vsp.SimResults` and related protobuf-defined types
+import pytest
+from enum import Enum
+from typing import Dict, Optional
+from dataclasses import dataclass
 
+import vlsirtools.spice as vsp
 
-# Union of the two result-types, returned by many simulation methods
-SimResultUnion = Union[vsp.SimResult, sd.SimResult]
 
+class SimulatorTestMode(Enum):
+    """# Enumerated Per-Simulator Test Modes"""
 
-class SupportedSimulators(Enum):
-    """Enumerated, Internally-Defined Spice-Class Simulators"""
+    REQUIRED = "required"
+    IF_AVAILABLE = "if_available"
+    DISABLED = "disabled"
 
-    SPECTRE = "spectre"
-    XYCE = "xyce"
-    NGSPICE = "ngspice"
+    def skip(self) -> bool:
+        """Boolean indication of whether this Simulator should be skipped."""
+        return self.value == "disabled"
 
 
-def default() -> Optional[SupportedSimulators]:
-    """Get the default simulator, for this Python-process and its environment.
-    This largely consists of a priority-ordered walk through `SupportedSimulators`,
-    returning the first whose `available()` method indicates its availability.
-    Returns `None` if no such simulator appears available."""
+@dataclass
+class Simulator:
+    marker: str
+    # Simulator name/ command-line option/ pytest-marker name
+    available: bool
+    # Boolean indicator of availability in the current environment
+
+    def getoption(self, config: "Config") -> Optional["SimulatorTestMode"]:
+        """Get this simulator's pytest option"""
+        option = config.getoption(f"--{self.marker}")
+        if option is None:
+            return None
+        return SimulatorTestMode(option)
+
+
+# The "registry" of supported simulators and their availability in the current process environment
+# In other words, the stuff about the simulators that we know before we start running tests
+simulators: Dict[str, Simulator] = {
+    s.marker: s
+    for s in [
+        Simulator(marker="spectre", available=vsp.spectre.available()),
+        Simulator(marker="xyce", available=vsp.xyce.available()),
+        Simulator(marker="ngspice", available=vsp.ngspice.available()),
+    ]
+}
+
+
+class Why(Enum):
+    """# Enumerated reasons to be enabled or disabled."""
+
+    DISABLED = "DISABLED"
+    NOT_AVAILABLE = "NOT_AVAILABLE"
+    AVAILABLE = "AVAILABLE"
+    REQUIRED = "REQUIRED"
+
+    def enabled(self) -> bool:
+        """# Boolean enabledness indicator"""
+        if self in (Why.DISABLED, Why.NOT_AVAILABLE):
+            return False
+        if self in (Why.REQUIRED, Why.AVAILABLE):
+            return True
+        raise ValueError(f"Unknown Why: {self}")
 
-    from .spectre import available as spectre_available
-    from .xyce import available as xyce_available
-    from .ngspice import available as ngspice_available
 
-    if spectre_available():
-        return SupportedSimulators.SPECTRE
-    if xyce_available():
-        return SupportedSimulators.XYCE
-    if ngspice_available():
-        return SupportedSimulators.NGSPICE
-    return None  # Nothing found
+@dataclass
+class SimulatorSettingPair:
+    """# Simulator-Setting Pair
+    The combination of a `Simulator` and its current test-setting."""
+
+    simulator: Simulator  # The simulator
+    mode: SimulatorTestMode  # Configured test mode
+    enabled: bool  # Boolean indicator of whether this simulator is enabled
+    why: Why  # Why this simulator is enabled or disabled
+
+    @staticmethod
+    def new(simulator: Simulator, mode: SimulatorTestMode) -> "SimulatorSettingPair":
+        """# Create a SimulatorSettingPair from a Simulator and a test mode."""
+
+        # Mostly suss out the reason "why"
+        if mode == SimulatorTestMode.DISABLED:
+            why = Why.DISABLED
+        elif mode == SimulatorTestMode.IF_AVAILABLE:
+            why = Why.AVAILABLE if simulator.available else Why.NOT_AVAILABLE
+        elif mode == SimulatorTestMode.REQUIRED:
+            why = Why.REQUIRED
+        else:
+            raise ValueError(f"Unknown mode: {mode}")
+
+        return SimulatorSettingPair(
+            simulator=simulator,
+            mode=mode,
+            enabled=why.enabled(),
+            why=why,
+        )
 
 
-@dataclass
-class SimOptions:
-    """Options to `vsp.Sim` which are *not* passed along to the simulator.
-    I.e. options which effect the Python-process invoking simulation,
-    but not the internals of the simulation itself."""
-
-    # Simulator. FIXME: debatable whether to include this.
-    simulator: SupportedSimulators = field(default_factory=default)
-
-    # In-memory results format
-    fmt: ResultFormat = ResultFormat.VLSIR_PROTO
-
-    # Simulation run-directory. Uses a `tempdir` if unspecified.
-    rundir: Optional[os.PathLike] = None
-
-
-# Shorthand type alias for "an element or list thereof", used by all the call signatures below
-T = TypeVar("T")
-OneOrMore = Union[T, Sequence[T]]
-
-
-def sim(
-    inp: OneOrMore[vsp.SimInput], opts: Optional[SimOptions] = None
-) -> OneOrMore[SimResultUnion]:
-    """
-    Execute one or more `vlir.spice.Sim`.
-    Dispatches across `SupportedSimulators` specified in `SimOptions` `opts`.
-    Uses the default `Simulator` as detected by the `default` method if no `simulator` is specified.
-    """
-    return asyncio.run(sim_async(inp, opts))
-
-
-async def sim_async(
-    inp: OneOrMore[vsp.SimInput], opts: Optional[SimOptions] = None
-) -> Awaitable[OneOrMore[SimResultUnion]]:
-    """
-    Asynchronously execute one or more `vlir.spice.Sim`.
-    Dispatches across `SupportedSimulators` specified in `SimOptions` `opts`.
-    Uses the default `Simulator` as detected by the `default` method if no `simulator` is specified.
-    """
-    from .xyce import XyceSim
-    from .spectre import SpectreSim
-    from .ngspice import NGSpiceSim
-
-    # Sort out the difference between "One" "OrMore" cases of input
-    # For a single `SimInput`, create a list, but note we only want to return a single `SimResult`
-    inp_is_a_single_sim = False
-    if not isinstance(inp, Sequence):
-        inp = [inp]
-        inp_is_a_single_sim = True
-    for x in inp:
-        if not isinstance(x, vsp.SimInput):
-            raise TypeError(f"Expected `vsp.SimInput`, got {x}")
-
-    if opts is None:  # Create the default `SimOptions`
-        opts = SimOptions()
-
-    if opts.simulator is None:  # If we didn't specify or find a simulator, fail.
-        msg = f"vlsirtools.spice: No Supported Simulators available for call to `sim()`"
-        raise RuntimeError(msg)
-
-    # Get the per-simulator callable
-    if opts.simulator == SupportedSimulators.XYCE:
-        cls = XyceSim
-    elif opts.simulator == SupportedSimulators.SPECTRE:
-        cls = SpectreSim
-    elif opts.simulator == SupportedSimulators.NGSPICE:
-        cls = NGSpiceSim
-    else:
-        raise ValueError(f"Unsupported simulator: {opts.simulator}")
-
-    if len(inp) > 1 and opts.rundir is not None:
-        # FIXME: how to ultimately handle this "multi-inputs plus specified directory" case
-        raise RuntimeError("Cannot specify a run-directory for multiple simulations")
-
-    # And do the real work, invoking the target simulator
-    futures = [cls.sim(i, opts) for i in inp]
-    results = await asyncio.gather(*futures)
-
-    # For the sequence of inputs case, return the sequence of results that came back
-    if not inp_is_a_single_sim:
-        return results
-
-    # Unpack the single-input case
-    if len(results) != 1:
-        raise RuntimeError("Expected a single result")
-    return results[0]
-
-
-class SimError(Exception):
-    """Exception raised when a simulation fails."""
-
-    def __init__(self, sim: "Sim", stdout: bytes, stderr: bytes) -> None:
-        s = dedent(
-            f"""
-            rundir: {str(sim.rundir)}
-            stdout: {str(stdout)}
-            stderr: {str(stderr)}
-        """
+def pytest_configure(config):
+    """# PyTest Configuration
+    Adds a marker for each supported simulator."""
+
+    for s in simulators.keys():
+        config.addinivalue_line("markers", f"{s}")
+
+
+def pytest_addoption(parser):
+    """PyTest Command-Line Option Additions"""
+
+    # Add the `--simulator_test_mode` option
+    parser.addoption(
+        "--simulator_test_mode",
+        action="store",
+        default=SimulatorTestMode.IF_AVAILABLE.value,
+        help=f"Simulation test mode. One of {[m.value for m in SimulatorTestMode]}.",
+    )
+    # Add an option for each supported simulator
+    for s in simulators.keys():
+        parser.addoption(
+            f"--{s}",
+            action="store",
+            default=None,
+            help=f"{s.title()} test mode. One of {[m.value for m in SimulatorTestMode]}.",
         )
-        super().__init__(s)
-        self.rundir = sim.rundir
-        self.stdout = stdout
-        self.stderr = stderr
 
 
-class SimProcessError(SimError):
-    """Exception raised when an external simulator process fails."""
+# Skip markers
+skip_disabled = pytest.mark.skip(reason="Disabled by command-line simulator options")
+skip_not_available = pytest.mark.skip(
+    reason="Simulator not available & not required by command-line options"
+)
+
+
+def pytest_collection_modifyitems(config, items):
+    """Examine each test item, and skip them based on `SimulatorSettings`."""
+
+    # First grab the "overall mode"
+    default_mode = SimulatorTestMode(config.getoption("--simulator_test_mode"))
+
+    # Now check for any simulator-specific overrides, and turn them into setting-pairs
+    simulator_settings = {
+        s.marker: SimulatorSettingPair.new(
+            simulator=s, mode=s.getoption(config) or default_mode
+        )
+        for s in simulators.values()
+    }
+
+    # print(f"Testing with simulation settings:")
+    # print(simulator_settings)
 
-    def __init__(self, sim: "Sim", e: subprocess.CalledProcessError) -> None:
-        super().__init__(sim=sim, stdout=e.stdout, stderr=e.stderr)
+    # Alright finally the point: apply the `skip` attribute to test we don't wanna run.
+    for item in items:
+        for marker in simulators.keys():
+            if marker in item.keywords:
+                pair = simulator_settings[marker]
+                if pair.why == Why.DISABLED:
+                    item.add_marker(skip_disabled)
+                elif pair.why == Why.NOT_AVAILABLE:
+                    item.add_marker(skip_not_available)
```

### Comparing `vlsirtools-3.0.dev3/vlsirtools.egg-info/PKG-INFO` & `vlsirtools-4.0.0rc0/readme.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: vlsirtools
-Version: 3.0.dev3
-Summary: Tools for the Vlsir IC Design Schema
-Home-page: https://github.com/Vlsir/Vlsir
-Author: Dan Fritchman
-Author-email: dan@fritch.mn
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 
 # Vlsir Tools 
 
 Python-based tools and utilites for working with the Vlsir IC design schema. 
 
 ## Netlisting 
 
@@ -28,47 +16,34 @@
     """Enumerated, Internally-Defined Spice-Class Simulators"""
 
     SPECTRE = "spectre"
     XYCE = "xyce"
     NGSPICE = "ngspice"
 ```
 
-The primary entry-point for simulation is `vlsirtools.spice.sim`. 
+The primary entry-point for simulation is `vlsirtools.spice.sim`. By default, `sim` runs your chosen simulator in parallel over the list of `SimInputs` provided as `inp`.
 
 ```python
 def sim(
     inp: OneOrMore[vsp.SimInput], opts: Optional[SimOptions] = None
 ) -> OneOrMore[SimResultUnion]:
 ```
 
 The `sim` function takes as input one or more `vlsir.spice.SimInput`s and a set of simulation options (`vlsirtools.spice.SimOptions`), and returns one of two result-types depending on its input `options`.
 
-
 ```python
 class ResultFormat(Enum):
     """Enumerated Result Formats"""
 
     SIM_DATA = "sim_data" 
     VLSIR_PROTO = "vlsir_proto" 
 ```
 
 The `VLSIR_PROTO` result-format returns a `vlsir.spice.SimResult` object, which is a protobuf-encoded representation of the simulation results. The `SIM_DATA` format instead uses the types defined in `vlsirtools.spice.sim_data`, a python-native combination of dataclasses and numpy arrays. The former is generally more convenient for sharing with other programs, and the latter for further in-Python processing. 
 
-Simulations can be invoked asynchronously by instead invoking `vlsirtools.spice.sim_async`. 
-Its interface is identical to `vlsirtools.spice.sim`, but for returning an `Awaitable`. 
-
-```python
-async def sim_async(
-    inp: OneOrMore[vsp.SimInput], opts: Optional[SimOptions] = None
-) -> Awaitable[OneOrMore[SimResultUnion]]:
-```
-
-Asynchronously invoking simulation is particularly valuable for large batches of simulations, 
-e.g. for "corner" or other parametric variations, as the simulator invocations can be run in parallel.
-
 ### Simulator and Analysis Support
 
 Each spice-class simulator includes its own netlist syntax and opinions about the specification for analyses. 
 The `vlsir.spice` schema  
 
 | Analysis             | Spectre            | Xyce               | NgSpice     |
 | -------------------- | ------------------ | ------------------ | ------------------ |
```

### Comparing `vlsirtools-3.0.dev3/vlsirtools.egg-info/SOURCES.txt` & `vlsirtools-4.0.0rc0/vlsirtools.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 .gitignore
 LICENSE
 readme.md
 setup.py
 tests/__init__.py
+tests/test_primitives.py
 tests/test_vlsirtools.py
 vlsirtools/__init__.py
+vlsirtools/primitives.py
+vlsirtools/pytest.py
+vlsirtools/spicetype.py
 vlsirtools.egg-info/PKG-INFO
 vlsirtools.egg-info/SOURCES.txt
 vlsirtools.egg-info/dependency_links.txt
 vlsirtools.egg-info/requires.txt
 vlsirtools.egg-info/top_level.txt
 vlsirtools/netlist/__init__.py
 vlsirtools/netlist/base.py
```

