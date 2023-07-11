# Comparing `tmp/cardo-python-utils-0.2.3.tar.gz` & `tmp/cardo-python-utils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardo-python-utils-0.2.3.tar", last modified: Mon Jul  3 15:47:26 2023, max compression
+gzip compressed data, was "cardo-python-utils-0.2.4.tar", last modified: Tue Jul 11 13:47:31 2023, max compression
```

## Comparing `cardo-python-utils-0.2.3.tar` & `cardo-python-utils-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-03 15:47:26.026253 cardo-python-utils-0.2.3/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/LICENSE
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/MANIFEST.in
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-07-03 15:47:26.026253 cardo-python-utils-0.2.3/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.3/README.rst
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-03 15:47:26.026253 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-07-03 15:47:26.000000 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2023-07-03 15:47:26.000000 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-07-03 15:47:26.000000 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2023-07-03 15:47:26.000000 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/requires.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2023-07-03 15:47:26.000000 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/top_level.txt
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-03 15:47:26.026253 cardo-python-utils-0.2.3/python_utils/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1949 2023-06-09 16:10:08.000000 cardo-python-utils-0.2.3/python_utils/choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/data_structures.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/db.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/django_utils.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    15143 2023-07-03 15:47:15.000000 cardo-python-utils-0.2.3/python_utils/esma_choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/exceptions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/imports.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/math.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/pandas_utils.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/rest.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/text.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/time.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/types_hinting.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2023-07-03 15:47:26.026253 cardo-python-utils-0.2.3/setup.cfg
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/setup.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-11 13:47:31.368748 cardo-python-utils-0.2.4/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/LICENSE
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/MANIFEST.in
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-07-11 13:47:31.368748 cardo-python-utils-0.2.4/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.4/README.rst
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-11 13:47:31.364748 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-07-11 13:47:31.000000 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2023-07-11 13:47:31.000000 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-07-11 13:47:31.000000 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2023-07-11 13:47:31.000000 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/requires.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2023-07-11 13:47:31.000000 cardo-python-utils-0.2.4/cardo_python_utils.egg-info/top_level.txt
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-11 13:47:31.368748 cardo-python-utils-0.2.4/python_utils/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2501 2023-07-11 13:35:59.000000 cardo-python-utils-0.2.4/python_utils/choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/data_structures.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/db.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/django_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16152 2023-07-11 13:44:06.000000 cardo-python-utils-0.2.4/python_utils/esma_choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/exceptions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/imports.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/math.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/pandas_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/rest.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/text.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/time.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/python_utils/types_hinting.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2023-07-11 13:47:31.368748 cardo-python-utils-0.2.4/setup.cfg
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.4/setup.py
```

### Comparing `cardo-python-utils-0.2.3/LICENSE` & `cardo-python-utils-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/PKG-INFO` & `cardo-python-utils-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cardo-python-utils-0.2.3/README.rst` & `cardo-python-utils-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/cardo_python_utils.egg-info/PKG-INFO` & `cardo-python-utils-0.2.4/cardo_python_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cardo-python-utils-0.2.3/cardo_python_utils.egg-info/SOURCES.txt` & `cardo-python-utils-0.2.4/cardo_python_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/python_utils/choices.py` & `cardo-python-utils-0.2.4/python_utils/choices.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,31 @@
     @classmethod
     @abstractmethod
     def list_as(cls, item_type):
         """List choices as"""
 
 
 class ChoiceEnumMeta(EnumMeta, IChoice, ABC):
+    def __new__(mcls, *args, **kwargs):
+        new_cls = super().__new__(mcls, *args, **kwargs)
+
+        # Make sure that the int values are unique
+        unique_values = set()
+        duplicate_values = set()
+        for el in new_cls.list_as(int):
+            if el in unique_values:
+                duplicate_values.add(str(el))
+            else:
+                unique_values.add(el)
+
+        if duplicate_values:
+            raise ValueError(f"Duplicate int values in {new_cls.__name__}: {', '.join(duplicate_values)}")
+
+        return new_cls
+
     def __contains__(cls, item: int | str) -> bool:
         if isinstance(item, int):
             member_values = [v.value[0] for v in cls.__members__.values()]
         elif isinstance(item, str):
             item = item.lower()
             member_values = [v.value[1].lower() for v in cls.__members__.values()]
         else:
```

### Comparing `cardo-python-utils-0.2.3/python_utils/data_structures.py` & `cardo-python-utils-0.2.4/python_utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/python_utils/django_utils.py` & `cardo-python-utils-0.2.4/python_utils/django_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/python_utils/esma_choices.py` & `cardo-python-utils-0.2.4/python_utils/esma_choices.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 """
 This module contains choices used also in ESMA reports.
 
 Choices structure:
-Example: GUAR = 40, "Guarantee"
-    GUAR -> ESMA code for the choice, to be used in reports
-    40 -> value stored in database
-    "Guarantee" -> human-readable name, used for display purposes
+Example: OVRD = 1, "Overdraft or Working Capital"
+    OVRD -> ESMA code for the choice, to be used in reports
+    1 -> value stored in database
+    "Overdraft or Working Capital" -> human-readable name, used for display purposes
+
+Exceptions:
+    There might be cases in which multiple choices are mapped to the same ESMA code.
+    In this case, some characters are added at the end of the ESMA code to differentiate it.
+    Example:
+        GUAR_G1 = 40, "Guarantee"
+        GUAR_G2 = 41, "Government Guarantee"
+    In such cases, only the part before the underscore (GUAR) (or the first 4 letters) is used in reports.
 """
 
 
 from python_utils.choices import ChoiceEnum
 
 
 class FinancialCreditAssetFinancingPurposeChoices(ChoiceEnum):
@@ -108,17 +116,36 @@
     EGAR = 2, "Enforcement of Guarantees"
     ALEN = 3, "Additional Lending"
     CASR = 4, "Cash Recoveries"
     MIXD = 5, "Mixed"
     OTHR = 10, "Other"
 
 
+class RealEstateAssetClassChoices(ChoiceEnum):
+    OTRE_R1 = 30, "Other Real Estate"
+    OTRE_R2 = 31, "Hospitality"
+    OTHR_R1 = 32, "Plot of land"
+    OTHR_R2 = 33, "Agricultural"
+    OTHR_R3 = 34, "Ancillary units"
+    CBLD_R1 = 35, "Retail"
+    CBLD_R2 = 36, "Office"
+    IBLD = 37, "Industrial"
+    RBLD = 38, "Residential"
+
+
+
 class GuaranteeAssetClassChoices(ChoiceEnum):
-    GUAR = 40, "Guarantee"
-    GOVG = 41, "Government Guarantee"
+    GUAR_G1 = 40, "Personal Guarantee"
+    GUAR_G2 = 41, "Government Guarantee"
+    GUAR_G3 = 42, "Bank Guarantee"
+    GUAR_G4 = 43, "Corporate Guarantee"
+    OTHR_G1 = 44, "Pledge on titles"
+    OTHR_G2 = 45, "Pledge on goods or inventory"
+    OTHR_G3 = 46, "Pledge on others"
+    OTHR_G4 = 47, "Patronage letter"
 
 
 class ESMAAccountStatusChoices(ChoiceEnum):
     PERF = 1, 'Performing'
     RNAR = 2, 'Restructured - No Arrears'
     RARR = 3, 'Restructured - Arrears'
     DFLT = 4, 'Defaulted according to Article 178 of Regulation (EU) No 575/2013'
```

### Comparing `cardo-python-utils-0.2.3/python_utils/exceptions.py` & `cardo-python-utils-0.2.4/python_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/python_utils/imports.py` & `cardo-python-utils-0.2.4/python_utils/imports.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/python_utils/math.py` & `cardo-python-utils-0.2.4/python_utils/math.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/python_utils/pandas_utils.py` & `cardo-python-utils-0.2.4/python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/python_utils/rest.py` & `cardo-python-utils-0.2.4/python_utils/rest.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/python_utils/text.py` & `cardo-python-utils-0.2.4/python_utils/text.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/python_utils/time.py` & `cardo-python-utils-0.2.4/python_utils/time.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.3/setup.cfg` & `cardo-python-utils-0.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardo-python-utils
-version = 0.2.3
+version = 0.2.4
 description = Python library enhanced with a wide range of functions for different scenarios.
 long_description = file: README.rst
 url = https://github.com/CardoAI/cardo-python-utils
 author = Kristi Kotini
 author_email = hello@cardoai.com
 license = MIT (X11)
 classifiers =
```

