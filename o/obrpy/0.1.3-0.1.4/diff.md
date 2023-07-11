# Comparing `tmp/obrpy-0.1.3.tar.gz` & `tmp/obrpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obrpy-0.1.3.tar", last modified: Tue Jul 11 12:07:32 2023, max compression
+gzip compressed data, was "obrpy-0.1.4.tar", last modified: Tue Jul 11 12:11:25 2023, max compression
```

## Comparing `obrpy-0.1.3.tar` & `obrpy-0.1.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:07:32.226841 obrpy-0.1.3/
--rw-rw-rw-   0        0        0      283 2023-07-11 12:07:32.226841 obrpy-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 12:07:23.777505 obrpy-0.1.3/obrpy/
-drwxrwxrwx   0        0        0        0 2023-07-11 12:07:23.809503 obrpy-0.1.3/obrpy/ANALYSIS/
--rw-rw-rw-   0        0        0     9204 2023-05-30 09:48:03.000000 obrpy-0.1.3/obrpy/ANALYSIS/global_analysis.py
--rw-rw-rw-   0        0        0     8127 2023-07-11 12:03:35.000000 obrpy-0.1.3/obrpy/ANALYSIS/local_analysis.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:07:23.817927 obrpy-0.1.3/obrpy/SIGNAL/
--rw-rw-rw-   0        0        0     4869 2023-06-20 13:21:44.000000 obrpy-0.1.3/obrpy/SIGNAL/cross_spectrum.py
--rw-rw-rw-   0        0        0     4804 2023-06-20 13:20:49.000000 obrpy-0.1.3/obrpy/SIGNAL/spectral_shift.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:07:23.817927 obrpy-0.1.3/obrpy/UTILS/
--rw-rw-rw-   0        0        0    11916 2023-06-05 08:24:09.000000 obrpy-0.1.3/obrpy/UTILS/read_OBR.py
--rw-rw-rw-   0        0        0    11436 2023-06-19 11:27:53.000000 obrpy-0.1.3/obrpy/UTILS/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:07:23.817927 obrpy-0.1.3/obrpy/ZERO_LAYERS/
--rw-rw-rw-   0        0        0      908 2023-06-20 13:34:29.000000 obrpy-0.1.3/obrpy/ZERO_LAYERS/psss.py
--rw-rw-rw-   0        0        0    16219 2023-07-11 08:56:44.000000 obrpy-0.1.3/obrpy/__init__.py
--rw-rw-rw-   0        0        0     1447 2023-06-20 07:02:11.000000 obrpy-0.1.3/obrpy/checkouts.py
--rw-rw-rw-   0        0        0      195 2023-06-20 06:55:40.000000 obrpy-0.1.3/obrpy/clear.py
--rw-rw-rw-   0        0        0      683 2023-06-19 10:46:23.000000 obrpy-0.1.3/obrpy/fuego.py
--rw-rw-rw-   0        0        0     1347 2023-06-19 10:11:39.000000 obrpy-0.1.3/obrpy/gui.py
--rw-rw-rw-   0        0        0     1531 2023-06-21 10:56:37.000000 obrpy-0.1.3/obrpy/load.py
--rw-rw-rw-   0        0        0     7636 2023-07-11 08:56:44.000000 obrpy-0.1.3/obrpy/obr.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:07:32.145458 obrpy-0.1.3/obrpy/obrsdk/
--rw-rw-rw-   0        0        0    73728 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/CommandProcessor.dll
--rw-rw-rw-   0        0        0    53248 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/CyUSBComm.dll
--rw-rw-rw-   0        0        0   217088 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/KL2DLL32.DLL
--rw-rw-rw-   0        0        0   282624 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/LtCore.dll
--rw-rw-rw-   0        0        0 24322048 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/LtMath.dll
--rw-rw-rw-   0        0        0   110592 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/Phoenix.dll
--rw-rw-rw-   0        0        0   106496 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/RemoteInterface.dll
--rw-rw-rw-   0        0        0    57344 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/boost_date_time-mt.dll
--rw-rw-rw-   0        0        0    77824 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/boost_filesystem-mt.dll
--rw-rw-rw-   0        0        0    11776 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/boost_system-mt.dll
--rw-rw-rw-   0        0        0    53248 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/boost_thread-mt.dll
--rw-rw-rw-   0        0        0   756640 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/libiomp5md.dll
--rwxrwxrwx   0        0        0    66560 2023-04-25 11:55:06.000000 obrpy-0.1.3/obrpy/obrsdk/obr.exe
--rw-rw-rw-   0        0        0   466944 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/ova32.dll
--rw-rw-rw-   0        0        0   100692 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/ova32.lib
--rw-rw-rw-   0        0        0    28672 2023-04-25 10:36:31.000000 obrpy-0.1.3/obrpy/obrsdk/ovaGUI.dll
--rw-rw-rw-   0        0        0     2123 2023-04-25 15:28:15.000000 obrpy-0.1.3/obrpy/obrsdk.py
--rw-rw-rw-   0        0        0      972 2023-06-05 07:51:39.000000 obrpy-0.1.3/obrpy/save.py
--rw-rw-rw-   0        0        0     3390 2023-07-11 08:56:44.000000 obrpy-0.1.3/obrpy/settings.py
--rw-rw-rw-   0        0        0     3481 2023-06-20 08:20:09.000000 obrpy-0.1.3/obrpy/take_a_look.py
--rw-rw-rw-   0        0        0     1849 2023-07-04 09:10:10.000000 obrpy-0.1.3/obrpy/to_export.py
--rw-rw-rw-   0        0        0     1073 2023-06-21 10:56:29.000000 obrpy-0.1.3/obrpy/to_import.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:07:23.809503 obrpy-0.1.3/obrpy.egg-info/
--rw-rw-rw-   0        0        0      283 2023-07-11 12:07:23.000000 obrpy-0.1.3/obrpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1310 2023-07-11 12:07:23.000000 obrpy-0.1.3/obrpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:07:23.000000 obrpy-0.1.3/obrpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      445 2023-07-11 12:07:23.000000 obrpy-0.1.3/obrpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-11 12:07:23.000000 obrpy-0.1.3/obrpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 12:07:32.226841 obrpy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2035 2023-07-11 12:04:12.000000 obrpy-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:07:32.226841 obrpy-0.1.3/test/
--rw-rw-rw-   0        0        0     1039 2023-06-01 11:42:02.000000 obrpy-0.1.3/test/test.py
--rw-rw-rw-   0        0        0      986 2023-07-04 08:52:43.000000 obrpy-0.1.3/test/test_dataset.py
--rw-rw-rw-   0        0        0     2576 2023-06-19 10:59:54.000000 obrpy-0.1.3/test/test_export_obrfiles.py
--rw-rw-rw-   0        0        0      624 2023-06-19 11:01:21.000000 obrpy-0.1.3/test/test_export_settings.py
--rw-rw-rw-   0        0        0      622 2023-06-19 11:11:13.000000 obrpy-0.1.3/test/test_export_slices.py
--rw-rw-rw-   0        0        0     5988 2023-07-11 09:08:46.000000 obrpy-0.1.3/test/test_import.py
--rw-rw-rw-   0        0        0     3082 2023-07-03 08:50:22.000000 obrpy-0.1.3/test/test_linked_attr.py
--rw-rw-rw-   0        0        0     1792 2023-06-20 10:57:12.000000 obrpy-0.1.3/test/test_obr_ini.py
--rw-rw-rw-   0        0        0      432 2023-06-20 14:17:15.000000 obrpy-0.1.3/test/test_psss_dataset.py
--rw-rw-rw-   0        0        0      700 2023-06-20 13:35:30.000000 obrpy-0.1.3/test/test_slices.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:11:25.144841 obrpy-0.1.4/
+-rw-rw-rw-   0        0        0      283 2023-07-11 12:11:25.144841 obrpy-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 12:11:25.023667 obrpy-0.1.4/obrpy/
+drwxrwxrwx   0        0        0        0 2023-07-11 12:11:25.039667 obrpy-0.1.4/obrpy/ANALYSIS/
+-rw-rw-rw-   0        0        0     9204 2023-05-30 09:48:03.000000 obrpy-0.1.4/obrpy/ANALYSIS/global_analysis.py
+-rw-rw-rw-   0        0        0     8061 2023-07-11 12:10:19.000000 obrpy-0.1.4/obrpy/ANALYSIS/local_analysis.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:11:25.047663 obrpy-0.1.4/obrpy/SIGNAL/
+-rw-rw-rw-   0        0        0     4869 2023-06-20 13:21:44.000000 obrpy-0.1.4/obrpy/SIGNAL/cross_spectrum.py
+-rw-rw-rw-   0        0        0     4804 2023-06-20 13:20:49.000000 obrpy-0.1.4/obrpy/SIGNAL/spectral_shift.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:11:25.047663 obrpy-0.1.4/obrpy/UTILS/
+-rw-rw-rw-   0        0        0    11916 2023-06-05 08:24:09.000000 obrpy-0.1.4/obrpy/UTILS/read_OBR.py
+-rw-rw-rw-   0        0        0    11436 2023-06-19 11:27:53.000000 obrpy-0.1.4/obrpy/UTILS/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:11:25.047663 obrpy-0.1.4/obrpy/ZERO_LAYERS/
+-rw-rw-rw-   0        0        0      908 2023-06-20 13:34:29.000000 obrpy-0.1.4/obrpy/ZERO_LAYERS/psss.py
+-rw-rw-rw-   0        0        0    16219 2023-07-11 08:56:44.000000 obrpy-0.1.4/obrpy/__init__.py
+-rw-rw-rw-   0        0        0     1447 2023-06-20 07:02:11.000000 obrpy-0.1.4/obrpy/checkouts.py
+-rw-rw-rw-   0        0        0      195 2023-06-20 06:55:40.000000 obrpy-0.1.4/obrpy/clear.py
+-rw-rw-rw-   0        0        0      683 2023-06-19 10:46:23.000000 obrpy-0.1.4/obrpy/fuego.py
+-rw-rw-rw-   0        0        0     1347 2023-06-19 10:11:39.000000 obrpy-0.1.4/obrpy/gui.py
+-rw-rw-rw-   0        0        0     1531 2023-06-21 10:56:37.000000 obrpy-0.1.4/obrpy/load.py
+-rw-rw-rw-   0        0        0     7636 2023-07-11 08:56:44.000000 obrpy-0.1.4/obrpy/obr.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:11:25.128844 obrpy-0.1.4/obrpy/obrsdk/
+-rw-rw-rw-   0        0        0    73728 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/CommandProcessor.dll
+-rw-rw-rw-   0        0        0    53248 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/CyUSBComm.dll
+-rw-rw-rw-   0        0        0   217088 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/KL2DLL32.DLL
+-rw-rw-rw-   0        0        0   282624 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/LtCore.dll
+-rw-rw-rw-   0        0        0 24322048 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/LtMath.dll
+-rw-rw-rw-   0        0        0   110592 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/Phoenix.dll
+-rw-rw-rw-   0        0        0   106496 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/RemoteInterface.dll
+-rw-rw-rw-   0        0        0    57344 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/boost_date_time-mt.dll
+-rw-rw-rw-   0        0        0    77824 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/boost_filesystem-mt.dll
+-rw-rw-rw-   0        0        0    11776 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/boost_system-mt.dll
+-rw-rw-rw-   0        0        0    53248 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/boost_thread-mt.dll
+-rw-rw-rw-   0        0        0   756640 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/libiomp5md.dll
+-rwxrwxrwx   0        0        0    66560 2023-04-25 11:55:06.000000 obrpy-0.1.4/obrpy/obrsdk/obr.exe
+-rw-rw-rw-   0        0        0   466944 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/ova32.dll
+-rw-rw-rw-   0        0        0   100692 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/ova32.lib
+-rw-rw-rw-   0        0        0    28672 2023-04-25 10:36:31.000000 obrpy-0.1.4/obrpy/obrsdk/ovaGUI.dll
+-rw-rw-rw-   0        0        0     2123 2023-04-25 15:28:15.000000 obrpy-0.1.4/obrpy/obrsdk.py
+-rw-rw-rw-   0        0        0      972 2023-06-05 07:51:39.000000 obrpy-0.1.4/obrpy/save.py
+-rw-rw-rw-   0        0        0     3390 2023-07-11 08:56:44.000000 obrpy-0.1.4/obrpy/settings.py
+-rw-rw-rw-   0        0        0     3481 2023-06-20 08:20:09.000000 obrpy-0.1.4/obrpy/take_a_look.py
+-rw-rw-rw-   0        0        0     1849 2023-07-04 09:10:10.000000 obrpy-0.1.4/obrpy/to_export.py
+-rw-rw-rw-   0        0        0     1073 2023-06-21 10:56:29.000000 obrpy-0.1.4/obrpy/to_import.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:11:25.039667 obrpy-0.1.4/obrpy.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-07-11 12:11:24.000000 obrpy-0.1.4/obrpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1310 2023-07-11 12:11:24.000000 obrpy-0.1.4/obrpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 12:11:24.000000 obrpy-0.1.4/obrpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      445 2023-07-11 12:11:24.000000 obrpy-0.1.4/obrpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 12:11:24.000000 obrpy-0.1.4/obrpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 12:11:25.144841 obrpy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2035 2023-07-11 12:11:20.000000 obrpy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:11:25.144841 obrpy-0.1.4/test/
+-rw-rw-rw-   0        0        0     1039 2023-06-01 11:42:02.000000 obrpy-0.1.4/test/test.py
+-rw-rw-rw-   0        0        0      986 2023-07-04 08:52:43.000000 obrpy-0.1.4/test/test_dataset.py
+-rw-rw-rw-   0        0        0     2576 2023-06-19 10:59:54.000000 obrpy-0.1.4/test/test_export_obrfiles.py
+-rw-rw-rw-   0        0        0      624 2023-06-19 11:01:21.000000 obrpy-0.1.4/test/test_export_settings.py
+-rw-rw-rw-   0        0        0      622 2023-06-19 11:11:13.000000 obrpy-0.1.4/test/test_export_slices.py
+-rw-rw-rw-   0        0        0     5988 2023-07-11 09:08:46.000000 obrpy-0.1.4/test/test_import.py
+-rw-rw-rw-   0        0        0     3082 2023-07-03 08:50:22.000000 obrpy-0.1.4/test/test_linked_attr.py
+-rw-rw-rw-   0        0        0     1792 2023-06-20 10:57:12.000000 obrpy-0.1.4/test/test_obr_ini.py
+-rw-rw-rw-   0        0        0      432 2023-06-20 14:17:15.000000 obrpy-0.1.4/test/test_psss_dataset.py
+-rw-rw-rw-   0        0        0      700 2023-06-20 13:35:30.000000 obrpy-0.1.4/test/test_slices.py
```

### Comparing `obrpy-0.1.3/obrpy/ANALYSIS/global_analysis.py` & `obrpy-0.1.4/obrpy/ANALYSIS/global_analysis.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/ANALYSIS/local_analysis.py` & `obrpy-0.1.4/obrpy/ANALYSIS/local_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,14 @@
             'delta'             : delta,
             'window'            : window,
             'date'              : time.strftime("%Y,%m,%d,%H:%M:%S"),
             'parent_file'       : OBRfile.ID,
             'P'                 : P[i-window:i+window],
             'S'                 : S[i-window:i+window]}
 
