# Comparing `tmp/panther_core-0.4.9.tar.gz` & `tmp/panther_core-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther_core-0.4.9.tar", last modified: Thu Feb 16 20:08:24 2023, max compression
+gzip compressed data, was "panther_core-0.5.0.tar", last modified: Tue Jul 11 18:53:20 2023, max compression
```

## Comparing `panther_core-0.4.9.tar` & `panther_core-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 cdzombak   (501) staff       (20)        0 2023-02-16 20:08:24.034899 panther_core-0.4.9/
--rw-r--r--   0 cdzombak   (501) staff       (20)    34522 2022-08-22 19:18:23.000000 panther_core-0.4.9/LICENSE.txt
--rw-r--r--   0 cdzombak   (501) staff       (20)      170 2022-08-22 19:18:23.000000 panther_core-0.4.9/MANIFEST.in
--rw-r--r--   0 cdzombak   (501) staff       (20)      601 2023-02-16 20:08:24.034967 panther_core-0.4.9/PKG-INFO
--rw-r--r--   0 cdzombak   (501) staff       (20)     1855 2022-08-22 19:18:23.000000 panther_core-0.4.9/README.md
-drwxr-xr-x   0 cdzombak   (501) staff       (20)        0 2023-02-16 20:08:24.031948 panther_core-0.4.9/panther_core/
--rw-r--r--   0 cdzombak   (501) staff       (20)       30 2022-09-29 20:25:27.000000 panther_core-0.4.9/panther_core/__init__.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     4873 2022-12-07 21:36:42.000000 panther_core-0.4.9/panther_core/data_model.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     8875 2022-12-16 18:38:01.000000 panther_core-0.4.9/panther_core/detection.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     4058 2022-09-29 20:25:27.000000 panther_core-0.4.9/panther_core/enriched_event.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     1649 2022-12-07 21:36:42.000000 panther_core-0.4.9/panther_core/exceptions.py
-drwxr-xr-x   0 cdzombak   (501) staff       (20)        0 2023-02-16 20:08:24.034185 panther_core-0.4.9/panther_core/exec/
--rw-r--r--   0 cdzombak   (501) staff       (20)      735 2022-08-22 19:18:23.000000 panther_core-0.4.9/panther_core/exec/__init__.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     2755 2022-12-07 21:36:42.000000 panther_core-0.4.9/panther_core/exec/common.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     7274 2022-09-29 20:25:27.000000 panther_core-0.4.9/panther_core/exec/results.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     4786 2022-09-29 20:25:27.000000 panther_core-0.4.9/panther_core/exec/task.py
--rw-r--r--   0 cdzombak   (501) staff       (20)    17952 2023-02-16 20:07:15.000000 panther_core-0.4.9/panther_core/filter.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     7418 2022-08-22 19:18:23.000000 panther_core-0.4.9/panther_core/immutable.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     1373 2022-09-29 20:25:27.000000 panther_core-0.4.9/panther_core/policy.py
--rw-r--r--   0 cdzombak   (501) staff       (20)    30296 2022-12-16 18:38:01.000000 panther_core-0.4.9/panther_core/rule.py
-drwxr-xr-x   0 cdzombak   (501) staff       (20)        0 2023-02-16 20:08:24.034690 panther_core-0.4.9/panther_core/snapshots/
--rw-r--r--   0 cdzombak   (501) staff       (20)       21 2022-09-29 20:25:27.000000 panther_core-0.4.9/panther_core/snapshots/__init__.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     5226 2022-12-07 21:36:42.000000 panther_core-0.4.9/panther_core/snapshots/_func.py
--rw-r--r--   0 cdzombak   (501) staff       (20)    10921 2022-12-07 21:36:42.000000 panther_core-0.4.9/panther_core/testing.py
--rw-r--r--   0 cdzombak   (501) staff       (20)    12668 2022-12-07 21:36:42.000000 panther_core-0.4.9/panther_core/testing_exec_output.py
--rw-r--r--   0 cdzombak   (501) staff       (20)     1943 2022-12-07 21:36:42.000000 panther_core-0.4.9/panther_core/util.py
-drwxr-xr-x   0 cdzombak   (501) staff       (20)        0 2023-02-16 20:08:24.033183 panther_core-0.4.9/panther_core.egg-info/
--rw-r--r--   0 cdzombak   (501) staff       (20)      601 2023-02-16 20:08:23.000000 panther_core-0.4.9/panther_core.egg-info/PKG-INFO
--rw-r--r--   0 cdzombak   (501) staff       (20)      738 2023-02-16 20:08:23.000000 panther_core-0.4.9/panther_core.egg-info/SOURCES.txt
--rw-r--r--   0 cdzombak   (501) staff       (20)        1 2023-02-16 20:08:23.000000 panther_core-0.4.9/panther_core.egg-info/dependency_links.txt
--rw-r--r--   0 cdzombak   (501) staff       (20)       12 2023-02-16 20:08:23.000000 panther_core-0.4.9/panther_core.egg-info/requires.txt
--rw-r--r--   0 cdzombak   (501) staff       (20)       54 2023-02-16 20:08:23.000000 panther_core-0.4.9/panther_core.egg-info/top_level.txt
--rw-r--r--   0 cdzombak   (501) staff       (20)      271 2023-02-16 20:08:15.000000 panther_core-0.4.9/requirements.txt
--rw-r--r--   0 cdzombak   (501) staff       (20)      106 2023-02-16 20:08:24.035323 panther_core-0.4.9/setup.cfg
--rw-r--r--   0 cdzombak   (501) staff       (20)     1309 2023-02-16 20:07:15.000000 panther_core-0.4.9/setup.py
+drwxr-xr-x   0 danakatzenelson   (501) staff       (20)        0 2023-07-11 18:53:20.683855 panther_core-0.5.0/
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)    34522 2023-05-26 19:00:56.000000 panther_core-0.5.0/LICENSE.txt
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)      170 2023-05-26 19:00:56.000000 panther_core-0.5.0/MANIFEST.in
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)      601 2023-07-11 18:53:20.683922 panther_core-0.5.0/PKG-INFO
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     1855 2023-05-26 19:00:56.000000 panther_core-0.5.0/README.md
+drwxr-xr-x   0 danakatzenelson   (501) staff       (20)        0 2023-07-11 18:53:20.680143 panther_core-0.5.0/panther_core/
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)       30 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/__init__.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     4873 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/data_model.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     8875 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/detection.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     6643 2023-07-11 18:41:23.000000 panther_core-0.5.0/panther_core/enriched_event.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     1649 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/exceptions.py
+drwxr-xr-x   0 danakatzenelson   (501) staff       (20)        0 2023-07-11 18:53:20.683021 panther_core-0.5.0/panther_core/exec/
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)      735 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/exec/__init__.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     2755 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/exec/common.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     7274 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/exec/results.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     4786 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/exec/task.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)    17952 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/filter.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     7479 2023-07-11 18:41:23.000000 panther_core-0.5.0/panther_core/immutable.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     1373 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/policy.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)    30425 2023-07-11 18:41:23.000000 panther_core-0.5.0/panther_core/rule.py
+drwxr-xr-x   0 danakatzenelson   (501) staff       (20)        0 2023-07-11 18:53:20.683503 panther_core-0.5.0/panther_core/snapshots/
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)       21 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/snapshots/__init__.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     5226 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/snapshots/_func.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)    10921 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/testing.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)    12668 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/testing_exec_output.py
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     1943 2023-05-26 19:00:56.000000 panther_core-0.5.0/panther_core/util.py
+drwxr-xr-x   0 danakatzenelson   (501) staff       (20)        0 2023-07-11 18:53:20.681577 panther_core-0.5.0/panther_core.egg-info/
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)      601 2023-07-11 18:53:20.000000 panther_core-0.5.0/panther_core.egg-info/PKG-INFO
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)      738 2023-07-11 18:53:20.000000 panther_core-0.5.0/panther_core.egg-info/SOURCES.txt
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)        1 2023-07-11 18:53:20.000000 panther_core-0.5.0/panther_core.egg-info/dependency_links.txt
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)       12 2023-07-11 18:53:20.000000 panther_core-0.5.0/panther_core.egg-info/requires.txt
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)       54 2023-07-11 18:53:20.000000 panther_core-0.5.0/panther_core.egg-info/top_level.txt
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)      271 2023-07-11 18:53:11.000000 panther_core-0.5.0/requirements.txt
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)      106 2023-07-11 18:53:20.684227 panther_core-0.5.0/setup.cfg
+-rw-r--r--   0 danakatzenelson   (501) staff       (20)     1309 2023-07-11 18:41:23.000000 panther_core-0.5.0/setup.py
```

### Comparing `panther_core-0.4.9/LICENSE.txt` & `panther_core-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/PKG-INFO` & `panther_core-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: panther_core
-Version: 0.4.9
+Version: 0.5.0
 Summary: Panther core library
 Home-page: https://github.com/panther-labs/panther_core
