# Comparing `tmp/acquire-3.8.dev1.tar.gz` & `tmp/acquire-3.8.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.8.dev1.tar", last modified: Fri Jul  7 12:12:55 2023, max compression
+gzip compressed data, was "acquire-3.8.dev2.tar", last modified: Tue Jul 11 09:12:26 2023, max compression
```

## Comparing `acquire-3.8.dev1.tar` & `acquire-3.8.dev2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:55.250716 acquire-3.8.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-07 12:12:37.000000 acquire-3.8.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-07 12:12:37.000000 acquire-3.8.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 12:12:37.000000 acquire-3.8.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-07 12:12:55.250716 acquire-3.8.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-07 12:12:37.000000 acquire-3.8.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:55.234715 acquire-3.8.dev1/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:38.000000 acquire-3.8.dev1/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76239 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:55.238715 acquire-3.8.dev1/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:38.000000 acquire-3.8.dev1/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:55.242715 acquire-3.8.dev1/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:38.000000 acquire-3.8.dev1/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:55.242715 acquire-3.8.dev1/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:55.242715 acquire-3.8.dev1/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:38.000000 acquire-3.8.dev1/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:55.246715 acquire-3.8.dev1/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:38.000000 acquire-3.8.dev1/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-07 12:12:37.000000 acquire-3.8.dev1/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-07 12:12:55.000000 acquire-3.8.dev1/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:55.238715 acquire-3.8.dev1/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-07 12:12:55.000000 acquire-3.8.dev1/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-07 12:12:55.000000 acquire-3.8.dev1/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:12:55.000000 acquire-3.8.dev1/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 12:12:55.000000 acquire-3.8.dev1/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 12:12:55.000000 acquire-3.8.dev1/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 12:12:55.000000 acquire-3.8.dev1/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-07 12:12:44.000000 acquire-3.8.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:12:55.250716 acquire-3.8.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:55.250716 acquire-3.8.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:38.000000 acquire-3.8.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:12:55.250716 acquire-3.8.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/test_decryptor_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-07 12:12:37.000000 acquire-3.8.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.480426 acquire-3.8.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 09:12:04.000000 acquire-3.8.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-11 09:12:04.000000 acquire-3.8.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 09:12:04.000000 acquire-3.8.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-11 09:12:26.480426 acquire-3.8.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-11 09:12:04.000000 acquire-3.8.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.456426 acquire-3.8.dev2/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77540 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.460426 acquire-3.8.dev2/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.464426 acquire-3.8.dev2/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.468426 acquire-3.8.dev2/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.468426 acquire-3.8.dev2/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.472426 acquire-3.8.dev2/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.460426 acquire-3.8.dev2/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-11 09:12:13.000000 acquire-3.8.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:12:26.480426 acquire-3.8.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.476426 acquire-3.8.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.480426 acquire-3.8.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_decryptor_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tox.ini
```

### Comparing `acquire-3.8.dev1/LICENSE` & `acquire-3.8.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/PKG-INFO` & `acquire-3.8.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.8.dev1
+Version: 3.8.dev2
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.8.dev1/README.md` & `acquire-3.8.dev2/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/acquire.py` & `acquire-3.8.dev2/acquire/acquire.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import enum
 import functools
 import io
 import itertools
+import json
 import logging
 import os
 import shutil
 import subprocess
 import sys
 import time
 import urllib.parse
@@ -15,14 +16,15 @@
 from pathlib import Path
 from typing import Optional, Union
 
 from dissect.target import Target, exceptions
 from dissect.target.filesystems import dir, ntfs
 from dissect.target.helpers import fsutil
 from dissect.target.loaders.remote import RemoteStreamConnection
+from dissect.target.loaders.targetd import TargetdLoader
 from dissect.target.plugins.apps.webservers import iis
 from dissect.target.plugins.os.windows.log import evt, evtx
 
 from acquire.collector import Collector, get_full_formatted_report, get_report_summary
 from acquire.dynamic.windows.named_objects import NamedObjectType
 from acquire.esxi import esxi_memory_context_manager
 from acquire.hashes import (
@@ -1636,24 +1638,61 @@
             target.os,
         )
         log.warning("features may not work as expected. Please notify upstream for any missing artifacts or features.")
         log.warning("")
         log.warning("========================================== WARNING ==========================================")
 
 
