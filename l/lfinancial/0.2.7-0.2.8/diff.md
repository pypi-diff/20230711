# Comparing `tmp/lfinancial-0.2.7.tar.gz` & `tmp/lfinancial-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.2.7.tar", last modified: Tue Jul 11 08:39:18 2023, max compression
+gzip compressed data, was "lfinancial-0.2.8.tar", last modified: Tue Jul 11 14:39:17 2023, max compression
```

## Comparing `lfinancial-0.2.7.tar` & `lfinancial-0.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:39:18.538564 lfinancial-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-11 08:38:57.000000 lfinancial-0.2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-11 08:39:18.538564 lfinancial-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 08:38:57.000000 lfinancial-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:39:18.534564 lfinancial-0.2.7/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:39:18.538564 lfinancial-0.2.7/lfinancial/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/contry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/timezone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:39:18.534564 lfinancial-0.2.7/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-11 08:39:18.000000 lfinancial-0.2.7/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-11 08:39:18.000000 lfinancial-0.2.7/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:39:18.000000 lfinancial-0.2.7/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 08:39:18.000000 lfinancial-0.2.7/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 08:39:18.538564 lfinancial-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-11 08:38:57.000000 lfinancial-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:39:18.538564 lfinancial-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 08:38:57.000000 lfinancial-0.2.7/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:17.766598 lfinancial-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-11 14:39:00.000000 lfinancial-0.2.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-11 14:39:17.766598 lfinancial-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 14:39:00.000000 lfinancial-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:17.762598 lfinancial-0.2.8/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:17.766598 lfinancial-0.2.8/lfinancial/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/contry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/timezone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:17.762598 lfinancial-0.2.8/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-11 14:39:17.000000 lfinancial-0.2.8/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-11 14:39:17.000000 lfinancial-0.2.8/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:39:17.000000 lfinancial-0.2.8/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 14:39:17.000000 lfinancial-0.2.8/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:39:17.766598 lfinancial-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-11 14:39:00.000000 lfinancial-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:17.766598 lfinancial-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 14:39:00.000000 lfinancial-0.2.8/tests/test_document.py
```

### Comparing `lfinancial-0.2.7/LICENSE.txt` & `lfinancial-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/PKG-INFO` & `lfinancial-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.7
+Version: 0.2.8
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lfinancial-0.2.7/README.md` & `lfinancial-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/factory.py` & `lfinancial-0.2.8/lfinancial/factory.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/financial.py` & `lfinancial-0.2.8/lfinancial/financial.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 from lfinancial.factory import GeneratorFactory
 
 
 class Financial:
     def __init__(self):
         self._generator_factory = GeneratorFactory()
 
-    def __generate(self, generator_name, country):
+    def _generate(self, generator_name, country):
         generator = self._generator_factory.create_generator(generator_name)
         return generator.gen(generator_name, country)
 
     def ssn(self, country=None):
-        return self.__generate("SSN", country)
+        return self._generate("SSN", country)
 
     def id_card(self, country=None):
-        return self.__generate("IDCard", country)
+        return self._generate("IDCard", country)
 
     def passport(self, country=None):
-        return self.__generate("Passport", country)
+        return self._generate("Passport", country)
 
     def nric(self, country=None):
-        return self.__generate("NRIC", country)
+        return self._generate("NRIC", country)
 
     def my_number(self, country=None):
-        return self.__generate("MyNumber", country)
+        return self._generate("MyNumber", country)
 
     def first_name(self, country=None):
-        return self.__generate("first_name", country)
+        return self._generate("first_name", country)
 
     def middle_name(self, country=None):
-        return self.__generate("middle_name", country)
+        return self._generate("middle_name", country)
 
     def last_name(self, country=None):
-        return self.__generate("last_name", country)
+        return self._generate("last_name", country)
 
     def cn_name(self, country=None):
-        return self.__generate("cn_name", country)
+        return self._generate("cn_name", country)
 
     def kana_name(self, country=None):
-        return self.__generate("kana_name", country)
+        return self._generate("kana_name", country)
 
     def cellphone(self, country=None):
-        return self.__generate("cellphone", country)
+        return self._generate("cellphone", country)
 
     def area_code(self, country=None):
-        return self.__generate("area_code", country)
+        return self._generate("area_code", country)
 
     def high_risk_country(self, country=None):
-        return self.__generate("high_risk", country)
+        return self._generate("high_risk", country)
 
     def email(self, suffix=None):
-        return self.__generate("email", suffix)
+        return self._generate("email", suffix)
 
     def bank(self, country=None):
-        return self.__generate("bank", country)
+        return self._generate("bank", country)
 
     def currency(self, country=None):
-        return self.__generate("currency", country)
+        return self._generate("currency", country)
 
     def swift_code(self, country=None):
-        return self.__generate("swift_code", country)
+        return self._generate("swift_code", country)
 
     def stock_exchange(self, country=None):
-        return self.__generate("stock_exchange", country)
+        return self._generate("stock_exchange", country)
 
     def ticker_symbol(self, country=None):
-        return self.__generate("ticker_symbol", country)
+        return self._generate("ticker_symbol", country)
 
     def tz_identifier(self, country=None):
-        return self.__generate("tz_identifier", country)
+        return self._generate("tz_identifier", country)
 
     def locale(self, country=None):
-        return self.__generate("locale", country)
+        return self._generate("locale", country)
 
     def product(self, country=None):
-        return self.__generate("product", country)
+        return self._generate("product", country)
 
 
 if __name__ == '__main__':
     f = Financial()
     print(f.ssn())
     print(f.id_card())
     print(f.passport())
```

### Comparing `lfinancial-0.2.7/lfinancial/generators/bank.py` & `lfinancial-0.2.8/lfinancial/generators/bank.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/const.py` & `lfinancial-0.2.8/lfinancial/generators/const.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/contry.py` & `lfinancial-0.2.8/lfinancial/generators/contry.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/currency.py` & `lfinancial-0.2.8/lfinancial/generators/currency.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/document.py` & `lfinancial-0.2.8/lfinancial/generators/document.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/locale.py` & `lfinancial-0.2.8/lfinancial/generators/locale.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/mail.py` & `lfinancial-0.2.8/lfinancial/generators/mail.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/name.py` & `lfinancial-0.2.8/lfinancial/generators/name.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/phone.py` & `lfinancial-0.2.8/lfinancial/generators/phone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/stock.py` & `lfinancial-0.2.8/lfinancial/generators/stock.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/swift.py` & `lfinancial-0.2.8/lfinancial/generators/swift.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial/generators/timezone.py` & `lfinancial-0.2.8/lfinancial/generators/timezone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.2.8/lfinancial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.7
+Version: 0.2.8
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lfinancial-0.2.7/lfinancial.egg-info/SOURCES.txt` & `lfinancial-0.2.8/lfinancial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.7/setup.py` & `lfinancial-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lfinancial',
-    version='0.2.7',
+    version='0.2.8',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=find_packages(exclude=excluded_packages),
```

