# Comparing `tmp/rec_to_binaries-0.7.4.tar.gz` & `tmp/rec_to_binaries-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rec_to_binaries-0.7.4.tar", last modified: Sun Aug 21 16:31:37 2022, max compression
+gzip compressed data, was "rec_to_binaries-0.7.5.tar", last modified: Tue Jul 11 17:51:21 2023, max compression
```

## Comparing `rec_to_binaries-0.7.4.tar` & `rec_to_binaries-0.7.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2022-08-21 16:31:37.314275 rec_to_binaries-0.7.4/
--rw-r--r--   0 edeno      (501) staff       (20)     1072 2019-10-02 17:31:08.000000 rec_to_binaries-0.7.4/LICENSE
--rw-r--r--   0 edeno      (501) staff       (20)      303 2022-08-21 16:31:37.313800 rec_to_binaries-0.7.4/PKG-INFO
--rw-r--r--   0 edeno      (501) staff       (20)    13373 2020-02-01 15:11:41.000000 rec_to_binaries-0.7.4/README.md
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2022-08-21 16:31:37.309480 rec_to_binaries-0.7.4/rec_to_binaries/
--rw-r--r--   0 edeno      (501) staff       (20)       65 2020-11-09 18:48:12.000000 rec_to_binaries-0.7.4/rec_to_binaries/__init__.py
--rw-r--r--   0 edeno      (501) staff       (20)     3950 2021-11-19 19:18:27.000000 rec_to_binaries-0.7.4/rec_to_binaries/adjust_timestamps.py
--rw-r--r--   0 edeno      (501) staff       (20)     8689 2021-11-19 19:18:47.000000 rec_to_binaries-0.7.4/rec_to_binaries/binary_utils.py
--rw-r--r--   0 edeno      (501) staff       (20)    12075 2022-08-21 15:53:21.000000 rec_to_binaries-0.7.4/rec_to_binaries/core.py
--rw-r--r--   0 edeno      (501) staff       (20)     1583 2021-11-19 19:18:40.000000 rec_to_binaries-0.7.4/rec_to_binaries/create_system_time.py
--rw-r--r--   0 edeno      (501) staff       (20)     2945 2021-11-19 19:18:42.000000 rec_to_binaries-0.7.4/rec_to_binaries/read_binaries.py
--rw-r--r--   0 edeno      (501) staff       (20)    69669 2022-08-21 16:27:11.000000 rec_to_binaries-0.7.4/rec_to_binaries/trodes_data.py
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2022-08-21 16:31:37.312973 rec_to_binaries-0.7.4/rec_to_binaries.egg-info/
--rw-r--r--   0 edeno      (501) staff       (20)      303 2022-08-21 16:31:37.000000 rec_to_binaries-0.7.4/rec_to_binaries.egg-info/PKG-INFO
--rw-r--r--   0 edeno      (501) staff       (20)      443 2022-08-21 16:31:37.000000 rec_to_binaries-0.7.4/rec_to_binaries.egg-info/SOURCES.txt
--rw-r--r--   0 edeno      (501) staff       (20)        1 2022-08-21 16:31:37.000000 rec_to_binaries-0.7.4/rec_to_binaries.egg-info/dependency_links.txt
--rw-r--r--   0 edeno      (501) staff       (20)       19 2022-08-21 16:31:37.000000 rec_to_binaries-0.7.4/rec_to_binaries.egg-info/requires.txt
--rw-r--r--   0 edeno      (501) staff       (20)       16 2022-08-21 16:31:37.000000 rec_to_binaries-0.7.4/rec_to_binaries.egg-info/top_level.txt
--rw-r--r--   0 edeno      (501) staff       (20)       38 2022-08-21 16:31:37.314616 rec_to_binaries-0.7.4/setup.cfg
--rw-r--r--   0 edeno      (501) staff       (20)      572 2022-08-21 16:29:14.000000 rec_to_binaries-0.7.4/setup.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-11 17:51:21.617487 rec_to_binaries-0.7.5/
+-rw-r--r--   0 edeno      (501) staff       (20)     1072 2019-10-02 17:31:08.000000 rec_to_binaries-0.7.5/LICENSE
+-rw-r--r--   0 edeno      (501) staff       (20)      303 2023-07-11 17:51:21.617324 rec_to_binaries-0.7.5/PKG-INFO
+-rw-r--r--   0 edeno      (501) staff       (20)    13373 2020-02-01 15:11:41.000000 rec_to_binaries-0.7.5/README.md
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-11 17:51:21.616307 rec_to_binaries-0.7.5/rec_to_binaries/
+-rw-r--r--   0 edeno      (501) staff       (20)       65 2020-11-09 18:48:12.000000 rec_to_binaries-0.7.5/rec_to_binaries/__init__.py
+-rw-r--r--   0 edeno      (501) staff       (20)     3950 2021-11-19 19:18:27.000000 rec_to_binaries-0.7.5/rec_to_binaries/adjust_timestamps.py
+-rw-r--r--   0 edeno      (501) staff       (20)     8689 2021-11-19 19:18:47.000000 rec_to_binaries-0.7.5/rec_to_binaries/binary_utils.py
+-rw-r--r--   0 edeno      (501) staff       (20)    12075 2022-08-21 15:53:21.000000 rec_to_binaries-0.7.5/rec_to_binaries/core.py
+-rw-r--r--   0 edeno      (501) staff       (20)     1583 2021-11-19 19:18:40.000000 rec_to_binaries-0.7.5/rec_to_binaries/create_system_time.py
+-rw-r--r--   0 edeno      (501) staff       (20)     2945 2021-11-19 19:18:42.000000 rec_to_binaries-0.7.5/rec_to_binaries/read_binaries.py
+-rw-r--r--   0 edeno      (501) staff       (20)    69665 2023-07-11 15:18:15.000000 rec_to_binaries-0.7.5/rec_to_binaries/trodes_data.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-11 17:51:21.617106 rec_to_binaries-0.7.5/rec_to_binaries.egg-info/
+-rw-r--r--   0 edeno      (501) staff       (20)      303 2023-07-11 17:51:21.000000 rec_to_binaries-0.7.5/rec_to_binaries.egg-info/PKG-INFO
+-rw-r--r--   0 edeno      (501) staff       (20)      443 2023-07-11 17:51:21.000000 rec_to_binaries-0.7.5/rec_to_binaries.egg-info/SOURCES.txt
+-rw-r--r--   0 edeno      (501) staff       (20)        1 2023-07-11 17:51:21.000000 rec_to_binaries-0.7.5/rec_to_binaries.egg-info/dependency_links.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       19 2023-07-11 17:51:21.000000 rec_to_binaries-0.7.5/rec_to_binaries.egg-info/requires.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       16 2023-07-11 17:51:21.000000 rec_to_binaries-0.7.5/rec_to_binaries.egg-info/top_level.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       38 2023-07-11 17:51:21.617533 rec_to_binaries-0.7.5/setup.cfg
+-rw-r--r--   0 edeno      (501) staff       (20)      572 2023-07-11 17:37:43.000000 rec_to_binaries-0.7.5/setup.py
```

### Comparing `rec_to_binaries-0.7.4/LICENSE` & `rec_to_binaries-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rec_to_binaries-0.7.4/README.md` & `rec_to_binaries-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `rec_to_binaries-0.7.4/rec_to_binaries/adjust_timestamps.py` & `rec_to_binaries-0.7.5/rec_to_binaries/adjust_timestamps.py`

 * *Files identical despite different names*

