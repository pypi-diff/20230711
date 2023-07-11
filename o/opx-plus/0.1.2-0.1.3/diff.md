# Comparing `tmp/opx_plus-0.1.2.tar.gz` & `tmp/opx_plus-0.1.3.tar.gz`

## Comparing `opx_plus-0.1.2.tar` & `opx_plus-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.DS_Store
--rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 opx_plus-0.1.2/opx_plus.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 opx_plus-0.1.2/requirements.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 opx_plus-0.1.2/top_level.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/.gitignore
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/OPX_Plus.iml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/vcs.xml
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opx_plus-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opx_plus-0.1.2/src/__init__.py
--rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 opx_plus-0.1.2/src/opx_plus.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 opx_plus-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 opx_plus-0.1.2/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 opx_plus-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 opx_plus-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 opx_plus-0.1.3/.DS_Store
+-rw-r--r--   0        0        0    10750 2020-02-02 00:00:00.000000 opx_plus-0.1.3/opx_plus.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 opx_plus-0.1.3/requirements.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 opx_plus-0.1.3/top_level.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 opx_plus-0.1.3/.idea/.gitignore
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 opx_plus-0.1.3/.idea/OPX_Plus.iml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 opx_plus-0.1.3/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 opx_plus-0.1.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opx_plus-0.1.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 opx_plus-0.1.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opx_plus-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opx_plus-0.1.3/src/__init__.py
+-rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 opx_plus-0.1.3/src/opx_plus.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 opx_plus-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 opx_plus-0.1.3/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 opx_plus-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 opx_plus-0.1.3/PKG-INFO
```

### Comparing `opx_plus-0.1.2/.DS_Store` & `opx_plus-0.1.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.2/opx_plus.py` & `opx_plus-0.1.3/src/opx_plus.py`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.2/.idea/workspace.xml` & `opx_plus-0.1.3/.idea/workspace.xml`

 * *Files 8% similar despite different names*

#### Comparing `opx_plus-0.1.2/.idea/workspace.xml` & `opx_plus-0.1.3/.idea/workspace.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="e970cb05-7d56-441a-b2e6-7549de815664" name="Changes" comment="trying some suggestions from jeffrey to make the module install proerply..">
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/opx_plus.py" beforeDir="false" afterPath="$PROJECT_DIR$/opx_plus.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
@@ -22,22 +24,23 @@
   <component name="ProjectLevelVcsManager" settingsEditedManually="true">
     <ConfirmationsSetting value="2" id="Add"/>
   </component>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "ASKED_ADD_EXTERNAL_FILES": "true",
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "last_opened_file_path": "/Users/stevenwilson/PycharmProjects/opx_plus"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;ASKED_ADD_EXTERNAL_FILES&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/Users/stevenwilson/PycharmProjects/opx_plus&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$"/>
     </key>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
```

### Comparing `opx_plus-0.1.2/src/opx_plus.py` & `opx_plus-0.1.3/opx_plus.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,33 +82,37 @@
         print("------------------")
         quit()
     else:
         print("All mandatory files found")
         print("------------------")
 
 
-def open_template(template_path: object, *date_cells: str) -> object:
+def open_template(template_path: object, *date_cells: str, previous_day=False) -> object:
     wb = openpyxl.load_workbook(template_path)
     ws = wb[wb.sheetnames[0]]
     print(f'Opened "{ws.title}" from "{template_path.split("/")[-1]}"')
-    today_date = datetime.date.today()
+
+    if previous_day:
+        today_date = datetime.date.today() - datetime.timedelta(days=1)
+    else:
+        today_date = datetime.date.today()
 
     for cell in date_cells:
         ws[cell] = today_date
         print(f"cell {cell} updated with today's date")
     return wb, ws
 
 
-def save_file(new_file_location, file_name, workbook, afterdatetext="", previousday=False):
-    if afterdatetext != "":
-        afterdatetext = " " + afterdatetext
-    if previousday:
-        new_file_path = f'{new_file_location}{file_name} {datetime.date.today() - datetime.timedelta(days=1)}{afterdatetext}.xlsx'
+def save_file(new_file_location, file_name, workbook, after_date_text="", previous_day=False):
+    if after_date_text != "":
+        after_date_text = " " + after_date_text
+    if previous_day:
+        new_file_path = f'{new_file_location}{file_name} {datetime.date.today() - datetime.timedelta(days=1)}{after_date_text}.xlsx'
     else:
-        new_file_path = f'{new_file_location}{file_name} {datetime.date.today()}{afterdatetext}.xlsx'
+        new_file_path = f'{new_file_location}{file_name} {datetime.date.today()}{after_date_text}.xlsx'
     workbook.save(new_file_path)
     print(f'saved at: {new_file_path}')
     print(f"Opening {new_file_path.split('/')[-1]}")
     print("------------------")
     new_file_path = f'"{new_file_path}"'
     os.system("open " + new_file_path)
 
@@ -165,14 +169,36 @@
                 to_sheet[f'{column_letter}{row_index + row_incrementer}'].value = s
     if include_header:
         print(f'C&Ped VALUE & HEADERs from {csv_path.split("/")[-1]} to "{to_sheet.title}"')
     else:
         print(f'C&Ped VALUEs from {csv_path.split("/")[-1]} to "{to_sheet.title}"')
 
 
+def paste_df_to_sheet(df, to_sheet, include_header=False):
+    data = df.values.tolist()
+    if include_header:
+        data = [df.columns.tolist()] + data
+
+    row_incrementer = 1
+    if not include_header:
+        data = data[1:]
+        row_incrementer += 1
+
+    for row_index, row in enumerate(data):
+        for column_index, cell in enumerate(row):
+            column_letter = openpyxl.utils.get_column_letter(column_index + 1)
+            s = cell
+            if s is not None:
+                try:
+                    s = float(s)
+                except ValueError:
+                    pass
+            to_sheet[f'{column_letter}{row_index + row_incrementer}'].value = s
+
+
 def copy_over_and_down_formulas(from_ws, to_ws, formula_cells):
     for row in openpyxl.utils.rows_from_range(formula_cells):
         c_list = []
         for cell in row:
             c_list.append(cell.rstrip('1234567890'))
             to_ws[cell].value = from_ws[cell].value
     # drag down formulas
```

### Comparing `opx_plus-0.1.2/LICENSE.txt` & `opx_plus-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.2/README.md` & `opx_plus-0.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -5,42 +5,46 @@
 ### Has the Following Dependencies
 ```
 import openpyxl, glob, webbrowser, warnings, csv, datetime, os, time
 from copy import copy
 from openpyxl.formula.translate import Translator
 ```
 
-## Additional Functions
+## Functions
 ### Files
 ```
-get_file_path(file_path, name_search, *if_missing_urls)
-check_mandatory_files(f_list)
+- get_file_path(file_path, name_search, *if_missing_urls)
+- check_mandatory_files(f_list)
 
-0pen_template(template_path: object, *date_cells: str)
-open_vals_only_sheet(from_wb_path, sheet_id=0)
+- open_template(template_path: object, *date_cells: str, previousday=False)
+- save_file(new_file_location, file_name, workbook, afterdatetext="", previousday=False)
+- remove(file_path)
 
-save_file(new_file_location, file_name, workbook, afterdatetext="", previousday=False)
-remove(file_path)
 ```
-### Move Data
+### Import Data
+```
+- open_vals_only_sheet(from_wb_path, sheet_id=0):
+- paste_sheet_to_sheet(from_ws, to_ws, cell_range)
+- paste_csv_vals_to_sheet(csv_path, to_sheet, include_header=False)
+- paste_df_to_sheet(df, to_sheet, include_header=False)
 ```
-paste_sheet_to_sheet(from_ws, to_ws, cell_range)
-paste_csv_vals_to_sheet(csv_path, to_sheet, include_header=False)
 
