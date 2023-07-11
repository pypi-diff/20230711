# Comparing `tmp/gladier-tools-0.4.4.tar.gz` & `tmp/gladier-tools-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gladier-tools-0.4.4.tar", last modified: Wed Apr 19 21:17:32 2023, max compression
+gzip compressed data, was "gladier-tools-0.5.0b1.tar", last modified: Tue Jul 11 16:11:29 2023, max compression
```

## Comparing `gladier-tools-0.4.4.tar` & `gladier-tools-0.5.0b1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.239287 gladier-tools-0.4.4/gladier_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.239287 gladier-tools-0.4.4/gladier_tools/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/experimental/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.239287 gladier-tools-0.4.4/gladier_tools/experimental/globus/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/experimental/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/experimental/globus/mkdir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/globus/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/globus/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/posix/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/asymmetric_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/asymmetric_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/https_download_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/shell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/posix/untar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/publish/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/publish/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/publish/publishv2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/tests/posix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_gladier_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_shell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/posix/test_untar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/gladier_tools/tests/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/publish/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/tests/publish/test_publishv2.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/gladier_tools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:17:32.239287 gladier-tools-0.4.4/gladier_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 21:17:32.000000 gladier-tools-0.4.4/gladier_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-19 21:17:32.000000 gladier-tools-0.4.4/gladier_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:17:32.000000 gladier-tools-0.4.4/gladier_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 21:17:32.000000 gladier-tools-0.4.4/gladier_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 21:17:32.000000 gladier-tools-0.4.4/gladier_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 21:17:32.243287 gladier-tools-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-19 21:17:23.000000 gladier-tools-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.694307 gladier-tools-0.5.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-11 16:11:29.694307 gladier-tools-0.5.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.690307 gladier-tools-0.5.0b1/gladier_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.690307 gladier-tools-0.5.0b1/gladier_tools/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/experimental/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.690307 gladier-tools-0.5.0b1/gladier_tools/experimental/globus/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/experimental/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/experimental/globus/mkdir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.690307 gladier-tools-0.5.0b1/gladier_tools/globus/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/globus/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.694307 gladier-tools-0.5.0b1/gladier_tools/posix/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/posix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/posix/asymmetric_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/posix/asymmetric_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/posix/decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/posix/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/posix/https_download_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/posix/shell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/posix/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/posix/untar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.694307 gladier-tools-0.5.0b1/gladier_tools/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/publish/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/publish/publishv2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.694307 gladier-tools-0.5.0b1/gladier_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.694307 gladier-tools-0.5.0b1/gladier_tools/tests/posix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/posix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/posix/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/posix/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_gladier_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_shell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_untar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.694307 gladier-tools-0.5.0b1/gladier_tools/tests/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/publish/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/tests/publish/test_publishv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/gladier_tools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:11:29.690307 gladier-tools-0.5.0b1/gladier_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-11 16:11:29.000000 gladier-tools-0.5.0b1/gladier_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-11 16:11:29.000000 gladier-tools-0.5.0b1/gladier_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:11:29.000000 gladier-tools-0.5.0b1/gladier_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 16:11:29.000000 gladier-tools-0.5.0b1/gladier_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 16:11:29.000000 gladier-tools-0.5.0b1/gladier_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 16:11:29.694307 gladier-tools-0.5.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-11 16:11:20.000000 gladier-tools-0.5.0b1/setup.py
```

### Comparing `gladier-tools-0.4.4/LICENSE` & `gladier-tools-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/PKG-INFO` & `gladier-tools-0.5.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier-tools
-Version: 0.4.4
+Version: 0.5.0b1
 Summary: A set of reusable Gladier Tools
 Home-page: https://github.com/globus-gladier/gladier-tools
 Maintainer: The Gladier Team
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gladier-tools-0.4.4/README.rst` & `gladier-tools-0.5.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/experimental/__init__.py` & `gladier-tools-0.5.0b1/gladier_tools/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/experimental/base.py` & `gladier-tools-0.5.0b1/gladier_tools/experimental/base.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/experimental/globus/mkdir.py` & `gladier-tools-0.5.0b1/gladier_tools/experimental/globus/mkdir.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/globus/transfer.py` & `gladier-tools-0.5.0b1/gladier_tools/globus/transfer.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/posix/asymmetric_decrypt.py` & `gladier-tools-0.5.0b1/gladier_tools/posix/asymmetric_decrypt.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,17 +66,17 @@
     :param asym_decrypt_password: (Optional) If the private file is password
         protected, pass it in through this argument.
     :param output_file: (Optional) Path to the output file which holds the
         decrypted contents.
     :returns output_path: Location of the decrypted file.
     """
 
-    funcx_functions = [asymmetric_decrypt]
+    compute_functions = [asymmetric_decrypt]
     required_input = [
         'private_key_path',
         'asym_decrypt_file',
-        'funcx_endpoint_compute'
+        'compute_endpoint'
     ]
 
     flow_input = {
         'private_key_path': '~/.ssh/id_rsa'
     }
```

### Comparing `gladier-tools-0.4.4/gladier_tools/posix/asymmetric_encrypt.py` & `gladier-tools-0.5.0b1/gladier_tools/posix/asymmetric_encrypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         the RSA public key. Defaults to ~/.ssh/id_rsa.pub
     :param asym_encrypt_file: File which needs to be encrypted.
     :param funcx_endpoint_compute: By default, uses the ``compute``
         funcx endpoint.
     :returns output_path: Location of the encrypted file.
     """
 
