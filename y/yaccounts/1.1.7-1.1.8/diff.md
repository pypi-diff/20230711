# Comparing `tmp/yaccounts-1.1.7.tar.gz` & `tmp/yaccounts-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaccounts-1.1.7.tar", last modified: Tue Jul 11 04:09:10 2023, max compression
+gzip compressed data, was "yaccounts-1.1.8.tar", last modified: Tue Jul 11 15:26:17 2023, max compression
```

## Comparing `yaccounts-1.1.7.tar` & `yaccounts-1.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:09:10.365062 yaccounts-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 04:09:10.365062 yaccounts-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:09:10.365062 yaccounts-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 04:08:48.000000 yaccounts-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:09:10.365062 yaccounts-1.1.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-11 04:08:48.000000 yaccounts-1.1.7/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:09:10.365062 yaccounts-1.1.7/yaccounts/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/operating_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/workbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-11 04:08:48.000000 yaccounts-1.1.7/yaccounts/worksheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:09:10.365062 yaccounts-1.1.7/yaccounts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 04:09:10.000000 yaccounts-1.1.7/yaccounts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-11 04:09:10.000000 yaccounts-1.1.7/yaccounts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:09:10.000000 yaccounts-1.1.7/yaccounts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 04:09:10.000000 yaccounts-1.1.7/yaccounts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 04:09:10.000000 yaccounts-1.1.7/yaccounts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:26:17.571589 yaccounts-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 15:26:17.567589 yaccounts-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:26:17.571589 yaccounts-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 15:25:53.000000 yaccounts-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:26:17.563589 yaccounts-1.1.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-11 15:25:53.000000 yaccounts-1.1.8/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:26:17.567589 yaccounts-1.1.8/yaccounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/operating_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/workbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/worksheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:26:17.567589 yaccounts-1.1.8/yaccounts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 15:26:17.000000 yaccounts-1.1.8/yaccounts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-11 15:26:17.000000 yaccounts-1.1.8/yaccounts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:26:17.000000 yaccounts-1.1.8/yaccounts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 15:26:17.000000 yaccounts-1.1.8/yaccounts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 15:26:17.000000 yaccounts-1.1.8/yaccounts.egg-info/top_level.txt
```

### Comparing `yaccounts-1.1.7/test/test.py` & `yaccounts-1.1.8/test/test.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.7/yaccounts/config.py` & `yaccounts-1.1.8/yaccounts/config.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.7/yaccounts/operating_unit.py` & `yaccounts-1.1.8/yaccounts/operating_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,46 +13,44 @@
     def __init__(
         self,
         worksheet,
         operating_unit,
         year,
         name=None,
         budgeted_account=None,
+        student_aid=None,
+        hide_student_wages=False,
     ) -> None:
         self.worksheet = worksheet
         self.operating_unit = str(operating_unit)
         self.name = name
         self.year = year
+        self.student_aid = student_aid
+        self.hide_student_wages = hide_student_wages
 
         if budgeted_account is None:
-            self.budgeted_account = operating_unit.startswith("R")
+            self.budgeted_account = self.operating_unit.startswith("R")
         else:
             self.budgeted_account = budgeted_account
 
         # Create a new dataframe with months of the year as column headers
         self.df_gen = pd.DataFrame(
             columns=("Type", *[calendar.month_abbr[i] for i in range(1, 13)])
         )
 
         self.row_colors = {}
         self.hidden_rows = []
 
-        # Default options
-        self.set_options()
-
         self.df = None
 
         if self.budgeted_account:
             self.previous_expenditures = self.analyzer.get_previous_expenditures(
                 self.operating_unit, self.year - 1
             )
 
-    def set_options(self, hide_student_wages=False):
-        self.hide_student_wages = hide_student_wages
-
     def run(self, df):
         self.df = df
         if self.year:
             # Filter df on 'Fiscal Year' column
             self.df = self.df[self.df["Fiscal Year"] == self.year]
 
         if self.budgeted_account:
```

### Comparing `yaccounts-1.1.7/yaccounts/workbook.py` & `yaccounts-1.1.8/yaccounts/workbook.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.7/yaccounts/worksheet.py` & `yaccounts-1.1.8/yaccounts/worksheet.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 class Worksheet:
     def __init__(self, workbook, sheet) -> None:
         self.workbook = workbook
         self.operating_units = []
         self.sheet = sheet
         self.next_start_row = 0
 
-    def add_operating_unit(self, operating_unit, name=None, year=None):
+    def add_operating_unit(self, operating_unit, name=None, year=None, **options):
         if year is None:
             # Get all years for this operating unit from the dataframe
             years = sorted(
                 self.workbook.analyzer.df[
                     self.workbook.analyzer.df["Operating Unit"] == operating_unit
                 ]["Fiscal Year"].unique()
             )
         else:
             years = ensure_tuple(year)
 
         for year in years:
-            self.operating_units.append(OperatingUnit(self, operating_unit, year, name=name))
+            self.operating_units.append(
+                OperatingUnit(self, operating_unit, year, name=name, **options)
+            )
 
     def format_cell(self, row, col, format):
         self.sheet.conditional_format(row, col, row, col, {"type": "no_errors", "format": format})
 
     def format_row(self, row, format):
         self.sheet.conditional_format(row, 0, row, 13, {"type": "no_errors", "format": format})
         #     sheet.write_blank(row, i, sheet[row, i].value, color)
```

