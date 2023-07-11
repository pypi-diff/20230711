# Comparing `tmp/mdrpaLibrary-2.0.tar.gz` & `tmp/mdrpaLibrary-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrpaLibrary-2.0.tar", last modified: Thu Jul  6 12:10:08 2023, max compression
+gzip compressed data, was "mdrpaLibrary-2.1.tar", last modified: Tue Jul 11 09:10:09 2023, max compression
```

## Comparing `mdrpaLibrary-2.0.tar` & `mdrpaLibrary-2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 12:10:08.702796 mdrpaLibrary-2.0/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-06 12:10:08.702628 mdrpaLibrary-2.0/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 12:10:08.701269 mdrpaLibrary-2.0/mdrpaLibrary/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:24:56.000000 mdrpaLibrary-2.0/mdrpaLibrary/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3325 2023-07-06 11:19:01.000000 mdrpaLibrary-2.0/mdrpaLibrary/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      491 2023-07-05 17:39:47.000000 mdrpaLibrary-2.0/mdrpaLibrary/getUiModels.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3352 2023-07-06 11:19:23.000000 mdrpaLibrary-2.0/mdrpaLibrary/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1982 2023-07-06 12:07:38.000000 mdrpaLibrary-2.0/mdrpaLibrary/modelDrivenRpa.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3366 2023-07-06 11:20:06.000000 mdrpaLibrary-2.0/mdrpaLibrary/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3425 2023-07-06 11:20:26.000000 mdrpaLibrary-2.0/mdrpaLibrary/selectFromDropdownModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-06 11:20:30.000000 mdrpaLibrary-2.0/mdrpaLibrary/sendReportModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 12:10:08.702304 mdrpaLibrary-2.0/mdrpaLibrary/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-2.0/mdrpaLibrary/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2484 2023-07-05 16:13:57.000000 mdrpaLibrary-2.0/mdrpaLibrary/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 12:10:08.702006 mdrpaLibrary-2.0/mdrpaLibrary.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-06 12:10:08.000000 mdrpaLibrary-2.0/mdrpaLibrary.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-06 12:10:08.000000 mdrpaLibrary-2.0/mdrpaLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-06 12:10:08.000000 mdrpaLibrary-2.0/mdrpaLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-06 12:10:08.000000 mdrpaLibrary-2.0/mdrpaLibrary.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-06 12:10:08.702848 mdrpaLibrary-2.0/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-06 12:07:51.000000 mdrpaLibrary-2.0/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:10:09.868921 mdrpaLibrary-2.1/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-11 09:10:09.868752 mdrpaLibrary-2.1/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:10:09.867161 mdrpaLibrary-2.1/mdrpaLibrary/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:24:56.000000 mdrpaLibrary-2.1/mdrpaLibrary/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3325 2023-07-06 11:19:01.000000 mdrpaLibrary-2.1/mdrpaLibrary/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      529 2023-07-11 08:54:27.000000 mdrpaLibrary-2.1/mdrpaLibrary/getUiModels.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3352 2023-07-06 11:19:23.000000 mdrpaLibrary-2.1/mdrpaLibrary/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     1870 2023-07-11 09:08:10.000000 mdrpaLibrary-2.1/mdrpaLibrary/modelDrivenRpa.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3366 2023-07-06 11:20:06.000000 mdrpaLibrary-2.1/mdrpaLibrary/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3425 2023-07-06 11:20:26.000000 mdrpaLibrary-2.1/mdrpaLibrary/selectFromDropdownModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      863 2023-07-06 11:20:30.000000 mdrpaLibrary-2.1/mdrpaLibrary/sendReportModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:10:09.868393 mdrpaLibrary-2.1/mdrpaLibrary/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-2.1/mdrpaLibrary/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2350 2023-07-11 08:04:53.000000 mdrpaLibrary-2.1/mdrpaLibrary/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 09:10:09.868100 mdrpaLibrary-2.1/mdrpaLibrary.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-11 09:10:09.000000 mdrpaLibrary-2.1/mdrpaLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-11 09:10:09.000000 mdrpaLibrary-2.1/mdrpaLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-11 09:10:09.000000 mdrpaLibrary-2.1/mdrpaLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-11 09:10:09.000000 mdrpaLibrary-2.1/mdrpaLibrary.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-11 09:10:09.868971 mdrpaLibrary-2.1/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-11 09:09:13.000000 mdrpaLibrary-2.1/setup.py
```

### Comparing `mdrpaLibrary-2.0/mdrpaLibrary/clickButtonModel.robot` & `mdrpaLibrary-2.1/mdrpaLibrary/clickButtonModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.0/mdrpaLibrary/inputFieldModel.robot` & `mdrpaLibrary-2.1/mdrpaLibrary/inputFieldModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.0/mdrpaLibrary/modelDrivenRpa.py` & `mdrpaLibrary-2.1/mdrpaLibrary/modelDrivenRpa.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,18 @@
             'selectFromDropdownModel.robot',
             'getUiModels.robot',
             'sendReportModel.robot'
         ]  
 
     def import_resource_file(self, resource_file):
         file_path = os.path.join(self.resource_dir, resource_file)
