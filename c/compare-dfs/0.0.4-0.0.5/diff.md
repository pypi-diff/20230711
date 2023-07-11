# Comparing `tmp/compare_dfs-0.0.4.tar.gz` & `tmp/compare_dfs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compare_dfs-0.0.4.tar", last modified: Tue Jul 11 02:38:29 2023, max compression
+gzip compressed data, was "compare_dfs-0.0.5.tar", last modified: Tue Jul 11 02:41:34 2023, max compression
```

## Comparing `compare_dfs-0.0.4.tar` & `compare_dfs-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:38:29.124809 compare_dfs-0.0.4/
--rw-r--r--   0 rikka      (501) staff       (20)     1073 2023-07-07 08:06:52.000000 compare_dfs-0.0.4/LICENSE
--rw-r--r--   0 rikka      (501) staff       (20)     1443 2023-07-11 02:38:29.124647 compare_dfs-0.0.4/PKG-INFO
--rw-r--r--   0 rikka      (501) staff       (20)     1017 2023-07-11 02:38:01.000000 compare_dfs-0.0.4/README.md
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:38:29.123712 compare_dfs-0.0.4/compare_dfs/
--rw-r--r--   0 rikka      (501) staff       (20)     3068 2023-07-11 02:37:39.000000 compare_dfs-0.0.4/compare_dfs/__init__.py
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:38:29.124459 compare_dfs-0.0.4/compare_dfs.egg-info/
--rw-r--r--   0 rikka      (501) staff       (20)     1443 2023-07-11 02:38:29.000000 compare_dfs-0.0.4/compare_dfs.egg-info/PKG-INFO
--rw-r--r--   0 rikka      (501) staff       (20)      190 2023-07-11 02:38:29.000000 compare_dfs-0.0.4/compare_dfs.egg-info/SOURCES.txt
--rw-r--r--   0 rikka      (501) staff       (20)        1 2023-07-11 02:38:29.000000 compare_dfs-0.0.4/compare_dfs.egg-info/dependency_links.txt
--rw-r--r--   0 rikka      (501) staff       (20)       12 2023-07-11 02:38:29.000000 compare_dfs-0.0.4/compare_dfs.egg-info/top_level.txt
--rw-r--r--   0 rikka      (501) staff       (20)       38 2023-07-11 02:38:29.124862 compare_dfs-0.0.4/setup.cfg
--rw-r--r--   0 rikka      (501) staff       (20)      673 2023-07-11 02:38:27.000000 compare_dfs-0.0.4/setup.py
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:41:34.529718 compare_dfs-0.0.5/
+-rw-r--r--   0 rikka      (501) staff       (20)     1073 2023-07-07 08:06:52.000000 compare_dfs-0.0.5/LICENSE
+-rw-r--r--   0 rikka      (501) staff       (20)     1448 2023-07-11 02:41:34.529566 compare_dfs-0.0.5/PKG-INFO
+-rw-r--r--   0 rikka      (501) staff       (20)     1022 2023-07-11 02:41:14.000000 compare_dfs-0.0.5/README.md
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:41:34.528766 compare_dfs-0.0.5/compare_dfs/
+-rw-r--r--   0 rikka      (501) staff       (20)     3068 2023-07-11 02:37:39.000000 compare_dfs-0.0.5/compare_dfs/__init__.py
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:41:34.529397 compare_dfs-0.0.5/compare_dfs.egg-info/
+-rw-r--r--   0 rikka      (501) staff       (20)     1448 2023-07-11 02:41:34.000000 compare_dfs-0.0.5/compare_dfs.egg-info/PKG-INFO
+-rw-r--r--   0 rikka      (501) staff       (20)      190 2023-07-11 02:41:34.000000 compare_dfs-0.0.5/compare_dfs.egg-info/SOURCES.txt
+-rw-r--r--   0 rikka      (501) staff       (20)        1 2023-07-11 02:41:34.000000 compare_dfs-0.0.5/compare_dfs.egg-info/dependency_links.txt
+-rw-r--r--   0 rikka      (501) staff       (20)       12 2023-07-11 02:41:34.000000 compare_dfs-0.0.5/compare_dfs.egg-info/top_level.txt
+-rw-r--r--   0 rikka      (501) staff       (20)       38 2023-07-11 02:41:34.529763 compare_dfs-0.0.5/setup.cfg
+-rw-r--r--   0 rikka      (501) staff       (20)      673 2023-07-11 02:41:25.000000 compare_dfs-0.0.5/setup.py
```

### Comparing `compare_dfs-0.0.4/LICENSE` & `compare_dfs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `compare_dfs-0.0.4/PKG-INFO` & `compare_dfs-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compare_dfs
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 ```bash
 pip install compare_dfs
 ```
 
 ## 使用
 ```python
 import pandas as pd
-import compare_dfs.compare as compare
+from compare_dfs import compare as compare
 
 df1 = pd.DataFrame({
     "id": [1, 2, 3, 4, 5],
     "name": ["a", "b", "c", "d", "e"],
     "age1": [10, 20, 30, 40, 50],
 })
 df2 = pd.DataFrame({
```

### Comparing `compare_dfs-0.0.4/README.md` & `compare_dfs-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ```bash
 pip install compare_dfs
 ```
 
 ## 使用
 ```python
 import pandas as pd
-import compare_dfs.compare as compare
+from compare_dfs import compare as compare
 
 df1 = pd.DataFrame({
     "id": [1, 2, 3, 4, 5],
     "name": ["a", "b", "c", "d", "e"],
     "age1": [10, 20, 30, 40, 50],
 })
 df2 = pd.DataFrame({
```

### Comparing `compare_dfs-0.0.4/compare_dfs/__init__.py` & `compare_dfs-0.0.5/compare_dfs/__init__.py`

 * *Files identical despite different names*

### Comparing `compare_dfs-0.0.4/compare_dfs.egg-info/PKG-INFO` & `compare_dfs-0.0.5/compare_dfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compare-dfs
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 ```bash
 pip install compare_dfs
 ```
 
 ## 使用
 ```python
 import pandas as pd
-import compare_dfs.compare as compare
+from compare_dfs import compare as compare
 
 df1 = pd.DataFrame({
     "id": [1, 2, 3, 4, 5],
     "name": ["a", "b", "c", "d", "e"],
     "age1": [10, 20, 30, 40, 50],
 })
 df2 = pd.DataFrame({
```

### Comparing `compare_dfs-0.0.4/setup.py` & `compare_dfs-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="compare_dfs", # Replace with your own username
-    version="0.0.4",
+    version="0.0.5",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

