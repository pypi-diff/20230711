# Comparing `tmp/statprocon-0.0.5.tar.gz` & `tmp/statprocon-0.0.6.tar.gz`

## Comparing `statprocon-0.0.5.tar` & `statprocon-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 statprocon-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.5/requirements-dev.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/xmr.iml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.5/statprocon/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.5/statprocon/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.5/statprocon/charts/__init__.py
--rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 statprocon-0.0.5/statprocon/charts/xmr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 statprocon-0.0.5/tests/test_xmr.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.5/LICENSE
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 statprocon-0.0.5/README.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 statprocon-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 statprocon-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.6/requirements-dev.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/xmr.iml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.6/statprocon/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.6/statprocon/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.6/statprocon/charts/__init__.py
+-rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 statprocon-0.0.6/statprocon/charts/xmr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     8265 2020-02-02 00:00:00.000000 statprocon-0.0.6/tests/test_xmr.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 statprocon-0.0.6/README.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 statprocon-0.0.6/PKG-INFO
```

### Comparing `statprocon-0.0.5/requirements-dev.txt` & `statprocon-0.0.6/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.5/.idea/workspace.xml` & `statprocon-0.0.6/.idea/workspace.xml`

 * *Files 4% similar despite different names*

#### Comparing `statprocon-0.0.5/.idea/workspace.xml` & `statprocon-0.0.6/.idea/workspace.xml`

```diff
@@ -43,20 +43,20 @@
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">
     <property name="RunOnceActivity.OpenProjectViewOnStart" value="true"/>
     <property name="RunOnceActivity.ShowReadmeOnStart" value="true"/>
     <property name="WebServerToolWindowFactoryState" value="false"/>
-    <property name="last_opened_file_path" value="$PROJECT_DIR$"/>
+    <property name="last_opened_file_path" value="$PROJECT_DIR$/statprocon"/>
     <property name="node.js.detected.package.eslint" value="true"/>
     <property name="node.js.detected.package.tslint" value="true"/>
     <property name="node.js.selected.package.eslint" value="(autodetect)"/>
     <property name="node.js.selected.package.tslint" value="(autodetect)"/>
-    <property name="settings.editor.selected.configurable" value="com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable"/>
+    <property name="settings.editor.selected.configurable" value="preferences.externalTools"/>
   </component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/statprocon/charts"/>
       <recent name="$PROJECT_DIR$"/>
     </key>
   </component>
@@ -88,15 +88,15 @@
       <changelist id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment=""/>
       <created>1688827023388</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1688827023388</updated>
       <workItem from="1688827024910" duration="1917000"/>
       <workItem from="1688848868641" duration="17704000"/>
-      <workItem from="1688944372544" duration="1441000"/>
+      <workItem from="1688944372544" duration="9103000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `statprocon-0.0.5/.idea/xmr.iml` & `statprocon-0.0.6/.idea/xmr.iml`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.5/statprocon/charts/xmr.py` & `statprocon-0.0.6/statprocon/charts/xmr.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from typing import cast, Union, Optional
 
 TYPE_COUNTS = list[Decimal | int]
 TYPE_MOVING_RANGES = list[Decimal | int | None]
 
 
 class XmR:
+    ROUNDING = 3
+
     def __init__(
             self,
             counts: TYPE_COUNTS,
             subset_start_index: int = 0,
             subset_end_index: Optional[int] = None,
     ):
         """
@@ -23,14 +25,32 @@
         self.i = max(0, subset_start_index)
         self.j = len(counts)
         if subset_end_index:
             self.j = min(self.j, subset_end_index)
 
         assert self.i <= self.j
 
+    def __repr__(self):
+        result = ''
+        for k, v in self.to_dict().items():
+            k_format = '{0: <6}'.format(k)
+            result += f'{k_format}: {v}\n'
+        return result
+
+    def to_dict(self):
+        return {
+            'Counts': self.counts,
+            'UNPL': self.upper_natural_process_limit(),
+            'X bar': self.x_average(),
+            'LNPL': self.lower_natural_process_limit(),
+            'MR': self.moving_ranges(),
+            'URL': self.upper_range_limit(),
+            'MR bar': self.mr_average(),
+        }
+
     def moving_ranges(self) -> TYPE_MOVING_RANGES:
         """
         Moving ranges are the absolute differences between successive count values.
         The first element will always be None
         """
         if self._mr:
             return self._mr
@@ -42,36 +62,38 @@
             else:
                 value = cast(Union[Decimal | int], abs(c - self.counts[i - 1]))
                 result.append(value)
         self._mr = result
         return self._mr
 
     def x_average(self) -> Decimal:
-        return self.mean(self.counts[self.i:self.j])
+        avg = self.mean(self.counts[self.i:self.j])
+        return self.round(avg)
 
     def mr_average(self) -> Decimal:
         assert self.moving_ranges()[0] is None
         valid_values = cast(TYPE_COUNTS, self.moving_ranges()[self.i+1:self.j])
-        return self.mean(valid_values)
+        avg = self.mean(valid_values)
+        return self.round(avg)
 
     def upper_range_limit(self) -> Decimal:
         limit = Decimal('3.268') * self.mr_average()
-        return round(limit, 3)
+        return self.round(limit)
 
     def upper_natural_process_limit(self) -> Decimal:
         limit = self.x_average() + (Decimal('2.660') * self.mr_average())
-        return round(limit, 3)
+        return self.round(limit)
 
     def lower_natural_process_limit(self) -> Decimal:
         """
         LNPL can be negative.
         It's the caller's responsibility to take max(LNPL, 0) if a negative LNPL does not make sense
         """
         limit = self.x_average() - (Decimal('2.660') * self.mr_average())
-        return round(limit, 3)
+        return self.round(limit)
 
     def rule_1_x_indices_beyond_limits(
             self,
             upper_limit: Optional[Decimal] = None,
             lower_limit: Optional[Decimal] = None
     ) -> list[bool]:
         """
