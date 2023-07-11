# Comparing `tmp/qiskit_hangyul-0.2.0.tar.gz` & `tmp/qiskit_hangyul-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_hangyul-0.2.0.tar", last modified: Tue Jul 11 10:14:36 2023, max compression
+gzip compressed data, was "qiskit_hangyul-0.3.0.tar", last modified: Tue Jul 11 10:18:13 2023, max compression
```

## Comparing `qiskit_hangyul-0.2.0.tar` & `qiskit_hangyul-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-11 10:14:36.900600 qiskit_hangyul-0.2.0/
--rw-r--r--   0 hangyulson   (501) staff       (20)      334 2023-07-11 10:14:36.900684 qiskit_hangyul-0.2.0/PKG-INFO
--rw-r--r--   0 hangyulson   (501) staff       (20)       26 2023-04-08 21:37:34.000000 qiskit_hangyul-0.2.0/README.md
-drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-11 10:14:36.899693 qiskit_hangyul-0.2.0/qiskit_hangyul.egg-info/
--rw-r--r--   0 hangyulson   (501) staff       (20)      334 2023-07-11 10:14:36.000000 qiskit_hangyul-0.2.0/qiskit_hangyul.egg-info/PKG-INFO
--rw-r--r--   0 hangyulson   (501) staff       (20)      259 2023-07-11 10:14:36.000000 qiskit_hangyul-0.2.0/qiskit_hangyul.egg-info/SOURCES.txt
--rw-r--r--   0 hangyulson   (501) staff       (20)        1 2023-07-11 10:14:36.000000 qiskit_hangyul-0.2.0/qiskit_hangyul.egg-info/dependency_links.txt
--rw-r--r--   0 hangyulson   (501) staff       (20)       18 2023-07-11 10:14:36.000000 qiskit_hangyul-0.2.0/qiskit_hangyul.egg-info/requires.txt
--rw-r--r--   0 hangyulson   (501) staff       (20)        9 2023-07-11 10:14:36.000000 qiskit_hangyul-0.2.0/qiskit_hangyul.egg-info/top_level.txt
-drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-11 10:14:36.900267 qiskit_hangyul-0.2.0/quantier/
--rw-r--r--   0 hangyulson   (501) staff       (20)       54 2023-07-11 10:04:05.000000 qiskit_hangyul-0.2.0/quantier/__init__.py
--rw-r--r--   0 hangyulson   (501) staff       (20)     4181 2023-07-11 09:43:02.000000 qiskit_hangyul-0.2.0/quantier/quantier.py
--rw-r--r--   0 hangyulson   (501) staff       (20)       38 2023-07-11 10:14:36.900983 qiskit_hangyul-0.2.0/setup.cfg
--rw-r--r--   0 hangyulson   (501) staff       (20)      660 2023-07-11 10:14:23.000000 qiskit_hangyul-0.2.0/setup.py
+drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-11 10:18:13.361948 qiskit_hangyul-0.3.0/
+-rw-r--r--   0 hangyulson   (501) staff       (20)      334 2023-07-11 10:18:13.362034 qiskit_hangyul-0.3.0/PKG-INFO
+-rw-r--r--   0 hangyulson   (501) staff       (20)       26 2023-04-08 21:37:34.000000 qiskit_hangyul-0.3.0/README.md
+drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-11 10:18:13.361144 qiskit_hangyul-0.3.0/qiskit_hangyul.egg-info/
+-rw-r--r--   0 hangyulson   (501) staff       (20)      334 2023-07-11 10:18:13.000000 qiskit_hangyul-0.3.0/qiskit_hangyul.egg-info/PKG-INFO
+-rw-r--r--   0 hangyulson   (501) staff       (20)      259 2023-07-11 10:18:13.000000 qiskit_hangyul-0.3.0/qiskit_hangyul.egg-info/SOURCES.txt
+-rw-r--r--   0 hangyulson   (501) staff       (20)        1 2023-07-11 10:18:13.000000 qiskit_hangyul-0.3.0/qiskit_hangyul.egg-info/dependency_links.txt
+-rw-r--r--   0 hangyulson   (501) staff       (20)       18 2023-07-11 10:18:13.000000 qiskit_hangyul-0.3.0/qiskit_hangyul.egg-info/requires.txt
+-rw-r--r--   0 hangyulson   (501) staff       (20)        9 2023-07-11 10:18:13.000000 qiskit_hangyul-0.3.0/qiskit_hangyul.egg-info/top_level.txt
+drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-11 10:18:13.361647 qiskit_hangyul-0.3.0/quantier/
+-rw-r--r--   0 hangyulson   (501) staff       (20)       54 2023-07-11 10:04:05.000000 qiskit_hangyul-0.3.0/quantier/__init__.py
+-rw-r--r--   0 hangyulson   (501) staff       (20)     4149 2023-07-11 10:17:22.000000 qiskit_hangyul-0.3.0/quantier/quantier.py
+-rw-r--r--   0 hangyulson   (501) staff       (20)       38 2023-07-11 10:18:13.362332 qiskit_hangyul-0.3.0/setup.cfg
+-rw-r--r--   0 hangyulson   (501) staff       (20)      660 2023-07-11 10:17:33.000000 qiskit_hangyul-0.3.0/setup.py
```

### Comparing `qiskit_hangyul-0.2.0/quantier/quantier.py` & `qiskit_hangyul-0.3.0/quantier/quantier.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,10 +130,8 @@
         if name is None:
             return [self._simulator, self._backend]
         if name.lower() == 'quantier':
             return [self._backend]
         if name.lower() == 'quantier_simulator':
             return [self._simulator]
         else:
-            return []
-
-provider = QuantierProvider()
+            return []
```

### Comparing `qiskit_hangyul-0.2.0/setup.py` & `qiskit_hangyul-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qiskit_hangyul",
-    version="0.2.0",
+    version="0.3.0",
     description="A quantum provider for Qiskit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["quantier"],
     package_dir={"quantier": "quantier"},
     classifiers=[
         "Programming Language :: Python :: 3",
```

