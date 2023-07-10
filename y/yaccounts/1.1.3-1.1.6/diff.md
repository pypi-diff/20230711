# Comparing `tmp/yaccounts-1.1.3.tar.gz` & `tmp/yaccounts-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaccounts-1.1.3.tar", last modified: Mon Jul 10 21:17:42 2023, max compression
+gzip compressed data, was "yaccounts-1.1.6.tar", last modified: Mon Jul 10 22:37:10 2023, max compression
```

## Comparing `yaccounts-1.1.3.tar` & `yaccounts-1.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 21:17:42.596136 yaccounts-1.1.3/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-10 21:17:42.596136 yaccounts-1.1.3/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-10 21:17:42.596136 yaccounts-1.1.3/setup.cfg
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      395 2023-07-10 21:16:52.000000 yaccounts-1.1.3/setup.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 21:17:42.596136 yaccounts-1.1.3/test/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1199 2023-07-10 14:33:50.000000 yaccounts-1.1.3/test/test.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 21:17:42.596136 yaccounts-1.1.3/yaccounts/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-10 14:33:38.000000 yaccounts-1.1.3/yaccounts/__init__.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3628 2023-07-10 15:17:36.000000 yaccounts-1.1.3/yaccounts/analyzer.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     4702 2023-07-10 21:16:42.000000 yaccounts-1.1.3/yaccounts/config.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     9762 2023-07-10 15:17:36.000000 yaccounts-1.1.3/yaccounts/operating_unit.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      290 2023-07-10 14:33:38.000000 yaccounts-1.1.3/yaccounts/utils.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1097 2023-07-10 14:33:38.000000 yaccounts-1.1.3/yaccounts/workbook.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2683 2023-07-10 15:17:36.000000 yaccounts-1.1.3/yaccounts/worksheet.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-10 21:17:42.596136 yaccounts-1.1.3/yaccounts.egg-info/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-10 21:17:42.000000 yaccounts-1.1.3/yaccounts.egg-info/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      341 2023-07-10 21:17:42.000000 yaccounts-1.1.3/yaccounts.egg-info/SOURCES.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-07-10 21:17:42.000000 yaccounts-1.1.3/yaccounts.egg-info/dependency_links.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       45 2023-07-10 21:17:42.000000 yaccounts-1.1.3/yaccounts.egg-info/requires.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       10 2023-07-10 21:17:42.000000 yaccounts-1.1.3/yaccounts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:37:10.310799 yaccounts-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 22:37:10.310799 yaccounts-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 22:37:10.310799 yaccounts-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 22:36:48.000000 yaccounts-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:37:10.310799 yaccounts-1.1.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-10 22:36:48.000000 yaccounts-1.1.6/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:37:10.310799 yaccounts-1.1.6/yaccounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/operating_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/workbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-10 22:36:48.000000 yaccounts-1.1.6/yaccounts/worksheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:37:10.310799 yaccounts-1.1.6/yaccounts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-10 22:37:10.000000 yaccounts-1.1.6/yaccounts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-10 22:37:10.000000 yaccounts-1.1.6/yaccounts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:37:10.000000 yaccounts-1.1.6/yaccounts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 22:37:10.000000 yaccounts-1.1.6/yaccounts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 22:37:10.000000 yaccounts-1.1.6/yaccounts.egg-info/top_level.txt
```

### Comparing `yaccounts-1.1.3/test/test.py` & `yaccounts-1.1.6/test/test.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.3/yaccounts/analyzer.py` & `yaccounts-1.1.6/yaccounts/analyzer.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.3/yaccounts/config.py` & `yaccounts-1.1.6/yaccounts/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,140 +1,139 @@
 CODES_STUDENT_WAGES = (
-    5510, # Contracts: Student teaching assist salary
-    5599, # Contracts: Student Asst Salary (Reclass)
-    5572, # Contracts: Stdnt Research Assist Sal-FICA
-    5570, # Contracts: Student Research Assist Salary
-    5610, # Time Cards: Student Wages-Teaching Assist
-    5672, # Time Cards: Stdnt Wages Rsrch Assist-FICA
-    5600, # Time Cards: Student Wages
-    5602, # Time Cards: Student Wages-FICA
-    5720, # Non-Student Wages: Category 1 no Benefit
-    5750, # Non-Student Wages: Category 2 Part Benefit
-    8905, # Sponsored Research: Research Participant Stipends
-    5812, # ?
+    5510,  # Contracts: Student teaching assist salary
+    5599,  # Contracts: Student Asst Salary (Reclass)
+    5572,  # Contracts: Stdnt Research Assist Sal-FICA
+    5570,  # Contracts: Student Research Assist Salary
+    5610,  # Time Cards: Student Wages-Teaching Assist
+    5672,  # Time Cards: Stdnt Wages Rsrch Assist-FICA
+    5600,  # Time Cards: Student Wages
+    5602,  # Time Cards: Student Wages-FICA
+    5720,  # Non-Student Wages: Category 1 no Benefit
+    5750,  # Non-Student Wages: Category 2 Part Benefit
+    8905,  # Sponsored Research: Research Participant Stipends
+    5812,  # Payroll Incentives (Cell Phone Personal Use)
 )
 
 # These student benefits aren't attached to an individual student
 # name, so they must be separated out
 CODES_STUDENT_BENEFITS = (
-    5670, # Time Cards: Student Wages-Research Assist
-    5699, # Time Cards: Student Wages (Reclass)
-    5950, # Student Contract Benefits
-    5960, # Student Time Card Benefits
-    5970, # Non Student Benefits
-    5999, # Benefits (reclass)
+    5670,  # Time Cards: Student Wages-Research Assist
+    5699,  # Time Cards: Student Wages (Reclass)
+    5950,  # Student Contract Benefits
+    5960,  # Student Time Card Benefits
+    5970,  # Non Student Benefits
+    5999,  # Benefits (reclass)
 )
 
 CODES_STUDENT_TUITION = (
-    6300, # Scholarships
-    6303, # 
-    6304, # 
-    6309, # 
-    6319, # Student Aid (reclass) 
-    6390, # Other Student Aid
+    6300,  # Scholarships
+    6303,  # Graduate Tuition
+    6304,  # Graduate Cash Award
+    6309,  # Scholarships (reclass)
+    6319,  # Student Aid (reclass)
+    6390,  # Other Student Aid
 )
 
 CODES_FACULTY_SPRING_SUMMER = (
-    5920, # Faculty Supplemental Benefits
-    5260, # Faculty Sal-Spr/Sum-Benefits
-    5220, # Faculty Sal-Spr/Sum No Ben
-    5240, # Faculty Sal-Supp (Overload)
+    5920,  # Faculty Supplemental Benefits
+    5260,  # Faculty Sal-Spr/Sum-Benefits
+    5220,  # Faculty Sal-Spr/Sum No Ben
+    5240,  # Faculty Sal-Supp (Overload)
 )
 
 CODES_TRAVEL = (
-    6190, # Employee Development/Training
-    6400, # Insurance Expense
-    6494, # Other Medical
-    7000, # Domestic-Business Travel
-    7010, # Domestic-Recruiting Travel
-    7020, # Domestic-Prof Developmt Travel
-    7030, # Domestic-Student Travel
-    7050, # Foreign-Business Travel
-    7060, # Foreign-Recruiting Travel
-    7070, # Foreign-Prof Developmt Travel
-    7080, # Foreign-Student Travel
+    6190,  # Employee Development/Training
+    6400,  # Insurance Expense
+    6494,  # Other Medical
+    7000,  # Domestic-Business Travel
+    7010,  # Domestic-Recruiting Travel
+    7020,  # Domestic-Prof Developmt Travel
+    7030,  # Domestic-Student Travel
+    7050,  # Foreign-Business Travel
+    7060,  # Foreign-Recruiting Travel
+    7070,  # Foreign-Prof Developmt Travel
+    7080,  # Foreign-Student Travel
 )
 
 CODES_SUPPLIES = (
-    2200, #
-    5980, # Other Payroll Benefits
-    6000, # Software Acquisitions/Support
-    6005, # Software / Media Licenses
-    6100, # Supplies
-    6109, # Supplies (reclass)
-    6110, # Supplies-BYU Store
-    6120, # Printing and Copying
-    6125, # Research Publications Costs
-    6130, # Postage and Mailing
-    6140, # Telecommunications
-    6160, # Advertising and Promotion
-    6180, # Hosting, Food, Entertainment
-    6185, # Guest Tickets
-    6192, # Employee Memberships, Dues
-    6200, # Contract Service-Off Campus
-    6210, # Contract Services-Campus
-    6220, # Rental Expense - Intra Campus
-    6250, # Non-capital equipment
-    6255, # Non-Cap Access Equipment
-    6270, # Equipment Maintenance
-    6403, # Other Academic Payments
-    6405, # Prizes
-    6600, # Access Equipment
-    6610, # Access Lab Equipment
-    6480, # Legal Fees
-    6490, # Other Expense
-    6499, # Other Expense (reclass)
-    8940, # Conference Hosting (R-project)
+    2200,  # Accrued Liabilities - Faculty computers?
+    5980,  # Other Payroll Benefits
+    6000,  # Software Acquisitions/Support
+    6005,  # Software / Media Licenses
+    6100,  # Supplies
+    6109,  # Supplies (reclass)
+    6110,  # Supplies-BYU Store
+    6120,  # Printing and Copying
+    6125,  # Research Publications Costs
+    6130,  # Postage and Mailing
+    6140,  # Telecommunications
+    6160,  # Advertising and Promotion
+    6180,  # Hosting, Food, Entertainment
+    6185,  # Guest Tickets
+    6192,  # Employee Memberships, Dues
+    6200,  # Contract Service-Off Campus
+    6210,  # Contract Services-Campus
+    6220,  # Rental Expense - Intra Campus
+    6250,  # Non-capital equipment
+    6255,  # Non-Cap Access Equipment
+    6270,  # Equipment Maintenance
+    6403,  # Other Academic Payments
+    6405,  # Prizes
+    6600,  # Access Equipment
+    6610,  # Access Lab Equipment
+    6480,  # Legal Fees
+    6490,  # Other Expense
+    6499,  # Other Expense (reclass)
+    8940,  # Conference Hosting (R-project)
 )
 
 CODES_CAPITAL = (
-    1625, #
-    1725, # 
-    8930, # Research Capital Equipment
-    9126, # AM Retirement-Assets
-    9127, # AM Retirement-Accum Depr
-    9136, # AM Transfer-Assets
-    9137, # AM Tansfer-Accum Depr
+    1625,  # Capital Equipment
+    1725,  # AccDepre-Capital Equipment
+    8930,  # Research Capital Equipment
+    9126,  # AM Retirement-Assets
+    9127,  # AM Retirement-Accum Depr
+    9136,  # AM Transfer-Assets
+    9137,  # AM Tansfer-Accum Depr
 )
 
 CODES_OVERHEAD = (
-    8990, # Facilities & Admin Recovery
-    8991, # Waived Facilities & Admin Cost
-    8993, # Subcontract Facilities & Admin
+    8990,  # Facilities & Admin Recovery
+    8991,  # Waived Facilities & Admin Cost
+    8993,  # Subcontract Facilities & Admin
 )
 
 CODES_INTEREST = (
-    4711, # Interest Alloc-Claim on Cash
-    4719, # Non-Invest-Intrst Inc(reclass)
-    # These probably need to go to another location. They are put here temporarily
-    4755, # Distributed Royalty Income
-    4891, # Endowment Payout (UFS only)
+    4711,  # Interest Alloc-Claim on Cash
+    4719,  # Non-Invest-Intrst Inc(reclass)
 )
 
 # Income only applies to non-budgeted accounts
 CODES_INCOME = (
-    8920, # Subawards w/ F&A
-    8925, # Subawards w/out F&A
-    9250, # Transfer Into Net Assets
-    9260, # Transfer Out of Net Assets
-    3500, # 
+    3500,  # Beginning Net Assets
+    4755,  # Distributed Royalty Income
+    4891,  # Endowment Payout (UFS only)
+    8920,  # Subawards w/ F&A
+    8925,  # Subawards w/out F&A
+    9250,  # Transfer Into Net Assets
+    9260,  # Transfer Out of Net Assets
 )
 
 # Non-budgeted accounts, don't normally use BUDGET lines and they
 # can be removed, except for these codes
 CODES_NON_BUDGETED_BUDGET_CODES = (10,)
 
 # These codes aren't used by anything and can be removed from the data
 CODES_IGNORED = (
-    1010, #
-    1235, #
-    2000, #
-    2210, #
-    4200, # Gift Revenue-Cash
-    4220, # Grants & Contract Revenue
+    1010,  # Claim on Cash
+    1235,  # Sponsored Programs Receivable
+    2000,  # Accounts Payable
+    2210,  # Accrued Payroll-Biweekly
+    4200,  # Gift Revenue-Cash
+    4220,  # Grants & Contract Revenue
 )
 
 COL_NAME_AMOUNT = "JRNL Monetary Amount -no scrn aggregation"
 
 COLOR_STUDENT_WAGES = "rosybrown"
 COLOR_STUDENT_BENEFITS = "moccasin"
 COLOR_STUDENT_TUITION = "moccasin"
```

### Comparing `yaccounts-1.1.3/yaccounts/operating_unit.py` & `yaccounts-1.1.6/yaccounts/operating_unit.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.3/yaccounts/workbook.py` & `yaccounts-1.1.6/yaccounts/workbook.py`

 * *Files identical despite different names*

### Comparing `yaccounts-1.1.3/yaccounts/worksheet.py` & `yaccounts-1.1.6/yaccounts/worksheet.py`

 * *Files identical despite different names*

