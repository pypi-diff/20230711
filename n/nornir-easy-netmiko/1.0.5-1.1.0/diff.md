# Comparing `tmp/nornir_easy_netmiko-1.0.5.tar.gz` & `tmp/nornir_easy_netmiko-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_easy_netmiko-1.0.5.tar", max compression
+gzip compressed data, was "nornir_easy_netmiko-1.1.0.tar", max compression
```

## Comparing `nornir_easy_netmiko-1.0.5.tar` & `nornir_easy_netmiko-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      667 2023-07-11 12:53:08.966072 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/__init__.py
--rw-r--r--   0        0        0      170 2023-07-11 12:53:09.017084 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/connections/__init__.py
--rw-r--r--   0        0        0      315 2023-07-11 12:53:09.052091 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      341 2023-07-11 12:53:09.071095 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1699 2023-07-11 12:53:09.087099 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc
--rw-r--r--   0        0        0     2406 2023-07-11 12:53:09.103103 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc
--rw-r--r--   0        0        0     1661 2023-07-11 12:53:09.033087 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/connections/netmiko.py
--rw-r--r--   0        0        0      958 2023-07-11 12:53:09.123107 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/errors/__init__.py
--rw-r--r--   0        0        0     1140 2023-07-11 12:53:09.142111 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      634 2023-07-11 12:53:09.161115 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__init__.py
--rw-r--r--   0        0        0      746 2023-07-11 12:53:09.279142 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      836 2023-07-11 12:53:09.294145 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      953 2023-07-11 12:53:09.310149 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc
--rw-r--r--   0        0        0     1316 2023-07-11 12:53:09.329153 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc
--rw-r--r--   0        0        0     1372 2023-07-11 12:53:09.345157 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc
--rw-r--r--   0        0        0     1840 2023-07-11 12:53:09.359161 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc
--rw-r--r--   0        0        0     1405 2023-07-11 12:53:09.375164 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc
--rw-r--r--   0        0        0     1852 2023-07-11 12:53:09.390170 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc
--rw-r--r--   0        0        0     1240 2023-07-11 12:53:09.404170 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc
--rw-r--r--   0        0        0     1596 2023-07-11 12:53:09.420174 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc
--rw-r--r--   0        0        0     1608 2023-07-11 12:53:09.435177 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc
--rw-r--r--   0        0        0     1759 2023-07-11 12:53:09.450181 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc
--rw-r--r--   0        0        0     1691 2023-07-11 12:53:09.465184 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc
--rw-r--r--   0        0        0     2291 2023-07-11 12:53:09.479189 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc
--rw-r--r--   0        0        0      683 2023-07-11 12:53:09.177120 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_commit.py
--rw-r--r--   0        0        0     1189 2023-07-11 12:53:09.194123 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_file_transfer.py
--rw-r--r--   0        0        0     1179 2023-07-11 12:53:09.210126 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_multiline.py
--rw-r--r--   0        0        0     1061 2023-07-11 12:53:09.227130 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_save_config.py
--rw-r--r--   0        0        0     1445 2023-07-11 12:53:09.244135 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_send_command.py
--rw-r--r--   0        0        0     2442 2023-07-11 12:53:09.261139 nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_send_config.py
--rw-r--r--   0        0        0     1031 2023-07-11 12:51:37.002416 nornir_easy_netmiko-1.0.5/pyproject.toml
--rw-r--r--   0        0        0       21 2023-07-10 07:56:02.280008 nornir_easy_netmiko-1.0.5/README.md
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nornir_easy_netmiko-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      667 2023-07-11 12:53:08.966072 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-11 12:53:09.017084 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/connections/__init__.py
+-rw-r--r--   0        0        0      315 2023-07-11 12:53:09.052091 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      351 2023-07-11 12:53:24.061131 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/connections/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1699 2023-07-11 12:53:09.087099 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc
+-rw-r--r--   0        0        0     2416 2023-07-11 12:53:24.066134 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc
+-rw-r--r--   0        0        0     1673 2023-07-11 12:54:07.775433 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/connections/netmiko.py
+-rw-r--r--   0        0        0      958 2023-07-11 12:53:09.123107 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/errors/__init__.py
+-rw-r--r--   0        0        0     1140 2023-07-11 12:53:09.142111 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1896 2023-07-11 12:53:24.263177 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      634 2023-07-11 12:53:09.161115 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-11 12:53:09.279142 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      846 2023-07-11 12:53:24.217167 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      953 2023-07-11 12:53:09.310149 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc
+-rw-r--r--   0        0        0     1326 2023-07-11 12:53:24.223169 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc
+-rw-r--r--   0        0        0     1372 2023-07-11 12:53:09.345157 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc
+-rw-r--r--   0        0        0     1850 2023-07-11 12:53:24.227169 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc
+-rw-r--r--   0        0        0     1405 2023-07-11 12:53:09.375164 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc
+-rw-r--r--   0        0        0     1862 2023-07-11 12:53:24.273180 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc
+-rw-r--r--   0        0        0     1240 2023-07-11 12:53:09.404170 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc
+-rw-r--r--   0        0        0     1606 2023-07-11 12:53:24.232171 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1608 2023-07-11 12:53:09.435177 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc
+-rw-r--r--   0        0        0     2206 2023-07-11 12:53:24.236172 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc
+-rw-r--r--   0        0        0     1691 2023-07-11 12:53:09.465184 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc
+-rw-r--r--   0        0        0     3912 2023-07-11 12:53:24.268179 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-311.pyc
+-rw-r--r--   0        0        0      683 2023-07-11 12:53:09.177120 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_commit.py
+-rw-r--r--   0        0        0     1189 2023-07-11 12:53:09.194123 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_file_transfer.py
+-rw-r--r--   0        0        0     1179 2023-07-11 12:53:09.210126 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_multiline.py
+-rw-r--r--   0        0        0     1061 2023-07-11 12:53:09.227130 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_save_config.py
+-rw-r--r--   0        0        0     1445 2023-07-11 12:53:09.244135 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_send_command.py
+-rw-r--r--   0        0        0     2442 2023-07-11 12:53:09.261139 nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_send_config.py
+-rw-r--r--   0        0        0     1031 2023-07-11 12:54:18.163330 nornir_easy_netmiko-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-07-10 07:56:02.280008 nornir_easy_netmiko-1.1.0/README.md
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 nornir_easy_netmiko-1.1.0/PKG-INFO
```

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/__init__.py` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/connections/__pycache__/netmiko.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x39098b64 (Thu Jun 15 12:51:05 2023 UTC)
+moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
 files sz: 1661
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
@@ -55,15 +55,15 @@
    
     10          62 LOAD_CONST              10 (('ios', 'nxos', 'nxos_ssh', 'eos', 'junos', 'iosxr'))
                 64 BUILD_CONST_KEY_MAP      6
                 66 STORE_NAME               9 (napalm_to_netmiko_map)
    
     20          68 PUSH_NULL
                 70 LOAD_BUILD_CLASS
