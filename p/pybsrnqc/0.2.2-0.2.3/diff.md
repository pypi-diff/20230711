# Comparing `tmp/pybsrnqc-0.2.2.tar.gz` & `tmp/pybsrnqc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybsrnqc-0.2.2.tar", last modified: Mon Sep 26 07:14:31 2022, max compression
+gzip compressed data, was "pybsrnqc-0.2.3.tar", last modified: Tue Jul 11 07:47:11 2023, max compression
```

## Comparing `pybsrnqc-0.2.2.tar` & `pybsrnqc-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-26 07:14:31.535302 pybsrnqc-0.2.2/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1062 2021-07-22 10:08:42.000000 pybsrnqc-0.2.2/LICENSE
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      134 2022-06-15 11:45:37.000000 pybsrnqc-0.2.2/MANIFEST.in
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)    10976 2022-09-26 07:14:31.535302 pybsrnqc-0.2.2/PKG-INFO
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10198 2022-09-26 07:13:26.000000 pybsrnqc-0.2.2/README.md
-drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-26 07:14:31.535302 pybsrnqc-0.2.2/pybsrnqc/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      150 2021-07-22 12:06:54.000000 pybsrnqc-0.2.2/pybsrnqc/__init__.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6299 2022-09-26 07:08:36.000000 pybsrnqc-0.2.2/pybsrnqc/automaticQC.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      308 2021-07-22 12:06:54.000000 pybsrnqc-0.2.2/pybsrnqc/callbackSave.js
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      272 2021-07-22 12:06:54.000000 pybsrnqc-0.2.2/pybsrnqc/callbackSelect.js
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3631 2022-06-15 10:21:10.000000 pybsrnqc-0.2.2/pybsrnqc/coef_calculator.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    13722 2022-06-25 08:07:03.000000 pybsrnqc-0.2.2/pybsrnqc/coef_study.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1660 2022-06-24 09:45:16.000000 pybsrnqc-0.2.2/pybsrnqc/config.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2152 2022-09-26 07:07:42.000000 pybsrnqc-0.2.2/pybsrnqc/open_data.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12232 2021-11-04 10:31:00.000000 pybsrnqc-0.2.2/pybsrnqc/plot_limits.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6180 2021-11-04 10:31:00.000000 pybsrnqc-0.2.2/pybsrnqc/qc_functions.py
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     9334 2022-06-24 09:24:54.000000 pybsrnqc-0.2.2/pybsrnqc/qcrad.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      603 2022-06-24 07:28:22.000000 pybsrnqc-0.2.2/pybsrnqc/qcrad_conf.json
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      651 2021-08-05 07:45:51.000000 pybsrnqc-0.2.2/pybsrnqc/utils.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3917 2021-11-04 08:02:05.000000 pybsrnqc-0.2.2/pybsrnqc/visualPlot.py
-drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-26 07:14:31.535302 pybsrnqc-0.2.2/pybsrnqc.egg-info/
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)    10976 2022-09-26 07:14:31.000000 pybsrnqc-0.2.2/pybsrnqc.egg-info/PKG-INFO
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      519 2022-09-26 07:14:31.000000 pybsrnqc-0.2.2/pybsrnqc.egg-info/SOURCES.txt
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)        1 2022-09-26 07:14:31.000000 pybsrnqc-0.2.2/pybsrnqc.egg-info/dependency_links.txt
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)       96 2022-09-26 07:14:31.000000 pybsrnqc-0.2.2/pybsrnqc.egg-info/requires.txt
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)        9 2022-09-26 07:14:31.000000 pybsrnqc-0.2.2/pybsrnqc.egg-info/top_level.txt
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)       38 2022-09-26 07:14:31.535302 pybsrnqc-0.2.2/setup.cfg
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1280 2022-09-26 07:13:32.000000 pybsrnqc-0.2.2/setup.py
+drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2023-07-11 07:47:11.557207 pybsrnqc-0.2.3/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1062 2021-07-22 10:08:42.000000 pybsrnqc-0.2.3/LICENSE
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      134 2022-06-15 11:45:37.000000 pybsrnqc-0.2.3/MANIFEST.in
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)    10956 2023-07-11 07:47:11.557207 pybsrnqc-0.2.3/PKG-INFO
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10198 2022-09-26 07:13:26.000000 pybsrnqc-0.2.3/README.md
+drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2023-07-11 07:47:11.557207 pybsrnqc-0.2.3/pybsrnqc/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      150 2021-07-22 12:06:54.000000 pybsrnqc-0.2.3/pybsrnqc/__init__.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6299 2022-09-26 07:08:36.000000 pybsrnqc-0.2.3/pybsrnqc/automaticQC.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      308 2021-07-22 12:06:54.000000 pybsrnqc-0.2.3/pybsrnqc/callbackSave.js
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      272 2021-07-22 12:06:54.000000 pybsrnqc-0.2.3/pybsrnqc/callbackSelect.js
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3631 2022-06-15 10:21:10.000000 pybsrnqc-0.2.3/pybsrnqc/coef_calculator.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    13695 2023-07-11 07:30:53.000000 pybsrnqc-0.2.3/pybsrnqc/coef_study.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1660 2022-06-24 09:45:16.000000 pybsrnqc-0.2.3/pybsrnqc/config.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2152 2022-09-26 07:07:42.000000 pybsrnqc-0.2.3/pybsrnqc/open_data.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12232 2021-11-04 10:31:00.000000 pybsrnqc-0.2.3/pybsrnqc/plot_limits.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6180 2021-11-04 10:31:00.000000 pybsrnqc-0.2.3/pybsrnqc/qc_functions.py
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     9334 2022-06-24 09:24:54.000000 pybsrnqc-0.2.3/pybsrnqc/qcrad.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      603 2022-06-24 07:28:22.000000 pybsrnqc-0.2.3/pybsrnqc/qcrad_conf.json
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      651 2021-08-05 07:45:51.000000 pybsrnqc-0.2.3/pybsrnqc/utils.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3926 2023-07-11 07:44:30.000000 pybsrnqc-0.2.3/pybsrnqc/visualPlot.py
+drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2023-07-11 07:47:11.557207 pybsrnqc-0.2.3/pybsrnqc.egg-info/
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)    10956 2023-07-11 07:47:11.000000 pybsrnqc-0.2.3/pybsrnqc.egg-info/PKG-INFO
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      519 2023-07-11 07:47:11.000000 pybsrnqc-0.2.3/pybsrnqc.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)        1 2023-07-11 07:47:11.000000 pybsrnqc-0.2.3/pybsrnqc.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      109 2023-07-11 07:47:11.000000 pybsrnqc-0.2.3/pybsrnqc.egg-info/requires.txt
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)        9 2023-07-11 07:47:11.000000 pybsrnqc-0.2.3/pybsrnqc.egg-info/top_level.txt
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)       38 2023-07-11 07:47:11.557207 pybsrnqc-0.2.3/setup.cfg
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1318 2023-07-11 07:47:02.000000 pybsrnqc-0.2.3/setup.py
```

### Comparing `pybsrnqc-0.2.2/LICENSE` & `pybsrnqc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/PKG-INFO` & `pybsrnqc-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pybsrnqc
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package to study BSRN data and their quality control
 Home-page: https://github.com/LE2P/pybsrnqc/tree/main/pybsrnqc
 Author: Maelle Baronnet
 Author-email: maelle.baronnet@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -323,9 +322,7 @@
 ```python
 coef_calculator.compute(path=None, level='level_2', bw_sel=None, station=Station())
   # path : path of the directory with the data files
   # level : 'level_2' (default) to plot the 2nd level limits, 'level_1' for the 1st level
   # bw_sel : bandwidth selection method. None correspond to the scott method. 'silverman' or others can be inquired.
   # station : object class Station containing station location
 ```
