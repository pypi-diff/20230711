# Comparing `tmp/fastapi-config-0.0.7.tar.gz` & `tmp/fastapi-config-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-config-0.0.7.tar", last modified: Sat Mar  4 15:56:32 2023, max compression
+gzip compressed data, was "fastapi-config-0.1.0.tar", last modified: Tue Jul 11 09:32:22 2023, max compression
```

## Comparing `fastapi-config-0.0.7.tar` & `fastapi-config-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      634 2023-03-04 15:55:30.457379 fastapi-config-0.0.7/fastapi_config/__init__.py
--rw-r--r--   0        0        0      782 2022-11-01 03:21:56.458970 fastapi-config-0.0.7/fastapi_config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1262 2023-02-19 02:33:52.552483 fastapi-config-0.0.7/fastapi_config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      741 2022-06-09 08:50:34.271959 fastapi-config-0.0.7/fastapi_config/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2296 2022-10-18 08:05:35.268848 fastapi-config-0.0.7/fastapi_config/__pycache__/admin.cpython-310.pyc
--rw-r--r--   0        0        0     3560 2023-02-19 02:33:52.667418 fastapi-config-0.0.7/fastapi_config/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0     2306 2022-09-05 09:29:24.603752 fastapi-config-0.0.7/fastapi_config/__pycache__/admin.cpython-38.pyc
--rw-r--r--   0        0        0     6356 2022-10-28 13:32:21.776806 fastapi-config-0.0.7/fastapi_config/__pycache__/backends.cpython-310.pyc
--rw-r--r--   0        0        0    12499 2023-02-19 02:33:55.040060 fastapi-config-0.0.7/fastapi_config/__pycache__/backends.cpython-311.pyc
--rw-r--r--   0        0        0     5929 2022-09-05 09:29:24.607751 fastapi-config-0.0.7/fastapi_config/__pycache__/backends.cpython-38.pyc
--rw-r--r--   0        0        0     1154 2022-10-18 10:55:39.532279 fastapi-config-0.0.7/fastapi_config/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0     1782 2023-02-19 02:33:55.046056 fastapi-config-0.0.7/fastapi_config/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     1211 2022-09-05 09:29:24.613748 fastapi-config-0.0.7/fastapi_config/__pycache__/models.cpython-38.pyc
--rw-r--r--   0        0        0     1397 2022-10-18 08:04:30.997929 fastapi-config-0.0.7/fastapi_config/admin.py
--rw-r--r--   0        0        0     5874 2022-10-28 13:32:14.500158 fastapi-config-0.0.7/fastapi_config/backends.py
--rw-r--r--   0        0        0      817 2022-06-09 03:34:17.003719 fastapi-config-0.0.7/fastapi_config/locale/base.pot
--rw-r--r--   0        0        0      638 2022-10-19 03:28:59.990259 fastapi-config-0.0.7/fastapi_config/locale/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      985 2022-10-19 03:28:59.990259 fastapi-config-0.0.7/fastapi_config/locale/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      620 2022-10-19 03:28:59.992242 fastapi-config-0.0.7/fastapi_config/locale/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      930 2022-06-09 03:34:17.012714 fastapi-config-0.0.7/fastapi_config/locale/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      744 2022-10-18 10:55:12.342781 fastapi-config-0.0.7/fastapi_config/models.py
--rw-r--r--   0        0        0     1871 2023-03-03 14:20:26.728096 fastapi-config-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3128 2022-10-19 03:35:12.706229 fastapi-config-0.0.7/README.md
--rw-r--r--   0        0        0       39 2022-06-09 04:05:48.168639 fastapi-config-0.0.7/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2022-06-09 04:05:48.169636 fastapi-config-0.0.7/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      303 2022-06-09 04:05:48.167636 fastapi-config-0.0.7/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2022-06-09 07:19:39.527714 fastapi-config-0.0.7/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      295 2022-09-23 08:24:02.275552 fastapi-config-0.0.7/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-09-23 08:24:02.276556 fastapi-config-0.0.7/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2022-06-09 03:56:09.908766 fastapi-config-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0    12288 2023-02-19 02:33:55.671700 fastapi-config-0.0.7/tests/amisadmin.db
--rw-r--r--   0        0        0      800 2022-10-28 13:32:14.296273 fastapi-config-0.0.7/tests/conftest.py
--rw-r--r--   0        0        0     1426 2022-10-28 09:37:49.010537 fastapi-config-0.0.7/tests/test_DbConfigStore.py
--rw-r--r--   0        0        0     4025 1970-01-01 00:00:00.000000 fastapi-config-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      634 2023-07-11 09:29:29.117238 fastapi-config-0.1.0/fastapi_config/__init__.py
+-rw-r--r--   0        0        0      782 2022-11-01 03:21:56.458970 fastapi-config-0.1.0/fastapi_config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1262 2023-07-11 09:28:42.881368 fastapi-config-0.1.0/fastapi_config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      741 2022-06-09 08:50:34.271959 fastapi-config-0.1.0/fastapi_config/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2296 2022-10-18 08:05:35.268848 fastapi-config-0.1.0/fastapi_config/__pycache__/admin.cpython-310.pyc
+-rw-r--r--   0        0        0     3663 2023-07-11 09:28:42.913364 fastapi-config-0.1.0/fastapi_config/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0     2306 2022-09-05 09:29:24.603752 fastapi-config-0.1.0/fastapi_config/__pycache__/admin.cpython-38.pyc
+-rw-r--r--   0        0        0     6356 2022-10-28 13:32:21.776806 fastapi-config-0.1.0/fastapi_config/__pycache__/backends.cpython-310.pyc
+-rw-r--r--   0        0        0    12499 2023-07-11 09:14:38.487832 fastapi-config-0.1.0/fastapi_config/__pycache__/backends.cpython-311.pyc
+-rw-r--r--   0        0        0     5929 2022-09-05 09:29:24.607751 fastapi-config-0.1.0/fastapi_config/__pycache__/backends.cpython-38.pyc
+-rw-r--r--   0        0        0     1154 2022-10-18 10:55:39.532279 fastapi-config-0.1.0/fastapi_config/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0        0        0     2311 2023-07-11 09:28:44.586347 fastapi-config-0.1.0/fastapi_config/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     1211 2022-09-05 09:29:24.613748 fastapi-config-0.1.0/fastapi_config/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0        0        0     1490 2023-07-11 09:27:57.191148 fastapi-config-0.1.0/fastapi_config/admin.py
+-rw-r--r--   0        0        0     6035 2023-07-11 09:11:37.628968 fastapi-config-0.1.0/fastapi_config/backends.py
+-rw-r--r--   0        0        0      879 2023-07-11 09:21:03.349260 fastapi-config-0.1.0/fastapi_config/locale/base.pot
+-rw-r--r--   0        0        0      730 2023-07-11 09:25:23.827140 fastapi-config-0.1.0/fastapi_config/locale/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     1087 2023-07-11 09:22:29.921434 fastapi-config-0.1.0/fastapi_config/locale/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      702 2023-07-11 09:25:23.832137 fastapi-config-0.1.0/fastapi_config/locale/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     1016 2023-07-11 09:21:26.013287 fastapi-config-0.1.0/fastapi_config/locale/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1083 2023-07-11 09:28:14.837608 fastapi-config-0.1.0/fastapi_config/models.py
+-rw-r--r--   0        0        0     1864 2023-07-11 09:14:35.873489 fastapi-config-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3128 2022-10-19 03:35:12.706229 fastapi-config-0.1.0/README.md
+-rw-r--r--   0        0        0       39 2022-06-09 04:05:48.168639 fastapi-config-0.1.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2022-06-09 04:05:48.169636 fastapi-config-0.1.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      303 2022-06-09 04:05:48.167636 fastapi-config-0.1.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2022-06-09 07:19:39.527714 fastapi-config-0.1.0/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      295 2022-09-23 08:24:02.275552 fastapi-config-0.1.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-09-23 08:24:02.276556 fastapi-config-0.1.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2022-06-09 03:56:09.908766 fastapi-config-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    12288 2023-07-11 09:28:45.219956 fastapi-config-0.1.0/tests/amisadmin.db
+-rw-r--r--   0        0        0      800 2022-10-28 13:32:14.296273 fastapi-config-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1426 2022-10-28 09:37:49.010537 fastapi-config-0.1.0/tests/test_DbConfigStore.py
+-rw-r--r--   0        0        0     4025 1970-01-01 00:00:00.000000 fastapi-config-0.1.0/PKG-INFO
```

### Comparing `fastapi-config-0.0.7/fastapi_config/__init__.py` & `fastapi-config-0.1.0/fastapi_config/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.7"
+__version__ = "0.1.0"
 __url__ = "https://github.com/amisadmin/fastapi_config"
 
 import gettext
 import os
 
 from fastapi_amis_admin import i18n