-                72 LOAD_CONST              11 (<code object Netmiko, file "e:\资料\nornir\nornir_easy_netmiko\connections\netmiko.py", line 20>)
+                72 LOAD_CONST              11 (<code object Netmiko, file "E:\资料\nornir_myproject\nornir_easy_netmiko\connections\netmiko.py", line 20>)
                 74 MAKE_FUNCTION            0
                 76 LOAD_CONST              12 ('Netmiko')
                 78 PRECALL                  2
                 82 CALL                     2
                 92 STORE_NAME              10 (Netmiko)
                 94 LOAD_CONST              13 (None)
                 96 RETURN_VALUE
@@ -152,20 +152,20 @@
                      138 BINARY_SUBSCR
          
           28         148 LOAD_CONST              10 ('return')
          
           37         150 LOAD_CONST               2 (None)
          
           28         152 BUILD_TUPLE             16
-                     154 LOAD_CONST              11 (<code object open, file "e:\资料\nornir\nornir_easy_netmiko\connections\netmiko.py", line 28>)
+                     154 LOAD_CONST              11 (<code object open, file "E:\资料\nornir_myproject\nornir_easy_netmiko\connections\netmiko.py", line 28>)
                      156 MAKE_FUNCTION            5 (defaults, annotations)
                      158 STORE_NAME              10 (open)
          
           62         160 LOAD_CONST              14 (('return', None))
-                     162 LOAD_CONST              12 (<code object close, file "e:\资料\nornir\nornir_easy_netmiko\connections\netmiko.py", line 62>)
+                     162 LOAD_CONST              12 (<code object close, file "E:\资料\nornir_myproject\nornir_easy_netmiko\connections\netmiko.py", line 62>)
                      164 MAKE_FUNCTION            4 (annotations)
                      166 STORE_NAME              11 (close)
                      168 LOAD_CONST               2 (None)
                      170 RETURN_VALUE
          consts
             'Netmiko'
             '\n    This plugin connects to the device using the Netmiko driver and sets the\n    relevant connection.\n    Inventory:\n        extras: maps to argument passed to ``ConnectHandler``.\n    '
@@ -285,15 +285,15 @@
                   'ssh_config_file'
                   'device_type'
                   ()
                names      ('ssh', 'config_file', 'AttributeError', 'napalm_to_netmiko_map', 'get', 'update', 'ConnectHandler', 'connection')
                varnames   ('self', 'hostname', 'username', 'password', 'port', 'platform', 'extras', 'configuration', 'parameters', 'connection')
                freevars   ()
                cellvars   ()
