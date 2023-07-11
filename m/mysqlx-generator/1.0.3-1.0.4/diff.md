# Comparing `tmp/mysqlx-generator-1.0.3.tar.gz` & `tmp/mysqlx-generator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-generator-1.0.3.tar", last modified: Tue Jul 11 03:36:14 2023, max compression
+gzip compressed data, was "dist\mysqlx-generator-1.0.4.tar", last modified: Tue Jul 11 05:40:10 2023, max compression
```

## Comparing `mysqlx-generator-1.0.3.tar` & `mysqlx-generator-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-generator-1.0.3/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator/
--rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.0.3/mysqlx_generator/generator.tpl
--rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.0.3/mysqlx_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-11 02:26:11.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2805 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       59 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      325 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/mysqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2805 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2322 2023-07-11 03:27:01.000000 mysqlx-generator-1.0.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-11 03:36:14.000000 mysqlx-generator-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1186 2023-07-11 03:36:04.000000 mysqlx-generator-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 05:40:10.000000 mysqlx-generator-1.0.4/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-generator-1.0.4/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-11 05:40:10.000000 mysqlx-generator-1.0.4/mysqlx_generator/
+-rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.0.4/mysqlx_generator/generator.tpl
+-rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.0.4/mysqlx_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 05:40:10.000000 mysqlx-generator-1.0.4/mysqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-11 05:40:10.000000 mysqlx-generator-1.0.4/mysqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 02:26:11.000000 mysqlx-generator-1.0.4/mysqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2812 2023-07-11 05:40:10.000000 mysqlx-generator-1.0.4/mysqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-07-11 05:40:10.000000 mysqlx-generator-1.0.4/mysqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      325 2023-07-11 05:40:10.000000 mysqlx-generator-1.0.4/mysqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-07-11 05:40:10.000000 mysqlx-generator-1.0.4/mysqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2812 2023-07-11 05:40:10.000000 mysqlx-generator-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2317 2023-07-11 05:28:55.000000 mysqlx-generator-1.0.4/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-11 05:40:10.000000 mysqlx-generator-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1200 2023-07-11 05:39:47.000000 mysqlx-generator-1.0.4/setup.py
```

### Comparing `mysqlx-generator-1.0.3/LICENSE` & `mysqlx-generator-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.0.3/mysqlx_generator/generator.tpl` & `mysqlx-generator-1.0.4/mysqlx_generator/generator.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.0.3/mysqlx_generator/__init__.py` & `mysqlx-generator-1.0.4/mysqlx_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.0.3/mysqlx_generator.egg-info/PKG-INFO` & `mysqlx-generator-1.0.4/mysqlx_generator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.0.3
+Version: 1.0.4
 Summary: mysqlx-generator is a model code generator from db tables for mysqlx.
-Home-page: https://gitee.com/summry/mysqlx/generator.md
+Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
@@ -29,15 +29,15 @@
 
    if __name__ == '__main__':
        coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
        # you can generate one table
        coder.generate_with_tables(tables='user', path='models.py')
        # you can generate many tables
        coder.generate_with_tables(tables=['user', 'person'], path='models.py')
-       # you can generate all tables for given schema. if you not given schema, default current schema
+       # you can generate all tables for given schema. default current schema if not given schema
        coder.generate_with_schema(schema='test', path='models.py')
 
 If you run last code, then generate a file ‘models.py’ in current
 directory like follow:
 
 .. code:: python
```

### Comparing `mysqlx-generator-1.0.3/PKG-INFO` & `mysqlx-generator-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.0.3
+Version: 1.0.4
 Summary: mysqlx-generator is a model code generator from db tables for mysqlx.
-Home-page: https://gitee.com/summry/mysqlx/generator.md
+Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
@@ -29,15 +29,15 @@
 
    if __name__ == '__main__':
        coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
        # you can generate one table
        coder.generate_with_tables(tables='user', path='models.py')
        # you can generate many tables
        coder.generate_with_tables(tables=['user', 'person'], path='models.py')
-       # you can generate all tables for given schema. if you not given schema, default current schema
+       # you can generate all tables for given schema. default current schema if not given schema
        coder.generate_with_schema(schema='test', path='models.py')
 
 If you run last code, then generate a file ‘models.py’ in current
 directory like follow:
 
 .. code:: python
```

### Comparing `mysqlx-generator-1.0.3/README.rst` & `mysqlx-generator-1.0.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
    if __name__ == '__main__':
        coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
        # you can generate one table
        coder.generate_with_tables(tables='user', path='models.py')
        # you can generate many tables
        coder.generate_with_tables(tables=['user', 'person'], path='models.py')
-       # you can generate all tables for given schema. if you not given schema, default current schema
+       # you can generate all tables for given schema. default current schema if not given schema
        coder.generate_with_schema(schema='test', path='models.py')
 
 If you run last code, then generate a file ‘models.py’ in current
 directory like follow:
 
 .. code:: python
```

### Comparing `mysqlx-generator-1.0.3/setup.py` & `mysqlx-generator-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 setup(
     name='mysqlx-generator',
     packages=['mysqlx_generator'],
     description="mysqlx-generator is a model code generator from db tables for mysqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'Jinja2>=3.0.3',
+        'Jinja2>=3.0.0',
         'mysqlx>=1.3.7',
-        'mysql-connector-python>=8.0.20',
+        # 'mysql-connector-python>=8.0.20',
     ],
-    version='1.0.3',
-    url='https://gitee.com/summry/mysqlx/generator.md',
+    version='1.0.4',
+    url='https://gitee.com/summry/mysqlx/blob/master/generator.md',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['MySQL', 'mysqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
```

