# Comparing `tmp/mwsqlite-1.2.2.tar.gz` & `tmp/mwsqlite-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mwsqlite-1.2.2.tar", last modified: Mon Jun 26 20:58:46 2023, max compression
+gzip compressed data, was "dist\mwsqlite-1.2.3.tar", last modified: Tue Jul 11 11:00:06 2023, max compression
```

## Comparing `mwsqlite-1.2.2.tar` & `mwsqlite-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 20:58:46.077516 mwsqlite-1.2.2/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 mwsqlite-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     3172 2023-06-26 20:58:46.078517 mwsqlite-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2075 2022-12-19 15:39:05.000000 mwsqlite-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 20:58:46.064513 mwsqlite-1.2.2/mwsqlite/
--rw-rw-rw-   0        0        0      186 2022-12-19 10:39:07.000000 mwsqlite-1.2.2/mwsqlite/__init__.py
--rw-rw-rw-   0        0        0     1513 2022-12-23 17:48:52.000000 mwsqlite-1.2.2/mwsqlite/_types.py
--rw-rw-rw-   0        0        0    14773 2023-06-26 20:56:30.000000 mwsqlite-1.2.2/mwsqlite/mw_sql.py
--rw-rw-rw-   0        0        0     3388 2022-12-23 15:06:08.000000 mwsqlite-1.2.2/mwsqlite/sql_compile.py
--rw-rw-rw-   0        0        0      551 2022-12-23 17:48:26.000000 mwsqlite-1.2.2/mwsqlite/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:58:46.076516 mwsqlite-1.2.2/mwsqlite.egg-info/
--rw-rw-rw-   0        0        0     3172 2023-06-26 20:58:45.000000 mwsqlite-1.2.2/mwsqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-26 20:58:45.000000 mwsqlite-1.2.2/mwsqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 20:58:45.000000 mwsqlite-1.2.2/mwsqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-26 20:58:45.000000 mwsqlite-1.2.2/mwsqlite.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-26 20:58:45.000000 mwsqlite-1.2.2/mwsqlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 20:58:46.079516 mwsqlite-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1666 2023-06-26 20:52:20.000000 mwsqlite-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 11:00:06.830474 mwsqlite-1.2.3/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 mwsqlite-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3172 2023-07-11 11:00:06.831475 mwsqlite-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2075 2022-12-19 15:39:05.000000 mwsqlite-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 11:00:06.805468 mwsqlite-1.2.3/mwsqlite/
+-rw-rw-rw-   0        0        0      186 2022-12-19 10:39:07.000000 mwsqlite-1.2.3/mwsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1979 2023-07-11 10:59:01.000000 mwsqlite-1.2.3/mwsqlite/_types.py
+-rw-rw-rw-   0        0        0    14773 2023-06-26 20:56:30.000000 mwsqlite-1.2.3/mwsqlite/mw_sql.py
+-rw-rw-rw-   0        0        0     3388 2022-12-23 15:06:08.000000 mwsqlite-1.2.3/mwsqlite/sql_compile.py
+-rw-rw-rw-   0        0        0      551 2022-12-23 17:48:26.000000 mwsqlite-1.2.3/mwsqlite/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 11:00:06.829473 mwsqlite-1.2.3/mwsqlite.egg-info/
+-rw-rw-rw-   0        0        0     3172 2023-07-11 11:00:06.000000 mwsqlite-1.2.3/mwsqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-11 11:00:06.000000 mwsqlite-1.2.3/mwsqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 11:00:06.000000 mwsqlite-1.2.3/mwsqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 11:00:06.000000 mwsqlite-1.2.3/mwsqlite.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-11 11:00:06.000000 mwsqlite-1.2.3/mwsqlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 11:00:06.832717 mwsqlite-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1666 2023-07-11 10:56:50.000000 mwsqlite-1.2.3/setup.py
```

### Comparing `mwsqlite-1.2.2/LICENSE` & `mwsqlite-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.2/PKG-INFO` & `mwsqlite-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mwsqlite
-Version: 1.2.2
+Version: 1.2.3
 Summary: Simply python library for interact with (EOSIO) WAX blockchain
 Home-page: https://github.com/makarworld/mwsqlite.git
-Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.2.zip
+Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.3.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mwsqlite-1.2.2/README.md` & `mwsqlite-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.2/mwsqlite/_types.py` & `mwsqlite-1.2.3/mwsqlite/_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -39,14 +39,29 @@
         return self.__dict__.__repr__()
     
     def __str__(self):
         return self.__dict__.__str__()
     
     def dict(self):
         return self.__dict__ 
+    
+    def to_dict(self):
+        _dict = {}
+        for k, v in self.__dict__.items():
+            if isinstance(v, Struct):
+                _dict[k] = v.to_dict()
+
+            if isinstance(v, list):
+                for i in range(len(v)):
+                    if isinstance(v[i], Struct):
+                        _dict[k].append(v[i].to_dict())
+                    else:
+                        _dict[k].append(v[i])
+        return _dict
+        
 
     def __getattr__(self, item):
         return None
 
     def __getitem__(self, item):
         return self.get(item)
```

### Comparing `mwsqlite-1.2.2/mwsqlite/mw_sql.py` & `mwsqlite-1.2.3/mwsqlite/mw_sql.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.2/mwsqlite/sql_compile.py` & `mwsqlite-1.2.3/mwsqlite/sql_compile.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.2/mwsqlite/utils.py` & `mwsqlite-1.2.3/mwsqlite/utils.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.2.2/mwsqlite.egg-info/PKG-INFO` & `mwsqlite-1.2.3/mwsqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mwsqlite
-Version: 1.2.2
+Version: 1.2.3
 Summary: Simply python library for interact with (EOSIO) WAX blockchain
 Home-page: https://github.com/makarworld/mwsqlite.git
-Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.2.zip
+Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.3.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mwsqlite-1.2.2/setup.py` & `mwsqlite-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.2.2'
+version = '1.2.3'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="mwsqlite",
     version=version,
```