-def acquire_target(target: Target, args: argparse.Namespace, output_ts: Optional[str] = None):
+def modargs2json(args: argparse.Namespace) -> dict:
+    json_opts = {}
+    for module in MODULES.values():
+        cli_arg = module.__cli_args__[0][1]
+        if opt := cli_arg.get("dest"):
+            json_opts[opt] = getattr(args, opt)
+    return json_opts
+
+
+def acquire_target(target: Target, *args, **kwargs):
+    if isinstance(target._loader, TargetdLoader):
+        files = acquire_target_targetd(target, *args, **kwargs)
+    else:
+        files = acquire_target_regular(target, *args, **kwargs)
+    return files
+
+
+def acquire_target_targetd(target: Target, args: argparse.Namespace, output_ts: Optional[str] = None):
+    files = []
+    if not len(target.hostname()):
+        log.error("Unable to initialize targetd.")
+        return files
+    json_opts = modargs2json(args)
+    json_opts["profile"] = args.profile
+    json_opts["file"] = args.file
+    json_opts["directory"] = args.directory
+    json_opts["glob"] = args.glob
+    m = {"targetd-meta": "acquire", "args": json_opts}
+    json_str = json.dumps(m)
+    targetd = target._loader.instance.client
+    targetd.send_message(json_str.encode("utf-8"))
+    targetd.sync()
+    for stream in targetd.streams:
+        files.append(stream.out_file)
+    return files
+
+
+def acquire_target_regular(target: Target, args: argparse.Namespace, output_ts: Optional[str] = None):
+    files = []
     output_ts = output_ts or get_utc_now_str()
     if args.log_to_dir:
         log_file = args.log_path.joinpath(format_output_name("Unknown", output_ts, "log"))
         # This will also rename the log file on disk, which was opened in main(), if the name is different
         reconfigure_log_file(log, log_file, delay=True)
     else:
         log_file = args.log_path
 
-    files = []
     skip_list = set()
     if log_file:
         files.append(log_file)
         if target.path.name == "local":
             skip_list.add(normalize_path(target, log_file, resolve=True))
 
     print_disks_overview(target)
```

### Comparing `acquire-3.8.dev1/acquire/collector.py` & `acquire-3.8.dev2/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/crypt.py` & `acquire-3.8.dev2/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/dynamic/windows/collect.py` & `acquire-3.8.dev2/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/dynamic/windows/handles.py` & `acquire-3.8.dev2/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/dynamic/windows/named_objects.py` & `acquire-3.8.dev2/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/dynamic/windows/ntdll.py` & `acquire-3.8.dev2/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/dynamic/windows/types.py` & `acquire-3.8.dev2/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/esxi.py` & `acquire-3.8.dev2/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/hashes.py` & `acquire-3.8.dev2/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/log.py` & `acquire-3.8.dev2/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/outputs/base.py` & `acquire-3.8.dev2/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/outputs/dir.py` & `acquire-3.8.dev2/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/outputs/tar.py` & `acquire-3.8.dev2/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/tools/decrypter.py` & `acquire-3.8.dev2/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/uploaders/minio.py` & `acquire-3.8.dev2/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/uploaders/plugin.py` & `acquire-3.8.dev2/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/uploaders/plugin_registry.py` & `acquire-3.8.dev2/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire/utils.py` & `acquire-3.8.dev2/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/acquire.egg-info/PKG-INFO` & `acquire-3.8.dev2/acquire.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.8.dev1
+Version: 3.8.dev2
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.8.dev1/acquire.egg-info/SOURCES.txt` & `acquire-3.8.dev2/acquire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/pyproject.toml` & `acquire-3.8.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/conftest.py` & `acquire-3.8.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/docs/Makefile` & `acquire-3.8.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/docs/conf.py` & `acquire-3.8.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/test_acquire_command.py` & `acquire-3.8.dev2/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/test_collector.py` & `acquire-3.8.dev2/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/test_decryptor_funcs.py` & `acquire-3.8.dev2/tests/test_decryptor_funcs.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/test_esxi_memory.py` & `acquire-3.8.dev2/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/test_file_sorting.py` & `acquire-3.8.dev2/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/test_minio_uploader.py` & `acquire-3.8.dev2/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/test_plugin.py` & `acquire-3.8.dev2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tests/test_utils.py` & `acquire-3.8.dev2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev1/tox.ini` & `acquire-3.8.dev2/tox.ini`

 * *Files identical despite different names*

