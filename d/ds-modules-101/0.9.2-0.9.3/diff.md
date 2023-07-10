# Comparing `tmp/ds_modules_101-0.9.2.tar.gz` & `tmp/ds_modules_101-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds_modules_101-0.9.2.tar", last modified: Mon Jul 10 21:56:23 2023, max compression
+gzip compressed data, was "ds_modules_101-0.9.3.tar", last modified: Mon Jul 10 22:01:03 2023, max compression
```

## Comparing `ds_modules_101-0.9.2.tar` & `ds_modules_101-0.9.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.732485 ds_modules_101-0.9.2/
--rw-r--r--   0 tanselarif   (501) staff       (20)     1073 2021-08-24 18:53:55.000000 ds_modules_101-0.9.2/LICENSE
--rw-r--r--   0 tanselarif   (501) staff       (20)      125 2022-04-28 16:26:06.000000 ds_modules_101-0.9.2/MANIFEST.in
--rw-r--r--   0 tanselarif   (501) staff       (20)      475 2023-07-10 21:56:23.732200 ds_modules_101-0.9.2/PKG-INFO
--rw-r--r--   0 tanselarif   (501) staff       (20)      116 2021-08-24 18:53:55.000000 ds_modules_101-0.9.2/README.md
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.704789 ds_modules_101-0.9.2/ds_modules_101/
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.706977 ds_modules_101-0.9.2/ds_modules_101/Data/
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.707570 ds_modules_101-0.9.2/ds_modules_101/Data/Docs/
--rw-r--r--   0 tanselarif   (501) staff       (20)    29564 2022-04-28 17:10:05.000000 ds_modules_101-0.9.2/ds_modules_101/Data/Docs/Word_Doc.docx
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.710457 ds_modules_101-0.9.2/ds_modules_101/Data/HR/
--rw-rw-r--   0 tanselarif   (501) staff       (20)   551779 2021-10-03 02:44:20.000000 ds_modules_101-0.9.2/ds_modules_101/Data/HR/HR copy.csv
--rw-r--r--   0 tanselarif   (501) staff       (20)  1282980 2021-10-05 22:32:32.000000 ds_modules_101-0.9.2/ds_modules_101/Data/HR/HR.csv
--rw-r--r--   0 tanselarif   (501) staff       (20)      415 2022-04-28 19:18:17.000000 ds_modules_101-0.9.2/ds_modules_101/Data/__init__.py
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.713652 ds_modules_101-0.9.2/ds_modules_101/Data/ibd/
--rw-r--r--   0 tanselarif   (501) staff       (20)  2572014 2021-07-28 19:25:49.000000 ds_modules_101-0.9.2/ds_modules_101/Data/ibd/IBD.csv
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.718957 ds_modules_101-0.9.2/ds_modules_101/Data/titanic/
--rw-r--r--   0 tanselarif   (501) staff       (20)    60302 2021-08-24 18:53:55.000000 ds_modules_101-0.9.2/ds_modules_101/Data/titanic/titanic.csv
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.728150 ds_modules_101-0.9.2/ds_modules_101/Models/
--rw-r--r--   0 tanselarif   (501) staff       (20)    37024 2021-10-10 11:46:28.000000 ds_modules_101-0.9.2/ds_modules_101/Models/LinearRegression.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    49293 2021-12-26 00:13:46.000000 ds_modules_101-0.9.2/ds_modules_101/Models/LogisticRegression.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    16172 2021-10-14 19:09:04.000000 ds_modules_101-0.9.2/ds_modules_101/Models/Microsimulation.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    29240 2021-09-25 18:40:16.000000 ds_modules_101-0.9.2/ds_modules_101/Models/MultinomialLogisticRegression.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    34551 2023-07-10 21:48:58.000000 ds_modules_101-0.9.2/ds_modules_101/Models/TimeSeries.py
--rw-r--r--   0 tanselarif   (501) staff       (20)      527 2023-03-13 16:59:45.000000 ds_modules_101-0.9.2/ds_modules_101/Models/__init__.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    14097 2021-08-29 12:38:02.000000 ds_modules_101-0.9.2/ds_modules_101/Models/logreg.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    30048 2021-09-09 17:10:53.000000 ds_modules_101-0.9.2/ds_modules_101/Models/oaxaca.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    30582 2021-09-03 21:21:08.000000 ds_modules_101-0.9.2/ds_modules_101/Models/oaxaca_old.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    26547 2021-08-24 18:53:55.000000 ds_modules_101-0.9.2/ds_modules_101/Models/ordinal_logistic_regression.py
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.730706 ds_modules_101-0.9.2/ds_modules_101/Plotting/
--rw-r--r--   0 tanselarif   (501) staff       (20)      370 2022-03-26 10:59:57.000000 ds_modules_101-0.9.2/ds_modules_101/Plotting/__init__.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    18250 2022-03-26 19:54:14.000000 ds_modules_101-0.9.2/ds_modules_101/Plotting/barplot.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    29927 2022-06-10 10:36:22.000000 ds_modules_101-0.9.2/ds_modules_101/Plotting/cleveland_plot.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    43685 2021-08-24 18:53:55.000000 ds_modules_101-0.9.2/ds_modules_101/Plotting/heatmap.py
--rw-r--r--   0 tanselarif   (501) staff       (20)     5255 2021-08-24 18:53:55.000000 ds_modules_101-0.9.2/ds_modules_101/Plotting/sankey_chart.py
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.731559 ds_modules_101-0.9.2/ds_modules_101/Utilities/
--rw-r--r--   0 tanselarif   (501) staff       (20)       38 2022-04-28 17:20:46.000000 ds_modules_101-0.9.2/ds_modules_101/Utilities/__init__.py
--rw-r--r--   0 tanselarif   (501) staff       (20)    15359 2022-04-28 19:34:04.000000 ds_modules_101-0.9.2/ds_modules_101/Utilities/word_doc_creator.py
--rw-r--r--   0 tanselarif   (501) staff       (20)        0 2021-08-24 18:53:55.000000 ds_modules_101-0.9.2/ds_modules_101/__init__.py
-drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 21:56:23.706771 ds_modules_101-0.9.2/ds_modules_101.egg-info/
--rw-r--r--   0 tanselarif   (501) staff       (20)      475 2023-07-10 21:56:23.000000 ds_modules_101-0.9.2/ds_modules_101.egg-info/PKG-INFO
--rw-r--r--   0 tanselarif   (501) staff       (20)     1137 2023-07-10 21:56:23.000000 ds_modules_101-0.9.2/ds_modules_101.egg-info/SOURCES.txt
--rw-r--r--   0 tanselarif   (501) staff       (20)        1 2023-07-10 21:56:23.000000 ds_modules_101-0.9.2/ds_modules_101.egg-info/dependency_links.txt
--rw-r--r--   0 tanselarif   (501) staff       (20)      120 2023-07-10 21:56:23.000000 ds_modules_101-0.9.2/ds_modules_101.egg-info/requires.txt
--rw-r--r--   0 tanselarif   (501) staff       (20)       15 2023-07-10 21:56:23.000000 ds_modules_101-0.9.2/ds_modules_101.egg-info/top_level.txt
--rw-r--r--   0 tanselarif   (501) staff       (20)       38 2023-07-10 21:56:23.732555 ds_modules_101-0.9.2/setup.cfg
--rw-r--r--   0 tanselarif   (501) staff       (20)     1061 2023-07-10 21:54:07.000000 ds_modules_101-0.9.2/setup.py
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.915105 ds_modules_101-0.9.3/
+-rw-r--r--   0 tanselarif   (501) staff       (20)     1073 2021-08-24 18:53:55.000000 ds_modules_101-0.9.3/LICENSE
+-rw-r--r--   0 tanselarif   (501) staff       (20)      125 2022-04-28 16:26:06.000000 ds_modules_101-0.9.3/MANIFEST.in
+-rw-r--r--   0 tanselarif   (501) staff       (20)      475 2023-07-10 22:01:03.914831 ds_modules_101-0.9.3/PKG-INFO
+-rw-r--r--   0 tanselarif   (501) staff       (20)      116 2021-08-24 18:53:55.000000 ds_modules_101-0.9.3/README.md
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.891238 ds_modules_101-0.9.3/ds_modules_101/
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.892207 ds_modules_101-0.9.3/ds_modules_101/Data/
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.892496 ds_modules_101-0.9.3/ds_modules_101/Data/Docs/
+-rw-r--r--   0 tanselarif   (501) staff       (20)    29564 2022-04-28 17:10:05.000000 ds_modules_101-0.9.3/ds_modules_101/Data/Docs/Word_Doc.docx
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.894679 ds_modules_101-0.9.3/ds_modules_101/Data/HR/
+-rw-rw-r--   0 tanselarif   (501) staff       (20)   551779 2021-10-03 02:44:20.000000 ds_modules_101-0.9.3/ds_modules_101/Data/HR/HR copy.csv
+-rw-r--r--   0 tanselarif   (501) staff       (20)  1282980 2021-10-05 22:32:32.000000 ds_modules_101-0.9.3/ds_modules_101/Data/HR/HR.csv
+-rw-r--r--   0 tanselarif   (501) staff       (20)      415 2022-04-28 19:18:17.000000 ds_modules_101-0.9.3/ds_modules_101/Data/__init__.py
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.897543 ds_modules_101-0.9.3/ds_modules_101/Data/ibd/
+-rw-r--r--   0 tanselarif   (501) staff       (20)  2572014 2021-07-28 19:25:49.000000 ds_modules_101-0.9.3/ds_modules_101/Data/ibd/IBD.csv
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.903119 ds_modules_101-0.9.3/ds_modules_101/Data/titanic/
+-rw-r--r--   0 tanselarif   (501) staff       (20)    60302 2021-08-24 18:53:55.000000 ds_modules_101-0.9.3/ds_modules_101/Data/titanic/titanic.csv
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.911419 ds_modules_101-0.9.3/ds_modules_101/Models/
+-rw-r--r--   0 tanselarif   (501) staff       (20)    37024 2021-10-10 11:46:28.000000 ds_modules_101-0.9.3/ds_modules_101/Models/LinearRegression.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    49293 2021-12-26 00:13:46.000000 ds_modules_101-0.9.3/ds_modules_101/Models/LogisticRegression.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    16172 2021-10-14 19:09:04.000000 ds_modules_101-0.9.3/ds_modules_101/Models/Microsimulation.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    29240 2021-09-25 18:40:16.000000 ds_modules_101-0.9.3/ds_modules_101/Models/MultinomialLogisticRegression.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    34551 2023-07-10 21:48:58.000000 ds_modules_101-0.9.3/ds_modules_101/Models/TimeSeries.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)      543 2023-07-10 22:00:08.000000 ds_modules_101-0.9.3/ds_modules_101/Models/__init__.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    14097 2021-08-29 12:38:02.000000 ds_modules_101-0.9.3/ds_modules_101/Models/logreg.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    30048 2021-09-09 17:10:53.000000 ds_modules_101-0.9.3/ds_modules_101/Models/oaxaca.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    30582 2021-09-03 21:21:08.000000 ds_modules_101-0.9.3/ds_modules_101/Models/oaxaca_old.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    26547 2021-08-24 18:53:55.000000 ds_modules_101-0.9.3/ds_modules_101/Models/ordinal_logistic_regression.py
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.913817 ds_modules_101-0.9.3/ds_modules_101/Plotting/
+-rw-r--r--   0 tanselarif   (501) staff       (20)      370 2022-03-26 10:59:57.000000 ds_modules_101-0.9.3/ds_modules_101/Plotting/__init__.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    18250 2022-03-26 19:54:14.000000 ds_modules_101-0.9.3/ds_modules_101/Plotting/barplot.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    29927 2022-06-10 10:36:22.000000 ds_modules_101-0.9.3/ds_modules_101/Plotting/cleveland_plot.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    43685 2021-08-24 18:53:55.000000 ds_modules_101-0.9.3/ds_modules_101/Plotting/heatmap.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)     5255 2021-08-24 18:53:55.000000 ds_modules_101-0.9.3/ds_modules_101/Plotting/sankey_chart.py
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.914363 ds_modules_101-0.9.3/ds_modules_101/Utilities/
+-rw-r--r--   0 tanselarif   (501) staff       (20)       38 2022-04-28 17:20:46.000000 ds_modules_101-0.9.3/ds_modules_101/Utilities/__init__.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)    15359 2022-04-28 19:34:04.000000 ds_modules_101-0.9.3/ds_modules_101/Utilities/word_doc_creator.py
+-rw-r--r--   0 tanselarif   (501) staff       (20)        0 2021-08-24 18:53:55.000000 ds_modules_101-0.9.3/ds_modules_101/__init__.py
+drwxr-xr-x   0 tanselarif   (501) staff       (20)        0 2023-07-10 22:01:03.892033 ds_modules_101-0.9.3/ds_modules_101.egg-info/
+-rw-r--r--   0 tanselarif   (501) staff       (20)      475 2023-07-10 22:01:03.000000 ds_modules_101-0.9.3/ds_modules_101.egg-info/PKG-INFO
+-rw-r--r--   0 tanselarif   (501) staff       (20)     1137 2023-07-10 22:01:03.000000 ds_modules_101-0.9.3/ds_modules_101.egg-info/SOURCES.txt
+-rw-r--r--   0 tanselarif   (501) staff       (20)        1 2023-07-10 22:01:03.000000 ds_modules_101-0.9.3/ds_modules_101.egg-info/dependency_links.txt
+-rw-r--r--   0 tanselarif   (501) staff       (20)      120 2023-07-10 22:01:03.000000 ds_modules_101-0.9.3/ds_modules_101.egg-info/requires.txt
+-rw-r--r--   0 tanselarif   (501) staff       (20)       15 2023-07-10 22:01:03.000000 ds_modules_101-0.9.3/ds_modules_101.egg-info/top_level.txt
+-rw-r--r--   0 tanselarif   (501) staff       (20)       38 2023-07-10 22:01:03.915175 ds_modules_101-0.9.3/setup.cfg
+-rw-r--r--   0 tanselarif   (501) staff       (20)     1061 2023-07-10 22:00:54.000000 ds_modules_101-0.9.3/setup.py
```

### Comparing `ds_modules_101-0.9.2/LICENSE` & `ds_modules_101-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Data/Docs/Word_Doc.docx` & `ds_modules_101-0.9.3/ds_modules_101/Data/Docs/Word_Doc.docx`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Data/HR/HR copy.csv` & `ds_modules_101-0.9.3/ds_modules_101/Data/HR/HR copy.csv`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Data/HR/HR.csv` & `ds_modules_101-0.9.3/ds_modules_101/Data/HR/HR.csv`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Data/ibd/IBD.csv` & `ds_modules_101-0.9.3/ds_modules_101/Data/ibd/IBD.csv`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Data/titanic/titanic.csv` & `ds_modules_101-0.9.3/ds_modules_101/Data/titanic/titanic.csv`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Models/LinearRegression.py` & `ds_modules_101-0.9.3/ds_modules_101/Models/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Models/LogisticRegression.py` & `ds_modules_101-0.9.3/ds_modules_101/Models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Models/Microsimulation.py` & `ds_modules_101-0.9.3/ds_modules_101/Models/Microsimulation.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Models/MultinomialLogisticRegression.py` & `ds_modules_101-0.9.3/ds_modules_101/Models/MultinomialLogisticRegression.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Models/TimeSeries.py` & `ds_modules_101-0.9.3/ds_modules_101/Models/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Models/__init__.py` & `ds_modules_101-0.9.3/ds_modules_101/Models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 from .ordinal_logistic_regression import OrderedModel
 from .oaxaca import Oaxaca
 from .logreg import log_reg_basic,log_reg,log_reg_with_feature_selection,log_reg_diagnostic_performance,log_reg_diagnostic_correlations,logistic_regression_get_report
 from .LogisticRegression import LogisticRegressionClass
 from .LinearRegression import LinearRegressionClass
 from .MultinomialLogisticRegression import MultinomialLogisticRegressionClass
 from .Microsimulation import MicrosimulationClass
-from .TimeSeries import analyse_time_series
+from .TimeSeries import analyse_time_series,get_time_series
```

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Models/logreg.py` & `ds_modules_101-0.9.3/ds_modules_101/Models/logreg.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Models/oaxaca.py` & `ds_modules_101-0.9.3/ds_modules_101/Models/oaxaca.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Models/oaxaca_old.py` & `ds_modules_101-0.9.3/ds_modules_101/Models/oaxaca_old.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Models/ordinal_logistic_regression.py` & `ds_modules_101-0.9.3/ds_modules_101/Models/ordinal_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Plotting/barplot.py` & `ds_modules_101-0.9.3/ds_modules_101/Plotting/barplot.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Plotting/cleveland_plot.py` & `ds_modules_101-0.9.3/ds_modules_101/Plotting/cleveland_plot.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Plotting/heatmap.py` & `ds_modules_101-0.9.3/ds_modules_101/Plotting/heatmap.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Plotting/sankey_chart.py` & `ds_modules_101-0.9.3/ds_modules_101/Plotting/sankey_chart.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101/Utilities/word_doc_creator.py` & `ds_modules_101-0.9.3/ds_modules_101/Utilities/word_doc_creator.py`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/ds_modules_101.egg-info/SOURCES.txt` & `ds_modules_101-0.9.3/ds_modules_101.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds_modules_101-0.9.2/setup.py` & `ds_modules_101-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='ds_modules_101',
-    version='0.9.2',
+    version='0.9.3',
     description="A small package to help with some routine Data Science activities",
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Tansel Arif',
     author_email='tanselarif21@gmail.com',
```

