# Comparing `tmp/compare_dfs-0.0.5.tar.gz` & `tmp/compare_dfs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compare_dfs-0.0.5.tar", last modified: Tue Jul 11 02:41:34 2023, max compression
+gzip compressed data, was "compare_dfs-0.0.6.tar", last modified: Tue Jul 11 02:48:38 2023, max compression
```

## Comparing `compare_dfs-0.0.5.tar` & `compare_dfs-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:41:34.529718 compare_dfs-0.0.5/
--rw-r--r--   0 rikka      (501) staff       (20)     1073 2023-07-07 08:06:52.000000 compare_dfs-0.0.5/LICENSE
--rw-r--r--   0 rikka      (501) staff       (20)     1448 2023-07-11 02:41:34.529566 compare_dfs-0.0.5/PKG-INFO
--rw-r--r--   0 rikka      (501) staff       (20)     1022 2023-07-11 02:41:14.000000 compare_dfs-0.0.5/README.md
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:41:34.528766 compare_dfs-0.0.5/compare_dfs/
--rw-r--r--   0 rikka      (501) staff       (20)     3068 2023-07-11 02:37:39.000000 compare_dfs-0.0.5/compare_dfs/__init__.py
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:41:34.529397 compare_dfs-0.0.5/compare_dfs.egg-info/
--rw-r--r--   0 rikka      (501) staff       (20)     1448 2023-07-11 02:41:34.000000 compare_dfs-0.0.5/compare_dfs.egg-info/PKG-INFO
--rw-r--r--   0 rikka      (501) staff       (20)      190 2023-07-11 02:41:34.000000 compare_dfs-0.0.5/compare_dfs.egg-info/SOURCES.txt
--rw-r--r--   0 rikka      (501) staff       (20)        1 2023-07-11 02:41:34.000000 compare_dfs-0.0.5/compare_dfs.egg-info/dependency_links.txt
--rw-r--r--   0 rikka      (501) staff       (20)       12 2023-07-11 02:41:34.000000 compare_dfs-0.0.5/compare_dfs.egg-info/top_level.txt
--rw-r--r--   0 rikka      (501) staff       (20)       38 2023-07-11 02:41:34.529763 compare_dfs-0.0.5/setup.cfg
--rw-r--r--   0 rikka      (501) staff       (20)      673 2023-07-11 02:41:25.000000 compare_dfs-0.0.5/setup.py
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:48:38.655380 compare_dfs-0.0.6/
+-rw-r--r--   0 rikka      (501) staff       (20)     1073 2023-07-07 08:06:52.000000 compare_dfs-0.0.6/LICENSE
+-rw-r--r--   0 rikka      (501) staff       (20)     1653 2023-07-11 02:48:38.655233 compare_dfs-0.0.6/PKG-INFO
+-rw-r--r--   0 rikka      (501) staff       (20)     1227 2023-07-11 02:48:21.000000 compare_dfs-0.0.6/README.md
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:48:38.654386 compare_dfs-0.0.6/compare_dfs/
+-rw-r--r--   0 rikka      (501) staff       (20)     3064 2023-07-11 02:47:00.000000 compare_dfs-0.0.6/compare_dfs/__init__.py
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:48:38.655052 compare_dfs-0.0.6/compare_dfs.egg-info/
+-rw-r--r--   0 rikka      (501) staff       (20)     1653 2023-07-11 02:48:38.000000 compare_dfs-0.0.6/compare_dfs.egg-info/PKG-INFO
+-rw-r--r--   0 rikka      (501) staff       (20)      190 2023-07-11 02:48:38.000000 compare_dfs-0.0.6/compare_dfs.egg-info/SOURCES.txt
+-rw-r--r--   0 rikka      (501) staff       (20)        1 2023-07-11 02:48:38.000000 compare_dfs-0.0.6/compare_dfs.egg-info/dependency_links.txt
+-rw-r--r--   0 rikka      (501) staff       (20)       12 2023-07-11 02:48:38.000000 compare_dfs-0.0.6/compare_dfs.egg-info/top_level.txt
+-rw-r--r--   0 rikka      (501) staff       (20)       38 2023-07-11 02:48:38.655427 compare_dfs-0.0.6/setup.cfg
+-rw-r--r--   0 rikka      (501) staff       (20)      673 2023-07-11 02:48:35.000000 compare_dfs-0.0.6/setup.py
```

### Comparing `compare_dfs-0.0.5/LICENSE` & `compare_dfs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `compare_dfs-0.0.5/PKG-INFO` & `compare_dfs-0.0.6/compare_dfs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: compare_dfs
-Version: 0.0.5
+Name: compare-dfs
+Version: 0.0.6
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
-from compare_dfs import compare as compare
+import compare_dfs as cpdfs
 
 df1 = pd.DataFrame({
     "id": [1, 2, 3, 4, 5],
     "name": ["a", "b", "c", "d", "e"],
     "age1": [10, 20, 30, 40, 50],
 })
 df2 = pd.DataFrame({
@@ -36,24 +36,34 @@
     "name": ["a", "b", "f", "d", "e"],
     "age2": [10, 25, 30, 40, 50],
 })
 
 df1.set_index("id", inplace=True)
 df2.set_index("id", inplace=True)
 
-# 检查所有列名一致的列，其余请填入different_col_names
-compare(df1, df2, different_col_names=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
+different_colnames = cpdfs.compare_colnames(df1, df2)
+print(different_colnames)
+
+print(cpdfs.compare(df1, df2, different_colnames, dfname_1="左表", dfname_2="右表"))
 ```
 输出：
 ```
+只在第一个表中的列名：{'age1'}
+只在第二个表中的列名：{'age2'}
+[('age1', 'age2')]
 左表中有，右表中没有的索引：{5}
 右表中有，左表中没有的索引：{6}
 =====================================
    name_左表 name_右表
 id                
 3        c       f
 =====================================
     age1  age2
 id            
 2     20    25
 =====================================
+[   name_左表 name_右表
+id                
+3        c       f,     age1  age2
+id            
+2     20    25]
 ```
