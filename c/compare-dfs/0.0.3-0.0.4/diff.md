# Comparing `tmp/compare_dfs-0.0.3.tar.gz` & `tmp/compare_dfs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compare_dfs-0.0.3.tar", last modified: Fri Jul  7 09:03:49 2023, max compression
+gzip compressed data, was "compare_dfs-0.0.4.tar", last modified: Tue Jul 11 02:38:29 2023, max compression
```

## Comparing `compare_dfs-0.0.3.tar` & `compare_dfs-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:03:49.779730 compare_dfs-0.0.3/
--rw-r--r--   0 rikka      (501) staff       (20)     1073 2023-07-07 08:06:52.000000 compare_dfs-0.0.3/LICENSE
--rw-r--r--   0 rikka      (501) staff       (20)     1402 2023-07-07 09:03:49.779574 compare_dfs-0.0.3/PKG-INFO
--rw-r--r--   0 rikka      (501) staff       (20)      976 2023-07-07 09:02:55.000000 compare_dfs-0.0.3/README.md
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:03:49.778755 compare_dfs-0.0.3/compare_dfs/
--rw-r--r--   0 rikka      (501) staff       (20)     2395 2023-07-07 08:44:18.000000 compare_dfs-0.0.3/compare_dfs/__init__.py
-drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-07 09:03:49.779383 compare_dfs-0.0.3/compare_dfs.egg-info/
--rw-r--r--   0 rikka      (501) staff       (20)     1402 2023-07-07 09:03:49.000000 compare_dfs-0.0.3/compare_dfs.egg-info/PKG-INFO
--rw-r--r--   0 rikka      (501) staff       (20)      190 2023-07-07 09:03:49.000000 compare_dfs-0.0.3/compare_dfs.egg-info/SOURCES.txt
--rw-r--r--   0 rikka      (501) staff       (20)        1 2023-07-07 09:03:49.000000 compare_dfs-0.0.3/compare_dfs.egg-info/dependency_links.txt
--rw-r--r--   0 rikka      (501) staff       (20)       12 2023-07-07 09:03:49.000000 compare_dfs-0.0.3/compare_dfs.egg-info/top_level.txt
--rw-r--r--   0 rikka      (501) staff       (20)       38 2023-07-07 09:03:49.779782 compare_dfs-0.0.3/setup.cfg
--rw-r--r--   0 rikka      (501) staff       (20)      673 2023-07-07 09:03:43.000000 compare_dfs-0.0.3/setup.py
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:38:29.124809 compare_dfs-0.0.4/
+-rw-r--r--   0 rikka      (501) staff       (20)     1073 2023-07-07 08:06:52.000000 compare_dfs-0.0.4/LICENSE
+-rw-r--r--   0 rikka      (501) staff       (20)     1443 2023-07-11 02:38:29.124647 compare_dfs-0.0.4/PKG-INFO
+-rw-r--r--   0 rikka      (501) staff       (20)     1017 2023-07-11 02:38:01.000000 compare_dfs-0.0.4/README.md
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:38:29.123712 compare_dfs-0.0.4/compare_dfs/
+-rw-r--r--   0 rikka      (501) staff       (20)     3068 2023-07-11 02:37:39.000000 compare_dfs-0.0.4/compare_dfs/__init__.py
+drwxr-xr-x   0 rikka      (501) staff       (20)        0 2023-07-11 02:38:29.124459 compare_dfs-0.0.4/compare_dfs.egg-info/
+-rw-r--r--   0 rikka      (501) staff       (20)     1443 2023-07-11 02:38:29.000000 compare_dfs-0.0.4/compare_dfs.egg-info/PKG-INFO
+-rw-r--r--   0 rikka      (501) staff       (20)      190 2023-07-11 02:38:29.000000 compare_dfs-0.0.4/compare_dfs.egg-info/SOURCES.txt
+-rw-r--r--   0 rikka      (501) staff       (20)        1 2023-07-11 02:38:29.000000 compare_dfs-0.0.4/compare_dfs.egg-info/dependency_links.txt
+-rw-r--r--   0 rikka      (501) staff       (20)       12 2023-07-11 02:38:29.000000 compare_dfs-0.0.4/compare_dfs.egg-info/top_level.txt
+-rw-r--r--   0 rikka      (501) staff       (20)       38 2023-07-11 02:38:29.124862 compare_dfs-0.0.4/setup.cfg
+-rw-r--r--   0 rikka      (501) staff       (20)      673 2023-07-11 02:38:27.000000 compare_dfs-0.0.4/setup.py
```

### Comparing `compare_dfs-0.0.3/LICENSE` & `compare_dfs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `compare_dfs-0.0.3/PKG-INFO` & `compare_dfs-0.0.4/compare_dfs.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: compare_dfs
-Version: 0.0.3
+Name: compare-dfs
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,28 +27,30 @@
 import compare_dfs.compare as compare
 
 df1 = pd.DataFrame({
     "id": [1, 2, 3, 4, 5],
     "name": ["a", "b", "c", "d", "e"],
     "age1": [10, 20, 30, 40, 50],
 })
-                   
 df2 = pd.DataFrame({
     "id": [1, 2, 3, 4, 6],
     "name": ["a", "b", "f", "d", "e"],
     "age2": [10, 25, 30, 40, 50],
 })
 
+df1.set_index("id", inplace=True)
+df2.set_index("id", inplace=True)
+
 # 检查所有列名一致的列，其余请填入different_col_names
-compare(df1, df2, col_index="id", different_col_names=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
+compare(df1, df2, different_col_names=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
 ```
 输出：
 ```
-左表中有，右表中没有的id：{5}
-右表中有，左表中没有的id：{6}
+左表中有，右表中没有的索引：{5}
+右表中有，左表中没有的索引：{6}
 =====================================
    name_左表 name_右表
 id                
 3        c       f
 =====================================
     age1  age2
 id
```

