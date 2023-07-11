# Comparing `tmp/Iretax-0.0.2.tar.gz` & `tmp/iretax-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Iretax-0.0.2.tar", last modified: Tue Jul 11 07:27:46 2023, max compression
+gzip compressed data, was "iretax-0.0.3.tar", last modified: Tue Jul 11 07:36:16 2023, max compression
```

## Comparing `Iretax-0.0.2.tar` & `iretax-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 07:27:46.522438 Iretax-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-10 16:57:31.000000 Iretax-0.0.2/LICENSE
--rw-rw-rw-   0        0        0    12292 2023-07-11 07:27:46.520318 Iretax-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    11777 2023-07-11 07:26:05.000000 Iretax-0.0.2/README.md
--rw-rw-rw-   0        0        0      601 2023-07-11 07:25:58.000000 Iretax-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 07:27:46.522438 Iretax-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 07:27:46.406406 Iretax-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 07:27:46.503435 Iretax-0.0.2/src/Iretax.egg-info/
--rw-rw-rw-   0        0        0    12292 2023-07-11 07:27:46.000000 Iretax-0.0.2/src/Iretax.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-07-11 07:27:46.000000 Iretax-0.0.2/src/Iretax.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 07:27:46.000000 Iretax-0.0.2/src/Iretax.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 07:27:46.000000 Iretax-0.0.2/src/Iretax.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 07:27:46.508421 Iretax-0.0.2/src/iretax/
--rw-rw-rw-   0        0        0       92 2023-07-10 08:47:50.000000 Iretax-0.0.2/src/iretax/__init__.py
--rw-rw-rw-   0        0        0     2918 2023-07-10 08:44:23.000000 Iretax-0.0.2/src/iretax/rebate_calculator.py
--rw-rw-rw-   0        0        0     2172 2023-07-10 16:31:46.000000 Iretax-0.0.2/src/iretax/tax_calculator.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:27:46.518720 Iretax-0.0.2/tests/
--rw-rw-rw-   0        0        0     1105 2023-07-10 09:47:29.000000 Iretax-0.0.2/tests/test_rebate_calculator.py
--rw-rw-rw-   0        0        0     1083 2023-07-10 16:36:53.000000 Iretax-0.0.2/tests/test_tax_calculator.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:36:16.985349 iretax-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-10 16:57:31.000000 iretax-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0    12292 2023-07-11 07:36:16.983346 iretax-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11777 2023-07-11 07:31:01.000000 iretax-0.0.3/README.md
+-rw-rw-rw-   0        0        0      601 2023-07-11 07:35:15.000000 iretax-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 07:36:16.986347 iretax-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 07:36:16.932428 iretax-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 07:36:16.973344 iretax-0.0.3/src/Iretax.egg-info/
+-rw-rw-rw-   0        0        0    12292 2023-07-11 07:36:16.000000 iretax-0.0.3/src/Iretax.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-07-11 07:36:16.000000 iretax-0.0.3/src/Iretax.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 07:36:16.000000 iretax-0.0.3/src/Iretax.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 07:36:16.000000 iretax-0.0.3/src/Iretax.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 07:36:16.978346 iretax-0.0.3/src/iretax/
+-rw-rw-rw-   0        0        0       92 2023-07-10 08:47:50.000000 iretax-0.0.3/src/iretax/__init__.py
+-rw-rw-rw-   0        0        0     2918 2023-07-10 08:44:23.000000 iretax-0.0.3/src/iretax/rebate_calculator.py
+-rw-rw-rw-   0        0        0     2172 2023-07-10 16:31:46.000000 iretax-0.0.3/src/iretax/tax_calculator.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:36:16.981345 iretax-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1105 2023-07-10 09:47:29.000000 iretax-0.0.3/tests/test_rebate_calculator.py
+-rw-rw-rw-   0        0        0     1083 2023-07-10 16:36:53.000000 iretax-0.0.3/tests/test_tax_calculator.py
```

### Comparing `Iretax-0.0.2/LICENSE` & `iretax-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Iretax-0.0.2/PKG-INFO` & `iretax-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
-Name: Iretax
-Version: 0.0.2
+Name: iretax
+Version: 0.0.3
 Summary: A Tax Calculation and Rebate System
 Author-email: Shubham Goswami <goswamis@tcd.ie>
 Project-URL: Homepage, https://github.com/ShubhZ33/iretax
 Project-URL: Bug Tracker, https://github.com/ShubhZ33/iretax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iretax
-Iretax
+iretax
 
 iretax is a Python-based library designed specifically for the Ireland tax system. It serves as a comprehensive tool for individuals, tax professionals, and software developers in Ireland seeking a reliable, easy-to-use solution for tax-related computations for the 2023 tax year.
 
 The iretax library provides a simplified approach to calculating taxes and rebates in Ireland. It features two main components: TaxCalculator and RebateCalculator. The TaxCalculator class offers functionality to calculate taxes based on factors such as income and marital status, aligning with the 2023 tax brackets and rates. The RebateCalculator class aids users in determining the applicable tax rebates, encompassing various eligibility codes specific to the Ireland tax system.
 
