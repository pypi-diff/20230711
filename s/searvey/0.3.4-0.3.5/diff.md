# Comparing `tmp/searvey-0.3.4-py3-none-any.whl.zip` & `tmp/searvey-0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 43235 bytes, number of entries: 18
+Zip file size: 43269 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      372 b- defN 80-Jan-01 00:00 searvey/__init__.py
--rw-r--r--  2.0 unx    35798 b- defN 80-Jan-01 00:00 searvey/coops.py
+-rw-r--r--  2.0 unx    35796 b- defN 80-Jan-01 00:00 searvey/coops.py
 -rw-r--r--  2.0 unx     2497 b- defN 80-Jan-01 00:00 searvey/critech.py
 -rw-r--r--  2.0 unx      462 b- defN 80-Jan-01 00:00 searvey/custom_types.py
 -rw-r--r--  2.0 unx     2513 b- defN 80-Jan-01 00:00 searvey/erddap.py
 -rw-r--r--  2.0 unx    12611 b- defN 80-Jan-01 00:00 searvey/ioc.py
 -rw-r--r--  2.0 unx     1389 b- defN 80-Jan-01 00:00 searvey/models.py
 -rw-r--r--  2.0 unx     4405 b- defN 80-Jan-01 00:00 searvey/multi.py
 -rw-r--r--  2.0 unx      975 b- defN 80-Jan-01 00:00 searvey/rate_limit.py
--rw-r--r--  2.0 unx     5122 b- defN 80-Jan-01 00:00 searvey/stations.py
+-rw-r--r--  2.0 unx     5244 b- defN 80-Jan-01 00:00 searvey/stations.py
 -rw-r--r--  2.0 unx     2896 b- defN 80-Jan-01 00:00 searvey/uhslc.py
 -rw-r--r--  2.0 unx     1358 b- defN 80-Jan-01 00:00 searvey/us_states.json
 -rw-r--r--  2.0 unx    13116 b- defN 80-Jan-01 00:00 searvey/usgs.py
 -rw-r--r--  2.0 unx     4751 b- defN 80-Jan-01 00:00 searvey/utils.py
--rw-r--r--  2.0 unx    35145 b- defN 80-Jan-01 00:00 searvey-0.3.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     4051 b- defN 80-Jan-01 00:00 searvey-0.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 searvey-0.3.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1342 b- defN 16-Jan-01 00:00 searvey-0.3.4.dist-info/RECORD
-18 files, 128891 bytes uncompressed, 41103 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx    35145 b- defN 80-Jan-01 00:00 searvey-0.3.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4051 b- defN 80-Jan-01 00:00 searvey-0.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 searvey-0.3.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1342 b- defN 16-Jan-01 00:00 searvey-0.3.5.dist-info/RECORD
+18 files, 129011 bytes uncompressed, 41137 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: searvey/usgs.py
 Comment: 
 
 Filename: searvey/utils.py
 Comment: 
 
-Filename: searvey-0.3.4.dist-info/LICENSE
+Filename: searvey-0.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: searvey-0.3.4.dist-info/METADATA
+Filename: searvey-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: searvey-0.3.4.dist-info/WHEEL
+Filename: searvey-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: searvey-0.3.4.dist-info/RECORD
+Filename: searvey-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## searvey/coops.py

```diff
@@ -817,18 +817,17 @@
     8720625  RCYF1     Racy Point, St Johns River    FL  discontinued  2019-08-05 14:00:00,2017-06-14 15:36:00,2017-0...  POINT (-81.56250 29.79688)
     8423898  FTPN3                     Fort Point    NH  discontinued  2020-04-13 00:00:00,2014-08-05 00:00:00,2012-0...  POINT (-70.68750 43.06250)
     8726667  MCYF1             Mckay Bay Entrance    FL  discontinued  2020-05-20 00:00:00,2019-03-08 00:00:00,2017-0...  POINT (-82.43750 27.90625)
     [164 rows x 6 columns]
     """
 
     stations = coops_stations(station_status=station_status)
-    if region:
+    if region is not None:
         return stations[stations.within(region)]
-    else:
-        return stations
+    return stations
 
 
 def coops_stations_within_bounds(
     minx: float,
     miny: float,
     maxx: float,
     maxy: float,
```

## searvey/stations.py

