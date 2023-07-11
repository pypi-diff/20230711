# Comparing `tmp/acro-0.3.0.tar.gz` & `tmp/acro-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acro-0.3.0.tar", last modified: Tue Jul  4 13:23:06 2023, max compression
+gzip compressed data, was "acro-0.4.0.tar", last modified: Tue Jul 11 11:27:04 2023, max compression
```

## Comparing `acro-0.3.0.tar` & `acro-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-04 13:23:06.670482 acro-0.3.0/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-09-08 13:00:24.000000 acro-0.3.0/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-07-04 13:23:06.670482 acro-0.3.0/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2227 2023-06-28 14:56:03.000000 acro-0.3.0/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-04 13:23:06.670482 acro-0.3.0/acro/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       32 2023-06-30 14:21:04.000000 acro-0.3.0/acro/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    31733 2023-07-03 21:17:41.000000 acro-0.3.0/acro/acro.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1072 2023-06-29 14:07:18.000000 acro-0.3.0/acro/default.yaml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15983 2023-07-04 13:10:14.000000 acro-0.3.0/acro/record.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10248 2023-07-04 13:10:14.000000 acro-0.3.0/acro/utils.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-04 13:23:06.670482 acro-0.3.0/acro.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-07-04 13:23:06.000000 acro-0.3.0/acro.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      323 2023-07-04 13:23:06.000000 acro-0.3.0/acro.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-04 13:23:06.000000 acro-0.3.0/acro.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       46 2023-07-04 13:23:06.000000 acro-0.3.0/acro.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-07-04 13:23:06.000000 acro-0.3.0/acro.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-04 13:23:06.670482 acro-0.3.0/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-07-04 13:18:25.000000 acro-0.3.0/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-04 13:23:06.670482 acro-0.3.0/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2022-09-26 11:44:01.000000 acro-0.3.0/test/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2056 2023-06-30 14:25:22.000000 acro-0.3.0/test/stata.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12940 2023-07-04 13:10:14.000000 acro-0.3.0/test/test_initial.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8932 2023-07-03 19:49:42.000000 acro-0.3.0/test/test_stata_interface.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:27:04.854569 acro-0.4.0/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2023-07-11 11:22:02.000000 acro-0.4.0/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-07-11 11:27:04.854569 acro-0.4.0/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2227 2023-07-11 11:22:02.000000 acro-0.4.0/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:27:04.854569 acro-0.4.0/acro/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       32 2023-07-11 11:22:02.000000 acro-0.4.0/acro/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    32413 2023-07-11 11:22:02.000000 acro-0.4.0/acro/acro.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1072 2023-07-11 11:22:02.000000 acro-0.4.0/acro/default.yaml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19383 2023-07-11 11:22:02.000000 acro-0.4.0/acro/record.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10320 2023-07-11 11:22:02.000000 acro-0.4.0/acro/utils.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       49 2023-07-11 11:22:02.000000 acro-0.4.0/acro/version.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:27:04.854569 acro-0.4.0/acro.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-07-11 11:27:04.000000 acro-0.4.0/acro.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      339 2023-07-11 11:27:04.000000 acro-0.4.0/acro.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-11 11:27:04.000000 acro-0.4.0/acro.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       46 2023-07-11 11:27:04.000000 acro-0.4.0/acro.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-07-11 11:27:04.000000 acro-0.4.0/acro.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-11 11:27:04.854569 acro-0.4.0/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-07-11 11:22:14.000000 acro-0.4.0/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:27:04.854569 acro-0.4.0/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-07-11 11:22:02.000000 acro-0.4.0/test/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2056 2023-07-11 11:22:02.000000 acro-0.4.0/test/stata.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14281 2023-07-11 11:22:02.000000 acro-0.4.0/test/test_initial.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9013 2023-07-11 11:22:02.000000 acro-0.4.0/test/test_stata_interface.py
```

### Comparing `acro-0.3.0/LICENSE` & `acro-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acro-0.3.0/PKG-INFO` & `acro-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acro
-Version: 0.3.0
+Version: 0.4.0
 Summary: ACRO: Tools for the Automatic Checking of Research Outputs
 Home-page: https://github.com/AI-SDC/ACRO
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `acro-0.3.0/README.md` & `acro-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `acro-0.3.0/acro/acro.py` & `acro-0.4.0/acro/acro.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """ACRO: Automatic Checking of Research Outputs."""
 
+import json
 import logging
+import os
 import pathlib
 import warnings
 from collections.abc import Callable
 from inspect import stack
 
 import pandas as pd
 import statsmodels.api as sm
@@ -81,29 +83,38 @@
 
         Returns
         -------
         Records
             Object storing the outputs.
         """
         self.results.finalise(path, ext)
+        config_filename: str = os.path.normpath(f"{path}/config.json")
+        with open(config_filename, "w", newline="", encoding="utf-8") as file:
+            json.dump(self.config, file, indent=4, sort_keys=False)
         return self.results
 
     def remove_output(self, key: str) -> None:
         """Removes an output from the results.
 
         Parameters
         ----------
         key : str
             Key specifying which output to remove, e.g., 'output_0'.
         """
         self.results.remove(key)
 
-    def print_outputs(self) -> None:
-        """Prints the current results dictionary."""
-        self.results.print()
+    def print_outputs(self) -> str:
+        """Prints the current results dictionary.
+
+        Returns
+        -------
+        str
+            String representation of all outputs.
+        """
+        return self.results.print()
 
     def custom_output(self, filename: str, comment: str = "") -> None:
         """Adds an unsupported output to the results dictionary.
 
         Parameters
         ----------
         filename : str