@@ -180,14 +202,17 @@
                 successive_values = near_limits[i - 3:i + 1]
                 if abs(sum(successive_values)) >= 3:
                     for j in range(i - 3, i + 1):
                         result[j] = True
 
         return result
 
+    def round(self, value: Decimal):
+        return round(value, self.ROUNDING)
+
     @staticmethod
     def _points_beyond_limits(
             data: TYPE_COUNTS | TYPE_MOVING_RANGES,
             upper_limit: Decimal,
             lower_limit: Decimal = Decimal('0')
     ) -> list[bool]:
         result = [False] * len(data)
```

### Comparing `statprocon-0.0.5/tests/test_xmr.py` & `statprocon-0.0.6/tests/test_xmr.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,33 @@
 class XmRTestCase(unittest.TestCase):
     def test_empty_data(self):
         counts = []
         xmr = XmR(counts)
         mr = xmr.moving_ranges()
         self.assertEqual(mr, [])
 
+    def test_repr(self):
+        counts = [3, 4, 5]
+        xmr = XmR(counts)
+
+        expected = """Counts: [3, 4, 5]
+UNPL  : 6.660
+X bar : 4.000
+LNPL  : 1.340
+MR    : [None, 1, 1]
+URL   : 3.268
+MR bar: 1.000
+"""
+        self.assertEqual(xmr.__repr__(), expected)
+
+    def test_average_contains_one_more_exponent_as_input(self):
+        counts = [3, 3, 4]
+        xmr = XmR(counts)
+        self.assertEqual(xmr.x_average(), Decimal('3.333'))
+
     def test_moving_range_ints(self):
         counts = [1, 10, 100, 50]
         xmr = XmR(counts)
         mr = xmr.moving_ranges()
         self.assertEqual(mr, [None, 9, 90, 50])
 
     def test_moving_range_decimals(self):
@@ -24,37 +43,37 @@
         mr = xmr.moving_ranges()
         self.assertEqual(mr, [None, Decimal('9.74'), Decimal('5.99')])
 
     def test_upper_range_limit(self):
         counts = [1, 10, 100, 50]
         xmr = XmR(counts)
         url = xmr.upper_range_limit()
-        self.assertEqual(url, Decimal('162.311'))
+        self.assertEqual(url, Decimal('162.312'))
 
     def test_upper_natural_process_limit(self):
         counts = [1, 10, 100, 50]
         xmr = XmR(counts)
         limit = xmr.upper_natural_process_limit()
-        self.assertEqual(limit, Decimal('172.363'))
+        self.assertEqual(limit, Decimal('172.364'))
 
     def test_lower_natural_process_limit(self):
         counts = [1, 10, 100, 50]
         xmr = XmR(counts)
         limit = xmr.lower_natural_process_limit()
-        self.assertEqual(limit, Decimal('-91.863'))
+        self.assertEqual(limit, Decimal('-91.864'))
 
     def test_limits_with_subsets(self):
         counts = [1] * 25
         counts[1] = 10
         counts[2] = 100
         counts[3] = 50
 
         xmr = XmR(counts, subset_end_index=24)
-        self.assertEqual(xmr.upper_natural_process_limit(), Decimal('30.441'))
-        self.assertEqual(xmr.upper_range_limit(), Decimal('28.133'))
+        self.assertEqual(xmr.upper_natural_process_limit(), Decimal('30.442'))
+        self.assertEqual(xmr.upper_range_limit(), Decimal('28.134'))
 
         # Adjust manually so that all subset values should be 1
         xmr.i = 4
         self.assertEqual(xmr.x_average(), 1)
         self.assertEqual(xmr.lower_natural_process_limit(), xmr.upper_natural_process_limit())
 
     def test_rule_1_points_beyond_upper_limits(self):
@@ -186,15 +205,15 @@
         """
 
         x_values = [120, 140, 100, 150, 260, 150, 100, 120, 300, 300, 275, 300, 140, 170, 150, 150, 190, 180]
         mr_values = [None, 20, 40, 50, 110, 110, 50, 20, 180, 0, 25, 25, 160, 30, 20, 0, 40, 10]
         x_avg = Decimal('183.1')
         mr_avg = Decimal('52.4')
 
-        # changes are due to rounding and using constants with 2 sig digits
+        # changes are due to rounding
         unpl = Decimal('322.3')  # 322.5 in book
         lnpl = Decimal('43.8')  # 43.7 in book
         url = Decimal('171.1')  # 171.3 in book
 
         xmr = XmR(x_values)
 
         self.assertListEqual(xmr.moving_ranges(), mr_values)
```

### Comparing `statprocon-0.0.5/LICENSE` & `statprocon-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.5/README.md` & `statprocon-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.5/pyproject.toml` & `statprocon-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statprocon"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Matt McCormick", email="mattmccor@gmail.com" },
 ]
 description = "A Python helper library for generating Process Behaviour Charts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `statprocon-0.0.5/PKG-INFO` & `statprocon-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statprocon
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python helper library for generating Process Behaviour Charts
 Project-URL: Homepage, https://github.com/mattmccormick/statprocon
 Project-URL: Bug Tracker, https://github.com/mattmccormick/statprocon/issues
 Project-URL: Changelog, https://github.com/mattmccormick/statprocon/blob/main/CHANGELOG.md
 Author-email: Matt McCormick <mattmccor@gmail.com>
 License-File: LICENSE
 Keywords: Process Behavior Chart,Process Behaviour Chart,QCC,Quality Control Chart,SPC,Shewhart,Statistical Process Control,Wheeler,XmR
```

