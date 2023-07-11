# Comparing `tmp/tradingcomdados-1.2.3.tar.gz` & `tmp/tradingcomdados-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingcomdados-1.2.3.tar", last modified: Tue Jul 11 00:58:29 2023, max compression
+gzip compressed data, was "tradingcomdados-1.2.4.tar", last modified: Tue Jul 11 15:05:28 2023, max compression
```

## Comparing `tradingcomdados-1.2.3.tar` & `tradingcomdados-1.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 00:58:29.394648 tradingcomdados-1.2.3/
--rw-rw-rw-   0        0        0     1702 2023-07-11 00:58:29.393648 tradingcomdados-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.2.3/README.md
--rw-rw-rw-   0        0        0      452 2023-07-11 00:58:03.000000 tradingcomdados-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 00:58:29.394648 tradingcomdados-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 00:58:29.323644 tradingcomdados-1.2.3/tradingcomdados/
--rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.2.3/tradingcomdados/__init__.py
--rw-rw-rw-   0        0        0     3723 2023-07-11 00:58:03.000000 tradingcomdados-1.2.3/tradingcomdados/alternative_data.py
--rw-rw-rw-   0        0        0    11046 2023-07-11 00:58:03.000000 tradingcomdados-1.2.3/tradingcomdados/data_provider.py
--rw-rw-rw-   0        0        0     6915 2023-07-11 00:58:03.000000 tradingcomdados-1.2.3/tradingcomdados/portfolio.py
--rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.2.3/tradingcomdados/ta_indicators.py
--rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.2.3/tradingcomdados/unsupervised_learning.py
-drwxrwxrwx   0        0        0        0 2023-07-11 00:58:29.392648 tradingcomdados-1.2.3/tradingcomdados.egg-info/
--rw-rw-rw-   0        0        0     1702 2023-07-11 00:58:27.000000 tradingcomdados-1.2.3/tradingcomdados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-07-11 00:58:27.000000 tradingcomdados-1.2.3/tradingcomdados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 00:58:27.000000 tradingcomdados-1.2.3/tradingcomdados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-07-11 00:58:27.000000 tradingcomdados-1.2.3/tradingcomdados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-11 00:58:27.000000 tradingcomdados-1.2.3/tradingcomdados.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 15:05:28.158914 tradingcomdados-1.2.4/
+-rw-rw-rw-   0        0        0     1702 2023-07-11 15:05:28.157914 tradingcomdados-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.2.4/README.md
+-rw-rw-rw-   0        0        0      452 2023-07-11 15:05:14.000000 tradingcomdados-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 15:05:28.159915 tradingcomdados-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:05:28.146754 tradingcomdados-1.2.4/tradingcomdados/
+-rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.2.4/tradingcomdados/__init__.py
+-rw-rw-rw-   0        0        0     2941 2023-07-11 15:01:25.000000 tradingcomdados-1.2.4/tradingcomdados/alternative_data.py
+-rw-rw-rw-   0        0        0    11046 2023-07-11 14:55:53.000000 tradingcomdados-1.2.4/tradingcomdados/data_provider.py
+-rw-rw-rw-   0        0        0     6915 2023-07-11 00:58:03.000000 tradingcomdados-1.2.4/tradingcomdados/portfolio.py
+-rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.2.4/tradingcomdados/ta_indicators.py
+-rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.2.4/tradingcomdados/unsupervised_learning.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:05:28.156916 tradingcomdados-1.2.4/tradingcomdados.egg-info/
+-rw-rw-rw-   0        0        0     1702 2023-07-11 15:05:24.000000 tradingcomdados-1.2.4/tradingcomdados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-07-11 15:05:25.000000 tradingcomdados-1.2.4/tradingcomdados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 15:05:24.000000 tradingcomdados-1.2.4/tradingcomdados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-07-11 15:05:25.000000 tradingcomdados-1.2.4/tradingcomdados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-11 15:05:25.000000 tradingcomdados-1.2.4/tradingcomdados.egg-info/top_level.txt
```

### Comparing `tradingcomdados-1.2.3/PKG-INFO` & `tradingcomdados-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.2.3
+Version: 1.2.4
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
```

### Comparing `tradingcomdados-1.2.3/README.md` & `tradingcomdados-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.3/setup.py` & `tradingcomdados-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.3/tradingcomdados/data_provider.py` & `tradingcomdados-1.2.4/tradingcomdados/data_provider.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.3/tradingcomdados/portfolio.py` & `tradingcomdados-1.2.4/tradingcomdados/portfolio.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.3/tradingcomdados/ta_indicators.py` & `tradingcomdados-1.2.4/tradingcomdados/ta_indicators.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.3/tradingcomdados/unsupervised_learning.py` & `tradingcomdados-1.2.4/tradingcomdados/unsupervised_learning.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.3/tradingcomdados.egg-info/PKG-INFO` & `tradingcomdados-1.2.4/tradingcomdados.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.2.3
+Version: 1.2.4
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
```