-               filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\connections\\netmiko.py'
+               filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\connections\\netmiko.py'
                name       'open'
                firstlineno 28
                lnotab
                   0x020b02010201020102fc0607020316fe020102ff0803120104ff080304
                   0236010a0208012a011801
             code
                argcount  : 1
@@ -315,33 +315,33 @@
                             54 RETURN_VALUE
                consts
                   None
                names      ('connection', 'disconnect')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\connections\\netmiko.py'
+               filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\connections\\netmiko.py'
                name       'close'
                firstlineno 62
                lnotab 0x0201
             (None, None)
             ('return', None)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Optional', 'str', 'int', 'Dict', 'Any', 'Config', 'open', 'close')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\connections\\netmiko.py'
+         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\connections\\netmiko.py'
          name       'Netmiko'
          firstlineno 20
          lnotab
             0x0a01040e020102f804020efe02030efd02040efc02050efb02060efa02
             071ef902080ef8020902f70822
       'Netmiko'
       None
    names      ('typing', 'Any', 'Dict', 'Optional', 'netmiko', 'ConnectHandler', 'nornir.core.configuration', 'Config', 'CONNECTION_NAME', 'napalm_to_netmiko_map', 'Netmiko')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\connections\\netmiko.py'
+   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\connections\\netmiko.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020114020c020c0304030201020102010201020102fa060a
```

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/connections/netmiko.py` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/connections/netmiko.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, Optional
 
 from netmiko import ConnectHandler
 
 from nornir.core.configuration import Config
 
 
