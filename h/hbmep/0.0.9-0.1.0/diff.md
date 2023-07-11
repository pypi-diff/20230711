# Comparing `tmp/hbmep-0.0.9.tar.gz` & `tmp/hbmep-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbmep-0.0.9.tar", last modified: Fri Jul  7 19:56:08 2023, max compression
+gzip compressed data, was "hbmep-0.1.0.tar", last modified: Tue Jul 11 14:29:14 2023, max compression
```

## Comparing `hbmep-0.0.9.tar` & `hbmep-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,29 @@
-drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-07 19:56:08.050421 hbmep-0.0.9/
--rw-rw-r--   0 vishu     (1000) vishu     (1000)     1074 2023-07-07 18:08:45.000000 hbmep-0.0.9/LICENSE
--rw-rw-r--   0 vishu     (1000) vishu     (1000)     1151 2023-07-07 19:56:08.050421 hbmep-0.0.9/PKG-INFO
--rw-rw-r--   0 vishu     (1000) vishu     (1000)       77 2023-07-07 19:55:45.000000 hbmep-0.0.9/README.md
--rw-rw-r--   0 vishu     (1000) vishu     (1000)     1431 2023-07-07 19:55:08.000000 hbmep-0.0.9/pyproject.toml
--rw-rw-r--   0 vishu     (1000) vishu     (1000)       38 2023-07-07 19:56:08.050421 hbmep-0.0.9/setup.cfg
-drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-07 19:56:08.050421 hbmep-0.0.9/src/
-drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-07 19:56:08.050421 hbmep-0.0.9/src/hbmep/
--rw-rw-r--   0 vishu     (1000) vishu     (1000)        0 2023-07-05 16:33:07.000000 hbmep-0.0.9/src/hbmep/__init__.py
--rw-rw-r--   0 vishu     (1000) vishu     (1000)        0 2023-07-07 19:52:36.000000 hbmep-0.0.9/src/hbmep/__main__.py
-drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-07 19:56:08.050421 hbmep-0.0.9/src/hbmep.egg-info/
--rw-rw-r--   0 vishu     (1000) vishu     (1000)     1151 2023-07-07 19:56:08.000000 hbmep-0.0.9/src/hbmep.egg-info/PKG-INFO
--rw-rw-r--   0 vishu     (1000) vishu     (1000)      240 2023-07-07 19:56:08.000000 hbmep-0.0.9/src/hbmep.egg-info/SOURCES.txt
--rw-rw-r--   0 vishu     (1000) vishu     (1000)        1 2023-07-07 19:56:08.000000 hbmep-0.0.9/src/hbmep.egg-info/dependency_links.txt
--rw-rw-r--   0 vishu     (1000) vishu     (1000)      225 2023-07-07 19:56:08.000000 hbmep-0.0.9/src/hbmep.egg-info/requires.txt
--rw-rw-r--   0 vishu     (1000) vishu     (1000)        6 2023-07-07 19:56:08.000000 hbmep-0.0.9/src/hbmep.egg-info/top_level.txt
+drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-11 14:29:14.678804 hbmep-0.1.0/
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)     1074 2023-07-07 18:08:45.000000 hbmep-0.1.0/LICENSE
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)     1450 2023-07-11 14:29:14.678804 hbmep-0.1.0/PKG-INFO
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)      359 2023-07-10 19:03:07.000000 hbmep-0.1.0/README.md
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)     1359 2023-07-11 14:13:03.000000 hbmep-0.1.0/pyproject.toml
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)       38 2023-07-11 14:29:14.678804 hbmep-0.1.0/setup.cfg
+drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-11 14:29:14.678804 hbmep-0.1.0/src/
+drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-11 14:29:14.678804 hbmep-0.1.0/src/hbmep/
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)        0 2023-07-05 16:33:07.000000 hbmep-0.1.0/src/hbmep/__init__.py
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)     1834 2023-07-10 15:56:29.000000 hbmep-0.1.0/src/hbmep/config.py
+drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-11 14:29:14.678804 hbmep-0.1.0/src/hbmep/dataset/
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)       28 2023-07-06 19:46:12.000000 hbmep-0.1.0/src/hbmep/dataset/__init__.py
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)     7396 2023-07-11 13:12:16.000000 hbmep-0.1.0/src/hbmep/dataset/core.py
+drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-11 14:29:14.678804 hbmep-0.1.0/src/hbmep/models/
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)      105 2023-07-10 20:32:33.000000 hbmep-0.1.0/src/hbmep/models/__init__.py
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)    19115 2023-07-10 20:50:40.000000 hbmep-0.1.0/src/hbmep/models/baseline.py
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)     1285 2023-07-11 13:16:26.000000 hbmep-0.1.0/src/hbmep/models/core.py
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)     3887 2023-07-10 19:19:02.000000 hbmep-0.1.0/src/hbmep/models/rectified_logistic.py
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)      482 2023-07-10 19:10:48.000000 hbmep-0.1.0/src/hbmep/models/utils.py
+drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-11 14:29:14.678804 hbmep-0.1.0/src/hbmep/utils/
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)       20 2023-07-05 16:33:07.000000 hbmep-0.1.0/src/hbmep/utils/__init__.py
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)      712 2023-07-10 20:34:29.000000 hbmep-0.1.0/src/hbmep/utils/constants.py
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)     1558 2023-07-07 18:11:23.000000 hbmep-0.1.0/src/hbmep/utils/utils.py
+drwxrwxr-x   0 vishu     (1000) vishu     (1000)        0 2023-07-11 14:29:14.678804 hbmep-0.1.0/src/hbmep.egg-info/
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)     1450 2023-07-11 14:29:14.000000 hbmep-0.1.0/src/hbmep.egg-info/PKG-INFO
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)      524 2023-07-11 14:29:14.000000 hbmep-0.1.0/src/hbmep.egg-info/SOURCES.txt
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)        1 2023-07-11 14:29:14.000000 hbmep-0.1.0/src/hbmep.egg-info/dependency_links.txt
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)      156 2023-07-11 14:29:14.000000 hbmep-0.1.0/src/hbmep.egg-info/requires.txt
+-rw-rw-r--   0 vishu     (1000) vishu     (1000)        6 2023-07-11 14:29:14.000000 hbmep-0.1.0/src/hbmep.egg-info/top_level.txt
```

### Comparing `hbmep-0.0.9/LICENSE` & `hbmep-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hbmep-0.0.9/pyproject.toml` & `hbmep-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hbmep"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
     { name="Vishweshwar Tyagi, James R. McIntosh", email="vt2353@cumc.columbia.edu" }
 ]
 description = "Package for hierarchical Bayesian modeling of Motor Evoked Potential (MEP) size"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -26,24 +26,23 @@
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: MacOS"
 ]
 dependencies = [
     "numpy==1.24.2",
     "pandas==2.0.2",
-    "fastparquet==2023.2.0",
     "scikit-learn==1.2.1",
     "jax[cpu]==0.4.11",
-    "flax==0.6.11",
     "numpyro[cpu]==0.12.1",
-    "h5py==3.8.0",
-    "mat73==0.60",
     "arviz==0.15.1",
-    "graphviz==0.20.1",
     "matplotlib==3.7.0",
-    "seaborn==0.12.2",
+    "seaborn==0.12.2"
+]
+
+[project.optional-dependencies]
+dev = [
     "jupyter==1.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hbmep/hbmep"
 "Bug Tracker" = "https://github.com/hbmep/hbmep/issues"
```

