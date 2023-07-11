# Comparing `tmp/json-lineage-0.2.1.tar.gz` & `tmp/json-lineage-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-lineage-0.2.1.tar", last modified: Sat Jul  1 00:13:12 2023, max compression
+gzip compressed data, was "json-lineage-0.2.2.tar", last modified: Tue Jul 11 00:55:44 2023, max compression
```

## Comparing `json-lineage-0.2.1.tar` & `json-lineage-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 salaah    (1000) salaah    (1000)        0 2023-07-01 00:13:12.618601 json-lineage-0.2.1/
--rw-r--r--   0 salaah    (1000) salaah    (1000)       36 2023-06-25 16:23:27.000000 json-lineage-0.2.1/MANIFEST.in
--rw-r--r--   0 salaah    (1000) salaah    (1000)     5931 2023-07-01 00:13:12.618601 json-lineage-0.2.1/PKG-INFO
--rw-r--r--   0 salaah    (1000) salaah    (1000)     4966 2023-07-01 00:04:13.000000 json-lineage-0.2.1/README.md
-drwxr-xr-x   0 salaah    (1000) salaah    (1000)        0 2023-07-01 00:13:12.608601 json-lineage-0.2.1/json_lineage/
--rw-r--r--   0 salaah    (1000) salaah    (1000)      186 2023-06-24 17:15:20.000000 json-lineage-0.2.1/json_lineage/__init__.py
--rw-r--r--   0 salaah    (1000) salaah    (1000)       61 2023-06-24 13:46:28.000000 json-lineage-0.2.1/json_lineage/__main__.py
-drwxr-xr-x   0 salaah    (1000) salaah    (1000)        0 2023-07-01 00:13:12.618601 json-lineage-0.2.1/json_lineage/bin/
--rwxr-xr-x   0 salaah    (1000) salaah    (1000)  6157264 2023-07-01 00:13:12.000000 json-lineage-0.2.1/json_lineage/bin/jsonl_converter
--rwxr-xr-x   0 salaah    (1000) salaah    (1000)  8016285 2023-07-01 00:13:12.000000 json-lineage-0.2.1/json_lineage/bin/jsonl_converter.exe
--rw-r--r--   0 salaah    (1000) salaah    (1000)      903 2023-06-25 02:04:26.000000 json-lineage-0.2.1/json_lineage/bin/tmp.py
--rw-r--r--   0 salaah    (1000) salaah    (1000)     5390 2023-06-29 01:14:14.000000 json-lineage-0.2.1/json_lineage/bin_interface.py
--rw-r--r--   0 salaah    (1000) salaah    (1000)     1723 2023-06-28 01:15:22.000000 json-lineage-0.2.1/json_lineage/cli.py
--rw-r--r--   0 salaah    (1000) salaah    (1000)      145 2023-06-25 13:37:01.000000 json-lineage-0.2.1/json_lineage/exceptions.py
--rw-r--r--   0 salaah    (1000) salaah    (1000)      621 2023-06-28 01:15:22.000000 json-lineage-0.2.1/json_lineage/public.py
-drwxr-xr-x   0 salaah    (1000) salaah    (1000)        0 2023-07-01 00:13:12.608601 json-lineage-0.2.1/json_lineage.egg-info/
--rw-r--r--   0 salaah    (1000) salaah    (1000)     5931 2023-07-01 00:13:12.000000 json-lineage-0.2.1/json_lineage.egg-info/PKG-INFO
--rw-r--r--   0 salaah    (1000) salaah    (1000)      605 2023-07-01 00:13:12.000000 json-lineage-0.2.1/json_lineage.egg-info/SOURCES.txt
--rw-r--r--   0 salaah    (1000) salaah    (1000)        1 2023-07-01 00:13:12.000000 json-lineage-0.2.1/json_lineage.egg-info/dependency_links.txt
--rw-r--r--   0 salaah    (1000) salaah    (1000)        1 2023-06-25 15:05:21.000000 json-lineage-0.2.1/json_lineage.egg-info/not-zip-safe
--rw-r--r--   0 salaah    (1000) salaah    (1000)       13 2023-07-01 00:13:12.000000 json-lineage-0.2.1/json_lineage.egg-info/top_level.txt
--rw-r--r--   0 salaah    (1000) salaah    (1000)      165 2023-06-24 00:00:43.000000 json-lineage-0.2.1/pyproject.toml
--rw-r--r--   0 salaah    (1000) salaah    (1000)     1052 2023-07-01 00:13:12.618601 json-lineage-0.2.1/setup.cfg
--rw-r--r--   0 salaah    (1000) salaah    (1000)       37 2023-06-25 16:23:27.000000 json-lineage-0.2.1/setup.py
-drwxr-xr-x   0 salaah    (1000) salaah    (1000)        0 2023-07-01 00:13:12.618601 json-lineage-0.2.1/tests/
--rw-r--r--   0 salaah    (1000) salaah    (1000)      213 2023-06-24 00:04:22.000000 json-lineage-0.2.1/tests/__init__.py
--rw-r--r--   0 salaah    (1000) salaah    (1000)      212 2023-06-24 00:04:22.000000 json-lineage-0.2.1/tests/helpers.py
--rw-r--r--   0 salaah    (1000) salaah    (1000)     9376 2023-06-28 01:15:22.000000 json-lineage-0.2.1/tests/test_bin_interface.py
--rw-r--r--   0 salaah    (1000) salaah    (1000)     2441 2023-06-24 16:22:51.000000 json-lineage-0.2.1/tests/test_cli.py
--rw-r--r--   0 salaah    (1000) salaah    (1000)      322 2023-06-24 00:04:22.000000 json-lineage-0.2.1/tests/test_exceptions.py
--rw-r--r--   0 salaah    (1000) salaah    (1000)      568 2023-06-24 17:15:20.000000 json-lineage-0.2.1/tests/test_public.py
+drwxr-xr-x   0 salaah    (1000) salaah    (1000)        0 2023-07-11 00:55:44.820816 json-lineage-0.2.2/
+-rw-r--r--   0 salaah    (1000) salaah    (1000)       36 2023-06-25 16:23:27.000000 json-lineage-0.2.2/MANIFEST.in
+-rw-r--r--   0 salaah    (1000) salaah    (1000)     6120 2023-07-11 00:55:44.820816 json-lineage-0.2.2/PKG-INFO
+-rw-r--r--   0 salaah    (1000) salaah    (1000)     5155 2023-07-10 01:49:06.000000 json-lineage-0.2.2/README.md
+drwxr-xr-x   0 salaah    (1000) salaah    (1000)        0 2023-07-11 00:55:44.810816 json-lineage-0.2.2/json_lineage/
+-rw-r--r--   0 salaah    (1000) salaah    (1000)      186 2023-06-24 17:15:20.000000 json-lineage-0.2.2/json_lineage/__init__.py
+-rw-r--r--   0 salaah    (1000) salaah    (1000)       61 2023-06-24 13:46:28.000000 json-lineage-0.2.2/json_lineage/__main__.py
+drwxr-xr-x   0 salaah    (1000) salaah    (1000)        0 2023-07-11 00:55:44.820816 json-lineage-0.2.2/json_lineage/bin/
+-rwxr-xr-x   0 salaah    (1000) salaah    (1000)  6157264 2023-07-09 01:58:18.000000 json-lineage-0.2.2/json_lineage/bin/jsonl_converter
+-rwxr-xr-x   0 salaah    (1000) salaah    (1000)  8016285 2023-07-09 01:58:18.000000 json-lineage-0.2.2/json_lineage/bin/jsonl_converter.exe
+-rw-r--r--   0 salaah    (1000) salaah    (1000)      903 2023-06-25 02:04:26.000000 json-lineage-0.2.2/json_lineage/bin/tmp.py
+-rw-r--r--   0 salaah    (1000) salaah    (1000)     5426 2023-07-11 00:54:58.000000 json-lineage-0.2.2/json_lineage/bin_interface.py
+-rw-r--r--   0 salaah    (1000) salaah    (1000)     1759 2023-07-11 00:54:58.000000 json-lineage-0.2.2/json_lineage/cli.py
+-rw-r--r--   0 salaah    (1000) salaah    (1000)      145 2023-06-25 13:37:01.000000 json-lineage-0.2.2/json_lineage/exceptions.py
+-rw-r--r--   0 salaah    (1000) salaah    (1000)      621 2023-06-28 01:15:22.000000 json-lineage-0.2.2/json_lineage/public.py
+drwxr-xr-x   0 salaah    (1000) salaah    (1000)        0 2023-07-11 00:55:44.810816 json-lineage-0.2.2/json_lineage.egg-info/
+-rw-r--r--   0 salaah    (1000) salaah    (1000)     6120 2023-07-11 00:55:44.000000 json-lineage-0.2.2/json_lineage.egg-info/PKG-INFO
+-rw-r--r--   0 salaah    (1000) salaah    (1000)      605 2023-07-11 00:55:44.000000 json-lineage-0.2.2/json_lineage.egg-info/SOURCES.txt
+-rw-r--r--   0 salaah    (1000) salaah    (1000)        1 2023-07-11 00:55:44.000000 json-lineage-0.2.2/json_lineage.egg-info/dependency_links.txt
+-rw-r--r--   0 salaah    (1000) salaah    (1000)        1 2023-06-25 15:05:21.000000 json-lineage-0.2.2/json_lineage.egg-info/not-zip-safe
+-rw-r--r--   0 salaah    (1000) salaah    (1000)       13 2023-07-11 00:55:44.000000 json-lineage-0.2.2/json_lineage.egg-info/top_level.txt
+-rw-r--r--   0 salaah    (1000) salaah    (1000)      165 2023-06-24 00:00:43.000000 json-lineage-0.2.2/pyproject.toml
+-rw-r--r--   0 salaah    (1000) salaah    (1000)     1052 2023-07-11 00:55:44.820816 json-lineage-0.2.2/setup.cfg
+-rw-r--r--   0 salaah    (1000) salaah    (1000)       37 2023-06-25 16:23:27.000000 json-lineage-0.2.2/setup.py
+drwxr-xr-x   0 salaah    (1000) salaah    (1000)        0 2023-07-11 00:55:44.820816 json-lineage-0.2.2/tests/
+-rw-r--r--   0 salaah    (1000) salaah    (1000)      213 2023-06-24 00:04:22.000000 json-lineage-0.2.2/tests/__init__.py
+-rw-r--r--   0 salaah    (1000) salaah    (1000)      212 2023-06-24 00:04:22.000000 json-lineage-0.2.2/tests/helpers.py
+-rw-r--r--   0 salaah    (1000) salaah    (1000)     9372 2023-07-11 00:54:58.000000 json-lineage-0.2.2/tests/test_bin_interface.py
+-rw-r--r--   0 salaah    (1000) salaah    (1000)     2441 2023-06-24 16:22:51.000000 json-lineage-0.2.2/tests/test_cli.py
+-rw-r--r--   0 salaah    (1000) salaah    (1000)      322 2023-06-24 00:04:22.000000 json-lineage-0.2.2/tests/test_exceptions.py
+-rw-r--r--   0 salaah    (1000) salaah    (1000)      568 2023-06-24 17:15:20.000000 json-lineage-0.2.2/tests/test_public.py
```

### Comparing `json-lineage-0.2.1/PKG-INFO` & `json-lineage-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-lineage
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library to parse JSON files iteratively without loading the whole file into memory
 Home-page: https://github.com/Salaah01/json-lineage
 Author: "Salaah Amin"
 License: "MIT"
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 - [JSON Lineage](#json-lineage)
   - [Table of Contents](#table-of-contents)
   - [Introduction](#introduction)
   - [Adapters](#adapters)
     - [Python](#python)
       - [Why not Just Use Python's `json` Library?](#why-not-just-use-pythons-json-library)
       - [Functionality](#functionality)
-      - [Benchmarks](#benchmarks)
+      - [Performance Comparison](#performance-comparison)
       - [Installation](#installation)
       - [Usage](#usage)
         - [Iterating over a JSON file](#iterating-over-a-json-file)
         - [Iterating over a JSON file asynchronously](#iterating-over-a-json-file-asynchronously)
         - [Poorly Formatted JSON](#poorly-formatted-json)
   - [Under the Hood](#under-the-hood)
 
@@ -48,46 +48,43 @@
 
 Additionally, this project contains adapters for easy integration into other programming languages. Currently, there is only a Python adapter, but more are planned.
 
 ## Adapters
 
 ### Python
 
-The Python adapter is a wrapper around the underlying Rust program. It allows for easy integration into Python programs.
-It is designed to feel a similar to the built-in `json` module in Python.
+The Python adapter is a wrapper around the underlying Rust program, providing seamless integration into Python applications. It is designed to have a similar feel to Python's built-in json module.
 
 #### Why not Just Use Python's `json` Library?
 
-Given that Python already has a built-in JSON parser, you may be wondering why you would want to use this library.
-The answer is, well, it depends.
+You might wonder why you would choose to use this library instead of Python's built-in JSON library. The answer depends on your specific use case.
 
-If you are parsing a small JSON file, then you probably don't want to use this library.
+If you are parsing a small JSON file, Python's JSON library is likely sufficient and performs well. However, when dealing with very large JSON files that exceed the available memory, JSON Lineage offers significant benefits.
 
-Python's JSON library is written in C and is very fast. However, as it loads the entire JSON file into memory, it is not suitable for parsing very large JSON files. This is where JSON Lineage comes in.
+Python's JSON library is written in C and is highly optimised for speed. However, it loads the entire JSON file into memory, making it unsuitable for parsing very large JSON files. This is where JSON Lineage shines.
 
-JSON Lineage is designed to parse very
-large JSON files that would otherwise not fit into memory. It does this by parsing the JSON file one object at a time.
+JSON Lineage is specifically designed to parse very large JSON files that would not fit into memory. It achieves this by parsing the JSON file one object at a time.
 
 #### Functionality
 
 The following functionality is provided:
 
 * `load` - Generate an iterator that returns each object in a JSON file.
 * `aload` - Generates an asynchronous iterator that returns each object in a JSON file.
 
 A CLI is also provided for easy conversion of JSON files to JSONL files.
 For information on how to use the CLI, run: `python -m json_lineage --help`.
 
-#### Benchmarks
+#### Performance Comparison
 
 The following graphs compare the speed and memory usage of Python's JSON library vs JSON Lineage.
 
 The benchmarks show that up to a file size of 500MB, the speed difference is negligible. However, already at this point, Python requires almost 2GB of memory to parse the JSON file, while JSON Lineage only requires 1.5GB.
 
-As the file size continues to grow, Python's JSON library continues to be faster, but the memory usage continues to grow at a linear rate. JSON Lineage, on the other hand, continues to use the same amount of memory.
+As the file size continues to grow, Python's JSON library continues to be faster, but the memory usage continues to grow at a linear rate. JSON Lineage, in contrast, continues to use the same amount of memory.
 
 
 ![Benchmark of difference in time as file size grows](/docs/benchmark/time_diff_chart.png)
 
 ![Benchmark of difference in memory as file size grows](/docs/benchmark/mem_diff_chart.png)
 
 #### Installation
```

### Comparing `json-lineage-0.2.1/README.md` & `json-lineage-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 - [JSON Lineage](#json-lineage)
   - [Table of Contents](#table-of-contents)
   - [Introduction](#introduction)
   - [Adapters](#adapters)
     - [Python](#python)
       - [Why not Just Use Python's `json` Library?](#why-not-just-use-pythons-json-library)
       - [Functionality](#functionality)
-      - [Benchmarks](#benchmarks)
+      - [Performance Comparison](#performance-comparison)
       - [Installation](#installation)
       - [Usage](#usage)
         - [Iterating over a JSON file](#iterating-over-a-json-file)
         - [Iterating over a JSON file asynchronously](#iterating-over-a-json-file-asynchronously)
         - [Poorly Formatted JSON](#poorly-formatted-json)
   - [Under the Hood](#under-the-hood)
 
@@ -25,46 +25,43 @@
 
 Additionally, this project contains adapters for easy integration into other programming languages. Currently, there is only a Python adapter, but more are planned.
 
 ## Adapters
 
 ### Python
 
-The Python adapter is a wrapper around the underlying Rust program. It allows for easy integration into Python programs.
-It is designed to feel a similar to the built-in `json` module in Python.
+The Python adapter is a wrapper around the underlying Rust program, providing seamless integration into Python applications. It is designed to have a similar feel to Python's built-in json module.
 
 #### Why not Just Use Python's `json` Library?
 
-Given that Python already has a built-in JSON parser, you may be wondering why you would want to use this library.
-The answer is, well, it depends.
+You might wonder why you would choose to use this library instead of Python's built-in JSON library. The answer depends on your specific use case.
 
-If you are parsing a small JSON file, then you probably don't want to use this library.
+If you are parsing a small JSON file, Python's JSON library is likely sufficient and performs well. However, when dealing with very large JSON files that exceed the available memory, JSON Lineage offers significant benefits.
 
-Python's JSON library is written in C and is very fast. However, as it loads the entire JSON file into memory, it is not suitable for parsing very large JSON files. This is where JSON Lineage comes in.
+Python's JSON library is written in C and is highly optimised for speed. However, it loads the entire JSON file into memory, making it unsuitable for parsing very large JSON files. This is where JSON Lineage shines.
 
-JSON Lineage is designed to parse very
-large JSON files that would otherwise not fit into memory. It does this by parsing the JSON file one object at a time.
+JSON Lineage is specifically designed to parse very large JSON files that would not fit into memory. It achieves this by parsing the JSON file one object at a time.
 
 #### Functionality
 
 The following functionality is provided:
 
 * `load` - Generate an iterator that returns each object in a JSON file.
 * `aload` - Generates an asynchronous iterator that returns each object in a JSON file.
 
 A CLI is also provided for easy conversion of JSON files to JSONL files.
 For information on how to use the CLI, run: `python -m json_lineage --help`.
 
-#### Benchmarks
+#### Performance Comparison
 
 The following graphs compare the speed and memory usage of Python's JSON library vs JSON Lineage.
 
 The benchmarks show that up to a file size of 500MB, the speed difference is negligible. However, already at this point, Python requires almost 2GB of memory to parse the JSON file, while JSON Lineage only requires 1.5GB.
 
-As the file size continues to grow, Python's JSON library continues to be faster, but the memory usage continues to grow at a linear rate. JSON Lineage, on the other hand, continues to use the same amount of memory.
+As the file size continues to grow, Python's JSON library continues to be faster, but the memory usage continues to grow at a linear rate. JSON Lineage, in contrast, continues to use the same amount of memory.
 
 
 ![Benchmark of difference in time as file size grows](/docs/benchmark/time_diff_chart.png)
 
 ![Benchmark of difference in memory as file size grows](/docs/benchmark/mem_diff_chart.png)
 
 #### Installation
```

### Comparing `json-lineage-0.2.1/json_lineage/bin/jsonl_converter` & `json-lineage-0.2.2/json_lineage/bin/jsonl_converter`

 * *Files identical despite different names*

### Comparing `json-lineage-0.2.1/json_lineage/bin/jsonl_converter.exe` & `json-lineage-0.2.2/json_lineage/bin/jsonl_converter.exe`

 * *Files identical despite different names*

### Comparing `json-lineage-0.2.1/json_lineage/bin/tmp.py` & `json-lineage-0.2.2/json_lineage/bin/tmp.py`

 * *Files identical despite different names*

### Comparing `json-lineage-0.2.1/json_lineage/bin_interface.py` & `json-lineage-0.2.2/json_lineage/bin_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import json
 import os
 import platform
 import subprocess
 import typing as _t
 from collections.abc import Awaitable, Coroutine
 
 from .exceptions import BinaryExecutionException
@@ -95,15 +96,15 @@
         if self.process.stdout is None:
             raise StopIteration
         line = self.process.stdout.readline().strip()
         self.raise_err_if_stderr()
         if not line and self.process.poll() is not None:
             raise StopIteration
 
-        return line
+        return json.loads(line)
 
     def raise_err_if_stderr(self) -> None:
         """Raise an exception if the process has exited with a non-zero
         code.
         """
         if self.process.poll() is not None and self.process.poll() != 0:
             if self.process.stderr is None:
@@ -157,15 +158,15 @@
             )
         output = await self.read_output(self.process)
         await self.raise_err_if_stderr()
 
         if not output:
             raise StopAsyncIteration
 
-        return output
+        return json.loads(output)
 
     async def read_output(self, process: asyncio.subprocess.Process) -> str:
         if process.stdout is None:
             return ""
         line = await process.stdout.readline()
         if not line:
             return ""
```

### Comparing `json-lineage-0.2.1/json_lineage/cli.py` & `json-lineage-0.2.2/json_lineage/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains the command line interface for the json_lineage
 adapter.
 """
 
 import argparse
+import json
 
 from .bin_interface import BinaryReader
 
 
 def parse_args() -> argparse.Namespace:
     """Parses the command line arguments."""
     parser = argparse.ArgumentParser(
@@ -38,22 +39,22 @@
 
     return parser.parse_args()
 
 
 def print_lines(reader: BinaryReader) -> None:
     """Prints the lines from the given reader to stdout."""
     for line in reader:
-        print(line)
+        print(json.dumps(line))
 
 
 def write_lines(reader: BinaryReader, filepath: str) -> None:
     """Writes the lines from the given reader to the given filepath."""
     with open(filepath, "w") as f:
         for line in reader:
-            f.write(line + "\n")
+            f.write(json.dumps(line) + "\n")
 
 
 def main() -> None:
     """The main entrypoint for the json_lineage adapter when run as a
     module.
     """
     args = parse_args()
```

### Comparing `json-lineage-0.2.1/json_lineage/public.py` & `json-lineage-0.2.2/json_lineage/public.py`

 * *Files identical despite different names*

### Comparing `json-lineage-0.2.1/json_lineage.egg-info/PKG-INFO` & `json-lineage-0.2.2/json_lineage.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-lineage
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library to parse JSON files iteratively without loading the whole file into memory
 Home-page: https://github.com/Salaah01/json-lineage
 Author: "Salaah Amin"
 License: "MIT"
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 - [JSON Lineage](#json-lineage)
   - [Table of Contents](#table-of-contents)
   - [Introduction](#introduction)
   - [Adapters](#adapters)
     - [Python](#python)
       - [Why not Just Use Python's `json` Library?](#why-not-just-use-pythons-json-library)
       - [Functionality](#functionality)
-      - [Benchmarks](#benchmarks)
+      - [Performance Comparison](#performance-comparison)
       - [Installation](#installation)
       - [Usage](#usage)
         - [Iterating over a JSON file](#iterating-over-a-json-file)
         - [Iterating over a JSON file asynchronously](#iterating-over-a-json-file-asynchronously)
         - [Poorly Formatted JSON](#poorly-formatted-json)
   - [Under the Hood](#under-the-hood)
 
@@ -48,46 +48,43 @@
 
 Additionally, this project contains adapters for easy integration into other programming languages. Currently, there is only a Python adapter, but more are planned.
 
 ## Adapters
 
 ### Python
 
-The Python adapter is a wrapper around the underlying Rust program. It allows for easy integration into Python programs.
-It is designed to feel a similar to the built-in `json` module in Python.
+The Python adapter is a wrapper around the underlying Rust program, providing seamless integration into Python applications. It is designed to have a similar feel to Python's built-in json module.
 
 #### Why not Just Use Python's `json` Library?
 
-Given that Python already has a built-in JSON parser, you may be wondering why you would want to use this library.
-The answer is, well, it depends.
+You might wonder why you would choose to use this library instead of Python's built-in JSON library. The answer depends on your specific use case.
 
-If you are parsing a small JSON file, then you probably don't want to use this library.
+If you are parsing a small JSON file, Python's JSON library is likely sufficient and performs well. However, when dealing with very large JSON files that exceed the available memory, JSON Lineage offers significant benefits.
 
-Python's JSON library is written in C and is very fast. However, as it loads the entire JSON file into memory, it is not suitable for parsing very large JSON files. This is where JSON Lineage comes in.
+Python's JSON library is written in C and is highly optimised for speed. However, it loads the entire JSON file into memory, making it unsuitable for parsing very large JSON files. This is where JSON Lineage shines.
 
-JSON Lineage is designed to parse very
-large JSON files that would otherwise not fit into memory. It does this by parsing the JSON file one object at a time.
+JSON Lineage is specifically designed to parse very large JSON files that would not fit into memory. It achieves this by parsing the JSON file one object at a time.
 
 #### Functionality
 
 The following functionality is provided:
 
 * `load` - Generate an iterator that returns each object in a JSON file.
 * `aload` - Generates an asynchronous iterator that returns each object in a JSON file.
 
 A CLI is also provided for easy conversion of JSON files to JSONL files.
 For information on how to use the CLI, run: `python -m json_lineage --help`.
 
-#### Benchmarks
+#### Performance Comparison
 
 The following graphs compare the speed and memory usage of Python's JSON library vs JSON Lineage.
 
 The benchmarks show that up to a file size of 500MB, the speed difference is negligible. However, already at this point, Python requires almost 2GB of memory to parse the JSON file, while JSON Lineage only requires 1.5GB.
 
-As the file size continues to grow, Python's JSON library continues to be faster, but the memory usage continues to grow at a linear rate. JSON Lineage, on the other hand, continues to use the same amount of memory.
+As the file size continues to grow, Python's JSON library continues to be faster, but the memory usage continues to grow at a linear rate. JSON Lineage, in contrast, continues to use the same amount of memory.
 
 
 ![Benchmark of difference in time as file size grows](/docs/benchmark/time_diff_chart.png)
 
 ![Benchmark of difference in memory as file size grows](/docs/benchmark/mem_diff_chart.png)
 
 #### Installation
```

### Comparing `json-lineage-0.2.1/json_lineage.egg-info/SOURCES.txt` & `json-lineage-0.2.2/json_lineage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json-lineage-0.2.1/setup.cfg` & `json-lineage-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = json-lineage
-version = 0.2.1
+version = 0.2.2
 description = Library to parse JSON files iteratively without loading the whole file into memory
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = "MIT"
 license_file = "LICENSE"
 author = "Salaah Amin"
 url = https://github.com/Salaah01/json-lineage
```

### Comparing `json-lineage-0.2.1/tests/test_bin_interface.py` & `json-lineage-0.2.2/tests/test_bin_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,16 +123,16 @@
         self.reader._proc.communicate()
 
     def test_iter_next_valid(self):
         """Test that the `__next__` method iterates over the binary stdout
         correctly.
         """
         iterator = iter(self.reader)
-        self.assertEqual(next(iterator), '{"a": {"B": 1},"b": 2}')
-        self.assertEqual(next(iterator), '{"a": 1,"b": 2}')
+        self.assertEqual(next(iterator), {"a": {"B": 1}, "b": 2})
+        self.assertEqual(next(iterator), {"a": 1, "b": 2})
         with self.assertRaises(StopIteration):
             next(iterator)
 
     def test_raises_err_if_non_0_return_code_with_stderr_from_bin(self):
         """Test that the `__next__` method raises a `BinaryExecutionException`
         if the binary returns a non-zero return code and there is stderr from
         the binary.
@@ -209,16 +209,16 @@
         self.assertIsInstance(aiter_, bin_interface.AsyncBinaryIterator)
 
     async def test__anext__valid(self):
         """Test that the `__anext__` method iterates over the binary stdout
         correctly.
         """
         iterator = self.reader.__aiter__()
-        self.assertEqual(await iterator.__anext__(), '{"a": {"B": 1},"b": 2}')
-        self.assertEqual(await iterator.__anext__(), '{"a": 1,"b": 2}')
+        self.assertEqual(await iterator.__anext__(), {"a": {"B": 1}, "b": 2})
+        self.assertEqual(await iterator.__anext__(), {"a": 1, "b": 2})
         with self.assertRaises(StopAsyncIteration):
             await iterator.__anext__()
 
 
 class TestAsyncBinaryIterator(ReaderInstanceMixin, IsolatedAsyncioTestCase):
     """Tests for the `AsyncBinaryIterator` class."""
```

### Comparing `json-lineage-0.2.1/tests/test_cli.py` & `json-lineage-0.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `json-lineage-0.2.1/tests/test_public.py` & `json-lineage-0.2.2/tests/test_public.py`

 * *Files identical despite different names*

