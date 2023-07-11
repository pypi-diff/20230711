# Comparing `tmp/yaccounts-1.1.8.tar.gz` & `tmp/yaccounts-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaccounts-1.1.8.tar", last modified: Tue Jul 11 15:26:17 2023, max compression
+gzip compressed data, was "yaccounts-1.1.9.tar", last modified: Tue Jul 11 19:36:22 2023, max compression
```

## Comparing `yaccounts-1.1.8.tar` & `yaccounts-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:26:17.571589 yaccounts-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 15:26:17.567589 yaccounts-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:26:17.571589 yaccounts-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 15:25:53.000000 yaccounts-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:26:17.563589 yaccounts-1.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-11 15:25:53.000000 yaccounts-1.1.8/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:26:17.567589 yaccounts-1.1.8/yaccounts/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/operating_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/workbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-11 15:25:53.000000 yaccounts-1.1.8/yaccounts/worksheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:26:17.567589 yaccounts-1.1.8/yaccounts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 15:26:17.000000 yaccounts-1.1.8/yaccounts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-11 15:26:17.000000 yaccounts-1.1.8/yaccounts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:26:17.000000 yaccounts-1.1.8/yaccounts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 15:26:17.000000 yaccounts-1.1.8/yaccounts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 15:26:17.000000 yaccounts-1.1.8/yaccounts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:22.791805 yaccounts-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 19:36:22.791805 yaccounts-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:36:22.791805 yaccounts-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 19:35:56.000000 yaccounts-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:22.787805 yaccounts-1.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-11 19:35:56.000000 yaccounts-1.1.9/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:22.791805 yaccounts-1.1.9/yaccounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:35:56.000000 yaccounts-1.1.9/yaccounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-11 19:35:56.000000 yaccounts-1.1.9/yaccounts/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-11 19:35:56.000000 yaccounts-1.1.9/yaccounts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10672 2023-07-11 19:35:56.000000 yaccounts-1.1.9/yaccounts/operating_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 19:35:56.000000 yaccounts-1.1.9/yaccounts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-11 19:35:56.000000 yaccounts-1.1.9/yaccounts/workbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-11 19:35:56.000000 yaccounts-1.1.9/yaccounts/worksheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:22.791805 yaccounts-1.1.9/yaccounts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 19:36:22.000000 yaccounts-1.1.9/yaccounts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-11 19:36:22.000000 yaccounts-1.1.9/yaccounts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:36:22.000000 yaccounts-1.1.9/yaccounts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 19:36:22.000000 yaccounts-1.1.9/yaccounts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 19:36:22.000000 yaccounts-1.1.9/yaccounts.egg-info/top_level.txt
```

### Comparing `yaccounts-1.1.8/test/test.py` & `yaccounts-1.1.9/test/test.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.8/yaccounts/analyzer.py` & `yaccounts-1.1.9/yaccounts/analyzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import pathlib
 import pandas as pd
 import yaml
 
-from .config import CODES_IGNORED, COL_NAME_AMOUNT, all_expense_codes, all_handled_codes
+from .config import (
+    CODES_IGNORED,
+    COL_NAME_AMOUNT,
+    all_expense_codes,
+    all_handled_codes,
+    student_aid_expense_codes,
+)
 from .utils import filter_df_on_operating_units
 from .workbook import Workbook
 
 
 class CsvDataAnalyzer:
     def __init__(self, csv_path, split_notebooks=False, yml_config=None) -> None:
         self.csv_path = csv_path
@@ -70,26 +76,21 @@
 
     @classmethod
     def _add_operating_unit_with_options(cls, worksheet, operating_unit, name, options):
         worksheet.add_operating_unit(
             operating_unit,
             name,
             year=options["year"] if "year" in options else None,
-            student_aid=(
-                options["student_aid"][operating_unit]
-                if "student_aid" in options and operating_unit in options["student_aid"]
-                else None
-            ),
-            **{k: v for k, v in options.items() if k not in ("year", "student_aid")},
+            **{k: v for k, v in options.items() if k not in ("year",)},
         )
 
     def _get_default_options(self):
         return {
             "year": None,
-            "student_aid": {},
+            "student_aid": None,
             "budgeted_account": None,
             "hide_student_wages": False,
         }
 
     def _setup_workbooks_from_config(self):
         options = self._get_default_options()
 
@@ -176,7 +177,20 @@
         """Return the sum of expenditures for this year and all previous years"""
         return self.df[
             (self.df["Operating Unit"] == operating_unit)
             & (self.df["Fiscal Year"] <= year)
             & (self.df["JRNL Line Ledger"] == "ACTUALS")
             & (self.df["Account"].isin(all_expense_codes()))
         ][COL_NAME_AMOUNT].sum()
+
+    def get_previous_expenditures_student_aid(self, operating_unit, year, month):
+        """Return the sum of student aid expenditures up to and including the given month"""
+
+        return self.df[
+            (self.df["Operating Unit"] == operating_unit)
+            & (self.df["JRNL Line Ledger"] == "ACTUALS")
+            & (self.df["Account"].isin(student_aid_expense_codes()))
+            & (
+                (self.df["Fiscal Year"] < year)
+                | ((self.df["Fiscal Year"] == year) & (self.df["Accounting Period"] <= month))
+            )
+        ][COL_NAME_AMOUNT].sum()
```

### Comparing `yaccounts-1.1.8/yaccounts/config.py` & `yaccounts-1.1.9/yaccounts/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,28 +36,33 @@
 CODES_FACULTY_SPRING_SUMMER = (
     5920,  # Faculty Supplemental Benefits
     5260,  # Faculty Sal-Spr/Sum-Benefits
     5220,  # Faculty Sal-Spr/Sum No Ben
     5240,  # Faculty Sal-Supp (Overload)
 )
 
