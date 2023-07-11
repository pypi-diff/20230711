# Comparing `tmp/ecallisto_ng-0.0.7.tar.gz` & `tmp/ecallisto_ng-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.0.7.tar", last modified: Tue Jul 11 08:48:50 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.1.0.tar", last modified: Tue Jul 11 14:51:53 2023, max compression
```

## Comparing `ecallisto_ng-0.0.7.tar` & `ecallisto_ng-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.7/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2927 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2346 2023-07-11 08:39:18.000000 ecallisto_ng-0.0.7/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-11 08:48:41.000000 ecallisto_ng-0.0.7/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.7/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3096 2023-07-10 16:52:06.000000 ecallisto_ng-0.0.7/src/ecallisto_ng/data_fetching/get_data.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.0.7/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.0.7/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 08:48:50.071461 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2927 2023-07-11 08:48:50.000000 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      380 2023-07-11 08:48:50.000000 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-11 08:48:50.000000 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-11 08:48:50.000000 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-11 08:48:50.000000 ecallisto_ng-0.0.7/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 14:51:53.792578 ecallisto_ng-0.1.0/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.0/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-11 14:51:53.792578 ecallisto_ng-0.1.0/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2967 2023-07-11 14:51:23.000000 ecallisto_ng-0.1.0/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-11 14:51:42.000000 ecallisto_ng-0.1.0/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-11 14:51:53.792578 ecallisto_ng-0.1.0/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 14:51:53.781745 ecallisto_ng-0.1.0/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 14:51:53.781745 ecallisto_ng-0.1.0/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.0/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 14:51:53.792578 ecallisto_ng-0.1.0/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3433 2023-07-11 14:37:07.000000 ecallisto_ng-0.1.0/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2005 2023-07-11 14:37:47.000000 ecallisto_ng-0.1.0/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 14:51:53.792578 ecallisto_ng-0.1.0/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.0/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 14:51:53.792578 ecallisto_ng-0.1.0/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.0/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-11 14:51:53.781745 ecallisto_ng-0.1.0/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-11 14:51:53.000000 ecallisto_ng-0.1.0/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      430 2023-07-11 14:51:53.000000 ecallisto_ng-0.1.0/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-11 14:51:53.000000 ecallisto_ng-0.1.0/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-11 14:51:53.000000 ecallisto_ng-0.1.0/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-11 14:51:53.000000 ecallisto_ng-0.1.0/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.0.7/LICENSE` & `ecallisto_ng-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.7/README.md` & `ecallisto_ng-0.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ecallisto NG 
 Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API. 
-The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto API via the link: [https://v000792.fhnw.ch/api/data](https://v000792.fhnw.ch/api/data).
+The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto API via the link: [https://v000792.fhnw.ch/api/redoc](https://v000792.fhnw.ch/api/redoc).
 
 ## Installation
 To install this package, clone this repository and use pip for installation. Execute the following command in your terminal:
 ```pip install -e .```
 
 ## PyPI
 Ecallisto NG is conveniently available on PyPI as well. To download, visit the following link: [https://pypi.org/project/ecallisto-ng/](https://pypi.org/project/ecallisto-ng/)
@@ -28,14 +28,29 @@
     "timebucket": "15m",
     "agg_function": "MAX",
 }
 
 df = get_data(**parameters)
 ```
 
+### Getting Data Availability
+You can also check the availability of data using the `get_tables` and `get_table_names_with_data_between_dates` function, housed under the `ecallisto_ng.data_fetching.get_information` module. Here's an example:
+
+```python
+from ecallisto_ng.data_fetching.get_information import get_tables, get_table_names_with_data_between_dates
+from datetime import datetime, timedelta
+
+get_tables()[:5]
+
+get_table_names_with_data_between_dates(
+    start_datetime=(datetime.now() - timedelta(hours=24)).strftime("%Y-%m-%d %H:%M:%S"),
+    end_datetime=datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+)
+```
+
 ### Plotting 
 Ecallisto NG provides basic plotting capabilities. Here's an example of how to generate a spectogram:
 ```python
 from ecallisto_ng.plotting.utils import fill_missing_timesteps_with_nan, plot_spectogram
 
 df_filled = fill_missing_timesteps_with_nan(df)
 plot_spectogram(df_filled,  parameters["instrument_name"], parameters["start_datetime"], parameters["end_datetime"])
```

### Comparing `ecallisto_ng-0.0.7/pyproject.toml` & `ecallisto_ng-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.0.7"
+version = "0.1.0"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.0.7/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.1.0/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,18 @@
         "start_datetime": start_datetime,
         "end_datetime": end_datetime,
         "timebucket": timebucket,
         "agg_function": agg_function,
         "return_type": return_type,
     }
 
+    assert pd.to_datetime(start_datetime) < pd.to_datetime(end_datetime), (
+        f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
+    )
+
     response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
 
     if response.status_code == 200:
         url = (
             response.json()["json_url"]
             if return_type == "json"
             else response.json()["fits_url"]
@@ -66,14 +70,17 @@
         while True:
             # Sleep for a short period of time to allow the data to be fetched
             time.sleep(5)
             # Check if the file is available yet
             file_response = requests.get(url)
             if file_response.status_code == 200:
                 # If the file is available, return the data
+                respone_json = file_response.json()
+                if 'error' in respone_json.keys():
+                    raise ValueError(respone_json['error'])
                 if return_type == "json":
                     df = pd.DataFrame(file_response.json())
                     return df
                 else:
                     fits_path = (
                         f"{instrument_name}_{start_datetime}_{end_datetime}.fits"
                     )
@@ -83,7 +90,8 @@
             elif file_response.status_code == 404:
                 # If the file is not found, continue waiting
                 continue
             else:
                 raise ValueError(f"Error getting file from API: {file_response.text}")
     else:
         raise ValueError(f"Error getting data from API: {response.text}")
+
```

### Comparing `ecallisto_ng-0.0.7/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.1.0/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.7/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.1.0/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

