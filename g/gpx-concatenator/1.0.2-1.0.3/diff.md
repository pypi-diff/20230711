# Comparing `tmp/gpx-concatenator-1.0.2.tar.gz` & `tmp/gpx-concatenator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx-concatenator-1.0.2.tar", last modified: Sun Jul  9 14:57:34 2023, max compression
+gzip compressed data, was "gpx-concatenator-1.0.3.tar", last modified: Tue Jul 11 21:08:58 2023, max compression
```

## Comparing `gpx-concatenator-1.0.2.tar` & `gpx-concatenator-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:57:34.661633 gpx-concatenator-1.0.2/
--rw-r--r--   0 teolebras   (501) staff       (20)     1070 2023-07-09 14:10:22.000000 gpx-concatenator-1.0.2/LICENSE
--rw-r--r--   0 teolebras   (501) staff       (20)     3997 2023-07-09 14:57:34.657697 gpx-concatenator-1.0.2/PKG-INFO
--rw-r--r--   0 teolebras   (501) staff       (20)     3777 2023-07-09 14:15:47.000000 gpx-concatenator-1.0.2/README.md
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:57:34.638372 gpx-concatenator-1.0.2/gpx_concatenator/
--rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:20.000000 gpx-concatenator-1.0.2/gpx_concatenator/__init__.py
--rw-r--r--   0 teolebras   (501) staff       (20)     3801 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.2/gpx_concatenator/gpx_colorizer.py
--rw-r--r--   0 teolebras   (501) staff       (20)     2646 2023-07-09 14:03:22.000000 gpx-concatenator-1.0.2/gpx_concatenator/gpx_concatenator.py
--rw-r--r--   0 teolebras   (501) staff       (20)     1071 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.2/gpx_concatenator/gpx_file.py
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:57:34.653791 gpx-concatenator-1.0.2/gpx_concatenator.egg-info/
--rw-r--r--   0 teolebras   (501) staff       (20)     3997 2023-07-09 14:57:34.000000 gpx-concatenator-1.0.2/gpx_concatenator.egg-info/PKG-INFO
--rw-r--r--   0 teolebras   (501) staff       (20)      394 2023-07-09 14:57:34.000000 gpx-concatenator-1.0.2/gpx_concatenator.egg-info/SOURCES.txt
--rw-r--r--   0 teolebras   (501) staff       (20)        1 2023-07-09 14:57:34.000000 gpx-concatenator-1.0.2/gpx_concatenator.egg-info/dependency_links.txt
--rw-r--r--   0 teolebras   (501) staff       (20)       55 2023-07-09 14:57:34.000000 gpx-concatenator-1.0.2/gpx_concatenator.egg-info/entry_points.txt
--rw-r--r--   0 teolebras   (501) staff       (20)       25 2023-07-09 14:57:34.000000 gpx-concatenator-1.0.2/gpx_concatenator.egg-info/top_level.txt
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:57:34.656611 gpx-concatenator-1.0.2/scripts/
--rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:26.000000 gpx-concatenator-1.0.2/scripts/__init__.py
--rw-r--r--   0 teolebras   (501) staff       (20)     1219 2023-07-09 14:56:43.000000 gpx-concatenator-1.0.2/scripts/main.py
--rw-r--r--   0 teolebras   (501) staff       (20)       38 2023-07-09 14:57:34.666121 gpx-concatenator-1.0.2/setup.cfg
--rw-r--r--   0 teolebras   (501) staff       (20)      585 2023-07-09 14:56:50.000000 gpx-concatenator-1.0.2/setup.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:08:58.889330 gpx-concatenator-1.0.3/
+-rw-r--r--   0 teolebras   (501) staff       (20)     1070 2023-07-09 14:10:22.000000 gpx-concatenator-1.0.3/LICENSE
+-rw-r--r--   0 teolebras   (501) staff       (20)     3822 2023-07-11 21:08:58.887494 gpx-concatenator-1.0.3/PKG-INFO
+-rw-r--r--   0 teolebras   (501) staff       (20)     3602 2023-07-11 21:07:45.000000 gpx-concatenator-1.0.3/README.md
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:08:58.854107 gpx-concatenator-1.0.3/gpx_concatenator/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:20.000000 gpx-concatenator-1.0.3/gpx_concatenator/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     3801 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.3/gpx_concatenator/gpx_colorizer.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     2646 2023-07-09 14:03:22.000000 gpx-concatenator-1.0.3/gpx_concatenator/gpx_concatenator.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     1071 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.3/gpx_concatenator/gpx_file.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:08:58.878183 gpx-concatenator-1.0.3/gpx_concatenator/tests/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 15:24:44.000000 gpx-concatenator-1.0.3/gpx_concatenator/tests/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     2204 2023-07-09 15:22:39.000000 gpx-concatenator-1.0.3/gpx_concatenator/tests/gpx_colorizer_test.py
+-rw-r--r--   0 teolebras   (501) staff       (20)      870 2023-07-09 15:37:16.000000 gpx-concatenator-1.0.3/gpx_concatenator/tests/gpx_file_test.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:08:58.874477 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/
+-rw-r--r--   0 teolebras   (501) staff       (20)     3822 2023-07-11 21:08:58.000000 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/PKG-INFO
+-rw-r--r--   0 teolebras   (501) staff       (20)      514 2023-07-11 21:08:58.000000 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/SOURCES.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)        1 2023-07-11 21:08:58.000000 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/dependency_links.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)       55 2023-07-11 21:08:58.000000 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/entry_points.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)       25 2023-07-11 21:08:58.000000 gpx-concatenator-1.0.3/gpx_concatenator.egg-info/top_level.txt
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 21:08:58.883477 gpx-concatenator-1.0.3/scripts/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:26.000000 gpx-concatenator-1.0.3/scripts/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     1243 2023-07-11 21:06:01.000000 gpx-concatenator-1.0.3/scripts/main.py
+-rw-r--r--   0 teolebras   (501) staff       (20)       38 2023-07-11 21:08:58.891451 gpx-concatenator-1.0.3/setup.cfg
+-rw-r--r--   0 teolebras   (501) staff       (20)      585 2023-07-11 21:07:57.000000 gpx-concatenator-1.0.3/setup.py
```

### Comparing `gpx-concatenator-1.0.2/LICENSE` & `gpx-concatenator-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.2/PKG-INFO` & `gpx-concatenator-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx-concatenator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tool for concatenating GPX files
 Author: iambrianna
 Author-email: iambrianna@proton.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPX Concatenator