-Download-URL: https://github.com/panther-labs/panther_core/archive/refs/tags/v0.4.9.tar.gz
+Download-URL: https://github.com/panther-labs/panther_core/archive/refs/tags/v0.5.0.tar.gz
 Author: Panther Labs Inc
 Author-email: pypi@runpanther.io
 License: AGPL-3.0
 Keywords: Security,CLI
 Classifier: Topic :: Security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `panther_core-0.4.9/README.md` & `panther_core-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/data_model.py` & `panther_core-0.5.0/panther_core/data_model.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/detection.py` & `panther_core-0.5.0/panther_core/detection.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/enriched_event.py` & `panther_core-0.5.0/panther_core/enriched_event.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
+from collections import OrderedDict
 from collections.abc import Mapping
 from functools import reduce
-from typing import Any, Optional
+from typing import Any, List, Optional, Sequence, Union
 
 from .data_model import E_NO_DATA_MODEL_FOUND, DataModel
 from .exceptions import PantherError
 from .immutable import ImmutableCaseInsensitiveDict, json_encoder
 
 __all__ = ["PantherEvent"]
 
@@ -64,19 +65,82 @@
         if method:
             return getattr(method, "__name__", repr(method))
         # no matches, return None by default
         return None
 
     def deep_get(self, *keys: str, default: Any = None) -> Any:
         """Safely return the value of an arbitrarily nested map"""
-        return reduce(
+        out = reduce(
             lambda d, key: d.get(key, default) if isinstance(d, Mapping) else default,
             keys,
             self,
         )
+        if out is None:
+            return default
+        return out
+
+    def deep_walk(
+        self, *keys: str, default: Optional[str] = None, return_val: str = "all"
+    ) -> Union[Optional[Any], Optional[List[Any]]]:
+        """Safely retrieve a value stored in complex dictionary structure
+
+        Similar to deep_get but supports accessing dictionary keys within nested lists as well
+
+        Parameters:
+        keys (str): comma-separated list of keys used to traverse the event object
+        default (str): the default value to return if the desired key's value is not present
+        return_val (str): string specifying which value to return
+                        possible values are "first", "last", or "all"
+
+        Returns:
+        any | list[any]: A single value if return_val is "first", "last",
+                        or if "all" is a list containing one element,
+                        otherwise a list of values
+        """
+
+        def _empty_list(sub_obj: Any) -> bool:
+            return (
+                all(_empty_list(next_obj) for next_obj in sub_obj)
+                if isinstance(sub_obj, Sequence) and not isinstance(sub_obj, str)
+                else False
+            )
+
+        obj = self._container
+
+        if not keys:
+            return default if _empty_list(obj) or obj is None else obj
+
+        current_key = keys[0]
+        found: OrderedDict = OrderedDict()
+
+        if isinstance(obj, Mapping):
+            next_key = PantherEvent(obj.get(current_key, default))
+            return (
+                next_key.deep_walk(*keys[1:], default=default, return_val=return_val)
+                if next_key is not None
+                else default
+            )
+        if isinstance(obj, Sequence) and not isinstance(obj, str):
+            for item in obj:
+                next_item = PantherEvent(item)
+                value = next_item.deep_walk(*keys, default=default, return_val=return_val)
+                if value is not None:
+                    if isinstance(value, Sequence) and not isinstance(value, str):
+                        for sub_item in value:
+                            found[sub_item] = None
+                    else:
+                        found[value] = None
+        found_list: list[Any] = list(found.keys())
+        if not found_list:
+            return default
+        return {
+            "first": found_list[0],
+            "last": found_list[-1],
+            "all": found_list[0] if len(found_list) == 1 else found_list,
+        }.get(return_val, "all")
 
     def _validate(self) -> None:
         if not self.data_model:
             raise PantherError(E_NO_DATA_MODEL_FOUND, self._container.get("p_log_type"))
 
     def _get_json_path(self, key: str) -> Any:
         if not self.data_model:  # makes linter happy, we never call this if not set
```