@@ -256,28 +267,28 @@
         # pd.crosstab returns nan for an empty cell
         for name, mask in masks.items():
             mask.fillna(value=1, inplace=True)
             mask = mask.astype(int)
             mask.replace({0: False, 1: True}, inplace=True)
             masks[name] = mask
 
-        # build the properties dictionary
-        properties: dict = {"method": "crosstab", "suppressed": self.suppress}
-        utils.update_table_properties(masks, properties)
+        # build the sdc dictionary
+        sdc: dict = utils.get_table_sdc(masks, self.suppress)
         # get the status and summary
-        status, summary = utils.get_summary(properties)
+        status, summary = utils.get_summary(sdc)
         # apply the suppression
         safe_table, outcome = utils.apply_suppression(table, masks)
         if self.suppress:
             table = safe_table
         # record output
         self.results.add(
             status=status,
             output_type="table",
-            properties=properties,
+            properties={"method": "crosstab"},
+            sdc=sdc,
             command=command,
             summary=summary,
             outcome=outcome,
             output=[table],
         )
         return table
 
@@ -395,28 +406,28 @@
             # check for missing values -- currently unsupported
             if utils.CHECK_MISSING_VALUES:
                 agg = [utils.agg_missing] * n_agg if n_agg > 1 else utils.agg_missing
                 masks["missing"] = pd.pivot_table(  # type: ignore
                     data, values, index, columns, aggfunc=agg
                 )
 
-        # build the properties dictionary
-        properties: dict = {"method": "pivot_table", "suppressed": self.suppress}
-        utils.update_table_properties(masks, properties)
+        # build the sdc dictionary
+        sdc: dict = utils.get_table_sdc(masks, self.suppress)
         # get the status and summary
-        status, summary = utils.get_summary(properties)
+        status, summary = utils.get_summary(sdc)
         # apply the suppression
         safe_table, outcome = utils.apply_suppression(table, masks)
         if self.suppress:
             table = safe_table
         # record output
         self.results.add(
             status=status,
             output_type="table",
-            properties=properties,
+            properties={"method": "pivot_table"},
+            sdc=sdc,
             command=command,
             summary=summary,
             outcome=outcome,
             output=[table],
         )
         return table
 
@@ -488,14 +499,15 @@
         results = model.fit()
         status, summary, dof = self.__check_model_dof("ols", model)
         tables: list[SimpleTable] = results.summary().tables
         self.results.add(
             status=status,
             output_type="regression",
             properties={"method": "ols", "dof": dof},
+            sdc={},
             command=command,
             summary=summary,
             outcome=DataFrame(),
             output=utils.get_summary_dataframes(tables),
         )
         return results
 
@@ -551,14 +563,15 @@
         results = model.fit()
         status, summary, dof = self.__check_model_dof("olsr", model)
         tables: list[SimpleTable] = results.summary().tables
         self.results.add(
             status=status,
             output_type="regression",
             properties={"method": "olsr", "dof": dof},
+            sdc={},
             command=command,
             summary=summary,
             outcome=DataFrame(),
             output=utils.get_summary_dataframes(tables),
         )
         return results
 
@@ -599,14 +612,15 @@
         results = model.fit()
         status, summary, dof = self.__check_model_dof("logit", model)
         tables: list[SimpleTable] = results.summary().tables
         self.results.add(
             status=status,
             output_type="regression",
             properties={"method": "logit", "dof": dof},
+            sdc={},
             command=command,
             summary=summary,
             outcome=DataFrame(),
             output=utils.get_summary_dataframes(tables),
         )
         return results
 
@@ -662,14 +676,15 @@
         results = model.fit()
         status, summary, dof = self.__check_model_dof("logitr", model)
         tables: list[SimpleTable] = results.summary().tables
         self.results.add(
             status=status,
             output_type="regression",
             properties={"method": "logitr", "dof": dof},
+            sdc={},
             command=command,
             summary=summary,
             outcome=DataFrame(),
             output=utils.get_summary_dataframes(tables),
         )
         return results
 
@@ -710,14 +725,15 @@
         results = model.fit()
         status, summary, dof = self.__check_model_dof("probit", model)
         tables: list[SimpleTable] = results.summary().tables
         self.results.add(
             status=status,
             output_type="regression",
             properties={"method": "probit", "dof": dof},
+            sdc={},
             command=command,
             summary=summary,
             outcome=DataFrame(),
             output=utils.get_summary_dataframes(tables),
         )
         return results
 
@@ -773,14 +789,15 @@
         results = model.fit()
         status, summary, dof = self.__check_model_dof("probitr", model)
         tables: list[SimpleTable] = results.summary().tables
         self.results.add(
             status=status,
             output_type="regression",
             properties={"method": "probitr", "dof": dof},
+            sdc={},
             command=command,
             summary=summary,
             outcome=DataFrame(),
             output=utils.get_summary_dataframes(tables),
         )
         return results
 