```

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/__init__.cpython-310.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/__init__.cpython-311.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/__init__.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x82906063 (Tue Nov  1 03:20:34 2022 UTC)
+moddate:  0xbf20ad64 (Tue Jul 11 09:28:31 2023 UTC)
 files sz: 634
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
@@ -19,15 +19,15 @@
       0d0000000000000000000000000000000000000000650a6406a6020000ab
       02000000000000000064096701ac08a6030000ab03000000000000000064
       0a9c02a6010000ab0100000000000000000100640b640c6c0e6d0f5a0f6d
       105a100100640b640d6c116d125a126d135a130100640b640e6c146d155a
       15010064035300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('0.0.6')
+     1           2 LOAD_CONST               0 ('0.0.8')
                  4 STORE_NAME               0 (__version__)
    
      2           6 LOAD_CONST               1 ('https://github.com/amisadmin/fastapi_config')
                  8 STORE_NAME               1 (__url__)
    
      4          10 LOAD_CONST               2 (0)
                 12 LOAD_CONST               3 (None)
@@ -127,15 +127,15 @@
                384 IMPORT_NAME             20 (models)
                386 IMPORT_FROM             21 (ConfigModel)
                388 STORE_NAME              21 (ConfigModel)
                390 POP_TOP
                392 LOAD_CONST               3 (None)
                394 RETURN_VALUE
    consts
-      '0.0.6'
+      '0.0.8'
       'https://github.com/amisadmin/fastapi_config'
       0
       None
       ('i18n',)
       'messages'
       'locale'
       'zh_CN'
```

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/__init__.cpython-38.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/admin.cpython-310.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/admin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/admin.cpython-311.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/admin.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x0e5e4e63 (Tue Oct 18 08:04:30 2022 UTC)
-files sz: 1397
+moddate:  0x9d20ad64 (Tue Jul 11 09:27:57 2023 UTC)
+files sz: 1490
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -100,17 +100,17 @@
                142 LOAD_CONST              13 ('ConfigModelAdmin')
                144 LOAD_NAME                3 (admin)
                146 LOAD_ATTR               24 (ModelAdmin)
                156 PRECALL                  3
                160 CALL                     3
                170 STORE_NAME              25 (ConfigModelAdmin)
    
-    21         172 PUSH_NULL
+    22         172 PUSH_NULL
                174 LOAD_BUILD_CLASS
