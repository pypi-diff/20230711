# Comparing `tmp/SusteenExToPy-0.0.6.tar.gz` & `tmp/SusteenExToPy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SusteenExToPy-0.0.6.tar", last modified: Tue Jul 11 08:03:28 2023, max compression
+gzip compressed data, was "SusteenExToPy-0.0.7.tar", last modified: Tue Jul 11 14:34:25 2023, max compression
```

## Comparing `SusteenExToPy-0.0.6.tar` & `SusteenExToPy-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 08:03:28.413846 SusteenExToPy-0.0.6/
--rw-rw-rw-   0        0        0        0 2023-07-11 07:50:01.000000 SusteenExToPy-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      512 2023-07-11 08:03:28.413846 SusteenExToPy-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      108 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      691 2023-07-11 08:03:28.418172 SusteenExToPy-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 08:03:28.097790 SusteenExToPy-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 08:03:28.320656 SusteenExToPy-0.0.6/src/SusteenExToPy/
--rw-rw-rw-   0        0        0     8893 2022-04-21 10:44:54.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/Cell.py
--rw-rw-rw-   0        0        0       58 2021-11-25 12:38:23.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/CellBase.py
--rw-rw-rw-   0        0        0     1796 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/ExcelCompiler.py
--rw-rw-rw-   0        0        0      338 2021-11-25 12:38:23.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/ExcelError.py
--rw-rw-rw-   0        0        0    20727 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/Range.py
--rw-rw-rw-   0        0        0    45260 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/Spreadsheet.py
--rw-rw-rw-   0        0        0      323 2021-11-25 12:38:23.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 08:03:28.407999 SusteenExToPy-0.0.6/src/SusteenExToPy/ast/
--rw-rw-rw-   0        0        0    24426 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/ast/__init__.py
--rw-rw-rw-   0        0        0    14013 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/ast/astnodes.py
--rw-rw-rw-   0        0        0    88704 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/excellib.py
--rw-rw-rw-   0        0        0      430 2021-11-25 12:38:23.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/functions.json
--rw-rw-rw-   0        0        0    12013 2022-04-21 11:22:09.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/reader.py
--rw-rw-rw-   0        0        0     1387 2021-12-13 14:11:39.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/roundxtest.py
--rw-rw-rw-   0        0        0     8515 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/serializer.py
--rw-rw-rw-   0        0        0    29893 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/tokenizer.py
--rw-rw-rw-   0        0        0    18661 2021-11-25 12:38:23.000000 SusteenExToPy-0.0.6/src/SusteenExToPy/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 08:03:28.370489 SusteenExToPy-0.0.6/src/SusteenExToPy.egg-info/
--rw-rw-rw-   0        0        0      512 2023-07-11 08:03:28.000000 SusteenExToPy-0.0.6/src/SusteenExToPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-07-11 08:03:28.000000 SusteenExToPy-0.0.6/src/SusteenExToPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 08:03:28.000000 SusteenExToPy-0.0.6/src/SusteenExToPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-11 08:03:28.000000 SusteenExToPy-0.0.6/src/SusteenExToPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:25.140578 SusteenExToPy-0.0.7/
+-rw-rw-rw-   0        0        0        0 2023-07-11 07:50:01.000000 SusteenExToPy-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      512 2023-07-11 14:34:25.141872 SusteenExToPy-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      691 2023-07-11 14:34:25.146329 SusteenExToPy-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:24.973300 SusteenExToPy-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:25.090605 SusteenExToPy-0.0.7/src/SusteenExToPy/
+-rw-rw-rw-   0        0        0     8909 2023-07-11 14:19:24.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/Cell.py
+-rw-rw-rw-   0        0        0       58 2021-11-25 12:38:23.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/CellBase.py
+-rw-rw-rw-   0        0        0     1796 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/ExcelCompiler.py
+-rw-rw-rw-   0        0        0      338 2021-11-25 12:38:23.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/ExcelError.py
+-rw-rw-rw-   0        0        0    20742 2023-07-11 14:32:28.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/Range.py
+-rw-rw-rw-   0        0        0    45276 2023-07-11 14:32:25.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/Spreadsheet.py
+-rw-rw-rw-   0        0        0      323 2021-11-25 12:38:23.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:25.138538 SusteenExToPy-0.0.7/src/SusteenExToPy/ast/
+-rw-rw-rw-   0        0        0    24442 2023-07-11 14:16:50.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/ast/__init__.py
+-rw-rw-rw-   0        0        0    14029 2023-07-11 14:18:13.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/ast/astnodes.py
+-rw-rw-rw-   0        0        0    88720 2023-07-11 14:32:32.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/excellib.py
+-rw-rw-rw-   0        0        0      430 2021-11-25 12:38:23.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/functions.json
+-rw-rw-rw-   0        0        0    12013 2022-04-21 11:22:09.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/reader.py
+-rw-rw-rw-   0        0        0     1387 2021-12-13 14:11:39.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/roundxtest.py
+-rw-rw-rw-   0        0        0     8531 2023-07-11 14:32:27.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/serializer.py
+-rw-rw-rw-   0        0        0    29893 2022-04-21 10:44:58.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/tokenizer.py
+-rw-rw-rw-   0        0        0    18677 2023-07-11 14:32:54.000000 SusteenExToPy-0.0.7/src/SusteenExToPy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:25.115139 SusteenExToPy-0.0.7/src/SusteenExToPy.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-07-11 14:34:24.000000 SusteenExToPy-0.0.7/src/SusteenExToPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-07-11 14:34:24.000000 SusteenExToPy-0.0.7/src/SusteenExToPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:34:24.000000 SusteenExToPy-0.0.7/src/SusteenExToPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-11 14:34:24.000000 SusteenExToPy-0.0.7/src/SusteenExToPy.egg-info/top_level.txt
```

### Comparing `SusteenExToPy-0.0.6/PKG-INFO` & `SusteenExToPy-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SusteenExToPy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: jurjen de groot
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SusteenExToPy-0.0.6/setup.cfg` & `SusteenExToPy-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7573 7465 656e 4578 546f 5079   = SusteenExToPy
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 360d 0a61 7574 686f 7220 3d20 6a75 726a  6..author = jurj
+00000030: 370d 0a61 7574 686f 7220 3d20 6a75 726a  7..author = jurj
 00000040: 656e 2064 6520 6772 6f6f 740d 0a61 7574  en de groot..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6175 7468  hor_email = auth
 00000060: 6f72 4065 7861 6d70 6c65 2e63 6f6d 0d0a  or@example.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000080: 736d 616c 6c20 6578 616d 706c 6520 7061  small example pa
 00000090: 636b 6167 650d 0a6c 6f6e 675f 6465 7363  ckage..long_desc
 000000a0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file:
```

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/Cell.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/Cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from __future__ import absolute_import, division
 
 from SusteenExToPy.CellBase import CellBase
 from SusteenExToPy.Range import RangeCore
 from SusteenExToPy.utils import *
 
-from openpyxl.compat import unicode
+# from openpyxl.compat import unicode
+unicode = str
 
 
 class Cell(CellBase):
     ctr = 0
     __named_range = None
 
     @classmethod
```

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/ExcelCompiler.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/ExcelCompiler.py`

 * *Files identical despite different names*

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/Range.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/Range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import absolute_import, division, print_function
 
 from SusteenExToPy.CellBase import CellBase
 from SusteenExToPy.ExcelError import ErrorCodes, ExcelError
 from SusteenExToPy.utils import *
 
-from openpyxl.compat import unicode
-
+# from openpyxl.compat import unicode
+unicode = str
 
 # WARNING: Range should never be imported directly. Import Range from excelutils instead.
 
 ### Range Utils ###
 
 parse_cell_addr_cache = {}
```

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/Spreadsheet.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/Spreadsheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from SusteenExToPy.utils import *
 
 import warnings
 import os.path
 import networkx
 from networkx.readwrite import json_graph
 
-from openpyxl.compat import unicode
+# from openpyxl.compat import unicode
+unicode = str
 
 
 class Spreadsheet(object):
     def __init__(self, file=None, ignore_sheets=[], ignore_hidden=False, debug=False):
         # print("___### Initializing Excel Compiler ###___")
 
         if file is None:
```

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/ast/__init__.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/ast/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # cython: profile=True
 
 import collections
 import six
 
 import networkx
 from networkx.classes.digraph import DiGraph
-from openpyxl.compat import unicode
+# from openpyxl.compat import unicode
+unicode = str
 
 from SusteenExToPy.utils import uniqueify, flatten, max_dimension, col2num, resolve_range
 from SusteenExToPy.Cell import Cell
 from SusteenExToPy.Range import parse_cell_address
 from SusteenExToPy.tokenizer import ExcelParser, f_token
 from .astnodes import *
```

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/ast/astnodes.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/ast/astnodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import print_function
 # cython: profile=True
 
-from openpyxl.compat import unicode
+# from openpyxl.compat import unicode
+unicode = str
 
 from SusteenExToPy.excellib import FUNCTION_MAP, IND_FUN
 from SusteenExToPy.utils import is_range, split_range, split_address, resolve_range
 from SusteenExToPy.ExcelError import *
 
 
 def to_str(my_string):
```

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/excellib.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/excellib.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 import datetime
 import random
 from math import log, ceil
 from decimal import Decimal, ROUND_UP, ROUND_HALF_UP
 from calendar import monthrange
 from dateutil.relativedelta import relativedelta
 
-from openpyxl.compat import unicode
+# from openpyxl.compat import unicode
+unicode = str
 
 from SusteenExToPy.utils import *
 from SusteenExToPy.Range import RangeCore as Range
 from SusteenExToPy.ExcelError import *
 from functools import reduce
 
 ######################################################################################
```

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/reader.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/reader.py`

 * *Files identical despite different names*

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/roundxtest.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/roundxtest.py`

 * *Files identical despite different names*

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/serializer.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import json
 import gzip
 import networkx
 
 from networkx.classes.digraph import DiGraph
 from networkx.readwrite import json_graph
 from networkx.drawing.nx_pydot import write_dot
-from openpyxl.compat import unicode
+# from openpyxl.compat import unicode
+unicode = str
 
 from SusteenExToPy.Cell import Cell
 from SusteenExToPy.Range import RangeCore, RangeFactory
 
 SEP = ";;"
 
 ########### based on custom format #################
```

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/tokenizer.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/tokenizer.py`

 * *Files identical despite different names*

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy/utils.py` & `SusteenExToPy-0.0.7/src/SusteenExToPy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 try:
     from functools import lru_cache
 except ImportError:  # fix for Python 2.7
     from backports.functools_lru_cache import lru_cache
 from six import string_types
 from copy import deepcopy
 
-from openpyxl.compat import unicode
+# from openpyxl.compat import unicode
+unicode = str
 
 from .ExcelError import ExcelError
 
 ASCII = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
 
 # source: https://github.com/dgorissen/pycel/blob/master/src/pycel/excelutil.py
```

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy.egg-info/PKG-INFO` & `SusteenExToPy-0.0.7/src/SusteenExToPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SusteenExToPy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: jurjen de groot
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SusteenExToPy-0.0.6/src/SusteenExToPy.egg-info/SOURCES.txt` & `SusteenExToPy-0.0.7/src/SusteenExToPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