-    funcx_functions = [asymmetric_encrypt]
+    compute_functions = [asymmetric_encrypt]
     required_input = [
         'public_key_path',
         'asym_encrypt_file',
-        'funcx_endpoint_compute'
+        'compute_endpoint'
     ]
     flow_input = {
         'public_key_path': '~/.ssh/id_rsa.pub'
     }
```

### Comparing `gladier-tools-0.4.4/gladier_tools/posix/decrypt.py` & `gladier-tools-0.5.0b1/gladier_tools/posix/decrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,13 +56,13 @@
         If not provided, the decrypted file will have the same name as the input
         file, with the last 4 characters truncated(assuming it was a .aes file).
     :param funcx_endpoint_compute: By default, uses the ``compute`` funcx
         endpoint.
     :returns output_path: Location of the decrypted file.
     """
 
-    funcx_functions = [decrypt]
+    compute_functions = [decrypt]
     required_input = [
         'decrypt_input',
         'decrypt_key',
-        'funcx_endpoint_compute'
+        'compute_endpoint'
     ]
```

### Comparing `gladier-tools-0.4.4/gladier_tools/posix/encrypt.py` & `gladier-tools-0.5.0b1/gladier_tools/posix/encrypt.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,13 +50,13 @@
     :param encrypt_key: Symmetric key or "password" which can be used to
         decrypt the encrypted file.
     :param funcx_endpoint_compute: By default, uses the ``compute``
         funcx endpoint.
     :returns output_path: Location of the encrypted file.
     """
 
-    funcx_functions = [encrypt]
+    compute_functions = [encrypt]
     required_input = [
         'encrypt_input',
         'encrypt_key',
-        'funcx_endpoint_compute'
+        'compute_endpoint'
     ]
```

### Comparing `gladier-tools-0.4.4/gladier_tools/posix/https_download_file.py` & `gladier-tools-0.5.0b1/gladier_tools/posix/https_download_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,18 +35,18 @@
         open(full_name , 'wb').write(r.content)
 
     return full_name
 
 @generate_flow_definition
 class HttpsDownloadFile(GladierBaseTool):
 
-    funcx_functions = [https_download_file]
+    compute_functions = [https_download_file]
     flow_input = {
         'headers':'',
         }
     required_input = [
         'server_url',
         'file_name',
         'file_path',
         'headers',
-        'funcx_endpoint_non_compute'
+        'compute_endpoint'
         ]