-            for e in new_row.keys():
-                print(e)
-
             # Append new row
             new_information = pd.concat([new_information, pd.DataFrame([new_row])], ignore_index=True)
 
             # Append new element
             slice_obj = self.Slice()
             for val in column_names:
                 setattr(slice_obj, val, new_row[val])
```

### Comparing `obrpy-0.1.3/obrpy/SIGNAL/cross_spectrum.py` & `obrpy-0.1.4/obrpy/SIGNAL/cross_spectrum.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/SIGNAL/spectral_shift.py` & `obrpy-0.1.4/obrpy/SIGNAL/spectral_shift.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/UTILS/read_OBR.py` & `obrpy-0.1.4/obrpy/UTILS/read_OBR.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/UTILS/utils.py` & `obrpy-0.1.4/obrpy/UTILS/utils.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/ZERO_LAYERS/psss.py` & `obrpy-0.1.4/obrpy/ZERO_LAYERS/psss.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/__init__.py` & `obrpy-0.1.4/obrpy/__init__.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/checkouts.py` & `obrpy-0.1.4/obrpy/checkouts.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/fuego.py` & `obrpy-0.1.4/obrpy/fuego.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/gui.py` & `obrpy-0.1.4/obrpy/gui.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/load.py` & `obrpy-0.1.4/obrpy/load.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obr.py` & `obrpy-0.1.4/obrpy/obr.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/CommandProcessor.dll` & `obrpy-0.1.4/obrpy/obrsdk/CommandProcessor.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/CyUSBComm.dll` & `obrpy-0.1.4/obrpy/obrsdk/CyUSBComm.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/KL2DLL32.DLL` & `obrpy-0.1.4/obrpy/obrsdk/KL2DLL32.DLL`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/LtCore.dll` & `obrpy-0.1.4/obrpy/obrsdk/LtCore.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/LtMath.dll` & `obrpy-0.1.4/obrpy/obrsdk/LtMath.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/Phoenix.dll` & `obrpy-0.1.4/obrpy/obrsdk/Phoenix.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/RemoteInterface.dll` & `obrpy-0.1.4/obrpy/obrsdk/RemoteInterface.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/boost_date_time-mt.dll` & `obrpy-0.1.4/obrpy/obrsdk/boost_date_time-mt.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/boost_filesystem-mt.dll` & `obrpy-0.1.4/obrpy/obrsdk/boost_filesystem-mt.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/boost_system-mt.dll` & `obrpy-0.1.4/obrpy/obrsdk/boost_system-mt.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/boost_thread-mt.dll` & `obrpy-0.1.4/obrpy/obrsdk/boost_thread-mt.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/libiomp5md.dll` & `obrpy-0.1.4/obrpy/obrsdk/libiomp5md.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/obr.exe` & `obrpy-0.1.4/obrpy/obrsdk/obr.exe`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/ova32.dll` & `obrpy-0.1.4/obrpy/obrsdk/ova32.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/ova32.lib` & `obrpy-0.1.4/obrpy/obrsdk/ova32.lib`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk/ovaGUI.dll` & `obrpy-0.1.4/obrpy/obrsdk/ovaGUI.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/obrsdk.py` & `obrpy-0.1.4/obrpy/obrsdk.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/save.py` & `obrpy-0.1.4/obrpy/save.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/settings.py` & `obrpy-0.1.4/obrpy/settings.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/take_a_look.py` & `obrpy-0.1.4/obrpy/take_a_look.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/to_export.py` & `obrpy-0.1.4/obrpy/to_export.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy/to_import.py` & `obrpy-0.1.4/obrpy/to_import.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/obrpy.egg-info/SOURCES.txt` & `obrpy-0.1.4/obrpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/setup.py` & `obrpy-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.3' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.1.4' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'obrpy' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Andres Pedraza Rodriguez' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'a.pedraza@upm.es' #Modificar con vuestros datos
 URL = 'https://github.com/temisAP' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = "This library is aimed for using Luna's OBR-4600 with Python." #Descripción corta
```

### Comparing `obrpy-0.1.3/test/test.py` & `obrpy-0.1.4/test/test.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/test/test_dataset.py` & `obrpy-0.1.4/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/test/test_export_obrfiles.py` & `obrpy-0.1.4/test/test_export_obrfiles.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/test/test_export_settings.py` & `obrpy-0.1.4/test/test_export_settings.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/test/test_export_slices.py` & `obrpy-0.1.4/test/test_export_slices.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/test/test_import.py` & `obrpy-0.1.4/test/test_import.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/test/test_linked_attr.py` & `obrpy-0.1.4/test/test_linked_attr.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/test/test_obr_ini.py` & `obrpy-0.1.4/test/test_obr_ini.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.3/test/test_slices.py` & `obrpy-0.1.4/test/test_slices.py`

 * *Files identical despite different names*

