# Comparing `tmp/audit_logging_pepsico-0.0.9.tar.gz` & `tmp/audit_logging_pepsico-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audit_logging_pepsico-0.0.9.tar", last modified: Fri Jun  9 13:25:48 2023, max compression
+gzip compressed data, was "audit_logging_pepsico-1.0.0.tar", last modified: Tue Jul 11 12:15:31 2023, max compression
```

## Comparing `audit_logging_pepsico-0.0.9.tar` & `audit_logging_pepsico-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:25:48.662654 audit_logging_pepsico-0.0.9/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-0.0.9/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 13:25:48.661945 audit_logging_pepsico-0.0.9/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-0.0.9/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:25:48.657523 audit_logging_pepsico-0.0.9/audit_logging_pepsico/
--rw-rw-r--   0 jatintalati   (501) staff       (20)     2059 2023-05-21 21:09:26.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico/Kafka_log.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico/audit.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico/audit_config.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico/constants.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     5368 2023-06-09 13:25:10.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico/kafka_utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-06-09 13:25:48.661061 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-06-09 13:25:48.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-06-09 13:25:48.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-06-09 13:25:48.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       88 2023-06-09 13:25:48.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-06-09 13:25:48.000000 audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      742 2023-06-09 13:25:33.000000 audit_logging_pepsico-0.0.9/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-06-09 13:25:48.663075 audit_logging_pepsico-0.0.9/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 12:15:31.585992 audit_logging_pepsico-1.0.0/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-1.0.0/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-07-11 12:15:31.585702 audit_logging_pepsico-1.0.0/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-1.0.0/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 12:15:31.580128 audit_logging_pepsico-1.0.0/audit_logging_pepsico/
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2059 2023-05-21 21:09:26.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico/Kafka_log.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico/audit.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico/audit_config.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico/constants.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     5368 2023-06-09 13:25:10.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico/kafka_utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 12:15:31.585085 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-07-11 12:15:31.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-07-11 12:15:31.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-07-11 12:15:31.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       35 2023-07-11 12:15:31.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-07-11 12:15:31.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      669 2023-07-11 12:12:54.000000 audit_logging_pepsico-1.0.0/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-07-11 12:15:31.586109 audit_logging_pepsico-1.0.0/setup.cfg
```

### Comparing `audit_logging_pepsico-0.0.9/LICENSE` & `audit_logging_pepsico-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.9/PKG-INFO` & `audit_logging_pepsico-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audit_logging_pepsico
-Version: 0.0.9
+Version: 1.0.0
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `audit_logging_pepsico-0.0.9/README.md` & `audit_logging_pepsico-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.9/audit_logging_pepsico/Kafka_log.py` & `audit_logging_pepsico-1.0.0/audit_logging_pepsico/Kafka_log.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.9/audit_logging_pepsico/audit.py` & `audit_logging_pepsico-1.0.0/audit_logging_pepsico/audit.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.9/audit_logging_pepsico/audit_config.py` & `audit_logging_pepsico-1.0.0/audit_logging_pepsico/audit_config.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.9/audit_logging_pepsico/kafka_utilities.py` & `audit_logging_pepsico-1.0.0/audit_logging_pepsico/kafka_utilities.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.9/audit_logging_pepsico.egg-info/PKG-INFO` & `audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audit-logging-pepsico
-Version: 0.0.9
+Version: 1.0.0
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

