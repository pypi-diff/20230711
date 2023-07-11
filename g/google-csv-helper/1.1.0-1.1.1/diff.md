# Comparing `tmp/google-csv-helper-1.1.0.tar.gz` & `tmp/google-csv-helper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-csv-helper-1.1.0.tar", last modified: Tue Jun 27 17:17:12 2023, max compression
+gzip compressed data, was "google-csv-helper-1.1.1.tar", last modified: Tue Jul 11 00:51:14 2023, max compression
```

## Comparing `google-csv-helper-1.1.0.tar` & `google-csv-helper-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:17:12.052785 google-csv-helper-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-27 17:17:12.052785 google-csv-helper-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:17:12.052785 google-csv-helper-1.1.0/google_csv_helper/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/adsense_csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/csv_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/ga3_csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/google_csv_helper/ga4_csv_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:17:12.052785 google-csv-helper-1.1.0/google_csv_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 17:17:12.000000 google-csv-helper-1.1.0/google_csv_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:17:12.052785 google-csv-helper-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-27 17:16:53.000000 google-csv-helper-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:51:14.438626 google-csv-helper-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-11 00:50:57.000000 google-csv-helper-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-11 00:51:14.438626 google-csv-helper-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-11 00:50:57.000000 google-csv-helper-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:51:14.434626 google-csv-helper-1.1.1/google_csv_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 00:50:57.000000 google-csv-helper-1.1.1/google_csv_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-07-11 00:50:57.000000 google-csv-helper-1.1.1/google_csv_helper/adsense_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-11 00:50:57.000000 google-csv-helper-1.1.1/google_csv_helper/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-11 00:50:57.000000 google-csv-helper-1.1.1/google_csv_helper/csv_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-07-11 00:50:57.000000 google-csv-helper-1.1.1/google_csv_helper/csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-07-11 00:50:57.000000 google-csv-helper-1.1.1/google_csv_helper/ga3_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-11 00:50:57.000000 google-csv-helper-1.1.1/google_csv_helper/ga4_csv_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:51:14.434626 google-csv-helper-1.1.1/google_csv_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-11 00:51:14.000000 google-csv-helper-1.1.1/google_csv_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-11 00:51:14.000000 google-csv-helper-1.1.1/google_csv_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 00:51:14.000000 google-csv-helper-1.1.1/google_csv_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 00:51:14.000000 google-csv-helper-1.1.1/google_csv_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 00:51:14.000000 google-csv-helper-1.1.1/google_csv_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 00:51:14.000000 google-csv-helper-1.1.1/google_csv_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 00:51:14.438626 google-csv-helper-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-11 00:50:57.000000 google-csv-helper-1.1.1/setup.py
```

### Comparing `google-csv-helper-1.1.0/LICENSE` & `google-csv-helper-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.1.0/PKG-INFO` & `google-csv-helper-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-csv-helper
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.
 Home-page: https://github.com/changyy/google-csv-helper
 Download-URL: https://pypi.org/project/google-csv-helper/
 Author: Yuan-Yi Chang
 Author-email: <changyy.csie@gmail.com>
 Keywords: python,google,csv,adsense,admob,report
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-csv-helper-1.1.0/README.md` & `google-csv-helper-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.1.0/google_csv_helper/adsense_csv_helper.py` & `google-csv-helper-1.1.1/google_csv_helper/adsense_csv_helper.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.1.0/google_csv_helper/cmd.py` & `google-csv-helper-1.1.1/google_csv_helper/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from google_csv_helper import ga4_csv_helper
 
 def main():
     def valid_date(data: str):
         output = datetime.date.today()
         if data != "today":
             try:
-                return datetime.datetime.strptime(data, "%Y-%m-%d")
+                dt = datetime.datetime.strptime(data, "%Y-%m-%d")
+                return datetime.date(dt.year, dt.month, dt.day)
             except ValueError:
                 raise argparse.ArgumentTypeError(f"not a valid date: {data}")
         return output
     parser = argparse.ArgumentParser()
     parser.add_argument("csv_dir", nargs="*", type=str, help="the directory where the csv file is located")
     parser.add_argument("--output", choices=['json', 'markdown'], default='json', help="results format")
     parser.add_argument("--output-type", choices=['adsense', 'ga3', 'ga4'], default="adsense", help="the report")
```

### Comparing `google-csv-helper-1.1.0/google_csv_helper/csv_common.py` & `google-csv-helper-1.1.1/google_csv_helper/csv_common.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.1.0/google_csv_helper/csv_helper.py` & `google-csv-helper-1.1.1/google_csv_helper/csv_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,17 @@
         return
 
     def handleDataFrameMerge(self, oldDataFrame: pandas.DataFrame, newDataFrame: pandas.DataFrame, keyField:str, valueField:str) -> pandas.DataFrame:
         #print("in handleDataFrameMerge")
         # https://pandas.pydata.org/docs/reference/api/pandas.concat.html?highlight=concat#pandas.concat
         # https://pandas.pydata.org/docs/reference/api/pandas.merge_ordered.html
         output = pandas.merge_ordered(oldDataFrame, newDataFrame)
+        #print("##########")
+        #print(output)
+        #print("##------##")
         while True:
             oldSize = len(output.index)
             #print(f"Init size: {oldSize},  {output.index}")
             if oldSize <= 1:
                 break
             prev = None
             for i in output.index:
```

### Comparing `google-csv-helper-1.1.0/google_csv_helper/ga3_csv_helper.py` & `google-csv-helper-1.1.1/google_csv_helper/ga3_csv_helper.py`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.1.0/google_csv_helper.egg-info/PKG-INFO` & `google-csv-helper-1.1.1/google_csv_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-csv-helper
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.
 Home-page: https://github.com/changyy/google-csv-helper
 Download-URL: https://pypi.org/project/google-csv-helper/
 Author: Yuan-Yi Chang
 Author-email: <changyy.csie@gmail.com>
 Keywords: python,google,csv,adsense,admob,report
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-csv-helper-1.1.0/setup.py` & `google-csv-helper-1.1.1/setup.py`

 * *Files identical despite different names*

