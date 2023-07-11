# Comparing `tmp/bpmn-tools-0.1.3.tar.gz` & `tmp/bpmn-tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpmn-tools-0.1.3.tar", last modified: Fri Jul  7 14:37:15 2023, max compression
+gzip compressed data, was "bpmn-tools-0.1.4.tar", last modified: Tue Jul 11 11:17:53 2023, max compression
```

## Comparing `bpmn-tools-0.1.3.tar` & `bpmn-tools-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.124358 bpmn-tools-0.1.3/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.121156 bpmn-tools-0.1.3/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.1.3/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.1.3/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.1.3/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-07-07 14:37:15.124243 bpmn-tools-0.1.3/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.122069 bpmn-tools-0.1.3/bpmn_tools/
--rw-r--r--   0 xtof       (501) staff       (20)       91 2023-07-07 14:16:02.000000 bpmn-tools-0.1.3/bpmn_tools/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-06-25 07:47:11.000000 bpmn-tools-0.1.3/bpmn_tools/collaboration.py
--rw-r--r--   0 xtof       (501) staff       (20)      957 2023-05-31 08:54:54.000000 bpmn-tools-0.1.3/bpmn_tools/colors.py
--rw-r--r--   0 xtof       (501) staff       (20)     6375 2023-07-07 14:28:39.000000 bpmn-tools-0.1.3/bpmn_tools/diagrams.py
--rw-r--r--   0 xtof       (501) staff       (20)     8045 2023-07-07 14:09:04.000000 bpmn-tools-0.1.3/bpmn_tools/flow.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.123112 bpmn-tools-0.1.3/bpmn_tools/layout/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.1.3/bpmn_tools/layout/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     4984 2023-07-07 14:04:06.000000 bpmn-tools-0.1.3/bpmn_tools/layout/simple.py
--rw-r--r--   0 xtof       (501) staff       (20)     3228 2023-06-25 08:13:52.000000 bpmn-tools-0.1.3/bpmn_tools/notation.py
--rw-r--r--   0 xtof       (501) staff       (20)      865 2023-07-07 09:23:39.000000 bpmn-tools-0.1.3/bpmn_tools/util.py
--rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.1.3/bpmn_tools/visitor.py
--rw-r--r--   0 xtof       (501) staff       (20)     4665 2023-07-07 10:03:09.000000 bpmn-tools-0.1.3/bpmn_tools/xml.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.122915 bpmn-tools-0.1.3/bpmn_tools.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      703 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       48 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       24 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       22 2023-07-07 14:37:15.000000 bpmn-tools-0.1.3/bpmn_tools.egg-info/top_level.txt
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.123314 bpmn-tools-0.1.3/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.3/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.1.3/docs/conf.py
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-07-07 14:37:15.124399 bpmn-tools-0.1.3/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.1.3/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-07 14:37:15.124066 bpmn-tools-0.1.3/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.3/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1326 2023-05-30 20:03:04.000000 bpmn-tools-0.1.3/tests/test_colors.py
--rw-r--r--   0 xtof       (501) staff       (20)     2208 2023-05-31 08:38:49.000000 bpmn-tools-0.1.3/tests/test_flows.py
--rw-r--r--   0 xtof       (501) staff       (20)    10458 2023-05-30 19:47:37.000000 bpmn-tools-0.1.3/tests/test_hello.py
--rw-r--r--   0 xtof       (501) staff       (20)     4076 2023-05-31 08:39:36.000000 bpmn-tools-0.1.3/tests/test_lanes.py
--rw-r--r--   0 xtof       (501) staff       (20)     1275 2023-07-07 09:43:06.000000 bpmn-tools-0.1.3/tests/test_roundtrip.py
--rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.1.3/tests/test_visitor.py
--rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.1.3/tests/test_xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-11 11:17:53.006038 bpmn-tools-0.1.4/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-11 11:17:53.002972 bpmn-tools-0.1.4/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.1.4/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.1.4/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.1.4/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-07-11 11:17:53.005925 bpmn-tools-0.1.4/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-11 11:17:53.003865 bpmn-tools-0.1.4/bpmn_tools/
+-rw-r--r--   0 xtof       (501) staff       (20)       91 2023-07-11 11:14:16.000000 bpmn-tools-0.1.4/bpmn_tools/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-06-25 07:47:11.000000 bpmn-tools-0.1.4/bpmn_tools/collaboration.py
+-rw-r--r--   0 xtof       (501) staff       (20)      957 2023-05-31 08:54:54.000000 bpmn-tools-0.1.4/bpmn_tools/colors.py
+-rw-r--r--   0 xtof       (501) staff       (20)     6375 2023-07-07 14:28:39.000000 bpmn-tools-0.1.4/bpmn_tools/diagrams.py
+-rw-r--r--   0 xtof       (501) staff       (20)     8045 2023-07-11 11:15:52.000000 bpmn-tools-0.1.4/bpmn_tools/flow.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-11 11:17:53.004672 bpmn-tools-0.1.4/bpmn_tools/layout/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.1.4/bpmn_tools/layout/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4984 2023-07-07 14:04:06.000000 bpmn-tools-0.1.4/bpmn_tools/layout/simple.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3228 2023-06-25 08:13:52.000000 bpmn-tools-0.1.4/bpmn_tools/notation.py
+-rw-r--r--   0 xtof       (501) staff       (20)      865 2023-07-07 09:23:39.000000 bpmn-tools-0.1.4/bpmn_tools/util.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.1.4/bpmn_tools/visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4665 2023-07-07 10:03:09.000000 bpmn-tools-0.1.4/bpmn_tools/xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-11 11:17:53.004496 bpmn-tools-0.1.4/bpmn_tools.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-07-11 11:17:52.000000 bpmn-tools-0.1.4/bpmn_tools.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      726 2023-07-11 11:17:52.000000 bpmn-tools-0.1.4/bpmn_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-07-11 11:17:52.000000 bpmn-tools-0.1.4/bpmn_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       48 2023-07-11 11:17:52.000000 bpmn-tools-0.1.4/bpmn_tools.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       24 2023-07-11 11:17:52.000000 bpmn-tools-0.1.4/bpmn_tools.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       22 2023-07-11 11:17:52.000000 bpmn-tools-0.1.4/bpmn_tools.egg-info/top_level.txt
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-11 11:17:53.004851 bpmn-tools-0.1.4/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.4/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.1.4/docs/conf.py
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-07-11 11:17:53.006073 bpmn-tools-0.1.4/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.1.4/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-11 11:17:53.005751 bpmn-tools-0.1.4/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.4/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1326 2023-05-30 20:03:04.000000 bpmn-tools-0.1.4/tests/test_colors.py
+-rw-r--r--   0 xtof       (501) staff       (20)      548 2023-07-11 11:15:54.000000 bpmn-tools-0.1.4/tests/test_elements.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2208 2023-05-31 08:38:49.000000 bpmn-tools-0.1.4/tests/test_flows.py
+-rw-r--r--   0 xtof       (501) staff       (20)    10458 2023-05-30 19:47:37.000000 bpmn-tools-0.1.4/tests/test_hello.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4076 2023-05-31 08:39:36.000000 bpmn-tools-0.1.4/tests/test_lanes.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1275 2023-07-07 09:43:06.000000 bpmn-tools-0.1.4/tests/test_roundtrip.py
+-rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.1.4/tests/test_visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.1.4/tests/test_xml.py
```

### Comparing `bpmn-tools-0.1.3/.github/README.md` & `bpmn-tools-0.1.4/.github/README.md`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/LICENSE.txt` & `bpmn-tools-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/PKG-INFO` & `bpmn-tools-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpmn-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: a collection of tools to work with BPMN
 Home-page: https://github.com/christophevg/bpmn-tools
 Author: Christophe VG
 License: MIT
 Description: # BPMN Tools
         
         > a collection of tools to work with BPMN
```

