# Comparing `tmp/mysqlx-generator-1.0.2.tar.gz` & `tmp/mysqlx-generator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-generator-1.0.2.tar", last modified: Tue Jul 11 03:10:45 2023, max compression
+gzip compressed data, was "dist\mysqlx-generator-1.0.3.tar", last modified: Tue Jul 11 03:36:14 2023, max compression
```

## Comparing `mysqlx-generator-1.0.2.tar` & `mysqlx-generator-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 03:10:45.000000 mysqlx-generator-1.0.2/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-generator-1.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-11 03:10:45.000000 mysqlx-generator-1.0.2/mysqlx_generator/
--rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.0.2/mysqlx_generator/generator.tpl
--rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.0.2/mysqlx_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:10:45.000000 mysqlx-generator-1.0.2/mysqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-11 03:10:45.000000 mysqlx-generator-1.0.2/mysqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-11 02:26:11.000000 mysqlx-generator-1.0.2/mysqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2828 2023-07-11 03:10:45.000000 mysqlx-generator-1.0.2/mysqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       59 2023-07-11 03:10:45.000000 mysqlx-generator-1.0.2/mysqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      325 2023-07-11 03:10:45.000000 mysqlx-generator-1.0.2/mysqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-07-11 03:10:45.000000 mysqlx-generator-1.0.2/mysqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2828 2023-07-11 03:10:45.000000 mysqlx-generator-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2344 2023-07-11 02:18:05.000000 mysqlx-generator-1.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-11 03:10:45.000000 mysqlx-generator-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1186 2023-07-11 03:10:20.000000 mysqlx-generator-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-generator-1.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator/
+-rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.0.3/mysqlx_generator/generator.tpl
+-rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.0.3/mysqlx_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 02:26:11.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2805 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      325 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2805 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2322 2023-07-11 03:27:01.000000 mysqlx-generator-1.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1186 2023-07-11 03:36:04.000000 mysqlx-generator-1.0.3/setup.py
```

### Comparing `mysqlx-generator-1.0.2/LICENSE` & `mysqlx-generator-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.0.2/mysqlx_generator/generator.tpl` & `mysqlx-generator-1.0.3/mysqlx_generator/generator.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.0.2/mysqlx_generator/__init__.py` & `mysqlx-generator-1.0.3/mysqlx_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.0.2/mysqlx_generator.egg-info/PKG-INFO` & `mysqlx-generator-1.0.3/mysqlx_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.0.2
+Version: 1.0.3
 Summary: mysqlx-generator is a model code generator from db tables for mysqlx.
 Home-page: https://gitee.com/summry/mysqlx/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Install
 '''''''
 
 .. code:: shell
 
-   pip install mysqlx
    pip install mysqlx-generator
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```

### Comparing `mysqlx-generator-1.0.2/PKG-INFO` & `mysqlx-generator-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.0.2
+Version: 1.0.3
 Summary: mysqlx-generator is a model code generator from db tables for mysqlx.
 Home-page: https://gitee.com/summry/mysqlx/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Install
 '''''''
 
 .. code:: shell
 
-   pip install mysqlx
    pip install mysqlx-generator
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```

### Comparing `mysqlx-generator-1.0.2/README.rst` & `mysqlx-generator-1.0.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Install
 '''''''
 
 .. code:: shell
 
-   pip install mysqlx
    pip install mysqlx-generator
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```

### Comparing `mysqlx-generator-1.0.2/setup.py` & `mysqlx-generator-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,24 +14,24 @@
     name='mysqlx-generator',
     packages=['mysqlx_generator'],
     description="mysqlx-generator is a model code generator from db tables for mysqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
-        'mysqlx>=1.3.0',
+        'mysqlx>=1.3.7',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.0.2',
+    version='1.0.3',
     url='https://gitee.com/summry/mysqlx/generator.md',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['MySQL', 'mysqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
-    python_requires='>=3.6.0',
+    python_requires='>=3.7.0',
     zip_safe=False
 )
```

