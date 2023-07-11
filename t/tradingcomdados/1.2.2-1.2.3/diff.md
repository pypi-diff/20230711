# Comparing `tmp/tradingcomdados-1.2.2.tar.gz` & `tmp/tradingcomdados-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingcomdados-1.2.2.tar", last modified: Wed Jul  5 01:16:39 2023, max compression
+gzip compressed data, was "tradingcomdados-1.2.3.tar", last modified: Tue Jul 11 00:58:29 2023, max compression
```

## Comparing `tradingcomdados-1.2.2.tar` & `tradingcomdados-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 01:16:39.700714 tradingcomdados-1.2.2/
--rw-rw-rw-   0        0        0     1702 2023-07-05 01:16:39.700714 tradingcomdados-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.2.2/README.md
--rw-rw-rw-   0        0        0      452 2023-07-05 01:14:34.000000 tradingcomdados-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 01:16:39.701711 tradingcomdados-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 01:16:39.687712 tradingcomdados-1.2.2/tradingcomdados/
--rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.2.2/tradingcomdados/__init__.py
--rw-rw-rw-   0        0        0     2080 2023-07-02 18:17:22.000000 tradingcomdados-1.2.2/tradingcomdados/alternative_data.py
--rw-rw-rw-   0        0        0    11915 2023-07-05 01:13:25.000000 tradingcomdados-1.2.2/tradingcomdados/data_provider.py
--rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.2.2/tradingcomdados/ta_indicators.py
--rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.2.2/tradingcomdados/unsupervised_learning.py
-drwxrwxrwx   0        0        0        0 2023-07-05 01:16:39.699714 tradingcomdados-1.2.2/tradingcomdados.egg-info/
--rw-rw-rw-   0        0        0     1702 2023-07-05 01:16:38.000000 tradingcomdados-1.2.2/tradingcomdados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-05 01:16:38.000000 tradingcomdados-1.2.2/tradingcomdados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 01:16:38.000000 tradingcomdados-1.2.2/tradingcomdados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-07-05 01:16:38.000000 tradingcomdados-1.2.2/tradingcomdados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-05 01:16:38.000000 tradingcomdados-1.2.2/tradingcomdados.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 00:58:29.394648 tradingcomdados-1.2.3/
+-rw-rw-rw-   0        0        0     1702 2023-07-11 00:58:29.393648 tradingcomdados-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.2.3/README.md
+-rw-rw-rw-   0        0        0      452 2023-07-11 00:58:03.000000 tradingcomdados-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 00:58:29.394648 tradingcomdados-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 00:58:29.323644 tradingcomdados-1.2.3/tradingcomdados/
+-rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.2.3/tradingcomdados/__init__.py
+-rw-rw-rw-   0        0        0     3723 2023-07-11 00:58:03.000000 tradingcomdados-1.2.3/tradingcomdados/alternative_data.py
+-rw-rw-rw-   0        0        0    11046 2023-07-11 00:58:03.000000 tradingcomdados-1.2.3/tradingcomdados/data_provider.py
+-rw-rw-rw-   0        0        0     6915 2023-07-11 00:58:03.000000 tradingcomdados-1.2.3/tradingcomdados/portfolio.py
+-rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.2.3/tradingcomdados/ta_indicators.py
+-rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.2.3/tradingcomdados/unsupervised_learning.py
+drwxrwxrwx   0        0        0        0 2023-07-11 00:58:29.392648 tradingcomdados-1.2.3/tradingcomdados.egg-info/
+-rw-rw-rw-   0        0        0     1702 2023-07-11 00:58:27.000000 tradingcomdados-1.2.3/tradingcomdados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-07-11 00:58:27.000000 tradingcomdados-1.2.3/tradingcomdados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 00:58:27.000000 tradingcomdados-1.2.3/tradingcomdados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-07-11 00:58:27.000000 tradingcomdados-1.2.3/tradingcomdados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-11 00:58:27.000000 tradingcomdados-1.2.3/tradingcomdados.egg-info/top_level.txt
```

### Comparing `tradingcomdados-1.2.2/PKG-INFO` & `tradingcomdados-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.2.2
+Version: 1.2.3
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
```

### Comparing `tradingcomdados-1.2.2/README.md` & `tradingcomdados-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.2/setup.py` & `tradingcomdados-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.2/tradingcomdados/data_provider.py` & `tradingcomdados-1.2.3/tradingcomdados/data_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,11 @@
 import pandas as pd
 import requests as req
 