```

### Comparing `gladier-tools-0.4.4/gladier_tools/posix/shell_cmd.py` & `gladier-tools-0.5.0b1/gladier_tools/posix/shell_cmd.py`

 * *Files 11% similar despite different names*

```diff
@@ -127,9 +127,9 @@
         **kwargs:
         nil:
 
     Returns:
         A tuple containing the return code of the command execution, the string
         of the standard out and standard error (if capture_output is True)
     """
-    funcx_functions = [shell_cmd]
-    required_input = ["args", "funcx_endpoint_compute"]
+    compute_functions = [shell_cmd]
+    required_input = ["args", "compute_endpoint"]
```

### Comparing `gladier-tools-0.4.4/gladier_tools/posix/tar.py` & `gladier-tools-0.5.0b1/gladier_tools/posix/tar.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,12 +31,12 @@
     :param tar_input: Input directory to archive.
     :param tar_output: (optional) output file to save the new archive. Defaults to the original
                        input file with an extension (myfile.tgz) if not given.
     :param funcx_endpoint_compute: By default, uses the ``compute`` funcx endpoint.
     :returns path: The name of the newly created archive.
     """
 
-    funcx_functions = [tar]
+    compute_functions = [tar]
     required_input = [
         'tar_input',
-        'funcx_endpoint_compute',
+        'compute_endpoint',
     ]
