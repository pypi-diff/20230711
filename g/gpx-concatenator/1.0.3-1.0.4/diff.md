# Comparing `tmp/gpx-concatenator-1.0.3.tar.gz` & `tmp/gpx-concatenator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx-concatenator-1.0.3.tar", last modified: Tue Jul 11 21:08:58 2023, max compression
+gzip compressed data, was "gpx-concatenator-1.0.4.tar", last modified: Tue Jul 11 21:27:26 2023, max compression
```

## Comparing `gpx-concatenator-1.0.3.tar` & `gpx-concatenator-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:08:58.889330 gpx-concatenator-1.0.3/
--rw-r--r--   0 teolebras   (501) staff       (20)     1070 2023-07-09 14:10:22.000000 gpx-concatenator-1.0.3/LICENSE
--rw-r--r--   0 teolebras   (501) staff       (20)     3822 2023-07-11 21:08:58.887494 gpx-concatenator-1.0.3/PKG-INFO
--rw-r--r--   0 teolebras   (501) staff       (20)     3602 2023-07-11 21:07:45.000000 gpx-concatenator-1.0.3/README.md
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:08:58.854107 gpx-concatenator-1.0.3/gpx_concatenator/
--rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:20.000000 gpx-concatenator-1.0.3/gpx_concatenator/__init__.py
--rw-r--r--   0 teolebras   (501) staff       (20)     3801 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.3/gpx_concatenator/gpx_colorizer.py
--rw-r--r--   0 teolebras   (501) staff       (20)     2646 2023-07-09 14:03:22.000000 gpx-concatenator-1.0.3/gpx_concatenator/gpx_concatenator.py
--rw-r--r--   0 teolebras   (501) staff       (20)     1071 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.3/gpx_concatenator/gpx_file.py
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:08:58.878183 gpx-concatenator-1.0.3/gpx_concatenator/tests/
--rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 15:24:44.000000 gpx-concatenator-1.0.3/gpx_concatenator/tests/__init__.py
--rw-r--r--   0 teolebras   (501) staff       (20)     2204 2023-07-09 15:22:39.000000 gpx-concatenator-1.0.3/gpx_concatenator/tests/gpx_colorizer_test.py
--rw-r--r--   0 teolebras   (501) staff       (20)      870 2023-07-09 15:37:16.000000 gpx-concatenator-1.0.3/gpx_concatenator/tests/gpx_file_test.py
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:08:58.874477 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/
--rw-r--r--   0 teolebras   (501) staff       (20)     3822 2023-07-11 21:08:58.000000 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/PKG-INFO
--rw-r--r--   0 teolebras   (501) staff       (20)      514 2023-07-11 21:08:58.000000 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/SOURCES.txt
--rw-r--r--   0 teolebras   (501) staff       (20)        1 2023-07-11 21:08:58.000000 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/dependency_links.txt
--rw-r--r--   0 teolebras   (501) staff       (20)       55 2023-07-11 21:08:58.000000 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/entry_points.txt
--rw-r--r--   0 teolebras   (501) staff       (20)       25 2023-07-11 21:08:58.000000 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/top_level.txt
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:08:58.883477 gpx-concatenator-1.0.3/scripts/
--rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:26.000000 gpx-concatenator-1.0.3/scripts/__init__.py
--rw-r--r--   0 teolebras   (501) staff       (20)     1243 2023-07-11 21:06:01.000000 gpx-concatenator-1.0.3/scripts/main.py
--rw-r--r--   0 teolebras   (501) staff       (20)       38 2023-07-11 21:08:58.891451 gpx-concatenator-1.0.3/setup.cfg
--rw-r--r--   0 teolebras   (501) staff       (20)      585 2023-07-11 21:07:57.000000 gpx-concatenator-1.0.3/setup.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:27:26.558239 gpx-concatenator-1.0.4/
+-rw-r--r--   0 teolebras   (501) staff       (20)     1070 2023-07-09 14:10:22.000000 gpx-concatenator-1.0.4/LICENSE
+-rw-r--r--   0 teolebras   (501) staff       (20)     3822 2023-07-11 21:27:26.557509 gpx-concatenator-1.0.4/PKG-INFO
+-rw-r--r--   0 teolebras   (501) staff       (20)     3602 2023-07-11 21:07:45.000000 gpx-concatenator-1.0.4/README.md
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:27:26.532336 gpx-concatenator-1.0.4/gpx_concatenator/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:20.000000 gpx-concatenator-1.0.4/gpx_concatenator/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     3801 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.4/gpx_concatenator/gpx_colorizer.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     2646 2023-07-09 14:03:22.000000 gpx-concatenator-1.0.4/gpx_concatenator/gpx_concatenator.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     1071 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.4/gpx_concatenator/gpx_file.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:27:26.554063 gpx-concatenator-1.0.4/gpx_concatenator/tests/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 15:24:44.000000 gpx-concatenator-1.0.4/gpx_concatenator/tests/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     2204 2023-07-09 15:22:39.000000 gpx-concatenator-1.0.4/gpx_concatenator/tests/gpx_colorizer_test.py
+-rw-r--r--   0 teolebras   (501) staff       (20)      870 2023-07-09 15:37:16.000000 gpx-concatenator-1.0.4/gpx_concatenator/tests/gpx_file_test.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:27:26.548111 gpx-concatenator-1.0.4/gpx_concatenator.egg-info/
+-rw-r--r--   0 teolebras   (501) staff       (20)     3822 2023-07-11 21:27:26.000000 gpx-concatenator-1.0.4/gpx_concatenator.egg-info/PKG-INFO
+-rw-r--r--   0 teolebras   (501) staff       (20)      514 2023-07-11 21:27:26.000000 gpx-concatenator-1.0.4/gpx_concatenator.egg-info/SOURCES.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)        1 2023-07-11 21:27:26.000000 gpx-concatenator-1.0.4/gpx_concatenator.egg-info/dependency_links.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)       55 2023-07-11 21:27:26.000000 gpx-concatenator-1.0.4/gpx_concatenator.egg-info/entry_points.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)       25 2023-07-11 21:27:26.000000 gpx-concatenator-1.0.4/gpx_concatenator.egg-info/top_level.txt
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:27:26.556198 gpx-concatenator-1.0.4/scripts/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:26.000000 gpx-concatenator-1.0.4/scripts/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     1424 2023-07-11 21:27:04.000000 gpx-concatenator-1.0.4/scripts/main.py
+-rw-r--r--   0 teolebras   (501) staff       (20)       38 2023-07-11 21:27:26.558845 gpx-concatenator-1.0.4/setup.cfg
+-rw-r--r--   0 teolebras   (501) staff       (20)      585 2023-07-11 21:27:09.000000 gpx-concatenator-1.0.4/setup.py
```

### Comparing `gpx-concatenator-1.0.3/LICENSE` & `gpx-concatenator-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.3/PKG-INFO` & `gpx-concatenator-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx-concatenator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tool for concatenating GPX files
 Author: iambrianna
 Author-email: iambrianna@proton.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPX Concatenator
