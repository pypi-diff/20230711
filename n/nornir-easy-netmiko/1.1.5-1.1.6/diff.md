# Comparing `tmp/nornir_easy_netmiko-1.1.5.tar.gz` & `tmp/nornir_easy_netmiko-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_easy_netmiko-1.1.5.tar", max compression
+gzip compressed data, was "nornir_easy_netmiko-1.1.6.tar", max compression
```

## Comparing `nornir_easy_netmiko-1.1.5.tar` & `nornir_easy_netmiko-1.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      667 2023-07-11 12:53:08.966072 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/__init__.py
--rw-r--r--   0        0        0      170 2023-07-11 12:53:09.017084 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__init__.py
--rw-r--r--   0        0        0      315 2023-07-11 12:53:09.052091 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      351 2023-07-11 12:53:24.061131 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1699 2023-07-11 12:53:09.087099 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc
--rw-r--r--   0        0        0     2432 2023-07-11 12:56:20.297848 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc
--rw-r--r--   0        0        0     1673 2023-07-11 12:54:07.775433 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/netmiko.py
--rw-r--r--   0        0        0      958 2023-07-11 12:53:09.123107 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__init__.py
--rw-r--r--   0        0        0     1140 2023-07-11 12:53:09.142111 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1896 2023-07-11 12:53:24.263177 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      634 2023-07-11 12:53:09.161115 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__init__.py
--rw-r--r--   0        0        0      746 2023-07-11 12:53:09.279142 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      846 2023-07-11 12:53:24.217167 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      953 2023-07-11 12:53:09.310149 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc
--rw-r--r--   0        0        0     1326 2023-07-11 12:53:24.223169 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc
--rw-r--r--   0        0        0     1372 2023-07-11 12:53:09.345157 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc
--rw-r--r--   0        0        0     1850 2023-07-11 12:53:24.227169 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc
--rw-r--r--   0        0        0     1405 2023-07-11 12:53:09.375164 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc
--rw-r--r--   0        0        0     1862 2023-07-11 12:53:24.273180 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc
--rw-r--r--   0        0        0     1240 2023-07-11 12:53:09.404170 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc
--rw-r--r--   0        0        0     1606 2023-07-11 12:53:24.232171 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc
--rw-r--r--   0        0        0     1608 2023-07-11 12:53:09.435177 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc
--rw-r--r--   0        0        0     2206 2023-07-11 12:53:24.236172 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc
--rw-r--r--   0        0        0     1691 2023-07-11 12:53:09.465184 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc
--rw-r--r--   0        0        0     3912 2023-07-11 12:53:24.268179 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc
--rw-r--r--   0        0        0      683 2023-07-11 12:53:09.177120 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_commit.py
--rw-r--r--   0        0        0     1189 2023-07-11 12:53:09.194123 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_file_transfer.py
--rw-r--r--   0        0        0     1179 2023-07-11 12:53:09.210126 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_multiline.py
--rw-r--r--   0        0        0     1061 2023-07-11 12:53:09.227130 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_save_config.py
--rw-r--r--   0        0        0     1445 2023-07-11 12:53:09.244135 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_send_command.py
--rw-r--r--   0        0        0     2442 2023-07-11 12:53:09.261139 nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_send_config.py
--rw-r--r--   0        0        0     1024 2023-07-11 13:08:23.146075 nornir_easy_netmiko-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       21 2023-07-10 07:56:02.280008 nornir_easy_netmiko-1.1.5/README.md
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nornir_easy_netmiko-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      667 2023-07-11 13:12:50.179098 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-11 13:12:50.237110 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__init__.py
+-rw-r--r--   0        0        0      315 2023-07-11 13:12:50.269117 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      351 2023-07-11 13:13:51.455855 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1699 2023-07-11 13:12:50.302125 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc
+-rw-r--r--   0        0        0     2425 2023-07-11 13:13:51.459856 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc
+-rw-r--r--   0        0        0     1666 2023-07-11 13:13:38.039628 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/netmiko.py
+-rw-r--r--   0        0        0      958 2023-07-11 13:12:50.335132 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__init__.py
+-rw-r--r--   0        0        0     1140 2023-07-11 13:12:50.352136 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1896 2023-07-11 13:13:51.657900 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      634 2023-07-11 13:12:50.370140 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-11 13:12:50.482165 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      846 2023-07-11 13:13:51.613890 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      953 2023-07-11 13:12:50.518173 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc
+-rw-r--r--   0        0        0     1326 2023-07-11 13:13:51.618891 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc
+-rw-r--r--   0        0        0     1372 2023-07-11 13:12:50.553180 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc
+-rw-r--r--   0        0        0     1850 2023-07-11 13:13:51.623892 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc
+-rw-r--r--   0        0        0     1405 2023-07-11 13:12:50.584188 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc
+-rw-r--r--   0        0        0     1862 2023-07-11 13:13:51.667902 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc
+-rw-r--r--   0        0        0     1240 2023-07-11 13:12:50.620195 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc
+-rw-r--r--   0        0        0     1606 2023-07-11 13:13:51.627893 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1608 2023-07-11 13:12:50.656204 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc
+-rw-r--r--   0        0        0     2206 2023-07-11 13:13:51.632894 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc
+-rw-r--r--   0        0        0     1691 2023-07-11 13:12:50.693213 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc
+-rw-r--r--   0        0        0     3912 2023-07-11 13:13:51.662901 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc
+-rw-r--r--   0        0        0      683 2023-07-11 13:12:50.385143 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_commit.py
+-rw-r--r--   0        0        0     1189 2023-07-11 13:12:50.400146 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_file_transfer.py
+-rw-r--r--   0        0        0     1179 2023-07-11 13:12:50.416150 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_multiline.py
+-rw-r--r--   0        0        0     1061 2023-07-11 13:12:50.431153 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_save_config.py
+-rw-r--r--   0        0        0     1445 2023-07-11 13:12:50.446157 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_send_command.py
+-rw-r--r--   0        0        0     2442 2023-07-11 13:12:50.461160 nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_send_config.py
+-rw-r--r--   0        0        0     1024 2023-07-11 13:13:47.427008 nornir_easy_netmiko-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-07-10 07:56:02.280008 nornir_easy_netmiko-1.1.6/README.md
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nornir_easy_netmiko-1.1.6/PKG-INFO
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/__init__.py` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xef50ad64 (Tue Jul 11 12:54:07 2023 UTC)
-files sz: 1673
+moddate:  0x8255ad64 (Tue Jul 11 13:13:38 2023 UTC)
+files sz: 1666
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -34,15 +34,15 @@
      5          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               3 (('Config',))
                 38 IMPORT_NAME              6 (nornir.core.configuration)
                 40 IMPORT_FROM              7 (Config)
                 42 STORE_NAME               7 (Config)
                 44 POP_TOP
    
-     8          46 LOAD_CONST               4 ('nornir_easy_netmiko')
+     8          46 LOAD_CONST               4 ('easy_netmiko')
                 48 STORE_NAME               8 (CONNECTION_NAME)
    
     11          50 LOAD_CONST               5 ('cisco_ios')
    
     12          52 LOAD_CONST               6 ('cisco_nxos')
    
     13          54 LOAD_CONST               6 ('cisco_nxos')
@@ -68,15 +68,15 @@
                 94 LOAD_CONST              13 (None)
                 96 RETURN_VALUE
    consts
       0
       ('Any', 'Dict', 'Optional')
       ('ConnectHandler',)
       ('Config',)
-      'nornir_easy_netmiko'
+      'easy_netmiko'
       'cisco_ios'
       'cisco_nxos'
       'arista_eos'
       'juniper_junos'
       'cisco_xr'
       ('ios', 'nxos', 'nxos_ssh', 'eos', 'junos', 'iosxr')
       code
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/connections/netmiko.py` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/connections/netmiko.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, Optional
 
 from netmiko import ConnectHandler
 
 from nornir.core.configuration import Config
 
 