-CONNECTION_NAME = "netmiko"
+CONNECTION_NAME = "nornir_easy_netmiko"
 
 napalm_to_netmiko_map = {
     "ios": "cisco_ios",
     "nxos": "cisco_nxos",
     "nxos_ssh": "cisco_nxos",
     "eos": "arista_eos",
     "junos": "juniper_junos",
```

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/errors/__init__.py` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/errors/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__init__.py` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/__init__.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1d0d8b64 (Thu Jun 15 13:07:41 2023 UTC)
+moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
 files sz: 634
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
@@ -68,11 +68,11 @@
       ('netmiko_multiline',)
       ('netmiko_commit', 'netmiko_file_transfer', 'netmiko_save_config', 'netmiko_send_command', 'netmiko_send_config', 'netmiko_multiline')
       None
    names      ('nornir_easy_netmiko.tasks.netmiko_commit', 'netmiko_commit', 'nornir_easy_netmiko.tasks.netmiko_file_transfer', 'netmiko_file_transfer', 'nornir_easy_netmiko.tasks.netmiko_save_config', 'netmiko_save_config', 'nornir_easy_netmiko.tasks.netmiko_send_command', 'netmiko_send_command', 'nornir_easy_netmiko.tasks.netmiko_send_config', 'netmiko_send_config', 'nornir_easy_netmiko.tasks.netmiko_multiline', 'netmiko_multiline', '__all__')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\__init__.py'
+   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c010c010c010c010c010c03
```

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_commit.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x1e0d8b64 (Thu Jun 15 13:07:42 2023 UTC)
-files sz: 684
+moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
+files sz: 683
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a0401
@@ -38,15 +38,15 @@
      6          42 LOAD_CONST               4 ('task')
                 44 LOAD_NAME                4 (Task)
                 46 LOAD_CONST               5 ('kwargs')
                 48 LOAD_NAME                1 (Any)
                 50 LOAD_CONST               6 ('return')
                 52 LOAD_NAME                3 (Result)
                 54 BUILD_TUPLE              6
-                56 LOAD_CONST               7 (<code object netmiko_commit, file "e:\资料\nornir\nornir_easy_netmiko\tasks\netmiko_commit.py", line 6>)
+                56 LOAD_CONST               7 (<code object netmiko_commit, file "E:\资料\nornir_myproject\nornir_easy_netmiko\tasks\netmiko_commit.py", line 6>)
                 58 MAKE_FUNCTION            4 (annotations)
                 60 STORE_NAME               7 (netmiko_commit)
                 62 LOAD_CONST               8 (None)
                 64 RETURN_VALUE
    consts
       0
       ('Any',)
@@ -118,20 +118,20 @@
             True
             ('host', 'result', 'changed')
             ()
          names      ('host', 'get_connection', 'CONNECTION_NAME', 'nornir', 'config', 'commit', 'check_config_mode', 'exit_config_mode', 'Result')
          varnames   ('task', 'kwargs', 'conn', 'result')
          freevars   ()
          cellvars   ()
-         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_commit.py'
+         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_commit.py'
          name       'netmiko_commit'
          firstlineno 6
          lnotab 0x020b54011a0228012801
       None
    names      ('typing', 'Any', 'nornir.core.task', 'Result', 'Task', 'nornir_easy_netmiko.connections', 'CONNECTION_NAME', 'netmiko_commit')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_commit.py'
+   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_commit.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0110010c03
```

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_file_transfer.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1d0d8b64 (Thu Jun 15 13:07:41 2023 UTC)
+moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
 files sz: 1189
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
@@ -59,15 +59,15 @@
      8          68 LOAD_NAME                1 (Any)
    
      7          70 LOAD_CONST               9 ('return')
    
      9          72 LOAD_NAME                5 (Result)
    
      7          74 BUILD_TUPLE             10
-                76 LOAD_CONST              10 (<code object netmiko_file_transfer, file "e:\资料\nornir\nornir_easy_netmiko\tasks\netmiko_file_transfer.py", line 7>)
+                76 LOAD_CONST              10 (<code object netmiko_file_transfer, file "E:\资料\nornir_myproject\nornir_easy_netmiko\tasks\netmiko_file_transfer.py", line 7>)
                 78 MAKE_FUNCTION            4 (annotations)
                 80 STORE_NAME              10 (netmiko_file_transfer)
                 82 LOAD_CONST              11 (None)
                 84 RETURN_VALUE
    consts
       0
       ('Any',)
@@ -183,24 +183,24 @@
             'file_verified'
             'file_transferred'
             ('host', 'result', 'changed')
          names      ('host', 'get_connection', 'CONNECTION_NAME', 'nornir', 'config', 'setdefault', 'file_transfer', 'get', 'Result')
          varnames   ('task', 'source_file', 'dest_file', 'kwargs', 'net_connect', 'scp_result', 'file_valid')
          freevars   ()
          cellvars   ()
-         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_file_transfer.py'
+         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_file_transfer.py'
          name       'netmiko_file_transfer'
          firstlineno 7
          lnotab
             0x021154012c010c0102ff020104ff040102ff06032e01120220010c011c
             ff
       None
    names      ('typing', 'Any', 'netmiko', 'file_transfer', 'nornir.core.task', 'Result', 'Task', 'nornir_easy_netmiko.connections', 'CONNECTION_NAME', 'str', 'netmiko_file_transfer')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_file_transfer.py'
+   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_file_transfer.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c0110010c03020102ff020102ff020102ff020102ff02
       0202fe
```

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_multiline.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1d0d8b64 (Thu Jun 15 13:07:41 2023 UTC)
+moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
 files sz: 1179
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
@@ -77,15 +77,15 @@
     11         118 LOAD_NAME                4 (Any)
    
      6         120 LOAD_CONST              10 ('return')
    
     12         122 LOAD_NAME                6 (Result)
    
      6         124 BUILD_TUPLE             12
-               126 LOAD_CONST              11 (<code object netmiko_multiline, file "e:\资料\nornir\nornir_easy_netmiko\tasks\netmiko_multiline.py", line 6>)
+               126 LOAD_CONST              11 (<code object netmiko_multiline, file "E:\资料\nornir_myproject\nornir_easy_netmiko\tasks\netmiko_multiline.py", line 6>)
                128 MAKE_FUNCTION            5 (defaults, annotations)
                130 STORE_NAME              12 (netmiko_multiline)
                132 LOAD_CONST              12 (None)
                134 RETURN_VALUE
    consts
       0
       ('Sequence', 'Union', 'List', 'Any')
@@ -171,23 +171,23 @@
          consts
             '\n    Execute Netmiko send_multiline method (or send_multiline_timing)\n\n    Arguments:\n        commands: List or list of lists (see Netmiko send_multiline)\n        use_timing: Set to True to switch to send_multiline_timing method.\n        enable: Set to True to force Netmiko .enable() call.\n        kwargs: Additional arguments to pass to send_multiline method.\n\n    Returns:\n        Result object with the following attributes set:\n          * result: String result showing you the output from commands\n    '
             ('host', 'result')
          names      ('host', 'get_connection', 'CONNECTION_NAME', 'nornir', 'config', 'enable', 'send_multiline_timing', 'send_multiline', 'Result')
          varnames   ('task', 'commands', 'use_timing', 'enable', 'kwargs', 'net_connect', 'result')
          freevars   ()
          cellvars   ()
-         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_multiline.py'
+         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_multiline.py'
          name       'netmiko_multiline'
          firstlineno 6
          lnotab 0x021454010401280104011e021c01
       None
       (False, False)
    names      ('typing', 'Sequence', 'Union', 'List', 'Any', 'nornir.core.task', 'Result', 'Task', 'nornir_easy_netmiko.connections', 'CONNECTION_NAME', 'str', 'bool', 'netmiko_multiline')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_multiline.py'
+   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_multiline.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201180110010c06020102fc040102ff02022afe020302fd020402
       fc020502fb020602fa
```

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_save_config.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1d0d8b64 (Thu Jun 15 13:07:41 2023 UTC)
+moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
 files sz: 1061
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
@@ -48,15 +48,15 @@
      6          48 LOAD_NAME                5 (str)
    
      5          50 LOAD_CONST               9 ('return')
    
      7          52 LOAD_NAME                1 (Result)
    
      5          54 BUILD_TUPLE             10
-                56 LOAD_CONST              10 (<code object netmiko_save_config, file "e:\资料\nornir\nornir_easy_netmiko\tasks\netmiko_save_config.py", line 5>)
+                56 LOAD_CONST              10 (<code object netmiko_save_config, file "E:\资料\nornir_myproject\nornir_easy_netmiko\tasks\netmiko_save_config.py", line 5>)
                 58 MAKE_FUNCTION            5 (defaults, annotations)
                 60 STORE_NAME               7 (netmiko_save_config)
                 62 LOAD_CONST              11 (None)
                 64 RETURN_VALUE
    consts
       0
       ('Result', 'Task')
@@ -135,23 +135,23 @@
             ('confirm', 'confirm_response')
             True
             ('host', 'result', 'changed')
          names      ('host', 'get_connection', 'CONNECTION_NAME', 'nornir', 'config', 'save_config', 'Result')
          varnames   ('task', 'cmd', 'confirm', 'confirm_response', 'conn', 'result')
          freevars   ()
          cellvars   ()
-         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_save_config.py'
+         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_save_config.py'
          name       'netmiko_save_config'
          firstlineno 5
          lnotab 0x020f54010401180106ff14042e01
       None
       ('', False, '')
    names      ('nornir.core.task', 'Result', 'Task', 'nornir_easy_netmiko.connections', 'CONNECTION_NAME', 'str', 'bool', 'netmiko_save_config')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_save_config.py'
+   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_save_config.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020110010c0402ff040102ff020102ff020102ff020102ff020202
       fe
```

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_command.cpython-311.pyc`

 * *Files 27% similar despite different names*

#### Python bytecode

```diff
@@ -1,177 +1,230 @@
 magic:    0xa70d0d0a
-moddate:  0x5a108b64 (Thu Jun 15 13:21:30 2023 UTC)
-files sz: 1170
+moddate:  0xb550ad64 (Tue Jul 11 12:53:09 2023 UTC)
+files sz: 1445
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 13
+   stacksize : 14
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a0401
-      00640064036c056d065a06010009000900640d6405650464066507640765
-      086408650864096501640a6503660c640b84055a09640c5300
+      00640064036c056d065a066d075a070100640064046c086d095a09010064
+      0064056c0a6d0b5a0b0100650b09000900640f640765076408650c640965
+      0d640a650d640b6501640c6506660c640d8405a6000000ab000000000000
+      0000005a0e640e5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Any',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Any)
                 10 STORE_NAME               1 (Any)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('Result', 'Task'))
