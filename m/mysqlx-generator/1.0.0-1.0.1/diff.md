# Comparing `tmp/mysqlx-generator-1.0.0.tar.gz` & `tmp/mysqlx-generator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-generator-1.0.0.tar", last modified: Tue Jul 11 02:28:15 2023, max compression
+gzip compressed data, was "dist\mysqlx-generator-1.0.1.tar", last modified: Tue Jul 11 02:30:54 2023, max compression
```

## Comparing `mysqlx-generator-1.0.0.tar` & `mysqlx-generator-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 02:28:15.000000 mysqlx-generator-1.0.0/
--rw-rw-rw-   0        0        0     1189 2023-07-11 02:28:12.000000 mysqlx-generator-1.0.0/generator_setup.py
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-generator-1.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-11 02:28:15.000000 mysqlx-generator-1.0.0/mysqlx_generator/
--rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.0.0/mysqlx_generator/generator.tpl
--rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.0.0/mysqlx_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 02:28:15.000000 mysqlx-generator-1.0.0/mysqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-11 02:28:15.000000 mysqlx-generator-1.0.0/mysqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-11 02:26:11.000000 mysqlx-generator-1.0.0/mysqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2828 2023-07-11 02:28:15.000000 mysqlx-generator-1.0.0/mysqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       59 2023-07-11 02:28:15.000000 mysqlx-generator-1.0.0/mysqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      344 2023-07-11 02:28:15.000000 mysqlx-generator-1.0.0/mysqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-07-11 02:28:15.000000 mysqlx-generator-1.0.0/mysqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2828 2023-07-11 02:28:15.000000 mysqlx-generator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-generator-1.0.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-11 02:28:15.000000 mysqlx-generator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1234 2023-07-10 14:23:24.000000 mysqlx-generator-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:30:54.000000 mysqlx-generator-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-generator-1.0.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-11 02:30:54.000000 mysqlx-generator-1.0.1/mysqlx_generator/
+-rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.0.1/mysqlx_generator/generator.tpl
+-rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.0.1/mysqlx_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:30:54.000000 mysqlx-generator-1.0.1/mysqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-11 02:30:54.000000 mysqlx-generator-1.0.1/mysqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 02:26:11.000000 mysqlx-generator-1.0.1/mysqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2828 2023-07-11 02:30:54.000000 mysqlx-generator-1.0.1/mysqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2023-07-11 02:30:54.000000 mysqlx-generator-1.0.1/mysqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      325 2023-07-11 02:30:54.000000 mysqlx-generator-1.0.1/mysqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-07-11 02:30:54.000000 mysqlx-generator-1.0.1/mysqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2828 2023-07-11 02:30:54.000000 mysqlx-generator-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-generator-1.0.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-11 02:30:54.000000 mysqlx-generator-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1189 2023-07-11 02:30:42.000000 mysqlx-generator-1.0.1/setup.py
```

### Comparing `mysqlx-generator-1.0.0/generator_setup.py` & `mysqlx-generator-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysqlx>=1.3.0',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.0.0',
+    version='1.0.1',
     url='https://gitee.com/summry/mysqlx/generator.md',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['MySQL', 'mysqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `mysqlx-generator-1.0.0/LICENSE` & `mysqlx-generator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.0.0/mysqlx_generator/generator.tpl` & `mysqlx-generator-1.0.1/mysqlx_generator/generator.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.0.0/mysqlx_generator/__init__.py` & `mysqlx-generator-1.0.1/mysqlx_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.0.0/mysqlx_generator.egg-info/PKG-INFO` & `mysqlx-generator-1.0.1/mysqlx_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.0.0
+Version: 1.0.1
 Summary: mysqlx-generator is a model code generator from db tables for mysqlx.
 Home-page: https://gitee.com/summry/mysqlx/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-generator-1.0.0/PKG-INFO` & `mysqlx-generator-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.0.0
+Version: 1.0.1
 Summary: mysqlx-generator is a model code generator from db tables for mysqlx.
 Home-page: https://gitee.com/summry/mysqlx/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-generator-1.0.0/README.rst` & `mysqlx-generator-1.0.1/README.rst`

 * *Files identical despite different names*