### Comparing `panther_core-0.4.9/panther_core/exceptions.py` & `panther_core-0.5.0/panther_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/exec/__init__.py` & `panther_core-0.5.0/panther_core/exec/__init__.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/exec/common.py` & `panther_core-0.5.0/panther_core/exec/common.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/exec/results.py` & `panther_core-0.5.0/panther_core/exec/results.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/exec/task.py` & `panther_core-0.5.0/panther_core/exec/task.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/filter.py` & `panther_core-0.5.0/panther_core/filter.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/immutable.py` & `panther_core-0.5.0/panther_core/immutable.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,16 +86,18 @@
         self._keymap_key_iterator: Union[None, Iterator[str]] = None
         self._keymap_fully_built = False
 
     @classmethod
     def mutable_type(cls) -> Type[dict]:
         return dict
 
-    def _shallow_copy(self, obj: dict) -> dict:
-        return obj.copy()
+    def _shallow_copy(self, obj: Any) -> dict:
+        if hasattr(type(obj), "copy"):
+            return obj.copy()
+        return obj
 
     def to_dict(self) -> dict:
         """
         Create a deep copy as a mutable dictionary.
         """
         return self.copy()
```

### Comparing `panther_core-0.4.9/panther_core/policy.py` & `panther_core-0.5.0/panther_core/policy.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/rule.py` & `panther_core-0.5.0/panther_core/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
 TRUNCATED_STRING_SUFFIX = "... (truncated)"
 
 DEFAULT_DETECTION_DEDUP_PERIOD_MINS = 60
 
 # Used to check dynamic severity output
 SEVERITY_TYPES = ["INFO", "LOW", "MEDIUM", "HIGH", "CRITICAL"]
