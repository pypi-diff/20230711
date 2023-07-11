# Comparing `tmp/watts-0.5.0.tar.gz` & `tmp/watts-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watts-0.5.0.tar", last modified: Fri Feb 10 16:05:28 2023, max compression
+gzip compressed data, was "watts-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `watts-0.5.0.tar` & `watts-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-02-10 16:05:16.151578 watts-0.5.0/LICENSE
--rw-r--r--   0        0        0     2001 2023-02-10 16:05:16.151578 watts-0.5.0/README.md
--rw-r--r--   0        0        0     1496 2023-02-10 16:05:16.159578 watts-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      595 2023-02-10 16:05:16.159578 watts-0.5.0/src/watts/__init__.py
--rw-r--r--   0        0        0     3589 2023-02-10 16:05:16.159578 watts-0.5.0/src/watts/console.py
--rw-r--r--   0        0        0     4528 2023-02-10 16:05:16.159578 watts-0.5.0/src/watts/database.py
--rw-r--r--   0        0        0     3667 2023-02-10 16:05:16.159578 watts-0.5.0/src/watts/fileutils.py
--rw-r--r--   0        0        0     8579 2023-02-10 16:05:16.159578 watts-0.5.0/src/watts/parameters.py
--rw-r--r--   0        0        0    10189 2023-02-10 16:05:16.159578 watts-0.5.0/src/watts/plugin.py
--rw-r--r--   0        0        0     2214 2023-02-10 16:05:16.159578 watts-0.5.0/src/watts/plugin_abce.py
--rw-r--r--   0        0        0     2821 2023-02-10 16:05:16.159578 watts-0.5.0/src/watts/plugin_accert.py
--rw-r--r--   0        0        0     8118 2023-02-10 16:05:16.163579 watts-0.5.0/src/watts/plugin_dakota.py
--rw-r--r--   0        0        0     2622 2023-02-10 16:05:16.163579 watts-0.5.0/src/watts/plugin_mcnp.py
--rw-r--r--   0        0        0     3677 2023-02-10 16:05:16.163579 watts-0.5.0/src/watts/plugin_moose.py
--rw-r--r--   0        0        0     5424 2023-02-10 16:05:16.163579 watts-0.5.0/src/watts/plugin_openmc.py
--rw-r--r--   0        0        0     3724 2023-02-10 16:05:16.163579 watts-0.5.0/src/watts/plugin_pyarc.py
--rw-r--r--   0        0        0     8275 2023-02-10 16:05:16.163579 watts-0.5.0/src/watts/plugin_relap5.py
--rw-r--r--   0        0        0     5172 2023-02-10 16:05:16.163579 watts-0.5.0/src/watts/plugin_sas.py
--rw-r--r--   0        0        0     1960 2023-02-10 16:05:16.163579 watts-0.5.0/src/watts/plugin_serpent.py
--rw-r--r--   0        0        0     4099 2023-02-10 16:05:16.163579 watts-0.5.0/src/watts/results.py
--rw-r--r--   0        0        0     1925 2023-02-10 16:05:16.163579 watts-0.5.0/src/watts/template.py
--rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 watts-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-11 16:06:39.083480 watts-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2001 2023-07-11 16:06:39.083480 watts-0.5.1/README.md
+-rw-r--r--   0        0        0     1542 2023-07-11 16:06:39.095480 watts-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-07-11 16:06:39.095480 watts-0.5.1/src/watts/__init__.py
+-rw-r--r--   0        0        0     3589 2023-07-11 16:06:39.095480 watts-0.5.1/src/watts/console.py
+-rw-r--r--   0        0        0     4528 2023-07-11 16:06:39.095480 watts-0.5.1/src/watts/database.py
+-rw-r--r--   0        0        0     3813 2023-07-11 16:06:39.095480 watts-0.5.1/src/watts/fileutils.py
+-rw-r--r--   0        0        0    10216 2023-07-11 16:06:39.095480 watts-0.5.1/src/watts/fundamental_data.py
+-rw-r--r--   0        0        0   472648 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/mass_1.mas20.txt
+-rw-r--r--   0        0        0     8579 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/parameters.py
+-rw-r--r--   0        0        0    10344 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin.py
+-rw-r--r--   0        0        0     2633 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin_abce.py
+-rw-r--r--   0        0        0     2821 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin_accert.py
+-rw-r--r--   0        0        0     8118 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin_dakota.py
+-rw-r--r--   0        0        0    11782 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin_mcnp.py
+-rw-r--r--   0        0        0     3677 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin_moose.py
+-rw-r--r--   0        0        0     5424 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin_openmc.py
+-rw-r--r--   0        0        0     3724 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin_pyarc.py
+-rw-r--r--   0        0        0     8275 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin_relap5.py
+-rw-r--r--   0        0        0     5394 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin_sas.py
+-rw-r--r--   0        0        0     1960 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/plugin_serpent.py
+-rw-r--r--   0        0        0     4099 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/results.py
+-rw-r--r--   0        0        0     1925 2023-07-11 16:06:39.099480 watts-0.5.1/src/watts/template.py
+-rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 watts-0.5.1/PKG-INFO
```

### Comparing `watts-0.5.0/LICENSE` & `watts-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/README.md` & `watts-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/pyproject.toml` & `watts-0.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "watts"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
     { name = "UChicago Argonne, LLC", email = "watts@anl.gov" },
 ]
 license = { file = "LICENSE" }
 description = "Workflow and Template Toolkit for Simulation"
 readme = "README.md"
 classifiers = [
@@ -22,14 +22,15 @@
     "Topic :: Scientific/Engineering",
     "Programming Language :: C++",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.7"
 dependencies = [
     "Jinja2",
     "dill",
     "numpy",
     "pandas",
```

### Comparing `watts-0.5.0/src/watts/__init__.py` & `watts-0.5.1/src/watts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 from .template import *
 from .parameters import *
 from .database import *
 
 # This allows a user to write watts.Quantity
 from astropy.units import Quantity
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
```

### Comparing `watts-0.5.0/src/watts/console.py` & `watts-0.5.1/src/watts/console.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/database.py` & `watts-0.5.1/src/watts/database.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/fileutils.py` & `watts-0.5.1/src/watts/fileutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,45 @@
 # SPDX-License-Identifier: MIT
 
 from contextlib import contextmanager
 import errno
 import os
 import platform
 import select
+import shutil
 import subprocess
 import sys
 import tempfile
 from typing import Union
 
 if sys.platform != 'win32':
     import fcntl
 
 # Type for arguments that accept file paths
 PathLike = Union[str, bytes, os.PathLike]
 
 
 @contextmanager
-def cd_tmpdir():
-    """Context manager to change to/return from a tmpdir."""
-    with tempfile.TemporaryDirectory() as tmpdir:
-        cwd = os.getcwd()
-        try:
-            os.chdir(tmpdir)
-            yield
-        finally:
-            os.chdir(cwd)
+def cd_tmpdir(cleanup: bool = True):
+    """Context manager to change to/return from a tmpdir.
+
+    Parameters
+    ----------
+    cleanup
+        Whether to clean up the temporary directory
+    """
+    tmpdir = tempfile.mkdtemp()
+    cwd = os.getcwd()
+    try:
+        os.chdir(tmpdir)
+        yield
+    finally:
+        os.chdir(cwd)
+        if cleanup:
+            shutil.rmtree(tmpdir)
 
 
 def open_file(path: PathLike):
     """Open a file in explorer/finder/nautilus
 
     Parameters
     ----------
```

### Comparing `watts-0.5.0/src/watts/parameters.py` & `watts-0.5.1/src/watts/parameters.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/plugin.py` & `watts-0.5.1/src/watts/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-FileCopyrightText: 2022-2023 UChicago Argonne, LLC
 # SPDX-License-Identifier: MIT
 
 from abc import ABC, abstractmethod
 from contextlib import redirect_stdout, redirect_stderr
-from datetime import datetime
 import os
 from pathlib import Path
 import shutil
 import time
 from typing import Optional, List, Union
 import uuid
 
@@ -64,25 +63,29 @@
     def run(self):
         ...
 
     @abstractmethod
     def postrun(self, params: Parameters, exec_info: ExecInfo) -> Results:
         ...
 
-    def __call__(self, params: Parameters = None, name: str = '', verbose=True, **kwargs) -> Results:
+    def __call__(self, params: Parameters = None, name: str = '', verbose=True,
+                 cleanup: bool = True, **kwargs) -> Results:
         """Run the complete workflow for the plugin
 
         Parameters
         ----------
         params
             Parameters used in generating inputs
         name
             Name associated with execution of plugin
         verbose
             Whether to print execution information
+        cleanup
+            Determines whether the temporary directory will be cleaned up
+            immediately after execution.
         **kwargs
             Keyword arguments passed to the `run` method
 
         Returns
         -------
         Results from running plugin
         """
@@ -98,16 +101,16 @@
         if params is None:
             params = Parameters()
 
         # Create execution info
         timestamp = time.time_ns()
         exec_info = ExecInfo(db.job_id, plugin_name, name, timestamp)
 
-        with cd_tmpdir():
-            # Copy extra inputs to temporary directory
+        with cd_tmpdir(cleanup=cleanup):
+            # Copy extra inputs to execution directory
             cwd = Path.cwd()
             for path in self.extra_inputs:
                 shutil.copy(str(path), str(cwd))  # Remove str() for Python 3.8+
 
             # Generate input files and perform any other prerun actions
             self.prerun(params)
```

### Comparing `watts-0.5.0/src/watts/plugin_abce.py` & `watts-0.5.1/src/watts/plugin_abce.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-2023 UChicago Argonne, LLC
 # SPDX-License-Identifier: MIT
 
+from pathlib import Path
 import sys
 from typing import List, Optional
 
 from .fileutils import PathLike
 from .parameters import Parameters
 from .plugin import PluginGeneric, _find_executable
 from .results import Results, ExecInfo
@@ -50,14 +51,24 @@
         executable = _find_executable(executable, 'ABCE_DIR')
         execute_command = [sys.executable, '{self.executable}', '--settings_file', '{self.input_name}']
         super().__init__(
             executable, execute_command, template_file, extra_inputs,
             extra_template_inputs, 'ABCE', show_stdout, show_stderr)
         self.input_name = 'settings.yml'
 
+    @PluginGeneric.executable.setter
+    def executable(self, exe: PathLike):
+        if not exe.is_file():
+            raise RuntimeError(
+                f"{self.plugin_name} script '{exe}' does not exist. The "
+                "ABCE_DIR environment variable needs to be set to a directory "
+                "containing the run.py script."
+            )
+        self._executable = Path(exe)
+
 
 class ResultsABCE(Results):
     """ABCE simulation results
 
     Parameters
     ----------
     params
```

### Comparing `watts-0.5.0/src/watts/plugin_accert.py` & `watts-0.5.1/src/watts/plugin_accert.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/plugin_dakota.py` & `watts-0.5.1/src/watts/plugin_dakota.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/plugin_moose.py` & `watts-0.5.1/src/watts/plugin_moose.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/plugin_openmc.py` & `watts-0.5.1/src/watts/plugin_openmc.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/plugin_pyarc.py` & `watts-0.5.1/src/watts/plugin_pyarc.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/plugin_relap5.py` & `watts-0.5.1/src/watts/plugin_relap5.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/plugin_sas.py` & `watts-0.5.1/src/watts/plugin_sas.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,23 @@
 
         """
         csv_files = glob.glob("*.csv") # List all csv files
 
         csv_data = {}
         for file in csv_files:
             if os.path.getsize(file) > 0: # Check if file is empty
+                csv_data_sub = {}
                 csv_file_df = pd.read_csv(file)
+
                 for column_name in csv_file_df.columns:
-                    csv_data[column_name] =  np.array(csv_file_df[column_name])
+                    csv_data_sub[column_name] =  np.array(csv_file_df[column_name])
+
+                csv_data[file[:-4]] = csv_data_sub # Save sub dictionary as csv file name
+                                                   # Removed .csv extension from file name
+
         return csv_data
 
 
 class PluginSAS(PluginGeneric):
     """Plugin for running SAS
 
     Parameters
```

### Comparing `watts-0.5.0/src/watts/plugin_serpent.py` & `watts-0.5.1/src/watts/plugin_serpent.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/results.py` & `watts-0.5.1/src/watts/results.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/src/watts/template.py` & `watts-0.5.1/src/watts/template.py`

 * *Files identical despite different names*

### Comparing `watts-0.5.0/PKG-INFO` & `watts-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watts
-Version: 0.5.0
+Version: 0.5.1
 Summary: Workflow and Template Toolkit for Simulation
 Author-email: "UChicago Argonne, LLC" <watts@anl.gov>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -15,14 +15,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2
 Requires-Dist: dill
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: platformdirs
 Requires-Dist: prettytable
 Requires-Dist: astropy
```