@@ -32,32 +32,32 @@
 ```
 
 ## Usage
 
 Once installed, you can use the `gpx-concatenator` command to concatenate and colorize GPX files. Here's an example usage:
 
 ```
-gpx-concatenator --input-dir <input-directory> --output-file <output-file-name> --enable-metadata --enable-coloring
+gpx-concatenator -i <input-directory> -o <output-file-name> -m -c
 ```
 
-Replace `<input-directory>` with the directory containing the input GPX files, and `<output-file-name>` with the desired name of the output GPX file. The `--enable-metadata` flag enables metadata in the output file, and the `--enable-coloring` flag enables coloring of the tracks.
+Replace `<input-directory>` with the directory containing the input GPX files, and `<output-file-name>` with the desired name of the output GPX file. The `-m` flag enables metadata in the output file, and the `-c` flag enables coloring of the tracks.
 
 ### Command-line Arguments
 
 The following command-line arguments are available:
 
-- `--input-dir`: Specifies the directory containing the input GPX files. The default value is `input`.
+- `-i, --input-dir`: Specifies the directory containing the input GPX files. The default value is `input`.
 
-- `--output-file`: Specifies the name of the output GPX file. The default value is `output.gpx`.
+- `-o, --output-file`: Specifies the name of the output GPX file. The default value is `output.gpx`.
 
-- `--enable-metadata`: Enables metadata in the output GPX file. This is an optional flag.
+- `-m, --enable-metadata`: Enables metadata in the output GPX file. This is an optional flag.
 
-- `--enable-coloring`: Enables coloring of the tracks in the output GPX file. This is an optional flag.
+- `-c, --enable-coloring`: Enables coloring of the tracks in the output GPX file. This is an optional flag.
 
-For more information on available command-line arguments, use the `--help` flag:
+For more information on available command-line arguments, use the `-h, --help` flag:
 
 ```
 gpx-concatenator --help
 ```
 
 ### Input Files
 
@@ -67,16 +67,13 @@
 
 The concatenated GPX file will be created with the specified name in the current working directory. If the file already exists, it will be overwritten.
 
 ## License
 
 This project is licensed under the MIT License.
 
-
      _                 _          _                         
     (_)               | |        (_)                        
      _  __ _ _ __ ___ | |__  _ __ _  __ _ _ __  _ __   __ _ 
     | |/ _` | '_ ` _ \| '_ \| '__| |/ _` | '_ \| '_ \ / _` |
     | | (_| | | | | | | |_) | |  | | (_| | | | | | | | (_| |
     |_|\__,_|_| |_| |_|_.__/|_|  |_|\__,_|_| |_|_| |_|\__,_|
-                                                        
-
```

### Comparing `gpx-concatenator-1.0.2/README.md` & `gpx-concatenator-1.0.3/gpx_concatenator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: gpx-concatenator
+Version: 1.0.3
+Summary: Tool for concatenating GPX files
+Author: iambrianna
+Author-email: iambrianna@proton.me
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # GPX Concatenator
 
 GPX Concatenator is a Python project that provides a set of scripts for concatenating and colorizing GPX (GPS Exchange Format) files.
 
 ## Files
 
 The project consists of the following files:
@@ -23,32 +32,32 @@
 ```
 
 ## Usage
 
 Once installed, you can use the `gpx-concatenator` command to concatenate and colorize GPX files. Here's an example usage:
 
 ```
-gpx-concatenator --input-dir <input-directory> --output-file <output-file-name> --enable-metadata --enable-coloring
+gpx-concatenator -i <input-directory> -o <output-file-name> -m -c
 ```
 
-Replace `<input-directory>` with the directory containing the input GPX files, and `<output-file-name>` with the desired name of the output GPX file. The `--enable-metadata` flag enables metadata in the output file, and the `--enable-coloring` flag enables coloring of the tracks.
+Replace `<input-directory>` with the directory containing the input GPX files, and `<output-file-name>` with the desired name of the output GPX file. The `-m` flag enables metadata in the output file, and the `-c` flag enables coloring of the tracks.
 
 ### Command-line Arguments
 
 The following command-line arguments are available:
 
-- `--input-dir`: Specifies the directory containing the input GPX files. The default value is `input`.
+- `-i, --input-dir`: Specifies the directory containing the input GPX files. The default value is `input`.
 
-- `--output-file`: Specifies the name of the output GPX file. The default value is `output.gpx`.
+- `-o, --output-file`: Specifies the name of the output GPX file. The default value is `output.gpx`.
 
-- `--enable-metadata`: Enables metadata in the output GPX file. This is an optional flag.
+- `-m, --enable-metadata`: Enables metadata in the output GPX file. This is an optional flag.
 
-- `--enable-coloring`: Enables coloring of the tracks in the output GPX file. This is an optional flag.
+- `-c, --enable-coloring`: Enables coloring of the tracks in the output GPX file. This is an optional flag.
 
-For more information on available command-line arguments, use the `--help` flag:
+For more information on available command-line arguments, use the `-h, --help` flag:
 
 ```
 gpx-concatenator --help
 ```
 
 ### Input Files
 
@@ -58,16 +67,13 @@
 
 The concatenated GPX file will be created with the specified name in the current working directory. If the file already exists, it will be overwritten.
 
 ## License
 
 This project is licensed under the MIT License.
 
-
      _                 _          _                         
     (_)               | |        (_)                        
      _  __ _ _ __ ___ | |__  _ __ _  __ _ _ __  _ __   __ _ 
     | |/ _` | '_ ` _ \| '_ \| '__| |/ _` | '_ \| '_ \ / _` |
     | | (_| | | | | | | |_) | |  | | (_| | | | | | | | (_| |
     |_|\__,_|_| |_| |_|_.__/|_|  |_|\__,_|_| |_|_| |_|\__,_|
-                                                        
-
```

### Comparing `gpx-concatenator-1.0.2/gpx_concatenator/gpx_colorizer.py` & `gpx-concatenator-1.0.3/gpx_concatenator/gpx_colorizer.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.2/gpx_concatenator/gpx_concatenator.py` & `gpx-concatenator-1.0.3/gpx_concatenator/gpx_concatenator.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.2/gpx_concatenator/gpx_file.py` & `gpx-concatenator-1.0.3/gpx_concatenator/gpx_file.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.2/gpx_concatenator.egg-info/PKG-INFO` & `gpx-concatenator-1.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: gpx-concatenator
-Version: 1.0.2
-Summary: Tool for concatenating GPX files
-Author: iambrianna
-Author-email: iambrianna@proton.me
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # GPX Concatenator
 
 GPX Concatenator is a Python project that provides a set of scripts for concatenating and colorizing GPX (GPS Exchange Format) files.
 
 ## Files
 
 The project consists of the following files:
@@ -32,32 +23,32 @@
 ```
 
 ## Usage
 
 Once installed, you can use the `gpx-concatenator` command to concatenate and colorize GPX files. Here's an example usage:
 
 ```
-gpx-concatenator --input-dir <input-directory> --output-file <output-file-name> --enable-metadata --enable-coloring
+gpx-concatenator -i <input-directory> -o <output-file-name> -m -c
 ```
 
-Replace `<input-directory>` with the directory containing the input GPX files, and `<output-file-name>` with the desired name of the output GPX file. The `--enable-metadata` flag enables metadata in the output file, and the `--enable-coloring` flag enables coloring of the tracks.
+Replace `<input-directory>` with the directory containing the input GPX files, and `<output-file-name>` with the desired name of the output GPX file. The `-m` flag enables metadata in the output file, and the `-c` flag enables coloring of the tracks.
 
 ### Command-line Arguments
 
 The following command-line arguments are available:
 
-- `--input-dir`: Specifies the directory containing the input GPX files. The default value is `input`.
+- `-i, --input-dir`: Specifies the directory containing the input GPX files. The default value is `input`.
 
-- `--output-file`: Specifies the name of the output GPX file. The default value is `output.gpx`.
+- `-o, --output-file`: Specifies the name of the output GPX file. The default value is `output.gpx`.
 
-- `--enable-metadata`: Enables metadata in the output GPX file. This is an optional flag.
+- `-m, --enable-metadata`: Enables metadata in the output GPX file. This is an optional flag.
 
-- `--enable-coloring`: Enables coloring of the tracks in the output GPX file. This is an optional flag.
+- `-c, --enable-coloring`: Enables coloring of the tracks in the output GPX file. This is an optional flag.
 
-For more information on available command-line arguments, use the `--help` flag:
+For more information on available command-line arguments, use the `-h, --help` flag:
 
 ```
 gpx-concatenator --help
 ```
 
 ### Input Files
 
@@ -67,16 +58,13 @@
 
 The concatenated GPX file will be created with the specified name in the current working directory. If the file already exists, it will be overwritten.
 
 ## License
 
 This project is licensed under the MIT License.
 
-
      _                 _          _                         
     (_)               | |        (_)                        
      _  __ _ _ __ ___ | |__  _ __ _  __ _ _ __  _ __   __ _ 
     | |/ _` | '_ ` _ \| '_ \| '__| |/ _` | '_ \| '_ \ / _` |
     | | (_| | | | | | | |_) | |  | | (_| | | | | | | | (_| |
-    |_|\__,_|_| |_| |_|_.__/|_|  |_|\__,_|_| |_|_| |_|\__,_|
-                                                        
-                                                        
+    |_|\__,_|_| |_| |_|_.__/|_|  |_|\__,_|_| |_|_| |_|\__,_|
```

### Comparing `gpx-concatenator-1.0.2/scripts/main.py` & `gpx-concatenator-1.0.3/scripts/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import argparse
 from gpx_concatenator.gpx_concatenator import GPXConcatenator
 
 def main():
     # Create an argument parser
     parser = argparse.ArgumentParser(description='GPX Concatenator')
-    parser.add_argument('--input-dir', default='input', help='Directory containing input files')
-    parser.add_argument('--output-file', default='output.gpx', help='Output file name')
-    parser.add_argument('--enable-metadata', action='store_true', help='Enable metadata in the output file')
-    parser.add_argument('--enable-coloring', action='store_true', help='Enable coloring in the output file')
+    parser.add_argument('-i', '--input-dir', default='input', help='Directory containing input files')
+    parser.add_argument('-o', '--output-file', default='output.gpx', help='Output file name')
+    parser.add_argument('-m', '--enable-metadata', action='store_true', help='Enable metadata in the output file')
+    parser.add_argument('-c', '--enable-coloring', action='store_true', help='Enable coloring in the output file')
 
     # Parse the command-line arguments
     args = parser.parse_args()
 
     # Get the input files from the specified directory
     input_files = sorted([os.path.join(args.input_dir, file) for file in os.listdir(args.input_dir) if file.endswith('.gpx')])
```

### Comparing `gpx-concatenator-1.0.2/setup.py` & `gpx-concatenator-1.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='gpx-concatenator',
-    version='1.0.2',
+    version='1.0.3',
     description='Tool for concatenating GPX files',
     author='iambrianna',
     author_email='iambrianna@proton.me',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'gpx-concatenator = scripts.main:main',
```