@@ -804,14 +821,26 @@
         output : str
             The name of the output.
         comment : str
             The comment.
         """
         self.results.add_comments(output, comment)
 
+    def add_exception(self, output: str, reason: str) -> None:
+        """Adds an exception request to an output.
+
+        Parameters
+        ----------
+        output : str
+            The name of the output.
+        reason : str
+            The comment.
+        """
+        self.results.add_exception(output, reason)
+
 
 def add_constant(data, prepend: bool = True, has_constant: str = "skip"):
     """Add a column of ones to an array.
 
     Parameters
     ----------
     data : array_like
```

### Comparing `acro-0.3.0/acro/default.yaml` & `acro-0.4.0/acro/default.yaml`

 * *Files identical despite different names*

### Comparing `acro-0.3.0/acro/record.py` & `acro-0.4.0/acro/record.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """ACRO: Output storage and serialization."""
 
 import datetime
+import hashlib
 import json
 import logging
 import os
 import shutil
-import warnings
 from pathlib import Path
 from typing import Any
 
 import pandas as pd
 from pandas import DataFrame
 
+from .version import __version__
+
 logger = logging.getLogger("acro:records")
 
 
 def load_outcome(outcome: dict) -> DataFrame:
     """Returns a DataFrame from an outcome dictionary.
 
     Parameters
@@ -63,34 +65,39 @@
         Unique identifier.
     status : str
         SDC status: {"pass", "fail", "review"}
     output_type : str
         Type of output, e.g., "regression"
     properties : dict
         Dictionary containing structured output data.
+    sdc : dict
+        Dictionary containing SDC results.
     command : str
         String representation of the operation performed.
     summary : str
         String summarising the ACRO checks.
     outcome : DataFrame
         DataFrame describing the details of ACRO checks.
     output : Any
         List of output DataFrames.
-    comments : list[str] | None
+    comments : list[str]
         List of strings entered by the user to add comments to the output.
+    exception : str
+        Description of why an exception to fail/review should be granted.
     timestamp : str
         Time the record was created in ISO format.
     """
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         uid: str,
         status: str,
         output_type: str,
         properties: dict,
+        sdc: dict,
         command: str,
         summary: str,
         outcome: DataFrame,
         output: list[str] | list[DataFrame],
         comments: list[str] | None = None,
     ) -> None:
         """Constructs a new output record.
@@ -101,14 +108,16 @@
             Unique identifier.
         status : str
             SDC status: {"pass", "fail", "review"}
         output_type : str
             Type of output, e.g., "regression"
         properties : dict
             Dictionary containing structured output data.
+        sdc : dict
+            Dictionary containing SDC results.
         command : str
             String representation of the operation performed.
         summary : str
             String summarising the ACRO checks.
         outcome : DataFrame
             DataFrame describing the details of ACRO checks.
         output : list[str] | list[DataFrame]
@@ -116,19 +125,21 @@
         comments : list[str] | None, default None
             List of strings entered by the user to add comments to the output.
         """
         self.uid: str = uid
         self.status: str = status
         self.output_type: str = output_type
         self.properties: dict = properties
+        self.sdc: dict = sdc
         self.command: str = command
         self.summary: str = summary
         self.outcome: DataFrame = outcome
         self.output: Any = output
         self.comments: list[str] = [] if comments is None else comments
+        self.exception: str = ""
         now = datetime.datetime.now()
         self.timestamp: str = now.isoformat()
 
     def serialize_output(self, path: str = "outputs") -> list[str]:
         """Serializes outputs.
 
         Parameters
@@ -160,42 +171,36 @@
         if self.output_type == "custom":
             for filename in self.output:
                 if os.path.exists(filename):
                     shutil.copy(filename, path)
                     output.append(Path(filename).name)
         return output
 
-    def to_dict(self, path: str = "outputs", serialize: bool = True) -> dict:
-        """Returns a dictionary representation of an output and serializes
-        any DataFrame outputs as csv.
+    def __str__(self) -> str:
+        """Returns a string representation of a record.
 
-        Parameters
-        ----------
-        path : str
-            Name of the folder that outputs are to be written.
-        serialize : bool, default True
-            Whether to serialize individual output DataFrames.
+        Returns
+        -------
+        str
+            The record.
         """
-        output = self.output
-        if serialize:
-            output = self.serialize_output(path)
-        # convert to dictionary
-        output_dict = {
-            "uid": self.uid,
-            "status": self.status,
-            "type": self.output_type,
-            "properties": self.properties,
-            "command": self.command,
-            "summary": self.summary,
-            "outcome": json.loads(self.outcome.to_json()),
-            "output": output,
-            "timestamp": self.timestamp,
-            "comments": self.comments,
-        }
-        return output_dict
+        return (
+            f"uid: {self.uid}\n"
+            f"status: {self.status}\n"
+            f"type: {self.output_type}\n"
+            f"properties: {self.properties}\n"
+            f"sdc: {self.sdc}\n"
+            f"command: {self.command}\n"
+            f"summary: {self.summary}\n"
+            f"outcome: {self.outcome}\n"
+            f"output: {self.output}\n"
+            f"timestamp: {self.timestamp}\n"
+            f"comments: {self.comments}\n"
+            f"exception: {self.exception}\n"
+        )
 
 
 class Records:
     """Stores data related to a collection of output records."""
 
     def __init__(self) -> None:
         """Constructs a new object for storing multiple records."""
