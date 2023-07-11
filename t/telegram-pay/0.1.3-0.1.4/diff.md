# Comparing `tmp/telegram_pay-0.1.3.tar.gz` & `tmp/telegram_pay-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_pay-0.1.3.tar", max compression
+gzip compressed data, was "telegram_pay-0.1.4.tar", max compression
```

## Comparing `telegram_pay-0.1.3.tar` & `telegram_pay-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1084 2023-04-19 12:42:24.063222 telegram_pay-0.1.3/LICENSE
--rw-r--r--   0        0        0      447 2023-04-22 15:59:09.736770 telegram_pay-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      379 2023-04-19 12:42:24.064220 telegram_pay-0.1.3/README.md
--rw-r--r--   0        0        0       74 2023-04-19 12:42:24.066213 telegram_pay-0.1.3/telegram_pay/__init__.py
--rw-r--r--   0        0        0     1915 2023-04-19 12:42:24.066213 telegram_pay-0.1.3/telegram_pay/enums.py
--rw-r--r--   0        0        0     4528 2023-04-22 15:58:05.914989 telegram_pay-0.1.3/telegram_pay/models.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 telegram_pay-0.1.3/setup.py
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 telegram_pay-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-19 12:42:24.063222 telegram_pay-0.1.4/LICENSE
+-rw-r--r--   0        0        0      446 2023-07-11 09:17:10.622629 telegram_pay-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      379 2023-04-19 12:42:24.064220 telegram_pay-0.1.4/README.md
+-rw-r--r--   0        0        0       74 2023-04-19 12:42:24.066213 telegram_pay-0.1.4/telegram_pay/__init__.py
+-rw-r--r--   0        0        0     1915 2023-04-19 12:42:24.066213 telegram_pay-0.1.4/telegram_pay/enums.py
+-rw-r--r--   0        0        0     4528 2023-04-22 15:58:05.914989 telegram_pay-0.1.4/telegram_pay/models.py
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 telegram_pay-0.1.4/PKG-INFO
```

### Comparing `telegram_pay-0.1.3/LICENSE` & `telegram_pay-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_pay-0.1.3/telegram_pay/enums.py` & `telegram_pay-0.1.4/telegram_pay/enums.py`

 * *Files identical despite different names*

### Comparing `telegram_pay-0.1.3/telegram_pay/models.py` & `telegram_pay-0.1.4/telegram_pay/models.py`

 * *Files identical despite different names*

### Comparing `telegram_pay-0.1.3/PKG-INFO` & `telegram_pay-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: telegram-pay
-Version: 0.1.3
+Version: 0.1.4
 Summary: Wrapper for api.pay.4u.studio
 License: MIT
 Author: Snimshchikov Ilya
 Author-email: snimshchikov.ilya@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Requires-Dist: pytz (>=2022.7.1,<2023.0.0)
 Description-Content-Type: text/markdown
 
 # Install
 `pip install telegram-pay`
 
 # Use
```