-CONNECTION_NAME = "nornir_easy_netmiko"
+CONNECTION_NAME = "easy_netmiko"
 
 napalm_to_netmiko_map = {
     "ios": "cisco_ios",
     "nxos": "cisco_nxos",
     "nxos_ssh": "cisco_nxos",
     "eos": "arista_eos",
     "junos": "juniper_junos",
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__init__.py` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-311.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
+moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
 files sz: 958
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__init__.py` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
+moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
 files sz: 634
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
+moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
 files sz: 683
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
+moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
 files sz: 1189
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
+moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
 files sz: 1179
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
+moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
 files sz: 1061
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
+moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
 files sz: 1445
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 14
    flags     : 0
    code
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
+moddate:  0x5255ad64 (Tue Jul 11 13:12:50 2023 UTC)
 files sz: 2442
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
```

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_commit.py` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_commit.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_file_transfer.py` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_file_transfer.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_multiline.py` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_multiline.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_save_config.py` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_save_config.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_send_command.py` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_send_command.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/nornir_easy_netmiko/tasks/netmiko_send_config.py` & `nornir_easy_netmiko-1.1.6/nornir_easy_netmiko/tasks/netmiko_send_config.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.1.5/pyproject.toml` & `nornir_easy_netmiko-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir_easy_netmiko"
-version = "1.1.5"
+version = "1.1.6"
 description = "Netmiko's plugins for Nornir. Support jinja2 and optimized exception."
 license = "Apache-2.0"
 readme = "README.md"
 authors = ['Des1r3 <linzx@anonymous.com>']
 repository = "https://github.com/Des1r3/nornir_easy_netmiko"
 classifiers = [
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `nornir_easy_netmiko-1.1.5/PKG-INFO` & `nornir_easy_netmiko-1.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-easy-netmiko
-Version: 1.1.5
+Version: 1.1.6
 Summary: Netmiko's plugins for Nornir. Support jinja2 and optimized exception.
 Home-page: https://github.com/Des1r3/nornir_easy_netmiko
 License: Apache-2.0
 Author: Des1r3
 Author-email: linzx@anonymous.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