@@ -203,14 +208,15 @@
         self.output_id: int = 0
 
     def add(  # pylint: disable=too-many-arguments
         self,
         status: str,
         output_type: str,
         properties: dict,
+        sdc: dict,
         command: str,
         summary: str,
         outcome: DataFrame,
         output: list[str] | list[DataFrame],
         comments: list[str] | None = None,
     ) -> None:
         """Adds an output to the results.
@@ -219,14 +225,16 @@
         ----------
         status : str
             SDC status: {"pass", "fail", "review"}
         output_type : str
             Type of output, e.g., "regression"
         properties : dict
             Dictionary containing structured output data.
+        sdc : dict
+            Dictionary containing SDC results.
         command : str
             String representation of the operation performed.
         summary : str
             String summarising the ACRO checks.
         outcome : DataFrame
             DataFrame describing the details of ACRO checks.
         output : list[str | list[DataFrame]
@@ -235,14 +243,15 @@
             List of strings entered by the user to add comments to the output.
         """
         new = Record(
             uid=f"output_{self.output_id}",
             status=status,
             output_type=output_type,
             properties=properties,
+            sdc=sdc,
             command=command,
             summary=summary,
             outcome=outcome,
             output=output,
             comments=comments,
         )
         self.results[new.uid] = new
@@ -253,19 +262,18 @@
         """Removes an output from the results.
 
         Parameters
         ----------
         key : str
             Key specifying which output to remove, e.g., 'output_0'.
         """
-        if key in self.results:
-            del self.results[key]
-            logger.info("remove(): %s removed", key)
-        else:
-            warnings.warn(f"unable to remove {key}, key not found", stacklevel=8)
+        if key not in self.results:
+            raise ValueError(f"unable to remove {key}, key not found")
+        del self.results[key]
+        logger.info("remove(): %s removed", key)
 
     def get(self, key: str) -> Record:
         """Returns a specified output from the results.
 
         Parameters
         ----------
         key : str
@@ -318,14 +326,15 @@
             An optional comment.
         """
         output = Record(
             uid=f"output_{self.output_id}",
             status="review",
             output_type="custom",
             properties={},
+            sdc={},
             command="custom",
             summary="review",
             outcome=DataFrame(),
             output=[os.path.normpath(filename)],
             comments=None if comment is None else [comment],
         )
         self.results[output.uid] = output
@@ -336,80 +345,132 @@
         Parameters
         ----------
         old : str
             The old name of the output.
         new : str
             The new name of the output.
         """
-        if old in self.results:
-            self.results[new] = self.results[old]
-            self.results[new].uid = new
-            del self.results[old]
-            logger.info("rename_output(): %s renamed to %s", old, new)
-        else:
-            warnings.warn(f"unable to rename {old}, key not found", stacklevel=8)
+        if old not in self.results:
+            raise ValueError(f"unable to rename {old}, key not found")
+        if new in self.results:
+            raise ValueError(f"unable to rename, {new} already exists")
+        self.results[new] = self.results[old]
+        self.results[new].uid = new
+        del self.results[old]
+        logger.info("rename_output(): %s renamed to %s", old, new)
 
     def add_comments(self, output: str, comment: str) -> None:
         """Adds a comment to an output.
 
         Parameters
         ----------
         output : str
             The name of the output.
         comment : str
             The comment.
         """
-        if output in self.results:
-            self.results[output].comments.append(comment)
-            logger.info("a comment was added to %s", output)
-        else:
-            warnings.warn(f"unable to find {output}, key not found", stacklevel=8)
+        if output not in self.results:
+            raise ValueError(f"unable to find {output}, key not found")
+        self.results[output].comments.append(comment)
+        logger.info("a comment was added to %s", output)
+
+    def add_exception(self, output: str, reason: str) -> None:
+        """Adds an exception request to an output.
+
+        Parameters
+        ----------
+        output : str
+            The name of the output.
+        reason : str
+            The reason the output should be released.
+        """
+        if output not in self.results:
+            raise ValueError(f"unable to add exception: {output} not found")
+        self.results[output].exception = reason
+        logger.info("exception request was added to %s", output)
+
+    def print(self) -> str:
+        """Prints the current results.
 