```diff
@@ -47,14 +47,16 @@
     now_utc = datetime.datetime.now(datetime.timezone.utc)
     activity_threshold_ts = now_utc - activity_threshold
 
     # Get full metadata
     ioc_gdf = ioc.get_ioc_stations(region=region)
 
     # Normalize IOC
+    # Drop delay `NA'` : https://github.com/oceanmodeling/searvey/issues/91
+    ioc_gdf = ioc_gdf[ioc_gdf.delay != "NA'"]
     # Convert delay to minutes
     ioc_gdf = ioc_gdf.assign(
         delay=pd.concat(
             (
                 ioc_gdf.delay[ioc_gdf.delay.str.endswith("'")].str[:-1].astype(int),
                 ioc_gdf.delay[ioc_gdf.delay.str.endswith("h")].str[:-1].astype(int) * 60,
                 ioc_gdf.delay[ioc_gdf.delay.str.endswith("d")].str[:-1].astype(int) * 24 * 60,
```

## Comparing `searvey-0.3.4.dist-info/LICENSE` & `searvey-0.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `searvey-0.3.4.dist-info/METADATA` & `searvey-0.3.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searvey
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Home-page: https://github.com/oceanmodeling/searvey.git
 License: GPL-3.0-or-later
 Author: Panos Mavrogiorgos
 Author-email: pmav99@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

## Comparing `searvey-0.3.4.dist-info/RECORD` & `searvey-0.3.5.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 searvey/__init__.py,sha256=tGsvJhmuYSykgwKFvDGTXiKFsQg3F1Fj8wWQPsiNzgw,372
-searvey/coops.py,sha256=eHTIchEA51w4twMWVyHA0w7-KGRT0mL9cwMbOXar34w,35798
+searvey/coops.py,sha256=E_ugI3VAp-4PkVv2cmaL9GBxKiIOGHYvVTXMiTlsbZM,35796
 searvey/critech.py,sha256=rlHWrtAKdFza9N7GMoKltvslqmkmdRdutsbxKIcD7Jg,2497
 searvey/custom_types.py,sha256=H0bQOND1rGkFxr2nLK8Q-Z0YzgebhERfhxv8MNUAiFQ,462
 searvey/erddap.py,sha256=1vZr_D-r3SqK56N65kYgpbAg-6xi3_wFQekw4s8lMeM,2513
 searvey/ioc.py,sha256=O68KB54QVJCjsNIR15MN8AAzKt23KY31Wjjan8EhLR8,12611
 searvey/models.py,sha256=fmRVoh9pnYE9nUzp1n53fkJVWPvJU3E38qmCZn0u5qk,1389
 searvey/multi.py,sha256=0ueJdcyqVpj3PSEhGQkO1UEVl5jBjrdPaOz7NM-lneg,4405
 searvey/rate_limit.py,sha256=DgvKX8Ww1qej2gZrJquoetHi9vSk4ErI6iTYQ3oGTdA,975
-searvey/stations.py,sha256=nlHO4iu43534t79agbNNWnZDbN13eIw_SJMlob5MN6A,5122
+searvey/stations.py,sha256=7s97dZLNwZ2DQd6Luo7YD1TnmmLj6dvUmqH6rJIZdZ8,5244
 searvey/uhslc.py,sha256=i4g2O-ie3gj6IPzpsS9ySSbMl9YtU_cGBXs_qoyt1VA,2896
 searvey/us_states.json,sha256=EBZm8uzX4PWgD1kgg2hBR-TEl2QbduSq2tG9sekOywE,1358
 searvey/usgs.py,sha256=Qpw_DTP8CtGqDcCuKKHvmA2zG1d6jjSUXsYy5_OKfhA,13116
 searvey/utils.py,sha256=xQ_c6SrfYgOutLo2dV9-neD6I6dT-Xk4sdRctiWVjKY,4751
-searvey-0.3.4.dist-info/LICENSE,sha256=CsWICdCWFNMlGUJiXuxfrxFHw1uyVPns0jZJmzcWkjI,35145
-searvey-0.3.4.dist-info/METADATA,sha256=ZQXTuQaAY6YFM6AADfvTqhygn4P8YBNwbDHjXNKwkzI,4051
-searvey-0.3.4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-searvey-0.3.4.dist-info/RECORD,,
+searvey-0.3.5.dist-info/LICENSE,sha256=CsWICdCWFNMlGUJiXuxfrxFHw1uyVPns0jZJmzcWkjI,35145
+searvey-0.3.5.dist-info/METADATA,sha256=c81toHrinG8WuKK5QWfH84alr2KmRocm5LWK5R8KVLA,4051
+searvey-0.3.5.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+searvey-0.3.5.dist-info/RECORD,,
```