-import functools
-import logging
 
-logging.basicConfig(level=logging.DEBUG)
-logger = logging.getLogger()
-
-
-def _logging_error(func):
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        args_repr = [repr(a) for a in args]
-        kwargs_repr = [f"{k}={v!r}" for k, v in kwargs.items()]
-        signature = ", ".join(args_repr + kwargs_repr)
-        logger.debug(f"function {func.__name__} called with args {signature}")
-        try:
-            result = func(*args, **kwargs)
-            return result
-        except Exception as e:
-            logger.exception(
-                f"Exception raised in {func.__name__}. exception: {str(e)}"
-            )
-            raise e
-
-    return wrapper
-
-
-@_logging_error
 def _run_request(
     data_type: str,
     request_type: str,
     ticker: str,
     date_begin: str,
     date_end: str,
     api_key: str,
@@ -76,15 +50,14 @@
 
     except:
         print(
             "An error occured during the process of gathering data, please check the ticker and dates used and also remember to use a valid api key"
         )
 
 
-@_logging_error
 def _run_request_report(
     data_type: str,
     request_type: str,
     ticker: str,
     date_begin: str,
     trimester: str,
     api_key: str,
@@ -119,15 +92,14 @@
 
     except:
         print(
             "An error occured during the process of gathering data, please check the ticker and dates used and also remember to use a valid api key"
         )
 
 
-@_logging_error
 def _request_type_validation(data_type, request_type, ticker):
 
     try:
         url_base = "https://api.fintz.com.br"
 
         if data_type == "stock":
 
@@ -199,30 +171,28 @@
 
     except:
         return print(
             "Input request_type option not found, take a look at the documentation."
         )
 
 
-@_logging_error
 def _transform_to_dataframe(res, request_type):
     try:
         if request_type != "treasury_historical":
             df = pd.json_normalize(res)
 
         else:
             df = pd.DataFrame.from_dict(res["dados"])
 
         return df
 
     except:
         print("An error occured converting data from JSON to pandas DataFrame.")
 
 
-@_logging_error
 def get_data(
     data_type: str,
     request_type: str,
     ticker: str,
     date_begin: str,
     date_end: str,
     api_key: str,
@@ -264,15 +234,14 @@
         data_type, request_type, ticker, date_begin, date_end, api_key, endpoint
     )
     df = _transform_to_dataframe(res, request_type)
 
     return df
 
 
-@_logging_error
 def get_data_tickers(
     data_type: str,
     request_type: str,
     tickers: list,
     date_begin: str,
     date_end: str,
     api_key: str,
@@ -302,15 +271,14 @@
     for i in tickers:
         temp = get_data(data_type, request_type, i, date_begin, date_end, api_key)
         df = pd.concat([df, temp], ignore_index=True)
 
     return df
 
 
-@_logging_error
 def get_data_report(
     data_type: str,
     request_type: str,
     ticker: str,
     date_begin: str,
     trimester: str,
     api_key: str,
@@ -348,15 +316,14 @@
         data_type, request_type, ticker, date_begin, trimester, api_key, endpoint
     )
     df = _transform_to_dataframe(res, request_type)
 
     return df
 
 
-@_logging_error
 def get_data_report_tickers(
     data_type: str,
     request_type: str,
     tickers: list,
     date_begin: str,
     trimester: str,
     api_key: str,
```

### Comparing `tradingcomdados-1.2.2/tradingcomdados/ta_indicators.py` & `tradingcomdados-1.2.3/tradingcomdados/ta_indicators.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.2/tradingcomdados/unsupervised_learning.py` & `tradingcomdados-1.2.3/tradingcomdados/unsupervised_learning.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.2/tradingcomdados.egg-info/PKG-INFO` & `tradingcomdados-1.2.3/tradingcomdados.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.2.2
+Version: 1.2.3
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
```