-    def print(self) -> None:
-        """Prints the current results."""
+        Returns
+        -------
+        str
+            String representation of all outputs.
+        """
         logger.debug("print()")
-        for name, output in self.results.items():
-            print(f"{name}:")
-            for key, item in output.to_dict(serialize=False).items():
-                print(f"{key}: {item}")
-            print("\n")
+        outputs: str = ""
+        for _, record in self.results.items():
+            outputs += str(record) + "\n"
+        print(outputs)
+        return outputs
+
+    def validate_outputs(self) -> None:
+        """Prompts researcher to complete any required fields."""
+        for _, record in self.results.items():
+            if record.status != "pass" and record.exception == "":
+                print(
+                    f"{str(record)}\n"
+                    f"The status of the record above is: {record.status}.\n"
+                    "Please explain why an exception should be granted.\n"
+                )
+                record.exception = input("")
+                print("")
 
     def finalise(self, path: str, ext: str) -> None:
         """Creates a results file for checking.
 
         Parameters
         ----------
         path : str
             Name of a folder to save outputs.
         ext : str
             Extension of the results file. Valid extensions: {json, xlsx}.
         """
         logger.debug("finalise()")
+        self.validate_outputs()
         if ext == "json":
             self.finalise_json(path)
         elif ext == "xlsx":
             self.finalise_excel(path)
         else:
             raise ValueError("Invalid file extension. Options: {json, xlsx}")
+        self.write_checksums(path)
         logger.info("outputs written to: %s", path)
 
     def finalise_json(self, path: str) -> None:
         """Writes outputs to a JSON file.
 
         Parameters
         ----------
         path : str
             Name of a folder to save outputs.
         """
         outputs: dict = {}
         for key, val in self.results.items():
-            outputs[key] = val.to_dict(path)
+            outputs[key] = {
+                "uid": val.uid,
+                "status": val.status,
+                "type": val.output_type,
+                "properties": val.properties,
+                "files": [],
+                "outcome": json.loads(val.outcome.to_json()),
+                "command": val.command,
+                "summary": val.summary,
+                "timestamp": val.timestamp,
+                "comments": val.comments,
+                "exception": val.exception,
+            }
+            files: list[str] = val.serialize_output(path)
+            for file in files:
+                outputs[key]["files"].append({"name": file, "sdc": val.sdc})
+
+        results: dict = {"version": __version__, "results": outputs}
         filename: str = os.path.normpath(f"{path}/results.json")
-        with open(filename, "w", newline="", encoding="utf-8") as file:
-            json.dump(outputs, file, indent=4, sort_keys=False)
+        with open(filename, "w", newline="", encoding="utf-8") as handle:
+            json.dump(results, handle, indent=4, sort_keys=False)
 
     def finalise_excel(self, path: str) -> None:
         """Writes outputs to an excel spreadsheet.
 
         Parameters
         ----------
         path : str
@@ -452,32 +513,71 @@
                 if output.outcome is not None:
                     output.outcome.to_excel(writer, sheet_name=output_id, startrow=4)
                 # output
                 for table in output.output:
                     start = 1 + writer.sheets[output_id].max_row
                     table.to_excel(writer, sheet_name=output_id, startrow=start)
 
-    def load_json(self, path: str) -> None:
-        """Loads outputs from a JSON file.
+    def write_checksums(self, path: str) -> None:
+        """Writes checksums for each file to checksums folder.
 
         Parameters
         ----------
         path : str
-            Name of an output folder containing results.json.
+            Name of a folder to save outputs.
         """
-        self.results = {}
-        filename = os.path.normpath(f"{path}/results.json")
-        with open(filename, newline="", encoding="utf-8") as file:
-            data = json.load(file)
-            for key, val in data.items():
-                self.results[key] = Record(
-                    val["uid"],
-                    val["status"],
-                    val["type"],
-                    val["properties"],
-                    val["command"],
-                    val["summary"],
-                    load_outcome(val["outcome"]),
-                    load_output(path, val["output"]),
-                    val["comments"],
-                )
-                self.results[key].timestamp = val["timestamp"]
+        checksums: dict[str, str] = {}
+        for name in os.listdir(path):
+            filename = os.path.join(path, name)
+            if os.path.isfile(filename):
+                with open(filename, "rb") as file:
+                    read = file.read()
+                    checksums[name] = hashlib.sha256(read).hexdigest()
+        checksums_dir: str = os.path.normpath(f"{path}/checksums")
+        os.makedirs(checksums_dir, exist_ok=True)
+        for name, sha256 in checksums.items():
+            filename = os.path.join(checksums_dir, name + ".txt")
+            with open(filename, "w", encoding="utf-8") as file:
+                file.write(sha256)
+
+
+def load_records(path: str) -> Records:
+    """Loads outputs from a JSON file.
+
+    Parameters
+    ----------
+    path : str
+        Name of an output folder containing results.json.
+
+    Returns
+    -------
+    Records
+        The loaded records.
+    """
+    records = Records()
+    filename = os.path.normpath(f"{path}/results.json")
+    with open(filename, newline="", encoding="utf-8") as handle:
+        data = json.load(handle)
+        if data["version"] != __version__:  # pragma: no cover
+            raise ValueError("error loading output")
+        for key, val in data["results"].items():
+            files: list[dict] = val["files"]
+            filenames: list = []
+            sdcs: list = []
+            for file in files:
+                filenames.append(file["name"])
+                sdcs.append(file["sdc"])
+            records.results[key] = Record(
+                uid=val["uid"],
+                status=val["status"],
+                output_type=val["type"],
+                properties=val["properties"],
+                sdc=sdcs[0],
+                command=val["command"],
+                summary=val["summary"],
+                outcome=load_outcome(val["outcome"]),
+                output=load_output(path, filenames),
+                comments=val["comments"],
+            )
+            records.results[key].exception = val["exception"]
+            records.results[key].timestamp = val["timestamp"]
+    return records
```

### Comparing `acro-0.3.0/acro/utils.py` & `acro-0.4.0/acro/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -214,79 +214,81 @@
             except TypeError:
                 logger.warning("problem mask %s is not binary", name)
         outcome_df = outcome_df.replace({"": "ok"})
     logger.info("outcome_df:\n%s", outcome_df)
     return safe_df, outcome_df
 
 
-def update_table_properties(masks: dict[str, DataFrame], properties: dict) -> None:
-    """Updates the properties dictionary using the suppression masks.
+def get_table_sdc(masks: dict[str, DataFrame], suppress: bool) -> dict:
+    """Returns the SDC dictionary using the suppression masks.
 
     Parameters
     ----------
     masks : dict[str, DataFrame]
         Dictionary of tables specifying suppression masks for application.
-    properties : dict
-        Properties of the SDC checks.
+    suppress : bool
+        Whether suppression has been applied.
     """
     # summary of cells to be suppressed
