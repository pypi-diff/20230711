# Comparing `tmp/mymulti_key_dict-0.13.tar.gz` & `tmp/mymulti_key_dict-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mymulti_key_dict-0.13.tar", last modified: Sat Jul  8 20:07:55 2023, max compression
+gzip compressed data, was "mymulti_key_dict-0.14.tar", last modified: Mon Jul 10 20:31:41 2023, max compression
```

## Comparing `mymulti_key_dict-0.13.tar` & `mymulti_key_dict-0.14.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 20:07:55.595488 mymulti_key_dict-0.13/
--rw-rw-rw-   0        0        0     1148 2023-07-08 20:07:49.000000 mymulti_key_dict-0.13/LICENSE.rst
--rw-rw-rw-   0        0        0      119 2023-07-08 20:07:48.000000 mymulti_key_dict-0.13/MANIFEST.in
--rw-rw-rw-   0        0        0     4641 2023-07-08 20:07:55.595488 mymulti_key_dict-0.13/PKG-INFO
--rw-rw-rw-   0        0        0     3952 2023-07-06 02:45:45.000000 mymulti_key_dict-0.13/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 20:07:55.590502 mymulti_key_dict-0.13/mymulti_key_dict/
--rw-rw-rw-   0        0        0     3952 2023-07-06 02:45:45.000000 mymulti_key_dict-0.13/mymulti_key_dict/README.MD
--rw-rw-rw-   0        0        0     5896 2023-07-08 20:05:58.000000 mymulti_key_dict-0.13/mymulti_key_dict/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-08 20:07:54.000000 mymulti_key_dict-0.13/mymulti_key_dict/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-07-08 20:07:54.000000 mymulti_key_dict-0.13/mymulti_key_dict/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-08 20:07:55.594491 mymulti_key_dict-0.13/mymulti_key_dict.egg-info/
--rw-rw-rw-   0        0        0     4641 2023-07-08 20:07:55.000000 mymulti_key_dict-0.13/mymulti_key_dict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-07-08 20:07:55.000000 mymulti_key_dict-0.13/mymulti_key_dict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 20:07:55.000000 mymulti_key_dict-0.13/mymulti_key_dict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 20:07:55.000000 mymulti_key_dict-0.13/mymulti_key_dict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-08 20:07:55.596486 mymulti_key_dict-0.13/setup.cfg
--rw-rw-rw-   0        0        0     1325 2023-07-08 20:07:54.000000 mymulti_key_dict-0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:31:41.238138 mymulti_key_dict-0.14/
+-rw-rw-rw-   0        0        0     1148 2023-07-10 20:31:31.000000 mymulti_key_dict-0.14/LICENSE.rst
+-rw-rw-rw-   0        0        0      119 2023-07-10 20:31:29.000000 mymulti_key_dict-0.14/MANIFEST.in
+-rw-rw-rw-   0        0        0     4637 2023-07-10 20:31:41.238138 mymulti_key_dict-0.14/PKG-INFO
+-rw-rw-rw-   0        0        0     3948 2023-07-10 20:31:05.000000 mymulti_key_dict-0.14/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 20:31:41.235146 mymulti_key_dict-0.14/mymulti_key_dict/
+-rw-rw-rw-   0        0        0     3948 2023-07-10 20:31:05.000000 mymulti_key_dict-0.14/mymulti_key_dict/README.MD
+-rw-rw-rw-   0        0        0     3634 2023-07-10 20:25:19.000000 mymulti_key_dict-0.14/mymulti_key_dict/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 20:31:40.000000 mymulti_key_dict-0.14/mymulti_key_dict/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-07-10 20:31:40.000000 mymulti_key_dict-0.14/mymulti_key_dict/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-10 20:31:41.238138 mymulti_key_dict-0.14/mymulti_key_dict.egg-info/
+-rw-rw-rw-   0        0        0     4637 2023-07-10 20:31:40.000000 mymulti_key_dict-0.14/mymulti_key_dict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-07-10 20:31:41.000000 mymulti_key_dict-0.14/mymulti_key_dict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 20:31:40.000000 mymulti_key_dict-0.14/mymulti_key_dict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-10 20:31:40.000000 mymulti_key_dict-0.14/mymulti_key_dict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-10 20:31:41.239135 mymulti_key_dict-0.14/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2023-07-10 20:31:40.000000 mymulti_key_dict-0.14/setup.py
```

### Comparing `mymulti_key_dict-0.13/LICENSE.rst` & `mymulti_key_dict-0.14/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mymulti_key_dict-0.13/PKG-INFO` & `mymulti_key_dict-0.14/mymulti_key_dict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mymulti_key_dict
-Version: 0.13
+Name: mymulti-key-dict
+Version: 0.14
 Summary: Access nested dict elements as d[[1,2,3]] instead of d[1][2][3] - compatible with dict() - no requirements
 Home-page: https://github.com/hansalemaos/mymulti_key_dict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nested,dicts
 Classifier: Development Status :: 4 - Beta
