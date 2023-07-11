# Comparing `tmp/lfinancial-0.2.6.tar.gz` & `tmp/lfinancial-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.2.6.tar", last modified: Mon Jul 10 14:54:38 2023, max compression
+gzip compressed data, was "lfinancial-0.2.7.tar", last modified: Tue Jul 11 08:39:18 2023, max compression
```

## Comparing `lfinancial-0.2.6.tar` & `lfinancial-0.2.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:38.120964 lfinancial-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-10 14:54:20.000000 lfinancial-0.2.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-10 14:54:38.120964 lfinancial-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-10 14:54:20.000000 lfinancial-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:38.116964 lfinancial-0.2.6/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:38.120964 lfinancial-0.2.6/lfinancial/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/contry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-10 14:54:20.000000 lfinancial-0.2.6/lfinancial/generators/timezone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:38.120964 lfinancial-0.2.6/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-10 14:54:38.000000 lfinancial-0.2.6/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-10 14:54:38.000000 lfinancial-0.2.6/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:54:38.000000 lfinancial-0.2.6/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 14:54:38.000000 lfinancial-0.2.6/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:54:38.120964 lfinancial-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-10 14:54:20.000000 lfinancial-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:54:38.120964 lfinancial-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-10 14:54:20.000000 lfinancial-0.2.6/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:39:18.538564 lfinancial-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-11 08:38:57.000000 lfinancial-0.2.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-11 08:39:18.538564 lfinancial-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 08:38:57.000000 lfinancial-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:39:18.534564 lfinancial-0.2.7/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:39:18.538564 lfinancial-0.2.7/lfinancial/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/contry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-11 08:38:57.000000 lfinancial-0.2.7/lfinancial/generators/timezone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:39:18.534564 lfinancial-0.2.7/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-11 08:39:18.000000 lfinancial-0.2.7/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-11 08:39:18.000000 lfinancial-0.2.7/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:39:18.000000 lfinancial-0.2.7/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 08:39:18.000000 lfinancial-0.2.7/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 08:39:18.538564 lfinancial-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-11 08:38:57.000000 lfinancial-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:39:18.538564 lfinancial-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 08:38:57.000000 lfinancial-0.2.7/tests/test_document.py
```

### Comparing `lfinancial-0.2.6/LICENSE.txt` & `lfinancial-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/PKG-INFO` & `lfinancial-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.6
+Version: 0.2.7
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -93,8 +93,11 @@
 # AAPL
 
 f.tz_identifier()
 # Asia/Baku
 
 f.locale()
 # zh-CN
+
+f.product()
+# Shares
 ```
```

### Comparing `lfinancial-0.2.6/README.md` & `lfinancial-0.2.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -81,8 +81,11 @@
 # AAPL
 
 f.tz_identifier()
 # Asia/Baku
 
 f.locale()
 # zh-CN
+
+f.product()
+# Shares
 ```
```

### Comparing `lfinancial-0.2.6/lfinancial/factory.py` & `lfinancial-0.2.7/lfinancial/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from lfinancial.generators.contry import CountryGenerator
 from lfinancial.generators.currency import CurrencyGenerator
 from lfinancial.generators.document import IDCodeGenerator
 from lfinancial.generators.locale import LocaleGenerator
 from lfinancial.generators.mail import EmailGenerator
 from lfinancial.generators.name import NameGenerator
 from lfinancial.generators.phone import PhoneGenerator
-from lfinancial.generators.stock import StockGenerator
+from lfinancial.generators.stock import StockGenerator, TradeProduct
 from lfinancial.generators.swift import SwiftGenerator
 from lfinancial.generators.timezone import TimeZoneGenerator
 
 
 class GeneratorFactory:
     def __init__(self):
         self.generators = {
@@ -31,14 +31,15 @@
             "bank": BankGenerator(),
             "currency": CurrencyGenerator(),
             "swift_code": SwiftGenerator(),
             "stock_exchange": StockGenerator(),
             "ticker_symbol": StockGenerator(),
             "tz_identifier": TimeZoneGenerator(),
             "locale": LocaleGenerator(),
+            "product": StockGenerator(),
         }
 
     def register_generator(self, name, generator):
         self.generators[name] = generator
 
     def create_generator(self, name):
         if name in self.generators:
```

### Comparing `lfinancial-0.2.6/lfinancial/financial.py` & `lfinancial-0.2.7/lfinancial/financial.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 
     def tz_identifier(self, country=None):
         return self.__generate("tz_identifier", country)
 
     def locale(self, country=None):
         return self.__generate("locale", country)
 
+    def product(self, country=None):
+        return self.__generate("product", country)
+
 
 if __name__ == '__main__':
     f = Financial()
     print(f.ssn())
     print(f.id_card())
     print(f.passport())
     print(f.nric())
@@ -92,7 +95,8 @@
     print(f.bank())
     print(f.currency())
     print(f.swift_code())
     print(f.stock_exchange())
     print(f.ticker_symbol())
     print(f.tz_identifier())
     print(f.locale())
+    print(f.product())
```

### Comparing `lfinancial-0.2.6/lfinancial/generators/bank.py` & `lfinancial-0.2.7/lfinancial/generators/bank.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial/generators/const.py` & `lfinancial-0.2.7/lfinancial/generators/const.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial/generators/contry.py` & `lfinancial-0.2.7/lfinancial/generators/contry.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial/generators/currency.py` & `lfinancial-0.2.7/lfinancial/generators/currency.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial/generators/document.py` & `lfinancial-0.2.7/lfinancial/generators/document.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial/generators/locale.py` & `lfinancial-0.2.7/lfinancial/generators/locale.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial/generators/mail.py` & `lfinancial-0.2.7/lfinancial/generators/mail.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial/generators/name.py` & `lfinancial-0.2.7/lfinancial/generators/name.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial/generators/phone.py` & `lfinancial-0.2.7/lfinancial/generators/phone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial/generators/stock.py` & `lfinancial-0.2.7/lfinancial/generators/stock.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import random
 
 
 class StockGenerator:
 
     def __init__(self):
         self.default_country = {
-            "stock_exchange":
-                "US",
-
-            "ticker_symbol":
-                "US"
-
+            "stock_exchange": "US",
+            "ticker_symbol": "US",
+            "product": "US"
         }
 
     def gen(self, stock_type, country):
         if country is None:
             country = self.default_country.get(stock_type)
 
         match stock_type:
             case "stock_exchange":
-
                 stock_type = StockExchange(country)
             case "ticker_symbol":
-
                 stock_type = TickerSymbol(country)
+            case "product":
+                stock_type = TradeProduct(country)
             case _:
-                raise ValueError(f"U"
-                                 f"nsupported name type: {stock_type}.")
+                raise ValueError(f"Unsupported name type: {stock_type}.")
 
         return stock_type.gen()
 
 
 class StockType:
     def __init__(self, country):
         self.country = country
@@ -163,7 +159,38 @@
         "YNDX",
         "YUMC",
         "YY",
     )
 
     def gen(self):
         return random.choice(self.ticker_symbols)
+
+
+class TradeProduct(StockType):
+    product = (
+        "A-shares",
+        "ADR",
+        "Bond",
+        "Business Trusts",
+        "Callable Bull/Bear Contract",
+        "Closed-end Funds",
+        "Crypto",
+        "DLCs",
+        "ETFs",
+        "Foreign Exchange Futures",
+        "Fractional Shares",
+        "Futures",
+        "Index",
+        "Inside Certificate",
+        "Leveraged Foreign Exchange",
+        "Preference Shares",
+        "REITs",
+        "Share Price Index Futures",
+        "Shares",
+        "Stock Index Option",
+        "Stock Option",
+        "Trusts",
+        "Warrants"
+    )
+
+    def gen(self):
+        return random.choice(self.product)
```

### Comparing `lfinancial-0.2.6/lfinancial/generators/swift.py` & `lfinancial-0.2.7/lfinancial/generators/swift.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial/generators/timezone.py` & `lfinancial-0.2.7/lfinancial/generators/timezone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.2.7/lfinancial.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.6
+Version: 0.2.7
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -93,8 +93,11 @@
 # AAPL
 
 f.tz_identifier()
 # Asia/Baku
 
 f.locale()
 # zh-CN
+
+f.product()
+# Shares
 ```
```

### Comparing `lfinancial-0.2.6/lfinancial.egg-info/SOURCES.txt` & `lfinancial-0.2.7/lfinancial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.6/setup.py` & `lfinancial-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lfinancial',
-    version='0.2.6',
+    version='0.2.7',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=find_packages(exclude=excluded_packages),
```