```

### Comparing `gladier-tools-0.4.4/gladier_tools/posix/untar.py` & `gladier-tools-0.5.0b1/gladier_tools/posix/untar.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,12 +47,12 @@
                        input file with an extension '.tgz' removed.
     :param funcx_endpoint_compute: By default, uses the ``compute`` funcx endpoint.  # noqa
     :returns path: The output location of the extracted archive
     :raises ValueError: If any files within the tar would extract to a non-relative location
     :raises FileNotFoundError: If the file does not exist.
     """
 
-    funcx_functions = [untar]
+    compute_functions = [untar]
     required_input = [
             'untar_input',
-            'funcx_endpoint_compute',
+            'compute_endpoint',
         ]
```

### Comparing `gladier-tools-0.4.4/gladier_tools/publish/publish.py` & `gladier-tools-0.5.0b1/gladier_tools/publish/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,20 +112,20 @@
     flow_definition = {
         'Comment': 'Publish metadata to Globus Search, with data from the result.',
         'StartAt': 'PublishGatherMetadata',
         'States': {
             'PublishGatherMetadata': {
                 'Comment': 'Say something to start the conversation',
                 'Type': 'Action',
-                'ActionUrl': 'https://compute2.dev.funcx.org/fxap',
+                'ActionUrl': 'https://compute.actions.globus.org',
                 'ExceptionOnActionFailure': False,
                 'Parameters': {
                     'tasks': [{
-                        'endpoint.$': '$.input.funcx_endpoint_non_compute',
-                        'function.$': '$.input.publish_gather_metadata_funcx_id',
+                        'endpoint.$': '$.input.compute_endpoint',
+                        'function.$': '$.input.publish_gather_metadata_function_id',
                         'payload.$': '$.input.pilot',
                     }]
                 },
                 'ResultPath': '$.PublishGatherMetadata',
                 'WaitTime': 60,
                 'Next': 'PublishTransfer',
             },
@@ -149,17 +149,17 @@
                 'End': True
             },
         }
     }
 
     required_input = [
         'pilot',
-        'funcx_endpoint_non_compute',
+        'compute_endpoint',
     ]
 
     flow_input = {
 
     }
 
-    funcx_functions = [
+    compute_functions = [
         publish_gather_metadata,
     ]
```

### Comparing `gladier-tools-0.4.4/gladier_tools/publish/publishv2.py` & `gladier-tools-0.5.0b1/gladier_tools/publish/publishv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,21 +311,21 @@
     flow_definition = {
         "Comment": "Publish metadata to Globus Search, with data from the result.",
         "StartAt": "Publishv2GatherMetadata",
         "States": {
             "Publishv2GatherMetadata": {
                 "Comment": "Generate search metadata and a transfer document",
                 "Type": "Action",
-                "ActionUrl": "https://compute2.dev.funcx.org/fxap",
+                "ActionUrl": "https://compute.actions.globus.org",
                 "ExceptionOnActionFailure": True,
                 "Parameters": {
                     "tasks": [
                         {
-                            "endpoint.$": "$.input.funcx_endpoint_non_compute",
-                            "function.$": "$.input.publishv2_gather_metadata_funcx_id",
+                            "endpoint.$": "$.input.compute_endpoint",
+                            "function.$": "$.input.publishv2_gather_metadata_function_id",
                             "payload.$": "$.input.publishv2",
                         }
                     ]
                 },
                 "ResultPath": "$.Publishv2GatherMetadata",
                 "WaitTime": 600,
                 "Next": "Publishv2ChoiceTransfer",
@@ -404,15 +404,15 @@
                 "End": True,
             },
         },
     }
 
     required_input = [
         "publishv2",
-        "funcx_endpoint_non_compute",
+        "compute_endpoint",
     ]
 
     flow_input = {}
 
-    funcx_functions = [
+    compute_functions = [
         publishv2_gather_metadata,
     ]
```

### Comparing `gladier-tools-0.4.4/gladier_tools/tests/posix/test_decrypt.py` & `gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_decrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/tests/posix/test_encrypt.py` & `gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/tests/posix/test_gladier_tools.py` & `gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_gladier_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
 from gladier import GladierBaseClient, generate_flow_definition
 
+from .mocks import MOCK_LOGIN_MANAGER
+
 GLADIER_TOOLS = [
     # Posix
     'gladier_tools.posix.Tar',
     'gladier_tools.posix.UnTar',
     'gladier_tools.posix.Encrypt',
     'gladier_tools.posix.Decrypt',
     'gladier_tools.posix.AsymmetricEncrypt',
@@ -22,8 +24,8 @@
 @pytest.mark.parametrize('import_string', GLADIER_TOOLS)
 def test_use_gladier_tool(import_string):
 
     @generate_flow_definition
     class MyGladierClass(GladierBaseClient):
         gladier_tools = [import_string]
 
-    MyGladierClass(auto_login=False)
+    MyGladierClass(login_manager=MOCK_LOGIN_MANAGER)
```

### Comparing `gladier-tools-0.4.4/gladier_tools/tests/posix/test_shell_cmd.py` & `gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_shell_cmd.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/tests/posix/test_tar.py` & `gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_tar.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/tests/posix/test_untar.py` & `gladier-tools-0.5.0b1/gladier_tools/tests/posix/test_untar.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/tests/publish/test_publish.py` & `gladier-tools-0.5.0b1/gladier_tools/tests/publish/test_publish.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools/tests/publish/test_publishv2.py` & `gladier-tools-0.5.0b1/gladier_tools/tests/publish/test_publishv2.py`

 * *Files identical despite different names*

### Comparing `gladier-tools-0.4.4/gladier_tools.egg-info/PKG-INFO` & `gladier-tools-0.5.0b1/gladier_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier-tools
-Version: 0.4.4
+Version: 0.5.0b1
 Summary: A set of reusable Gladier Tools
 Home-page: https://github.com/globus-gladier/gladier-tools
 Maintainer: The Gladier Team
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gladier-tools-0.4.4/gladier_tools.egg-info/SOURCES.txt` & `gladier-tools-0.5.0b1/gladier_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 gladier_tools/posix/untar.py
 gladier_tools/publish/__init__.py
 gladier_tools/publish/publish.py
 gladier_tools/publish/publishv2.py
 gladier_tools/tests/__init__.py
 gladier_tools/tests/posix/__init__.py
 gladier_tools/tests/posix/conftest.py
+gladier_tools/tests/posix/mocks.py
 gladier_tools/tests/posix/test_decrypt.py
 gladier_tools/tests/posix/test_encrypt.py
 gladier_tools/tests/posix/test_gladier_tools.py
 gladier_tools/tests/posix/test_shell_cmd.py
 gladier_tools/tests/posix/test_tar.py
 gladier_tools/tests/posix/test_untar.py
 gladier_tools/tests/publish/__init__.py
```

### Comparing `gladier-tools-0.4.4/setup.py` & `gladier-tools-0.5.0b1/setup.py`

 * *Files identical despite different names*