@@ -37,15 +37,15 @@
 
 Furthermore, the MultiKeyDict class provides methods for converting the nested dictionary to 
 a normal dictionary, making a deep copy of the dictionary, retrieving items, keys, and values, 
 updating the dictionary with another dictionary, clearing the dictionary, and more. 
 These methods make it convenient to perform common dictionary operations 
 while preserving the nested structure.
 
-By extending the UserDict class, the MultiKeyDict class inherits the basic dictionary functionality 
+By extending the dict class, the MultiKeyDict class inherits the basic dictionary functionality 
 and adds the ability to handle nested keys. 
 It also overrides certain methods, such as **\_\_getitem\_\_**, **\_\_setitem\_\_**, **\_\_delitem\_\_**, and others, 
 to enable the list key functionality and provide the expected behavior for accessing 
 and modifying nested elements.
 
 
 ```python
```

### Comparing `mymulti_key_dict-0.13/README.md` & `mymulti_key_dict-0.14/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 Furthermore, the MultiKeyDict class provides methods for converting the nested dictionary to 
 a normal dictionary, making a deep copy of the dictionary, retrieving items, keys, and values, 
 updating the dictionary with another dictionary, clearing the dictionary, and more. 
 These methods make it convenient to perform common dictionary operations 
 while preserving the nested structure.
 
-By extending the UserDict class, the MultiKeyDict class inherits the basic dictionary functionality 
+By extending the dict class, the MultiKeyDict class inherits the basic dictionary functionality 
 and adds the ability to handle nested keys. 
 It also overrides certain methods, such as **\_\_getitem\_\_**, **\_\_setitem\_\_**, **\_\_delitem\_\_**, and others, 
 to enable the list key functionality and provide the expected behavior for accessing 
 and modifying nested elements.
 
 
 ```python
```

### Comparing `mymulti_key_dict-0.13/mymulti_key_dict/README.MD` & `mymulti_key_dict-0.14/mymulti_key_dict/README.MD`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 Furthermore, the MultiKeyDict class provides methods for converting the nested dictionary to 
 a normal dictionary, making a deep copy of the dictionary, retrieving items, keys, and values, 
 updating the dictionary with another dictionary, clearing the dictionary, and more. 
 These methods make it convenient to perform common dictionary operations 
 while preserving the nested structure.
 
-By extending the UserDict class, the MultiKeyDict class inherits the basic dictionary functionality 
+By extending the dict class, the MultiKeyDict class inherits the basic dictionary functionality 
 and adds the ability to handle nested keys. 
 It also overrides certain methods, such as **\_\_getitem\_\_**, **\_\_setitem\_\_**, **\_\_delitem\_\_**, and others, 
 to enable the list key functionality and provide the expected behavior for accessing 
 and modifying nested elements.
 
 
 ```python
```

### Comparing `mymulti_key_dict-0.13/mymulti_key_dict.egg-info/PKG-INFO` & `mymulti_key_dict-0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mymulti-key-dict
-Version: 0.13
+Name: mymulti_key_dict
+Version: 0.14
 Summary: Access nested dict elements as d[[1,2,3]] instead of d[1][2][3] - compatible with dict() - no requirements
 Home-page: https://github.com/hansalemaos/mymulti_key_dict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nested,dicts
 Classifier: Development Status :: 4 - Beta
@@ -37,15 +37,15 @@
 
 Furthermore, the MultiKeyDict class provides methods for converting the nested dictionary to 
 a normal dictionary, making a deep copy of the dictionary, retrieving items, keys, and values, 
 updating the dictionary with another dictionary, clearing the dictionary, and more. 
 These methods make it convenient to perform common dictionary operations 
 while preserving the nested structure.
 
-By extending the UserDict class, the MultiKeyDict class inherits the basic dictionary functionality 
+By extending the dict class, the MultiKeyDict class inherits the basic dictionary functionality 
 and adds the ability to handle nested keys. 
 It also overrides certain methods, such as **\_\_getitem\_\_**, **\_\_setitem\_\_**, **\_\_delitem\_\_**, and others, 
 to enable the list key functionality and provide the expected behavior for accessing 
 and modifying nested elements.
 
 
 ```python
```

### Comparing `mymulti_key_dict-0.13/setup.py` & `mymulti_key_dict-0.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.13'''
+VERSION = '''0.14'''
 DESCRIPTION = '''Access nested dict elements as d[[1,2,3]] instead of d[1][2][3] - compatible with dict() - no requirements'''
 
 # Setting up
 setup(
     name="mymulti_key_dict",
     version=VERSION,
     license='MIT',
```

