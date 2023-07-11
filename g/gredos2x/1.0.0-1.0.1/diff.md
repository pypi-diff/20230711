# Comparing `tmp/gredos2x-1.0.0.tar.gz` & `tmp/gredos2x-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gredos2x-1.0.0.tar", last modified: Tue Jul 11 20:59:33 2023, max compression
+gzip compressed data, was "gredos2x-1.0.1.tar", last modified: Tue Jul 11 21:08:52 2023, max compression
```

## Comparing `gredos2x-1.0.0.tar` & `gredos2x-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 grsk      (1000) grsk      (1000)        0 2023-07-11 20:59:33.142847 gredos2x-1.0.0/
--rw-r--r--   0 grsk      (1000) grsk      (1000)      717 2023-07-11 17:46:28.000000 gredos2x-1.0.0/LICENSE.txt
--rw-rw-r--   0 grsk      (1000) grsk      (1000)      681 2023-07-11 20:59:33.142847 gredos2x-1.0.0/PKG-INFO
--rw-r--r--   0 grsk      (1000) grsk      (1000)     5979 2023-07-11 20:42:49.000000 gredos2x-1.0.0/README.md
-drwxrwxr-x   0 grsk      (1000) grsk      (1000)        0 2023-07-11 20:59:33.142847 gredos2x-1.0.0/gredos2x.egg-info/
--rw-r--r--   0 grsk      (1000) grsk      (1000)      681 2023-07-11 20:59:33.000000 gredos2x-1.0.0/gredos2x.egg-info/PKG-INFO
--rw-r--r--   0 grsk      (1000) grsk      (1000)      189 2023-07-11 20:59:33.000000 gredos2x-1.0.0/gredos2x.egg-info/SOURCES.txt
--rw-r--r--   0 grsk      (1000) grsk      (1000)        1 2023-07-11 20:59:33.000000 gredos2x-1.0.0/gredos2x.egg-info/dependency_links.txt
--rw-r--r--   0 grsk      (1000) grsk      (1000)       52 2023-07-11 20:59:33.000000 gredos2x-1.0.0/gredos2x.egg-info/requires.txt
--rw-r--r--   0 grsk      (1000) grsk      (1000)        9 2023-07-11 20:59:33.000000 gredos2x-1.0.0/gredos2x.egg-info/top_level.txt
--rw-rw-r--   0 grsk      (1000) grsk      (1000)       38 2023-07-11 20:59:33.142847 gredos2x-1.0.0/setup.cfg
--rw-r--r--   0 grsk      (1000) grsk      (1000)      982 2023-07-11 20:59:26.000000 gredos2x-1.0.0/setup.py
+drwxrwxr-x   0 grsk      (1000) grsk      (1000)        0 2023-07-11 21:08:52.753442 gredos2x-1.0.1/
+-rw-r--r--   0 grsk      (1000) grsk      (1000)      717 2023-07-11 17:46:28.000000 gredos2x-1.0.1/LICENSE.txt
+-rw-rw-r--   0 grsk      (1000) grsk      (1000)     6701 2023-07-11 21:08:52.753442 gredos2x-1.0.1/PKG-INFO
+-rw-r--r--   0 grsk      (1000) grsk      (1000)     5979 2023-07-11 20:42:49.000000 gredos2x-1.0.1/README.md
+drwxrwxr-x   0 grsk      (1000) grsk      (1000)        0 2023-07-11 21:08:52.753442 gredos2x-1.0.1/gredos2x.egg-info/
+-rw-r--r--   0 grsk      (1000) grsk      (1000)     6701 2023-07-11 21:08:52.000000 gredos2x-1.0.1/gredos2x.egg-info/PKG-INFO
+-rw-r--r--   0 grsk      (1000) grsk      (1000)      189 2023-07-11 21:08:52.000000 gredos2x-1.0.1/gredos2x.egg-info/SOURCES.txt
+-rw-r--r--   0 grsk      (1000) grsk      (1000)        1 2023-07-11 21:08:52.000000 gredos2x-1.0.1/gredos2x.egg-info/dependency_links.txt
+-rw-r--r--   0 grsk      (1000) grsk      (1000)       52 2023-07-11 21:08:52.000000 gredos2x-1.0.1/gredos2x.egg-info/requires.txt
+-rw-r--r--   0 grsk      (1000) grsk      (1000)        9 2023-07-11 21:08:52.000000 gredos2x-1.0.1/gredos2x.egg-info/top_level.txt
+-rw-rw-r--   0 grsk      (1000) grsk      (1000)       38 2023-07-11 21:08:52.753442 gredos2x-1.0.1/setup.cfg
+-rw-r--r--   0 grsk      (1000) grsk      (1000)     1039 2023-07-11 21:07:31.000000 gredos2x-1.0.1/setup.py
```

### Comparing `gredos2x-1.0.0/LICENSE.txt` & `gredos2x-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gredos2x-1.0.0/README.md` & `gredos2x-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gredos2x-1.0.0/setup.py` & `gredos2x-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='gredos2x',
-    version='1.0.0',
+    version='1.0.1',
     author='Gregor Skrt',
     author_email='gregor.skrt@gmail.com',
     description='gredos2x is a format converter for Gredos power system model built by EIMV in 1991. This tool is a set of Python tools, for export to other formats and simulators and supports GIS data conversion from Gredos.',
-    #long_description=long_description, 
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     url='https://github.com/GSkrt/gredos2x',
     py_modules=['gredos2x'],
     install_requires = ['geopandas', 'fiona', 'sqlalchemy','pyodbc','sqlalchemy-access'],
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
```