-                18 IMPORT_NAME              2 (nornir.core.task)
-                20 IMPORT_FROM              3 (Result)
-                22 STORE_NAME               3 (Result)
-                24 IMPORT_FROM              4 (Task)
-                26 STORE_NAME               4 (Task)
+                16 LOAD_CONST               2 (('Template', 'StrictUndefined'))
+                18 IMPORT_NAME              2 (jinja2)
+                20 IMPORT_FROM              3 (Template)
+                22 STORE_NAME               3 (Template)
+                24 IMPORT_FROM              4 (StrictUndefined)
+                26 STORE_NAME               4 (StrictUndefined)
                 28 POP_TOP
    
      3          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('CONNECTION_NAME',))
-                34 IMPORT_NAME              5 (nornir_easy_netmiko.connections)
-                36 IMPORT_FROM              6 (CONNECTION_NAME)
-                38 STORE_NAME               6 (CONNECTION_NAME)
-                40 POP_TOP
+                32 LOAD_CONST               3 (('Result', 'Task'))
+                34 IMPORT_NAME              5 (nornir.core.task)
+                36 IMPORT_FROM              6 (Result)
+                38 STORE_NAME               6 (Result)
+                40 IMPORT_FROM              7 (Task)
+                42 STORE_NAME               7 (Task)
+                44 POP_TOP
    
-     9          42 NOP
+     4          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('CONNECTION_NAME',))
+                50 IMPORT_NAME              8 (nornir_easy_netmiko.connections)
+                52 IMPORT_FROM              9 (CONNECTION_NAME)
+                54 STORE_NAME               9 (CONNECTION_NAME)
+                56 POP_TOP
    
