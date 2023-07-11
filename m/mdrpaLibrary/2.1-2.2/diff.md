# Comparing `tmp/mdrpaLibrary-2.1.tar.gz` & `tmp/mdrpaLibrary-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrpaLibrary-2.1.tar", last modified: Tue Jul 11 09:10:09 2023, max compression
+gzip compressed data, was "mdrpaLibrary-2.2.tar", last modified: Tue Jul 11 09:23:48 2023, max compression
```

## Comparing `mdrpaLibrary-2.1.tar` & `mdrpaLibrary-2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:10:09.868921 mdrpaLibrary-2.1/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-11 09:10:09.868752 mdrpaLibrary-2.1/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:10:09.867161 mdrpaLibrary-2.1/mdrpaLibrary/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:24:56.000000 mdrpaLibrary-2.1/mdrpaLibrary/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3325 2023-07-06 11:19:01.000000 mdrpaLibrary-2.1/mdrpaLibrary/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      529 2023-07-11 08:54:27.000000 mdrpaLibrary-2.1/mdrpaLibrary/getUiModels.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3352 2023-07-06 11:19:23.000000 mdrpaLibrary-2.1/mdrpaLibrary/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1870 2023-07-11 09:08:10.000000 mdrpaLibrary-2.1/mdrpaLibrary/modelDrivenRpa.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3366 2023-07-06 11:20:06.000000 mdrpaLibrary-2.1/mdrpaLibrary/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3425 2023-07-06 11:20:26.000000 mdrpaLibrary-2.1/mdrpaLibrary/selectFromDropdownModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-06 11:20:30.000000 mdrpaLibrary-2.1/mdrpaLibrary/sendReportModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:10:09.868393 mdrpaLibrary-2.1/mdrpaLibrary/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-2.1/mdrpaLibrary/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2350 2023-07-11 08:04:53.000000 mdrpaLibrary-2.1/mdrpaLibrary/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:10:09.868100 mdrpaLibrary-2.1/mdrpaLibrary.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-11 09:10:09.000000 mdrpaLibrary-2.1/mdrpaLibrary.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-11 09:10:09.000000 mdrpaLibrary-2.1/mdrpaLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-11 09:10:09.000000 mdrpaLibrary-2.1/mdrpaLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-11 09:10:09.000000 mdrpaLibrary-2.1/mdrpaLibrary.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-11 09:10:09.868971 mdrpaLibrary-2.1/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-11 09:09:13.000000 mdrpaLibrary-2.1/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:23:48.611000 mdrpaLibrary-2.2/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-11 09:23:48.610881 mdrpaLibrary-2.2/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:23:48.609516 mdrpaLibrary-2.2/mdrpaLibrary/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:24:56.000000 mdrpaLibrary-2.2/mdrpaLibrary/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3325 2023-07-06 11:19:01.000000 mdrpaLibrary-2.2/mdrpaLibrary/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      529 2023-07-11 08:54:27.000000 mdrpaLibrary-2.2/mdrpaLibrary/getUiModels.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3352 2023-07-06 11:19:23.000000 mdrpaLibrary-2.2/mdrpaLibrary/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2005 2023-07-11 09:23:18.000000 mdrpaLibrary-2.2/mdrpaLibrary/modelDrivenRpa.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3366 2023-07-06 11:20:06.000000 mdrpaLibrary-2.2/mdrpaLibrary/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3425 2023-07-06 11:20:26.000000 mdrpaLibrary-2.2/mdrpaLibrary/selectFromDropdownModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-06 11:20:30.000000 mdrpaLibrary-2.2/mdrpaLibrary/sendReportModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:23:48.610707 mdrpaLibrary-2.2/mdrpaLibrary/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-2.2/mdrpaLibrary/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2350 2023-07-11 08:04:53.000000 mdrpaLibrary-2.2/mdrpaLibrary/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:23:48.610302 mdrpaLibrary-2.2/mdrpaLibrary.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-11 09:23:48.000000 mdrpaLibrary-2.2/mdrpaLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-11 09:23:48.000000 mdrpaLibrary-2.2/mdrpaLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-11 09:23:48.000000 mdrpaLibrary-2.2/mdrpaLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-11 09:23:48.000000 mdrpaLibrary-2.2/mdrpaLibrary.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-11 09:23:48.611041 mdrpaLibrary-2.2/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-11 09:23:35.000000 mdrpaLibrary-2.2/setup.py
```

### Comparing `mdrpaLibrary-2.1/mdrpaLibrary/clickButtonModel.robot` & `mdrpaLibrary-2.2/mdrpaLibrary/clickButtonModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.1/mdrpaLibrary/getUiModels.robot` & `mdrpaLibrary-2.2/mdrpaLibrary/getUiModels.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.1/mdrpaLibrary/inputFieldModel.robot` & `mdrpaLibrary-2.2/mdrpaLibrary/inputFieldModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.1/mdrpaLibrary/modelDrivenRpa.py` & `mdrpaLibrary-2.2/mdrpaLibrary/modelDrivenRpa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from robot.api.deco import keyword
 from robot.libraries.BuiltIn import BuiltIn
+import platform
 
 class ModelDrivenRpa:
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
 
     def __init__(self):
         self.builtin = BuiltIn()
         self.resource_dir = os.path.dirname(os.path.abspath(__file__))
@@ -15,17 +16,21 @@
             'selectFromDropdownModel.robot',
             'getUiModels.robot',
             'sendReportModel.robot'
         ]  
 
     def import_resource_file(self, resource_file):
         file_path = os.path.join(self.resource_dir, resource_file)
-        file_path = os.path.normpath(file_path)
-        self.builtin.import_resource(file_path)
 
+        if platform.system() == 'Windows':
+            file_path = file_path.replace('\\', '\\\\')
+        else:
+            file_path = file_path.replace('\\', '/')
+
+        self.builtin.import_resource(file_path)
 
     @keyword
     def click_button_model(self, *args):
         self.import_resource_file(self.resource_files[0])  
         self.builtin.run_keyword('Click Button Model', *args)
 
     @keyword
```

### Comparing `mdrpaLibrary-2.1/mdrpaLibrary/selectCheckboxModel.robot` & `mdrpaLibrary-2.2/mdrpaLibrary/selectCheckboxModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.1/mdrpaLibrary/selectFromDropdownModel.robot` & `mdrpaLibrary-2.2/mdrpaLibrary/selectFromDropdownModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.1/mdrpaLibrary/sendReportModel.robot` & `mdrpaLibrary-2.2/mdrpaLibrary/sendReportModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.1/mdrpaLibrary/utils/utils.robot` & `mdrpaLibrary-2.2/mdrpaLibrary/utils/utils.robot`

 * *Files identical despite different names*

