# Comparing `tmp/tenuki-0.1.0.tar.gz` & `tmp/tenuki-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenuki-0.1.0.tar", last modified: Mon Jul 10 20:04:31 2023, max compression
+gzip compressed data, was "tenuki-0.2.0.tar", last modified: Tue Jul 11 13:38:31 2023, max compression
```

## Comparing `tenuki-0.1.0.tar` & `tenuki-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:04:31.625433 tenuki-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-10 20:04:31.625433 tenuki-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-10 20:04:19.000000 tenuki-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 20:04:19.000000 tenuki-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:04:31.625433 tenuki-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-10 20:04:19.000000 tenuki-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:04:31.625433 tenuki-0.1.0/tenuki/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:04:19.000000 tenuki-0.1.0/tenuki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:04:19.000000 tenuki-0.1.0/tenuki/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-10 20:04:19.000000 tenuki-0.1.0/tenuki/rank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:04:31.625433 tenuki-0.1.0/tenuki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-10 20:04:31.000000 tenuki-0.1.0/tenuki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-10 20:04:31.000000 tenuki-0.1.0/tenuki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:04:31.000000 tenuki-0.1.0/tenuki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 20:04:31.000000 tenuki-0.1.0/tenuki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 20:04:31.000000 tenuki-0.1.0/tenuki.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:04:31.625433 tenuki-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-10 20:04:19.000000 tenuki-0.1.0/tests/test_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:38:31.227589 tenuki-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-11 13:38:31.227589 tenuki-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 13:38:19.000000 tenuki-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 13:38:19.000000 tenuki-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:38:31.227589 tenuki-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-11 13:38:19.000000 tenuki-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:38:31.223589 tenuki-0.2.0/tenuki/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:38:19.000000 tenuki-0.2.0/tenuki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-11 13:38:19.000000 tenuki-0.2.0/tenuki/egf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:38:19.000000 tenuki-0.2.0/tenuki/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-11 13:38:19.000000 tenuki-0.2.0/tenuki/rank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:38:31.227589 tenuki-0.2.0/tenuki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-11 13:38:31.000000 tenuki-0.2.0/tenuki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 13:38:31.000000 tenuki-0.2.0/tenuki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:38:31.000000 tenuki-0.2.0/tenuki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 13:38:31.000000 tenuki-0.2.0/tenuki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 13:38:31.000000 tenuki-0.2.0/tenuki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:38:31.227589 tenuki-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-11 13:38:19.000000 tenuki-0.2.0/tests/test_egf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-11 13:38:19.000000 tenuki-0.2.0/tests/test_rank.py
```

### Comparing `tenuki-0.1.0/PKG-INFO` & `tenuki-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenuki
-Version: 0.1.0
+Version: 0.2.0
 Summary: A set of development tools for go/baduk/wéiqí projects.
 Home-page: https://github.com/konradhalas/tenuki
 Author: Konrad Hałas
 Author-email: halas.konrad@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,21 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # tenuki
 
 A set of development tools for go/baduk/wéiqí projects.
 
+## Installation
+
+Use `pip` or your favorite package manager to install `tenuki`:
+
+```bash
+pip install tenuki
+```
 
 ## Rank
 
 `Rank` class is a representation of a player's rank.
 
 ```python
 from tenuki.rank import Rank
@@ -32,7 +39,21 @@
 rank_1 = Rank.parse("1d")
 rank_2 = Rank.parse("1k")
 
 assert rank_1 > rank_2
 assert rank_1.diff(rank_2) == 1
 assert rank_1 + 8 == Rank.parse("9d")
 ```
+
+### EGF
+
+#### GoR <-> Rank
+
+Convert between GoR and Rank:
+
+```python
+from tenuki.rank import Rank
+from tenuki.egf import gor_to_rank, rank_to_gor
+
+assert gor_to_rank(2100) == Rank.parse("1d")
+assert rank_to_gor(Rank.parse("1d")) == 2100
+```
```

### Comparing `tenuki-0.1.0/setup.py` & `tenuki-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="tenuki",
-    version="0.1.0",
+    version="0.2.0",
     description="A set of development tools for go/baduk/wéiqí projects.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Konrad Hałas",
     author_email="halas.konrad@gmail.com",
     url="https://github.com/konradhalas/tenuki",
     license="MIT",
```

### Comparing `tenuki-0.1.0/tenuki/rank.py` & `tenuki-0.2.0/tenuki/rank.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import re
 from dataclasses import dataclass
-from enum import StrEnum, Enum
+from enum import Enum
 from functools import total_ordering
 
 
 class RankLevel(Enum):
     KYU = "k"
     DAN = "d"
     PRO = "p"
@@ -21,14 +21,18 @@
 class Rank:
     value: int
     level: RankLevel
 
     def __str__(self):
         return f"{self.value}{self.level.value}"
 
+    def __post_init__(self):
+        if self.value < 1 or (self.level in [RankLevel.DAN, RankLevel.PRO] and self.value > 9):
+            raise ValueError(f"Invalid rank: {self.value}{self.level.value}")
+
     def __lt__(self, other: Rank) -> bool:
         if self.level == other.level:
             if self.level == RankLevel.KYU:
                 return self.value > other.value
             else:
                 return self.value < other.value
         return self.level < other.level
```

### Comparing `tenuki-0.1.0/tenuki.egg-info/PKG-INFO` & `tenuki-0.2.0/tenuki.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenuki
-Version: 0.1.0
+Version: 0.2.0
 Summary: A set of development tools for go/baduk/wéiqí projects.
 Home-page: https://github.com/konradhalas/tenuki
 Author: Konrad Hałas
 Author-email: halas.konrad@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,21 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # tenuki
 
 A set of development tools for go/baduk/wéiqí projects.
 
+## Installation
+
+Use `pip` or your favorite package manager to install `tenuki`:
+
+```bash
+pip install tenuki
+```
 
 ## Rank
 
 `Rank` class is a representation of a player's rank.
 
 ```python
 from tenuki.rank import Rank
@@ -32,7 +39,21 @@
 rank_1 = Rank.parse("1d")
 rank_2 = Rank.parse("1k")
 
 assert rank_1 > rank_2
 assert rank_1.diff(rank_2) == 1
 assert rank_1 + 8 == Rank.parse("9d")
 ```
+
+### EGF
+
+#### GoR <-> Rank
+
+Convert between GoR and Rank:
+
+```python
+from tenuki.rank import Rank
+from tenuki.egf import gor_to_rank, rank_to_gor
+
+assert gor_to_rank(2100) == Rank.parse("1d")
+assert rank_to_gor(Rank.parse("1d")) == 2100
+```
```

### Comparing `tenuki-0.1.0/tests/test_rank.py` & `tenuki-0.2.0/tests/test_rank.py`

 * *Files identical despite different names*