```

### Comparing `compare_dfs-0.0.5/compare_dfs/__init__.py` & `compare_dfs-0.0.6/compare_dfs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,30 +27,30 @@
     print(f"只在第二个表中的列名：{set_cols2 - set_cols1}")
     
     return [(col1, col2) for col1, col2 in zip(df1.columns, df2.columns) if col1 != col2]
 
 def compare(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
-    different_col_names: List[Tuple[str, str]] = None,
+    different_colnames: List[Tuple[str, str]] = None,
     dfname_1: str = "左表",
     dfname_2: str = "右表"
 ) -> List[pd.DataFrame]:
     """
     根据一列作为比较的唯一索引，比较两个DataFrame的不同
     
     Parameters
     ----------
     df1 : pd.DataFrame
         第一个DataFrame
     df2 : pd.DataFrame
         第二个DataFrame
     col_index : str
         作为比较的唯一索引的列名
-    different_col_names : List[Tuple[str, str]], optional
+    different_colnames : List[Tuple[str, str]], optional
         比较时，不同的列名，by default None
     dfname_1 : str, optional
         第一个DataFrame的名称，by default "左表"
     dfname_2 : str, optional
         第二个DataFrame的名称，by default "右表"
     
     Returns
@@ -65,15 +65,15 @@
     print(f"{dfname_2}中有，{dfname_1}中没有的索引：{index2 - index1}")
     
     joined = df1.join(df2, how="inner", lsuffix=f"_{dfname_1}", rsuffix=f"_{dfname_2}")
     
     set_cols1 = set(df1.columns)
     set_cols2 = set(df2.columns)
     
-    cols_to_compare = [(f"{col}_{dfname_1}", f"{col}_{dfname_2}") for col in set_cols1 & set_cols2] + different_col_names
+    cols_to_compare = [(f"{col}_{dfname_1}", f"{col}_{dfname_2}") for col in set_cols1 & set_cols2] + different_colnames
     
     result = []
     print("=====================================")
     for col1, col2 in cols_to_compare:
         diff = _compare_cols(joined, col1, col2)
         if not diff.empty:
             result.append(diff)
@@ -95,8 +95,8 @@
         "name": ["a", "b", "f", "d", "e"],
         "age2": [10, 25, 30, 40, 50],
     })
     
     df1.set_index("id", inplace=True)
     df2.set_index("id", inplace=True)
     
-    compare(df1, df2, different_col_names=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
+    compare(df1, df2, different_colnames=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
```

### Comparing `compare_dfs-0.0.5/setup.py` & `compare_dfs-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="compare_dfs", # Replace with your own username
-    version="0.0.5",
+    version="0.0.6",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