### Comparing `rec_to_binaries-0.7.4/rec_to_binaries/binary_utils.py` & `rec_to_binaries-0.7.5/rec_to_binaries/binary_utils.py`

 * *Files identical despite different names*

### Comparing `rec_to_binaries-0.7.4/rec_to_binaries/core.py` & `rec_to_binaries-0.7.5/rec_to_binaries/core.py`

 * *Files identical despite different names*

### Comparing `rec_to_binaries-0.7.4/rec_to_binaries/create_system_time.py` & `rec_to_binaries-0.7.5/rec_to_binaries/create_system_time.py`

 * *Files identical despite different names*

### Comparing `rec_to_binaries-0.7.4/rec_to_binaries/read_binaries.py` & `rec_to_binaries-0.7.5/rec_to_binaries/read_binaries.py`

 * *Files identical despite different names*

### Comparing `rec_to_binaries-0.7.4/rec_to_binaries/trodes_data.py` & `rec_to_binaries-0.7.5/rec_to_binaries/trodes_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
             with the directory column dropped
 
         """
         partial_extracted_columns = parser_datatype_fields + \
             ['dir_index', 'path']
         partial_extracted_paths = pd.DataFrame(
             columns=partial_extracted_columns)
-        for dir_index, directory in directory_entries_df['directory'].iteritems():
+        for dir_index, directory in directory_entries_df['directory'].items():
             file_list = TrodesAnimalInfo._get_extracted_file_list(
                 directory, ExtractedFileParser=ExtractedFileParser)
             directory_path_fields = []
             for filename_parser, file_path in file_list:
                 file_path_fields = []
                 for field in parser_datatype_fields:
                     file_path_fields.append(
```

### Comparing `rec_to_binaries-0.7.4/setup.py` & `rec_to_binaries-0.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 INSTALL_REQUIRES = ['numpy', 'pandas', 'scipy']
 TESTS_REQUIRE = ['pytest >= 2.7.1']
 
 setup(
     name='rec_to_binaries',
-    version='0.7.4',
+    version='0.7.5',
     license='MIT',
     description=('Covert SpikeGadgets rec files to binaries'),
     author='Eric Denovellis, Daniel Liu',
     author_email='Eric.Denovellis@ucsf.edu',
     url='https://github.com/LorenFrankLab/rec_to_binaries',
     packages=find_packages(),
     install_requires=INSTALL_REQUIRES,
```