+SEVERITY_DEFAULT = "DEFAULT"
 
 ALERT_CONTEXT_FUNCTION = "alert_context"
 DEDUP_FUNCTION = "dedup"
 DESCRIPTION_FUNCTION = "description"
 DESTINATIONS_FUNCTION = "destinations"
 REFERENCE_FUNCTION = "reference"
 RUNBOOK_FUNCTION = "runbook"
@@ -651,14 +652,16 @@
 
     def _get_severity(self, event: Mapping, use_default_on_exception: bool = True) -> Optional[str]:
 
         try:
             command = getattr(self._module, SEVERITY_FUNCTION)
             severity = self._run_command(command, event, str).upper()
             if severity not in SEVERITY_TYPES:
+                if severity == SEVERITY_DEFAULT:
+                    return self.detection_severity
                 self.logger.info(
                     "severity method for detection with id [%s] yielded [%s], expected [%s]",
                     self.detection_id,
                     severity,
                     str(SEVERITY_TYPES),
                 )
                 raise AssertionError(
```

### Comparing `panther_core-0.4.9/panther_core/snapshots/_func.py` & `panther_core-0.5.0/panther_core/snapshots/_func.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/testing.py` & `panther_core-0.5.0/panther_core/testing.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/testing_exec_output.py` & `panther_core-0.5.0/panther_core/testing_exec_output.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core/util.py` & `panther_core-0.5.0/panther_core/util.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/panther_core.egg-info/PKG-INFO` & `panther_core-0.5.0/panther_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: panther-core
-Version: 0.4.9
+Version: 0.5.0
 Summary: Panther core library
 Home-page: https://github.com/panther-labs/panther_core
-Download-URL: https://github.com/panther-labs/panther_core/archive/refs/tags/v0.4.9.tar.gz
+Download-URL: https://github.com/panther-labs/panther_core/archive/refs/tags/v0.5.0.tar.gz
 Author: Panther Labs Inc
 Author-email: pypi@runpanther.io
 License: AGPL-3.0
 Keywords: Security,CLI
 Classifier: Topic :: Security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `panther_core-0.4.9/panther_core.egg-info/SOURCES.txt` & `panther_core-0.5.0/panther_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panther_core-0.4.9/setup.py` & `panther_core-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from distutils.core import setup
 
 
-VERSION = "0.4.9"
+VERSION = "0.5.0"
 
 
 install_requires = [
     'jsonpath-ng',
 ]
 
 with open('requirements.txt') as f:
```