-    10          44 NOP
+     5          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               5 (('error_handle',))
+                62 IMPORT_NAME             10 (nornir_easy_netmiko.errors)
+                64 IMPORT_FROM             11 (error_handle)
+                66 STORE_NAME              11 (error_handle)
+                68 POP_TOP
    
-     6          46 LOAD_CONST              13 ((False, False))
-                48 LOAD_CONST               5 ('task')
+     7          70 LOAD_NAME               11 (error_handle)
    
-     7          50 LOAD_NAME                4 (Task)
+    11          72 NOP
    
-     6          52 LOAD_CONST               6 ('command_string')
+    12          74 NOP
    
-     8          54 LOAD_NAME                7 (str)
+     8          76 LOAD_CONST              15 ((False, False))
+                78 LOAD_CONST               7 ('task')
    
-     6          56 LOAD_CONST               7 ('use_timing')
+     9          80 LOAD_NAME                7 (Task)
    
-     9          58 LOAD_NAME                8 (bool)
+     8          82 LOAD_CONST               8 ('command_string')
    
-     6          60 LOAD_CONST               8 ('enable')
+    10          84 LOAD_NAME               12 (str)
    
-    10          62 LOAD_NAME                8 (bool)
+     8          86 LOAD_CONST               9 ('use_timing')
    
-     6          64 LOAD_CONST               9 ('kwargs')
+    11          88 LOAD_NAME               13 (bool)
    
-    11          66 LOAD_NAME                1 (Any)
+     8          90 LOAD_CONST              10 ('enable')
    
-     6          68 LOAD_CONST              10 ('return')
+    12          92 LOAD_NAME               13 (bool)
    
-    12          70 LOAD_NAME                3 (Result)
+     8          94 LOAD_CONST              11 ('kwargs')
    
-     6          72 BUILD_TUPLE             12
-                74 LOAD_CONST              11 (<code object netmiko_send_command, file "e:\资料\nornir\nornir_easy_netmiko\tasks\netmiko_send_command.py", line 6>)
-                76 MAKE_FUNCTION            5 (defaults, annotations)
-                78 STORE_NAME               9 (netmiko_send_command)
-                80 LOAD_CONST              12 (None)
-                82 RETURN_VALUE
+    13          96 LOAD_NAME                1 (Any)
+   
+     8          98 LOAD_CONST              12 ('return')
+   
+    14         100 LOAD_NAME                6 (Result)
+   
+     8         102 BUILD_TUPLE             12
+               104 LOAD_CONST              13 (<code object netmiko_send_command, file "E:\资料\nornir_myproject\nornir_easy_netmiko\tasks\netmiko_send_command.py", line 7>)
+               106 MAKE_FUNCTION            5 (defaults, annotations)
+   
+     7         108 PRECALL                  0
+               112 CALL                     0
+   
+     8         122 STORE_NAME              14 (netmiko_send_command)
+               124 LOAD_CONST              14 (None)
+               126 RETURN_VALUE
    consts
       0
       ('Any',)
+      ('Template', 'StrictUndefined')
       ('Result', 'Task')
       ('CONNECTION_NAME',)
+      ('error_handle',)
       False
       'task'
       'command_string'
       'use_timing'
       'enable'
       'kwargs'
       'return'
       code
          argcount  : 4
-         nlocals   : 7
+         nlocals   : 8
          stacksize : 5
          flags     : 11
          code
             0x97007c006a000000000000000000a00100000000000000000000000000
             000000000000007404000000000000000000007c006a0300000000000000
-            006a040000000000000000a6020000ab0200000000000000007d057c0372
-            147c05a0050000000000000000000000000000000000000000a6000000ab
-            00000000000000000001007c02720f02007c056a0600000000000000007c
-            01660169007c04a4018e017d066e0e02007c056a0700000000000000007c
-            01660169007c04a4018e017d067411000000000000000000007c006a0000
-            000000000000007c06ac01a6020000ab0200000000000000005300
-           6           0 RESUME                   0
+            006a040000000000000000a6020000ab0200000000000000007d05740b00
+            0000000000000000007c01740c000000000000000000006401ac02a60300
+            00ab0300000000000000007d067c06a00700000000000000000000000000
+            000000000000007c006a000000000000000000a008000000000000000000
+            0000000000000000000000a6000000ab000000000000000000a6010000ab
+            0100000000000000007d017c0372147c05a0090000000000000000000000
+            000000000000000000a6000000ab00000000000000000001007c02720f02
+            007c056a0a00000000000000007c01660169007c04a4018e017d076e0e02
+            007c056a0b00000000000000007c01660169007c04a4018e017d07741900
+            0000000000000000007c006a0000000000000000007c07ac03a6020000ab
+            0200000000000000005300
+           7           0 RESUME                   0
          
