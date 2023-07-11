# Comparing `tmp/skale-contracts-0.0.1.dev2080802541635176629.tar.gz` & `tmp/skale-contracts-0.0.1.dev2523088075247113431.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skale-contracts-0.0.1.dev2080802541635176629.tar", last modified: Mon Jul 10 15:05:43 2023, max compression
+gzip compressed data, was "skale-contracts-0.0.1.dev2523088075247113431.tar", last modified: Tue Jul 11 14:09:29 2023, max compression
```

## Comparing `skale-contracts-0.0.1.dev2080802541635176629.tar` & `skale-contracts-0.0.1.dev2523088075247113431.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:05:43.369622 skale-contracts-0.0.1.dev2080802541635176629/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-10 15:05:43.369622 skale-contracts-0.0.1.dev2080802541635176629/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 15:05:25.000000 skale-contracts-0.0.1.dev2080802541635176629/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 15:05:25.000000 skale-contracts-0.0.1.dev2080802541635176629/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-10 15:05:43.373623 skale-contracts-0.0.1.dev2080802541635176629/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:05:43.369622 skale-contracts-0.0.1.dev2080802541635176629/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:05:43.369622 skale-contracts-0.0.1.dev2080802541635176629/src/skale_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-10 15:05:43.000000 skale-contracts-0.0.1.dev2080802541635176629/src/skale_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 15:05:43.000000 skale-contracts-0.0.1.dev2080802541635176629/src/skale_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:05:43.000000 skale-contracts-0.0.1.dev2080802541635176629/src/skale_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 15:05:43.000000 skale-contracts-0.0.1.dev2080802541635176629/src/skale_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:05:43.000000 skale-contracts-0.0.1.dev2080802541635176629/src/skale_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 15:05:35.000000 skale-contracts-0.0.1.dev2080802541635176629/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:29.571729 skale-contracts-0.0.1.dev2523088075247113431/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-11 14:09:29.571729 skale-contracts-0.0.1.dev2523088075247113431/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 14:09:11.000000 skale-contracts-0.0.1.dev2523088075247113431/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 14:09:11.000000 skale-contracts-0.0.1.dev2523088075247113431/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-11 14:09:29.575729 skale-contracts-0.0.1.dev2523088075247113431/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:29.567729 skale-contracts-0.0.1.dev2523088075247113431/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:29.571729 skale-contracts-0.0.1.dev2523088075247113431/src/skale_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-11 14:09:29.000000 skale-contracts-0.0.1.dev2523088075247113431/src/skale_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-11 14:09:29.000000 skale-contracts-0.0.1.dev2523088075247113431/src/skale_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:09:29.000000 skale-contracts-0.0.1.dev2523088075247113431/src/skale_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 14:09:29.000000 skale-contracts-0.0.1.dev2523088075247113431/src/skale_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:09:29.000000 skale-contracts-0.0.1.dev2523088075247113431/src/skale_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 14:09:20.000000 skale-contracts-0.0.1.dev2523088075247113431/version.txt
```

### Comparing `skale-contracts-0.0.1.dev2080802541635176629/PKG-INFO` & `skale-contracts-0.0.1.dev2523088075247113431/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 0.0.1.dev2080802541635176629
+Version: 0.0.1.dev2523088075247113431
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `skale-contracts-0.0.1.dev2080802541635176629/setup.cfg` & `skale-contracts-0.0.1.dev2523088075247113431/setup.cfg`

 * *Files identical despite different names*

### Comparing `skale-contracts-0.0.1.dev2080802541635176629/src/skale_contracts.egg-info/PKG-INFO` & `skale-contracts-0.0.1.dev2523088075247113431/src/skale_contracts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 0.0.1.dev2080802541635176629
+Version: 0.0.1.dev2523088075247113431
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