-CODES_TRAVEL = (
+CODES_TRAVEL_FACULTY = (
     6190,  # Employee Development/Training
     6400,  # Insurance Expense
     6494,  # Other Medical
     7000,  # Domestic-Business Travel
     7010,  # Domestic-Recruiting Travel
     7020,  # Domestic-Prof Developmt Travel
-    7030,  # Domestic-Student Travel
     7050,  # Foreign-Business Travel
     7060,  # Foreign-Recruiting Travel
     7070,  # Foreign-Prof Developmt Travel
+)
+
+CODES_TRAVEL_STUDENT = (
+    7030,  # Domestic-Student Travel
     7080,  # Foreign-Student Travel
 )
 
+CODES_TRAVEL = CODES_TRAVEL_FACULTY + CODES_TRAVEL_STUDENT
+
 CODES_SUPPLIES = (
     2200,  # Accrued Liabilities - Faculty computers?
     5980,  # Other Payroll Benefits
     6000,  # Software Acquisitions/Support
     6005,  # Software / Media Licenses
     6100,  # Supplies
     6109,  # Supplies (reclass)
@@ -155,9 +160,15 @@
         + CODES_TRAVEL
         + CODES_SUPPLIES
         + CODES_OVERHEAD
         + CODES_CAPITAL
     )
 
 
+def student_aid_expense_codes():
+    return (
+        CODES_STUDENT_WAGES + CODES_STUDENT_BENEFITS + CODES_STUDENT_TUITION + CODES_TRAVEL_STUDENT
+    )
+
+
 def all_handled_codes():
     return all_expense_codes() + CODES_INTEREST + CODES_IGNORED + CODES_INCOME
```

### Comparing `yaccounts-1.1.8/yaccounts/operating_unit.py` & `yaccounts-1.1.9/yaccounts/operating_unit.py`

 * *Files 8% similar despite different names*

```diff
@@ -170,38 +170,58 @@
         if color:
             self.row_colors[len(self.df_gen)] = color
 
         return self.df_gen.tail(1).index[0]
 
     def add_balance_row(self):
         if self.budgeted_account:
-            self.df_gen.loc[len(self.df_gen)] = {
+            prev_expenditures_row = len(self.df_gen)
+            self.df_gen.loc[prev_expenditures_row] = {
                 "Type": "Previous Expenditures",
                 calendar.month_abbr[1]: self.previous_expenditures,
             }
 
-        self.df_gen.loc[len(self.df_gen)] = {"Type": "Balance (end of month)"}
+        # Create student aid rows
+        if self.student_aid:
+            student_aid_row = len(self.df_gen)
+            self.df_gen.loc[student_aid_row, "Type"] = "Student aid"
+
+            non_student_aid_row = len(self.df_gen)
+            self.df_gen.loc[non_student_aid_row, "Type"] = "Non-student aid"
+
+        # Create balance row
+        balance_row = len(self.df_gen)
+        self.df_gen.loc[balance_row] = {"Type": "Balance (end of month)"}
 
         # # Iterate through columns and calcuate the balance, which is the total income minus the total expenses
         for month in range(1, 13):
             income = self.df_gen.iloc[self.row_total_income][month]
             expenses = self.df_gen.iloc[self.row_total_expenses][month]
 
             if month > 1:
-                prev_balance = self.df_gen.iloc[len(self.df_gen) - 1, month - 1]
+                prev_balance = self.df_gen.iloc[balance_row, month - 1]
             elif self.budgeted_account:
-                prev_balance = -self.df_gen.iloc[len(self.df_gen) - 2, month]
+                prev_balance = -self.df_gen.iloc[prev_expenditures_row, month]
             else:
                 prev_balance = 0
 
             balance = income - expenses + prev_balance
             self.df_gen.iloc[len(self.df_gen) - 1, month] = balance
             if month == 12:
                 self.balance = balance
 
+            # Fill in student aid balances
+            if self.student_aid:
+                student_expenses = self.analyzer.get_previous_expenditures_student_aid(
+                    self.operating_unit, self.year, month
+                )
+                student_aid_balance = self.student_aid - student_expenses
+                self.df_gen.iloc[student_aid_row, month] = student_aid_balance
+                self.df_gen.iloc[non_student_aid_row, month] = balance - student_aid_balance
+
         self.row_colors[len(self.df_gen)] = "yellow"
 
     def create_student_wages(self):
         # Filter to only student wages ('Account' column in STUDENT_WAGES)
         df_students = self.df[
             (self.df["Account"].isin(CODES_STUDENT_WAGES))
             & (self.df["JRNL Line Ledger"] == "ACTUALS")
```

### Comparing `yaccounts-1.1.8/yaccounts/workbook.py` & `yaccounts-1.1.9/yaccounts/workbook.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.8/yaccounts/worksheet.py` & `yaccounts-1.1.9/yaccounts/worksheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.next_start_row = 0
 
     def add_operating_unit(self, operating_unit, name=None, year=None, **options):
         if year is None:
             # Get all years for this operating unit from the dataframe
             years = sorted(
                 self.workbook.analyzer.df[
-                    self.workbook.analyzer.df["Operating Unit"] == operating_unit
+                    self.workbook.analyzer.df["Operating Unit"] == str(operating_unit)
                 ]["Fiscal Year"].unique()
             )
         else:
             years = ensure_tuple(year)
 
         for year in years:
             self.operating_units.append(
```

