# Comparing `tmp/lime_nda-0.0.9.tar.gz` & `tmp/lime_nda-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime_nda-0.0.9.tar", last modified: Tue Jul 11 12:46:16 2023, max compression
+gzip compressed data, was "lime_nda-0.1.0.tar", last modified: Tue Jul 11 13:08:13 2023, max compression
```

## Comparing `lime_nda-0.0.9.tar` & `lime_nda-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:46:16.036322 lime_nda-0.0.9/
--rw-rw-rw-   0        0        0    35823 2023-07-11 10:38:49.000000 lime_nda-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1805 2023-07-11 12:46:16.034636 lime_nda-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-11 10:38:49.000000 lime_nda-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 12:46:15.981416 lime_nda-0.0.9/lime_nda/
--rw-rw-rw-   0        0        0      266 2023-07-11 10:38:49.000000 lime_nda-0.0.9/lime_nda/__init__.py
--rw-rw-rw-   0        0        0    17960 2023-07-11 12:44:29.000000 lime_nda-0.0.9/lime_nda/nda_functions.py
--rw-rw-rw-   0        0        0    13742 2023-07-11 10:38:49.000000 lime_nda-0.0.9/lime_nda/nda_version_8_0.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:46:16.028648 lime_nda-0.0.9/lime_nda.egg-info/
--rw-rw-rw-   0        0        0     1805 2023-07-11 12:46:15.000000 lime_nda-0.0.9/lime_nda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-11 12:46:15.000000 lime_nda-0.0.9/lime_nda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:46:15.000000 lime_nda-0.0.9/lime_nda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 12:46:15.000000 lime_nda-0.0.9/lime_nda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      665 2023-07-11 12:45:17.000000 lime_nda-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 12:46:16.037341 lime_nda-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 13:08:13.402786 lime_nda-0.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 10:38:49.000000 lime_nda-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1805 2023-07-11 13:08:13.401468 lime_nda-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-11 10:38:49.000000 lime_nda-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 13:08:13.353948 lime_nda-0.1.0/lime_nda/
+-rw-rw-rw-   0        0        0      266 2023-07-11 10:38:49.000000 lime_nda-0.1.0/lime_nda/__init__.py
+-rw-rw-rw-   0        0        0    17875 2023-07-11 13:00:13.000000 lime_nda-0.1.0/lime_nda/nda_functions.py
+-rw-rw-rw-   0        0        0    13742 2023-07-11 10:38:49.000000 lime_nda-0.1.0/lime_nda/nda_version_8_0.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:08:13.395630 lime_nda-0.1.0/lime_nda.egg-info/
+-rw-rw-rw-   0        0        0     1805 2023-07-11 13:08:13.000000 lime_nda-0.1.0/lime_nda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-11 13:08:13.000000 lime_nda-0.1.0/lime_nda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 13:08:13.000000 lime_nda-0.1.0/lime_nda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 13:08:13.000000 lime_nda-0.1.0/lime_nda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      665 2023-07-11 13:03:04.000000 lime_nda-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 13:08:13.404173 lime_nda-0.1.0/setup.cfg
```

### Comparing `lime_nda-0.0.9/LICENSE` & `lime_nda-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lime_nda-0.0.9/PKG-INFO` & `lime_nda-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime_nda
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python Package for working with NDA files, specifically for people at Lime.AI
 Author-email: Lime CellTesting <vividhgarg@outlook.com>
 Project-URL: Homepage, https://github.com/vividh-garg/NDA
 Project-URL: Bug Tracker, https://github.com/vividh-garg/NDA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lime_nda-0.0.9/README.md` & `lime_nda-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lime_nda-0.0.9/lime_nda/nda_functions.py` & `lime_nda-0.1.0/lime_nda/nda_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,35 +121,35 @@
 
     for i in range(min(df['cycle']),max(df['cycle']+1)):                         
         # df2=df.groupby('cycle').get_group(i)
 
         df2 = df[df['cycle']==i]
         cycle=i                                                                                                                                                                           
 
-        starting_date=df2['timestamp'].head(1).values[0]
-        end_date=df2['timestamp'].tail(1).values[0]
+        starting_date=list(df2['timestamp'])[0]
+        end_date=list(df2['timestamp'])[-1]
         
         df_chg=df2[(df2['step_name']==chg_temp)]
         df_dchg=df2[(df2['step_name']==dchg_temp)]
 
         charging_capacity=max(df_chg['capacity_mAh'],default=-1)
         discharging_capacity=max(df_dchg['capacity_mAh'],default=-1)
 
         charging_energy=max(df_chg['energy_mWh'],default=-1)
         discharging_energy=max(df_dchg['energy_mWh'],default=-1)
 
-        chg_starting_volt=df_chg['voltage_V'].head(1).values[0]
-        chg_ending_volt=df_chg['voltage_V'].tail(1).values[0]
-        dchg_starting_volt=df_dchg['voltage_V'].head(1).values[0]
-        dchg_ending_volt=df_dchg['voltage_V'].tail(1).values[0]
-
-        chg_starting_current=df_chg['current_mA'].head(1).values[0]
-        chg_ending_current=df_chg['current_mA'].tail(1).values[0]
-        dchg_starting_current=df_dchg['current_mA'].head(1).values[0]
-        dchg_ending_current=df_dchg['current_mA'].tail(1).values[0]
+        chg_starting_volt=list(df_chg['voltage_V'])[0]
+        chg_ending_volt=list(df_chg['voltage_V'])[-1]
+        dchg_starting_volt=list(df_dchg['voltage_V'])[0]
+        dchg_ending_volt=list(df_dchg['voltage_V'])[-1]
+
+        chg_starting_current=list(df_chg['current_mA'])[0]
+        chg_ending_current=list(df_chg['current_mA'])[-1]
+        dchg_starting_current=list(df_dchg['current_mA'])[0]
+        dchg_ending_current=list(df_dchg['current_mA'])[-1]
 
         charging_time=timedelta(seconds=list(df_chg['time_in_step'])[-1])
         discharging_time=timedelta(seconds=list(df_dchg['time_in_step'])[-1])
 
         dcir_cyl=df2.loc[df2['DCIR']>0,'DCIR']
     
         DCIR_avg=dcir_cyl.mean()
```

### Comparing `lime_nda-0.0.9/lime_nda/nda_version_8_0.py` & `lime_nda-0.1.0/lime_nda/nda_version_8_0.py`

 * *Files identical despite different names*

### Comparing `lime_nda-0.0.9/lime_nda.egg-info/PKG-INFO` & `lime_nda-0.1.0/lime_nda.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-nda
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python Package for working with NDA files, specifically for people at Lime.AI
 Author-email: Lime CellTesting <vividhgarg@outlook.com>
 Project-URL: Homepage, https://github.com/vividh-garg/NDA
 Project-URL: Bug Tracker, https://github.com/vividh-garg/NDA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lime_nda-0.0.9/pyproject.toml` & `lime_nda-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy","pandas"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lime_nda"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Lime CellTesting", email="vividhgarg@outlook.com" },
 ]
 description = 'Python Package for working with NDA files, specifically for people at Lime.AI' 
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

