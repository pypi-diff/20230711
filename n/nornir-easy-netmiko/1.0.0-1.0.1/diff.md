# Comparing `tmp/nornir_easy_netmiko-1.0.0.tar.gz` & `tmp/nornir_easy_netmiko-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_easy_netmiko-1.0.0.tar", max compression
+gzip compressed data, was "nornir_easy_netmiko-1.0.1.tar", max compression
```

## Comparing `nornir_easy_netmiko-1.0.0.tar` & `nornir_easy_netmiko-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      667 2023-07-11 12:06:54.998602 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/__init__.py
--rw-r--r--   0        0        0      170 2023-07-11 12:06:55.045613 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/connections/__init__.py
--rw-r--r--   0        0        0      315 2023-07-11 12:06:55.080621 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      341 2023-07-11 12:06:55.097624 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1699 2023-07-11 12:06:55.114629 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc
--rw-r--r--   0        0        0     2406 2023-07-11 12:06:55.126631 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc
--rw-r--r--   0        0        0     1661 2023-07-11 12:06:55.064618 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/connections/netmiko.py
--rw-r--r--   0        0        0      958 2023-07-11 12:06:55.143634 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/errors/__init__.py
--rw-r--r--   0        0        0     1140 2023-07-11 12:06:55.157639 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      634 2023-07-11 12:06:55.179643 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__init__.py
--rw-r--r--   0        0        0      746 2023-07-11 12:06:55.304671 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      836 2023-07-11 12:06:55.316674 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      953 2023-07-11 12:06:55.327677 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc
--rw-r--r--   0        0        0     1316 2023-07-11 12:06:55.344681 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc
--rw-r--r--   0        0        0     1372 2023-07-11 12:06:55.356684 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc
--rw-r--r--   0        0        0     1840 2023-07-11 12:06:55.373686 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc
--rw-r--r--   0        0        0     1405 2023-07-11 12:06:55.385690 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc
--rw-r--r--   0        0        0     1852 2023-07-11 12:06:55.397692 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc
--rw-r--r--   0        0        0     1240 2023-07-11 12:06:55.408696 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc
--rw-r--r--   0        0        0     1596 2023-07-11 12:06:55.425699 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc
--rw-r--r--   0        0        0     1608 2023-07-11 12:06:55.437701 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc
--rw-r--r--   0        0        0     1759 2023-07-11 12:06:55.448704 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc
--rw-r--r--   0        0        0     1691 2023-07-11 12:06:55.471709 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc
--rw-r--r--   0        0        0     2291 2023-07-11 12:06:55.483712 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc
--rw-r--r--   0        0        0      683 2023-07-11 12:06:55.198647 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_commit.py
--rw-r--r--   0        0        0     1189 2023-07-11 12:06:55.216651 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_file_transfer.py
--rw-r--r--   0        0        0     1179 2023-07-11 12:06:55.235656 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_multiline.py
--rw-r--r--   0        0        0     1061 2023-07-11 12:06:55.253660 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_save_config.py
--rw-r--r--   0        0        0     1445 2023-07-11 12:06:55.272664 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_send_command.py
--rw-r--r--   0        0        0     2442 2023-07-11 12:06:55.290669 nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_send_config.py
--rw-r--r--   0        0        0     1018 2023-07-11 12:29:53.322681 nornir_easy_netmiko-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-07-10 07:56:02.280008 nornir_easy_netmiko-1.0.0/README.md
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nornir_easy_netmiko-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      667 2023-07-11 12:45:58.083233 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-11 12:45:58.142246 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/connections/__init__.py
+-rw-r--r--   0        0        0      315 2023-07-11 12:45:58.184256 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      341 2023-07-11 12:45:58.202260 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1699 2023-07-11 12:45:58.222264 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc
+-rw-r--r--   0        0        0     2406 2023-07-11 12:45:58.237268 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc
+-rw-r--r--   0        0        0     1661 2023-07-11 12:45:58.162251 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/connections/netmiko.py
+-rw-r--r--   0        0        0      958 2023-07-11 12:45:58.256272 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/errors/__init__.py
+-rw-r--r--   0        0        0     1140 2023-07-11 12:45:58.278277 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      634 2023-07-11 12:45:58.301282 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-11 12:45:58.424311 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      836 2023-07-11 12:45:58.443314 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      953 2023-07-11 12:45:58.461318 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc
+-rw-r--r--   0        0        0     1316 2023-07-11 12:45:58.480323 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc
+-rw-r--r--   0        0        0     1372 2023-07-11 12:45:58.498326 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc
+-rw-r--r--   0        0        0     1840 2023-07-11 12:45:58.517331 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc
+-rw-r--r--   0        0        0     1405 2023-07-11 12:45:58.536335 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc
+-rw-r--r--   0        0        0     1852 2023-07-11 12:45:58.555339 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc
+-rw-r--r--   0        0        0     1240 2023-07-11 12:45:58.577345 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc
+-rw-r--r--   0        0        0     1596 2023-07-11 12:45:58.595348 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1608 2023-07-11 12:45:58.614352 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc
+-rw-r--r--   0        0        0     1759 2023-07-11 12:45:58.633357 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc
+-rw-r--r--   0        0        0     1691 2023-07-11 12:45:58.660363 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc
+-rw-r--r--   0        0        0     2291 2023-07-11 12:45:58.679367 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc
+-rw-r--r--   0        0        0      683 2023-07-11 12:45:58.317285 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_commit.py
+-rw-r--r--   0        0        0     1189 2023-07-11 12:45:58.333292 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_file_transfer.py
+-rw-r--r--   0        0        0     1179 2023-07-11 12:45:58.350294 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_multiline.py
+-rw-r--r--   0        0        0     1061 2023-07-11 12:45:58.365297 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_save_config.py
+-rw-r--r--   0        0        0     1445 2023-07-11 12:45:58.381300 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_send_command.py
+-rw-r--r--   0        0        0     2442 2023-07-11 12:45:58.403307 nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_send_config.py
+-rw-r--r--   0        0        0     1023 2023-07-11 12:41:46.128089 nornir_easy_netmiko-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-07-10 07:56:02.280008 nornir_easy_netmiko-1.0.1/README.md
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nornir_easy_netmiko-1.0.1/PKG-INFO
```

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/__init__.py` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/connections/netmiko.py` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/connections/netmiko.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/errors/__init__.py` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__init__.py` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_commit.py` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_commit.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_file_transfer.py` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_file_transfer.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_multiline.py` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_multiline.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_save_config.py` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_save_config.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_send_command.py` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_send_command.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/nornir_easy_netmiko/tasks/netmiko_send_config.py` & `nornir_easy_netmiko-1.0.1/nornir_easy_netmiko/tasks/netmiko_send_config.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.0/pyproject.toml` & `nornir_easy_netmiko-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir_easy_netmiko"
-version = "1.0.0"
+version = "1.0.1"
 description = "Netmiko's plugins for Nornir. Support jinja2 and optimized exception."
 license = "Apache-2.0"
 readme = "README.md"
 authors = ['Des1r3 <linzx@anonymous.com>']
 repository = "https://github.com/Des1r3/nornir_easy_netmiko"
 classifiers = [
         "License :: OSI Approved :: Apache Software License",
@@ -12,15 +12,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.plugins."nornir.plugins.connections"]
-"netmiko" = "nornir_netmiko.connections:easy_etmiko"
+"netmiko" = "nornir_easy_netmiko.connections:easy_etmiko"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 netmiko = "^4.0.0"
 jinja2 = "^3.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `nornir_easy_netmiko-1.0.0/PKG-INFO` & `nornir_easy_netmiko-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-easy-netmiko
-Version: 1.0.0
+Version: 1.0.1
 Summary: Netmiko's plugins for Nornir. Support jinja2 and optimized exception.
 Home-page: https://github.com/Des1r3/nornir_easy_netmiko
 License: Apache-2.0
 Author: Des1r3
 Author-email: linzx@anonymous.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