-          26           2 LOAD_FAST                0 (task)
+          28           2 LOAD_FAST                0 (task)
                        4 LOAD_ATTR                0 (host)
                       14 LOAD_METHOD              1 (get_connection)
                       36 LOAD_GLOBAL              4 (CONNECTION_NAME)
                       48 LOAD_FAST                0 (task)
                       50 LOAD_ATTR                3 (nornir)
                       60 LOAD_ATTR                4 (config)
                       70 PRECALL                  2
                       74 CALL                     2
                       84 STORE_FAST               5 (net_connect)
          
-          27          86 LOAD_FAST                3 (enable)
-                      88 POP_JUMP_FORWARD_IF_FALSE    20 (to 130)
-         
-          28          90 LOAD_FAST                5 (net_connect)
-                      92 LOAD_METHOD              5 (enable)
-                     114 PRECALL                  0
-                     118 CALL                     0
-                     128 POP_TOP
-         
-          29     >>  130 LOAD_FAST                2 (use_timing)
-                     132 POP_JUMP_FORWARD_IF_FALSE    15 (to 164)
-         
-          30         134 PUSH_NULL
-                     136 LOAD_FAST                5 (net_connect)
-                     138 LOAD_ATTR                6 (send_command_timing)
-                     148 LOAD_FAST                1 (command_string)
-                     150 BUILD_TUPLE              1
-                     152 BUILD_MAP                0
-                     154 LOAD_FAST                4 (kwargs)
-                     156 DICT_MERGE               1
-                     158 CALL_FUNCTION_EX         1
-                     160 STORE_FAST               6 (result)
-                     162 JUMP_FORWARD            14 (to 192)
-         
-          32     >>  164 PUSH_NULL
-                     166 LOAD_FAST                5 (net_connect)
-                     168 LOAD_ATTR                7 (send_command)
-                     178 LOAD_FAST                1 (command_string)
-                     180 BUILD_TUPLE              1
-                     182 BUILD_MAP                0
-                     184 LOAD_FAST                4 (kwargs)
-                     186 DICT_MERGE               1
-                     188 CALL_FUNCTION_EX         1
-                     190 STORE_FAST               6 (result)
-         
-          33     >>  192 LOAD_GLOBAL             17 (NULL + Result)
-                     204 LOAD_FAST                0 (task)
-                     206 LOAD_ATTR                0 (host)
-                     216 LOAD_FAST                6 (result)
-                     218 KW_NAMES                 1
-                     220 PRECALL                  2
-                     224 CALL                     2
-                     234 RETURN_VALUE
+          30          86 LOAD_GLOBAL             11 (NULL + Template)
+                      98 LOAD_FAST                1 (command_string)
+                     100 LOAD_GLOBAL             12 (StrictUndefined)
+                     112 LOAD_CONST               1 (True)
+                     114 KW_NAMES                 2
+                     116 PRECALL                  3
+                     120 CALL                     3
+                     130 STORE_FAST               6 (template)
+         
+          31         132 LOAD_FAST                6 (template)
+                     134 LOAD_METHOD              7 (render)
+                     156 LOAD_FAST                0 (task)
+                     158 LOAD_ATTR                0 (host)
+                     168 LOAD_METHOD              8 (dict)
+                     190 PRECALL                  0
+                     194 CALL                     0
+                     204 PRECALL                  1
+                     208 CALL                     1
+                     218 STORE_FAST               1 (command_string)
+         
+          33         220 LOAD_FAST                3 (enable)
+                     222 POP_JUMP_FORWARD_IF_FALSE    20 (to 264)
+         
+          34         224 LOAD_FAST                5 (net_connect)
+                     226 LOAD_METHOD              9 (enable)
+                     248 PRECALL                  0
+                     252 CALL                     0
+                     262 POP_TOP
+         
+          35     >>  264 LOAD_FAST                2 (use_timing)
+                     266 POP_JUMP_FORWARD_IF_FALSE    15 (to 298)
+         
+          36         268 PUSH_NULL
+                     270 LOAD_FAST                5 (net_connect)
+                     272 LOAD_ATTR               10 (send_command_timing)
+                     282 LOAD_FAST                1 (command_string)
+                     284 BUILD_TUPLE              1
+                     286 BUILD_MAP                0
+                     288 LOAD_FAST                4 (kwargs)
+                     290 DICT_MERGE               1
+                     292 CALL_FUNCTION_EX         1
+                     294 STORE_FAST               7 (result)
+                     296 JUMP_FORWARD            14 (to 326)
+         
+          38     >>  298 PUSH_NULL
+                     300 LOAD_FAST                5 (net_connect)
+                     302 LOAD_ATTR               11 (send_command)
+                     312 LOAD_FAST                1 (command_string)
+                     314 BUILD_TUPLE              1
+                     316 BUILD_MAP                0
+                     318 LOAD_FAST                4 (kwargs)
+                     320 DICT_MERGE               1
+                     322 CALL_FUNCTION_EX         1
+                     324 STORE_FAST               7 (result)
+         
+          39     >>  326 LOAD_GLOBAL             25 (NULL + Result)
+                     338 LOAD_FAST                0 (task)
+                     340 LOAD_ATTR                0 (host)
+                     350 LOAD_FAST                7 (result)
+                     352 KW_NAMES                 3
+                     354 PRECALL                  2
+                     358 CALL                     2
+                     368 RETURN_VALUE
          consts
             '\n    Execute Netmiko send_command method (or send_command_timing)\n\n    Arguments:\n        command_string: Command to execute on the remote network device.\n        use_timing: Set to True to switch to send_command_timing method.\n        enable: Set to True to force Netmiko .enable() call.\n        kwargs: Additional arguments to pass to send_command method.\n\n    Returns:\n        Result object with the following attributes set:\n          * result: Result of the show command (generally a string, but depends on use of TextFSM).\n    '