-    properties["negative"] = 0
-    properties["missing"] = 0
-    properties["threshold"] = 0
-    properties["p-ratio"] = 0
-    properties["nk-rule"] = 0
+    sdc: dict = {"summary": {"suppressed": suppress}, "cells": {}}
+    sdc["summary"]["negative"] = 0
+    sdc["summary"]["missing"] = 0
+    sdc["summary"]["threshold"] = 0
+    sdc["summary"]["p-ratio"] = 0
+    sdc["summary"]["nk-rule"] = 0
     for name, mask in masks.items():
-        properties[name] = int(mask.to_numpy().sum())
+        sdc["summary"][name] = int(mask.to_numpy().sum())
     # positions of cells to be suppressed
-    properties["sdc"] = {}
-    properties["sdc"]["negative"] = []
-    properties["sdc"]["missing"] = []
-    properties["sdc"]["threshold"] = []
-    properties["sdc"]["p-ratio"] = []
-    properties["sdc"]["nk-rule"] = []
+    sdc["cells"]["negative"] = []
+    sdc["cells"]["missing"] = []
+    sdc["cells"]["threshold"] = []
+    sdc["cells"]["p-ratio"] = []
+    sdc["cells"]["nk-rule"] = []
     for name, mask in masks.items():
         true_positions = np.column_stack(np.where(mask.values))
         for pos in true_positions:
             row_index, col_index = pos
-            properties["sdc"][name].append([int(row_index), int(col_index)])
+            sdc["cells"][name].append([int(row_index), int(col_index)])
+    return sdc
 
 
-def get_summary(properties: dict) -> tuple[str, str]:
+def get_summary(sdc: dict) -> tuple[str, str]:
     """Returns the status and summary of the suppression masks.
 
     Parameters
     ----------
-    properties : dict
+    sdc : dict
         Properties of the SDC checks.
 
     Returns
     -------
     str
         Status: {"review", "fail", "pass"}.
     str
         Summary of the suppression masks.
     """
     status: str = "pass"
     summary: str = ""
-    sup: str = "suppressed" if properties["suppressed"] else "may need suppressing"
-    if properties["negative"]:
+    sdc_summary = sdc["summary"]
+    sup: str = "suppressed" if sdc_summary["suppressed"] else "may need suppressing"
+    if sdc_summary["negative"] > 0:
         summary += "negative values found"
         status = "review"
-    elif properties["missing"]:
+    elif sdc_summary["missing"] > 0:
         summary += "missing values found"
         status = "review"
     else:
-        if properties["threshold"] > 0:
-            summary += f"threshold: {properties['threshold']} cells {sup}; "
+        if sdc_summary["threshold"] > 0:
+            summary += f"threshold: {sdc_summary['threshold']} cells {sup}; "
             status = "fail"
-        if properties["p-ratio"] > 0:
-            summary += f"p-ratio: {properties['p-ratio']} cells {sup}; "
+        if sdc_summary["p-ratio"] > 0:
+            summary += f"p-ratio: {sdc_summary['p-ratio']} cells {sup}; "
             status = "fail"
-        if properties["nk-rule"] > 0:
-            summary += f"nk-rule: {properties['nk-rule']} cells {sup}; "
+        if sdc_summary["nk-rule"] > 0:
+            summary += f"nk-rule: {sdc_summary['nk-rule']} cells {sup}; "
             status = "fail"
     if summary != "":
         summary = f"{status}; {summary}"
     else:
         summary = status
     logger.info("get_summary(): %s", summary)
     return status, summary
```

### Comparing `acro-0.3.0/acro.egg-info/PKG-INFO` & `acro-0.4.0/acro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acro
-Version: 0.3.0
+Version: 0.4.0
 Summary: ACRO: Tools for the Automatic Checking of Research Outputs
 Home-page: https://github.com/AI-SDC/ACRO
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `acro-0.3.0/setup.py` & `acro-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="acro",
-    version="0.3.0",
+    version="0.4.0",
     license="MIT",
     maintainer="Jim Smith",
     maintainer_email="james.smith@uwe.ac.uk",
     description="ACRO: Tools for the Automatic Checking of Research Outputs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-SDC/ACRO",
```

### Comparing `acro-0.3.0/test/stata.py` & `acro-0.4.0/test/stata.py`

 * *Files identical despite different names*

### Comparing `acro-0.3.0/test/test_initial.py` & `acro-0.4.0/test/test_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from acro import ACRO, add_constant, record, utils
-from acro.record import Records
+from acro.record import Records, load_records
 
 # pylint: disable=redefined-outer-name
 
 PATH: str = "RES_PYTEST"
 
 
 @pytest.fixture
@@ -63,29 +63,31 @@
 
 def test_crosstab_threshold(data, acro):
     """Crosstab threshold test."""
     _ = acro.crosstab(data.year, data.grant_type)
     output = acro.results.get_index(0)
     total_nan: int = output.output[0]["R/G"].isnull().sum()
     assert total_nan == 6