-The advantage of using iRetax is that it converts complex tax calculations into a few straightforward function calls. This accessibility makes tax calculations comprehensible to everyone, while ensuring accuracy and adherence to the current Irish tax codes, thereby minimizing potential errors in manual calculations.
+The advantage of using iretax is that it converts complex tax calculations into a few straightforward function calls. This accessibility makes tax calculations comprehensible to everyone, while ensuring accuracy and adherence to the current Irish tax codes, thereby minimizing potential errors in manual calculations.
 
 
 
 ## Installation
 
 The iretax package can be easily installed from TestPyPI by running the following command:
```

### Comparing `Iretax-0.0.2/README.md` & `iretax-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # iretax
-Iretax
+iretax
 
 iretax is a Python-based library designed specifically for the Ireland tax system. It serves as a comprehensive tool for individuals, tax professionals, and software developers in Ireland seeking a reliable, easy-to-use solution for tax-related computations for the 2023 tax year.
 
 The iretax library provides a simplified approach to calculating taxes and rebates in Ireland. It features two main components: TaxCalculator and RebateCalculator. The TaxCalculator class offers functionality to calculate taxes based on factors such as income and marital status, aligning with the 2023 tax brackets and rates. The RebateCalculator class aids users in determining the applicable tax rebates, encompassing various eligibility codes specific to the Ireland tax system.
 
-The advantage of using iRetax is that it converts complex tax calculations into a few straightforward function calls. This accessibility makes tax calculations comprehensible to everyone, while ensuring accuracy and adherence to the current Irish tax codes, thereby minimizing potential errors in manual calculations.
+The advantage of using iretax is that it converts complex tax calculations into a few straightforward function calls. This accessibility makes tax calculations comprehensible to everyone, while ensuring accuracy and adherence to the current Irish tax codes, thereby minimizing potential errors in manual calculations.
 
 
 
 ## Installation
 
 The iretax package can be easily installed from TestPyPI by running the following command:
```

### Comparing `Iretax-0.0.2/pyproject.toml` & `iretax-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "Iretax"
-version = "0.0.2"
+name = "iretax"
+version = "0.0.3"
 authors = [
   { name="Shubham Goswami", email="goswamis@tcd.ie" },
 ]
 description = "A Tax Calculation and Rebate System"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `Iretax-0.0.2/src/Iretax.egg-info/PKG-INFO` & `iretax-0.0.3/src/Iretax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
-Name: Iretax
-Version: 0.0.2
+Name: iretax
+Version: 0.0.3
 Summary: A Tax Calculation and Rebate System
 Author-email: Shubham Goswami <goswamis@tcd.ie>
 Project-URL: Homepage, https://github.com/ShubhZ33/iretax
 Project-URL: Bug Tracker, https://github.com/ShubhZ33/iretax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iretax
-Iretax
+iretax
 
 iretax is a Python-based library designed specifically for the Ireland tax system. It serves as a comprehensive tool for individuals, tax professionals, and software developers in Ireland seeking a reliable, easy-to-use solution for tax-related computations for the 2023 tax year.
 
 The iretax library provides a simplified approach to calculating taxes and rebates in Ireland. It features two main components: TaxCalculator and RebateCalculator. The TaxCalculator class offers functionality to calculate taxes based on factors such as income and marital status, aligning with the 2023 tax brackets and rates. The RebateCalculator class aids users in determining the applicable tax rebates, encompassing various eligibility codes specific to the Ireland tax system.
 
-The advantage of using iRetax is that it converts complex tax calculations into a few straightforward function calls. This accessibility makes tax calculations comprehensible to everyone, while ensuring accuracy and adherence to the current Irish tax codes, thereby minimizing potential errors in manual calculations.
+The advantage of using iretax is that it converts complex tax calculations into a few straightforward function calls. This accessibility makes tax calculations comprehensible to everyone, while ensuring accuracy and adherence to the current Irish tax codes, thereby minimizing potential errors in manual calculations.
 
 
 
 ## Installation
 
 The iretax package can be easily installed from TestPyPI by running the following command:
```

### Comparing `Iretax-0.0.2/src/iretax/rebate_calculator.py` & `iretax-0.0.3/src/iretax/rebate_calculator.py`

 * *Files identical despite different names*

### Comparing `Iretax-0.0.2/src/iretax/tax_calculator.py` & `iretax-0.0.3/src/iretax/tax_calculator.py`

 * *Files identical despite different names*

### Comparing `Iretax-0.0.2/tests/test_rebate_calculator.py` & `iretax-0.0.3/tests/test_rebate_calculator.py`

 * *Files identical despite different names*

### Comparing `Iretax-0.0.2/tests/test_tax_calculator.py` & `iretax-0.0.3/tests/test_tax_calculator.py`

 * *Files identical despite different names*

