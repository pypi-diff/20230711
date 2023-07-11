# Comparing `tmp/sintef-pyshop-1.4.2.tar.gz` & `tmp/sintef-pyshop-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sintef-pyshop-1.4.2.tar", last modified: Wed Jul  5 14:12:37 2023, max compression
+gzip compressed data, was "sintef-pyshop-1.4.3.tar", last modified: Tue Jul 11 08:08:51 2023, max compression
```

## Comparing `sintef-pyshop-1.4.2.tar` & `sintef-pyshop-1.4.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.172171 sintef-pyshop-1.4.2/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6128 2023-07-05 14:12:37.171172 sintef-pyshop-1.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5070 2023-07-05 14:04:50.000000 sintef-pyshop-1.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.147171 sintef-pyshop-1.4.2/pyshop/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.151171 sintef-pyshop-1.4.2/pyshop/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/helpers/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/helpers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/helpers/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/helpers/typing_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.155171 sintef-pyshop-1.4.2/pyshop/lp_model/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/lp_model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/lp_model/index.py
--rw-rw-rw-   0 root         (0) root         (0)     2555 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/lp_model/lp_model.py
--rw-rw-rw-   0 root         (0) root         (0)    10661 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/lp_model/row.py
--rw-rw-rw-   0 root         (0) root         (0)     9366 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/lp_model/var.py
--rw-rw-rw-   0 root         (0) root         (0)    13751 2023-06-08 08:59:06.000000 sintef-pyshop-1.4.2/pyshop/shop_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.163171 sintef-pyshop-1.4.2/pyshop/shopcore/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/shopcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/shopcore/command_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    24862 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/shopcore/model_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    12969 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/shopcore/script_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    15145 2023-07-05 14:04:50.000000 sintef-pyshop-1.4.2/pyshop/shopcore/shop_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/pyshop/shopcore/shop_rest.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 14:12:37.172171 sintef-pyshop-1.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1882 2023-06-07 13:14:22.000000 sintef-pyshop-1.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.167171 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6128 2023-07-05 14:12:37.000000 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      790 2023-07-05 14:12:37.000000 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 14:12:37.000000 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-05 14:12:37.000000 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-05 14:12:37.000000 sintef-pyshop-1.4.2/sintef_pyshop.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:12:37.170171 sintef-pyshop-1.4.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/tests/test_helpers_command.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-10 06:30:08.000000 sintef-pyshop-1.4.2/tests/test_helpers_time.py
--rw-rw-rw-   0 root         (0) root         (0)     8163 2023-07-05 14:04:50.000000 sintef-pyshop-1.4.2/tests/test_shop_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.608825 sintef-pyshop-1.4.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-07-11 08:08:51.607825 sintef-pyshop-1.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-07-04 11:41:21.000000 sintef-pyshop-1.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.576824 sintef-pyshop-1.4.3/pyshop/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.3/pyshop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.582824 sintef-pyshop-1.4.3/pyshop/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.3/pyshop/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.3/pyshop/helpers/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.3/pyshop/helpers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/helpers/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/helpers/typing_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.596825 sintef-pyshop-1.4.3/pyshop/lp_model/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/lp_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/lp_model/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/lp_model/lp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10661 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/lp_model/row.py
+-rw-rw-rw-   0 root         (0) root         (0)     9366 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/lp_model/var.py
+-rw-rw-rw-   0 root         (0) root         (0)    13751 2023-06-08 08:57:15.000000 sintef-pyshop-1.4.3/pyshop/shop_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.602825 sintef-pyshop-1.4.3/pyshop/shopcore/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/shopcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/shopcore/command_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    24862 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/shopcore/model_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    13037 2023-07-11 08:08:40.000000 sintef-pyshop-1.4.3/pyshop/shopcore/script_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    15169 2023-07-11 08:08:40.000000 sintef-pyshop-1.4.3/pyshop/shopcore/shop_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/pyshop/shopcore/shop_rest.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 08:08:51.608825 sintef-pyshop-1.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2023-06-07 13:27:40.000000 sintef-pyshop-1.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.604825 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-07-11 08:08:51.000000 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-07-11 08:08:51.000000 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 08:08:51.000000 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-11 08:08:51.000000 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 08:08:51.000000 sintef-pyshop-1.4.3/sintef_pyshop.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:08:51.606825 sintef-pyshop-1.4.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/tests/test_helpers_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.3/tests/test_helpers_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     8163 2023-07-05 14:05:21.000000 sintef-pyshop-1.4.3/tests/test_shop_api.py
```

### Comparing `sintef-pyshop-1.4.2/LICENSE` & `sintef-pyshop-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/PKG-INFO` & `sintef-pyshop-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
```

### Comparing `sintef-pyshop-1.4.2/README.md` & `sintef-pyshop-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/helpers/commands.py` & `sintef-pyshop-1.4.3/pyshop/helpers/commands.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/helpers/time.py` & `sintef-pyshop-1.4.3/pyshop/helpers/time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/helpers/timeseries.py` & `sintef-pyshop-1.4.3/pyshop/helpers/timeseries.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/helpers/typing_annotations.py` & `sintef-pyshop-1.4.3/pyshop/helpers/typing_annotations.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/lp_model/index.py` & `sintef-pyshop-1.4.3/pyshop/lp_model/index.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/lp_model/lp_model.py` & `sintef-pyshop-1.4.3/pyshop/lp_model/lp_model.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/lp_model/row.py` & `sintef-pyshop-1.4.3/pyshop/lp_model/row.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/lp_model/var.py` & `sintef-pyshop-1.4.3/pyshop/lp_model/var.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/shop_runner.py` & `sintef-pyshop-1.4.3/pyshop/shop_runner.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/shopcore/command_builder.py` & `sintef-pyshop-1.4.3/pyshop/shopcore/command_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/shopcore/model_builder.py` & `sintef-pyshop-1.4.3/pyshop/shopcore/model_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/pyshop/shopcore/script_generator.py` & `sintef-pyshop-1.4.3/pyshop/shopcore/script_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,18 @@
                     f.write("    xyt = []\n")
                     for xy in val:               
                         f.write(f"    x = {list(xy.index)}\n")
                         f.write(f"    y = {list(xy.values)}\n")
                         f.write(f"    xyt.append(pd.Series(y,index=x,name=Timestamp('{str(xy.name)}')))\n")
                     f.write(f"    {var_name}.{attr}.set(xyt)\n")                                                                   
                 elif dtype == "txy":