-    positions = output.properties["sdc"]["threshold"]
+    positions = output.sdc["cells"]["threshold"]
     for pos in positions:
         row, col = pos
         assert np.isnan(output.output[0].iloc[row, col])
+    acro.add_exception("output_0", "Let me have it")
     results: Records = acro.finalise()
     correct_summary: str = "fail; threshold: 6 cells suppressed; "
     output = results.get_index(0)
     assert output.summary == correct_summary
 
 
 def test_crosstab_multiple(data, acro):
     """Crosstab multiple rule test."""
     _ = acro.crosstab(
         data.year, data.grant_type, values=data.inc_grants, aggfunc="mean"
     )
+    acro.add_exception("output_0", "Let me have it")
     results: Records = acro.finalise()
     correct_summary: str = (
         "fail; threshold: 6 cells suppressed; p-ratio: 1 cells suppressed; "
         "nk-rule: 1 cells suppressed; "
     )
     output = results.get_index(0)
     assert output.summary == correct_summary
@@ -96,14 +98,16 @@
     data.loc[0:10, "inc_grants"] = -10
     _ = acro.crosstab(
         data.year, data.grant_type, values=data.inc_grants, aggfunc="mean"
     )
     _ = acro.pivot_table(
         data, index=["grant_type"], values=["inc_grants"], aggfunc=["mean", "std"]
     )
+    acro.add_exception("output_0", "Let me have it")
+    acro.add_exception("output_1", "I want this")
     results: Records = acro.finalise()
     correct_summary: str = "review; negative values found"
     output_0 = results.get_index(0)
     output_1 = results.get_index(1)
     assert output_0.summary == correct_summary
     assert output_1.summary == correct_summary
 
@@ -135,14 +139,15 @@
     _ = acro.pivot_table(
         data,
         index=["grant_type"],
         columns=["year"],
         values=["inc_grants"],
         aggfunc=["mean", "std"],
     )
+    acro.add_exception("output_0", "Let me have it")
     results: Records = acro.finalise()
     correct_summary: str = (
         "fail; threshold: 14 cells suppressed; "
         "p-ratio: 2 cells suppressed; nk-rule: 2 cells suppressed; "
     )
     output_0 = results.get_index(0)
     assert output_0.summary == correct_summary
@@ -219,157 +224,178 @@
     assert output_2.summary == correct_summary
     assert output_3.summary == correct_summary
 
 
 def test_finalise_excel(data, acro):
     """Finalise excel test."""
     _ = acro.crosstab(data.year, data.grant_type)
+    acro.add_exception("output_0", "Let me have it")
     results: Records = acro.finalise(PATH, "xlsx")
     output_0 = results.get_index(0)
     filename = os.path.normpath(f"{PATH}/results.xlsx")
     load_data = pd.read_excel(filename, sheet_name=output_0.uid)
     correct_cell: str = "_ = acro.crosstab(data.year, data.grant_type)"
     assert load_data.iloc[0, 0] == "Command"
     assert load_data.iloc[0, 1] == correct_cell
 
 
-def test_output_removal(data, acro):
+def test_output_removal(data, acro, monkeypatch):
     """Output removal and print test."""
     _ = acro.crosstab(data.year, data.grant_type)
     _ = acro.crosstab(data.year, data.grant_type)
     _ = acro.crosstab(data.year, data.grant_type)
+    exceptions = ["I want it", "Let me have it", "Please!"]
+    monkeypatch.setattr("builtins.input", lambda _: exceptions.pop(0))
     results: Records = acro.finalise()
     output_0 = results.get("output_0")
     output_1 = results.get("output_1")
     # remove something that is there
     acro.remove_output(output_0.uid)
     results = acro.finalise()
     correct_summary: str = "fail; threshold: 6 cells suppressed; "
     keys = results.get_keys()
     assert output_0.uid not in keys
     assert output_1.uid in keys
     assert output_1.summary == correct_summary
     acro.print_outputs()
     # remove something that is not there
-    with pytest.warns(UserWarning):
+    with pytest.raises(ValueError):
         acro.remove_output("123")
 
 
 def test_load_output():
     """Empty array when loading output."""
     with pytest.raises(ValueError):
         record.load_output(PATH, [])
 
 
 def test_finalise_invalid(data, acro):
     """Invalid output format when finalising."""
     _ = acro.crosstab(data.year, data.grant_type)
+    output_0 = acro.results.get_index(0)
+    output_0.exception = "Let me have it"
     with pytest.raises(ValueError):
         _ = acro.finalise(PATH, "123")
 
 
 def test_finalise_json(data, acro):
     """Finalise json test."""
     _ = acro.crosstab(data.year, data.grant_type)
+    acro.add_exception("output_0", "Let me have it")
     # write JSON
     result: Records = acro.finalise(PATH, "json")
     # load JSON
-    loaded: Records = Records()
-    loaded.load_json(PATH)
+    loaded: Records = load_records(PATH)
     orig = result.get_index(0)
     read = loaded.get_index(0)
+    print("*****************************")
+    print(orig)
+    print("*****************************")
+    print(read)
+    print("*****************************")
     # check equal
     assert orig.uid == read.uid
     assert orig.status == read.status
     assert orig.output_type == read.output_type
     assert orig.properties == read.properties