### Comparing `bpmn-tools-0.1.3/bpmn_tools/collaboration.py` & `bpmn-tools-0.1.4/bpmn_tools/collaboration.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/bpmn_tools/colors.py` & `bpmn-tools-0.1.4/bpmn_tools/colors.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/bpmn_tools/diagrams.py` & `bpmn-tools-0.1.4/bpmn_tools/diagrams.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/bpmn_tools/flow.py` & `bpmn-tools-0.1.4/bpmn_tools/flow.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,26 @@
     self.incoming = []
     self.outgoing = []
     self.x      = 0
     self.y      = 0
     self.width  = 100
     self.height = 80
 
+  @property
+  def process(self):
+    return self._parent
+
+  @property
+  def lane(self):
+    for lane in self.process.laneset.lanes:
+      for ref in lane.refs:
+        if ref.ref == self:
+          return lane
+    return None
+
   def append(self, child):
     if type(child) == Incoming:
       self.incoming.append(child)
       child._parent = self
     elif type(child) == Outgoing:
       self.outgoing.append(child)
       child._parent = self
@@ -152,26 +164,14 @@
 class Task(Element):
   __tag__     = "bpmn:task"
 
   def __init__(self, name="", **kwargs):
     super().__init__(**kwargs)
     self["name"] = name
 