### Comparing `compare_dfs-0.0.3/README.md` & `compare_dfs-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 import compare_dfs.compare as compare
 
 df1 = pd.DataFrame({
     "id": [1, 2, 3, 4, 5],
     "name": ["a", "b", "c", "d", "e"],
     "age1": [10, 20, 30, 40, 50],
 })
-                   
 df2 = pd.DataFrame({
     "id": [1, 2, 3, 4, 6],
     "name": ["a", "b", "f", "d", "e"],
     "age2": [10, 25, 30, 40, 50],
 })
 
+df1.set_index("id", inplace=True)
+df2.set_index("id", inplace=True)
+
 # 检查所有列名一致的列，其余请填入different_col_names
-compare(df1, df2, col_index="id", different_col_names=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
+compare(df1, df2, different_col_names=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
 ```
 输出：
 ```
-左表中有，右表中没有的id：{5}
-右表中有，左表中没有的id：{6}
+左表中有，右表中没有的索引：{5}
+右表中有，左表中没有的索引：{6}
 =====================================
    name_左表 name_右表
 id                
 3        c       f
 =====================================
     age1  age2
 id
```

### Comparing `compare_dfs-0.0.3/compare_dfs/__init__.py` & `compare_dfs-0.0.4/compare_dfs/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,40 @@
 import pandas as pd
 from typing import List, Tuple
 
 def _compare_cols(df, col1, col2):
     return df[df[col1] != df[col2]][[col1, col2]]
 
+def compare_colnames(df1: pd.DataFrame, df2: pd.DataFrame) -> List[Tuple[str, str]]:
+    """
+    比较两个DataFrame的列名
+    
+    Parameters
+    ----------
+    df1 : pd.DataFrame
+        第一个DataFrame
+    df2 : pd.DataFrame
+        第二个DataFrame
+    
+    Returns
+    -------
+    List[Tuple[str, str]]
+        返回名字不同但位置相同的列名对
+    """
+    set_cols1 = set(df1.columns)
+    set_cols2 = set(df2.columns)
+    
+    print(f"只在第一个表中的列名：{set_cols1 - set_cols2}")
+    print(f"只在第二个表中的列名：{set_cols2 - set_cols1}")
+    
+    return [(col1, col2) for col1, col2 in zip(df1.columns, df2.columns) if col1 != col2]
+
 def compare(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
-    col_index: str,
     different_col_names: List[Tuple[str, str]] = None,
     dfname_1: str = "左表",
     dfname_2: str = "右表"
 ) -> List[pd.DataFrame]:
     """
     根据一列作为比较的唯一索引，比较两个DataFrame的不同
     
@@ -31,45 +54,49 @@
         第二个DataFrame的名称，by default "右表"
     
     Returns
     -------
     List[pd.DataFrame]
         返回存在差异的数据
     """
-    set_index1 = set(df1[col_index])
-    set_index2 = set(df2[col_index])
+    index1 = set(df1.index)
+    index2 = set(df2.index)
     
-    print(f"{dfname_1}中有，{dfname_2}中没有的{col_index}：{set_index1 - set_index2}")
-    print(f"{dfname_2}中有，{dfname_1}中没有的{col_index}：{set_index2 - set_index1}")
+    print(f"{dfname_1}中有，{dfname_2}中没有的索引：{index1 - index2}")
+    print(f"{dfname_2}中有，{dfname_1}中没有的索引：{index2 - index1}")
     
-    merged = pd.merge(df1, df2, on=col_index, how="inner", suffixes=(f"_{dfname_1}", f"_{dfname_2}"))
-    merged.set_index(col_index, inplace=True)
+    joined = df1.join(df2, how="inner", lsuffix=f"_{dfname_1}", rsuffix=f"_{dfname_2}")
     
-    set_cols1 = set(df1.columns) - set([col_index])
-    set_cols2 = set(df2.columns) - set([col_index])
+    set_cols1 = set(df1.columns)
+    set_cols2 = set(df2.columns)
     
     cols_to_compare = [(f"{col}_{dfname_1}", f"{col}_{dfname_2}") for col in set_cols1 & set_cols2] + different_col_names
     
     result = []
     print("=====================================")
     for col1, col2 in cols_to_compare:
-        diff = _compare_cols(merged, col1, col2)
+        diff = _compare_cols(joined, col1, col2)
         if not diff.empty:
             result.append(diff)
             print(diff)
             print("=====================================")
             
     return result
 
-df1 = pd.DataFrame({
-    "id": [1, 2, 3, 4, 5],
-    "name": ["a", "b", "c", "d", "e"],
-    "age1": [10, 20, 30, 40, 50],
-})
-                   
-df2 = pd.DataFrame({
-    "id": [1, 2, 3, 4, 6],
-    "name": ["a", "b", "f", "d", "e"],
-    "age2": [10, 25, 30, 40, 50],
-})
-
-compare(df1, df2, col_index="id", different_col_names=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
+if __name__ == "__main__":
+    
+    df1 = pd.DataFrame({
+        "id": [1, 2, 3, 4, 5],
+        "name": ["a", "b", "c", "d", "e"],
+        "age1": [10, 20, 30, 40, 50],
+    })
+                    
+    df2 = pd.DataFrame({
+        "id": [1, 2, 3, 4, 6],
+        "name": ["a", "b", "f", "d", "e"],
+        "age2": [10, 25, 30, 40, 50],
+    })
+    
+    df1.set_index("id", inplace=True)
+    df2.set_index("id", inplace=True)
+    
+    compare(df1, df2, different_col_names=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
```

### Comparing `compare_dfs-0.0.3/compare_dfs.egg-info/PKG-INFO` & `compare_dfs-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: compare-dfs
-Version: 0.0.3
+Name: compare_dfs
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,28 +27,30 @@
 import compare_dfs.compare as compare
 
 df1 = pd.DataFrame({
     "id": [1, 2, 3, 4, 5],
     "name": ["a", "b", "c", "d", "e"],
     "age1": [10, 20, 30, 40, 50],
 })
-                   
 df2 = pd.DataFrame({
     "id": [1, 2, 3, 4, 6],
     "name": ["a", "b", "f", "d", "e"],
     "age2": [10, 25, 30, 40, 50],
 })
 
+df1.set_index("id", inplace=True)
+df2.set_index("id", inplace=True)
+
 # 检查所有列名一致的列，其余请填入different_col_names
-compare(df1, df2, col_index="id", different_col_names=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
+compare(df1, df2, different_col_names=[("age1", "age2")], dfname_1="左表", dfname_2="右表")
 ```
 输出：
 ```
-左表中有，右表中没有的id：{5}
-右表中有，左表中没有的id：{6}
+左表中有，右表中没有的索引：{5}
+右表中有，左表中没有的索引：{6}
 =====================================
    name_左表 name_右表
 id                
 3        c       f
 =====================================
     age1  age2
 id
```

### Comparing `compare_dfs-0.0.3/setup.py` & `compare_dfs-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="compare_dfs", # Replace with your own username
-    version="0.0.3",
+    version="0.0.4",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