-copy_over_and_down_formulas(from_ws, to_ws, formula_cells)
-paste_cells_to_cells(from_ws, to_ws, from_cell_range, offset=(0, 0))
+### Move Data
+```
+- copy_over_and_down_formulas(from_ws, to_ws, formula_cells)
+- paste_cells_to_cells(from_ws, to_ws, from_cell_range, offset=(0, 0))
 ```
 
 ### Sub-Functions
 ```
-count_rows(worksheet)
-num_to_excel_col(n)
-excel_col_to_num(a)
+- count_rows(worksheet)
+- num_to_excel_col(n)
+- excel_col_to_num(a)
 
-to_unix_time(year=datetime.datetime.now().year, month=datetime.datetime.now().month,
+- to_unix_time(year=datetime.datetime.now().year, month=datetime.datetime.now().month,
                  day=datetime.datetime.now().day, hour=datetime.datetime.now().hour,
                  minute=datetime.datetime.now().minute, second=datetime.datetime.now().second, add_3_zeros=False,
                  subtract=datetime.timedelta(0))
-date_ranger()
-worksheet_reset(sheet_nam, wb)
+- date_ranger()
+- worksheet_reset(sheet_nam, wb)
 ```
```

### Comparing `opx_plus-0.1.2/pyproject.toml` & `opx_plus-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "opx_plus"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Steven Wilson", github="https://github.com/StevenWilson9" },
 ]
 description = "Adds additional functionality on top of OpenPyXL"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `opx_plus-0.1.2/PKG-INFO` & `opx_plus-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opx_plus
-Version: 0.1.2
+Version: 0.1.3
 Summary: Adds additional functionality on top of OpenPyXL
 Project-URL: Homepage, https://github.com/StevenWilson9/OPX_Plus
 Project-URL: Bug Tracker, https://github.com/StevenWilson9/OPX_Plus/issues
 Author: Steven Wilson
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,42 +20,46 @@
 ### Has the Following Dependencies
 ```
 import openpyxl, glob, webbrowser, warnings, csv, datetime, os, time
 from copy import copy
 from openpyxl.formula.translate import Translator
 ```
 
-## Additional Functions
+## Functions
 ### Files
 ```
-get_file_path(file_path, name_search, *if_missing_urls)
-check_mandatory_files(f_list)
+- get_file_path(file_path, name_search, *if_missing_urls)
+- check_mandatory_files(f_list)
 
-0pen_template(template_path: object, *date_cells: str)
-open_vals_only_sheet(from_wb_path, sheet_id=0)
+- open_template(template_path: object, *date_cells: str, previousday=False)
+- save_file(new_file_location, file_name, workbook, afterdatetext="", previousday=False)
+- remove(file_path)
 
-save_file(new_file_location, file_name, workbook, afterdatetext="", previousday=False)
-remove(file_path)
 ```
-### Move Data
+### Import Data
+```
+- open_vals_only_sheet(from_wb_path, sheet_id=0):
+- paste_sheet_to_sheet(from_ws, to_ws, cell_range)
+- paste_csv_vals_to_sheet(csv_path, to_sheet, include_header=False)
+- paste_df_to_sheet(df, to_sheet, include_header=False)
 ```
-paste_sheet_to_sheet(from_ws, to_ws, cell_range)
-paste_csv_vals_to_sheet(csv_path, to_sheet, include_header=False)
 
-copy_over_and_down_formulas(from_ws, to_ws, formula_cells)
-paste_cells_to_cells(from_ws, to_ws, from_cell_range, offset=(0, 0))
+### Move Data
+```
+- copy_over_and_down_formulas(from_ws, to_ws, formula_cells)
+- paste_cells_to_cells(from_ws, to_ws, from_cell_range, offset=(0, 0))
 ```
 
 ### Sub-Functions
 ```
-count_rows(worksheet)
-num_to_excel_col(n)
-excel_col_to_num(a)
+- count_rows(worksheet)
+- num_to_excel_col(n)
+- excel_col_to_num(a)
 
-to_unix_time(year=datetime.datetime.now().year, month=datetime.datetime.now().month,
+- to_unix_time(year=datetime.datetime.now().year, month=datetime.datetime.now().month,
                  day=datetime.datetime.now().day, hour=datetime.datetime.now().hour,
                  minute=datetime.datetime.now().minute, second=datetime.datetime.now().second, add_3_zeros=False,
                  subtract=datetime.timedelta(0))
-date_ranger()
-worksheet_reset(sheet_nam, wb)
+- date_ranger()
+- worksheet_reset(sheet_nam, wb)
 ```
```

