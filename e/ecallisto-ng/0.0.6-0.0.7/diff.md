# Comparing `tmp/ecallisto_ng-0.0.6.tar.gz` & `tmp/ecallisto_ng-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.0.6.tar", last modified: Mon Jul 10 17:56:58 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.0.7.tar", last modified: Tue Jul 11 08:48:50 2023, max compression
```

## Comparing `ecallisto_ng-0.0.6.tar` & `ecallisto_ng-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.6/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2773 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2192 2023-07-10 17:46:34.000000 ecallisto_ng-0.0.6/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-10 17:56:50.000000 ecallisto_ng-0.0.6/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.6/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3096 2023-07-10 16:52:06.000000 ecallisto_ng-0.0.6/src/ecallisto_ng/data_fetching/get_data.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4716 2023-07-10 17:16:31.000000 ecallisto_ng-0.0.6/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.0.6/src/ecallisto_ng/plotting/plotting_utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-10 17:56:58.697126 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2773 2023-07-10 17:56:58.000000 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      389 2023-07-10 17:56:58.000000 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-10 17:56:58.000000 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-10 17:56:58.000000 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-10 17:56:58.000000 ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.7/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2927 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2346 2023-07-11 08:39:18.000000 ecallisto_ng-0.0.7/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-11 08:48:41.000000 ecallisto_ng-0.0.7/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.7/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3096 2023-07-10 16:52:06.000000 ecallisto_ng-0.0.7/src/ecallisto_ng/data_fetching/get_data.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.0.7/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.0.7/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2927 2023-07-11 08:48:50.000000 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      380 2023-07-11 08:48:50.000000 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-11 08:48:50.000000 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-11 08:48:50.000000 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-11 08:48:50.000000 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.0.6/LICENSE` & `ecallisto_ng-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.6/PKG-INFO` & `ecallisto_ng-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-Metadata-Version: 2.1
-Name: ecallisto_ng
-Version: 0.0.6
-Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
-Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
-Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
-Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Ecallisto NG 
 Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API. 
 The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto API via the link: [https://v000792.fhnw.ch/api/data](https://v000792.fhnw.ch/api/data).
 
 ## Installation
 To install this package, clone this repository and use pip for installation. Execute the following command in your terminal:
 ```pip install -e .```
 
 ## PyPI
 Ecallisto NG is conveniently available on PyPI as well. To download, visit the following link: [https://pypi.org/project/ecallisto-ng/](https://pypi.org/project/ecallisto-ng/)
 
+## Example
+Please have a look at the jupyter notebook under `example`. 
+
 ## Usage
 Here's a guide on how to use the different features of Ecallisto NG:
 
 ### Data Fetching
 Fetching data is easy using the `get_data` function, housed under the `ecallisto_ng.data_fetching.get_data` module. Here's an example:
 
 ```python
@@ -36,31 +25,33 @@
     "instrument_name": "austria_unigraz_01",
     "start_datetime": "2021-03-01 06:30:00",
     "end_datetime": "2021-03-07 23:30:00",
     "timebucket": "15m",
     "agg_function": "MAX",
 }
 
-df = get_data(parameters)
+df = get_data(**parameters)
 ```
 
 ### Plotting 
 Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
 ```python
-from ecallisto_ng.plotting.plot import fill_missing_timesteps_with_nan, plot_spectogram
+from ecallisto_ng.plotting.utils import fill_missing_timesteps_with_nan, plot_spectogram
 
-df = fill_missing_timesteps_with_nan(df)
-plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
+df_filled = fill_missing_timesteps_with_nan(df)
+plot_spectogram(df_filled,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
 
 ### Spectogram editing
 We also provide some basic functionalities to edit the spectogram. Here's how you can do it:
 ```python
 from ecallisto_ng.data_processing.utils import elimwrongchannels, subtract_constant_background, subtract_rolling_background
 
 df = elimwrongchannels(df)
+df = fill_missing_timesteps_with_nan(df)
 df = subtract_constant_background(df)
 df = subtract_rolling_background(df)
 
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
 These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
+Be careful when using
```

### Comparing `ecallisto_ng-0.0.6/pyproject.toml` & `ecallisto_ng-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.0.6/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.0.7/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.6/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.0.7/src/ecallisto_ng/data_processing/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import pandas as pd
 from skimage import filters
 
 
 def elimwrongchannels(df, channel_std_mult=5, jump_std_mult=2):
     """
     Remove Radio Frequency Interference (RFI) from a spectrogram represented by a pandas DataFrame.
-
+    This function currently does not work when there is missing data. So it should be used before the function
+    `fill_missing_timesteps_with_nan`.
     Parameters
     ----------
     df : pandas.DataFrame
         Input DataFrame where the index represents time and the columns represent frequency channels.
     channel_std_mult : float, optional
         Multiplicative factor for the standard deviation threshold used in the first RFI elimination step.
         Channels with standard deviation less than this threshold times the mean standard deviation across all channels are retained.
@@ -82,39 +83,44 @@
         DataFrame with the constant background subtracted. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
 
     """
     df = df.copy()
     return df - df.iloc[0:n].median()
 
 
-def subtract_rolling_background(df, window=30, how="quantile", quantile_value=0.05):
+def subtract_rolling_background(df, window=30, center=False, how="quantile", quantile_value=0.05, **kwargs):
     """
     Subtract a rolling background from a spectrogram represented by a pandas DataFrame.
 
     The rolling background is calculated either as the median or a specific quantile value of each rolling window of size `window`.
 
     Parameters
     ----------
     df : pandas.DataFrame
         Input DataFrame where the index represents time and the columns represent frequency channels.
     window : int, default 30
         Size of the rolling window from which the background value is calculated.
+    center : bool, default False
+        If True, the rolling window is centered on the current timepoint. If False, the rolling window starts at the current timepoint.
+        See pandas.DataFrame.rolling for more details.
     how : str, default "median"
         Method to calculate the rolling background. If "median", the median value of the window is used.
         If "quantile", the quantile defined by `quantile_value` is used.
     quantile_value : float, default 0.5
         The quantile value to use when `how` is "quantile". Ignored if `how` is not "quantile".
+    **kwargs : dict
+        Additional keyword arguments passed to pandas.DataFrame.rolling.
 
     Returns
     -------
     pandas.DataFrame
         DataFrame with the rolling background subtracted. The DataFrame is oriented in the same way as the input DataFrame (time on index and frequency on columns).
 
     """
     df = df.copy()
     if how == "median":
-        df_rolling = df.rolling(window=window).median()
+        df_rolling = df.rolling(window=window, center=center, **kwargs).median()
     elif how == "quantile":
-        df_rolling = df.rolling(window=window).quantile(quantile_value)
+        df_rolling = df.rolling(window=window, center=center, **kwargs).quantile(quantile_value)
     else:
         raise ValueError("`how` must be 'median' or 'quantile'")
     return df - df_rolling
```

### Comparing `ecallisto_ng-0.0.6/src/ecallisto_ng/plotting/plotting_utils.py` & `ecallisto_ng-0.0.7/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.6/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ecallisto-ng
-Version: 0.0.6
+Name: ecallisto_ng
+Version: 0.0.7
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,17 @@
 ## Installation
 To install this package, clone this repository and use pip for installation. Execute the following command in your terminal:
 ```pip install -e .```
 
 ## PyPI
 Ecallisto NG is conveniently available on PyPI as well. To download, visit the following link: [https://pypi.org/project/ecallisto-ng/](https://pypi.org/project/ecallisto-ng/)
 
+## Example
+Please have a look at the jupyter notebook under `example`. 
+
 ## Usage
 Here's a guide on how to use the different features of Ecallisto NG:
 
 ### Data Fetching
 Fetching data is easy using the `get_data` function, housed under the `ecallisto_ng.data_fetching.get_data` module. Here's an example:
 
 ```python
@@ -36,31 +39,33 @@
     "instrument_name": "austria_unigraz_01",
     "start_datetime": "2021-03-01 06:30:00",
     "end_datetime": "2021-03-07 23:30:00",
     "timebucket": "15m",
     "agg_function": "MAX",
 }
 
-df = get_data(parameters)
+df = get_data(**parameters)
 ```
 
 ### Plotting 
 Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
 ```python
-from ecallisto_ng.plotting.plot import fill_missing_timesteps_with_nan, plot_spectogram
+from ecallisto_ng.plotting.utils import fill_missing_timesteps_with_nan, plot_spectogram
 
-df = fill_missing_timesteps_with_nan(df)
-plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
+df_filled = fill_missing_timesteps_with_nan(df)
+plot_spectogram(df_filled,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
 
 ### Spectogram editing
 We also provide some basic functionalities to edit the spectogram. Here's how you can do it:
 ```python
 from ecallisto_ng.data_processing.utils import elimwrongchannels, subtract_constant_background, subtract_rolling_background
 
 df = elimwrongchannels(df)
+df = fill_missing_timesteps_with_nan(df)
 df = subtract_constant_background(df)
 df = subtract_rolling_background(df)
 
 plot_spectogram(df,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
 ```
 These simple commands allow you to easily manipulate spectogram data, enabling effective use of the Ecallisto API for your needs.
+Be careful when using
```