```

### Comparing `gpx-concatenator-1.0.3/README.md` & `gpx-concatenator-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.3/gpx_concatenator/gpx_colorizer.py` & `gpx-concatenator-1.0.4/gpx_concatenator/gpx_colorizer.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.3/gpx_concatenator/gpx_concatenator.py` & `gpx-concatenator-1.0.4/gpx_concatenator/gpx_concatenator.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.3/gpx_concatenator/gpx_file.py` & `gpx-concatenator-1.0.4/gpx_concatenator/gpx_file.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.3/gpx_concatenator/tests/gpx_colorizer_test.py` & `gpx-concatenator-1.0.4/gpx_concatenator/tests/gpx_colorizer_test.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.3/gpx_concatenator/tests/gpx_file_test.py` & `gpx-concatenator-1.0.4/gpx_concatenator/tests/gpx_file_test.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.3/gpx_concatenator.egg-info/PKG-INFO` & `gpx-concatenator-1.0.4/gpx_concatenator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx-concatenator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tool for concatenating GPX files
 Author: iambrianna
 Author-email: iambrianna@proton.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPX Concatenator
```

### Comparing `gpx-concatenator-1.0.3/gpx_concatenator.egg-info/SOURCES.txt` & `gpx-concatenator-1.0.4/gpx_concatenator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.3/scripts/main.py` & `gpx-concatenator-1.0.4/scripts/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import os
 import argparse
 from gpx_concatenator.gpx_concatenator import GPXConcatenator
+import argcomplete
 
 def main():
     # Create an argument parser
     parser = argparse.ArgumentParser(description='GPX Concatenator')
-    parser.add_argument('-i', '--input-dir', default='input', help='Directory containing input files')
-    parser.add_argument('-o', '--output-file', default='output.gpx', help='Output file name')
+    parser.add_argument('-i', '--input-dir', default='input', help='Directory containing input files', type=argcomplete.completers.DirectoryCompleter())
+    parser.add_argument('-o', '--output-file', default='output.gpx', help='Output file name', type=argparse.FileType('w'))
     parser.add_argument('-m', '--enable-metadata', action='store_true', help='Enable metadata in the output file')
     parser.add_argument('-c', '--enable-coloring', action='store_true', help='Enable coloring in the output file')
 
+    # Activate autocompletion for paths
+    argcomplete.autocomplete(parser)
+
     # Parse the command-line arguments
     args = parser.parse_args()
 
     # Get the input files from the specified directory
     input_files = sorted([os.path.join(args.input_dir, file) for file in os.listdir(args.input_dir) if file.endswith('.gpx')])
 
     # Create an instance of GPXConcatenator with the specified parameters
     concatenator = GPXConcatenator(
         input_files,
-        args.output_file,
+        args.output_file.name,
         enable_metadata=args.enable_metadata,
         enable_coloring=args.enable_coloring
     )
 
     # Concatenate the files
     concatenator.concatenate_files()
```

### Comparing `gpx-concatenator-1.0.3/setup.py` & `gpx-concatenator-1.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='gpx-concatenator',
-    version='1.0.3',
+    version='1.0.4',
     description='Tool for concatenating GPX files',
     author='iambrianna',
     author_email='iambrianna@proton.me',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'gpx-concatenator = scripts.main:main',
```