-
-
```

### Comparing `pybsrnqc-0.2.2/README.md` & `pybsrnqc-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/pybsrnqc/automaticQC.py` & `pybsrnqc-0.2.3/pybsrnqc/automaticQC.py`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/pybsrnqc/coef_calculator.py` & `pybsrnqc-0.2.3/pybsrnqc/coef_calculator.py`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/pybsrnqc/coef_study.py` & `pybsrnqc-0.2.3/pybsrnqc/coef_study.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
         # Generation of coefficient
         dic = Coef()
         dic.__setattr__(coef_name, coef)
 
         # Generation of the outliers according to the equations and the density
 
         df_lim = df.copy()
-        df_lim['flag'] = <<<<<<<<<<<<<QC>>>>>>>>>>>>>.calc_lim(df, coef=dic)[3]
+        df_lim['flag'] = QC.calc_lim(df, coef=dic)[3]
 
         if level == 'level_2':
             df_lim['out_coef'] = np.array([0] * df_lim.shape[0])
             df_lim.loc[df_lim.flag == 4, "out_coef"] = 1
         else:
             df_lim['out_coef'] = np.array([0] * df_lim.shape[0])
             df_lim.loc[(df_lim.flag == 2) | (df_lim.flag == 4), "out_coef"] = 1
@@ -393,9 +393,9 @@
 
     if QC.vary == 'downward_avg':
         print()
         print('Lower limit')
         print(line_max_min)
 
         return df_scores, line_max, df_scores_min, line_max_min