-        if os.name == 'nt':  # Check if the platform is Windows
-          file_path = file_path.replace('/', '\\')  # Use backslash for Windows path separator
+        file_path = os.path.normpath(file_path)
         self.builtin.import_resource(file_path)
 
 
-
     @keyword
     def click_button_model(self, *args):
         self.import_resource_file(self.resource_files[0])  
         self.builtin.run_keyword('Click Button Model', *args)
 
     @keyword
     def input_field_model(self, *args):
```

### Comparing `mdrpaLibrary-2.0/mdrpaLibrary/selectCheckboxModel.robot` & `mdrpaLibrary-2.1/mdrpaLibrary/selectCheckboxModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.0/mdrpaLibrary/selectFromDropdownModel.robot` & `mdrpaLibrary-2.1/mdrpaLibrary/selectFromDropdownModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.0/mdrpaLibrary/sendReportModel.robot` & `mdrpaLibrary-2.1/mdrpaLibrary/sendReportModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.0/mdrpaLibrary/utils/utils.robot` & `mdrpaLibrary-2.1/mdrpaLibrary/utils/utils.robot`

 * *Files 7% similar despite different names*

```diff
@@ -29,45 +29,39 @@
 
 Set UI Element
     [Arguments]  ${model_name}   ${page_name}    ${element_name}   ${models}
     Set Suite Variable  ${model_name}
     Set Suite Variable  ${page_name}
     Set Suite Variable  ${element_name}
     ${model}=   Get Model From All Models   ${models}
-    log  ${model}
     ${page}=   Get Page From Model   ${model}
-    log  ${page}
     ${ui_element}=   Get Element From Model   ${page}
-    log  ${ui_element}
     [Return]    ${ui_element}
     
 Get Model From All Models
     [Arguments]   ${models}
     Set Suite Variable    ${return_model}    ${EMPTY}
     FOR    ${model}    IN    @{models}
         ${name}    Set Variable    ${model["application_name"]}
         Run Keyword If    '${name}' == '${model_name}'    Set Suite Variable    ${return_model}     ${model}
     END
-    log  ${return_model}
     [Return]    ${return_model}
 
 Get Page From Model
     [Arguments]   ${model}
     Set Suite Variable    ${return_page}    ${EMPTY}
     Set Suite Variable    ${pages}   ${model["pages"]} 
     FOR    ${page}    IN    @{pages}
         ${name}    Set Variable    ${page["page_name"]}
         Run Keyword If    '${name}' == '${page_name}'   Set Suite Variable    ${return_page}     ${page}
     END
-    log  ${return_page}
     [Return]    ${return_page}
     
 Get Element From Model
     [Arguments]   ${page}
     Set Suite Variable    ${return_element}    ${EMPTY}
     Set Suite Variable    ${elements}   ${page["ui_elements"]}  
     FOR    ${elem}    IN    @{elements}
         ${name}    Set Variable    ${elem["element_name"]}
         Run Keyword If    '${name}' == '${element_name}'   Set Suite Variable    ${return_element}     ${elem}  
     END
-    log  ${return_element}
     [Return]    ${return_element}
```