-                    val = remove_consecutive_duplicates(val)
+
+                    if time_res['starttime'] <= val.index[0]:
+                        val = remove_consecutive_duplicates(val)
+
                     if len(val.values) > 1:
                         f.write(f"    t = {list(val.index)}\n")
                         f.write(f"    {attr} = {list(val.values)}\n")
                         f.write(f"    {var_name}.{attr}.set(pd.Series({attr},index=t))\n")                  
                     #Use simple syntax if there is only one value in the txy
                     else:
                         f.write(f"    {var_name}.{attr}.set({val.values[0]})\n")
```

### Comparing `sintef-pyshop-1.4.2/pyshop/shopcore/shop_api.py` & `sintef-pyshop-1.4.3/pyshop/shopcore/shop_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,15 @@
 
         #If the dataframe is of length one, it is equivalent to setting a constant value starting at the txy start time
         if len(df.index) == 1:
             shop_api.SetTxySeries(object_type, object_name, attribute_name, txy_start_str, np.array([0]), df.values)
             return
 
         #Time vector in seconds
-        t = np.array([(t-txy_start_time).seconds for t in df.index])
+        t = np.array([(t-txy_start_time).total_seconds() for t in df.index])
 
         #Convert to the time unit of the optimization
         if time['timeunit'] == 'minute':
             t = t * 1.0/60
         elif time['timeunit'] == 'hour':
             t = t * 1.0/3600
 
@@ -297,18 +297,18 @@
             print(f"""Warning: TXY {attribute_name} on {object_type} {object_name} has higher resolution than the time unit of the optimization. 
                   Resampling will be done with averaging and front fill, precision may be lost""")
 
             #Resample time series with the time unit used in the optimization
             #Take the average when a lot of data is given within a single time step
             if time['timeunit'] == 'minute':
                 df = df.resample("min").mean().ffill()
-                t = np.array([(t-txy_start_time).seconds/60.0 for t in df.index])
+                t = np.array([(t-txy_start_time).total_seconds()/60.0 for t in df.index])
             elif time['timeunit'] == 'hour':
                 df = df.resample("H").mean().ffill()
-                t = np.array([(t-txy_start_time).seconds/3600.0 for t in df.index])
+                t = np.array([(t-txy_start_time).total_seconds()/3600.0 for t in df.index])
  
         shop_api.SetTxySeries(object_type, object_name, attribute_name, txy_start_str, t.astype(int), df.values)
 
 
 def get_time_resolution(shop_api:ShopApi) -> Dict[str,Any]:
     tz_name = get_shop_timzone_name(shop_api)
     starttime = get_shop_datetime(shop_api.GetStartTime(), tz_name)
```

### Comparing `sintef-pyshop-1.4.2/pyshop/shopcore/shop_rest.py` & `sintef-pyshop-1.4.3/pyshop/shopcore/shop_rest.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/setup.py` & `sintef-pyshop-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/sintef_pyshop.egg-info/PKG-INFO` & `sintef-pyshop-1.4.3/sintef_pyshop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
```

### Comparing `sintef-pyshop-1.4.2/sintef_pyshop.egg-info/SOURCES.txt` & `sintef-pyshop-1.4.3/sintef_pyshop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/tests/test_helpers_command.py` & `sintef-pyshop-1.4.3/tests/test_helpers_command.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/tests/test_helpers_time.py` & `sintef-pyshop-1.4.3/tests/test_helpers_time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.2/tests/test_shop_api.py` & `sintef-pyshop-1.4.3/tests/test_shop_api.py`

 * *Files identical despite different names*