-  @property
-  def process(self):
-    return self._parent
-
-  @property
-  def lane(self):
-    for lane in self.process.laneset.lanes:
-      for ref in lane.refs:
-        if ref.ref == self:
-          return lane
-    return None
-
 class UserTask(Task):
   __tag__ = "bpmn:userTask"
 
 class ScriptTask(Task):
   __tag__ = "bpmn:scriptTask"
 
 class ServiceTask(Task):
```

### Comparing `bpmn-tools-0.1.3/bpmn_tools/layout/simple.py` & `bpmn-tools-0.1.4/bpmn_tools/layout/simple.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/bpmn_tools/notation.py` & `bpmn-tools-0.1.4/bpmn_tools/notation.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/bpmn_tools/util.py` & `bpmn-tools-0.1.4/bpmn_tools/util.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/bpmn_tools/visitor.py` & `bpmn-tools-0.1.4/bpmn_tools/visitor.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/bpmn_tools/xml.py` & `bpmn-tools-0.1.4/bpmn_tools/xml.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/bpmn_tools.egg-info/PKG-INFO` & `bpmn-tools-0.1.4/bpmn_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpmn-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: a collection of tools to work with BPMN
 Home-page: https://github.com/christophevg/bpmn-tools
 Author: Christophe VG
 License: MIT
 Description: # BPMN Tools
         
         > a collection of tools to work with BPMN
```

### Comparing `bpmn-tools-0.1.3/bpmn_tools.egg-info/SOURCES.txt` & `bpmn-tools-0.1.4/bpmn_tools.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -19,13 +19,14 @@
 bpmn_tools.egg-info/top_level.txt
 bpmn_tools/layout/__init__.py
 bpmn_tools/layout/simple.py
 docs/__init__.py
 docs/conf.py
 tests/__init__.py
 tests/test_colors.py
+tests/test_elements.py
 tests/test_flows.py
 tests/test_hello.py
 tests/test_lanes.py
 tests/test_roundtrip.py
 tests/test_visitor.py
 tests/test_xml.py
```

### Comparing `bpmn-tools-0.1.3/docs/conf.py` & `bpmn-tools-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/setup.py` & `bpmn-tools-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/tests/test_colors.py` & `bpmn-tools-0.1.4/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/tests/test_flows.py` & `bpmn-tools-0.1.4/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/tests/test_hello.py` & `bpmn-tools-0.1.4/tests/test_hello.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/tests/test_lanes.py` & `bpmn-tools-0.1.4/tests/test_lanes.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/tests/test_roundtrip.py` & `bpmn-tools-0.1.4/tests/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.3/tests/test_visitor.py` & `bpmn-tools-0.1.4/tests/test_visitor.py`

 * *Files identical despite different names*