+    assert orig.sdc == read.sdc
     assert orig.command == read.command
     assert orig.summary == read.summary
     assert orig.comments == read.comments
     assert orig.timestamp == read.timestamp
     assert (orig.output[0].reset_index()).equals(read.output[0])
     # test reading JSON
     with open(os.path.normpath(f"{PATH}/results.json"), encoding="utf-8") as file:
         json_data = json.load(file)
-    assert json_data[orig.uid]["output"][0] == f"{orig.uid}_0.csv"
-    # regression check: the outcome fields are dicts not strings
-    assert json_data[orig.uid]["outcome"]["R/G"] == {
-        "2010": "threshold; ",
-        "2011": "threshold; ",
-        "2012": "threshold; ",
-        "2013": "threshold; ",
-        "2014": "threshold; ",
-        "2015": "threshold; ",
-    }
+    results: dict = json_data["results"]
+    assert results[orig.uid]["files"][0]["name"] == f"{orig.uid}_0.csv"
 
 
 def test_rename_output(data, acro):
     """Output renaming test."""
     _ = acro.crosstab(data.year, data.grant_type)
+    _ = acro.crosstab(data.year, data.grant_type)
+    acro.add_exception("output_0", "Let me have it")
+    acro.add_exception("output_1", "I want this")
     results: Records = acro.finalise()
     output_0 = results.get_index(0)
     orig_name = output_0.uid
     new_name = "cross_table"
     acro.rename_output(orig_name, new_name)
     results = acro.finalise()
     assert output_0.uid == new_name
     assert orig_name not in results.get_keys()
     assert os.path.exists(f"outputs/{new_name}_0.csv")
     # rename an output that doesn't exist
-    with pytest.warns(UserWarning):
+    with pytest.raises(ValueError):
         acro.rename_output("123", "name")
+    # rename an output to another that already exists
+    with pytest.raises(ValueError):
+        acro.rename_output("output_1", "cross_table")
 
 
 def test_add_comments(data, acro):
     """Adding comments to output test."""
     _ = acro.crosstab(data.year, data.grant_type)
+    acro.add_exception("output_0", "Let me have it")
     results: Records = acro.finalise()
     output_0 = results.get_index(0)
     assert output_0.comments == []
     comment = "This is a cross table between year and grant_type"
     acro.add_comments(output_0.uid, comment)
     assert output_0.comments == [comment]
     comment_1 = "6 cells were suppressed"
     acro.add_comments(output_0.uid, comment_1)
     assert output_0.comments == [comment, comment_1]
     # add a comment to something that is not there
-    with pytest.warns(UserWarning):
+    with pytest.raises(ValueError):
         acro.add_comments("123", "comment")
 
 
 def test_custom_output(acro):
     """Adding an unsupported output to the results dictionary test."""
     filename = "notebooks/XandY.jfif"
     file_path = os.path.normpath(filename)
     acro.custom_output(filename)
+    acro.add_exception("output_0", "Let me have it")
     results: Records = acro.finalise(path=PATH)
     output_0 = results.get_index(0)
     assert output_0.output == [file_path]
     assert os.path.exists(os.path.normpath(f"{PATH}/XandY.jfif"))
 
 
-def test_missing(data, acro):
+def test_missing(data, acro, monkeypatch):
     """Pivot table and Crosstab with negative values."""
     utils.CHECK_MISSING_VALUES = True
     data.loc[0:10, "inc_grants"] = np.NaN
     _ = acro.crosstab(
         data.year, data.grant_type, values=data.inc_grants, aggfunc="mean"
     )
     _ = acro.pivot_table(
         data, index=["grant_type"], values=["inc_grants"], aggfunc=["mean", "std"]
     )
+    exceptions = ["I want it", "Let me have it"]
+    monkeypatch.setattr("builtins.input", lambda _: exceptions.pop(0))
     results: Records = acro.finalise()
     correct_summary: str = "review; missing values found"
     output_0 = results.get_index(0)
     output_1 = results.get_index(1)
     assert output_0.summary == correct_summary
     assert output_1.summary == correct_summary
+    assert output_0.exception == "I want it"
+    assert output_1.exception == "Let me have it"
 
 
 def test_suppression_error(caplog):
     """Apply suppression type error test."""
     table_data = {"col1": [1, 2], "col2": [3, 4]}
     mask_data = {"col1": [np.NaN, True], "col2": [True, True]}
     table = pd.DataFrame(data=table_data)
     masks = {"test": pd.DataFrame(data=mask_data)}
     utils.apply_suppression(table, masks)
     assert "problem mask test is not binary" in caplog.text
+
+
+def test_adding_exception(acro):
+    """Adding an exception to an output that doesn't exist test."""
+    with pytest.raises(ValueError):
+        acro.add_exception("output_0", "Let me have it")
```

### Comparing `acro-0.3.0/test/test_stata_interface.py` & `acro-0.4.0/test/test_stata_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,16 +272,17 @@
         assert rets[0] == format_string, errmsg
         ret = rets[1]
         ret = ret.replace("NaN", "0")
         ret = ret.replace(".0", "")
         assert ret.split() == correct.split(), f"got\n{ret}\n expected\n{correct}"
 
 
-def test_stata_finalise():
+def test_stata_finalise(monkeypatch):
     """Checks finalise gets called correctly."""
+    monkeypatch.setattr("builtins.input", lambda _: "Let me have it")
     ret = dummy_acrohandler(
         data,
         command="finalise",
         varlist="",
         exclusion="",
         exp="",
         weights="",
```

