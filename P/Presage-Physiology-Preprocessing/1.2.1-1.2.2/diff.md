# Comparing `tmp/Presage Physiology Preprocessing-1.2.1.tar.gz` & `tmp/Presage Physiology Preprocessing-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Presage Physiology Preprocessing-1.2.1.tar", last modified: Wed Dec 21 13:46:15 2022, max compression
+gzip compressed data, was "Presage Physiology Preprocessing-1.2.2.tar", last modified: Tue Jul 11 16:39:31 2023, max compression
```

## Comparing `Presage Physiology Preprocessing-1.2.1.tar` & `Presage Physiology Preprocessing-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/
--rw-r--r--   0 root         (0) root         (0)     5759 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/Presage_Physiology_Preprocessing.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5759 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/Presage_Physiology_Preprocessing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/Presage_Physiology_Preprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/Presage_Physiology_Preprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/Presage_Physiology_Preprocessing.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/Presage_Physiology_Preprocessing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/Presage_Physiology_Preprocessing.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     4569 2022-12-21 13:44:21.000000 Presage Physiology Preprocessing-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/presage_physiology_preprocessing/
--rw-rw-rw-   0 root         (0) root         (0)      185 2022-12-21 13:44:21.000000 Presage Physiology Preprocessing-1.2.1/presage_physiology_preprocessing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2022-12-21 13:44:21.000000 Presage Physiology Preprocessing-1.2.1/presage_physiology_preprocessing/mediapipefunctions.py
--rw-rw-rw-   0 root         (0) root         (0)    18335 2022-12-21 13:44:21.000000 Presage Physiology Preprocessing-1.2.1/presage_physiology_preprocessing/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-12-21 13:46:14.000000 Presage Physiology Preprocessing-1.2.1/presage_physiology_preprocessing/version.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2022-12-21 13:46:15.000000 Presage Physiology Preprocessing-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1452 2022-12-21 13:44:21.000000 Presage Physiology Preprocessing-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:39:31.211368 Presage Physiology Preprocessing-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)     5759 2023-07-11 16:39:31.211368 Presage Physiology Preprocessing-1.2.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:39:31.207368 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5759 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-07-11 16:37:28.000000 Presage Physiology Preprocessing-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:39:31.211368 Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-11 16:37:28.000000 Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-07-11 16:37:28.000000 Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/mediapipefunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)    18335 2023-07-11 16:37:28.000000 Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-11 16:39:29.000000 Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-11 16:39:31.211368 Presage Physiology Preprocessing-1.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-11 16:37:28.000000 Presage Physiology Preprocessing-1.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Presage Physiology Preprocessing-1.2.1/PKG-INFO` & `Presage Physiology Preprocessing-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Presage Physiology Preprocessing
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python helper package used for preprocessing video before sending it to Presage Technologies Physiology API.
 Home-page: https://physiology.presagetech.com/
 Author: Presage Technologies
 Author-email: support@presagetech.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Presage-Security/presage_physiology_preprocessing/issues
 Description: # presage_physiology_preprocessing
```

### Comparing `Presage Physiology Preprocessing-1.2.1/Presage_Physiology_Preprocessing.egg-info/PKG-INFO` & `Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Presage-Physiology-Preprocessing
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python helper package used for preprocessing video before sending it to Presage Technologies Physiology API.
 Home-page: https://physiology.presagetech.com/
 Author: Presage Technologies
 Author-email: support@presagetech.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Presage-Security/presage_physiology_preprocessing/issues
 Description: # presage_physiology_preprocessing
```

### Comparing `Presage Physiology Preprocessing-1.2.1/Presage_Physiology_Preprocessing.egg-info/SOURCES.txt` & `Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Presage Physiology Preprocessing-1.2.1/README.md` & `Presage Physiology Preprocessing-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `Presage Physiology Preprocessing-1.2.1/presage_physiology_preprocessing/mediapipefunctions.py` & `Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/mediapipefunctions.py`

 * *Files identical despite different names*

### Comparing `Presage Physiology Preprocessing-1.2.1/presage_physiology_preprocessing/preprocessing.py` & `Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `Presage Physiology Preprocessing-1.2.1/setup.py` & `Presage Physiology Preprocessing-1.2.2/setup.py`

 * *Files identical despite different names*