+            True
+            ('undefined', 'trim_blocks')
             ('host', 'result')
-         names      ('host', 'get_connection', 'CONNECTION_NAME', 'nornir', 'config', 'enable', 'send_command_timing', 'send_command', 'Result')
-         varnames   ('task', 'command_string', 'use_timing', 'enable', 'kwargs', 'net_connect', 'result')
+         names      ('host', 'get_connection', 'CONNECTION_NAME', 'nornir', 'config', 'Template', 'StrictUndefined', 'render', 'dict', 'enable', 'send_command_timing', 'send_command', 'Result')
+         varnames   ('task', 'command_string', 'use_timing', 'enable', 'kwargs', 'net_connect', 'template', 'result')
          freevars   ()
          cellvars   ()
-         filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_send_command.py'
+         filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_send_command.py'
          name       'netmiko_send_command'
-         firstlineno 6
-         lnotab 0x021454010401280104011e021c01
+         firstlineno 7
+         lnotab 0x021554022e0158020401280104011e021c01
       None
       (False, False)
-   names      ('typing', 'Any', 'nornir.core.task', 'Result', 'Task', 'nornir_easy_netmiko.connections', 'CONNECTION_NAME', 'str', 'bool', 'netmiko_send_command')
+   names      ('typing', 'Any', 'jinja2', 'Template', 'StrictUndefined', 'nornir.core.task', 'Result', 'Task', 'nornir_easy_netmiko.connections', 'CONNECTION_NAME', 'nornir_easy_netmiko.errors', 'error_handle', 'str', 'bool', 'netmiko_send_command')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'e:\\资料\\nornir\\nornir_easy_netmiko\\tasks\\netmiko_send_command.py'
+   filename   'E:\\资料\\nornir_myproject\\nornir_easy_netmiko\\tasks\\netmiko_send_command.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c0110010c06020102fc040102ff020202fe020302fd020402
-      fc020502fb020602fa
+      0x00ff02010c01100110010c010c020204020102fc040102ff020202fe02
+      0302fd020402fc020502fb020602fa06ff0e01
```

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/__pycache__/netmiko_send_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_commit.py` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_commit.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_file_transfer.py` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_file_transfer.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_multiline.py` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_multiline.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_save_config.py` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_save_config.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_send_command.py` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_send_command.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/nornir_easy_netmiko/tasks/netmiko_send_config.py` & `nornir_easy_netmiko-1.1.0/nornir_easy_netmiko/tasks/netmiko_send_config.py`

 * *Files identical despite different names*

### Comparing `nornir_easy_netmiko-1.0.5/pyproject.toml` & `nornir_easy_netmiko-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir_easy_netmiko"
-version = "1.0.5"
+version = "1.1.0"
 description = "Netmiko's plugins for Nornir. Support jinja2 and optimized exception."
 license = "Apache-2.0"
 readme = "README.md"
 authors = ['Des1r3 <linzx@anonymous.com>']
 repository = "https://github.com/Des1r3/nornir_easy_netmiko"
 classifiers = [
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `nornir_easy_netmiko-1.0.5/PKG-INFO` & `nornir_easy_netmiko-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-easy-netmiko
-Version: 1.0.5
+Version: 1.1.0
 Summary: Netmiko's plugins for Nornir. Support jinja2 and optimized exception.
 Home-page: https://github.com/Des1r3/nornir_easy_netmiko
 License: Apache-2.0
 Author: Des1r3
 Author-email: linzx@anonymous.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