-<
+
     return df_scores, line_max
```

### Comparing `pybsrnqc-0.2.2/pybsrnqc/config.py` & `pybsrnqc-0.2.3/pybsrnqc/config.py`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/pybsrnqc/open_data.py` & `pybsrnqc-0.2.3/pybsrnqc/open_data.py`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/pybsrnqc/plot_limits.py` & `pybsrnqc-0.2.3/pybsrnqc/plot_limits.py`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/pybsrnqc/qc_functions.py` & `pybsrnqc-0.2.3/pybsrnqc/qc_functions.py`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/pybsrnqc/qcrad.py` & `pybsrnqc-0.2.3/pybsrnqc/qcrad.py`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/pybsrnqc/qcrad_conf.json` & `pybsrnqc-0.2.3/pybsrnqc/qcrad_conf.json`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/pybsrnqc/utils.py` & `pybsrnqc-0.2.3/pybsrnqc/utils.py`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/pybsrnqc/visualPlot.py` & `pybsrnqc-0.2.3/pybsrnqc/visualPlot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 from bokeh import events
 from bokeh.io import curdoc
 from bokeh.layouts import column, row
-from bokeh.models import CustomJS, HoverTool, Panel, Tabs, Button, DateFormatter
+from bokeh.models import CustomJS, HoverTool, Tabs, TabPanel, Button, DateFormatter
 from bokeh.models.widgets import DataTable, TableColumn
 from bokeh.palettes import Colorblind, Plasma
 from bokeh.plotting import ColumnDataSource, figure, output_file, show
 from os import makedirs, path
 from pandas import read_csv, to_datetime
 
 import importlib.resources
@@ -90,13 +90,13 @@
     with importlib.resources.path("pybsrnqc", "callbackSave.js") as data_path:
         f = open(data_path, "r")
     js_code = f.read()
     callback = CustomJS(args=dict(bsrnSelect=bsrnSelect), code=js_code)
     button_flag.js_on_event(events.ButtonClick, callback)
 
     # Layout
-    ltab = Panel(child=fig, title="Line")
-    stab = Panel(child=fig2, title="Scatter")
+    ltab = TabPanel(child=fig, title="Line")
+    stab = TabPanel(child=fig2, title="Scatter")
     tabs = Tabs(tabs=[ltab, stab])
     layout = row(tabs, column(tableData, button_flag))
 
     return show(layout)
```

### Comparing `pybsrnqc-0.2.2/pybsrnqc.egg-info/PKG-INFO` & `pybsrnqc-0.2.3/pybsrnqc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pybsrnqc
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package to study BSRN data and their quality control
 Home-page: https://github.com/LE2P/pybsrnqc/tree/main/pybsrnqc
 Author: Maelle Baronnet
 Author-email: maelle.baronnet@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -323,9 +322,7 @@
 ```python
 coef_calculator.compute(path=None, level='level_2', bw_sel=None, station=Station())
   # path : path of the directory with the data files
   # level : 'level_2' (default) to plot the 2nd level limits, 'level_1' for the 1st level
   # bw_sel : bandwidth selection method. None correspond to the scott method. 'silverman' or others can be inquired.
   # station : object class Station containing station location
 ```
-
-
```

### Comparing `pybsrnqc-0.2.2/pybsrnqc.egg-info/SOURCES.txt` & `pybsrnqc-0.2.3/pybsrnqc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybsrnqc-0.2.2/setup.py` & `pybsrnqc-0.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pybsrnqc',
-    version='0.2.2',
+    version='0.2.3',
     description='Package to study BSRN data and their quality control',
     url='https://github.com/LE2P/pybsrnqc/tree/main/pybsrnqc',
     author='Maelle Baronnet',
     author_email='maelle.baronnet@gmail.com',
     license='MIT',
     include_package_data=True,
     packages=['pybsrnqc'],
     install_requires=['pandas',
                       'numpy>=1.17.4',
                       'matplotlib>=3.3.2',
                       'pvlib>=0.8.0',
-                      'bokeh>=2.2.3',
+                      'bokeh==3.2.0',
                       'cryptography>=2.8',
-                      'pytz>=2019.3'
+                      'pytz>=2019.3',
+                      'scikit-learn'
                       ],
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
```

