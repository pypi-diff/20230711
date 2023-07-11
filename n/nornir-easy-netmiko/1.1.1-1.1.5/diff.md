# Comparing `tmp/nornir_easy_netmiko-1.1.1.tar.gz` & `tmp/nornir_easy_netmiko-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_easy_netmiko-1.1.1.tar", max compression
+gzip compressed data, was "nornir_easy_netmiko-1.1.5.tar", max compression
```

## Comparing `nornir_easy_netmiko-1.1.1.tar` & `nornir_easy_netmiko-1.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      667 2023-07-11 12:53:08.966072 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/__init__.py
--rw-r--r--   0        0        0      170 2023-07-11 12:53:09.017084 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/connections/__init__.py
--rw-r--r--   0        0        0      315 2023-07-11 12:53:09.052091 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      351 2023-07-11 12:53:24.061131 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1699 2023-07-11 12:53:09.087099 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc
--rw-r--r--   0        0        0     2432 2023-07-11 12:56:20.297848 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc
--rw-r--r--   0        0        0     1673 2023-07-11 12:54:07.775433 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/connections/netmiko.py
--rw-r--r--   0        0        0      958 2023-07-11 12:53:09.123107 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/errors/__init__.py
--rw-r--r--   0        0        0     1140 2023-07-11 12:53:09.142111 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1896 2023-07-11 12:53:24.263177 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      634 2023-07-11 12:53:09.161115 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__init__.py
--rw-r--r--   0        0        0      746 2023-07-11 12:53:09.279142 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      846 2023-07-11 12:53:24.217167 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      953 2023-07-11 12:53:09.310149 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc
--rw-r--r--   0        0        0     1326 2023-07-11 12:53:24.223169 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc
--rw-r--r--   0        0        0     1372 2023-07-11 12:53:09.345157 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc
--rw-r--r--   0        0        0     1850 2023-07-11 12:53:24.227169 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc
--rw-r--r--   0        0        0     1405 2023-07-11 12:53:09.375164 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc
--rw-r--r--   0        0        0     1862 2023-07-11 12:53:24.273180 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc
--rw-r--r--   0        0        0     1240 2023-07-11 12:53:09.404170 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc
--rw-r--r--   0        0        0     1606 2023-07-11 12:53:24.232171 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc
--rw-r--r--   0        0        0     1608 2023-07-11 12:53:09.435177 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc
--rw-r--r--   0        0        0     2206 2023-07-11 12:53:24.236172 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc
--rw-r--r--   0        0        0     1691 2023-07-11 12:53:09.465184 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc
--rw-r--r--   0        0        0     3912 2023-07-11 12:53:24.268179 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc
--rw-r--r--   0        0        0      683 2023-07-11 12:53:09.177120 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_commit.py
--rw-r--r--   0        0        0     1189 2023-07-11 12:53:09.194123 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_file_transfer.py
--rw-r--r--   0        0        0     1179 2023-07-11 12:53:09.210126 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_multiline.py
--rw-r--r--   0        0        0     1061 2023-07-11 12:53:09.227130 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_save_config.py
--rw-r--r--   0        0        0     1445 2023-07-11 12:53:09.244135 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_send_command.py
--rw-r--r--   0        0        0     2442 2023-07-11 12:53:09.261139 nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_send_config.py
--rw-r--r--   0        0        0     1031 2023-07-11 12:59:10.476033 nornir_easy_netmiko-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       21 2023-07-10 07:56:02.280008 nornir_easy_netmiko-1.1.1/README.md
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nornir_easy_netmiko-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      667 2023-07-11 12:53:08.966072 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-11 12:53:09.017084 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__init__.py
+-rw-r--r--   0        0        0      315 2023-07-11 12:53:09.052091 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      351 2023-07-11 12:53:24.061131 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1699 2023-07-11 12:53:09.087099 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc
+-rw-r--r--   0        0        0     2432 2023-07-11 12:56:20.297848 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc
+-rw-r--r--   0        0        0     1673 2023-07-11 12:54:07.775433 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/netmiko.py
+-rw-r--r--   0        0        0      958 2023-07-11 12:53:09.123107 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__init__.py
+-rw-r--r--   0        0        0     1140 2023-07-11 12:53:09.142111 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1896 2023-07-11 12:53:24.263177 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      634 2023-07-11 12:53:09.161115 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-11 12:53:09.279142 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      846 2023-07-11 12:53:24.217167 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      953 2023-07-11 12:53:09.310149 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc
+-rw-r--r--   0        0        0     1326 2023-07-11 12:53:24.223169 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc
+-rw-r--r--   0        0        0     1372 2023-07-11 12:53:09.345157 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc
+-rw-r--r--   0        0        0     1850 2023-07-11 12:53:24.227169 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc
+-rw-r--r--   0        0        0     1405 2023-07-11 12:53:09.375164 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc
+-rw-r--r--   0        0        0     1862 2023-07-11 12:53:24.273180 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc
+-rw-r--r--   0        0        0     1240 2023-07-11 12:53:09.404170 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc
+-rw-r--r--   0        0        0     1606 2023-07-11 12:53:24.232171 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1608 2023-07-11 12:53:09.435177 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc
+-rw-r--r--   0        0        0     2206 2023-07-11 12:53:24.236172 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc
+-rw-r--r--   0        0        0     1691 2023-07-11 12:53:09.465184 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc
+-rw-r--r--   0        0        0     3912 2023-07-11 12:53:24.268179 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc
+-rw-r--r--   0        0        0      683 2023-07-11 12:53:09.177120 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_commit.py
+-rw-r--r--   0        0        0     1189 2023-07-11 12:53:09.194123 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_file_transfer.py
+-rw-r--r--   0        0        0     1179 2023-07-11 12:53:09.210126 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_multiline.py
+-rw-r--r--   0        0        0     1061 2023-07-11 12:53:09.227130 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_save_config.py
+-rw-r--r--   0        0        0     1445 2023-07-11 12:53:09.244135 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_send_command.py
+-rw-r--r--   0        0        0     2442 2023-07-11 12:53:09.261139 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_send_config.py
+-rw-r--r--   0        0        0     1024 2023-07-11 13:08:23.146075 nornir_easy_netmiko-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-07-10 07:56:02.280008 nornir_easy_netmiko-1.1.5/README.md
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nornir_easy_netmiko-1.1.5/PKG-INFO
```

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/__init__.py` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/connections/netmiko.py` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/netmiko.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/errors/__init__.py` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-311.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__init__.py` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_commit.py` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_commit.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_file_transfer.py` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_file_transfer.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_multiline.py` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_multiline.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_save_config.py` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_save_config.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_send_command.py` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_send_command.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/nornir_easy_netmiko/tasks/netmiko_send_config.py` & `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_send_config.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.1/pyproject.toml` & `nornir_easy_netmiko-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir_easy_netmiko"
-version = "1.1.1"
+version = "1.1.5"
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
-"netmiko" = "nornir_easy_netmiko.connections:nornir_easy_netmiko"
+"easy_netmiko" = "nornir_easy_netmiko.connections:Netmiko"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 netmiko = "^4.0.0"
 jinja2 = "^3.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `nornir_easy_netmiko-1.1.1/PKG-INFO` & `nornir_easy_netmiko-1.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-easy-netmiko
-Version: 1.1.1
+Version: 1.1.5
 Summary: Netmiko's plugins for Nornir. Support jinja2 and optimized exception.
 Home-page: https://github.com/Des1r3/nornir_easy_netmiko
 License: Apache-2.0
 Author: Des1r3
 Author-email: linzx@anonymous.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