-               176 LOAD_CONST              14 (<code object ConfigAdmin, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\admin.py", line 21>)
+               176 LOAD_CONST              14 (<code object ConfigAdmin, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\admin.py", line 22>)
                178 MAKE_FUNCTION            0
                180 LOAD_CONST              15 ('ConfigAdmin')
                182 LOAD_NAME                3 (admin)
                184 LOAD_ATTR               26 (FormAdmin)
                194 PRECALL                  3
                198 CALL                     3
                208 STORE_NAME              27 (ConfigAdmin)
@@ -132,16 +132,16 @@
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0202006503020065046401a6010000ab01000000
-            00000000006402ac03a6020000ab0200000000000000005a0565065a0764
-            0467015a0864055300
+            00000000006402ac03a6020000ab0200000000000000005a0565065a0768
+            006404a3015a0868006405a3015a0964065300
           15           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ConfigModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
           16          10 PUSH_NULL
@@ -156,34 +156,41 @@
                       38 PRECALL                  2
                       42 CALL                     2
                       52 STORE_NAME               5 (page_schema)
          
           17          54 LOAD_NAME                6 (ConfigModel)
                       56 STORE_NAME               7 (model)
          
-          18          58 LOAD_CONST               4 ('key')
-                      60 BUILD_LIST               1
-                      62 STORE_NAME               8 (readonly_fields)
-                      64 LOAD_CONST               5 (None)
-                      66 RETURN_VALUE
+          18          58 BUILD_SET                0
+                      60 LOAD_CONST               4 (frozenset({'update_time', 'id', 'create_time'}))
+                      62 SET_UPDATE               1
+                      64 STORE_NAME               8 (create_exclude)
+         
+          19          66 BUILD_SET                0
+                      68 LOAD_CONST               5 (frozenset({'update_time', 'create_time', 'id', 'key'}))
+                      70 SET_UPDATE               1
+                      72 STORE_NAME               9 (update_exclude)
+                      74 LOAD_CONST               6 (None)
+                      76 RETURN_VALUE
          consts
             'ConfigModelAdmin'
             'Configuration'
             'fa fa-cog'
             ('label', 'icon')
-            'key'
+            frozenset({'update_time', 'id', 'create_time'})
+            frozenset({'update_time', 'create_time', 'id', 'key'})
             None
-         names      ('__name__', '__module__', '__qualname__', 'PageSchema', '_', 'page_schema', 'ConfigModel', 'model', 'readonly_fields')
+         names      ('__name__', '__module__', '__qualname__', 'PageSchema', '_', 'page_schema', 'ConfigModel', 'model', 'create_exclude', 'update_exclude')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'I:\\Python\\Project\\WWW\\fastapi-amis-admin\\fastapi_config\\fastapi_config\\admin.py'
          name       'ConfigModelAdmin'
          firstlineno 15
-         lnotab 0x0a012c010401
+         lnotab 0x0a012c0104010801
       'ConfigModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
@@ -192,85 +199,85 @@
             000000ac06a6010000ab0100000000000000005a0c641088006601640984
             0c5a0d650e640a8400a6000000ab0000000000000000005a0f640b651064
             0c6511640d65126513190000000000000000006606640e84045a14640b65
             10640d65126513190000000000000000006604640f84045a15880078015a
             165300
                        0 MAKE_CELL                0 (__class__)
          
-          21           2 RESUME                   0
+          22           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('ConfigAdmin')
                       10 STORE_NAME               2 (__qualname__)
                       12 SETUP_ANNOTATIONS
          
-          22          14 LOAD_CONST               1 ('/config')
+          23          14 LOAD_CONST               1 ('/config')
                       16 STORE_NAME               3 (router_prefix)
                       18 LOAD_NAME                4 (str)
                       20 LOAD_NAME                5 (__annotations__)
                       22 LOAD_CONST               2 ('router_prefix')
                       24 STORE_SUBSCR
          
-          23          28 LOAD_CONST               3 (None)
+          24          28 LOAD_CONST               3 (None)
                       30 STORE_NAME               6 (config_store)
                       32 LOAD_NAME                7 (BaseConfigStore)
                       34 LOAD_NAME                5 (__annotations__)
                       36 LOAD_CONST               4 ('config_store')
                       38 STORE_SUBSCR
          
-          24          42 LOAD_CONST               5 (True)
+          25          42 LOAD_CONST               5 (True)
                       44 STORE_NAME               8 (form_init)
          
-          25          46 PUSH_NULL
+          26          46 PUSH_NULL
                       48 LOAD_NAME                9 (Form)
                       50 LOAD_NAME               10 (DisplayModeEnum)
                       52 LOAD_ATTR               11 (horizontal)
                       62 KW_NAMES                 6
                       64 PRECALL                  1
                       68 CALL                     1
                       78 STORE_NAME              12 (form)
          
-          27          80 LOAD_CONST              16 (('app', 'AdminApp'))
+          28          80 LOAD_CONST              16 (('app', 'AdminApp'))
                       82 LOAD_CLOSURE             0 (__class__)
                       84 BUILD_TUPLE              1
-                      86 LOAD_CONST               9 (<code object __init__, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\admin.py", line 27>)
+                      86 LOAD_CONST               9 (<code object __init__, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\admin.py", line 28>)
                       88 MAKE_FUNCTION           12 (annotations, closure)
                       90 STORE_NAME              13 (__init__)
          
-          31          92 LOAD_NAME               14 (property)
+          32          92 LOAD_NAME               14 (property)
          
-          32          94 LOAD_CONST              10 (<code object page_path, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\admin.py", line 31>)
+          33          94 LOAD_CONST              10 (<code object page_path, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\admin.py", line 32>)
                       96 MAKE_FUNCTION            0
          
-          31          98 PRECALL                  0
+          32          98 PRECALL                  0
                      102 CALL                     0
          
-          32         112 STORE_NAME              15 (page_path)
+          33         112 STORE_NAME              15 (page_path)
          
-          35         114 LOAD_CONST              11 ('request')
+          36         114 LOAD_CONST              11 ('request')
                      116 LOAD_NAME               16 (Request)
                      118 LOAD_CONST              12 ('data')
                      120 LOAD_NAME               17 (BaseModel)
                      122 LOAD_CONST              13 ('return')
                      124 LOAD_NAME               18 (BaseApiOut)
                      126 LOAD_NAME               19 (Any)
                      128 BINARY_SUBSCR
                      138 BUILD_TUPLE              6
-                     140 LOAD_CONST              14 (<code object handle, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\admin.py", line 35>)
+                     140 LOAD_CONST              14 (<code object handle, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\admin.py", line 36>)
                      142 MAKE_FUNCTION            4 (annotations)
                      144 STORE_NAME              20 (handle)
          
-          38         146 LOAD_CONST              11 ('request')
+          39         146 LOAD_CONST              11 ('request')
                      148 LOAD_NAME               16 (Request)
                      150 LOAD_CONST              13 ('return')
                      152 LOAD_NAME               18 (BaseApiOut)
                      154 LOAD_NAME               19 (Any)
                      156 BINARY_SUBSCR
                      166 BUILD_TUPLE              4
-                     168 LOAD_CONST              15 (<code object get_init_data, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\admin.py", line 38>)
+                     168 LOAD_CONST              15 (<code object get_init_data, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\admin.py", line 39>)
                      170 MAKE_FUNCTION            4 (annotations)
                      172 STORE_NAME              21 (get_init_data)
                      174 LOAD_CLOSURE             0 (__class__)
                      176 COPY                     1
                      178 STORE_NAME              22 (__classcell__)
                      180 RETURN_VALUE
          consts
@@ -293,26 +300,26 @@
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   01000000000000000001007c006a02000000000000000070197407000000
                   000000000000007c006a0400000000000000006a050000000000000000ac
                   01a6010000ab0100000000000000007c005f020000000000000000640053
                   00
                              0 COPY_FREE_VARS           1
                
-                27           2 RESUME                   0
+                28           2 RESUME                   0
                
-                28           4 LOAD_GLOBAL              1 (NULL + super)
+                29           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__init__)
                             52 LOAD_FAST                1 (app)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 POP_TOP
                
-                29          70 LOAD_FAST                0 (self)
+                30          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                2 (config_store)
                             82 JUMP_IF_TRUE_OR_POP     25 (to 134)
                             84 LOAD_GLOBAL              7 (NULL + DbConfigStore)
                             96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                4 (site)
                            108 LOAD_ATTR                5 (db)
                            118 KW_NAMES                 1
@@ -327,29 +334,29 @@
                   ('db',)
                names      ('super', '__init__', 'config_store', 'DbConfigStore', 'site', 'db')
                varnames   ('self', 'app')
                freevars   ('__class__',)
                cellvars   ()
                filename   'I:\\Python\\Project\\WWW\\fastapi-amis-admin\\fastapi_config\\fastapi_config\\admin.py'
                name       '__init__'
-               firstlineno 27
+               firstlineno 28
                lnotab 0x04014201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
                   0x970064017401000000000000000000007c006a01000000000000000064
                   027c006a0100000000000000006a020000000000000000a6030000ab0300
                   00000000000000a0030000000000000000000000000000000000000000a6
                   000000ab0000000000000000009b009d025300
-                31           0 RESUME                   0
+                32           0 RESUME                   0
                
-                33           2 LOAD_CONST               1 ('/')
+                34           2 LOAD_CONST               1 ('/')
                              4 LOAD_GLOBAL              1 (NULL + getattr)
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (schema)
                             28 LOAD_CONST               2 ('__key__')
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                1 (schema)
                             42 LOAD_ATTR                2 (__name__)
@@ -367,34 +374,34 @@
                   '__key__'
                names      ('getattr', 'schema', '__name__', 'lower')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'I:\\Python\\Project\\WWW\\fastapi-amis-admin\\fastapi_config\\fastapi_config\\admin.py'
                name       'page_path'
-               firstlineno 31
+               firstlineno 32
                lnotab 0x0202
             'request'
             'data'
             'return'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 5
                flags     : 139
                code
                   0x4b00010097007401000000000000000000007c006a0100000000000000
                   00a00200000000000000000000000000000000000000007c02a6010000ab
                   010000000000000000830064007b03560097038604ac01a6010000ab0100
                   000000000000005300
-                35           0 RETURN_GENERATOR
+                36           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                36           6 LOAD_GLOBAL              1 (NULL + BaseApiOut)
+                37           6 LOAD_GLOBAL              1 (NULL + BaseApiOut)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (config_store)
                             30 LOAD_METHOD              2 (set)
                             52 LOAD_FAST                2 (data)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 GET_AWAITABLE            0
@@ -412,31 +419,31 @@
                   ('data',)
                names      ('BaseApiOut', 'config_store', 'set')
                varnames   ('self', 'request', 'data', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'I:\\Python\\Project\\WWW\\fastapi-amis-admin\\fastapi_config\\fastapi_config\\admin.py'
                name       'handle'
-               firstlineno 35
+               firstlineno 36
                lnotab 0x0601
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
                flags     : 139
                code
                   0x4b00010097007401000000000000000000007c006a0100000000000000
                   00a00200000000000000000000000000000000000000007c006a03000000
                   00000000006401ac02a6020000ab020000000000000000830064007b0356
                   0097038604ac03a6010000ab0100000000000000005300
-                38           0 RETURN_GENERATOR
+                39           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                39           6 LOAD_GLOBAL              1 (NULL + BaseApiOut)
+                40           6 LOAD_GLOBAL              1 (NULL + BaseApiOut)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (config_store)
                             30 LOAD_METHOD              2 (get)
                             52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (schema)
                             64 LOAD_CONST               1 (False)
                             66 KW_NAMES                 2
@@ -459,28 +466,28 @@
                   ('data',)
                names      ('BaseApiOut', 'config_store', 'get', 'schema')
                varnames   ('self', 'request', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'I:\\Python\\Project\\WWW\\fastapi-amis-admin\\fastapi_config\\fastapi_config\\admin.py'
                name       'get_init_data'
-               firstlineno 38
+               firstlineno 39
                lnotab 0x0601
             ('app', 'AdminApp')
          names      ('__name__', '__module__', '__qualname__', 'router_prefix', 'str', '__annotations__', 'config_store', 'BaseConfigStore', 'form_init', 'Form', 'DisplayModeEnum', 'horizontal', 'form', '__init__', 'property', 'page_path', 'Request', 'BaseModel', 'BaseApiOut', 'Any', 'handle', 'get_init_data', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'I:\\Python\\Project\\WWW\\fastapi-amis-admin\\fastapi_config\\fastapi_config\\admin.py'
          name       'ConfigAdmin'
-         firstlineno 21
+         firstlineno 22
          lnotab 0x0e010e010e01040122020c04020104ff0e0102032003
       'ConfigAdmin'
       None
    names      ('typing', 'Any', 'fastapi_amis_admin', 'admin', 'fastapi_amis_admin.admin', 'AdminApp', 'fastapi_amis_admin.amis', 'DisplayModeEnum', 'Form', 'PageSchema', 'fastapi_amis_admin.crud', 'BaseApiOut', 'fastapi_amis_admin.utils.translation', 'i18n', '_', 'pydantic', 'BaseModel', 'starlette.requests', 'Request', 'backends', 'BaseConfigStore', 'DbConfigStore', 'models', 'ConfigModel', 'ModelAdmin', 'ConfigModelAdmin', 'FormAdmin', 'ConfigAdmin')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'I:\\Python\\Project\\WWW\\fastapi-amis-admin\\fastapi_config\\fastapi_config\\admin.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c020c010c0114010c010c010c010c0210010c032606
+   lnotab 0x00ff02010c020c010c0114010c010c010c010c0210010c032607
```

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/admin.cpython-38.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/admin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/backends.cpython-310.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/backends.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/backends.cpython-311.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/backends.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xded95b63 (Fri Oct 28 13:32:14 2022 UTC)
-files sz: 5874
+moddate:  0xc91cad64 (Tue Jul 11 09:11:37 2023 UTC)
+files sz: 6035
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a046d055a056d
```

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/backends.cpython-38.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/backends.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/models.cpython-310.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/models.cpython-311.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/models.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,78 +1,88 @@
 magic:    0xa70d0d0a
-moddate:  0x10864e63 (Tue Oct 18 10:55:12 2022 UTC)
-files sz: 744
+moddate:  0xae20ad64 (Tue Jul 11 09:28:14 2023 UTC)
+files sz: 1083
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c046d055a060100640064046c076d085a086d095a090100640064056c
-      0a6d0b5a0b010002004700640684006407650b6408ac09a6040000ab0400
-      000000000000005a0c640a5300
+      0x9700640064016c006d005a000100640064026c016d025a020100640064
+      036c036d045a040100640064046c056d065a070100640064056c086d095a
+      096d0a5a0a6d0b5a0b0100640064066c0c6d0d5a0d010002004700640784
+      006408650d6409ac0aa6040000ab0400000000000000005a0e640b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('amis',))
-                 6 IMPORT_NAME              0 (fastapi_amis_admin)
-                 8 IMPORT_FROM              1 (amis)
-                10 STORE_NAME               1 (amis)
+                 4 LOAD_CONST               1 (('datetime',))
+                 6 IMPORT_NAME              0 (datetime)
+                 8 IMPORT_FROM              0 (datetime)
+                10 STORE_NAME               0 (datetime)
                 12 POP_TOP
    
-     2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('Field',))
-                18 IMPORT_NAME              2 (fastapi_amis_admin.models)
-                20 IMPORT_FROM              3 (Field)
-                22 STORE_NAME               3 (Field)
+     3          14 LOAD_CONST               0 (0)
+                16 LOAD_CONST               2 (('amis',))
+                18 IMPORT_NAME              1 (fastapi_amis_admin)
+                20 IMPORT_FROM              2 (amis)
+                22 STORE_NAME               2 (amis)
                 24 POP_TOP
    
-     3          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               3 (('i18n',))
-                30 IMPORT_NAME              4 (fastapi_amis_admin.utils.translation)
-                32 IMPORT_FROM              5 (i18n)
-                34 STORE_NAME               6 (_)
+     4          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               3 (('Field',))
+                30 IMPORT_NAME              3 (fastapi_amis_admin.models)
+                32 IMPORT_FROM              4 (Field)
+                34 STORE_NAME               4 (Field)
                 36 POP_TOP
    
-     4          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               4 (('Column', 'Text'))
-                42 IMPORT_NAME              7 (sqlalchemy)
-                44 IMPORT_FROM              8 (Column)
-                46 STORE_NAME               8 (Column)
-                48 IMPORT_FROM              9 (Text)
-                50 STORE_NAME               9 (Text)
-                52 POP_TOP
-   
-     5          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               5 (('SQLModel',))
-                58 IMPORT_NAME             10 (sqlmodel)
-                60 IMPORT_FROM             11 (SQLModel)
-                62 STORE_NAME              11 (SQLModel)
-                64 POP_TOP
-   
-     8          66 PUSH_NULL
-                68 LOAD_BUILD_CLASS
-                70 LOAD_CONST               6 (<code object ConfigModel, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\models.py", line 8>)
-                72 MAKE_FUNCTION            0
-                74 LOAD_CONST               7 ('ConfigModel')
-                76 LOAD_NAME               11 (SQLModel)
-                78 LOAD_CONST               8 (True)
-                80 KW_NAMES                 9
-                82 PRECALL                  4
-                86 CALL                     4
-                96 STORE_NAME              12 (ConfigModel)
-                98 LOAD_CONST              10 (None)
-               100 RETURN_VALUE
+     5          38 LOAD_CONST               0 (0)
+                40 LOAD_CONST               4 (('i18n',))
+                42 IMPORT_NAME              5 (fastapi_amis_admin.utils.translation)
+                44 IMPORT_FROM              6 (i18n)
+                46 STORE_NAME               7 (_)
+                48 POP_TOP
+   
+     6          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               5 (('Column', 'Text', 'func'))
+                54 IMPORT_NAME              8 (sqlalchemy)
+                56 IMPORT_FROM              9 (Column)
+                58 STORE_NAME               9 (Column)
+                60 IMPORT_FROM             10 (Text)
+                62 STORE_NAME              10 (Text)
+                64 IMPORT_FROM             11 (func)
+                66 STORE_NAME              11 (func)
+                68 POP_TOP
+   
+     7          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               6 (('SQLModel',))
+                74 IMPORT_NAME             12 (sqlmodel)
+                76 IMPORT_FROM             13 (SQLModel)
+                78 STORE_NAME              13 (SQLModel)
+                80 POP_TOP
+   
+    10          82 PUSH_NULL
+                84 LOAD_BUILD_CLASS
+                86 LOAD_CONST               7 (<code object ConfigModel, file "I:\Python\Project\WWW\fastapi-amis-admin\fastapi_config\fastapi_config\models.py", line 10>)
+                88 MAKE_FUNCTION            0
+                90 LOAD_CONST               8 ('ConfigModel')
+                92 LOAD_NAME               13 (SQLModel)
+                94 LOAD_CONST               9 (True)
+                96 KW_NAMES                10
+                98 PRECALL                  4
+               102 CALL                     4
+               112 STORE_NAME              14 (ConfigModel)
+               114 LOAD_CONST              11 (None)
+               116 RETURN_VALUE
    consts
       0
+      ('datetime',)
       ('amis',)
       ('Field',)
       ('i18n',)
-      ('Column', 'Text')
+      ('Column', 'Text', 'func')
       ('SQLModel',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 8
          flags     : 0
          code
@@ -83,40 +93,46 @@
             04640702006508640ca6010000ab0100000000000000006409ac0da60300
             00ab0300000000000000005a0b650a6507640e3c00000002006504640f02
             0065086410a6010000ab01000000000000000064116412ac13a6040000ab
             0400000000000000005a0c650a650764143c000000020065046407020065
             086415a6010000ab0100000000000000000200650d650e6404ac16a60200
             00ab0200000000000000000200650f6a1000000000000000006417ac18a6
             010000ab010000000000000000ac19a6040000ab0400000000000000005a
-            11650a6507641a3c00000064025300
-           8           0 RESUME                   0
+            11650a6507641a3c0000000200650465126a130000000000000000020065
+            08641ba6010000ab010000000000000000ac1ca6020000ab020000000000
+            0000005a1465126507641d3c0000000200650465126a1300000000000000
+            0002006508641ea6010000ab010000000000000000020065156a13000000
+            0000000000a6000000ab000000000000000000020065156a130000000000
+            000000a6000000ab000000000000000000641f9c02ac20a6030000ab0300
+            000000000000005a166512650764213c00000064025300
+          10           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ConfigModel')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-           9          12 LOAD_CONST               1 ('system_config')
+          11          12 LOAD_CONST               1 ('system_config')
                       14 STORE_NAME               3 (__tablename__)
          
-          10          16 PUSH_NULL
+          12          16 PUSH_NULL
                       18 LOAD_NAME                4 (Field)
                       20 LOAD_CONST               2 (None)
                       22 LOAD_CONST               3 (True)
                       24 LOAD_CONST               4 (False)
                       26 KW_NAMES                 5
                       28 PRECALL                  3
                       32 CALL                     3
                       42 STORE_NAME               5 (id)
                       44 LOAD_NAME                6 (int)
                       46 LOAD_NAME                7 (__annotations__)
                       48 LOAD_CONST               6 ('id')
                       50 STORE_SUBSCR
          
-          11          54 PUSH_NULL
+          13          54 PUSH_NULL
                       56 LOAD_NAME                4 (Field)
                       58 LOAD_CONST               7 (Ellipsis)
                       60 PUSH_NULL
                       62 LOAD_NAME                8 (_)
                       64 LOAD_CONST               8 ('Identify')
                       66 PRECALL                  1
                       70 CALL                     1
@@ -129,15 +145,15 @@
                       94 CALL                     6
                      104 STORE_NAME               9 (key)
                      106 LOAD_NAME               10 (str)
                      108 LOAD_NAME                7 (__annotations__)
                      110 LOAD_CONST              11 ('key')
                      112 STORE_SUBSCR
          
-          12         116 PUSH_NULL
+          14         116 PUSH_NULL
                      118 LOAD_NAME                4 (Field)
                      120 LOAD_CONST               7 (Ellipsis)
                      122 PUSH_NULL
                      124 LOAD_NAME                8 (_)
                      126 LOAD_CONST              12 ('Name')
                      128 PRECALL                  1
                      132 CALL                     1
@@ -147,15 +163,15 @@
                      150 CALL                     3
                      160 STORE_NAME              11 (name)
                      162 LOAD_NAME               10 (str)
                      164 LOAD_NAME                7 (__annotations__)
                      166 LOAD_CONST              14 ('name')
                      168 STORE_SUBSCR
          
-          13         172 PUSH_NULL
+          15         172 PUSH_NULL
                      174 LOAD_NAME                4 (Field)
                      176 LOAD_CONST              15 ('')
                      178 PUSH_NULL
                      180 LOAD_NAME                8 (_)
                      182 LOAD_CONST              16 ('Description')
                      184 PRECALL                  1
                      188 CALL                     1
@@ -166,15 +182,15 @@
                      208 CALL                     4
                      218 STORE_NAME              12 (desc)
                      220 LOAD_NAME               10 (str)
                      222 LOAD_NAME                7 (__annotations__)
                      224 LOAD_CONST              20 ('desc')
                      226 STORE_SUBSCR
          
-          14         230 PUSH_NULL
+          16         230 PUSH_NULL
                      232 LOAD_NAME                4 (Field)
                      234 LOAD_CONST               7 (Ellipsis)
                      236 PUSH_NULL
                      238 LOAD_NAME                8 (_)
                      240 LOAD_CONST              21 ('Data')
                      242 PRECALL                  1
                      246 CALL                     1
@@ -196,16 +212,68 @@
                      314 PRECALL                  4
                      318 CALL                     4
                      328 STORE_NAME              17 (data)
                      330 LOAD_NAME               10 (str)
                      332 LOAD_NAME                7 (__annotations__)
                      334 LOAD_CONST              26 ('data')
                      336 STORE_SUBSCR
-                     340 LOAD_CONST               2 (None)
-                     342 RETURN_VALUE
+         
+          17         340 PUSH_NULL
+                     342 LOAD_NAME                4 (Field)
+                     344 LOAD_NAME               18 (datetime)
+                     346 LOAD_ATTR               19 (now)
+                     356 PUSH_NULL
+                     358 LOAD_NAME                8 (_)
+                     360 LOAD_CONST              27 ('Create Time')
+                     362 PRECALL                  1
+                     366 CALL                     1
+                     376 KW_NAMES                28
+                     378 PRECALL                  2
+                     382 CALL                     2
+                     392 STORE_NAME              20 (create_time)
+                     394 LOAD_NAME               18 (datetime)
+                     396 LOAD_NAME                7 (__annotations__)
+                     398 LOAD_CONST              29 ('create_time')
+                     400 STORE_SUBSCR
+         
+          18         404 PUSH_NULL
+                     406 LOAD_NAME                4 (Field)
+         
+          19         408 LOAD_NAME               18 (datetime)
+                     410 LOAD_ATTR               19 (now)
+         
+          20         420 PUSH_NULL
+                     422 LOAD_NAME                8 (_)
+                     424 LOAD_CONST              30 ('Update Time')
+                     426 PRECALL                  1
+                     430 CALL                     1
+         
+          21         440 PUSH_NULL
+                     442 LOAD_NAME               21 (func)
+                     444 LOAD_ATTR               19 (now)
+                     454 PRECALL                  0
+                     458 CALL                     0
+                     468 PUSH_NULL
+                     470 LOAD_NAME               21 (func)
+                     472 LOAD_ATTR               19 (now)
+                     482 PRECALL                  0
+                     486 CALL                     0
+                     496 LOAD_CONST              31 (('onupdate', 'server_default'))
+                     498 BUILD_CONST_KEY_MAP      2
+         
+          18         500 KW_NAMES                32
+                     502 PRECALL                  3
+                     506 CALL                     3
+                     516 STORE_NAME              22 (update_time)
+                     518 LOAD_NAME               18 (datetime)
+                     520 LOAD_NAME                7 (__annotations__)
+                     522 LOAD_CONST              33 ('update_time')
+                     524 STORE_SUBSCR
+                     528 LOAD_CONST               2 (None)
+                     530 RETURN_VALUE
          consts
             'ConfigModel'
             'system_config'
             None
             True
             False
             ('default', 'primary_key', 'nullable')
@@ -226,27 +294,34 @@
             'desc'
             'Data'
             ('nullable',)
             'json'
             ('language',)
             ('title', 'sa_column', 'amis_form_item')
             'data'
-         names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Field', 'id', 'int', '__annotations__', '_', 'key', 'str', 'name', 'desc', 'Column', 'Text', 'amis', 'Editor', 'data')
+            'Create Time'
+            ('default_factory', 'title')
+            'create_time'
+            'Update Time'
+            ('onupdate', 'server_default')
+            ('default_factory', 'title', 'sa_column_kwargs')
+            'update_time'
+         names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Field', 'id', 'int', '__annotations__', '_', 'key', 'str', 'name', 'desc', 'Column', 'Text', 'amis', 'Editor', 'data', 'datetime', 'now', 'create_time', 'func', 'update_time')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'I:\\Python\\Project\\WWW\\fastapi-amis-admin\\fastapi_config\\fastapi_config\\models.py'
          name       'ConfigModel'
-         firstlineno 8
-         lnotab 0x0c01040126013e0138013a01
+         firstlineno 10
+         lnotab 0x0c01040126013e0138013a016e01400104010c0114013cfd
       'ConfigModel'
       True
       ('table',)
       None
-   names      ('fastapi_amis_admin', 'amis', 'fastapi_amis_admin.models', 'Field', 'fastapi_amis_admin.utils.translation', 'i18n', '_', 'sqlalchemy', 'Column', 'Text', 'sqlmodel', 'SQLModel', 'ConfigModel')
+   names      ('datetime', 'fastapi_amis_admin', 'amis', 'fastapi_amis_admin.models', 'Field', 'fastapi_amis_admin.utils.translation', 'i18n', '_', 'sqlalchemy', 'Column', 'Text', 'func', 'sqlmodel', 'SQLModel', 'ConfigModel')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'I:\\Python\\Project\\WWW\\fastapi-amis-admin\\fastapi_config\\fastapi_config\\models.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c010c0110010c03
+   lnotab 0x00ff02010c020c010c010c0114010c03
```

### Comparing `fastapi-config-0.0.7/fastapi_config/__pycache__/models.cpython-38.pyc` & `fastapi-config-0.1.0/fastapi_config/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/fastapi_config/admin.py` & `fastapi-config-0.1.0/fastapi_config/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from .backends import BaseConfigStore, DbConfigStore
 from .models import ConfigModel
 
 
 class ConfigModelAdmin(admin.ModelAdmin):
     page_schema = PageSchema(label=_("Configuration"), icon="fa fa-cog")
     model = ConfigModel
-    readonly_fields = ["key"]
+    create_exclude = {"id", "create_time", "update_time"}
+    update_exclude = {"id", "key", "create_time", "update_time"}
 
 
 class ConfigAdmin(admin.FormAdmin):
     router_prefix: str = "/config"
     config_store: BaseConfigStore = None
     form_init = True
     form = Form(mode=DisplayModeEnum.horizontal)
```

### Comparing `fastapi-config-0.0.7/fastapi_config/backends.py` & `fastapi-config-0.1.0/fastapi_config/backends.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-from typing import Dict, Optional, Type, TypeVar, Union, overload
-
-import asyncer
-from pydantic import BaseModel
-from sqlalchemy import select, update
-from sqlalchemy_database import AsyncDatabase, Database
-
-from fastapi_config.models import ConfigModel
-
-_BaseModelT = TypeVar("_BaseModelT", bound="BaseModel")
-_KT = Union[str, Type[_BaseModelT]]
-
-
-class BaseConfigStore:
-    def __init__(self):
-        self.__cached__: Dict[str, ConfigModel] = {}
-
-    def get_key(self, k: _KT) -> str:
-        return k if isinstance(k, str) else getattr(k, "__key__", k.__name__)
-
-    def clear_cache(self, k: _KT):
-        key = self.get_key(k)
-        if key in self.__cached__:
-            self.__cached__.pop(key)
-
-    async def read(self, k: _KT, cache: bool = True) -> Optional[ConfigModel]:
-        """读取配置存储库中ConfigModel对象"""
-        raise NotImplementedError()
-
-    async def save(self, k: _KT, data: str) -> bool:
-        """保存ConfigModel对象到存储库,如果不存在则插入,并且更新缓存."""
-        if not data:
-            return False
-        self.clear_cache(k)
-        return True
-
-    @overload
-    async def get(self, k: str, cache: bool = True) -> Optional[str]:
-        ...
-
-    @overload
-    async def get(self, k: Type[_BaseModelT], cache: bool = True) -> Optional[_BaseModelT]:
-        ...
-
-    async def get(self, k: _KT, cache: bool = True) -> Optional[Union[_BaseModelT, str]]:
-        obj = await self.read(k, cache=cache)
-        if not obj:
-            return None
-        return obj.data if isinstance(k, str) else k.parse_raw(obj.data)
-
-    @overload
-    async def set(self, k: _BaseModelT, v: str = None):
-        ...
-
-    @overload
-    async def set(self, k: _KT, v: str):
-        ...
-
-    async def set(self, k: Union[_KT, _BaseModelT], v: str = None):
-        """保存数据到存储库;如果不存在则插入"""
-        if issubclass(type(k), BaseModel):
-            key, data = k.__class__, k.json()
-        else:
-            key, data = k, v
-        await self.save(key, data=data)
-
-    """以下方法为同步方法,非必要不推荐频繁调用;如需频繁调用,可重写`sread`,`ssave`方法."""
-
-    def sread(self, k: _KT, cache: bool = True) -> Optional[ConfigModel]:
-        """读取配置,同步调用方法"""
-        key = self.get_key(k)
-        if not cache or key not in self.__cached__:
-            return asyncer.syncify(self.read, raise_sync_error=False)(k=k, cache=cache)
-        return self.__cached__[key]
-
-    def ssave(self, k: _KT, data: str) -> bool:
-        """保存配置,同步调用方法"""
-        return asyncer.syncify(self.save, raise_sync_error=False)(k, data)
-
-    @overload
-    def sget(self, k: str, cache: bool = True) -> Optional[str]:
-        ...
-
-    @overload
-    def sget(self, k: Type[_BaseModelT], cache: bool = True) -> Optional[_BaseModelT]:
-        ...
-
-    def sget(self, k: _KT, cache: bool = True) -> Optional[Union[_BaseModelT, str]]:
-        obj = self.sread(k, cache=cache)
-        if not obj:
-            return None
-        return obj.data if isinstance(k, str) else k.parse_raw(obj.data)
-
-    @overload
-    def sset(self, k: _BaseModelT, v: str = None):
-        ...
-
-    @overload
-    def sset(self, k: _KT, v: str):
-        ...
-
-    def sset(self, k: Union[_KT, _BaseModelT], v: str = None):
-        """保存数据到存储库;如果不存在则插入"""
-        if issubclass(type(k), BaseModel):
-            key, data = k.__class__, k.json()
-        else:
-            key, data = k, v
-        self.ssave(key, data=data)
-
-
-class DbConfigStore(BaseConfigStore):
-    def __init__(self, db: Union[Database, AsyncDatabase]):
-        super().__init__()
-        self.db = db
-
-    async def read(self, k: _KT, cache: bool = True) -> Optional[ConfigModel]:
-        key = self.get_key(k)
-        if not cache or key not in self.__cached__:
-            stmt = select(ConfigModel).where(ConfigModel.key == key)
-            obj = await self.db.async_scalar(stmt)
-            self.__cached__[key] = obj.copy() if obj else None  # fix: sqlalchemy Instance is not bound to a Session
-        return self.__cached__[key]
-
-    async def save(self, k: _KT, data: str) -> bool:
-        async with self.db():  # Create a new session
-            obj = await self.read(k, cache=False)
-            if obj is None:
-                key = self.get_key(k)
-                obj = ConfigModel(key=key, name=key, data=data)
-                self.db.add(obj)
-            else:
-                await self.db.async_execute(update(ConfigModel).where(ConfigModel.key == obj.key).values(data=data))
-            await self.db.async_commit()
-        self.clear_cache(k)
-        return True
-
-    def sread(self, k: _KT, cache: bool = True) -> Optional[ConfigModel]:
-        key = self.get_key(k)
-        if not cache or key not in self.__cached__:
-            stmt = select(ConfigModel).where(ConfigModel.key == key)
-            if isinstance(self.db, Database):
-                obj = self.db.session.scalar(stmt)
-            else:
-                obj = asyncer.syncify(self.db.session.scalar, raise_sync_error=False)(stmt)
-            self.__cached__[key] = obj.copy() if obj else None  # fix: sqlalchemy Instance is not bound to a Session
-        return self.__cached__[key]
-
-    def ssave(self, k: _KT, data: str) -> bool:
-        if not isinstance(self.db, Database):
-            return super().ssave(k=k, data=data)
-        with self.db() as session:  # Create a new session
-            obj = self.sread(k, cache=False)
-            if obj is None:
-                key = self.get_key(k)
-                obj = ConfigModel(key=key, name=key, data=data)
-                session.add(obj)
-            else:
-                session.execute(update(ConfigModel).where(ConfigModel.key == obj.key).values(data=data))
-            session.commit()
-        self.clear_cache(k)
-        return True
+from typing import Dict, Optional, Type, TypeVar, Union, overload
+
+import asyncer
+from pydantic import BaseModel
+from sqlalchemy import select, update
+from sqlalchemy_database import AsyncDatabase, Database
+
+from fastapi_config.models import ConfigModel
+
+_BaseModelT = TypeVar("_BaseModelT", bound="BaseModel")
+_KT = Union[str, Type[_BaseModelT]]
+
+
+class BaseConfigStore:
+    def __init__(self):
+        self.__cached__: Dict[str, ConfigModel] = {}
+
+    def get_key(self, k: _KT) -> str:
+        return k if isinstance(k, str) else getattr(k, "__key__", k.__name__)
+
+    def clear_cache(self, k: _KT):
+        key = self.get_key(k)
+        if key in self.__cached__:
+            self.__cached__.pop(key)
+
+    async def read(self, k: _KT, cache: bool = True) -> Optional[ConfigModel]:
+        """读取配置存储库中ConfigModel对象"""
+        raise NotImplementedError()
+
+    async def save(self, k: _KT, data: str) -> bool:
+        """保存ConfigModel对象到存储库,如果不存在则插入,并且更新缓存."""
+        if not data:
+            return False
+        self.clear_cache(k)
+        return True
+
+    @overload
+    async def get(self, k: str, cache: bool = True) -> Optional[str]:
+        ...
+
+    @overload
+    async def get(self, k: Type[_BaseModelT], cache: bool = True) -> Optional[_BaseModelT]:
+        ...
+
+    async def get(self, k: _KT, cache: bool = True) -> Optional[Union[_BaseModelT, str]]:
+        obj = await self.read(k, cache=cache)
+        if not obj:
+            return None
+        return obj.data if isinstance(k, str) else k.parse_raw(obj.data)
+
+    @overload
+    async def set(self, k: _BaseModelT, v: str = None):
+        ...
+
+    @overload
+    async def set(self, k: _KT, v: str):
+        ...
+
+    async def set(self, k: Union[_KT, _BaseModelT], v: str = None):
+        """保存数据到存储库;如果不存在则插入"""
+        if issubclass(type(k), BaseModel):
+            key, data = k.__class__, k.json()
+        else:
+            key, data = k, v
+        await self.save(key, data=data)
+
+    """以下方法为同步方法,非必要不推荐频繁调用;如需频繁调用,可重写`sread`,`ssave`方法."""
+
+    def sread(self, k: _KT, cache: bool = True) -> Optional[ConfigModel]:
+        """读取配置,同步调用方法"""
+        key = self.get_key(k)
+        if not cache or key not in self.__cached__:
+            return asyncer.syncify(self.read, raise_sync_error=False)(k=k, cache=cache)
+        return self.__cached__[key]
+
+    def ssave(self, k: _KT, data: str) -> bool:
+        """保存配置,同步调用方法"""
+        return asyncer.syncify(self.save, raise_sync_error=False)(k, data)
+
+    @overload
+    def sget(self, k: str, cache: bool = True) -> Optional[str]:
+        ...
+
+    @overload
+    def sget(self, k: Type[_BaseModelT], cache: bool = True) -> Optional[_BaseModelT]:
+        ...
+
+    def sget(self, k: _KT, cache: bool = True) -> Optional[Union[_BaseModelT, str]]:
+        obj = self.sread(k, cache=cache)
+        if not obj:
+            return None
+        return obj.data if isinstance(k, str) else k.parse_raw(obj.data)
+
+    @overload
+    def sset(self, k: _BaseModelT, v: str = None):
+        ...
+
+    @overload
+    def sset(self, k: _KT, v: str):
+        ...
+
+    def sset(self, k: Union[_KT, _BaseModelT], v: str = None):
+        """保存数据到存储库;如果不存在则插入"""
+        if issubclass(type(k), BaseModel):
+            key, data = k.__class__, k.json()
+        else:
+            key, data = k, v
+        self.ssave(key, data=data)
+
+
+class DbConfigStore(BaseConfigStore):
+    def __init__(self, db: Union[Database, AsyncDatabase]):
+        super().__init__()
+        self.db = db
+
+    async def read(self, k: _KT, cache: bool = True) -> Optional[ConfigModel]:
+        key = self.get_key(k)
+        if not cache or key not in self.__cached__:
+            stmt = select(ConfigModel).where(ConfigModel.key == key)
+            obj = await self.db.async_scalar(stmt)
+            self.__cached__[key] = obj.copy() if obj else None  # fix: sqlalchemy Instance is not bound to a Session
+        return self.__cached__[key]
+
+    async def save(self, k: _KT, data: str) -> bool:
+        async with self.db():  # Create a new session
+            obj = await self.read(k, cache=False)
+            if obj is None:
+                key = self.get_key(k)
+                obj = ConfigModel(key=key, name=key, data=data)
+                self.db.add(obj)
+            else:
+                await self.db.async_execute(update(ConfigModel).where(ConfigModel.key == obj.key).values(data=data))
+            await self.db.async_commit()
+        self.clear_cache(k)
+        return True
+
+    def sread(self, k: _KT, cache: bool = True) -> Optional[ConfigModel]:
+        key = self.get_key(k)
+        if not cache or key not in self.__cached__:
+            stmt = select(ConfigModel).where(ConfigModel.key == key)
+            if isinstance(self.db, Database):
+                obj = self.db.session.scalar(stmt)
+            else:
+                obj = asyncer.syncify(self.db.session.scalar, raise_sync_error=False)(stmt)
+            self.__cached__[key] = obj.copy() if obj else None  # fix: sqlalchemy Instance is not bound to a Session
+        return self.__cached__[key]
+
+    def ssave(self, k: _KT, data: str) -> bool:
+        if not isinstance(self.db, Database):
+            return super().ssave(k=k, data=data)
+        with self.db() as session:  # Create a new session
+            obj = self.sread(k, cache=False)
+            if obj is None:
+                key = self.get_key(k)
+                obj = ConfigModel(key=key, name=key, data=data)
+                session.add(obj)
+            else:
+                session.execute(update(ConfigModel).where(ConfigModel.key == obj.key).values(data=data))
+            session.commit()
+        self.clear_cache(k)
+        return True
```

### Comparing `fastapi-config-0.0.7/fastapi_config/locale/base.pot` & `fastapi-config-0.1.0/fastapi_config/locale/base.pot`

 * *Files 10% similar despite different names*

```diff
@@ -30,8 +30,14 @@
 msgstr ""
 
 #: models.py:20
 msgid "Description"
 msgstr ""
 
 msgid "Data"
+msgstr ""
+
+msgid "Create Time"
+msgstr ""
+
+msgid "Update Time"
 msgstr ""
```

### Comparing `fastapi-config-0.0.7/fastapi_config/locale/de_DE/LC_MESSAGES/messages.po` & `fastapi-config-0.1.0/fastapi_config/locale/de_DE/LC_MESSAGES/messages.po`

 * *Files 12% similar despite different names*

```diff
@@ -31,8 +31,14 @@
 msgstr "Name"
 
 #: models.py:20
 msgid "Description"
 msgstr "Beschreibung"
 
 msgid "Data"
-msgstr "Daten"
+msgstr "Daten"
+
+msgid "Create Time"
+msgstr "Erstellungszeit"
+
+msgid "Update Time"
+msgstr "Aktualisierungszeit"
```

### Comparing `fastapi-config-0.0.7/fastapi_config/locale/zh_CN/LC_MESSAGES/messages.po` & `fastapi-config-0.1.0/fastapi_config/locale/zh_CN/LC_MESSAGES/messages.po`

 * *Files 9% similar despite different names*

```diff
@@ -31,8 +31,14 @@
 msgstr "名称"
 
 #: models.py:20
 msgid "Description"
 msgstr "描述"
 
 msgid "Data"
-msgstr "数据"
+msgstr "数据"
+
+msgid "Create Time"
+msgstr "创建时间"
+
+msgid "Update Time"
+msgstr "更新时间"
```

### Comparing `fastapi-config-0.0.7/pyproject.toml` & `fastapi-config-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "fastapi-amis-admin>=0.4.0,<0.6.0",
+    "fastapi-amis-admin>=0.4.0",
     "asyncer>=0.0.1",
     "sqlalchemy-database>=0.1.0",
 ]
-version = "0.0.7"
+version = "0.1.0"
 
 [project.urls]
 -Source = "https://github.com/amisadmin/fastapi_config"
 FastAPI-Amis-Admin = "https://github.com/amisadmin/fastapi_amis_admin"
 
 [project.optional-dependencies]
 test = [
```

### Comparing `fastapi-config-0.0.7/README.md` & `fastapi-config-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/tests/conftest.py` & `fastapi-config-0.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/tests/test_DbConfigStore.py` & `fastapi-config-0.1.0/tests/test_DbConfigStore.py`

 * *Files identical despite different names*

### Comparing `fastapi-config-0.0.7/PKG-INFO` & `fastapi-config-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_config
-Version: 0.0.7
+Version: 0.1.0
 Summary: FastAPI-Config is a visual dynamic configuration management extension based on FastAPI-Amis-Admin.
 Keywords: FastAPI-Amis-Admin,FastAPI-Config,Python-Config
 Author-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: Apache Software License
```

