# Comparing `tmp/xinference-0.0.2.tar.gz` & `tmp/xinference-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinference-0.0.2.tar", last modified: Tue Jul 11 12:03:14 2023, max compression
+gzip compressed data, was "xinference-0.0.3.tar", last modified: Tue Jul 11 13:52:52 2023, max compression
```

## Comparing `xinference-0.0.2.tar` & `xinference-0.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.335573 xinference-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-11 12:03:02.000000 xinference-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 12:03:02.000000 xinference-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-11 12:03:14.335573 xinference-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-11 12:03:02.000000 xinference-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-11 12:03:02.000000 xinference-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-11 12:03:14.339573 xinference-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-11 12:03:02.000000 xinference-0.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-11 12:03:02.000000 xinference-0.0.2/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.339573 xinference-0.0.2/xinference/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 12:03:14.339573 xinference-0.0.2/xinference/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.331573 xinference-0.0.2/xinference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/restful_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.331573 xinference-0.0.2/xinference/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.335573 xinference-0.0.2/xinference/deploy/test/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/isolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.335573 xinference-0.0.2/xinference/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/locale/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/locale/zh_CN.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.335573 xinference-0.0.2/xinference/model/
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.335573 xinference-0.0.2/xinference/model/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/chatglm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/vicuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/wizardlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.327573 xinference-0.0.2/xinference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:03:13.000000 xinference-0.0.2/xinference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.991647 xinference-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-11 13:52:44.000000 xinference-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 13:52:44.000000 xinference-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-11 13:52:52.991647 xinference-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-11 13:52:44.000000 xinference-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-11 13:52:44.000000 xinference-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-11 13:52:52.991647 xinference-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-11 13:52:44.000000 xinference-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-11 13:52:44.000000 xinference-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.991647 xinference-0.0.3/xinference/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 13:52:52.991647 xinference-0.0.3/xinference/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.987647 xinference-0.0.3/xinference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/restful_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.987647 xinference-0.0.3/xinference/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.987647 xinference-0.0.3/xinference/deploy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/isolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.991647 xinference-0.0.3/xinference/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/locale/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/locale/zh_CN.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.991647 xinference-0.0.3/xinference/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.991647 xinference-0.0.3/xinference/model/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/vicuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/wizardlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.987647 xinference-0.0.3/xinference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/top_level.txt
```

### Comparing `xinference-0.0.2/LICENSE` & `xinference-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/PKG-INFO` & `xinference-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7869 6e66  : 2.1.Name: xinf
 00000020: 6572 656e 6365 0a56 6572 7369 6f6e 3a20  erence.Version: 
-00000030: 302e 302e 320a 5375 6d6d 6172 793a 204d  0.0.2.Summary: M
+00000030: 302e 302e 330a 5375 6d6d 6172 793a 204d  0.0.3.Summary: M
 00000040: 6f64 656c 2053 6572 7669 6e67 204d 6164  odel Serving Mad
 00000050: 6520 4561 7379 0a48 6f6d 652d 7061 6765  e Easy.Home-page
 00000060: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
 00000070: 2e63 6f6d 2f78 6f72 6269 7473 6169 2f69  .com/xorbitsai/i
 00000080: 6e66 6572 656e 6365 0a41 7574 686f 723a  nference.Author:
 00000090: 2051 696e 2058 7579 650a 4175 7468 6f72   Qin Xuye.Author
 000000a0: 2d65 6d61 696c 3a20 7169 6e78 7579 6540  -email: qinxuye@
@@ -153,461 +153,471 @@
 00000980: 2773 2073 7570 706f 7274 2074 6f20 696e  's support to in
 00000990: 636c 7564 6520 6164 6469 7469 6f6e 616c  clude additional
 000009a0: 2072 756e 7469 6d65 732c 200a 696e 636c   runtimes, .incl
 000009b0: 7564 696e 6720 5079 546f 7263 6820 616e  uding PyTorch an
 000009c0: 6420 4a41 582c 2069 6e20 7468 6520 6e65  d JAX, in the ne
 000009d0: 6172 2066 7574 7572 652e 0a0a 215b 6465  ar future...![de
 000009e0: 6d6f 5d28 6173 7365 7473 2f64 656d 6f2e  mo](assets/demo.
-000009f0: 6769 6629 0a0a 0a23 2320 4b65 7920 4665  gif)...## Key Fe
-00000a00: 6174 7572 6573 0af0 9f8c 9f20 2a2a 4d6f  atures..... **Mo
-00000a10: 6465 6c20 5365 7276 696e 6720 4d61 6465  del Serving Made
-00000a20: 2045 6173 792a 2a3a 2049 6e66 6572 656e   Easy**: Inferen
-00000a30: 6365 2073 696d 706c 6966 6965 7320 7468  ce simplifies th
-00000a40: 6520 7072 6f63 6573 7320 6f66 2073 6572  e process of ser
-00000a50: 7669 6e67 206c 6172 6765 206c 616e 6775  ving large langu
-00000a60: 6167 652c 2073 7065 6563 6820 0a72 6563  age, speech .rec
-00000a70: 6f67 6e69 7469 6f6e 2c20 616e 6420 6d75  ognition, and mu
-00000a80: 6c74 696d 6f64 616c 206d 6f64 656c 732e  ltimodal models.
-00000a90: 2059 6f75 2063 616e 2073 6574 2075 7020   You can set up 
-00000aa0: 616e 6420 6465 706c 6f79 2079 6f75 7220  and deploy your 
-00000ab0: 6d6f 6465 6c73 0a66 6f72 2065 7870 6572  models.for exper
-00000ac0: 696d 656e 7461 7469 6f6e 2061 6e64 2070  imentation and p
-00000ad0: 726f 6475 6374 696f 6e20 7769 7468 2061  roduction with a
-00000ae0: 2073 696e 676c 6520 636f 6d6d 616e 642e   single command.
-00000af0: 0a0a e29a a1ef b88f 202a 2a53 7461 7465  ........ **State
-00000b00: 2d6f 662d 7468 652d 4172 7420 4d6f 6465  -of-the-Art Mode
-00000b10: 6c73 2a2a 3a20 4578 7065 7269 6d65 6e74  ls**: Experiment
-00000b20: 2077 6974 6820 6375 7474 696e 672d 6564   with cutting-ed
-00000b30: 6765 2062 7569 6c74 2d69 6e20 6d6f 6465  ge built-in mode
-00000b40: 6c73 2075 7369 6e67 2061 2073 696e 676c  ls using a singl
-00000b50: 6520 0a63 6f6d 6d61 6e64 2e20 496e 6665  e .command. Infe
-00000b60: 7265 6e63 6520 7072 6f76 6964 6573 2061  rence provides a
-00000b70: 6363 6573 7320 746f 2073 7461 7465 2d6f  ccess to state-o
-00000b80: 662d 7468 652d 6172 7420 6f70 656e 2d73  f-the-art open-s
-00000b90: 6f75 7263 6520 6d6f 6465 6c73 210a 0af0  ource models!...
-00000ba0: 9f96 a520 2a2a 4865 7465 726f 6765 6e65  ... **Heterogene
-00000bb0: 6f75 7320 4861 7264 7761 7265 2055 7469  ous Hardware Uti
-00000bc0: 6c69 7a61 7469 6f6e 2a2a 3a20 4d61 6b65  lization**: Make
-00000bd0: 2074 6865 206d 6f73 7420 6f66 2079 6f75   the most of you
-00000be0: 7220 6861 7264 7761 7265 2072 6573 6f75  r hardware resou
-00000bf0: 7263 6573 2e20 586f 7262 6974 7320 0a49  rces. Xorbits .I
-00000c00: 6e66 6572 656e 6365 2069 6e74 656c 6c69  nference intelli
-00000c10: 6765 6e74 6c79 2075 7469 6c69 7a65 7320  gently utilizes 
-00000c20: 6865 7465 726f 6765 6e65 6f75 7320 6861  heterogeneous ha
-00000c30: 7264 7761 7265 2c20 696e 636c 7564 696e  rdware, includin
-00000c40: 6720 4750 5573 2061 6e64 2043 5055 732c  g GPUs and CPUs,
-00000c50: 2074 6f20 6d61 7869 6d69 7a65 0a70 6572   to maximize.per
-00000c60: 666f 726d 616e 6365 2061 6e64 2061 6363  formance and acc
-00000c70: 656c 6572 6174 6520 796f 7572 206d 6f64  elerate your mod
-00000c80: 656c 2069 6e66 6572 656e 6365 2074 6173  el inference tas
-00000c90: 6b73 2e0a 0ae2 9a99 efb8 8f20 2a2a 466c  ks......... **Fl
-00000ca0: 6578 6962 6c65 2041 5049 2061 6e64 2049  exible API and I
-00000cb0: 6e74 6572 6661 6365 732a 2a3a 2058 6f72  nterfaces**: Xor
-00000cc0: 6269 7473 2049 6e66 6572 656e 6365 206f  bits Inference o
-00000cd0: 6666 6572 7320 6d75 6c74 6970 6c65 2069  ffers multiple i
-00000ce0: 6e74 6572 6661 6365 7320 666f 7220 696e  nterfaces for in
-00000cf0: 7465 7261 6374 696e 670a 7769 7468 2079  teracting.with y
-00000d00: 6f75 7220 6d6f 6465 6c73 2e20 596f 7520  our models. You 
-00000d10: 6361 6e20 7574 696c 697a 6520 7468 6520  can utilize the 
-00000d20: 5250 4320 616e 6420 5245 5354 6675 6c20  RPC and RESTful 
-00000d30: 4150 4928 636f 6d70 6174 6962 6c65 2077  API(compatible w
-00000d40: 6974 6820 4f70 656e 4149 2041 5049 2920  ith OpenAI API) 
-00000d50: 746f 2069 6e74 6567 7261 7465 0a79 6f75  to integrate.you
-00000d60: 7220 6d6f 6465 6c73 2077 6974 6820 6578  r models with ex
-00000d70: 6973 7469 6e67 2073 7973 7465 6d73 206f  isting systems o
-00000d80: 7220 7573 6520 7468 6520 636f 6d6d 616e  r use the comman
-00000d90: 642d 6c69 6e65 2069 6e74 6572 6661 6365  d-line interface
-00000da0: 2028 434c 4929 2061 6e64 2074 6865 2069   (CLI) and the i
-00000db0: 6e74 7569 7469 7665 2057 6562 5549 0a66  ntuitive WebUI.f
-00000dc0: 6f72 2073 6561 6d6c 6573 7320 6d61 6e61  or seamless mana
-00000dd0: 6765 6d65 6e74 2061 6e64 206d 6f6e 6974  gement and monit
-00000de0: 6f72 696e 672e 0a0a f09f 8c90 202a 2a44  oring....... **D
-00000df0: 6973 7472 6962 7574 6564 2044 6570 6c6f  istributed Deplo
-00000e00: 796d 656e 742a 2a3a 2058 6f72 6269 7473  yment**: Xorbits
-00000e10: 2049 6e66 6572 656e 6365 2065 7863 656c   Inference excel
-00000e20: 7320 696e 2064 6973 7472 6962 7574 6564  s in distributed
-00000e30: 2064 6570 6c6f 796d 656e 7420 7363 656e   deployment scen
-00000e40: 6172 696f 732c 200a 616c 6c6f 7769 6e67  arios, .allowing
-00000e50: 2074 6865 2073 6561 6d6c 6573 7320 6469   the seamless di
-00000e60: 7374 7269 6275 7469 6f6e 206f 6620 6d6f  stribution of mo
-00000e70: 6465 6c20 696e 6665 7265 6e63 6520 6163  del inference ac
-00000e80: 726f 7373 206d 756c 7469 706c 6520 6465  ross multiple de
-00000e90: 7669 6365 7320 6f72 206d 6163 6869 6e65  vices or machine
-00000ea0: 732e 2049 740a 6c65 7665 7261 6765 7320  s. It.leverages 
-00000eb0: 6469 7374 7269 6275 7465 6420 636f 6d70  distributed comp
-00000ec0: 7574 696e 6720 7465 6368 6e69 7175 6573  uting techniques
-00000ed0: 2074 6f20 7061 7261 6c6c 656c 697a 6520   to parallelize 
-00000ee0: 616e 6420 7363 616c 6520 7468 6520 696e  and scale the in
-00000ef0: 6665 7265 6e63 6520 7072 6f63 6573 732e  ference process.
-00000f00: 0a0a f09f 948c 202a 2a42 7569 6c74 2d69  ...... **Built-i
-00000f10: 6e20 496e 7465 6772 6174 696f 6e20 7769  n Integration wi
-00000f20: 7468 2054 6869 7264 2d50 6172 7479 204c  th Third-Party L
-00000f30: 6962 7261 7269 6573 2a2a 3a20 586f 7262  ibraries**: Xorb
-00000f40: 6974 7320 496e 6665 7265 6e63 6520 7365  its Inference se
-00000f50: 616d 6c65 7373 6c79 2069 6e74 6567 7261  amlessly integra
-00000f60: 7465 730a 7769 7468 2070 6f70 756c 6172  tes.with popular
-00000f70: 2074 6869 7264 2d70 6172 7479 206c 6962   third-party lib
-00000f80: 7261 7269 6573 206c 696b 6520 4c61 6e67  raries like Lang
-00000f90: 4368 6169 6e20 616e 6420 4c6c 616d 6149  Chain and LlamaI
-00000fa0: 6e64 6578 2e20 2843 6f6d 696e 6720 736f  ndex. (Coming so
-00000fb0: 6f6e 290a 0a23 2320 4765 7474 696e 6720  on)..## Getting 
-00000fc0: 5374 6172 7465 640a 5869 6e66 6572 656e  Started.Xinferen
-00000fd0: 6365 2063 616e 2062 6520 696e 7374 616c  ce can be instal
-00000fe0: 6c65 6420 7669 6120 7069 7020 6672 6f6d  led via pip from
-00000ff0: 2050 7950 492e 2049 7420 6973 2068 6967   PyPI. It is hig
-00001000: 686c 7920 7265 636f 6d6d 656e 6465 6420  hly recommended 
-00001010: 746f 2063 7265 6174 6520 6120 6e65 7720  to create a new 
-00001020: 7669 7274 7561 6c0a 656e 7669 726f 6e6d  virtual.environm
-00001030: 656e 7420 746f 2061 766f 6964 2063 6f6e  ent to avoid con
-00001040: 666c 6963 7473 2e0a 6060 6062 6173 680a  flicts..```bash.
-00001050: 2420 7069 7020 696e 7374 616c 6c20 2278  $ pip install "x
-00001060: 696e 6665 7265 6e63 655b 616c 6c5d 220a  inference[all]".
-00001070: 6060 600a 2278 696e 6665 7265 6e63 655b  ```."xinference[
-00001080: 616c 6c5d 2220 696e 7374 616c 6c73 2061  all]" installs a
-00001090: 6c6c 2074 6865 206e 6563 6573 7361 7279  ll the necessary
-000010a0: 2070 6163 6b61 6765 7320 666f 7220 7365   packages for se
-000010b0: 7276 696e 6720 6d6f 6465 6c73 2e20 4966  rving models. If
-000010c0: 2079 6f75 2077 616e 7420 746f 2061 6368   you want to ach
-000010d0: 6965 7665 2061 6363 656c 6572 6174 696f  ieve acceleratio
-000010e0: 6e20 6f6e 200a 6469 6666 6572 656e 7420  n on .different 
-000010f0: 6861 7264 7761 7265 2c20 7265 6665 7220  hardware, refer 
-00001100: 746f 2074 6865 2069 6e73 7461 6c6c 6174  to the installat
-00001110: 696f 6e20 646f 6375 6d65 6e74 6174 696f  ion documentatio
-00001120: 6e20 6f66 2074 6865 2063 6f72 7265 7370  n of the corresp
-00001130: 6f6e 6469 6e67 2070 6163 6b61 6765 2e0a  onding package..
-00001140: 2d20 5b6c 6c61 6d61 2d63 7070 2d70 7974  - [llama-cpp-pyt
-00001150: 686f 6e5d 2868 7474 7073 3a2f 2f67 6974  hon](https://git
-00001160: 6875 622e 636f 6d2f 6162 6574 6c65 6e2f  hub.com/abetlen/
-00001170: 6c6c 616d 612d 6370 702d 7079 7468 6f6e  llama-cpp-python
-00001180: 2369 6e73 7461 6c6c 6174 696f 6e2d 6672  #installation-fr
-00001190: 6f6d 2d70 7970 692d 7265 636f 6d6d 656e  om-pypi-recommen
-000011a0: 6465 6429 2069 7320 7265 7175 6972 6564  ded) is required
-000011b0: 2074 6f20 7275 6e20 6062 6169 6368 7561   to run `baichua
-000011c0: 6e60 2c20 6077 697a 6172 646c 6d2d 7631  n`, `wizardlm-v1
-000011d0: 2e30 602c 2060 7669 6375 6e61 2d76 312e  .0`, `vicuna-v1.
-000011e0: 3360 2061 6e64 2060 6f72 6361 602e 0a2d  3` and `orca`..-
-000011f0: 205b 6368 6174 676c 6d2d 6370 702d 7079   [chatglm-cpp-py
-00001200: 7468 6f6e 5d28 6874 7470 733a 2f2f 6769  thon](https://gi
-00001210: 7468 7562 2e63 6f6d 2f6c 692d 706c 7573  thub.com/li-plus
-00001220: 2f63 6861 7467 6c6d 2e63 7070 2367 6574  /chatglm.cpp#get
-00001230: 7469 6e67 2d73 7461 7274 6564 2920 6973  ting-started) is
-00001240: 2072 6571 7569 7265 6420 746f 2072 756e   required to run
-00001250: 2060 6368 6174 676c 6d60 2061 6e64 2060   `chatglm` and `
-00001260: 6368 6174 676c 6d32 602e 0a0a 0a23 2323  chatglm2`....###
-00001270: 2044 6570 6c6f 796d 656e 740a 596f 7520   Deployment.You 
-00001280: 6361 6e20 6465 706c 6f79 2058 696e 6665  can deploy Xinfe
-00001290: 7265 6e63 6520 6c6f 6361 6c6c 7920 7769  rence locally wi
-000012a0: 7468 2061 2073 696e 676c 6520 636f 6d6d  th a single comm
-000012b0: 616e 6420 6f72 2064 6570 6c6f 7920 6974  and or deploy it
-000012c0: 2069 6e20 6120 6469 7374 7269 6275 7465   in a distribute
-000012d0: 6420 636c 7573 7465 722e 200a 0a23 2323  d cluster. ..###
-000012e0: 2320 4c6f 6361 6c0a 546f 2073 7461 7274  # Local.To start
-000012f0: 2061 206c 6f63 616c 2069 6e73 7461 6e63   a local instanc
-00001300: 6520 6f66 2058 696e 6665 7265 6e63 652c  e of Xinference,
-00001310: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
-00001320: 6e67 2063 6f6d 6d61 6e64 3a0a 6060 6062  ng command:.```b
-00001330: 6173 680a 2420 7869 6e66 6572 656e 6365  ash.$ xinference
-00001340: 0a60 6060 0a0a 2323 2323 2044 6973 7472  .```..#### Distr
-00001350: 6962 7574 6564 0a0a 546f 2064 6570 6c6f  ibuted..To deplo
-00001360: 7920 5869 6e66 6572 656e 6365 2069 6e20  y Xinference in 
-00001370: 6120 636c 7573 7465 722c 2079 6f75 206e  a cluster, you n
-00001380: 6565 6420 746f 2073 7461 7274 2061 2058  eed to start a X
-00001390: 696e 6665 7265 6e63 6520 7375 7065 7276  inference superv
-000013a0: 6973 6f72 206f 6e20 6f6e 6520 7365 7276  isor on one serv
-000013b0: 6572 2061 6e64 200a 5869 6e66 6572 656e  er and .Xinferen
-000013c0: 6365 2077 6f72 6b65 7273 206f 6e20 7468  ce workers on th
-000013d0: 6520 6f74 6865 7220 7365 7276 6572 732e  e other servers.
-000013e0: 2046 6f6c 6c6f 7720 7468 6520 7374 6570   Follow the step
-000013f0: 7320 6265 6c6f 773a 0a0a 2a2a 5374 6172  s below:..**Star
-00001400: 7469 6e67 2074 6865 2053 7570 6572 7669  ting the Supervi
-00001410: 736f 722a 2a3a 204f 6e20 7468 6520 7365  sor**: On the se
-00001420: 7276 6572 2077 6865 7265 2079 6f75 2077  rver where you w
-00001430: 616e 7420 746f 2072 756e 2074 6865 2058  ant to run the X
-00001440: 696e 6665 7265 6e63 6520 7375 7065 7276  inference superv
-00001450: 6973 6f72 2c20 7275 6e20 7468 6520 666f  isor, run the fo
-00001460: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
-00001470: 0a60 6060 6261 7368 0a24 2078 696e 6665  .```bash.$ xinfe
-00001480: 7265 6e63 652d 7375 7065 7276 6973 6f72  rence-supervisor
-00001490: 202d 4820 2224 7b73 7570 6572 7669 736f   -H "${superviso
-000014a0: 725f 686f 7374 7d22 0a60 6060 0a52 6570  r_host}".```.Rep
-000014b0: 6c61 6365 2060 247b 7375 7065 7276 6973  lace `${supervis
-000014c0: 6f72 5f68 6f73 747d 6020 7769 7468 2074  or_host}` with t
-000014d0: 6865 2061 6374 7561 6c20 686f 7374 206f  he actual host o
-000014e0: 6620 796f 7572 2073 7570 6572 7669 736f  f your superviso
-000014f0: 7220 7365 7276 6572 2e0a 0a2a 2a53 7461  r server...**Sta
-00001500: 7274 696e 6720 7468 6520 576f 726b 6572  rting the Worker
-00001510: 732a 2a3a 204f 6e20 6561 6368 206f 6620  s**: On each of 
-00001520: 7468 6520 6f74 6865 7220 7365 7276 6572  the other server
-00001530: 7320 7768 6572 6520 796f 7520 7761 6e74  s where you want
-00001540: 2074 6f20 7275 6e20 5869 6e66 6572 656e   to run Xinferen
-00001550: 6365 2077 6f72 6b65 7273 2c20 7275 6e20  ce workers, run 
-00001560: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00001570: 6d6d 616e 643a 0a60 6060 6261 7368 0a24  mmand:.```bash.$
-00001580: 2078 696e 6665 7265 6e63 652d 776f 726b   xinference-work
-00001590: 6572 202d 6520 2268 7474 703a 2f2f 247b  er -e "http://${
-000015a0: 7375 7065 7276 6973 6f72 5f68 6f73 747d  supervisor_host}
-000015b0: 3a39 3939 3722 0a60 6060 0a0a 4f6e 6365  :9997".```..Once
-000015c0: 2058 696e 6665 7265 6e63 6520 6973 2072   Xinference is r
-000015d0: 756e 6e69 6e67 2c20 616e 2065 6e64 706f  unning, an endpo
-000015e0: 696e 7420 7769 6c6c 2062 6520 6163 6365  int will be acce
-000015f0: 7373 6962 6c65 2066 6f72 206d 6f64 656c  ssible for model
-00001600: 206d 616e 6167 656d 656e 7420 7669 6120   management via 
-00001610: 434c 4920 6f72 0a58 696e 6665 7265 6e63  CLI or.Xinferenc
-00001620: 6520 2063 6c69 656e 742e 0a0a 2d20 466f  e  client...- Fo
-00001630: 7220 6c6f 6361 6c20 6465 706c 6f79 6d65  r local deployme
-00001640: 6e74 2c20 7468 6520 656e 6470 6f69 6e74  nt, the endpoint
-00001650: 2077 696c 6c20 6265 2060 6874 7470 3a2f   will be `http:/
-00001660: 2f6c 6f63 616c 686f 7374 3a39 3939 3760  /localhost:9997`
-00001670: 2e0a 2d20 466f 7220 636c 7573 7465 7220  ..- For cluster 
-00001680: 6465 706c 6f79 6d65 6e74 2c20 7468 6520  deployment, the 
-00001690: 656e 6470 6f69 6e74 2077 696c 6c20 6265  endpoint will be
-000016a0: 2060 6874 7470 3a2f 2f24 7b73 7570 6572   `http://${super
-000016b0: 7669 736f 725f 686f 7374 7d3a 3939 3937  visor_host}:9997
-000016c0: 602c 2077 6865 7265 0a60 247b 7375 7065  `, where.`${supe
-000016d0: 7276 6973 6f72 5f68 6f73 747d 6020 6973  rvisor_host}` is
-000016e0: 2074 6865 2068 6f73 746e 616d 6520 6f72   the hostname or
-000016f0: 2049 5020 6164 6472 6573 7320 6f66 2074   IP address of t
-00001700: 6865 2073 6572 7665 7220 7768 6572 6520  he server where 
-00001710: 7468 6520 7375 7065 7276 6973 6f72 2069  the supervisor i
-00001720: 7320 7275 6e6e 696e 672e 0a0a 596f 7520  s running...You 
-00001730: 6361 6e20 616c 736f 2076 6965 7720 6120  can also view a 
-00001740: 7765 6220 5549 2075 7369 6e67 2074 6865  web UI using the
-00001750: 2058 696e 6665 7265 6e63 6520 656e 6470   Xinference endp
-00001760: 6f69 6e74 2074 6f20 6368 6174 2077 6974  oint to chat wit
-00001770: 6820 616c 6c20 7468 6520 0a62 7569 6c74  h all the .built
-00001780: 696e 206d 6f64 656c 732e 2059 6f75 2063  in models. You c
-00001790: 616e 2065 7665 6e20 2a2a 6368 6174 2077  an even **chat w
-000017a0: 6974 6820 7477 6f20 6375 7474 696e 672d  ith two cutting-
-000017b0: 6564 6765 2041 4920 6d6f 6465 6c73 2073  edge AI models s
-000017c0: 6964 652d 6279 2d73 6964 6520 746f 2063  ide-by-side to c
-000017d0: 6f6d 7061 7265 0a74 6865 6972 2070 6572  ompare.their per
-000017e0: 666f 726d 616e 6365 2a2a 210a 0a21 5b77  formance**!..![w
-000017f0: 6562 2055 495d 2861 7373 6574 732f 7869  eb UI](assets/xi
-00001800: 6e66 6572 656e 6365 2d64 6f77 6e6c 6f61  nference-downloa
-00001810: 6469 6e67 2e70 6e67 290a 0a23 2323 2058  ding.png)..### X
-00001820: 696e 6665 7265 6e63 6520 434c 490a 5869  inference CLI.Xi
-00001830: 6e66 6572 656e 6365 2070 726f 7669 6465  nference provide
-00001840: 7320 6120 636f 6d6d 616e 6420 6c69 6e65  s a command line
-00001850: 2069 6e74 6572 6661 6365 2028 434c 4929   interface (CLI)
-00001860: 2066 6f72 206d 6f64 656c 206d 616e 6167   for model manag
-00001870: 656d 656e 742e 2048 6572 6520 6172 6520  ement. Here are 
-00001880: 736f 6d65 2075 7365 6675 6c20 0a63 6f6d  some useful .com
-00001890: 6d61 6e64 733a 0a0a 2d20 4c61 756e 6368  mands:..- Launch
-000018a0: 2061 206d 6f64 656c 2028 6120 6d6f 6465   a model (a mode
-000018b0: 6c20 5549 4420 7769 6c6c 2062 6520 7265  l UID will be re
-000018c0: 7475 726e 6564 293a 2060 7869 6e66 6572  turned): `xinfer
-000018d0: 656e 6365 206c 6175 6e63 6860 0a2d 204c  ence launch`.- L
-000018e0: 6973 7420 7275 6e6e 696e 6720 6d6f 6465  ist running mode
-000018f0: 6c73 3a20 6078 696e 6665 7265 6e63 6520  ls: `xinference 
-00001900: 6c69 7374 600a 2d20 4c69 7374 2061 6c6c  list`.- List all
-00001910: 2074 6865 2062 7569 6c74 696e 206d 6f64   the builtin mod
-00001920: 656c 733a 2060 7869 6e66 6572 656e 6365  els: `xinference
-00001930: 206c 6973 7420 2d2d 616c 6c60 0a2d 2054   list --all`.- T
-00001940: 6572 6d69 6e61 7465 2061 206d 6f64 656c  erminate a model
-00001950: 3a20 6078 696e 6665 7265 6e63 6520 7465  : `xinference te
-00001960: 726d 696e 6174 6520 2d2d 6d6f 6465 6c2d  rminate --model-
-00001970: 7569 6420 247b 6d6f 6465 6c5f 7569 647d  uid ${model_uid}
-00001980: 600a 0a23 2323 2058 696e 6665 7265 6e63  `..### Xinferenc
-00001990: 6520 436c 6965 6e74 0a58 696e 6665 7265  e Client.Xinfere
-000019a0: 6e63 6520 616c 736f 2070 726f 7669 6465  nce also provide
-000019b0: 7320 6120 636c 6965 6e74 2066 6f72 206d  s a client for m
-000019c0: 616e 6167 696e 6720 616e 6420 6163 6365  anaging and acce
-000019d0: 7373 696e 6720 6d6f 6465 6c73 2070 726f  ssing models pro
-000019e0: 6772 616d 6d61 7469 6361 6c6c 793a 0a0a  grammatically:..
-000019f0: 6060 6070 7974 686f 6e0a 6672 6f6d 2078  ```python.from x
-00001a00: 696e 6665 7265 6e63 652e 636c 6965 6e74  inference.client
-00001a10: 2069 6d70 6f72 7420 436c 6965 6e74 0a0a   import Client..
-00001a20: 636c 6965 6e74 203d 2043 6c69 656e 7428  client = Client(
-00001a30: 2268 7474 703a 2f2f 6c6f 6361 6c68 6f73  "http://localhos
-00001a40: 743a 3939 3937 2229 0a6d 6f64 656c 5f75  t:9997").model_u
-00001a50: 6964 203d 2063 6c69 656e 742e 6c61 756e  id = client.laun
-00001a60: 6368 5f6d 6f64 656c 286d 6f64 656c 5f6e  ch_model(model_n
-00001a70: 616d 653d 2263 6861 7467 6c6d 3222 290a  ame="chatglm2").
-00001a80: 6d6f 6465 6c20 3d20 636c 6965 6e74 2e67  model = client.g
-00001a90: 6574 5f6d 6f64 656c 286d 6f64 656c 5f75  et_model(model_u
-00001aa0: 6964 290a 0a63 6861 745f 6869 7374 6f72  id)..chat_histor
-00001ab0: 7920 3d20 5b5d 0a70 726f 6d70 7420 3d20  y = [].prompt = 
-00001ac0: 2257 6861 7420 6973 2074 6865 206c 6172  "What is the lar
-00001ad0: 6765 7374 2061 6e69 6d61 6c3f 220a 6d6f  gest animal?".mo
-00001ae0: 6465 6c2e 6368 6174 280a 2020 2020 2020  del.chat(.      
-00001af0: 2020 2020 2020 7072 6f6d 7074 2c0a 2020        prompt,.  
-00001b00: 2020 2020 2020 2020 2020 6368 6174 5f68            chat_h
-00001b10: 6973 746f 7279 2c0a 2020 2020 2020 2020  istory,.        
-00001b20: 2020 2020 6765 6e65 7261 7465 5f63 6f6e      generate_con
-00001b30: 6669 673d 7b22 6d61 785f 746f 6b65 6e73  fig={"max_tokens
-00001b40: 223a 2031 3032 347d 0a20 2020 2020 2020  ": 1024}.       
-00001b50: 2029 0a60 6060 0a0a 5265 7375 6c74 3a0a   ).```..Result:.
-00001b60: 6060 606a 736f 6e0a 7b0a 2020 2269 6422  ```json.{.  "id"
-00001b70: 3a20 2263 6861 7463 6d70 6c2d 3864 3736  : "chatcmpl-8d76
-00001b80: 6236 3561 2d62 6164 302d 3432 6566 2d39  b65a-bad0-42ef-9
-00001b90: 3132 642d 3461 3035 3333 6439 3064 3631  12d-4a0533d90d61
-00001ba0: 222c 0a20 2022 6d6f 6465 6c22 3a20 2235  ",.  "model": "5
-00001bb0: 3666 3639 3632 322d 3165 3733 2d31 3165  6f69622-1e73-11e
-00001bc0: 652d 6133 6264 2d39 6166 3966 3136 3831  e-a3bd-9af9f1681
-00001bd0: 3663 3622 2c0a 2020 226f 626a 6563 7422  6c6",.  "object"
-00001be0: 3a20 2263 6861 742e 636f 6d70 6c65 7469  : "chat.completi
-00001bf0: 6f6e 222c 0a20 2022 6372 6561 7465 6422  on",.  "created"
-00001c00: 3a20 3136 3838 3931 3931 3837 2c0a 2020  : 1688919187,.  
-00001c10: 2263 686f 6963 6573 223a 205b 0a20 2020  "choices": [.   
-00001c20: 207b 0a20 2020 2020 2022 696e 6465 7822   {.      "index"
-00001c30: 3a20 302c 0a20 2020 2020 2022 6d65 7373  : 0,.      "mess
-00001c40: 6167 6522 3a20 7b0a 2020 2020 2020 2020  age": {.        
-00001c50: 2272 6f6c 6522 3a20 2261 7373 6973 7461  "role": "assista
-00001c60: 6e74 222c 0a20 2020 2020 2020 2022 636f  nt",.        "co
-00001c70: 6e74 656e 7422 3a20 2254 6865 206c 6172  ntent": "The lar
-00001c80: 6765 7374 2061 6e69 6d61 6c20 7468 6174  gest animal that
-00001c90: 2068 6173 2062 6565 6e20 7363 6965 6e74   has been scient
-00001ca0: 6966 6963 616c 6c79 206d 6561 7375 7265  ifically measure
-00001cb0: 6420 6973 2074 6865 2062 6c75 6520 7768  d is the blue wh
-00001cc0: 616c 652c 2077 6869 6368 2068 6173 2061  ale, which has a
-00001cd0: 206d 6178 696d 756d 206c 656e 6774 6820   maximum length 
-00001ce0: 6f66 2061 726f 756e 6420 3233 206d 6574  of around 23 met
-00001cf0: 6572 7320 2837 3520 6665 6574 2920 666f  ers (75 feet) fo
-00001d00: 7220 6164 756c 7420 616e 696d 616c 7320  r adult animals 
-00001d10: 616e 6420 6361 6e20 7765 6967 6820 7570  and can weigh up
-00001d20: 2074 6f20 3135 302c 3030 3020 706f 756e   to 150,000 poun
-00001d30: 6473 2028 3638 2c30 3030 206b 6729 2e20  ds (68,000 kg). 
-00001d40: 486f 7765 7665 722c 2069 7420 6973 2069  However, it is i
-00001d50: 6d70 6f72 7461 6e74 2074 6f20 6e6f 7465  mportant to note
-00001d60: 2074 6861 7420 7468 6973 2069 7320 6a75   that this is ju
-00001d70: 7374 2061 6e20 6573 7469 6d61 7465 2061  st an estimate a
-00001d80: 6e64 2074 6861 7420 7468 6520 6c61 7267  nd that the larg
-00001d90: 6573 7420 616e 696d 616c 206b 6e6f 776e  est animal known
-00001da0: 2074 6f20 7363 6965 6e63 6520 6d61 7920   to science may 
-00001db0: 6265 206c 6172 6765 7220 7374 696c 6c2e  be larger still.
-00001dc0: 2053 6f6d 6520 7363 6965 6e74 6973 7473   Some scientists
-00001dd0: 2062 656c 6965 7665 2074 6861 7420 7468   believe that th
-00001de0: 6520 6c61 7267 6573 7420 616e 696d 616c  e largest animal
-00001df0: 7320 6d61 7920 6e6f 7420 6861 7665 2061  s may not have a
-00001e00: 2063 6c65 6172 205c 2273 697a 655c 2220   clear \"size\" 
-00001e10: 696e 2074 6865 2073 616d 6520 7761 7920  in the same way 
-00001e20: 7468 6174 2068 756d 616e 7320 646f 2c20  that humans do, 
-00001e30: 6173 2074 6865 6972 2073 697a 6520 6361  as their size ca
-00001e40: 6e20 7661 7279 2064 6570 656e 6469 6e67  n vary depending
-00001e50: 206f 6e20 7468 6520 656e 7669 726f 6e6d   on the environm
-00001e60: 656e 7420 616e 6420 7468 6520 7374 6167  ent and the stag
-00001e70: 6520 6f66 2074 6865 6972 206c 6966 652e  e of their life.
-00001e80: 220a 2020 2020 2020 7d2c 0a20 2020 2020  ".      },.     
-00001e90: 2022 6669 6e69 7368 5f72 6561 736f 6e22   "finish_reason"
-00001ea0: 3a20 224e 6f6e 6522 0a20 2020 207d 0a20  : "None".    }. 
-00001eb0: 205d 2c0a 2020 2275 7361 6765 223a 207b   ],.  "usage": {
-00001ec0: 0a20 2020 2022 7072 6f6d 7074 5f74 6f6b  .    "prompt_tok
-00001ed0: 656e 7322 3a20 2d31 2c0a 2020 2020 2263  ens": -1,.    "c
-00001ee0: 6f6d 706c 6574 696f 6e5f 746f 6b65 6e73  ompletion_tokens
-00001ef0: 223a 202d 312c 0a20 2020 2022 746f 7461  ": -1,.    "tota
-00001f00: 6c5f 746f 6b65 6e73 223a 202d 310a 2020  l_tokens": -1.  
-00001f10: 7d0a 7d0a 6060 600a 0a53 6565 205b 6578  }.}.```..See [ex
-00001f20: 616d 706c 6573 5d28 6578 616d 706c 6573  amples](examples
-00001f30: 2920 666f 7220 6d6f 7265 2065 7861 6d70  ) for more examp
-00001f40: 6c65 732e 0a0a 0a23 2320 4275 696c 7469  les....## Builti
-00001f50: 6e20 6d6f 6465 6c73 0a54 6f20 7669 6577  n models.To view
-00001f60: 2074 6865 2062 7569 6c74 696e 206d 6f64   the builtin mod
-00001f70: 656c 732c 2072 756e 2074 6865 2066 6f6c  els, run the fol
-00001f80: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
-00001f90: 6060 6062 6173 680a 2420 7869 6e66 6572  ```bash.$ xinfer
-00001fa0: 656e 6365 206c 6973 7420 2d2d 616c 6c0a  ence list --all.
-00001fb0: 6060 600a 0a7c 204e 616d 6520 2020 2020  ```..| Name     
-00001fc0: 2020 2020 2020 2020 2020 2020 7c20 5479              | Ty
-00001fd0: 7065 2020 2020 2020 2020 2020 2020 207c  pe             |
-00001fe0: 204c 616e 6775 6167 6520 7c20 466f 726d   Language | Form
-00001ff0: 6174 207c 2053 697a 6520 2869 6e20 6269  at | Size (in bi
-00002000: 6c6c 696f 6e73 2920 7c20 5175 616e 7469  llions) | Quanti
-00002010: 7a61 7469 6f6e 2020 2020 2020 2020 2020  zation          
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 207c 0a7c 202d 2d2d 2d2d 2d2d 2d2d 2d2d   |.| -----------
-00002040: 2d2d 2d2d 2d2d 2d2d 2d20 7c2d 2d2d 2d2d  --------- |-----
-00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
-00002060: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-00002070: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
-00002080: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00002090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000020a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-000020b0: 0a7c 2062 6169 6368 7561 6e20 2020 2020  .| baichuan     
-000020c0: 2020 2020 2020 2020 7c20 466f 756e 6461          | Founda
-000020d0: 7469 6f6e 204d 6f64 656c 207c 2065 6e2c  tion Model | en,
-000020e0: 207a 6820 2020 7c20 6767 6d6c 7633 207c   zh   | ggmlv3 |
-000020f0: 2037 2020 2020 2020 2020 2020 2020 2020   7              
-00002100: 2020 2020 7c20 2771 325f 4b27 2c20 2771      | 'q2_K', 'q
-00002110: 335f 4b5f 4c27 2c20 2e2e 2e20 2c20 2771  3_K_L', ... , 'q
-00002120: 365f 4b27 2c20 2771 385f 3027 207c 0a7c  6_K', 'q8_0' |.|
-00002130: 2063 6861 7467 6c6d 2020 2020 2020 2020   chatglm        
-00002140: 2020 2020 2020 7c20 5346 5420 4d6f 6465        | SFT Mode
-00002150: 6c20 2020 2020 2020 207c 2065 6e2c 207a  l        | en, z
-00002160: 6820 2020 7c20 6767 6d6c 7633 207c 2036  h   | ggmlv3 | 6
-00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2020 7c20 2771 345f 3027 2c20 2771 345f    | 'q4_0', 'q4_
-00002190: 3127 2c20 2771 355f 3027 2c20 2771 355f  1', 'q5_0', 'q5_
-000021a0: 3127 2c20 2771 385f 3027 207c 0a7c 2063  1', 'q8_0' |.| c
-000021b0: 6861 7467 6c6d 3220 2020 2020 2020 2020  hatglm2         
-000021c0: 2020 2020 7c20 5346 5420 4d6f 6465 6c20      | SFT Model 
-000021d0: 2020 2020 2020 207c 2065 6e2c 207a 6820         | en, zh 
-000021e0: 2020 7c20 6767 6d6c 7633 207c 2036 2020    | ggmlv3 | 6  
-000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 7c20 2771 345f 3027 2c20 2771 345f 3127  | 'q4_0', 'q4_1'
-00002210: 2c20 2771 355f 3027 2c20 2771 355f 3127  , 'q5_0', 'q5_1'
-00002220: 2c20 2771 385f 3027 207c 0a7c 2077 697a  , 'q8_0' |.| wiz
-00002230: 6172 646c 6d2d 7631 2e30 2020 2020 2020  ardlm-v1.0      
-00002240: 2020 7c20 5346 5420 4d6f 6465 6c20 2020    | SFT Model   
-00002250: 2020 2020 207c 2065 6e20 2020 2020 2020       | en       
-00002260: 7c20 6767 6d6c 7633 207c 2037 2c20 3133  | ggmlv3 | 7, 13
-00002270: 2c20 3333 2020 2020 2020 2020 2020 7c20  , 33          | 
-00002280: 2771 325f 4b27 2c20 2771 335f 4b5f 4c27  'q2_K', 'q3_K_L'
-00002290: 2c20 2e2e 2e20 2c20 2771 365f 4b27 2c20  , ... , 'q6_K', 
-000022a0: 2771 385f 3027 207c 0a7c 2076 6963 756e  'q8_0' |.| vicun
-000022b0: 612d 7631 2e33 2020 2020 2020 2020 2020  a-v1.3          
-000022c0: 7c20 5346 5420 4d6f 6465 6c20 2020 2020  | SFT Model     
-000022d0: 2020 207c 2065 6e20 2020 2020 2020 7c20     | en       | 
-000022e0: 6767 6d6c 7633 207c 2037 2c20 3133 2020  ggmlv3 | 7, 13  
-000022f0: 2020 2020 2020 2020 2020 2020 7c20 2771              | 'q
-00002300: 325f 4b27 2c20 2771 335f 4b5f 4c27 2c20  2_K', 'q3_K_L', 
-00002310: 2e2e 2e20 2c20 2771 365f 4b27 2c20 2771  ... , 'q6_K', 'q
-00002320: 385f 3027 207c 0a7c 206f 7263 6120 2020  8_0' |.| orca   
-00002330: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00002340: 5346 5420 4d6f 6465 6c20 2020 2020 2020  SFT Model       
-00002350: 207c 2065 6e20 2020 2020 2020 7c20 6767   | en       | gg
-00002360: 6d6c 7633 207c 2033 2c20 372c 2031 3320  mlv3 | 3, 7, 13 
-00002370: 2020 2020 2020 2020 2020 7c20 2771 345f            | 'q4_
-00002380: 3027 2c20 2771 345f 3127 2c20 2771 355f  0', 'q4_1', 'q5_
-00002390: 3027 2c20 2771 355f 3127 2c20 2771 385f  0', 'q5_1', 'q8_
-000023a0: 3027 207c 0a0a 0a2a 2a4e 4f54 452a 2a3a  0' |...**NOTE**:
-000023b0: 0a2d 2058 696e 6665 7265 6e63 6520 7769  .- Xinference wi
-000023c0: 6c6c 2064 6f77 6e6c 6f61 6420 6d6f 6465  ll download mode
-000023d0: 6c73 2061 7574 6f6d 6174 6963 616c 6c79  ls automatically
-000023e0: 2066 6f72 2079 6f75 2c20 616e 6420 6279   for you, and by
-000023f0: 2064 6566 6175 6c74 2074 6865 206d 6f64   default the mod
-00002400: 656c 7320 7769 6c6c 2062 6520 7361 7665  els will be save
-00002410: 6420 756e 6465 7220 6024 7b55 5345 527d  d under `${USER}
-00002420: 2f2e 7869 6e66 6572 656e 6365 2f63 6163  /.xinference/cac
-00002430: 6865 602e 0a2d 2046 6f75 6e64 6174 696f  he`..- Foundatio
-00002440: 6e20 6d6f 6465 6c73 206f 6e6c 7920 7072  n models only pr
-00002450: 6f76 6964 6520 696e 7465 7266 6163 6520  ovide interface 
-00002460: 6067 656e 6572 6174 6560 2e0a 2d20 5346  `generate`..- SF
-00002470: 5420 6d6f 6465 6c73 2070 726f 7669 6465  T models provide
-00002480: 2062 6f74 6820 6067 656e 6572 6174 6560   both `generate`
-00002490: 2061 6e64 2060 6368 6174 602e 0a0a 2323   and `chat`...##
-000024a0: 2052 6f61 646d 6170 0a58 696e 6665 7265   Roadmap.Xinfere
-000024b0: 6e63 6520 6973 2063 7572 7265 6e74 6c79  nce is currently
-000024c0: 2075 6e64 6572 2061 6374 6976 6520 6465   under active de
-000024d0: 7665 6c6f 706d 656e 742e 2048 6572 6527  velopment. Here'
-000024e0: 7320 6120 726f 6164 6d61 7020 6f75 746c  s a roadmap outl
-000024f0: 696e 696e 6720 6f75 7220 706c 616e 6e65  ining our planne
-00002500: 6420 0a64 6576 656c 6f70 6d65 6e74 7320  d .developments 
-00002510: 666f 7220 7468 6520 6e65 7874 2066 6577  for the next few
-00002520: 2077 6565 6b73 3a0a 0a23 2323 2050 7954   weeks:..### PyT
-00002530: 6f72 6368 2053 7570 706f 7274 0a57 6974  orch Support.Wit
-00002540: 6820 5079 546f 7263 6820 696e 7465 6772  h PyTorch integr
-00002550: 6174 696f 6e2c 2075 7365 7273 2077 696c  ation, users wil
-00002560: 6c20 6265 2061 626c 6520 746f 2073 6561  l be able to sea
-00002570: 6d6c 6573 736c 7920 7574 696c 697a 6520  mlessly utilize 
-00002580: 5079 546f 7263 6820 6d6f 6465 6c73 2066  PyTorch models f
-00002590: 726f 6d20 4875 6767 696e 6720 4661 6365  rom Hugging Face
-000025a0: 0a77 6974 6869 6e20 5869 6e66 6572 656e  .within Xinferen
-000025b0: 6365 2e0a 0a23 2323 204c 616e 6763 6861  ce...### Langcha
-000025c0: 696e 2026 204c 6c61 6d61 496e 6465 7820  in & LlamaIndex 
-000025d0: 696e 7465 6772 6174 696f 6e0a 5769 7468  integration.With
-000025e0: 2058 696e 6665 7265 6e63 652c 2069 7420   Xinference, it 
-000025f0: 7769 6c6c 2062 6520 6d75 6368 2065 6173  will be much eas
-00002600: 6965 7220 666f 7220 7573 6572 7320 746f  ier for users to
-00002610: 2075 7365 2074 6865 7365 206c 6962 7261   use these libra
-00002620: 7269 6573 2061 6e64 2062 7569 6c64 2061  ries and build a
-00002630: 7070 6c69 6361 7469 6f6e 7320 0a77 6974  pplications .wit
-00002640: 6820 4c4c 4d73 2e0a                      h LLMs..
+000009f0: 6769 6629 0a0a 3c64 6976 2061 6c69 676e  gif)..<div align
+00000a00: 3d22 6365 6e74 6572 223e 0a3c 693e 3c61  ="center">.<i><a
+00000a10: 2068 7265 663d 2268 7474 7073 3a2f 2f6a   href="https://j
+00000a20: 6f69 6e2e 736c 6163 6b2e 636f 6d2f 742f  oin.slack.com/t/
+00000a30: 786f 7262 6974 7369 6f2f 7368 6172 6564  xorbitsio/shared
+00000a40: 5f69 6e76 6974 652f 7a74 2d31 7a33 7a73  _invite/zt-1z3zs
+00000a50: 6d39 6570 2d38 3779 4939 595a 5f42 3739  m9ep-87yI9YZ_B79
+00000a60: 484c 4232 6363 5471 3457 4122 3ef0 9f91  HLB2ccTq4WA">...
+00000a70: 8920 4a6f 696e 206f 7572 2053 6c61 636b  . Join our Slack
+00000a80: 2063 6f6d 6d75 6e69 7479 213c 2f61 3e3c   community!</a><
+00000a90: 2f69 3e0a 3c2f 6469 763e 0a0a 2323 204b  /i>.</div>..## K
+00000aa0: 6579 2046 6561 7475 7265 730a f09f 8c9f  ey Features.....
+00000ab0: 202a 2a4d 6f64 656c 2053 6572 7669 6e67   **Model Serving
+00000ac0: 204d 6164 6520 4561 7379 2a2a 3a20 496e   Made Easy**: In
+00000ad0: 6665 7265 6e63 6520 7369 6d70 6c69 6669  ference simplifi
+00000ae0: 6573 2074 6865 2070 726f 6365 7373 206f  es the process o
+00000af0: 6620 7365 7276 696e 6720 6c61 7267 6520  f serving large 
+00000b00: 6c61 6e67 7561 6765 2c20 7370 6565 6368  language, speech
+00000b10: 200a 7265 636f 676e 6974 696f 6e2c 2061   .recognition, a
+00000b20: 6e64 206d 756c 7469 6d6f 6461 6c20 6d6f  nd multimodal mo
+00000b30: 6465 6c73 2e20 596f 7520 6361 6e20 7365  dels. You can se
+00000b40: 7420 7570 2061 6e64 2064 6570 6c6f 7920  t up and deploy 
+00000b50: 796f 7572 206d 6f64 656c 730a 666f 7220  your models.for 
+00000b60: 6578 7065 7269 6d65 6e74 6174 696f 6e20  experimentation 
+00000b70: 616e 6420 7072 6f64 7563 7469 6f6e 2077  and production w
+00000b80: 6974 6820 6120 7369 6e67 6c65 2063 6f6d  ith a single com
+00000b90: 6d61 6e64 2e0a 0ae2 9aa1 efb8 8f20 2a2a  mand......... **
+00000ba0: 5374 6174 652d 6f66 2d74 6865 2d41 7274  State-of-the-Art
+00000bb0: 204d 6f64 656c 732a 2a3a 2045 7870 6572   Models**: Exper
+00000bc0: 696d 656e 7420 7769 7468 2063 7574 7469  iment with cutti
+00000bd0: 6e67 2d65 6467 6520 6275 696c 742d 696e  ng-edge built-in
+00000be0: 206d 6f64 656c 7320 7573 696e 6720 6120   models using a 
+00000bf0: 7369 6e67 6c65 200a 636f 6d6d 616e 642e  single .command.
+00000c00: 2049 6e66 6572 656e 6365 2070 726f 7669   Inference provi
+00000c10: 6465 7320 6163 6365 7373 2074 6f20 7374  des access to st
+00000c20: 6174 652d 6f66 2d74 6865 2d61 7274 206f  ate-of-the-art o
+00000c30: 7065 6e2d 736f 7572 6365 206d 6f64 656c  pen-source model
+00000c40: 7321 0a0a f09f 96a5 202a 2a48 6574 6572  s!...... **Heter
+00000c50: 6f67 656e 656f 7573 2048 6172 6477 6172  ogeneous Hardwar
+00000c60: 6520 5574 696c 697a 6174 696f 6e2a 2a3a  e Utilization**:
+00000c70: 204d 616b 6520 7468 6520 6d6f 7374 206f   Make the most o
+00000c80: 6620 796f 7572 2068 6172 6477 6172 6520  f your hardware 
+00000c90: 7265 736f 7572 6365 732e 2058 6f72 6269  resources. Xorbi
+00000ca0: 7473 200a 496e 6665 7265 6e63 6520 696e  ts .Inference in
+00000cb0: 7465 6c6c 6967 656e 746c 7920 7574 696c  telligently util
+00000cc0: 697a 6573 2068 6574 6572 6f67 656e 656f  izes heterogeneo
+00000cd0: 7573 2068 6172 6477 6172 652c 2069 6e63  us hardware, inc
+00000ce0: 6c75 6469 6e67 2047 5055 7320 616e 6420  luding GPUs and 
+00000cf0: 4350 5573 2c20 746f 206d 6178 696d 697a  CPUs, to maximiz
+00000d00: 650a 7065 7266 6f72 6d61 6e63 6520 616e  e.performance an
+00000d10: 6420 6163 6365 6c65 7261 7465 2079 6f75  d accelerate you
+00000d20: 7220 6d6f 6465 6c20 696e 6665 7265 6e63  r model inferenc
+00000d30: 6520 7461 736b 732e 0a0a e29a 99ef b88f  e tasks.........
+00000d40: 202a 2a46 6c65 7869 626c 6520 4150 4920   **Flexible API 
+00000d50: 616e 6420 496e 7465 7266 6163 6573 2a2a  and Interfaces**
+00000d60: 3a20 586f 7262 6974 7320 496e 6665 7265  : Xorbits Infere
+00000d70: 6e63 6520 6f66 6665 7273 206d 756c 7469  nce offers multi
+00000d80: 706c 6520 696e 7465 7266 6163 6573 2066  ple interfaces f
+00000d90: 6f72 2069 6e74 6572 6163 7469 6e67 0a77  or interacting.w
+00000da0: 6974 6820 796f 7572 206d 6f64 656c 732e  ith your models.
+00000db0: 2059 6f75 2063 616e 2075 7469 6c69 7a65   You can utilize
+00000dc0: 2074 6865 2052 5043 2061 6e64 2052 4553   the RPC and RES
+00000dd0: 5466 756c 2041 5049 2863 6f6d 7061 7469  Tful API(compati
+00000de0: 626c 6520 7769 7468 204f 7065 6e41 4920  ble with OpenAI 
+00000df0: 4150 4929 2074 6f20 696e 7465 6772 6174  API) to integrat
+00000e00: 650a 796f 7572 206d 6f64 656c 7320 7769  e.your models wi
+00000e10: 7468 2065 7869 7374 696e 6720 7379 7374  th existing syst
+00000e20: 656d 7320 6f72 2075 7365 2074 6865 2063  ems or use the c
+00000e30: 6f6d 6d61 6e64 2d6c 696e 6520 696e 7465  ommand-line inte
+00000e40: 7266 6163 6520 2843 4c49 2920 616e 6420  rface (CLI) and 
+00000e50: 7468 6520 696e 7475 6974 6976 6520 5765  the intuitive We
+00000e60: 6255 490a 666f 7220 7365 616d 6c65 7373  bUI.for seamless
+00000e70: 206d 616e 6167 656d 656e 7420 616e 6420   management and 
+00000e80: 6d6f 6e69 746f 7269 6e67 2e0a 0af0 9f8c  monitoring......
+00000e90: 9020 2a2a 4469 7374 7269 6275 7465 6420  . **Distributed 
+00000ea0: 4465 706c 6f79 6d65 6e74 2a2a 3a20 586f  Deployment**: Xo
+00000eb0: 7262 6974 7320 496e 6665 7265 6e63 6520  rbits Inference 
+00000ec0: 6578 6365 6c73 2069 6e20 6469 7374 7269  excels in distri
+00000ed0: 6275 7465 6420 6465 706c 6f79 6d65 6e74  buted deployment
+00000ee0: 2073 6365 6e61 7269 6f73 2c20 0a61 6c6c   scenarios, .all
+00000ef0: 6f77 696e 6720 7468 6520 7365 616d 6c65  owing the seamle
+00000f00: 7373 2064 6973 7472 6962 7574 696f 6e20  ss distribution 
+00000f10: 6f66 206d 6f64 656c 2069 6e66 6572 656e  of model inferen
+00000f20: 6365 2061 6372 6f73 7320 6d75 6c74 6970  ce across multip
+00000f30: 6c65 2064 6576 6963 6573 206f 7220 6d61  le devices or ma
+00000f40: 6368 696e 6573 2e20 4974 0a6c 6576 6572  chines. It.lever
+00000f50: 6167 6573 2064 6973 7472 6962 7574 6564  ages distributed
+00000f60: 2063 6f6d 7075 7469 6e67 2074 6563 686e   computing techn
+00000f70: 6971 7565 7320 746f 2070 6172 616c 6c65  iques to paralle
+00000f80: 6c69 7a65 2061 6e64 2073 6361 6c65 2074  lize and scale t
+00000f90: 6865 2069 6e66 6572 656e 6365 2070 726f  he inference pro
+00000fa0: 6365 7373 2e0a 0af0 9f94 8c20 2a2a 4275  cess....... **Bu
+00000fb0: 696c 742d 696e 2049 6e74 6567 7261 7469  ilt-in Integrati
+00000fc0: 6f6e 2077 6974 6820 5468 6972 642d 5061  on with Third-Pa
+00000fd0: 7274 7920 4c69 6272 6172 6965 732a 2a3a  rty Libraries**:
+00000fe0: 2058 6f72 6269 7473 2049 6e66 6572 656e   Xorbits Inferen
+00000ff0: 6365 2073 6561 6d6c 6573 736c 7920 696e  ce seamlessly in
+00001000: 7465 6772 6174 6573 0a77 6974 6820 706f  tegrates.with po
+00001010: 7075 6c61 7220 7468 6972 642d 7061 7274  pular third-part
+00001020: 7920 6c69 6272 6172 6965 7320 6c69 6b65  y libraries like
+00001030: 204c 616e 6743 6861 696e 2061 6e64 204c   LangChain and L
+00001040: 6c61 6d61 496e 6465 782e 2028 436f 6d69  lamaIndex. (Comi
+00001050: 6e67 2073 6f6f 6e29 0a0a 2323 2047 6574  ng soon)..## Get
+00001060: 7469 6e67 2053 7461 7274 6564 0a58 696e  ting Started.Xin
+00001070: 6665 7265 6e63 6520 6361 6e20 6265 2069  ference can be i
+00001080: 6e73 7461 6c6c 6564 2076 6961 2070 6970  nstalled via pip
+00001090: 2066 726f 6d20 5079 5049 2e20 4974 2069   from PyPI. It i
+000010a0: 7320 6869 6768 6c79 2072 6563 6f6d 6d65  s highly recomme
+000010b0: 6e64 6564 2074 6f20 6372 6561 7465 2061  nded to create a
+000010c0: 206e 6577 2076 6972 7475 616c 0a65 6e76   new virtual.env
+000010d0: 6972 6f6e 6d65 6e74 2074 6f20 6176 6f69  ironment to avoi
+000010e0: 6420 636f 6e66 6c69 6374 732e 0a60 6060  d conflicts..```
+000010f0: 6261 7368 0a24 2070 6970 2069 6e73 7461  bash.$ pip insta
+00001100: 6c6c 2022 7869 6e66 6572 656e 6365 5b61  ll "xinference[a
+00001110: 6c6c 5d22 0a60 6060 0a22 7869 6e66 6572  ll]".```."xinfer
+00001120: 656e 6365 5b61 6c6c 5d22 2069 6e73 7461  ence[all]" insta
+00001130: 6c6c 7320 616c 6c20 7468 6520 6e65 6365  lls all the nece
+00001140: 7373 6172 7920 7061 636b 6167 6573 2066  ssary packages f
+00001150: 6f72 2073 6572 7669 6e67 206d 6f64 656c  or serving model
+00001160: 732e 2049 6620 796f 7520 7761 6e74 2074  s. If you want t
+00001170: 6f20 6163 6869 6576 6520 6163 6365 6c65  o achieve accele
+00001180: 7261 7469 6f6e 206f 6e20 0a64 6966 6665  ration on .diffe
+00001190: 7265 6e74 2068 6172 6477 6172 652c 2072  rent hardware, r
+000011a0: 6566 6572 2074 6f20 7468 6520 696e 7374  efer to the inst
+000011b0: 616c 6c61 7469 6f6e 2064 6f63 756d 656e  allation documen
+000011c0: 7461 7469 6f6e 206f 6620 7468 6520 636f  tation of the co
+000011d0: 7272 6573 706f 6e64 696e 6720 7061 636b  rresponding pack
+000011e0: 6167 652e 0a2d 205b 6c6c 616d 612d 6370  age..- [llama-cp
+000011f0: 702d 7079 7468 6f6e 5d28 6874 7470 733a  p-python](https:
+00001200: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6265  //github.com/abe
+00001210: 746c 656e 2f6c 6c61 6d61 2d63 7070 2d70  tlen/llama-cpp-p
+00001220: 7974 686f 6e23 696e 7374 616c 6c61 7469  ython#installati
+00001230: 6f6e 2d66 726f 6d2d 7079 7069 2d72 6563  on-from-pypi-rec
+00001240: 6f6d 6d65 6e64 6564 2920 6973 2072 6571  ommended) is req
+00001250: 7569 7265 6420 746f 2072 756e 2060 6261  uired to run `ba
+00001260: 6963 6875 616e 602c 2060 7769 7a61 7264  ichuan`, `wizard
+00001270: 6c6d 2d76 312e 3060 2c20 6076 6963 756e  lm-v1.0`, `vicun
+00001280: 612d 7631 2e33 6020 616e 6420 606f 7263  a-v1.3` and `orc
+00001290: 6160 2e0a 2d20 5b63 6861 7467 6c6d 2d63  a`..- [chatglm-c
+000012a0: 7070 2d70 7974 686f 6e5d 2868 7474 7073  pp-python](https
+000012b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6c69  ://github.com/li
+000012c0: 2d70 6c75 732f 6368 6174 676c 6d2e 6370  -plus/chatglm.cp
+000012d0: 7023 6765 7474 696e 672d 7374 6172 7465  p#getting-starte
+000012e0: 6429 2069 7320 7265 7175 6972 6564 2074  d) is required t
+000012f0: 6f20 7275 6e20 6063 6861 7467 6c6d 6020  o run `chatglm` 
+00001300: 616e 6420 6063 6861 7467 6c6d 3260 2e0a  and `chatglm2`..
+00001310: 0a0a 2323 2320 4465 706c 6f79 6d65 6e74  ..### Deployment
+00001320: 0a59 6f75 2063 616e 2064 6570 6c6f 7920  .You can deploy 
+00001330: 5869 6e66 6572 656e 6365 206c 6f63 616c  Xinference local
+00001340: 6c79 2077 6974 6820 6120 7369 6e67 6c65  ly with a single
+00001350: 2063 6f6d 6d61 6e64 206f 7220 6465 706c   command or depl
+00001360: 6f79 2069 7420 696e 2061 2064 6973 7472  oy it in a distr
+00001370: 6962 7574 6564 2063 6c75 7374 6572 2e20  ibuted cluster. 
+00001380: 0a0a 2323 2323 204c 6f63 616c 0a54 6f20  ..#### Local.To 
+00001390: 7374 6172 7420 6120 6c6f 6361 6c20 696e  start a local in
+000013a0: 7374 616e 6365 206f 6620 5869 6e66 6572  stance of Xinfer
+000013b0: 656e 6365 2c20 7275 6e20 7468 6520 666f  ence, run the fo
+000013c0: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
+000013d0: 0a60 6060 6261 7368 0a24 2078 696e 6665  .```bash.$ xinfe
+000013e0: 7265 6e63 650a 6060 600a 0a23 2323 2320  rence.```..#### 
+000013f0: 4469 7374 7269 6275 7465 640a 0a54 6f20  Distributed..To 
+00001400: 6465 706c 6f79 2058 696e 6665 7265 6e63  deploy Xinferenc
+00001410: 6520 696e 2061 2063 6c75 7374 6572 2c20  e in a cluster, 
+00001420: 796f 7520 6e65 6564 2074 6f20 7374 6172  you need to star
+00001430: 7420 6120 5869 6e66 6572 656e 6365 2073  t a Xinference s
+00001440: 7570 6572 7669 736f 7220 6f6e 206f 6e65  upervisor on one
+00001450: 2073 6572 7665 7220 616e 6420 0a58 696e   server and .Xin
+00001460: 6665 7265 6e63 6520 776f 726b 6572 7320  ference workers 
+00001470: 6f6e 2074 6865 206f 7468 6572 2073 6572  on the other ser
+00001480: 7665 7273 2e20 466f 6c6c 6f77 2074 6865  vers. Follow the
+00001490: 2073 7465 7073 2062 656c 6f77 3a0a 0a2a   steps below:..*
+000014a0: 2a53 7461 7274 696e 6720 7468 6520 5375  *Starting the Su
+000014b0: 7065 7276 6973 6f72 2a2a 3a20 4f6e 2074  pervisor**: On t
+000014c0: 6865 2073 6572 7665 7220 7768 6572 6520  he server where 
+000014d0: 796f 7520 7761 6e74 2074 6f20 7275 6e20  you want to run 
+000014e0: 7468 6520 5869 6e66 6572 656e 6365 2073  the Xinference s
+000014f0: 7570 6572 7669 736f 722c 2072 756e 2074  upervisor, run t
+00001500: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00001510: 6d61 6e64 3a0a 6060 6062 6173 680a 2420  mand:.```bash.$ 
+00001520: 7869 6e66 6572 656e 6365 2d73 7570 6572  xinference-super
+00001530: 7669 736f 7220 2d48 2022 247b 7375 7065  visor -H "${supe
+00001540: 7276 6973 6f72 5f68 6f73 747d 220a 6060  rvisor_host}".``
+00001550: 600a 5265 706c 6163 6520 6024 7b73 7570  `.Replace `${sup
+00001560: 6572 7669 736f 725f 686f 7374 7d60 2077  ervisor_host}` w
+00001570: 6974 6820 7468 6520 6163 7475 616c 2068  ith the actual h
+00001580: 6f73 7420 6f66 2079 6f75 7220 7375 7065  ost of your supe
+00001590: 7276 6973 6f72 2073 6572 7665 722e 0a0a  rvisor server...
+000015a0: 2a2a 5374 6172 7469 6e67 2074 6865 2057  **Starting the W
+000015b0: 6f72 6b65 7273 2a2a 3a20 4f6e 2065 6163  orkers**: On eac
+000015c0: 6820 6f66 2074 6865 206f 7468 6572 2073  h of the other s
+000015d0: 6572 7665 7273 2077 6865 7265 2079 6f75  ervers where you
+000015e0: 2077 616e 7420 746f 2072 756e 2058 696e   want to run Xin
+000015f0: 6665 7265 6e63 6520 776f 726b 6572 732c  ference workers,
+00001600: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
+00001610: 6e67 2063 6f6d 6d61 6e64 3a0a 6060 6062  ng command:.```b
+00001620: 6173 680a 2420 7869 6e66 6572 656e 6365  ash.$ xinference
+00001630: 2d77 6f72 6b65 7220 2d65 2022 6874 7470  -worker -e "http
+00001640: 3a2f 2f24 7b73 7570 6572 7669 736f 725f  ://${supervisor_
+00001650: 686f 7374 7d3a 3939 3937 220a 6060 600a  host}:9997".```.
+00001660: 0a4f 6e63 6520 5869 6e66 6572 656e 6365  .Once Xinference
+00001670: 2069 7320 7275 6e6e 696e 672c 2061 6e20   is running, an 
+00001680: 656e 6470 6f69 6e74 2077 696c 6c20 6265  endpoint will be
+00001690: 2061 6363 6573 7369 626c 6520 666f 7220   accessible for 
+000016a0: 6d6f 6465 6c20 6d61 6e61 6765 6d65 6e74  model management
+000016b0: 2076 6961 2043 4c49 206f 720a 5869 6e66   via CLI or.Xinf
+000016c0: 6572 656e 6365 2020 636c 6965 6e74 2e0a  erence  client..
+000016d0: 0a2d 2046 6f72 206c 6f63 616c 2064 6570  .- For local dep
+000016e0: 6c6f 796d 656e 742c 2074 6865 2065 6e64  loyment, the end
+000016f0: 706f 696e 7420 7769 6c6c 2062 6520 6068  point will be `h
+00001700: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+00001710: 3939 3937 602e 0a2d 2046 6f72 2063 6c75  9997`..- For clu
+00001720: 7374 6572 2064 6570 6c6f 796d 656e 742c  ster deployment,
+00001730: 2074 6865 2065 6e64 706f 696e 7420 7769   the endpoint wi
+00001740: 6c6c 2062 6520 6068 7474 703a 2f2f 247b  ll be `http://${
+00001750: 7375 7065 7276 6973 6f72 5f68 6f73 747d  supervisor_host}
+00001760: 3a39 3939 3760 2c20 7768 6572 650a 6024  :9997`, where.`$
+00001770: 7b73 7570 6572 7669 736f 725f 686f 7374  {supervisor_host
+00001780: 7d60 2069 7320 7468 6520 686f 7374 6e61  }` is the hostna
+00001790: 6d65 206f 7220 4950 2061 6464 7265 7373  me or IP address
+000017a0: 206f 6620 7468 6520 7365 7276 6572 2077   of the server w
+000017b0: 6865 7265 2074 6865 2073 7570 6572 7669  here the supervi
+000017c0: 736f 7220 6973 2072 756e 6e69 6e67 2e0a  sor is running..
+000017d0: 0a59 6f75 2063 616e 2061 6c73 6f20 7669  .You can also vi
+000017e0: 6577 2061 2077 6562 2055 4920 7573 696e  ew a web UI usin
+000017f0: 6720 7468 6520 5869 6e66 6572 656e 6365  g the Xinference
+00001800: 2065 6e64 706f 696e 7420 746f 2063 6861   endpoint to cha
+00001810: 7420 7769 7468 2061 6c6c 2074 6865 200a  t with all the .
+00001820: 6275 696c 7469 6e20 6d6f 6465 6c73 2e20  builtin models. 
+00001830: 596f 7520 6361 6e20 6576 656e 202a 2a63  You can even **c
+00001840: 6861 7420 7769 7468 2074 776f 2063 7574  hat with two cut
+00001850: 7469 6e67 2d65 6467 6520 4149 206d 6f64  ting-edge AI mod
+00001860: 656c 7320 7369 6465 2d62 792d 7369 6465  els side-by-side
+00001870: 2074 6f20 636f 6d70 6172 650a 7468 6569   to compare.thei
+00001880: 7220 7065 7266 6f72 6d61 6e63 652a 2a21  r performance**!
+00001890: 0a0a 215b 7765 6220 5549 5d28 6173 7365  ..![web UI](asse
+000018a0: 7473 2f78 696e 6665 7265 6e63 652d 646f  ts/xinference-do
+000018b0: 776e 6c6f 6164 696e 672e 706e 6729 0a0a  wnloading.png)..
+000018c0: 2323 2320 5869 6e66 6572 656e 6365 2043  ### Xinference C
+000018d0: 4c49 0a58 696e 6665 7265 6e63 6520 7072  LI.Xinference pr
+000018e0: 6f76 6964 6573 2061 2063 6f6d 6d61 6e64  ovides a command
+000018f0: 206c 696e 6520 696e 7465 7266 6163 6520   line interface 
+00001900: 2843 4c49 2920 666f 7220 6d6f 6465 6c20  (CLI) for model 
+00001910: 6d61 6e61 6765 6d65 6e74 2e20 4865 7265  management. Here
+00001920: 2061 7265 2073 6f6d 6520 7573 6566 756c   are some useful
+00001930: 200a 636f 6d6d 616e 6473 3a0a 0a2d 204c   .commands:..- L
+00001940: 6175 6e63 6820 6120 6d6f 6465 6c20 2861  aunch a model (a
+00001950: 206d 6f64 656c 2055 4944 2077 696c 6c20   model UID will 
+00001960: 6265 2072 6574 7572 6e65 6429 3a20 6078  be returned): `x
+00001970: 696e 6665 7265 6e63 6520 6c61 756e 6368  inference launch
+00001980: 600a 2d20 4c69 7374 2072 756e 6e69 6e67  `.- List running
+00001990: 206d 6f64 656c 733a 2060 7869 6e66 6572   models: `xinfer
+000019a0: 656e 6365 206c 6973 7460 0a2d 204c 6973  ence list`.- Lis
+000019b0: 7420 616c 6c20 7468 6520 6275 696c 7469  t all the builti
+000019c0: 6e20 6d6f 6465 6c73 3a20 6078 696e 6665  n models: `xinfe
+000019d0: 7265 6e63 6520 6c69 7374 202d 2d61 6c6c  rence list --all
+000019e0: 600a 2d20 5465 726d 696e 6174 6520 6120  `.- Terminate a 
+000019f0: 6d6f 6465 6c3a 2060 7869 6e66 6572 656e  model: `xinferen
+00001a00: 6365 2074 6572 6d69 6e61 7465 202d 2d6d  ce terminate --m
+00001a10: 6f64 656c 2d75 6964 2024 7b6d 6f64 656c  odel-uid ${model
+00001a20: 5f75 6964 7d60 0a0a 2323 2320 5869 6e66  _uid}`..### Xinf
+00001a30: 6572 656e 6365 2043 6c69 656e 740a 5869  erence Client.Xi
+00001a40: 6e66 6572 656e 6365 2061 6c73 6f20 7072  nference also pr
+00001a50: 6f76 6964 6573 2061 2063 6c69 656e 7420  ovides a client 
+00001a60: 666f 7220 6d61 6e61 6769 6e67 2061 6e64  for managing and
+00001a70: 2061 6363 6573 7369 6e67 206d 6f64 656c   accessing model
+00001a80: 7320 7072 6f67 7261 6d6d 6174 6963 616c  s programmatical
+00001a90: 6c79 3a0a 0a60 6060 7079 7468 6f6e 0a66  ly:..```python.f
+00001aa0: 726f 6d20 7869 6e66 6572 656e 6365 2e63  rom xinference.c
+00001ab0: 6c69 656e 7420 696d 706f 7274 2043 6c69  lient import Cli
+00001ac0: 656e 740a 0a63 6c69 656e 7420 3d20 436c  ent..client = Cl
+00001ad0: 6965 6e74 2822 6874 7470 3a2f 2f6c 6f63  ient("http://loc
+00001ae0: 616c 686f 7374 3a39 3939 3722 290a 6d6f  alhost:9997").mo
+00001af0: 6465 6c5f 7569 6420 3d20 636c 6965 6e74  del_uid = client
+00001b00: 2e6c 6175 6e63 685f 6d6f 6465 6c28 6d6f  .launch_model(mo
+00001b10: 6465 6c5f 6e61 6d65 3d22 6368 6174 676c  del_name="chatgl
+00001b20: 6d32 2229 0a6d 6f64 656c 203d 2063 6c69  m2").model = cli
+00001b30: 656e 742e 6765 745f 6d6f 6465 6c28 6d6f  ent.get_model(mo
+00001b40: 6465 6c5f 7569 6429 0a0a 6368 6174 5f68  del_uid)..chat_h
+00001b50: 6973 746f 7279 203d 205b 5d0a 7072 6f6d  istory = [].prom
+00001b60: 7074 203d 2022 5768 6174 2069 7320 7468  pt = "What is th
+00001b70: 6520 6c61 7267 6573 7420 616e 696d 616c  e largest animal
+00001b80: 3f22 0a6d 6f64 656c 2e63 6861 7428 0a20  ?".model.chat(. 
+00001b90: 2020 2020 2020 2020 2020 2070 726f 6d70             promp
+00001ba0: 742c 0a20 2020 2020 2020 2020 2020 2063  t,.            c
+00001bb0: 6861 745f 6869 7374 6f72 792c 0a20 2020  hat_history,.   
+00001bc0: 2020 2020 2020 2020 2067 656e 6572 6174           generat
+00001bd0: 655f 636f 6e66 6967 3d7b 226d 6178 5f74  e_config={"max_t
+00001be0: 6f6b 656e 7322 3a20 3130 3234 7d0a 2020  okens": 1024}.  
+00001bf0: 2020 2020 2020 290a 6060 600a 0a52 6573        ).```..Res
+00001c00: 756c 743a 0a60 6060 6a73 6f6e 0a7b 0a20  ult:.```json.{. 
+00001c10: 2022 6964 223a 2022 6368 6174 636d 706c   "id": "chatcmpl
+00001c20: 2d38 6437 3662 3635 612d 6261 6430 2d34  -8d76b65a-bad0-4
+00001c30: 3265 662d 3931 3264 2d34 6130 3533 3364  2ef-912d-4a0533d
+00001c40: 3930 6436 3122 2c0a 2020 226d 6f64 656c  90d61",.  "model
+00001c50: 223a 2022 3536 6636 3936 3232 2d31 6537  ": "56f69622-1e7
+00001c60: 332d 3131 6565 2d61 3362 642d 3961 6639  3-11ee-a3bd-9af9
+00001c70: 6631 3638 3136 6336 222c 0a20 2022 6f62  f16816c6",.  "ob
+00001c80: 6a65 6374 223a 2022 6368 6174 2e63 6f6d  ject": "chat.com
+00001c90: 706c 6574 696f 6e22 2c0a 2020 2263 7265  pletion",.  "cre
+00001ca0: 6174 6564 223a 2031 3638 3839 3139 3138  ated": 168891918
+00001cb0: 372c 0a20 2022 6368 6f69 6365 7322 3a20  7,.  "choices": 
+00001cc0: 5b0a 2020 2020 7b0a 2020 2020 2020 2269  [.    {.      "i
+00001cd0: 6e64 6578 223a 2030 2c0a 2020 2020 2020  ndex": 0,.      
+00001ce0: 226d 6573 7361 6765 223a 207b 0a20 2020  "message": {.   
+00001cf0: 2020 2020 2022 726f 6c65 223a 2022 6173       "role": "as
+00001d00: 7369 7374 616e 7422 2c0a 2020 2020 2020  sistant",.      
+00001d10: 2020 2263 6f6e 7465 6e74 223a 2022 5468    "content": "Th
+00001d20: 6520 6c61 7267 6573 7420 616e 696d 616c  e largest animal
+00001d30: 2074 6861 7420 6861 7320 6265 656e 2073   that has been s
+00001d40: 6369 656e 7469 6669 6361 6c6c 7920 6d65  cientifically me
+00001d50: 6173 7572 6564 2069 7320 7468 6520 626c  asured is the bl
+00001d60: 7565 2077 6861 6c65 2c20 7768 6963 6820  ue whale, which 
+00001d70: 6861 7320 6120 6d61 7869 6d75 6d20 6c65  has a maximum le
+00001d80: 6e67 7468 206f 6620 6172 6f75 6e64 2032  ngth of around 2
+00001d90: 3320 6d65 7465 7273 2028 3735 2066 6565  3 meters (75 fee
+00001da0: 7429 2066 6f72 2061 6475 6c74 2061 6e69  t) for adult ani
+00001db0: 6d61 6c73 2061 6e64 2063 616e 2077 6569  mals and can wei
+00001dc0: 6768 2075 7020 746f 2031 3530 2c30 3030  gh up to 150,000
+00001dd0: 2070 6f75 6e64 7320 2836 382c 3030 3020   pounds (68,000 
+00001de0: 6b67 292e 2048 6f77 6576 6572 2c20 6974  kg). However, it
+00001df0: 2069 7320 696d 706f 7274 616e 7420 746f   is important to
+00001e00: 206e 6f74 6520 7468 6174 2074 6869 7320   note that this 
+00001e10: 6973 206a 7573 7420 616e 2065 7374 696d  is just an estim
+00001e20: 6174 6520 616e 6420 7468 6174 2074 6865  ate and that the
+00001e30: 206c 6172 6765 7374 2061 6e69 6d61 6c20   largest animal 
+00001e40: 6b6e 6f77 6e20 746f 2073 6369 656e 6365  known to science
+00001e50: 206d 6179 2062 6520 6c61 7267 6572 2073   may be larger s
+00001e60: 7469 6c6c 2e20 536f 6d65 2073 6369 656e  till. Some scien
+00001e70: 7469 7374 7320 6265 6c69 6576 6520 7468  tists believe th
+00001e80: 6174 2074 6865 206c 6172 6765 7374 2061  at the largest a
+00001e90: 6e69 6d61 6c73 206d 6179 206e 6f74 2068  nimals may not h
+00001ea0: 6176 6520 6120 636c 6561 7220 5c22 7369  ave a clear \"si
+00001eb0: 7a65 5c22 2069 6e20 7468 6520 7361 6d65  ze\" in the same
+00001ec0: 2077 6179 2074 6861 7420 6875 6d61 6e73   way that humans
+00001ed0: 2064 6f2c 2061 7320 7468 6569 7220 7369   do, as their si
+00001ee0: 7a65 2063 616e 2076 6172 7920 6465 7065  ze can vary depe
+00001ef0: 6e64 696e 6720 6f6e 2074 6865 2065 6e76  nding on the env
+00001f00: 6972 6f6e 6d65 6e74 2061 6e64 2074 6865  ironment and the
+00001f10: 2073 7461 6765 206f 6620 7468 6569 7220   stage of their 
+00001f20: 6c69 6665 2e22 0a20 2020 2020 207d 2c0a  life.".      },.
+00001f30: 2020 2020 2020 2266 696e 6973 685f 7265        "finish_re
+00001f40: 6173 6f6e 223a 2022 4e6f 6e65 220a 2020  ason": "None".  
+00001f50: 2020 7d0a 2020 5d2c 0a20 2022 7573 6167    }.  ],.  "usag
+00001f60: 6522 3a20 7b0a 2020 2020 2270 726f 6d70  e": {.    "promp
+00001f70: 745f 746f 6b65 6e73 223a 202d 312c 0a20  t_tokens": -1,. 
+00001f80: 2020 2022 636f 6d70 6c65 7469 6f6e 5f74     "completion_t
+00001f90: 6f6b 656e 7322 3a20 2d31 2c0a 2020 2020  okens": -1,.    
+00001fa0: 2274 6f74 616c 5f74 6f6b 656e 7322 3a20  "total_tokens": 
+00001fb0: 2d31 0a20 207d 0a7d 0a60 6060 0a0a 5365  -1.  }.}.```..Se
+00001fc0: 6520 5b65 7861 6d70 6c65 735d 2865 7861  e [examples](exa
+00001fd0: 6d70 6c65 7329 2066 6f72 206d 6f72 6520  mples) for more 
+00001fe0: 6578 616d 706c 6573 2e0a 0a0a 2323 2042  examples....## B
+00001ff0: 7569 6c74 696e 206d 6f64 656c 730a 546f  uiltin models.To
+00002000: 2076 6965 7720 7468 6520 6275 696c 7469   view the builti
+00002010: 6e20 6d6f 6465 6c73 2c20 7275 6e20 7468  n models, run th
+00002020: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00002030: 616e 643a 0a60 6060 6261 7368 0a24 2078  and:.```bash.$ x
+00002040: 696e 6665 7265 6e63 6520 6c69 7374 202d  inference list -
+00002050: 2d61 6c6c 0a60 6060 0a0a 7c20 4e61 6d65  -all.```..| Name
+00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002070: 207c 2054 7970 6520 2020 2020 2020 2020   | Type         
+00002080: 2020 2020 7c20 4c61 6e67 7561 6765 207c      | Language |
+00002090: 2046 6f72 6d61 7420 7c20 5369 7a65 2028   Format | Size (
+000020a0: 696e 2062 696c 6c69 6f6e 7329 207c 2051  in billions) | Q
+000020b0: 7561 6e74 697a 6174 696f 6e20 2020 2020  uantization     
+000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020d0: 2020 2020 2020 7c0a 7c20 2d2d 2d2d 2d2d        |.| ------
+000020e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+000020f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002100: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  --|----------|--
+00002110: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
+00002120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
+00002130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002150: 2d2d 2d2d 7c0a 7c20 6261 6963 6875 616e  ----|.| baichuan
+00002160: 2020 2020 2020 2020 2020 2020 207c 2046               | F
+00002170: 6f75 6e64 6174 696f 6e20 4d6f 6465 6c20  oundation Model 
+00002180: 7c20 656e 2c20 7a68 2020 207c 2067 676d  | en, zh   | ggm
+00002190: 6c76 3320 7c20 3720 2020 2020 2020 2020  lv3 | 7         
+000021a0: 2020 2020 2020 2020 207c 2027 7132 5f4b           | 'q2_K
+000021b0: 272c 2027 7133 5f4b 5f4c 272c 202e 2e2e  ', 'q3_K_L', ...
+000021c0: 202c 2027 7136 5f4b 272c 2027 7138 5f30   , 'q6_K', 'q8_0
+000021d0: 2720 7c0a 7c20 6368 6174 676c 6d20 2020  ' |.| chatglm   
+000021e0: 2020 2020 2020 2020 2020 207c 2053 4654             | SFT
+000021f0: 204d 6f64 656c 2020 2020 2020 2020 7c20   Model        | 
+00002200: 656e 2c20 7a68 2020 207c 2067 676d 6c76  en, zh   | ggmlv
+00002210: 3320 7c20 3620 2020 2020 2020 2020 2020  3 | 6           
+00002220: 2020 2020 2020 207c 2027 7134 5f30 272c         | 'q4_0',
+00002230: 2027 7134 5f31 272c 2027 7135 5f30 272c   'q4_1', 'q5_0',
+00002240: 2027 7135 5f31 272c 2027 7138 5f30 2720   'q5_1', 'q8_0' 
+00002250: 7c0a 7c20 6368 6174 676c 6d32 2020 2020  |.| chatglm2    
+00002260: 2020 2020 2020 2020 207c 2053 4654 204d           | SFT M
+00002270: 6f64 656c 2020 2020 2020 2020 7c20 656e  odel        | en
+00002280: 2c20 7a68 2020 207c 2067 676d 6c76 3320  , zh   | ggmlv3 
+00002290: 7c20 3620 2020 2020 2020 2020 2020 2020  | 6             
+000022a0: 2020 2020 207c 2027 7134 5f30 272c 2027       | 'q4_0', '
+000022b0: 7134 5f31 272c 2027 7135 5f30 272c 2027  q4_1', 'q5_0', '
+000022c0: 7135 5f31 272c 2027 7138 5f30 2720 7c0a  q5_1', 'q8_0' |.
+000022d0: 7c20 7769 7a61 7264 6c6d 2d76 312e 3020  | wizardlm-v1.0 
+000022e0: 2020 2020 2020 207c 2053 4654 204d 6f64         | SFT Mod
+000022f0: 656c 2020 2020 2020 2020 7c20 656e 2020  el        | en  
+00002300: 2020 2020 207c 2067 676d 6c76 3320 7c20       | ggmlv3 | 
+00002310: 372c 2031 332c 2033 3320 2020 2020 2020  7, 13, 33       
+00002320: 2020 207c 2027 7132 5f4b 272c 2027 7133     | 'q2_K', 'q3
+00002330: 5f4b 5f4c 272c 202e 2e2e 202c 2027 7136  _K_L', ... , 'q6
+00002340: 5f4b 272c 2027 7138 5f30 2720 7c0a 7c20  _K', 'q8_0' |.| 
+00002350: 7669 6375 6e61 2d76 312e 3320 2020 2020  vicuna-v1.3     
+00002360: 2020 2020 207c 2053 4654 204d 6f64 656c       | SFT Model
+00002370: 2020 2020 2020 2020 7c20 656e 2020 2020          | en    
+00002380: 2020 207c 2067 676d 6c76 3320 7c20 372c     | ggmlv3 | 7,
+00002390: 2031 3320 2020 2020 2020 2020 2020 2020   13             
+000023a0: 207c 2027 7132 5f4b 272c 2027 7133 5f4b   | 'q2_K', 'q3_K
+000023b0: 5f4c 272c 202e 2e2e 202c 2027 7136 5f4b  _L', ... , 'q6_K
+000023c0: 272c 2027 7138 5f30 2720 7c0a 7c20 6f72  ', 'q8_0' |.| or
+000023d0: 6361 2020 2020 2020 2020 2020 2020 2020  ca              
+000023e0: 2020 207c 2053 4654 204d 6f64 656c 2020     | SFT Model  
+000023f0: 2020 2020 2020 7c20 656e 2020 2020 2020        | en      
+00002400: 207c 2067 676d 6c76 3320 7c20 332c 2037   | ggmlv3 | 3, 7
+00002410: 2c20 3133 2020 2020 2020 2020 2020 207c  , 13           |
+00002420: 2027 7134 5f30 272c 2027 7134 5f31 272c   'q4_0', 'q4_1',
+00002430: 2027 7135 5f30 272c 2027 7135 5f31 272c   'q5_0', 'q5_1',
+00002440: 2027 7138 5f30 2720 7c0a 0a0a 2a2a 4e4f   'q8_0' |...**NO
+00002450: 5445 2a2a 3a0a 2d20 5869 6e66 6572 656e  TE**:.- Xinferen
+00002460: 6365 2077 696c 6c20 646f 776e 6c6f 6164  ce will download
+00002470: 206d 6f64 656c 7320 6175 746f 6d61 7469   models automati
+00002480: 6361 6c6c 7920 666f 7220 796f 752c 2061  cally for you, a
+00002490: 6e64 2062 7920 6465 6661 756c 7420 7468  nd by default th
+000024a0: 6520 6d6f 6465 6c73 2077 696c 6c20 6265  e models will be
+000024b0: 2073 6176 6564 2075 6e64 6572 2060 247b   saved under `${
+000024c0: 5553 4552 7d2f 2e78 696e 6665 7265 6e63  USER}/.xinferenc
+000024d0: 652f 6361 6368 6560 2e0a 2d20 466f 756e  e/cache`..- Foun
+000024e0: 6461 7469 6f6e 206d 6f64 656c 7320 6f6e  dation models on
+000024f0: 6c79 2070 726f 7669 6465 2069 6e74 6572  ly provide inter
+00002500: 6661 6365 2060 6765 6e65 7261 7465 602e  face `generate`.
+00002510: 0a2d 2053 4654 206d 6f64 656c 7320 7072  .- SFT models pr
+00002520: 6f76 6964 6520 626f 7468 2060 6765 6e65  ovide both `gene
+00002530: 7261 7465 6020 616e 6420 6063 6861 7460  rate` and `chat`
+00002540: 2e0a 0a23 2320 526f 6164 6d61 700a 5869  ...## Roadmap.Xi
+00002550: 6e66 6572 656e 6365 2069 7320 6375 7272  nference is curr
+00002560: 656e 746c 7920 756e 6465 7220 6163 7469  ently under acti
+00002570: 7665 2064 6576 656c 6f70 6d65 6e74 2e20  ve development. 
+00002580: 4865 7265 2773 2061 2072 6f61 646d 6170  Here's a roadmap
+00002590: 206f 7574 6c69 6e69 6e67 206f 7572 2070   outlining our p
+000025a0: 6c61 6e6e 6564 200a 6465 7665 6c6f 706d  lanned .developm
+000025b0: 656e 7473 2066 6f72 2074 6865 206e 6578  ents for the nex
+000025c0: 7420 6665 7720 7765 656b 733a 0a0a 2323  t few weeks:..##
+000025d0: 2320 5079 546f 7263 6820 5375 7070 6f72  # PyTorch Suppor
+000025e0: 740a 5769 7468 2050 7954 6f72 6368 2069  t.With PyTorch i
+000025f0: 6e74 6567 7261 7469 6f6e 2c20 7573 6572  ntegration, user
+00002600: 7320 7769 6c6c 2062 6520 6162 6c65 2074  s will be able t
+00002610: 6f20 7365 616d 6c65 7373 6c79 2075 7469  o seamlessly uti
+00002620: 6c69 7a65 2050 7954 6f72 6368 206d 6f64  lize PyTorch mod
+00002630: 656c 7320 6672 6f6d 2048 7567 6769 6e67  els from Hugging
+00002640: 2046 6163 650a 7769 7468 696e 2058 696e   Face.within Xin
+00002650: 6665 7265 6e63 652e 0a0a 2323 2320 4c61  ference...### La
+00002660: 6e67 6368 6169 6e20 2620 4c6c 616d 6149  ngchain & LlamaI
+00002670: 6e64 6578 2069 6e74 6567 7261 7469 6f6e  ndex integration
+00002680: 0a57 6974 6820 5869 6e66 6572 656e 6365  .With Xinference
+00002690: 2c20 6974 2077 696c 6c20 6265 206d 7563  , it will be muc
+000026a0: 6820 6561 7369 6572 2066 6f72 2075 7365  h easier for use
+000026b0: 7273 2074 6f20 7573 6520 7468 6573 6520  rs to use these 
+000026c0: 6c69 6272 6172 6965 7320 616e 6420 6275  libraries and bu
+000026d0: 696c 6420 6170 706c 6963 6174 696f 6e73  ild applications
+000026e0: 200a 7769 7468 204c 4c4d 732e 0a          .with LLMs..
```

### Comparing `xinference-0.0.2/README.md` & `xinference-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,461 +100,472 @@
 00000630: 6665 7265 6e63 6527 7320 7375 7070 6f72  ference's suppor
 00000640: 7420 746f 2069 6e63 6c75 6465 2061 6464  t to include add
 00000650: 6974 696f 6e61 6c20 7275 6e74 696d 6573  itional runtimes
 00000660: 2c20 0a69 6e63 6c75 6469 6e67 2050 7954  , .including PyT
 00000670: 6f72 6368 2061 6e64 204a 4158 2c20 696e  orch and JAX, in
 00000680: 2074 6865 206e 6561 7220 6675 7475 7265   the near future
 00000690: 2e0a 0a21 5b64 656d 6f5d 2861 7373 6574  ...![demo](asset
-000006a0: 732f 6465 6d6f 2e67 6966 290a 0a0a 2323  s/demo.gif)...##
-000006b0: 204b 6579 2046 6561 7475 7265 730a f09f   Key Features...
-000006c0: 8c9f 202a 2a4d 6f64 656c 2053 6572 7669  .. **Model Servi
-000006d0: 6e67 204d 6164 6520 4561 7379 2a2a 3a20  ng Made Easy**: 
-000006e0: 496e 6665 7265 6e63 6520 7369 6d70 6c69  Inference simpli
-000006f0: 6669 6573 2074 6865 2070 726f 6365 7373  fies the process
-00000700: 206f 6620 7365 7276 696e 6720 6c61 7267   of serving larg
-00000710: 6520 6c61 6e67 7561 6765 2c20 7370 6565  e language, spee
-00000720: 6368 200a 7265 636f 676e 6974 696f 6e2c  ch .recognition,
-00000730: 2061 6e64 206d 756c 7469 6d6f 6461 6c20   and multimodal 
-00000740: 6d6f 6465 6c73 2e20 596f 7520 6361 6e20  models. You can 
-00000750: 7365 7420 7570 2061 6e64 2064 6570 6c6f  set up and deplo
-00000760: 7920 796f 7572 206d 6f64 656c 730a 666f  y your models.fo
-00000770: 7220 6578 7065 7269 6d65 6e74 6174 696f  r experimentatio
-00000780: 6e20 616e 6420 7072 6f64 7563 7469 6f6e  n and production
-00000790: 2077 6974 6820 6120 7369 6e67 6c65 2063   with a single c
-000007a0: 6f6d 6d61 6e64 2e0a 0ae2 9aa1 efb8 8f20  ommand......... 
-000007b0: 2a2a 5374 6174 652d 6f66 2d74 6865 2d41  **State-of-the-A
-000007c0: 7274 204d 6f64 656c 732a 2a3a 2045 7870  rt Models**: Exp
-000007d0: 6572 696d 656e 7420 7769 7468 2063 7574  eriment with cut
-000007e0: 7469 6e67 2d65 6467 6520 6275 696c 742d  ting-edge built-
-000007f0: 696e 206d 6f64 656c 7320 7573 696e 6720  in models using 
-00000800: 6120 7369 6e67 6c65 200a 636f 6d6d 616e  a single .comman
-00000810: 642e 2049 6e66 6572 656e 6365 2070 726f  d. Inference pro
-00000820: 7669 6465 7320 6163 6365 7373 2074 6f20  vides access to 
-00000830: 7374 6174 652d 6f66 2d74 6865 2d61 7274  state-of-the-art
-00000840: 206f 7065 6e2d 736f 7572 6365 206d 6f64   open-source mod
-00000850: 656c 7321 0a0a f09f 96a5 202a 2a48 6574  els!...... **Het
-00000860: 6572 6f67 656e 656f 7573 2048 6172 6477  erogeneous Hardw
-00000870: 6172 6520 5574 696c 697a 6174 696f 6e2a  are Utilization*
-00000880: 2a3a 204d 616b 6520 7468 6520 6d6f 7374  *: Make the most
-00000890: 206f 6620 796f 7572 2068 6172 6477 6172   of your hardwar
-000008a0: 6520 7265 736f 7572 6365 732e 2058 6f72  e resources. Xor
-000008b0: 6269 7473 200a 496e 6665 7265 6e63 6520  bits .Inference 
-000008c0: 696e 7465 6c6c 6967 656e 746c 7920 7574  intelligently ut
-000008d0: 696c 697a 6573 2068 6574 6572 6f67 656e  ilizes heterogen
-000008e0: 656f 7573 2068 6172 6477 6172 652c 2069  eous hardware, i
-000008f0: 6e63 6c75 6469 6e67 2047 5055 7320 616e  ncluding GPUs an
-00000900: 6420 4350 5573 2c20 746f 206d 6178 696d  d CPUs, to maxim
-00000910: 697a 650a 7065 7266 6f72 6d61 6e63 6520  ize.performance 
-00000920: 616e 6420 6163 6365 6c65 7261 7465 2079  and accelerate y
-00000930: 6f75 7220 6d6f 6465 6c20 696e 6665 7265  our model infere
-00000940: 6e63 6520 7461 736b 732e 0a0a e29a 99ef  nce tasks.......
-00000950: b88f 202a 2a46 6c65 7869 626c 6520 4150  .. **Flexible AP
-00000960: 4920 616e 6420 496e 7465 7266 6163 6573  I and Interfaces
-00000970: 2a2a 3a20 586f 7262 6974 7320 496e 6665  **: Xorbits Infe
-00000980: 7265 6e63 6520 6f66 6665 7273 206d 756c  rence offers mul
-00000990: 7469 706c 6520 696e 7465 7266 6163 6573  tiple interfaces
-000009a0: 2066 6f72 2069 6e74 6572 6163 7469 6e67   for interacting
-000009b0: 0a77 6974 6820 796f 7572 206d 6f64 656c  .with your model
-000009c0: 732e 2059 6f75 2063 616e 2075 7469 6c69  s. You can utili
-000009d0: 7a65 2074 6865 2052 5043 2061 6e64 2052  ze the RPC and R
-000009e0: 4553 5466 756c 2041 5049 2863 6f6d 7061  ESTful API(compa
-000009f0: 7469 626c 6520 7769 7468 204f 7065 6e41  tible with OpenA
-00000a00: 4920 4150 4929 2074 6f20 696e 7465 6772  I API) to integr
-00000a10: 6174 650a 796f 7572 206d 6f64 656c 7320  ate.your models 
-00000a20: 7769 7468 2065 7869 7374 696e 6720 7379  with existing sy
-00000a30: 7374 656d 7320 6f72 2075 7365 2074 6865  stems or use the
-00000a40: 2063 6f6d 6d61 6e64 2d6c 696e 6520 696e   command-line in
-00000a50: 7465 7266 6163 6520 2843 4c49 2920 616e  terface (CLI) an
-00000a60: 6420 7468 6520 696e 7475 6974 6976 6520  d the intuitive 
-00000a70: 5765 6255 490a 666f 7220 7365 616d 6c65  WebUI.for seamle
-00000a80: 7373 206d 616e 6167 656d 656e 7420 616e  ss management an
-00000a90: 6420 6d6f 6e69 746f 7269 6e67 2e0a 0af0  d monitoring....
-00000aa0: 9f8c 9020 2a2a 4469 7374 7269 6275 7465  ... **Distribute
-00000ab0: 6420 4465 706c 6f79 6d65 6e74 2a2a 3a20  d Deployment**: 
-00000ac0: 586f 7262 6974 7320 496e 6665 7265 6e63  Xorbits Inferenc
-00000ad0: 6520 6578 6365 6c73 2069 6e20 6469 7374  e excels in dist
-00000ae0: 7269 6275 7465 6420 6465 706c 6f79 6d65  ributed deployme
-00000af0: 6e74 2073 6365 6e61 7269 6f73 2c20 0a61  nt scenarios, .a
-00000b00: 6c6c 6f77 696e 6720 7468 6520 7365 616d  llowing the seam
-00000b10: 6c65 7373 2064 6973 7472 6962 7574 696f  less distributio
-00000b20: 6e20 6f66 206d 6f64 656c 2069 6e66 6572  n of model infer
-00000b30: 656e 6365 2061 6372 6f73 7320 6d75 6c74  ence across mult
-00000b40: 6970 6c65 2064 6576 6963 6573 206f 7220  iple devices or 
-00000b50: 6d61 6368 696e 6573 2e20 4974 0a6c 6576  machines. It.lev
-00000b60: 6572 6167 6573 2064 6973 7472 6962 7574  erages distribut
-00000b70: 6564 2063 6f6d 7075 7469 6e67 2074 6563  ed computing tec
-00000b80: 686e 6971 7565 7320 746f 2070 6172 616c  hniques to paral
-00000b90: 6c65 6c69 7a65 2061 6e64 2073 6361 6c65  lelize and scale
-00000ba0: 2074 6865 2069 6e66 6572 656e 6365 2070   the inference p
-00000bb0: 726f 6365 7373 2e0a 0af0 9f94 8c20 2a2a  rocess....... **
-00000bc0: 4275 696c 742d 696e 2049 6e74 6567 7261  Built-in Integra
-00000bd0: 7469 6f6e 2077 6974 6820 5468 6972 642d  tion with Third-
-00000be0: 5061 7274 7920 4c69 6272 6172 6965 732a  Party Libraries*
-00000bf0: 2a3a 2058 6f72 6269 7473 2049 6e66 6572  *: Xorbits Infer
-00000c00: 656e 6365 2073 6561 6d6c 6573 736c 7920  ence seamlessly 
-00000c10: 696e 7465 6772 6174 6573 0a77 6974 6820  integrates.with 
-00000c20: 706f 7075 6c61 7220 7468 6972 642d 7061  popular third-pa
-00000c30: 7274 7920 6c69 6272 6172 6965 7320 6c69  rty libraries li
-00000c40: 6b65 204c 616e 6743 6861 696e 2061 6e64  ke LangChain and
-00000c50: 204c 6c61 6d61 496e 6465 782e 2028 436f   LlamaIndex. (Co
-00000c60: 6d69 6e67 2073 6f6f 6e29 0a0a 2323 2047  ming soon)..## G
-00000c70: 6574 7469 6e67 2053 7461 7274 6564 0a58  etting Started.X
-00000c80: 696e 6665 7265 6e63 6520 6361 6e20 6265  inference can be
-00000c90: 2069 6e73 7461 6c6c 6564 2076 6961 2070   installed via p
-00000ca0: 6970 2066 726f 6d20 5079 5049 2e20 4974  ip from PyPI. It
-00000cb0: 2069 7320 6869 6768 6c79 2072 6563 6f6d   is highly recom
-00000cc0: 6d65 6e64 6564 2074 6f20 6372 6561 7465  mended to create
-00000cd0: 2061 206e 6577 2076 6972 7475 616c 0a65   a new virtual.e
-00000ce0: 6e76 6972 6f6e 6d65 6e74 2074 6f20 6176  nvironment to av
-00000cf0: 6f69 6420 636f 6e66 6c69 6374 732e 0a60  oid conflicts..`
-00000d00: 6060 6261 7368 0a24 2070 6970 2069 6e73  ``bash.$ pip ins
-00000d10: 7461 6c6c 2022 7869 6e66 6572 656e 6365  tall "xinference
-00000d20: 5b61 6c6c 5d22 0a60 6060 0a22 7869 6e66  [all]".```."xinf
-00000d30: 6572 656e 6365 5b61 6c6c 5d22 2069 6e73  erence[all]" ins
-00000d40: 7461 6c6c 7320 616c 6c20 7468 6520 6e65  talls all the ne
-00000d50: 6365 7373 6172 7920 7061 636b 6167 6573  cessary packages
-00000d60: 2066 6f72 2073 6572 7669 6e67 206d 6f64   for serving mod
-00000d70: 656c 732e 2049 6620 796f 7520 7761 6e74  els. If you want
-00000d80: 2074 6f20 6163 6869 6576 6520 6163 6365   to achieve acce
-00000d90: 6c65 7261 7469 6f6e 206f 6e20 0a64 6966  leration on .dif
-00000da0: 6665 7265 6e74 2068 6172 6477 6172 652c  ferent hardware,
-00000db0: 2072 6566 6572 2074 6f20 7468 6520 696e   refer to the in
-00000dc0: 7374 616c 6c61 7469 6f6e 2064 6f63 756d  stallation docum
-00000dd0: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
-00000de0: 636f 7272 6573 706f 6e64 696e 6720 7061  corresponding pa
-00000df0: 636b 6167 652e 0a2d 205b 6c6c 616d 612d  ckage..- [llama-
-00000e00: 6370 702d 7079 7468 6f6e 5d28 6874 7470  cpp-python](http
-00000e10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00000e20: 6265 746c 656e 2f6c 6c61 6d61 2d63 7070  betlen/llama-cpp
-00000e30: 2d70 7974 686f 6e23 696e 7374 616c 6c61  -python#installa
-00000e40: 7469 6f6e 2d66 726f 6d2d 7079 7069 2d72  tion-from-pypi-r
-00000e50: 6563 6f6d 6d65 6e64 6564 2920 6973 2072  ecommended) is r
-00000e60: 6571 7569 7265 6420 746f 2072 756e 2060  equired to run `
-00000e70: 6261 6963 6875 616e 602c 2060 7769 7a61  baichuan`, `wiza
-00000e80: 7264 6c6d 2d76 312e 3060 2c20 6076 6963  rdlm-v1.0`, `vic
-00000e90: 756e 612d 7631 2e33 6020 616e 6420 606f  una-v1.3` and `o
-00000ea0: 7263 6160 2e0a 2d20 5b63 6861 7467 6c6d  rca`..- [chatglm
-00000eb0: 2d63 7070 2d70 7974 686f 6e5d 2868 7474  -cpp-python](htt
-00000ec0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000ed0: 6c69 2d70 6c75 732f 6368 6174 676c 6d2e  li-plus/chatglm.
-00000ee0: 6370 7023 6765 7474 696e 672d 7374 6172  cpp#getting-star
-00000ef0: 7465 6429 2069 7320 7265 7175 6972 6564  ted) is required
-00000f00: 2074 6f20 7275 6e20 6063 6861 7467 6c6d   to run `chatglm
-00000f10: 6020 616e 6420 6063 6861 7467 6c6d 3260  ` and `chatglm2`
-00000f20: 2e0a 0a0a 2323 2320 4465 706c 6f79 6d65  ....### Deployme
-00000f30: 6e74 0a59 6f75 2063 616e 2064 6570 6c6f  nt.You can deplo
-00000f40: 7920 5869 6e66 6572 656e 6365 206c 6f63  y Xinference loc
-00000f50: 616c 6c79 2077 6974 6820 6120 7369 6e67  ally with a sing
-00000f60: 6c65 2063 6f6d 6d61 6e64 206f 7220 6465  le command or de
-00000f70: 706c 6f79 2069 7420 696e 2061 2064 6973  ploy it in a dis
-00000f80: 7472 6962 7574 6564 2063 6c75 7374 6572  tributed cluster
-00000f90: 2e20 0a0a 2323 2323 204c 6f63 616c 0a54  . ..#### Local.T
-00000fa0: 6f20 7374 6172 7420 6120 6c6f 6361 6c20  o start a local 
-00000fb0: 696e 7374 616e 6365 206f 6620 5869 6e66  instance of Xinf
-00000fc0: 6572 656e 6365 2c20 7275 6e20 7468 6520  erence, run the 
-00000fd0: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-00000fe0: 643a 0a60 6060 6261 7368 0a24 2078 696e  d:.```bash.$ xin
-00000ff0: 6665 7265 6e63 650a 6060 600a 0a23 2323  ference.```..###
-00001000: 2320 4469 7374 7269 6275 7465 640a 0a54  # Distributed..T
-00001010: 6f20 6465 706c 6f79 2058 696e 6665 7265  o deploy Xinfere
-00001020: 6e63 6520 696e 2061 2063 6c75 7374 6572  nce in a cluster
-00001030: 2c20 796f 7520 6e65 6564 2074 6f20 7374  , you need to st
-00001040: 6172 7420 6120 5869 6e66 6572 656e 6365  art a Xinference
-00001050: 2073 7570 6572 7669 736f 7220 6f6e 206f   supervisor on o
-00001060: 6e65 2073 6572 7665 7220 616e 6420 0a58  ne server and .X
-00001070: 696e 6665 7265 6e63 6520 776f 726b 6572  inference worker
-00001080: 7320 6f6e 2074 6865 206f 7468 6572 2073  s on the other s
-00001090: 6572 7665 7273 2e20 466f 6c6c 6f77 2074  ervers. Follow t
-000010a0: 6865 2073 7465 7073 2062 656c 6f77 3a0a  he steps below:.
-000010b0: 0a2a 2a53 7461 7274 696e 6720 7468 6520  .**Starting the 
-000010c0: 5375 7065 7276 6973 6f72 2a2a 3a20 4f6e  Supervisor**: On
-000010d0: 2074 6865 2073 6572 7665 7220 7768 6572   the server wher
-000010e0: 6520 796f 7520 7761 6e74 2074 6f20 7275  e you want to ru
-000010f0: 6e20 7468 6520 5869 6e66 6572 656e 6365  n the Xinference
-00001100: 2073 7570 6572 7669 736f 722c 2072 756e   supervisor, run
-00001110: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00001120: 6f6d 6d61 6e64 3a0a 6060 6062 6173 680a  ommand:.```bash.
-00001130: 2420 7869 6e66 6572 656e 6365 2d73 7570  $ xinference-sup
-00001140: 6572 7669 736f 7220 2d48 2022 247b 7375  ervisor -H "${su
-00001150: 7065 7276 6973 6f72 5f68 6f73 747d 220a  pervisor_host}".
-00001160: 6060 600a 5265 706c 6163 6520 6024 7b73  ```.Replace `${s
-00001170: 7570 6572 7669 736f 725f 686f 7374 7d60  upervisor_host}`
-00001180: 2077 6974 6820 7468 6520 6163 7475 616c   with the actual
-00001190: 2068 6f73 7420 6f66 2079 6f75 7220 7375   host of your su
-000011a0: 7065 7276 6973 6f72 2073 6572 7665 722e  pervisor server.
-000011b0: 0a0a 2a2a 5374 6172 7469 6e67 2074 6865  ..**Starting the
-000011c0: 2057 6f72 6b65 7273 2a2a 3a20 4f6e 2065   Workers**: On e
-000011d0: 6163 6820 6f66 2074 6865 206f 7468 6572  ach of the other
-000011e0: 2073 6572 7665 7273 2077 6865 7265 2079   servers where y
-000011f0: 6f75 2077 616e 7420 746f 2072 756e 2058  ou want to run X
-00001200: 696e 6665 7265 6e63 6520 776f 726b 6572  inference worker
-00001210: 732c 2072 756e 2074 6865 2066 6f6c 6c6f  s, run the follo
-00001220: 7769 6e67 2063 6f6d 6d61 6e64 3a0a 6060  wing command:.``
-00001230: 6062 6173 680a 2420 7869 6e66 6572 656e  `bash.$ xinferen
-00001240: 6365 2d77 6f72 6b65 7220 2d65 2022 6874  ce-worker -e "ht
-00001250: 7470 3a2f 2f24 7b73 7570 6572 7669 736f  tp://${superviso
-00001260: 725f 686f 7374 7d3a 3939 3937 220a 6060  r_host}:9997".``
-00001270: 600a 0a4f 6e63 6520 5869 6e66 6572 656e  `..Once Xinferen
-00001280: 6365 2069 7320 7275 6e6e 696e 672c 2061  ce is running, a
-00001290: 6e20 656e 6470 6f69 6e74 2077 696c 6c20  n endpoint will 
-000012a0: 6265 2061 6363 6573 7369 626c 6520 666f  be accessible fo
-000012b0: 7220 6d6f 6465 6c20 6d61 6e61 6765 6d65  r model manageme
-000012c0: 6e74 2076 6961 2043 4c49 206f 720a 5869  nt via CLI or.Xi
-000012d0: 6e66 6572 656e 6365 2020 636c 6965 6e74  nference  client
-000012e0: 2e0a 0a2d 2046 6f72 206c 6f63 616c 2064  ...- For local d
-000012f0: 6570 6c6f 796d 656e 742c 2074 6865 2065  eployment, the e
-00001300: 6e64 706f 696e 7420 7769 6c6c 2062 6520  ndpoint will be 
-00001310: 6068 7474 703a 2f2f 6c6f 6361 6c68 6f73  `http://localhos
-00001320: 743a 3939 3937 602e 0a2d 2046 6f72 2063  t:9997`..- For c
-00001330: 6c75 7374 6572 2064 6570 6c6f 796d 656e  luster deploymen
-00001340: 742c 2074 6865 2065 6e64 706f 696e 7420  t, the endpoint 
-00001350: 7769 6c6c 2062 6520 6068 7474 703a 2f2f  will be `http://
-00001360: 247b 7375 7065 7276 6973 6f72 5f68 6f73  ${supervisor_hos
-00001370: 747d 3a39 3939 3760 2c20 7768 6572 650a  t}:9997`, where.
-00001380: 6024 7b73 7570 6572 7669 736f 725f 686f  `${supervisor_ho
-00001390: 7374 7d60 2069 7320 7468 6520 686f 7374  st}` is the host
-000013a0: 6e61 6d65 206f 7220 4950 2061 6464 7265  name or IP addre
-000013b0: 7373 206f 6620 7468 6520 7365 7276 6572  ss of the server
-000013c0: 2077 6865 7265 2074 6865 2073 7570 6572   where the super
-000013d0: 7669 736f 7220 6973 2072 756e 6e69 6e67  visor is running
-000013e0: 2e0a 0a59 6f75 2063 616e 2061 6c73 6f20  ...You can also 
-000013f0: 7669 6577 2061 2077 6562 2055 4920 7573  view a web UI us
-00001400: 696e 6720 7468 6520 5869 6e66 6572 656e  ing the Xinferen
-00001410: 6365 2065 6e64 706f 696e 7420 746f 2063  ce endpoint to c
-00001420: 6861 7420 7769 7468 2061 6c6c 2074 6865  hat with all the
-00001430: 200a 6275 696c 7469 6e20 6d6f 6465 6c73   .builtin models
-00001440: 2e20 596f 7520 6361 6e20 6576 656e 202a  . You can even *
-00001450: 2a63 6861 7420 7769 7468 2074 776f 2063  *chat with two c
-00001460: 7574 7469 6e67 2d65 6467 6520 4149 206d  utting-edge AI m
-00001470: 6f64 656c 7320 7369 6465 2d62 792d 7369  odels side-by-si
-00001480: 6465 2074 6f20 636f 6d70 6172 650a 7468  de to compare.th
-00001490: 6569 7220 7065 7266 6f72 6d61 6e63 652a  eir performance*
-000014a0: 2a21 0a0a 215b 7765 6220 5549 5d28 6173  *!..![web UI](as
-000014b0: 7365 7473 2f78 696e 6665 7265 6e63 652d  sets/xinference-
-000014c0: 646f 776e 6c6f 6164 696e 672e 706e 6729  downloading.png)
-000014d0: 0a0a 2323 2320 5869 6e66 6572 656e 6365  ..### Xinference
-000014e0: 2043 4c49 0a58 696e 6665 7265 6e63 6520   CLI.Xinference 
-000014f0: 7072 6f76 6964 6573 2061 2063 6f6d 6d61  provides a comma
-00001500: 6e64 206c 696e 6520 696e 7465 7266 6163  nd line interfac
-00001510: 6520 2843 4c49 2920 666f 7220 6d6f 6465  e (CLI) for mode
-00001520: 6c20 6d61 6e61 6765 6d65 6e74 2e20 4865  l management. He
-00001530: 7265 2061 7265 2073 6f6d 6520 7573 6566  re are some usef
-00001540: 756c 200a 636f 6d6d 616e 6473 3a0a 0a2d  ul .commands:..-
-00001550: 204c 6175 6e63 6820 6120 6d6f 6465 6c20   Launch a model 
-00001560: 2861 206d 6f64 656c 2055 4944 2077 696c  (a model UID wil
-00001570: 6c20 6265 2072 6574 7572 6e65 6429 3a20  l be returned): 
-00001580: 6078 696e 6665 7265 6e63 6520 6c61 756e  `xinference laun
-00001590: 6368 600a 2d20 4c69 7374 2072 756e 6e69  ch`.- List runni
-000015a0: 6e67 206d 6f64 656c 733a 2060 7869 6e66  ng models: `xinf
-000015b0: 6572 656e 6365 206c 6973 7460 0a2d 204c  erence list`.- L
-000015c0: 6973 7420 616c 6c20 7468 6520 6275 696c  ist all the buil
-000015d0: 7469 6e20 6d6f 6465 6c73 3a20 6078 696e  tin models: `xin
-000015e0: 6665 7265 6e63 6520 6c69 7374 202d 2d61  ference list --a
-000015f0: 6c6c 600a 2d20 5465 726d 696e 6174 6520  ll`.- Terminate 
-00001600: 6120 6d6f 6465 6c3a 2060 7869 6e66 6572  a model: `xinfer
-00001610: 656e 6365 2074 6572 6d69 6e61 7465 202d  ence terminate -
-00001620: 2d6d 6f64 656c 2d75 6964 2024 7b6d 6f64  -model-uid ${mod
-00001630: 656c 5f75 6964 7d60 0a0a 2323 2320 5869  el_uid}`..### Xi
-00001640: 6e66 6572 656e 6365 2043 6c69 656e 740a  nference Client.
-00001650: 5869 6e66 6572 656e 6365 2061 6c73 6f20  Xinference also 
-00001660: 7072 6f76 6964 6573 2061 2063 6c69 656e  provides a clien
-00001670: 7420 666f 7220 6d61 6e61 6769 6e67 2061  t for managing a
-00001680: 6e64 2061 6363 6573 7369 6e67 206d 6f64  nd accessing mod
-00001690: 656c 7320 7072 6f67 7261 6d6d 6174 6963  els programmatic
-000016a0: 616c 6c79 3a0a 0a60 6060 7079 7468 6f6e  ally:..```python
-000016b0: 0a66 726f 6d20 7869 6e66 6572 656e 6365  .from xinference
-000016c0: 2e63 6c69 656e 7420 696d 706f 7274 2043  .client import C
-000016d0: 6c69 656e 740a 0a63 6c69 656e 7420 3d20  lient..client = 
-000016e0: 436c 6965 6e74 2822 6874 7470 3a2f 2f6c  Client("http://l
-000016f0: 6f63 616c 686f 7374 3a39 3939 3722 290a  ocalhost:9997").
-00001700: 6d6f 6465 6c5f 7569 6420 3d20 636c 6965  model_uid = clie
-00001710: 6e74 2e6c 6175 6e63 685f 6d6f 6465 6c28  nt.launch_model(
-00001720: 6d6f 6465 6c5f 6e61 6d65 3d22 6368 6174  model_name="chat
-00001730: 676c 6d32 2229 0a6d 6f64 656c 203d 2063  glm2").model = c
-00001740: 6c69 656e 742e 6765 745f 6d6f 6465 6c28  lient.get_model(
-00001750: 6d6f 6465 6c5f 7569 6429 0a0a 6368 6174  model_uid)..chat
-00001760: 5f68 6973 746f 7279 203d 205b 5d0a 7072  _history = [].pr
-00001770: 6f6d 7074 203d 2022 5768 6174 2069 7320  ompt = "What is 
-00001780: 7468 6520 6c61 7267 6573 7420 616e 696d  the largest anim
-00001790: 616c 3f22 0a6d 6f64 656c 2e63 6861 7428  al?".model.chat(
-000017a0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-000017b0: 6d70 742c 0a20 2020 2020 2020 2020 2020  mpt,.           
-000017c0: 2063 6861 745f 6869 7374 6f72 792c 0a20   chat_history,. 
-000017d0: 2020 2020 2020 2020 2020 2067 656e 6572             gener
-000017e0: 6174 655f 636f 6e66 6967 3d7b 226d 6178  ate_config={"max
-000017f0: 5f74 6f6b 656e 7322 3a20 3130 3234 7d0a  _tokens": 1024}.
-00001800: 2020 2020 2020 2020 290a 6060 600a 0a52          ).```..R
-00001810: 6573 756c 743a 0a60 6060 6a73 6f6e 0a7b  esult:.```json.{
-00001820: 0a20 2022 6964 223a 2022 6368 6174 636d  .  "id": "chatcm
-00001830: 706c 2d38 6437 3662 3635 612d 6261 6430  pl-8d76b65a-bad0
-00001840: 2d34 3265 662d 3931 3264 2d34 6130 3533  -42ef-912d-4a053
-00001850: 3364 3930 6436 3122 2c0a 2020 226d 6f64  3d90d61",.  "mod
-00001860: 656c 223a 2022 3536 6636 3936 3232 2d31  el": "56f69622-1
-00001870: 6537 332d 3131 6565 2d61 3362 642d 3961  e73-11ee-a3bd-9a
-00001880: 6639 6631 3638 3136 6336 222c 0a20 2022  f9f16816c6",.  "
-00001890: 6f62 6a65 6374 223a 2022 6368 6174 2e63  object": "chat.c
-000018a0: 6f6d 706c 6574 696f 6e22 2c0a 2020 2263  ompletion",.  "c
-000018b0: 7265 6174 6564 223a 2031 3638 3839 3139  reated": 1688919
-000018c0: 3138 372c 0a20 2022 6368 6f69 6365 7322  187,.  "choices"
-000018d0: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
-000018e0: 2269 6e64 6578 223a 2030 2c0a 2020 2020  "index": 0,.    
-000018f0: 2020 226d 6573 7361 6765 223a 207b 0a20    "message": {. 
-00001900: 2020 2020 2020 2022 726f 6c65 223a 2022         "role": "
-00001910: 6173 7369 7374 616e 7422 2c0a 2020 2020  assistant",.    
-00001920: 2020 2020 2263 6f6e 7465 6e74 223a 2022      "content": "
-00001930: 5468 6520 6c61 7267 6573 7420 616e 696d  The largest anim
-00001940: 616c 2074 6861 7420 6861 7320 6265 656e  al that has been
-00001950: 2073 6369 656e 7469 6669 6361 6c6c 7920   scientifically 
-00001960: 6d65 6173 7572 6564 2069 7320 7468 6520  measured is the 
-00001970: 626c 7565 2077 6861 6c65 2c20 7768 6963  blue whale, whic
-00001980: 6820 6861 7320 6120 6d61 7869 6d75 6d20  h has a maximum 
-00001990: 6c65 6e67 7468 206f 6620 6172 6f75 6e64  length of around
-000019a0: 2032 3320 6d65 7465 7273 2028 3735 2066   23 meters (75 f
-000019b0: 6565 7429 2066 6f72 2061 6475 6c74 2061  eet) for adult a
-000019c0: 6e69 6d61 6c73 2061 6e64 2063 616e 2077  nimals and can w
-000019d0: 6569 6768 2075 7020 746f 2031 3530 2c30  eigh up to 150,0
-000019e0: 3030 2070 6f75 6e64 7320 2836 382c 3030  00 pounds (68,00
-000019f0: 3020 6b67 292e 2048 6f77 6576 6572 2c20  0 kg). However, 
-00001a00: 6974 2069 7320 696d 706f 7274 616e 7420  it is important 
-00001a10: 746f 206e 6f74 6520 7468 6174 2074 6869  to note that thi
-00001a20: 7320 6973 206a 7573 7420 616e 2065 7374  s is just an est
-00001a30: 696d 6174 6520 616e 6420 7468 6174 2074  imate and that t
-00001a40: 6865 206c 6172 6765 7374 2061 6e69 6d61  he largest anima
-00001a50: 6c20 6b6e 6f77 6e20 746f 2073 6369 656e  l known to scien
-00001a60: 6365 206d 6179 2062 6520 6c61 7267 6572  ce may be larger
-00001a70: 2073 7469 6c6c 2e20 536f 6d65 2073 6369   still. Some sci
-00001a80: 656e 7469 7374 7320 6265 6c69 6576 6520  entists believe 
-00001a90: 7468 6174 2074 6865 206c 6172 6765 7374  that the largest
-00001aa0: 2061 6e69 6d61 6c73 206d 6179 206e 6f74   animals may not
-00001ab0: 2068 6176 6520 6120 636c 6561 7220 5c22   have a clear \"
-00001ac0: 7369 7a65 5c22 2069 6e20 7468 6520 7361  size\" in the sa
-00001ad0: 6d65 2077 6179 2074 6861 7420 6875 6d61  me way that huma
-00001ae0: 6e73 2064 6f2c 2061 7320 7468 6569 7220  ns do, as their 
-00001af0: 7369 7a65 2063 616e 2076 6172 7920 6465  size can vary de
-00001b00: 7065 6e64 696e 6720 6f6e 2074 6865 2065  pending on the e
-00001b10: 6e76 6972 6f6e 6d65 6e74 2061 6e64 2074  nvironment and t
-00001b20: 6865 2073 7461 6765 206f 6620 7468 6569  he stage of thei
-00001b30: 7220 6c69 6665 2e22 0a20 2020 2020 207d  r life.".      }
-00001b40: 2c0a 2020 2020 2020 2266 696e 6973 685f  ,.      "finish_
-00001b50: 7265 6173 6f6e 223a 2022 4e6f 6e65 220a  reason": "None".
-00001b60: 2020 2020 7d0a 2020 5d2c 0a20 2022 7573      }.  ],.  "us
-00001b70: 6167 6522 3a20 7b0a 2020 2020 2270 726f  age": {.    "pro
-00001b80: 6d70 745f 746f 6b65 6e73 223a 202d 312c  mpt_tokens": -1,
-00001b90: 0a20 2020 2022 636f 6d70 6c65 7469 6f6e  .    "completion
-00001ba0: 5f74 6f6b 656e 7322 3a20 2d31 2c0a 2020  _tokens": -1,.  
-00001bb0: 2020 2274 6f74 616c 5f74 6f6b 656e 7322    "total_tokens"
-00001bc0: 3a20 2d31 0a20 207d 0a7d 0a60 6060 0a0a  : -1.  }.}.```..
-00001bd0: 5365 6520 5b65 7861 6d70 6c65 735d 2865  See [examples](e
-00001be0: 7861 6d70 6c65 7329 2066 6f72 206d 6f72  xamples) for mor
-00001bf0: 6520 6578 616d 706c 6573 2e0a 0a0a 2323  e examples....##
-00001c00: 2042 7569 6c74 696e 206d 6f64 656c 730a   Builtin models.
-00001c10: 546f 2076 6965 7720 7468 6520 6275 696c  To view the buil
-00001c20: 7469 6e20 6d6f 6465 6c73 2c20 7275 6e20  tin models, run 
-00001c30: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00001c40: 6d6d 616e 643a 0a60 6060 6261 7368 0a24  mmand:.```bash.$
-00001c50: 2078 696e 6665 7265 6e63 6520 6c69 7374   xinference list
-00001c60: 202d 2d61 6c6c 0a60 6060 0a0a 7c20 4e61   --all.```..| Na
-00001c70: 6d65 2020 2020 2020 2020 2020 2020 2020  me              
-00001c80: 2020 207c 2054 7970 6520 2020 2020 2020     | Type       
-00001c90: 2020 2020 2020 7c20 4c61 6e67 7561 6765        | Language
-00001ca0: 207c 2046 6f72 6d61 7420 7c20 5369 7a65   | Format | Size
-00001cb0: 2028 696e 2062 696c 6c69 6f6e 7329 207c   (in billions) |
-00001cc0: 2051 7561 6e74 697a 6174 696f 6e20 2020   Quantization   
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ce0: 2020 2020 2020 2020 7c0a 7c20 2d2d 2d2d          |.| ----
-00001cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001d00: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
-00001d10: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d7c  ----|----------|
-00001d20: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-00001d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
-00001d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001d60: 2d2d 2d2d 2d2d 7c0a 7c20 6261 6963 6875  ------|.| baichu
-00001d70: 616e 2020 2020 2020 2020 2020 2020 207c  an             |
-00001d80: 2046 6f75 6e64 6174 696f 6e20 4d6f 6465   Foundation Mode
-00001d90: 6c20 7c20 656e 2c20 7a68 2020 207c 2067  l | en, zh   | g
-00001da0: 676d 6c76 3320 7c20 3720 2020 2020 2020  gmlv3 | 7       
-00001db0: 2020 2020 2020 2020 2020 207c 2027 7132             | 'q2
-00001dc0: 5f4b 272c 2027 7133 5f4b 5f4c 272c 202e  _K', 'q3_K_L', .
-00001dd0: 2e2e 202c 2027 7136 5f4b 272c 2027 7138  .. , 'q6_K', 'q8
-00001de0: 5f30 2720 7c0a 7c20 6368 6174 676c 6d20  _0' |.| chatglm 
-00001df0: 2020 2020 2020 2020 2020 2020 207c 2053               | S
-00001e00: 4654 204d 6f64 656c 2020 2020 2020 2020  FT Model        
-00001e10: 7c20 656e 2c20 7a68 2020 207c 2067 676d  | en, zh   | ggm
-00001e20: 6c76 3320 7c20 3620 2020 2020 2020 2020  lv3 | 6         
-00001e30: 2020 2020 2020 2020 207c 2027 7134 5f30           | 'q4_0
-00001e40: 272c 2027 7134 5f31 272c 2027 7135 5f30  ', 'q4_1', 'q5_0
-00001e50: 272c 2027 7135 5f31 272c 2027 7138 5f30  ', 'q5_1', 'q8_0
-00001e60: 2720 7c0a 7c20 6368 6174 676c 6d32 2020  ' |.| chatglm2  
-00001e70: 2020 2020 2020 2020 2020 207c 2053 4654             | SFT
-00001e80: 204d 6f64 656c 2020 2020 2020 2020 7c20   Model        | 
-00001e90: 656e 2c20 7a68 2020 207c 2067 676d 6c76  en, zh   | ggmlv
-00001ea0: 3320 7c20 3620 2020 2020 2020 2020 2020  3 | 6           
-00001eb0: 2020 2020 2020 207c 2027 7134 5f30 272c         | 'q4_0',
-00001ec0: 2027 7134 5f31 272c 2027 7135 5f30 272c   'q4_1', 'q5_0',
-00001ed0: 2027 7135 5f31 272c 2027 7138 5f30 2720   'q5_1', 'q8_0' 
-00001ee0: 7c0a 7c20 7769 7a61 7264 6c6d 2d76 312e  |.| wizardlm-v1.
-00001ef0: 3020 2020 2020 2020 207c 2053 4654 204d  0        | SFT M
-00001f00: 6f64 656c 2020 2020 2020 2020 7c20 656e  odel        | en
-00001f10: 2020 2020 2020 207c 2067 676d 6c76 3320         | ggmlv3 
-00001f20: 7c20 372c 2031 332c 2033 3320 2020 2020  | 7, 13, 33     
-00001f30: 2020 2020 207c 2027 7132 5f4b 272c 2027       | 'q2_K', '
-00001f40: 7133 5f4b 5f4c 272c 202e 2e2e 202c 2027  q3_K_L', ... , '
-00001f50: 7136 5f4b 272c 2027 7138 5f30 2720 7c0a  q6_K', 'q8_0' |.
-00001f60: 7c20 7669 6375 6e61 2d76 312e 3320 2020  | vicuna-v1.3   
-00001f70: 2020 2020 2020 207c 2053 4654 204d 6f64         | SFT Mod
-00001f80: 656c 2020 2020 2020 2020 7c20 656e 2020  el        | en  
-00001f90: 2020 2020 207c 2067 676d 6c76 3320 7c20       | ggmlv3 | 
-00001fa0: 372c 2031 3320 2020 2020 2020 2020 2020  7, 13           
-00001fb0: 2020 207c 2027 7132 5f4b 272c 2027 7133     | 'q2_K', 'q3
-00001fc0: 5f4b 5f4c 272c 202e 2e2e 202c 2027 7136  _K_L', ... , 'q6
-00001fd0: 5f4b 272c 2027 7138 5f30 2720 7c0a 7c20  _K', 'q8_0' |.| 
-00001fe0: 6f72 6361 2020 2020 2020 2020 2020 2020  orca            
-00001ff0: 2020 2020 207c 2053 4654 204d 6f64 656c       | SFT Model
-00002000: 2020 2020 2020 2020 7c20 656e 2020 2020          | en    
-00002010: 2020 207c 2067 676d 6c76 3320 7c20 332c     | ggmlv3 | 3,
-00002020: 2037 2c20 3133 2020 2020 2020 2020 2020   7, 13          
-00002030: 207c 2027 7134 5f30 272c 2027 7134 5f31   | 'q4_0', 'q4_1
-00002040: 272c 2027 7135 5f30 272c 2027 7135 5f31  ', 'q5_0', 'q5_1
-00002050: 272c 2027 7138 5f30 2720 7c0a 0a0a 2a2a  ', 'q8_0' |...**
-00002060: 4e4f 5445 2a2a 3a0a 2d20 5869 6e66 6572  NOTE**:.- Xinfer
-00002070: 656e 6365 2077 696c 6c20 646f 776e 6c6f  ence will downlo
-00002080: 6164 206d 6f64 656c 7320 6175 746f 6d61  ad models automa
-00002090: 7469 6361 6c6c 7920 666f 7220 796f 752c  tically for you,
-000020a0: 2061 6e64 2062 7920 6465 6661 756c 7420   and by default 
-000020b0: 7468 6520 6d6f 6465 6c73 2077 696c 6c20  the models will 
-000020c0: 6265 2073 6176 6564 2075 6e64 6572 2060  be saved under `
-000020d0: 247b 5553 4552 7d2f 2e78 696e 6665 7265  ${USER}/.xinfere
-000020e0: 6e63 652f 6361 6368 6560 2e0a 2d20 466f  nce/cache`..- Fo
-000020f0: 756e 6461 7469 6f6e 206d 6f64 656c 7320  undation models 
-00002100: 6f6e 6c79 2070 726f 7669 6465 2069 6e74  only provide int
-00002110: 6572 6661 6365 2060 6765 6e65 7261 7465  erface `generate
-00002120: 602e 0a2d 2053 4654 206d 6f64 656c 7320  `..- SFT models 
-00002130: 7072 6f76 6964 6520 626f 7468 2060 6765  provide both `ge
-00002140: 6e65 7261 7465 6020 616e 6420 6063 6861  nerate` and `cha
-00002150: 7460 2e0a 0a23 2320 526f 6164 6d61 700a  t`...## Roadmap.
-00002160: 5869 6e66 6572 656e 6365 2069 7320 6375  Xinference is cu
-00002170: 7272 656e 746c 7920 756e 6465 7220 6163  rrently under ac
-00002180: 7469 7665 2064 6576 656c 6f70 6d65 6e74  tive development
-00002190: 2e20 4865 7265 2773 2061 2072 6f61 646d  . Here's a roadm
-000021a0: 6170 206f 7574 6c69 6e69 6e67 206f 7572  ap outlining our
-000021b0: 2070 6c61 6e6e 6564 200a 6465 7665 6c6f   planned .develo
-000021c0: 706d 656e 7473 2066 6f72 2074 6865 206e  pments for the n
-000021d0: 6578 7420 6665 7720 7765 656b 733a 0a0a  ext few weeks:..
-000021e0: 2323 2320 5079 546f 7263 6820 5375 7070  ### PyTorch Supp
-000021f0: 6f72 740a 5769 7468 2050 7954 6f72 6368  ort.With PyTorch
-00002200: 2069 6e74 6567 7261 7469 6f6e 2c20 7573   integration, us
-00002210: 6572 7320 7769 6c6c 2062 6520 6162 6c65  ers will be able
-00002220: 2074 6f20 7365 616d 6c65 7373 6c79 2075   to seamlessly u
-00002230: 7469 6c69 7a65 2050 7954 6f72 6368 206d  tilize PyTorch m
-00002240: 6f64 656c 7320 6672 6f6d 2048 7567 6769  odels from Huggi
-00002250: 6e67 2046 6163 650a 7769 7468 696e 2058  ng Face.within X
-00002260: 696e 6665 7265 6e63 652e 0a0a 2323 2320  inference...### 
-00002270: 4c61 6e67 6368 6169 6e20 2620 4c6c 616d  Langchain & Llam
-00002280: 6149 6e64 6578 2069 6e74 6567 7261 7469  aIndex integrati
-00002290: 6f6e 0a57 6974 6820 5869 6e66 6572 656e  on.With Xinferen
-000022a0: 6365 2c20 6974 2077 696c 6c20 6265 206d  ce, it will be m
-000022b0: 7563 6820 6561 7369 6572 2066 6f72 2075  uch easier for u
-000022c0: 7365 7273 2074 6f20 7573 6520 7468 6573  sers to use thes
-000022d0: 6520 6c69 6272 6172 6965 7320 616e 6420  e libraries and 
-000022e0: 6275 696c 6420 6170 706c 6963 6174 696f  build applicatio
-000022f0: 6e73 200a 7769 7468 204c 4c4d 732e 0a    ns .with LLMs..
+000006a0: 732f 6465 6d6f 2e67 6966 290a 0a3c 6469  s/demo.gif)..<di
+000006b0: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+000006c0: 3e0a 3c69 3e3c 6120 6872 6566 3d22 6874  >.<i><a href="ht
+000006d0: 7470 733a 2f2f 6a6f 696e 2e73 6c61 636b  tps://join.slack
+000006e0: 2e63 6f6d 2f74 2f78 6f72 6269 7473 696f  .com/t/xorbitsio
+000006f0: 2f73 6861 7265 645f 696e 7669 7465 2f7a  /shared_invite/z
+00000700: 742d 317a 337a 736d 3965 702d 3837 7949  t-1z3zsm9ep-87yI
+00000710: 3959 5a5f 4237 3948 4c42 3263 6354 7134  9YZ_B79HLB2ccTq4
+00000720: 5741 223e f09f 9189 204a 6f69 6e20 6f75  WA">.... Join ou
+00000730: 7220 536c 6163 6b20 636f 6d6d 756e 6974  r Slack communit
+00000740: 7921 3c2f 613e 3c2f 693e 0a3c 2f64 6976  y!</a></i>.</div
+00000750: 3e0a 0a23 2320 4b65 7920 4665 6174 7572  >..## Key Featur
+00000760: 6573 0af0 9f8c 9f20 2a2a 4d6f 6465 6c20  es..... **Model 
+00000770: 5365 7276 696e 6720 4d61 6465 2045 6173  Serving Made Eas
+00000780: 792a 2a3a 2049 6e66 6572 656e 6365 2073  y**: Inference s
+00000790: 696d 706c 6966 6965 7320 7468 6520 7072  implifies the pr
+000007a0: 6f63 6573 7320 6f66 2073 6572 7669 6e67  ocess of serving
+000007b0: 206c 6172 6765 206c 616e 6775 6167 652c   large language,
+000007c0: 2073 7065 6563 6820 0a72 6563 6f67 6e69   speech .recogni
+000007d0: 7469 6f6e 2c20 616e 6420 6d75 6c74 696d  tion, and multim
+000007e0: 6f64 616c 206d 6f64 656c 732e 2059 6f75  odal models. You
+000007f0: 2063 616e 2073 6574 2075 7020 616e 6420   can set up and 
+00000800: 6465 706c 6f79 2079 6f75 7220 6d6f 6465  deploy your mode
+00000810: 6c73 0a66 6f72 2065 7870 6572 696d 656e  ls.for experimen
+00000820: 7461 7469 6f6e 2061 6e64 2070 726f 6475  tation and produ
+00000830: 6374 696f 6e20 7769 7468 2061 2073 696e  ction with a sin
+00000840: 676c 6520 636f 6d6d 616e 642e 0a0a e29a  gle command.....
+00000850: a1ef b88f 202a 2a53 7461 7465 2d6f 662d  .... **State-of-
+00000860: 7468 652d 4172 7420 4d6f 6465 6c73 2a2a  the-Art Models**
+00000870: 3a20 4578 7065 7269 6d65 6e74 2077 6974  : Experiment wit
+00000880: 6820 6375 7474 696e 672d 6564 6765 2062  h cutting-edge b
+00000890: 7569 6c74 2d69 6e20 6d6f 6465 6c73 2075  uilt-in models u
+000008a0: 7369 6e67 2061 2073 696e 676c 6520 0a63  sing a single .c
+000008b0: 6f6d 6d61 6e64 2e20 496e 6665 7265 6e63  ommand. Inferenc
+000008c0: 6520 7072 6f76 6964 6573 2061 6363 6573  e provides acces
+000008d0: 7320 746f 2073 7461 7465 2d6f 662d 7468  s to state-of-th
+000008e0: 652d 6172 7420 6f70 656e 2d73 6f75 7263  e-art open-sourc
+000008f0: 6520 6d6f 6465 6c73 210a 0af0 9f96 a520  e models!...... 
+00000900: 2a2a 4865 7465 726f 6765 6e65 6f75 7320  **Heterogeneous 
+00000910: 4861 7264 7761 7265 2055 7469 6c69 7a61  Hardware Utiliza
+00000920: 7469 6f6e 2a2a 3a20 4d61 6b65 2074 6865  tion**: Make the
+00000930: 206d 6f73 7420 6f66 2079 6f75 7220 6861   most of your ha
+00000940: 7264 7761 7265 2072 6573 6f75 7263 6573  rdware resources
+00000950: 2e20 586f 7262 6974 7320 0a49 6e66 6572  . Xorbits .Infer
+00000960: 656e 6365 2069 6e74 656c 6c69 6765 6e74  ence intelligent
+00000970: 6c79 2075 7469 6c69 7a65 7320 6865 7465  ly utilizes hete
+00000980: 726f 6765 6e65 6f75 7320 6861 7264 7761  rogeneous hardwa
+00000990: 7265 2c20 696e 636c 7564 696e 6720 4750  re, including GP
+000009a0: 5573 2061 6e64 2043 5055 732c 2074 6f20  Us and CPUs, to 
+000009b0: 6d61 7869 6d69 7a65 0a70 6572 666f 726d  maximize.perform
+000009c0: 616e 6365 2061 6e64 2061 6363 656c 6572  ance and acceler
+000009d0: 6174 6520 796f 7572 206d 6f64 656c 2069  ate your model i
+000009e0: 6e66 6572 656e 6365 2074 6173 6b73 2e0a  nference tasks..
+000009f0: 0ae2 9a99 efb8 8f20 2a2a 466c 6578 6962  ....... **Flexib
+00000a00: 6c65 2041 5049 2061 6e64 2049 6e74 6572  le API and Inter
+00000a10: 6661 6365 732a 2a3a 2058 6f72 6269 7473  faces**: Xorbits
+00000a20: 2049 6e66 6572 656e 6365 206f 6666 6572   Inference offer
+00000a30: 7320 6d75 6c74 6970 6c65 2069 6e74 6572  s multiple inter
+00000a40: 6661 6365 7320 666f 7220 696e 7465 7261  faces for intera
+00000a50: 6374 696e 670a 7769 7468 2079 6f75 7220  cting.with your 
+00000a60: 6d6f 6465 6c73 2e20 596f 7520 6361 6e20  models. You can 
+00000a70: 7574 696c 697a 6520 7468 6520 5250 4320  utilize the RPC 
+00000a80: 616e 6420 5245 5354 6675 6c20 4150 4928  and RESTful API(
+00000a90: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
+00000aa0: 4f70 656e 4149 2041 5049 2920 746f 2069  OpenAI API) to i
+00000ab0: 6e74 6567 7261 7465 0a79 6f75 7220 6d6f  ntegrate.your mo
+00000ac0: 6465 6c73 2077 6974 6820 6578 6973 7469  dels with existi
+00000ad0: 6e67 2073 7973 7465 6d73 206f 7220 7573  ng systems or us
+00000ae0: 6520 7468 6520 636f 6d6d 616e 642d 6c69  e the command-li
+00000af0: 6e65 2069 6e74 6572 6661 6365 2028 434c  ne interface (CL
+00000b00: 4929 2061 6e64 2074 6865 2069 6e74 7569  I) and the intui
+00000b10: 7469 7665 2057 6562 5549 0a66 6f72 2073  tive WebUI.for s
+00000b20: 6561 6d6c 6573 7320 6d61 6e61 6765 6d65  eamless manageme
+00000b30: 6e74 2061 6e64 206d 6f6e 6974 6f72 696e  nt and monitorin
+00000b40: 672e 0a0a f09f 8c90 202a 2a44 6973 7472  g....... **Distr
+00000b50: 6962 7574 6564 2044 6570 6c6f 796d 656e  ibuted Deploymen
+00000b60: 742a 2a3a 2058 6f72 6269 7473 2049 6e66  t**: Xorbits Inf
+00000b70: 6572 656e 6365 2065 7863 656c 7320 696e  erence excels in
+00000b80: 2064 6973 7472 6962 7574 6564 2064 6570   distributed dep
+00000b90: 6c6f 796d 656e 7420 7363 656e 6172 696f  loyment scenario
+00000ba0: 732c 200a 616c 6c6f 7769 6e67 2074 6865  s, .allowing the
+00000bb0: 2073 6561 6d6c 6573 7320 6469 7374 7269   seamless distri
+00000bc0: 6275 7469 6f6e 206f 6620 6d6f 6465 6c20  bution of model 
+00000bd0: 696e 6665 7265 6e63 6520 6163 726f 7373  inference across
+00000be0: 206d 756c 7469 706c 6520 6465 7669 6365   multiple device
+00000bf0: 7320 6f72 206d 6163 6869 6e65 732e 2049  s or machines. I
+00000c00: 740a 6c65 7665 7261 6765 7320 6469 7374  t.leverages dist
+00000c10: 7269 6275 7465 6420 636f 6d70 7574 696e  ributed computin
+00000c20: 6720 7465 6368 6e69 7175 6573 2074 6f20  g techniques to 
+00000c30: 7061 7261 6c6c 656c 697a 6520 616e 6420  parallelize and 
+00000c40: 7363 616c 6520 7468 6520 696e 6665 7265  scale the infere
+00000c50: 6e63 6520 7072 6f63 6573 732e 0a0a f09f  nce process.....
+00000c60: 948c 202a 2a42 7569 6c74 2d69 6e20 496e  .. **Built-in In
+00000c70: 7465 6772 6174 696f 6e20 7769 7468 2054  tegration with T
+00000c80: 6869 7264 2d50 6172 7479 204c 6962 7261  hird-Party Libra
+00000c90: 7269 6573 2a2a 3a20 586f 7262 6974 7320  ries**: Xorbits 
+00000ca0: 496e 6665 7265 6e63 6520 7365 616d 6c65  Inference seamle
+00000cb0: 7373 6c79 2069 6e74 6567 7261 7465 730a  ssly integrates.
+00000cc0: 7769 7468 2070 6f70 756c 6172 2074 6869  with popular thi
+00000cd0: 7264 2d70 6172 7479 206c 6962 7261 7269  rd-party librari
+00000ce0: 6573 206c 696b 6520 4c61 6e67 4368 6169  es like LangChai
+00000cf0: 6e20 616e 6420 4c6c 616d 6149 6e64 6578  n and LlamaIndex
+00000d00: 2e20 2843 6f6d 696e 6720 736f 6f6e 290a  . (Coming soon).
+00000d10: 0a23 2320 4765 7474 696e 6720 5374 6172  .## Getting Star
+00000d20: 7465 640a 5869 6e66 6572 656e 6365 2063  ted.Xinference c
+00000d30: 616e 2062 6520 696e 7374 616c 6c65 6420  an be installed 
+00000d40: 7669 6120 7069 7020 6672 6f6d 2050 7950  via pip from PyP
+00000d50: 492e 2049 7420 6973 2068 6967 686c 7920  I. It is highly 
+00000d60: 7265 636f 6d6d 656e 6465 6420 746f 2063  recommended to c
+00000d70: 7265 6174 6520 6120 6e65 7720 7669 7274  reate a new virt
+00000d80: 7561 6c0a 656e 7669 726f 6e6d 656e 7420  ual.environment 
+00000d90: 746f 2061 766f 6964 2063 6f6e 666c 6963  to avoid conflic
+00000da0: 7473 2e0a 6060 6062 6173 680a 2420 7069  ts..```bash.$ pi
+00000db0: 7020 696e 7374 616c 6c20 2278 696e 6665  p install "xinfe
+00000dc0: 7265 6e63 655b 616c 6c5d 220a 6060 600a  rence[all]".```.
+00000dd0: 2278 696e 6665 7265 6e63 655b 616c 6c5d  "xinference[all]
+00000de0: 2220 696e 7374 616c 6c73 2061 6c6c 2074  " installs all t
+00000df0: 6865 206e 6563 6573 7361 7279 2070 6163  he necessary pac
+00000e00: 6b61 6765 7320 666f 7220 7365 7276 696e  kages for servin
+00000e10: 6720 6d6f 6465 6c73 2e20 4966 2079 6f75  g models. If you
+00000e20: 2077 616e 7420 746f 2061 6368 6965 7665   want to achieve
+00000e30: 2061 6363 656c 6572 6174 696f 6e20 6f6e   acceleration on
+00000e40: 200a 6469 6666 6572 656e 7420 6861 7264   .different hard
+00000e50: 7761 7265 2c20 7265 6665 7220 746f 2074  ware, refer to t
+00000e60: 6865 2069 6e73 7461 6c6c 6174 696f 6e20  he installation 
+00000e70: 646f 6375 6d65 6e74 6174 696f 6e20 6f66  documentation of
+00000e80: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
+00000e90: 6e67 2070 6163 6b61 6765 2e0a 2d20 5b6c  ng package..- [l
+00000ea0: 6c61 6d61 2d63 7070 2d70 7974 686f 6e5d  lama-cpp-python]
+00000eb0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000ec0: 636f 6d2f 6162 6574 6c65 6e2f 6c6c 616d  com/abetlen/llam
+00000ed0: 612d 6370 702d 7079 7468 6f6e 2369 6e73  a-cpp-python#ins
+00000ee0: 7461 6c6c 6174 696f 6e2d 6672 6f6d 2d70  tallation-from-p
+00000ef0: 7970 692d 7265 636f 6d6d 656e 6465 6429  ypi-recommended)
+00000f00: 2069 7320 7265 7175 6972 6564 2074 6f20   is required to 
+00000f10: 7275 6e20 6062 6169 6368 7561 6e60 2c20  run `baichuan`, 
+00000f20: 6077 697a 6172 646c 6d2d 7631 2e30 602c  `wizardlm-v1.0`,
+00000f30: 2060 7669 6375 6e61 2d76 312e 3360 2061   `vicuna-v1.3` a
+00000f40: 6e64 2060 6f72 6361 602e 0a2d 205b 6368  nd `orca`..- [ch
+00000f50: 6174 676c 6d2d 6370 702d 7079 7468 6f6e  atglm-cpp-python
+00000f60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000f70: 2e63 6f6d 2f6c 692d 706c 7573 2f63 6861  .com/li-plus/cha
+00000f80: 7467 6c6d 2e63 7070 2367 6574 7469 6e67  tglm.cpp#getting
+00000f90: 2d73 7461 7274 6564 2920 6973 2072 6571  -started) is req
+00000fa0: 7569 7265 6420 746f 2072 756e 2060 6368  uired to run `ch
+00000fb0: 6174 676c 6d60 2061 6e64 2060 6368 6174  atglm` and `chat
+00000fc0: 676c 6d32 602e 0a0a 0a23 2323 2044 6570  glm2`....### Dep
+00000fd0: 6c6f 796d 656e 740a 596f 7520 6361 6e20  loyment.You can 
+00000fe0: 6465 706c 6f79 2058 696e 6665 7265 6e63  deploy Xinferenc
+00000ff0: 6520 6c6f 6361 6c6c 7920 7769 7468 2061  e locally with a
+00001000: 2073 696e 676c 6520 636f 6d6d 616e 6420   single command 
+00001010: 6f72 2064 6570 6c6f 7920 6974 2069 6e20  or deploy it in 
+00001020: 6120 6469 7374 7269 6275 7465 6420 636c  a distributed cl
+00001030: 7573 7465 722e 200a 0a23 2323 2320 4c6f  uster. ..#### Lo
+00001040: 6361 6c0a 546f 2073 7461 7274 2061 206c  cal.To start a l
+00001050: 6f63 616c 2069 6e73 7461 6e63 6520 6f66  ocal instance of
+00001060: 2058 696e 6665 7265 6e63 652c 2072 756e   Xinference, run
+00001070: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00001080: 6f6d 6d61 6e64 3a0a 6060 6062 6173 680a  ommand:.```bash.
+00001090: 2420 7869 6e66 6572 656e 6365 0a60 6060  $ xinference.```
+000010a0: 0a0a 2323 2323 2044 6973 7472 6962 7574  ..#### Distribut
+000010b0: 6564 0a0a 546f 2064 6570 6c6f 7920 5869  ed..To deploy Xi
+000010c0: 6e66 6572 656e 6365 2069 6e20 6120 636c  nference in a cl
+000010d0: 7573 7465 722c 2079 6f75 206e 6565 6420  uster, you need 
+000010e0: 746f 2073 7461 7274 2061 2058 696e 6665  to start a Xinfe
+000010f0: 7265 6e63 6520 7375 7065 7276 6973 6f72  rence supervisor
+00001100: 206f 6e20 6f6e 6520 7365 7276 6572 2061   on one server a
+00001110: 6e64 200a 5869 6e66 6572 656e 6365 2077  nd .Xinference w
+00001120: 6f72 6b65 7273 206f 6e20 7468 6520 6f74  orkers on the ot
+00001130: 6865 7220 7365 7276 6572 732e 2046 6f6c  her servers. Fol
+00001140: 6c6f 7720 7468 6520 7374 6570 7320 6265  low the steps be
+00001150: 6c6f 773a 0a0a 2a2a 5374 6172 7469 6e67  low:..**Starting
+00001160: 2074 6865 2053 7570 6572 7669 736f 722a   the Supervisor*
+00001170: 2a3a 204f 6e20 7468 6520 7365 7276 6572  *: On the server
+00001180: 2077 6865 7265 2079 6f75 2077 616e 7420   where you want 
+00001190: 746f 2072 756e 2074 6865 2058 696e 6665  to run the Xinfe
+000011a0: 7265 6e63 6520 7375 7065 7276 6973 6f72  rence supervisor
+000011b0: 2c20 7275 6e20 7468 6520 666f 6c6c 6f77  , run the follow
+000011c0: 696e 6720 636f 6d6d 616e 643a 0a60 6060  ing command:.```
+000011d0: 6261 7368 0a24 2078 696e 6665 7265 6e63  bash.$ xinferenc
+000011e0: 652d 7375 7065 7276 6973 6f72 202d 4820  e-supervisor -H 
+000011f0: 2224 7b73 7570 6572 7669 736f 725f 686f  "${supervisor_ho
+00001200: 7374 7d22 0a60 6060 0a52 6570 6c61 6365  st}".```.Replace
+00001210: 2060 247b 7375 7065 7276 6973 6f72 5f68   `${supervisor_h
+00001220: 6f73 747d 6020 7769 7468 2074 6865 2061  ost}` with the a
+00001230: 6374 7561 6c20 686f 7374 206f 6620 796f  ctual host of yo
+00001240: 7572 2073 7570 6572 7669 736f 7220 7365  ur supervisor se
+00001250: 7276 6572 2e0a 0a2a 2a53 7461 7274 696e  rver...**Startin
+00001260: 6720 7468 6520 576f 726b 6572 732a 2a3a  g the Workers**:
+00001270: 204f 6e20 6561 6368 206f 6620 7468 6520   On each of the 
+00001280: 6f74 6865 7220 7365 7276 6572 7320 7768  other servers wh
+00001290: 6572 6520 796f 7520 7761 6e74 2074 6f20  ere you want to 
+000012a0: 7275 6e20 5869 6e66 6572 656e 6365 2077  run Xinference w
+000012b0: 6f72 6b65 7273 2c20 7275 6e20 7468 6520  orkers, run the 
+000012c0: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+000012d0: 643a 0a60 6060 6261 7368 0a24 2078 696e  d:.```bash.$ xin
+000012e0: 6665 7265 6e63 652d 776f 726b 6572 202d  ference-worker -
+000012f0: 6520 2268 7474 703a 2f2f 247b 7375 7065  e "http://${supe
+00001300: 7276 6973 6f72 5f68 6f73 747d 3a39 3939  rvisor_host}:999
+00001310: 3722 0a60 6060 0a0a 4f6e 6365 2058 696e  7".```..Once Xin
+00001320: 6665 7265 6e63 6520 6973 2072 756e 6e69  ference is runni
+00001330: 6e67 2c20 616e 2065 6e64 706f 696e 7420  ng, an endpoint 
+00001340: 7769 6c6c 2062 6520 6163 6365 7373 6962  will be accessib
+00001350: 6c65 2066 6f72 206d 6f64 656c 206d 616e  le for model man
+00001360: 6167 656d 656e 7420 7669 6120 434c 4920  agement via CLI 
+00001370: 6f72 0a58 696e 6665 7265 6e63 6520 2063  or.Xinference  c
+00001380: 6c69 656e 742e 0a0a 2d20 466f 7220 6c6f  lient...- For lo
+00001390: 6361 6c20 6465 706c 6f79 6d65 6e74 2c20  cal deployment, 
+000013a0: 7468 6520 656e 6470 6f69 6e74 2077 696c  the endpoint wil
+000013b0: 6c20 6265 2060 6874 7470 3a2f 2f6c 6f63  l be `http://loc
+000013c0: 616c 686f 7374 3a39 3939 3760 2e0a 2d20  alhost:9997`..- 
+000013d0: 466f 7220 636c 7573 7465 7220 6465 706c  For cluster depl
+000013e0: 6f79 6d65 6e74 2c20 7468 6520 656e 6470  oyment, the endp
+000013f0: 6f69 6e74 2077 696c 6c20 6265 2060 6874  oint will be `ht
+00001400: 7470 3a2f 2f24 7b73 7570 6572 7669 736f  tp://${superviso
+00001410: 725f 686f 7374 7d3a 3939 3937 602c 2077  r_host}:9997`, w
+00001420: 6865 7265 0a60 247b 7375 7065 7276 6973  here.`${supervis
+00001430: 6f72 5f68 6f73 747d 6020 6973 2074 6865  or_host}` is the
+00001440: 2068 6f73 746e 616d 6520 6f72 2049 5020   hostname or IP 
+00001450: 6164 6472 6573 7320 6f66 2074 6865 2073  address of the s
+00001460: 6572 7665 7220 7768 6572 6520 7468 6520  erver where the 
+00001470: 7375 7065 7276 6973 6f72 2069 7320 7275  supervisor is ru
+00001480: 6e6e 696e 672e 0a0a 596f 7520 6361 6e20  nning...You can 
+00001490: 616c 736f 2076 6965 7720 6120 7765 6220  also view a web 
+000014a0: 5549 2075 7369 6e67 2074 6865 2058 696e  UI using the Xin
+000014b0: 6665 7265 6e63 6520 656e 6470 6f69 6e74  ference endpoint
+000014c0: 2074 6f20 6368 6174 2077 6974 6820 616c   to chat with al
+000014d0: 6c20 7468 6520 0a62 7569 6c74 696e 206d  l the .builtin m
+000014e0: 6f64 656c 732e 2059 6f75 2063 616e 2065  odels. You can e
+000014f0: 7665 6e20 2a2a 6368 6174 2077 6974 6820  ven **chat with 
+00001500: 7477 6f20 6375 7474 696e 672d 6564 6765  two cutting-edge
+00001510: 2041 4920 6d6f 6465 6c73 2073 6964 652d   AI models side-
+00001520: 6279 2d73 6964 6520 746f 2063 6f6d 7061  by-side to compa
+00001530: 7265 0a74 6865 6972 2070 6572 666f 726d  re.their perform
+00001540: 616e 6365 2a2a 210a 0a21 5b77 6562 2055  ance**!..![web U
+00001550: 495d 2861 7373 6574 732f 7869 6e66 6572  I](assets/xinfer
+00001560: 656e 6365 2d64 6f77 6e6c 6f61 6469 6e67  ence-downloading
+00001570: 2e70 6e67 290a 0a23 2323 2058 696e 6665  .png)..### Xinfe
+00001580: 7265 6e63 6520 434c 490a 5869 6e66 6572  rence CLI.Xinfer
+00001590: 656e 6365 2070 726f 7669 6465 7320 6120  ence provides a 
+000015a0: 636f 6d6d 616e 6420 6c69 6e65 2069 6e74  command line int
+000015b0: 6572 6661 6365 2028 434c 4929 2066 6f72  erface (CLI) for
+000015c0: 206d 6f64 656c 206d 616e 6167 656d 656e   model managemen
+000015d0: 742e 2048 6572 6520 6172 6520 736f 6d65  t. Here are some
+000015e0: 2075 7365 6675 6c20 0a63 6f6d 6d61 6e64   useful .command
+000015f0: 733a 0a0a 2d20 4c61 756e 6368 2061 206d  s:..- Launch a m
+00001600: 6f64 656c 2028 6120 6d6f 6465 6c20 5549  odel (a model UI
+00001610: 4420 7769 6c6c 2062 6520 7265 7475 726e  D will be return
+00001620: 6564 293a 2060 7869 6e66 6572 656e 6365  ed): `xinference
+00001630: 206c 6175 6e63 6860 0a2d 204c 6973 7420   launch`.- List 
+00001640: 7275 6e6e 696e 6720 6d6f 6465 6c73 3a20  running models: 
+00001650: 6078 696e 6665 7265 6e63 6520 6c69 7374  `xinference list
+00001660: 600a 2d20 4c69 7374 2061 6c6c 2074 6865  `.- List all the
+00001670: 2062 7569 6c74 696e 206d 6f64 656c 733a   builtin models:
+00001680: 2060 7869 6e66 6572 656e 6365 206c 6973   `xinference lis
+00001690: 7420 2d2d 616c 6c60 0a2d 2054 6572 6d69  t --all`.- Termi
+000016a0: 6e61 7465 2061 206d 6f64 656c 3a20 6078  nate a model: `x
+000016b0: 696e 6665 7265 6e63 6520 7465 726d 696e  inference termin
+000016c0: 6174 6520 2d2d 6d6f 6465 6c2d 7569 6420  ate --model-uid 
+000016d0: 247b 6d6f 6465 6c5f 7569 647d 600a 0a23  ${model_uid}`..#
+000016e0: 2323 2058 696e 6665 7265 6e63 6520 436c  ## Xinference Cl
+000016f0: 6965 6e74 0a58 696e 6665 7265 6e63 6520  ient.Xinference 
+00001700: 616c 736f 2070 726f 7669 6465 7320 6120  also provides a 
+00001710: 636c 6965 6e74 2066 6f72 206d 616e 6167  client for manag
+00001720: 696e 6720 616e 6420 6163 6365 7373 696e  ing and accessin
+00001730: 6720 6d6f 6465 6c73 2070 726f 6772 616d  g models program
+00001740: 6d61 7469 6361 6c6c 793a 0a0a 6060 6070  matically:..```p
+00001750: 7974 686f 6e0a 6672 6f6d 2078 696e 6665  ython.from xinfe
+00001760: 7265 6e63 652e 636c 6965 6e74 2069 6d70  rence.client imp
+00001770: 6f72 7420 436c 6965 6e74 0a0a 636c 6965  ort Client..clie
+00001780: 6e74 203d 2043 6c69 656e 7428 2268 7474  nt = Client("htt
+00001790: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3939  p://localhost:99
+000017a0: 3937 2229 0a6d 6f64 656c 5f75 6964 203d  97").model_uid =
+000017b0: 2063 6c69 656e 742e 6c61 756e 6368 5f6d   client.launch_m
+000017c0: 6f64 656c 286d 6f64 656c 5f6e 616d 653d  odel(model_name=
+000017d0: 2263 6861 7467 6c6d 3222 290a 6d6f 6465  "chatglm2").mode
+000017e0: 6c20 3d20 636c 6965 6e74 2e67 6574 5f6d  l = client.get_m
+000017f0: 6f64 656c 286d 6f64 656c 5f75 6964 290a  odel(model_uid).
+00001800: 0a63 6861 745f 6869 7374 6f72 7920 3d20  .chat_history = 
+00001810: 5b5d 0a70 726f 6d70 7420 3d20 2257 6861  [].prompt = "Wha
+00001820: 7420 6973 2074 6865 206c 6172 6765 7374  t is the largest
+00001830: 2061 6e69 6d61 6c3f 220a 6d6f 6465 6c2e   animal?".model.
+00001840: 6368 6174 280a 2020 2020 2020 2020 2020  chat(.          
+00001850: 2020 7072 6f6d 7074 2c0a 2020 2020 2020    prompt,.      
+00001860: 2020 2020 2020 6368 6174 5f68 6973 746f        chat_histo
+00001870: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
+00001880: 6765 6e65 7261 7465 5f63 6f6e 6669 673d  generate_config=
+00001890: 7b22 6d61 785f 746f 6b65 6e73 223a 2031  {"max_tokens": 1
+000018a0: 3032 347d 0a20 2020 2020 2020 2029 0a60  024}.        ).`
+000018b0: 6060 0a0a 5265 7375 6c74 3a0a 6060 606a  ``..Result:.```j
+000018c0: 736f 6e0a 7b0a 2020 2269 6422 3a20 2263  son.{.  "id": "c
+000018d0: 6861 7463 6d70 6c2d 3864 3736 6236 3561  hatcmpl-8d76b65a
+000018e0: 2d62 6164 302d 3432 6566 2d39 3132 642d  -bad0-42ef-912d-
+000018f0: 3461 3035 3333 6439 3064 3631 222c 0a20  4a0533d90d61",. 
+00001900: 2022 6d6f 6465 6c22 3a20 2235 3666 3639   "model": "56f69
+00001910: 3632 322d 3165 3733 2d31 3165 652d 6133  622-1e73-11ee-a3
+00001920: 6264 2d39 6166 3966 3136 3831 3663 3622  bd-9af9f16816c6"
+00001930: 2c0a 2020 226f 626a 6563 7422 3a20 2263  ,.  "object": "c
+00001940: 6861 742e 636f 6d70 6c65 7469 6f6e 222c  hat.completion",
+00001950: 0a20 2022 6372 6561 7465 6422 3a20 3136  .  "created": 16
+00001960: 3838 3931 3931 3837 2c0a 2020 2263 686f  88919187,.  "cho
+00001970: 6963 6573 223a 205b 0a20 2020 207b 0a20  ices": [.    {. 
+00001980: 2020 2020 2022 696e 6465 7822 3a20 302c       "index": 0,
+00001990: 0a20 2020 2020 2022 6d65 7373 6167 6522  .      "message"
+000019a0: 3a20 7b0a 2020 2020 2020 2020 2272 6f6c  : {.        "rol
+000019b0: 6522 3a20 2261 7373 6973 7461 6e74 222c  e": "assistant",
+000019c0: 0a20 2020 2020 2020 2022 636f 6e74 656e  .        "conten
+000019d0: 7422 3a20 2254 6865 206c 6172 6765 7374  t": "The largest
+000019e0: 2061 6e69 6d61 6c20 7468 6174 2068 6173   animal that has
+000019f0: 2062 6565 6e20 7363 6965 6e74 6966 6963   been scientific
+00001a00: 616c 6c79 206d 6561 7375 7265 6420 6973  ally measured is
+00001a10: 2074 6865 2062 6c75 6520 7768 616c 652c   the blue whale,
+00001a20: 2077 6869 6368 2068 6173 2061 206d 6178   which has a max
+00001a30: 696d 756d 206c 656e 6774 6820 6f66 2061  imum length of a
+00001a40: 726f 756e 6420 3233 206d 6574 6572 7320  round 23 meters 
+00001a50: 2837 3520 6665 6574 2920 666f 7220 6164  (75 feet) for ad
+00001a60: 756c 7420 616e 696d 616c 7320 616e 6420  ult animals and 
+00001a70: 6361 6e20 7765 6967 6820 7570 2074 6f20  can weigh up to 
+00001a80: 3135 302c 3030 3020 706f 756e 6473 2028  150,000 pounds (
+00001a90: 3638 2c30 3030 206b 6729 2e20 486f 7765  68,000 kg). Howe
+00001aa0: 7665 722c 2069 7420 6973 2069 6d70 6f72  ver, it is impor
+00001ab0: 7461 6e74 2074 6f20 6e6f 7465 2074 6861  tant to note tha
+00001ac0: 7420 7468 6973 2069 7320 6a75 7374 2061  t this is just a
+00001ad0: 6e20 6573 7469 6d61 7465 2061 6e64 2074  n estimate and t
+00001ae0: 6861 7420 7468 6520 6c61 7267 6573 7420  hat the largest 
+00001af0: 616e 696d 616c 206b 6e6f 776e 2074 6f20  animal known to 
+00001b00: 7363 6965 6e63 6520 6d61 7920 6265 206c  science may be l
+00001b10: 6172 6765 7220 7374 696c 6c2e 2053 6f6d  arger still. Som
+00001b20: 6520 7363 6965 6e74 6973 7473 2062 656c  e scientists bel
+00001b30: 6965 7665 2074 6861 7420 7468 6520 6c61  ieve that the la
+00001b40: 7267 6573 7420 616e 696d 616c 7320 6d61  rgest animals ma
+00001b50: 7920 6e6f 7420 6861 7665 2061 2063 6c65  y not have a cle
+00001b60: 6172 205c 2273 697a 655c 2220 696e 2074  ar \"size\" in t
+00001b70: 6865 2073 616d 6520 7761 7920 7468 6174  he same way that
+00001b80: 2068 756d 616e 7320 646f 2c20 6173 2074   humans do, as t
+00001b90: 6865 6972 2073 697a 6520 6361 6e20 7661  heir size can va
+00001ba0: 7279 2064 6570 656e 6469 6e67 206f 6e20  ry depending on 
+00001bb0: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
+00001bc0: 616e 6420 7468 6520 7374 6167 6520 6f66  and the stage of
+00001bd0: 2074 6865 6972 206c 6966 652e 220a 2020   their life.".  
+00001be0: 2020 2020 7d2c 0a20 2020 2020 2022 6669      },.      "fi
+00001bf0: 6e69 7368 5f72 6561 736f 6e22 3a20 224e  nish_reason": "N
+00001c00: 6f6e 6522 0a20 2020 207d 0a20 205d 2c0a  one".    }.  ],.
+00001c10: 2020 2275 7361 6765 223a 207b 0a20 2020    "usage": {.   
+00001c20: 2022 7072 6f6d 7074 5f74 6f6b 656e 7322   "prompt_tokens"
+00001c30: 3a20 2d31 2c0a 2020 2020 2263 6f6d 706c  : -1,.    "compl
+00001c40: 6574 696f 6e5f 746f 6b65 6e73 223a 202d  etion_tokens": -
+00001c50: 312c 0a20 2020 2022 746f 7461 6c5f 746f  1,.    "total_to
+00001c60: 6b65 6e73 223a 202d 310a 2020 7d0a 7d0a  kens": -1.  }.}.
+00001c70: 6060 600a 0a53 6565 205b 6578 616d 706c  ```..See [exampl
+00001c80: 6573 5d28 6578 616d 706c 6573 2920 666f  es](examples) fo
+00001c90: 7220 6d6f 7265 2065 7861 6d70 6c65 732e  r more examples.
+00001ca0: 0a0a 0a23 2320 4275 696c 7469 6e20 6d6f  ...## Builtin mo
+00001cb0: 6465 6c73 0a54 6f20 7669 6577 2074 6865  dels.To view the
+00001cc0: 2062 7569 6c74 696e 206d 6f64 656c 732c   builtin models,
+00001cd0: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
+00001ce0: 6e67 2063 6f6d 6d61 6e64 3a0a 6060 6062  ng command:.```b
+00001cf0: 6173 680a 2420 7869 6e66 6572 656e 6365  ash.$ xinference
+00001d00: 206c 6973 7420 2d2d 616c 6c0a 6060 600a   list --all.```.
+00001d10: 0a7c 204e 616d 6520 2020 2020 2020 2020  .| Name         
+00001d20: 2020 2020 2020 2020 7c20 5479 7065 2020          | Type  
+00001d30: 2020 2020 2020 2020 2020 207c 204c 616e             | Lan
+00001d40: 6775 6167 6520 7c20 466f 726d 6174 207c  guage | Format |
+00001d50: 2053 697a 6520 2869 6e20 6269 6c6c 696f   Size (in billio
+00001d60: 6e73 2920 7c20 5175 616e 7469 7a61 7469  ns) | Quantizati
+00001d70: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+00001d80: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00001d90: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00001da0: 2d2d 2d2d 2d20 7c2d 2d2d 2d2d 2d2d 2d2d  ----- |---------
+00001db0: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
+00001dc0: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d7c 2d2d  ----|--------|--
+00001dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001de0: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
+00001df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2062  -----------|.| b
+00001e10: 6169 6368 7561 6e20 2020 2020 2020 2020  aichuan         
+00001e20: 2020 2020 7c20 466f 756e 6461 7469 6f6e      | Foundation
+00001e30: 204d 6f64 656c 207c 2065 6e2c 207a 6820   Model | en, zh 
+00001e40: 2020 7c20 6767 6d6c 7633 207c 2037 2020    | ggmlv3 | 7  
+00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e60: 7c20 2771 325f 4b27 2c20 2771 335f 4b5f  | 'q2_K', 'q3_K_
+00001e70: 4c27 2c20 2e2e 2e20 2c20 2771 365f 4b27  L', ... , 'q6_K'
+00001e80: 2c20 2771 385f 3027 207c 0a7c 2063 6861  , 'q8_0' |.| cha
+00001e90: 7467 6c6d 2020 2020 2020 2020 2020 2020  tglm            
+00001ea0: 2020 7c20 5346 5420 4d6f 6465 6c20 2020    | SFT Model   
+00001eb0: 2020 2020 207c 2065 6e2c 207a 6820 2020       | en, zh   
+00001ec0: 7c20 6767 6d6c 7633 207c 2036 2020 2020  | ggmlv3 | 6    
+00001ed0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00001ee0: 2771 345f 3027 2c20 2771 345f 3127 2c20  'q4_0', 'q4_1', 
+00001ef0: 2771 355f 3027 2c20 2771 355f 3127 2c20  'q5_0', 'q5_1', 
+00001f00: 2771 385f 3027 207c 0a7c 2063 6861 7467  'q8_0' |.| chatg
+00001f10: 6c6d 3220 2020 2020 2020 2020 2020 2020  lm2             
+00001f20: 7c20 5346 5420 4d6f 6465 6c20 2020 2020  | SFT Model     
+00001f30: 2020 207c 2065 6e2c 207a 6820 2020 7c20     | en, zh   | 
+00001f40: 6767 6d6c 7633 207c 2036 2020 2020 2020  ggmlv3 | 6      
+00001f50: 2020 2020 2020 2020 2020 2020 7c20 2771              | 'q
+00001f60: 345f 3027 2c20 2771 345f 3127 2c20 2771  4_0', 'q4_1', 'q
+00001f70: 355f 3027 2c20 2771 355f 3127 2c20 2771  5_0', 'q5_1', 'q
+00001f80: 385f 3027 207c 0a7c 2077 697a 6172 646c  8_0' |.| wizardl
+00001f90: 6d2d 7631 2e30 2020 2020 2020 2020 7c20  m-v1.0        | 
+00001fa0: 5346 5420 4d6f 6465 6c20 2020 2020 2020  SFT Model       
+00001fb0: 207c 2065 6e20 2020 2020 2020 7c20 6767   | en       | gg
+00001fc0: 6d6c 7633 207c 2037 2c20 3133 2c20 3333  mlv3 | 7, 13, 33
+00001fd0: 2020 2020 2020 2020 2020 7c20 2771 325f            | 'q2_
+00001fe0: 4b27 2c20 2771 335f 4b5f 4c27 2c20 2e2e  K', 'q3_K_L', ..
+00001ff0: 2e20 2c20 2771 365f 4b27 2c20 2771 385f  . , 'q6_K', 'q8_
+00002000: 3027 207c 0a7c 2076 6963 756e 612d 7631  0' |.| vicuna-v1
+00002010: 2e33 2020 2020 2020 2020 2020 7c20 5346  .3          | SF
+00002020: 5420 4d6f 6465 6c20 2020 2020 2020 207c  T Model        |
+00002030: 2065 6e20 2020 2020 2020 7c20 6767 6d6c   en       | ggml
+00002040: 7633 207c 2037 2c20 3133 2020 2020 2020  v3 | 7, 13      
+00002050: 2020 2020 2020 2020 7c20 2771 325f 4b27          | 'q2_K'
+00002060: 2c20 2771 335f 4b5f 4c27 2c20 2e2e 2e20  , 'q3_K_L', ... 
+00002070: 2c20 2771 365f 4b27 2c20 2771 385f 3027  , 'q6_K', 'q8_0'
+00002080: 207c 0a7c 206f 7263 6120 2020 2020 2020   |.| orca       
+00002090: 2020 2020 2020 2020 2020 7c20 5346 5420            | SFT 
+000020a0: 4d6f 6465 6c20 2020 2020 2020 207c 2065  Model        | e
+000020b0: 6e20 2020 2020 2020 7c20 6767 6d6c 7633  n       | ggmlv3
+000020c0: 207c 2033 2c20 372c 2031 3320 2020 2020   | 3, 7, 13     
+000020d0: 2020 2020 2020 7c20 2771 345f 3027 2c20        | 'q4_0', 
+000020e0: 2771 345f 3127 2c20 2771 355f 3027 2c20  'q4_1', 'q5_0', 
+000020f0: 2771 355f 3127 2c20 2771 385f 3027 207c  'q5_1', 'q8_0' |
+00002100: 0a0a 0a2a 2a4e 4f54 452a 2a3a 0a2d 2058  ...**NOTE**:.- X
+00002110: 696e 6665 7265 6e63 6520 7769 6c6c 2064  inference will d
+00002120: 6f77 6e6c 6f61 6420 6d6f 6465 6c73 2061  ownload models a
+00002130: 7574 6f6d 6174 6963 616c 6c79 2066 6f72  utomatically for
+00002140: 2079 6f75 2c20 616e 6420 6279 2064 6566   you, and by def
+00002150: 6175 6c74 2074 6865 206d 6f64 656c 7320  ault the models 
+00002160: 7769 6c6c 2062 6520 7361 7665 6420 756e  will be saved un
+00002170: 6465 7220 6024 7b55 5345 527d 2f2e 7869  der `${USER}/.xi
+00002180: 6e66 6572 656e 6365 2f63 6163 6865 602e  nference/cache`.
+00002190: 0a2d 2046 6f75 6e64 6174 696f 6e20 6d6f  .- Foundation mo
+000021a0: 6465 6c73 206f 6e6c 7920 7072 6f76 6964  dels only provid
+000021b0: 6520 696e 7465 7266 6163 6520 6067 656e  e interface `gen
+000021c0: 6572 6174 6560 2e0a 2d20 5346 5420 6d6f  erate`..- SFT mo
+000021d0: 6465 6c73 2070 726f 7669 6465 2062 6f74  dels provide bot
+000021e0: 6820 6067 656e 6572 6174 6560 2061 6e64  h `generate` and
+000021f0: 2060 6368 6174 602e 0a0a 2323 2052 6f61   `chat`...## Roa
+00002200: 646d 6170 0a58 696e 6665 7265 6e63 6520  dmap.Xinference 
+00002210: 6973 2063 7572 7265 6e74 6c79 2075 6e64  is currently und
+00002220: 6572 2061 6374 6976 6520 6465 7665 6c6f  er active develo
+00002230: 706d 656e 742e 2048 6572 6527 7320 6120  pment. Here's a 
+00002240: 726f 6164 6d61 7020 6f75 746c 696e 696e  roadmap outlinin
+00002250: 6720 6f75 7220 706c 616e 6e65 6420 0a64  g our planned .d
+00002260: 6576 656c 6f70 6d65 6e74 7320 666f 7220  evelopments for 
+00002270: 7468 6520 6e65 7874 2066 6577 2077 6565  the next few wee
+00002280: 6b73 3a0a 0a23 2323 2050 7954 6f72 6368  ks:..### PyTorch
+00002290: 2053 7570 706f 7274 0a57 6974 6820 5079   Support.With Py
+000022a0: 546f 7263 6820 696e 7465 6772 6174 696f  Torch integratio
+000022b0: 6e2c 2075 7365 7273 2077 696c 6c20 6265  n, users will be
+000022c0: 2061 626c 6520 746f 2073 6561 6d6c 6573   able to seamles
+000022d0: 736c 7920 7574 696c 697a 6520 5079 546f  sly utilize PyTo
+000022e0: 7263 6820 6d6f 6465 6c73 2066 726f 6d20  rch models from 
+000022f0: 4875 6767 696e 6720 4661 6365 0a77 6974  Hugging Face.wit
+00002300: 6869 6e20 5869 6e66 6572 656e 6365 2e0a  hin Xinference..
+00002310: 0a23 2323 204c 616e 6763 6861 696e 2026  .### Langchain &
+00002320: 204c 6c61 6d61 496e 6465 7820 696e 7465   LlamaIndex inte
+00002330: 6772 6174 696f 6e0a 5769 7468 2058 696e  gration.With Xin
+00002340: 6665 7265 6e63 652c 2069 7420 7769 6c6c  ference, it will
+00002350: 2062 6520 6d75 6368 2065 6173 6965 7220   be much easier 
+00002360: 666f 7220 7573 6572 7320 746f 2075 7365  for users to use
+00002370: 2074 6865 7365 206c 6962 7261 7269 6573   these libraries
+00002380: 2061 6e64 2062 7569 6c64 2061 7070 6c69   and build appli
+00002390: 6361 7469 6f6e 7320 0a77 6974 6820 4c4c  cations .with LL
+000023a0: 4d73 2e0a                                Ms..
```

### Comparing `xinference-0.0.2/setup.cfg` & `xinference-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/setup.py` & `xinference-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/versioneer.py` & `xinference-0.0.3/versioneer.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/__init__.py` & `xinference-0.0.3/xinference/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/client.py` & `xinference-0.0.3/xinference/client.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/constants.py` & `xinference-0.0.3/xinference/constants.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/core/__init__.py` & `xinference-0.0.3/xinference/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/core/api.py` & `xinference-0.0.3/xinference/core/api.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/core/gradio.py` & `xinference-0.0.3/xinference/core/gradio.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 class GradioApp:
     def __init__(
         self,
         supervisor_address: str,
         gladiator_num: int = 2,
-        max_model_num: int = 2,
+        max_model_num: int = 3,
         use_launched_model: bool = False,
     ):
         self._api = SyncSupervisorAPI(supervisor_address)
         self._gladiator_num = gladiator_num
         self._max_model_num = max_model_num
         self._use_launched_model = use_launched_model
         self._locale = Locale()
@@ -309,18 +309,19 @@
 
         def clear_chat(
             _model_name: str,
             _model_format: str,
             _model_size_in_billions: str,
             _quantization: str,
         ):
-            return _model_name, gr.Chatbot.update(
-                label="-".join(
-                    [_model_name, _model_size_in_billions, _model_format, _quantization]
-                ),
+            full_name = "-".join(
+                [_model_name, _model_size_in_billions, _model_format, _quantization]
+            )
+            return str(uuid.uuid4()), gr.Chatbot.update(
+                label=full_name,
                 value=[],
             )
 
         invisible_text = gr.Textbox(visible=False)
         create_model.click(
             clear_chat,
             inputs=[model_name, model_format, model_size_in_billions, quantization],
```

### Comparing `xinference-0.0.2/xinference/core/model.py` & `xinference-0.0.3/xinference/core/model.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/core/resource.py` & `xinference-0.0.3/xinference/core/resource.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/core/restful_api.py` & `xinference-0.0.3/xinference/core/restful_api.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/core/service.py` & `xinference-0.0.3/xinference/core/service.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/deploy/__init__.py` & `xinference-0.0.3/xinference/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/deploy/cmdline.py` & `xinference-0.0.3/xinference/deploy/cmdline.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/deploy/local.py` & `xinference-0.0.3/xinference/deploy/local.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/deploy/supervisor.py` & `xinference-0.0.3/xinference/deploy/supervisor.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/deploy/test/__init__.py` & `xinference-0.0.3/xinference/deploy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/deploy/utils.py` & `xinference-0.0.3/xinference/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/deploy/worker.py` & `xinference-0.0.3/xinference/deploy/worker.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/isolation.py` & `xinference-0.0.3/xinference/isolation.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/locale/__init__.py` & `xinference-0.0.3/xinference/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/locale/utils.py` & `xinference-0.0.3/xinference/locale/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/locale/zh_CN.json` & `xinference-0.0.3/xinference/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/model/__init__.py` & `xinference-0.0.3/xinference/model/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/model/llm/__init__.py` & `xinference-0.0.3/xinference/model/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/model/llm/chatglm.py` & `xinference-0.0.3/xinference/model/llm/chatglm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/model/llm/core.py` & `xinference-0.0.3/xinference/model/llm/core.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/model/llm/orca.py` & `xinference-0.0.3/xinference/model/llm/orca.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/model/llm/vicuna.py` & `xinference-0.0.3/xinference/model/llm/vicuna.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/model/llm/wizardlm.py` & `xinference-0.0.3/xinference/model/llm/wizardlm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference/types.py` & `xinference-0.0.3/xinference/types.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.2/xinference.egg-info/PKG-INFO` & `xinference-0.0.3/xinference.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7869 6e66  : 2.1.Name: xinf
 00000020: 6572 656e 6365 0a56 6572 7369 6f6e 3a20  erence.Version: 
-00000030: 302e 302e 320a 5375 6d6d 6172 793a 204d  0.0.2.Summary: M
+00000030: 302e 302e 330a 5375 6d6d 6172 793a 204d  0.0.3.Summary: M
 00000040: 6f64 656c 2053 6572 7669 6e67 204d 6164  odel Serving Mad
 00000050: 6520 4561 7379 0a48 6f6d 652d 7061 6765  e Easy.Home-page
 00000060: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
 00000070: 2e63 6f6d 2f78 6f72 6269 7473 6169 2f69  .com/xorbitsai/i
 00000080: 6e66 6572 656e 6365 0a41 7574 686f 723a  nference.Author:
 00000090: 2051 696e 2058 7579 650a 4175 7468 6f72   Qin Xuye.Author
 000000a0: 2d65 6d61 696c 3a20 7169 6e78 7579 6540  -email: qinxuye@
@@ -153,461 +153,471 @@
 00000980: 2773 2073 7570 706f 7274 2074 6f20 696e  's support to in
 00000990: 636c 7564 6520 6164 6469 7469 6f6e 616c  clude additional
 000009a0: 2072 756e 7469 6d65 732c 200a 696e 636c   runtimes, .incl
 000009b0: 7564 696e 6720 5079 546f 7263 6820 616e  uding PyTorch an
 000009c0: 6420 4a41 582c 2069 6e20 7468 6520 6e65  d JAX, in the ne
 000009d0: 6172 2066 7574 7572 652e 0a0a 215b 6465  ar future...![de
 000009e0: 6d6f 5d28 6173 7365 7473 2f64 656d 6f2e  mo](assets/demo.
-000009f0: 6769 6629 0a0a 0a23 2320 4b65 7920 4665  gif)...## Key Fe
-00000a00: 6174 7572 6573 0af0 9f8c 9f20 2a2a 4d6f  atures..... **Mo
-00000a10: 6465 6c20 5365 7276 696e 6720 4d61 6465  del Serving Made
-00000a20: 2045 6173 792a 2a3a 2049 6e66 6572 656e   Easy**: Inferen
-00000a30: 6365 2073 696d 706c 6966 6965 7320 7468  ce simplifies th
-00000a40: 6520 7072 6f63 6573 7320 6f66 2073 6572  e process of ser
-00000a50: 7669 6e67 206c 6172 6765 206c 616e 6775  ving large langu
-00000a60: 6167 652c 2073 7065 6563 6820 0a72 6563  age, speech .rec
-00000a70: 6f67 6e69 7469 6f6e 2c20 616e 6420 6d75  ognition, and mu
-00000a80: 6c74 696d 6f64 616c 206d 6f64 656c 732e  ltimodal models.
-00000a90: 2059 6f75 2063 616e 2073 6574 2075 7020   You can set up 
-00000aa0: 616e 6420 6465 706c 6f79 2079 6f75 7220  and deploy your 
-00000ab0: 6d6f 6465 6c73 0a66 6f72 2065 7870 6572  models.for exper
-00000ac0: 696d 656e 7461 7469 6f6e 2061 6e64 2070  imentation and p
-00000ad0: 726f 6475 6374 696f 6e20 7769 7468 2061  roduction with a
-00000ae0: 2073 696e 676c 6520 636f 6d6d 616e 642e   single command.
-00000af0: 0a0a e29a a1ef b88f 202a 2a53 7461 7465  ........ **State
-00000b00: 2d6f 662d 7468 652d 4172 7420 4d6f 6465  -of-the-Art Mode
-00000b10: 6c73 2a2a 3a20 4578 7065 7269 6d65 6e74  ls**: Experiment
-00000b20: 2077 6974 6820 6375 7474 696e 672d 6564   with cutting-ed
-00000b30: 6765 2062 7569 6c74 2d69 6e20 6d6f 6465  ge built-in mode
-00000b40: 6c73 2075 7369 6e67 2061 2073 696e 676c  ls using a singl
-00000b50: 6520 0a63 6f6d 6d61 6e64 2e20 496e 6665  e .command. Infe
-00000b60: 7265 6e63 6520 7072 6f76 6964 6573 2061  rence provides a
-00000b70: 6363 6573 7320 746f 2073 7461 7465 2d6f  ccess to state-o
-00000b80: 662d 7468 652d 6172 7420 6f70 656e 2d73  f-the-art open-s
-00000b90: 6f75 7263 6520 6d6f 6465 6c73 210a 0af0  ource models!...
-00000ba0: 9f96 a520 2a2a 4865 7465 726f 6765 6e65  ... **Heterogene
-00000bb0: 6f75 7320 4861 7264 7761 7265 2055 7469  ous Hardware Uti
-00000bc0: 6c69 7a61 7469 6f6e 2a2a 3a20 4d61 6b65  lization**: Make
-00000bd0: 2074 6865 206d 6f73 7420 6f66 2079 6f75   the most of you
-00000be0: 7220 6861 7264 7761 7265 2072 6573 6f75  r hardware resou
-00000bf0: 7263 6573 2e20 586f 7262 6974 7320 0a49  rces. Xorbits .I
-00000c00: 6e66 6572 656e 6365 2069 6e74 656c 6c69  nference intelli
-00000c10: 6765 6e74 6c79 2075 7469 6c69 7a65 7320  gently utilizes 
-00000c20: 6865 7465 726f 6765 6e65 6f75 7320 6861  heterogeneous ha
-00000c30: 7264 7761 7265 2c20 696e 636c 7564 696e  rdware, includin
-00000c40: 6720 4750 5573 2061 6e64 2043 5055 732c  g GPUs and CPUs,
-00000c50: 2074 6f20 6d61 7869 6d69 7a65 0a70 6572   to maximize.per
-00000c60: 666f 726d 616e 6365 2061 6e64 2061 6363  formance and acc
-00000c70: 656c 6572 6174 6520 796f 7572 206d 6f64  elerate your mod
-00000c80: 656c 2069 6e66 6572 656e 6365 2074 6173  el inference tas
-00000c90: 6b73 2e0a 0ae2 9a99 efb8 8f20 2a2a 466c  ks......... **Fl
-00000ca0: 6578 6962 6c65 2041 5049 2061 6e64 2049  exible API and I
-00000cb0: 6e74 6572 6661 6365 732a 2a3a 2058 6f72  nterfaces**: Xor
-00000cc0: 6269 7473 2049 6e66 6572 656e 6365 206f  bits Inference o
-00000cd0: 6666 6572 7320 6d75 6c74 6970 6c65 2069  ffers multiple i
-00000ce0: 6e74 6572 6661 6365 7320 666f 7220 696e  nterfaces for in
-00000cf0: 7465 7261 6374 696e 670a 7769 7468 2079  teracting.with y
-00000d00: 6f75 7220 6d6f 6465 6c73 2e20 596f 7520  our models. You 
-00000d10: 6361 6e20 7574 696c 697a 6520 7468 6520  can utilize the 
-00000d20: 5250 4320 616e 6420 5245 5354 6675 6c20  RPC and RESTful 
-00000d30: 4150 4928 636f 6d70 6174 6962 6c65 2077  API(compatible w
-00000d40: 6974 6820 4f70 656e 4149 2041 5049 2920  ith OpenAI API) 
-00000d50: 746f 2069 6e74 6567 7261 7465 0a79 6f75  to integrate.you
-00000d60: 7220 6d6f 6465 6c73 2077 6974 6820 6578  r models with ex
-00000d70: 6973 7469 6e67 2073 7973 7465 6d73 206f  isting systems o
-00000d80: 7220 7573 6520 7468 6520 636f 6d6d 616e  r use the comman
-00000d90: 642d 6c69 6e65 2069 6e74 6572 6661 6365  d-line interface
-00000da0: 2028 434c 4929 2061 6e64 2074 6865 2069   (CLI) and the i
-00000db0: 6e74 7569 7469 7665 2057 6562 5549 0a66  ntuitive WebUI.f
-00000dc0: 6f72 2073 6561 6d6c 6573 7320 6d61 6e61  or seamless mana
-00000dd0: 6765 6d65 6e74 2061 6e64 206d 6f6e 6974  gement and monit
-00000de0: 6f72 696e 672e 0a0a f09f 8c90 202a 2a44  oring....... **D
-00000df0: 6973 7472 6962 7574 6564 2044 6570 6c6f  istributed Deplo
-00000e00: 796d 656e 742a 2a3a 2058 6f72 6269 7473  yment**: Xorbits
-00000e10: 2049 6e66 6572 656e 6365 2065 7863 656c   Inference excel
-00000e20: 7320 696e 2064 6973 7472 6962 7574 6564  s in distributed
-00000e30: 2064 6570 6c6f 796d 656e 7420 7363 656e   deployment scen
-00000e40: 6172 696f 732c 200a 616c 6c6f 7769 6e67  arios, .allowing
-00000e50: 2074 6865 2073 6561 6d6c 6573 7320 6469   the seamless di
-00000e60: 7374 7269 6275 7469 6f6e 206f 6620 6d6f  stribution of mo
-00000e70: 6465 6c20 696e 6665 7265 6e63 6520 6163  del inference ac
-00000e80: 726f 7373 206d 756c 7469 706c 6520 6465  ross multiple de
-00000e90: 7669 6365 7320 6f72 206d 6163 6869 6e65  vices or machine
-00000ea0: 732e 2049 740a 6c65 7665 7261 6765 7320  s. It.leverages 
-00000eb0: 6469 7374 7269 6275 7465 6420 636f 6d70  distributed comp
-00000ec0: 7574 696e 6720 7465 6368 6e69 7175 6573  uting techniques
-00000ed0: 2074 6f20 7061 7261 6c6c 656c 697a 6520   to parallelize 
-00000ee0: 616e 6420 7363 616c 6520 7468 6520 696e  and scale the in
-00000ef0: 6665 7265 6e63 6520 7072 6f63 6573 732e  ference process.
-00000f00: 0a0a f09f 948c 202a 2a42 7569 6c74 2d69  ...... **Built-i
-00000f10: 6e20 496e 7465 6772 6174 696f 6e20 7769  n Integration wi
-00000f20: 7468 2054 6869 7264 2d50 6172 7479 204c  th Third-Party L
-00000f30: 6962 7261 7269 6573 2a2a 3a20 586f 7262  ibraries**: Xorb
-00000f40: 6974 7320 496e 6665 7265 6e63 6520 7365  its Inference se
-00000f50: 616d 6c65 7373 6c79 2069 6e74 6567 7261  amlessly integra
-00000f60: 7465 730a 7769 7468 2070 6f70 756c 6172  tes.with popular
-00000f70: 2074 6869 7264 2d70 6172 7479 206c 6962   third-party lib
-00000f80: 7261 7269 6573 206c 696b 6520 4c61 6e67  raries like Lang
-00000f90: 4368 6169 6e20 616e 6420 4c6c 616d 6149  Chain and LlamaI
-00000fa0: 6e64 6578 2e20 2843 6f6d 696e 6720 736f  ndex. (Coming so
-00000fb0: 6f6e 290a 0a23 2320 4765 7474 696e 6720  on)..## Getting 
-00000fc0: 5374 6172 7465 640a 5869 6e66 6572 656e  Started.Xinferen
-00000fd0: 6365 2063 616e 2062 6520 696e 7374 616c  ce can be instal
-00000fe0: 6c65 6420 7669 6120 7069 7020 6672 6f6d  led via pip from
-00000ff0: 2050 7950 492e 2049 7420 6973 2068 6967   PyPI. It is hig
-00001000: 686c 7920 7265 636f 6d6d 656e 6465 6420  hly recommended 
-00001010: 746f 2063 7265 6174 6520 6120 6e65 7720  to create a new 
-00001020: 7669 7274 7561 6c0a 656e 7669 726f 6e6d  virtual.environm
-00001030: 656e 7420 746f 2061 766f 6964 2063 6f6e  ent to avoid con
-00001040: 666c 6963 7473 2e0a 6060 6062 6173 680a  flicts..```bash.
-00001050: 2420 7069 7020 696e 7374 616c 6c20 2278  $ pip install "x
-00001060: 696e 6665 7265 6e63 655b 616c 6c5d 220a  inference[all]".
-00001070: 6060 600a 2278 696e 6665 7265 6e63 655b  ```."xinference[
-00001080: 616c 6c5d 2220 696e 7374 616c 6c73 2061  all]" installs a
-00001090: 6c6c 2074 6865 206e 6563 6573 7361 7279  ll the necessary
-000010a0: 2070 6163 6b61 6765 7320 666f 7220 7365   packages for se
-000010b0: 7276 696e 6720 6d6f 6465 6c73 2e20 4966  rving models. If
-000010c0: 2079 6f75 2077 616e 7420 746f 2061 6368   you want to ach
-000010d0: 6965 7665 2061 6363 656c 6572 6174 696f  ieve acceleratio
-000010e0: 6e20 6f6e 200a 6469 6666 6572 656e 7420  n on .different 
-000010f0: 6861 7264 7761 7265 2c20 7265 6665 7220  hardware, refer 
-00001100: 746f 2074 6865 2069 6e73 7461 6c6c 6174  to the installat
-00001110: 696f 6e20 646f 6375 6d65 6e74 6174 696f  ion documentatio
-00001120: 6e20 6f66 2074 6865 2063 6f72 7265 7370  n of the corresp
-00001130: 6f6e 6469 6e67 2070 6163 6b61 6765 2e0a  onding package..
-00001140: 2d20 5b6c 6c61 6d61 2d63 7070 2d70 7974  - [llama-cpp-pyt
-00001150: 686f 6e5d 2868 7474 7073 3a2f 2f67 6974  hon](https://git
-00001160: 6875 622e 636f 6d2f 6162 6574 6c65 6e2f  hub.com/abetlen/
-00001170: 6c6c 616d 612d 6370 702d 7079 7468 6f6e  llama-cpp-python
-00001180: 2369 6e73 7461 6c6c 6174 696f 6e2d 6672  #installation-fr
-00001190: 6f6d 2d70 7970 692d 7265 636f 6d6d 656e  om-pypi-recommen
-000011a0: 6465 6429 2069 7320 7265 7175 6972 6564  ded) is required
-000011b0: 2074 6f20 7275 6e20 6062 6169 6368 7561   to run `baichua
-000011c0: 6e60 2c20 6077 697a 6172 646c 6d2d 7631  n`, `wizardlm-v1
-000011d0: 2e30 602c 2060 7669 6375 6e61 2d76 312e  .0`, `vicuna-v1.
-000011e0: 3360 2061 6e64 2060 6f72 6361 602e 0a2d  3` and `orca`..-
-000011f0: 205b 6368 6174 676c 6d2d 6370 702d 7079   [chatglm-cpp-py
-00001200: 7468 6f6e 5d28 6874 7470 733a 2f2f 6769  thon](https://gi
-00001210: 7468 7562 2e63 6f6d 2f6c 692d 706c 7573  thub.com/li-plus
-00001220: 2f63 6861 7467 6c6d 2e63 7070 2367 6574  /chatglm.cpp#get
-00001230: 7469 6e67 2d73 7461 7274 6564 2920 6973  ting-started) is
-00001240: 2072 6571 7569 7265 6420 746f 2072 756e   required to run
-00001250: 2060 6368 6174 676c 6d60 2061 6e64 2060   `chatglm` and `
-00001260: 6368 6174 676c 6d32 602e 0a0a 0a23 2323  chatglm2`....###
-00001270: 2044 6570 6c6f 796d 656e 740a 596f 7520   Deployment.You 
-00001280: 6361 6e20 6465 706c 6f79 2058 696e 6665  can deploy Xinfe
-00001290: 7265 6e63 6520 6c6f 6361 6c6c 7920 7769  rence locally wi
-000012a0: 7468 2061 2073 696e 676c 6520 636f 6d6d  th a single comm
-000012b0: 616e 6420 6f72 2064 6570 6c6f 7920 6974  and or deploy it
-000012c0: 2069 6e20 6120 6469 7374 7269 6275 7465   in a distribute
-000012d0: 6420 636c 7573 7465 722e 200a 0a23 2323  d cluster. ..###
-000012e0: 2320 4c6f 6361 6c0a 546f 2073 7461 7274  # Local.To start
-000012f0: 2061 206c 6f63 616c 2069 6e73 7461 6e63   a local instanc
-00001300: 6520 6f66 2058 696e 6665 7265 6e63 652c  e of Xinference,
-00001310: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
-00001320: 6e67 2063 6f6d 6d61 6e64 3a0a 6060 6062  ng command:.```b
-00001330: 6173 680a 2420 7869 6e66 6572 656e 6365  ash.$ xinference
-00001340: 0a60 6060 0a0a 2323 2323 2044 6973 7472  .```..#### Distr
-00001350: 6962 7574 6564 0a0a 546f 2064 6570 6c6f  ibuted..To deplo
-00001360: 7920 5869 6e66 6572 656e 6365 2069 6e20  y Xinference in 
-00001370: 6120 636c 7573 7465 722c 2079 6f75 206e  a cluster, you n
-00001380: 6565 6420 746f 2073 7461 7274 2061 2058  eed to start a X
-00001390: 696e 6665 7265 6e63 6520 7375 7065 7276  inference superv
-000013a0: 6973 6f72 206f 6e20 6f6e 6520 7365 7276  isor on one serv
-000013b0: 6572 2061 6e64 200a 5869 6e66 6572 656e  er and .Xinferen
-000013c0: 6365 2077 6f72 6b65 7273 206f 6e20 7468  ce workers on th
-000013d0: 6520 6f74 6865 7220 7365 7276 6572 732e  e other servers.
-000013e0: 2046 6f6c 6c6f 7720 7468 6520 7374 6570   Follow the step
-000013f0: 7320 6265 6c6f 773a 0a0a 2a2a 5374 6172  s below:..**Star
-00001400: 7469 6e67 2074 6865 2053 7570 6572 7669  ting the Supervi
-00001410: 736f 722a 2a3a 204f 6e20 7468 6520 7365  sor**: On the se
-00001420: 7276 6572 2077 6865 7265 2079 6f75 2077  rver where you w
-00001430: 616e 7420 746f 2072 756e 2074 6865 2058  ant to run the X
-00001440: 696e 6665 7265 6e63 6520 7375 7065 7276  inference superv
-00001450: 6973 6f72 2c20 7275 6e20 7468 6520 666f  isor, run the fo
-00001460: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
-00001470: 0a60 6060 6261 7368 0a24 2078 696e 6665  .```bash.$ xinfe
-00001480: 7265 6e63 652d 7375 7065 7276 6973 6f72  rence-supervisor
-00001490: 202d 4820 2224 7b73 7570 6572 7669 736f   -H "${superviso
-000014a0: 725f 686f 7374 7d22 0a60 6060 0a52 6570  r_host}".```.Rep
-000014b0: 6c61 6365 2060 247b 7375 7065 7276 6973  lace `${supervis
-000014c0: 6f72 5f68 6f73 747d 6020 7769 7468 2074  or_host}` with t
-000014d0: 6865 2061 6374 7561 6c20 686f 7374 206f  he actual host o
-000014e0: 6620 796f 7572 2073 7570 6572 7669 736f  f your superviso
-000014f0: 7220 7365 7276 6572 2e0a 0a2a 2a53 7461  r server...**Sta
-00001500: 7274 696e 6720 7468 6520 576f 726b 6572  rting the Worker
-00001510: 732a 2a3a 204f 6e20 6561 6368 206f 6620  s**: On each of 
-00001520: 7468 6520 6f74 6865 7220 7365 7276 6572  the other server
-00001530: 7320 7768 6572 6520 796f 7520 7761 6e74  s where you want
-00001540: 2074 6f20 7275 6e20 5869 6e66 6572 656e   to run Xinferen
-00001550: 6365 2077 6f72 6b65 7273 2c20 7275 6e20  ce workers, run 
-00001560: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00001570: 6d6d 616e 643a 0a60 6060 6261 7368 0a24  mmand:.```bash.$
-00001580: 2078 696e 6665 7265 6e63 652d 776f 726b   xinference-work
-00001590: 6572 202d 6520 2268 7474 703a 2f2f 247b  er -e "http://${
-000015a0: 7375 7065 7276 6973 6f72 5f68 6f73 747d  supervisor_host}
-000015b0: 3a39 3939 3722 0a60 6060 0a0a 4f6e 6365  :9997".```..Once
-000015c0: 2058 696e 6665 7265 6e63 6520 6973 2072   Xinference is r
-000015d0: 756e 6e69 6e67 2c20 616e 2065 6e64 706f  unning, an endpo
-000015e0: 696e 7420 7769 6c6c 2062 6520 6163 6365  int will be acce
-000015f0: 7373 6962 6c65 2066 6f72 206d 6f64 656c  ssible for model
-00001600: 206d 616e 6167 656d 656e 7420 7669 6120   management via 
-00001610: 434c 4920 6f72 0a58 696e 6665 7265 6e63  CLI or.Xinferenc
-00001620: 6520 2063 6c69 656e 742e 0a0a 2d20 466f  e  client...- Fo
-00001630: 7220 6c6f 6361 6c20 6465 706c 6f79 6d65  r local deployme
-00001640: 6e74 2c20 7468 6520 656e 6470 6f69 6e74  nt, the endpoint
-00001650: 2077 696c 6c20 6265 2060 6874 7470 3a2f   will be `http:/
-00001660: 2f6c 6f63 616c 686f 7374 3a39 3939 3760  /localhost:9997`
-00001670: 2e0a 2d20 466f 7220 636c 7573 7465 7220  ..- For cluster 
-00001680: 6465 706c 6f79 6d65 6e74 2c20 7468 6520  deployment, the 
-00001690: 656e 6470 6f69 6e74 2077 696c 6c20 6265  endpoint will be
-000016a0: 2060 6874 7470 3a2f 2f24 7b73 7570 6572   `http://${super
-000016b0: 7669 736f 725f 686f 7374 7d3a 3939 3937  visor_host}:9997
-000016c0: 602c 2077 6865 7265 0a60 247b 7375 7065  `, where.`${supe
-000016d0: 7276 6973 6f72 5f68 6f73 747d 6020 6973  rvisor_host}` is
-000016e0: 2074 6865 2068 6f73 746e 616d 6520 6f72   the hostname or
-000016f0: 2049 5020 6164 6472 6573 7320 6f66 2074   IP address of t
-00001700: 6865 2073 6572 7665 7220 7768 6572 6520  he server where 
-00001710: 7468 6520 7375 7065 7276 6973 6f72 2069  the supervisor i
-00001720: 7320 7275 6e6e 696e 672e 0a0a 596f 7520  s running...You 
-00001730: 6361 6e20 616c 736f 2076 6965 7720 6120  can also view a 
-00001740: 7765 6220 5549 2075 7369 6e67 2074 6865  web UI using the
-00001750: 2058 696e 6665 7265 6e63 6520 656e 6470   Xinference endp
-00001760: 6f69 6e74 2074 6f20 6368 6174 2077 6974  oint to chat wit
-00001770: 6820 616c 6c20 7468 6520 0a62 7569 6c74  h all the .built
-00001780: 696e 206d 6f64 656c 732e 2059 6f75 2063  in models. You c
-00001790: 616e 2065 7665 6e20 2a2a 6368 6174 2077  an even **chat w
-000017a0: 6974 6820 7477 6f20 6375 7474 696e 672d  ith two cutting-
-000017b0: 6564 6765 2041 4920 6d6f 6465 6c73 2073  edge AI models s
-000017c0: 6964 652d 6279 2d73 6964 6520 746f 2063  ide-by-side to c
-000017d0: 6f6d 7061 7265 0a74 6865 6972 2070 6572  ompare.their per
-000017e0: 666f 726d 616e 6365 2a2a 210a 0a21 5b77  formance**!..![w
-000017f0: 6562 2055 495d 2861 7373 6574 732f 7869  eb UI](assets/xi
-00001800: 6e66 6572 656e 6365 2d64 6f77 6e6c 6f61  nference-downloa
-00001810: 6469 6e67 2e70 6e67 290a 0a23 2323 2058  ding.png)..### X
-00001820: 696e 6665 7265 6e63 6520 434c 490a 5869  inference CLI.Xi
-00001830: 6e66 6572 656e 6365 2070 726f 7669 6465  nference provide
-00001840: 7320 6120 636f 6d6d 616e 6420 6c69 6e65  s a command line
-00001850: 2069 6e74 6572 6661 6365 2028 434c 4929   interface (CLI)
-00001860: 2066 6f72 206d 6f64 656c 206d 616e 6167   for model manag
-00001870: 656d 656e 742e 2048 6572 6520 6172 6520  ement. Here are 
-00001880: 736f 6d65 2075 7365 6675 6c20 0a63 6f6d  some useful .com
-00001890: 6d61 6e64 733a 0a0a 2d20 4c61 756e 6368  mands:..- Launch
-000018a0: 2061 206d 6f64 656c 2028 6120 6d6f 6465   a model (a mode
-000018b0: 6c20 5549 4420 7769 6c6c 2062 6520 7265  l UID will be re
-000018c0: 7475 726e 6564 293a 2060 7869 6e66 6572  turned): `xinfer
-000018d0: 656e 6365 206c 6175 6e63 6860 0a2d 204c  ence launch`.- L
-000018e0: 6973 7420 7275 6e6e 696e 6720 6d6f 6465  ist running mode
-000018f0: 6c73 3a20 6078 696e 6665 7265 6e63 6520  ls: `xinference 
-00001900: 6c69 7374 600a 2d20 4c69 7374 2061 6c6c  list`.- List all
-00001910: 2074 6865 2062 7569 6c74 696e 206d 6f64   the builtin mod
-00001920: 656c 733a 2060 7869 6e66 6572 656e 6365  els: `xinference
-00001930: 206c 6973 7420 2d2d 616c 6c60 0a2d 2054   list --all`.- T
-00001940: 6572 6d69 6e61 7465 2061 206d 6f64 656c  erminate a model
-00001950: 3a20 6078 696e 6665 7265 6e63 6520 7465  : `xinference te
-00001960: 726d 696e 6174 6520 2d2d 6d6f 6465 6c2d  rminate --model-
-00001970: 7569 6420 247b 6d6f 6465 6c5f 7569 647d  uid ${model_uid}
-00001980: 600a 0a23 2323 2058 696e 6665 7265 6e63  `..### Xinferenc
-00001990: 6520 436c 6965 6e74 0a58 696e 6665 7265  e Client.Xinfere
-000019a0: 6e63 6520 616c 736f 2070 726f 7669 6465  nce also provide
-000019b0: 7320 6120 636c 6965 6e74 2066 6f72 206d  s a client for m
-000019c0: 616e 6167 696e 6720 616e 6420 6163 6365  anaging and acce
-000019d0: 7373 696e 6720 6d6f 6465 6c73 2070 726f  ssing models pro
-000019e0: 6772 616d 6d61 7469 6361 6c6c 793a 0a0a  grammatically:..
-000019f0: 6060 6070 7974 686f 6e0a 6672 6f6d 2078  ```python.from x
-00001a00: 696e 6665 7265 6e63 652e 636c 6965 6e74  inference.client
-00001a10: 2069 6d70 6f72 7420 436c 6965 6e74 0a0a   import Client..
-00001a20: 636c 6965 6e74 203d 2043 6c69 656e 7428  client = Client(
-00001a30: 2268 7474 703a 2f2f 6c6f 6361 6c68 6f73  "http://localhos
-00001a40: 743a 3939 3937 2229 0a6d 6f64 656c 5f75  t:9997").model_u
-00001a50: 6964 203d 2063 6c69 656e 742e 6c61 756e  id = client.laun
-00001a60: 6368 5f6d 6f64 656c 286d 6f64 656c 5f6e  ch_model(model_n
-00001a70: 616d 653d 2263 6861 7467 6c6d 3222 290a  ame="chatglm2").
-00001a80: 6d6f 6465 6c20 3d20 636c 6965 6e74 2e67  model = client.g
-00001a90: 6574 5f6d 6f64 656c 286d 6f64 656c 5f75  et_model(model_u
-00001aa0: 6964 290a 0a63 6861 745f 6869 7374 6f72  id)..chat_histor
-00001ab0: 7920 3d20 5b5d 0a70 726f 6d70 7420 3d20  y = [].prompt = 
-00001ac0: 2257 6861 7420 6973 2074 6865 206c 6172  "What is the lar
-00001ad0: 6765 7374 2061 6e69 6d61 6c3f 220a 6d6f  gest animal?".mo
-00001ae0: 6465 6c2e 6368 6174 280a 2020 2020 2020  del.chat(.      
-00001af0: 2020 2020 2020 7072 6f6d 7074 2c0a 2020        prompt,.  
-00001b00: 2020 2020 2020 2020 2020 6368 6174 5f68            chat_h
-00001b10: 6973 746f 7279 2c0a 2020 2020 2020 2020  istory,.        
-00001b20: 2020 2020 6765 6e65 7261 7465 5f63 6f6e      generate_con
-00001b30: 6669 673d 7b22 6d61 785f 746f 6b65 6e73  fig={"max_tokens
-00001b40: 223a 2031 3032 347d 0a20 2020 2020 2020  ": 1024}.       
-00001b50: 2029 0a60 6060 0a0a 5265 7375 6c74 3a0a   ).```..Result:.
-00001b60: 6060 606a 736f 6e0a 7b0a 2020 2269 6422  ```json.{.  "id"
-00001b70: 3a20 2263 6861 7463 6d70 6c2d 3864 3736  : "chatcmpl-8d76
-00001b80: 6236 3561 2d62 6164 302d 3432 6566 2d39  b65a-bad0-42ef-9
-00001b90: 3132 642d 3461 3035 3333 6439 3064 3631  12d-4a0533d90d61
-00001ba0: 222c 0a20 2022 6d6f 6465 6c22 3a20 2235  ",.  "model": "5
-00001bb0: 3666 3639 3632 322d 3165 3733 2d31 3165  6f69622-1e73-11e
-00001bc0: 652d 6133 6264 2d39 6166 3966 3136 3831  e-a3bd-9af9f1681
-00001bd0: 3663 3622 2c0a 2020 226f 626a 6563 7422  6c6",.  "object"
-00001be0: 3a20 2263 6861 742e 636f 6d70 6c65 7469  : "chat.completi
-00001bf0: 6f6e 222c 0a20 2022 6372 6561 7465 6422  on",.  "created"
-00001c00: 3a20 3136 3838 3931 3931 3837 2c0a 2020  : 1688919187,.  
-00001c10: 2263 686f 6963 6573 223a 205b 0a20 2020  "choices": [.   
-00001c20: 207b 0a20 2020 2020 2022 696e 6465 7822   {.      "index"
-00001c30: 3a20 302c 0a20 2020 2020 2022 6d65 7373  : 0,.      "mess
-00001c40: 6167 6522 3a20 7b0a 2020 2020 2020 2020  age": {.        
-00001c50: 2272 6f6c 6522 3a20 2261 7373 6973 7461  "role": "assista
-00001c60: 6e74 222c 0a20 2020 2020 2020 2022 636f  nt",.        "co
-00001c70: 6e74 656e 7422 3a20 2254 6865 206c 6172  ntent": "The lar
-00001c80: 6765 7374 2061 6e69 6d61 6c20 7468 6174  gest animal that
-00001c90: 2068 6173 2062 6565 6e20 7363 6965 6e74   has been scient
-00001ca0: 6966 6963 616c 6c79 206d 6561 7375 7265  ifically measure
-00001cb0: 6420 6973 2074 6865 2062 6c75 6520 7768  d is the blue wh
-00001cc0: 616c 652c 2077 6869 6368 2068 6173 2061  ale, which has a
-00001cd0: 206d 6178 696d 756d 206c 656e 6774 6820   maximum length 
-00001ce0: 6f66 2061 726f 756e 6420 3233 206d 6574  of around 23 met
-00001cf0: 6572 7320 2837 3520 6665 6574 2920 666f  ers (75 feet) fo
-00001d00: 7220 6164 756c 7420 616e 696d 616c 7320  r adult animals 
-00001d10: 616e 6420 6361 6e20 7765 6967 6820 7570  and can weigh up
-00001d20: 2074 6f20 3135 302c 3030 3020 706f 756e   to 150,000 poun
-00001d30: 6473 2028 3638 2c30 3030 206b 6729 2e20  ds (68,000 kg). 
-00001d40: 486f 7765 7665 722c 2069 7420 6973 2069  However, it is i
-00001d50: 6d70 6f72 7461 6e74 2074 6f20 6e6f 7465  mportant to note
-00001d60: 2074 6861 7420 7468 6973 2069 7320 6a75   that this is ju
-00001d70: 7374 2061 6e20 6573 7469 6d61 7465 2061  st an estimate a
-00001d80: 6e64 2074 6861 7420 7468 6520 6c61 7267  nd that the larg
-00001d90: 6573 7420 616e 696d 616c 206b 6e6f 776e  est animal known
-00001da0: 2074 6f20 7363 6965 6e63 6520 6d61 7920   to science may 
-00001db0: 6265 206c 6172 6765 7220 7374 696c 6c2e  be larger still.
-00001dc0: 2053 6f6d 6520 7363 6965 6e74 6973 7473   Some scientists
-00001dd0: 2062 656c 6965 7665 2074 6861 7420 7468   believe that th
-00001de0: 6520 6c61 7267 6573 7420 616e 696d 616c  e largest animal
-00001df0: 7320 6d61 7920 6e6f 7420 6861 7665 2061  s may not have a
-00001e00: 2063 6c65 6172 205c 2273 697a 655c 2220   clear \"size\" 
-00001e10: 696e 2074 6865 2073 616d 6520 7761 7920  in the same way 
-00001e20: 7468 6174 2068 756d 616e 7320 646f 2c20  that humans do, 
-00001e30: 6173 2074 6865 6972 2073 697a 6520 6361  as their size ca
-00001e40: 6e20 7661 7279 2064 6570 656e 6469 6e67  n vary depending
-00001e50: 206f 6e20 7468 6520 656e 7669 726f 6e6d   on the environm
-00001e60: 656e 7420 616e 6420 7468 6520 7374 6167  ent and the stag
-00001e70: 6520 6f66 2074 6865 6972 206c 6966 652e  e of their life.
-00001e80: 220a 2020 2020 2020 7d2c 0a20 2020 2020  ".      },.     
-00001e90: 2022 6669 6e69 7368 5f72 6561 736f 6e22   "finish_reason"
-00001ea0: 3a20 224e 6f6e 6522 0a20 2020 207d 0a20  : "None".    }. 
-00001eb0: 205d 2c0a 2020 2275 7361 6765 223a 207b   ],.  "usage": {
-00001ec0: 0a20 2020 2022 7072 6f6d 7074 5f74 6f6b  .    "prompt_tok
-00001ed0: 656e 7322 3a20 2d31 2c0a 2020 2020 2263  ens": -1,.    "c
-00001ee0: 6f6d 706c 6574 696f 6e5f 746f 6b65 6e73  ompletion_tokens
-00001ef0: 223a 202d 312c 0a20 2020 2022 746f 7461  ": -1,.    "tota
-00001f00: 6c5f 746f 6b65 6e73 223a 202d 310a 2020  l_tokens": -1.  
-00001f10: 7d0a 7d0a 6060 600a 0a53 6565 205b 6578  }.}.```..See [ex
-00001f20: 616d 706c 6573 5d28 6578 616d 706c 6573  amples](examples
-00001f30: 2920 666f 7220 6d6f 7265 2065 7861 6d70  ) for more examp
-00001f40: 6c65 732e 0a0a 0a23 2320 4275 696c 7469  les....## Builti
-00001f50: 6e20 6d6f 6465 6c73 0a54 6f20 7669 6577  n models.To view
-00001f60: 2074 6865 2062 7569 6c74 696e 206d 6f64   the builtin mod
-00001f70: 656c 732c 2072 756e 2074 6865 2066 6f6c  els, run the fol
-00001f80: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
-00001f90: 6060 6062 6173 680a 2420 7869 6e66 6572  ```bash.$ xinfer
-00001fa0: 656e 6365 206c 6973 7420 2d2d 616c 6c0a  ence list --all.
-00001fb0: 6060 600a 0a7c 204e 616d 6520 2020 2020  ```..| Name     
-00001fc0: 2020 2020 2020 2020 2020 2020 7c20 5479              | Ty
-00001fd0: 7065 2020 2020 2020 2020 2020 2020 207c  pe             |
-00001fe0: 204c 616e 6775 6167 6520 7c20 466f 726d   Language | Form
-00001ff0: 6174 207c 2053 697a 6520 2869 6e20 6269  at | Size (in bi
-00002000: 6c6c 696f 6e73 2920 7c20 5175 616e 7469  llions) | Quanti
-00002010: 7a61 7469 6f6e 2020 2020 2020 2020 2020  zation          
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 207c 0a7c 202d 2d2d 2d2d 2d2d 2d2d 2d2d   |.| -----------
-00002040: 2d2d 2d2d 2d2d 2d2d 2d20 7c2d 2d2d 2d2d  --------- |-----
-00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
-00002060: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-00002070: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
-00002080: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00002090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000020a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-000020b0: 0a7c 2062 6169 6368 7561 6e20 2020 2020  .| baichuan     
-000020c0: 2020 2020 2020 2020 7c20 466f 756e 6461          | Founda
-000020d0: 7469 6f6e 204d 6f64 656c 207c 2065 6e2c  tion Model | en,
-000020e0: 207a 6820 2020 7c20 6767 6d6c 7633 207c   zh   | ggmlv3 |
-000020f0: 2037 2020 2020 2020 2020 2020 2020 2020   7              
-00002100: 2020 2020 7c20 2771 325f 4b27 2c20 2771      | 'q2_K', 'q
-00002110: 335f 4b5f 4c27 2c20 2e2e 2e20 2c20 2771  3_K_L', ... , 'q
-00002120: 365f 4b27 2c20 2771 385f 3027 207c 0a7c  6_K', 'q8_0' |.|
-00002130: 2063 6861 7467 6c6d 2020 2020 2020 2020   chatglm        
-00002140: 2020 2020 2020 7c20 5346 5420 4d6f 6465        | SFT Mode
-00002150: 6c20 2020 2020 2020 207c 2065 6e2c 207a  l        | en, z
-00002160: 6820 2020 7c20 6767 6d6c 7633 207c 2036  h   | ggmlv3 | 6
-00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2020 7c20 2771 345f 3027 2c20 2771 345f    | 'q4_0', 'q4_
-00002190: 3127 2c20 2771 355f 3027 2c20 2771 355f  1', 'q5_0', 'q5_
-000021a0: 3127 2c20 2771 385f 3027 207c 0a7c 2063  1', 'q8_0' |.| c
-000021b0: 6861 7467 6c6d 3220 2020 2020 2020 2020  hatglm2         
-000021c0: 2020 2020 7c20 5346 5420 4d6f 6465 6c20      | SFT Model 
-000021d0: 2020 2020 2020 207c 2065 6e2c 207a 6820         | en, zh 
-000021e0: 2020 7c20 6767 6d6c 7633 207c 2036 2020    | ggmlv3 | 6  
-000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 7c20 2771 345f 3027 2c20 2771 345f 3127  | 'q4_0', 'q4_1'
-00002210: 2c20 2771 355f 3027 2c20 2771 355f 3127  , 'q5_0', 'q5_1'
-00002220: 2c20 2771 385f 3027 207c 0a7c 2077 697a  , 'q8_0' |.| wiz
-00002230: 6172 646c 6d2d 7631 2e30 2020 2020 2020  ardlm-v1.0      
-00002240: 2020 7c20 5346 5420 4d6f 6465 6c20 2020    | SFT Model   
-00002250: 2020 2020 207c 2065 6e20 2020 2020 2020       | en       
-00002260: 7c20 6767 6d6c 7633 207c 2037 2c20 3133  | ggmlv3 | 7, 13
-00002270: 2c20 3333 2020 2020 2020 2020 2020 7c20  , 33          | 
-00002280: 2771 325f 4b27 2c20 2771 335f 4b5f 4c27  'q2_K', 'q3_K_L'
-00002290: 2c20 2e2e 2e20 2c20 2771 365f 4b27 2c20  , ... , 'q6_K', 
-000022a0: 2771 385f 3027 207c 0a7c 2076 6963 756e  'q8_0' |.| vicun
-000022b0: 612d 7631 2e33 2020 2020 2020 2020 2020  a-v1.3          
-000022c0: 7c20 5346 5420 4d6f 6465 6c20 2020 2020  | SFT Model     
-000022d0: 2020 207c 2065 6e20 2020 2020 2020 7c20     | en       | 
-000022e0: 6767 6d6c 7633 207c 2037 2c20 3133 2020  ggmlv3 | 7, 13  
-000022f0: 2020 2020 2020 2020 2020 2020 7c20 2771              | 'q
-00002300: 325f 4b27 2c20 2771 335f 4b5f 4c27 2c20  2_K', 'q3_K_L', 
-00002310: 2e2e 2e20 2c20 2771 365f 4b27 2c20 2771  ... , 'q6_K', 'q
-00002320: 385f 3027 207c 0a7c 206f 7263 6120 2020  8_0' |.| orca   
-00002330: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00002340: 5346 5420 4d6f 6465 6c20 2020 2020 2020  SFT Model       
-00002350: 207c 2065 6e20 2020 2020 2020 7c20 6767   | en       | gg
-00002360: 6d6c 7633 207c 2033 2c20 372c 2031 3320  mlv3 | 3, 7, 13 
-00002370: 2020 2020 2020 2020 2020 7c20 2771 345f            | 'q4_
-00002380: 3027 2c20 2771 345f 3127 2c20 2771 355f  0', 'q4_1', 'q5_
-00002390: 3027 2c20 2771 355f 3127 2c20 2771 385f  0', 'q5_1', 'q8_
-000023a0: 3027 207c 0a0a 0a2a 2a4e 4f54 452a 2a3a  0' |...**NOTE**:
-000023b0: 0a2d 2058 696e 6665 7265 6e63 6520 7769  .- Xinference wi
-000023c0: 6c6c 2064 6f77 6e6c 6f61 6420 6d6f 6465  ll download mode
-000023d0: 6c73 2061 7574 6f6d 6174 6963 616c 6c79  ls automatically
-000023e0: 2066 6f72 2079 6f75 2c20 616e 6420 6279   for you, and by
-000023f0: 2064 6566 6175 6c74 2074 6865 206d 6f64   default the mod
-00002400: 656c 7320 7769 6c6c 2062 6520 7361 7665  els will be save
-00002410: 6420 756e 6465 7220 6024 7b55 5345 527d  d under `${USER}
-00002420: 2f2e 7869 6e66 6572 656e 6365 2f63 6163  /.xinference/cac
-00002430: 6865 602e 0a2d 2046 6f75 6e64 6174 696f  he`..- Foundatio
-00002440: 6e20 6d6f 6465 6c73 206f 6e6c 7920 7072  n models only pr
-00002450: 6f76 6964 6520 696e 7465 7266 6163 6520  ovide interface 
-00002460: 6067 656e 6572 6174 6560 2e0a 2d20 5346  `generate`..- SF
-00002470: 5420 6d6f 6465 6c73 2070 726f 7669 6465  T models provide
-00002480: 2062 6f74 6820 6067 656e 6572 6174 6560   both `generate`
-00002490: 2061 6e64 2060 6368 6174 602e 0a0a 2323   and `chat`...##
-000024a0: 2052 6f61 646d 6170 0a58 696e 6665 7265   Roadmap.Xinfere
-000024b0: 6e63 6520 6973 2063 7572 7265 6e74 6c79  nce is currently
-000024c0: 2075 6e64 6572 2061 6374 6976 6520 6465   under active de
-000024d0: 7665 6c6f 706d 656e 742e 2048 6572 6527  velopment. Here'
-000024e0: 7320 6120 726f 6164 6d61 7020 6f75 746c  s a roadmap outl
-000024f0: 696e 696e 6720 6f75 7220 706c 616e 6e65  ining our planne
-00002500: 6420 0a64 6576 656c 6f70 6d65 6e74 7320  d .developments 
-00002510: 666f 7220 7468 6520 6e65 7874 2066 6577  for the next few
-00002520: 2077 6565 6b73 3a0a 0a23 2323 2050 7954   weeks:..### PyT
-00002530: 6f72 6368 2053 7570 706f 7274 0a57 6974  orch Support.Wit
-00002540: 6820 5079 546f 7263 6820 696e 7465 6772  h PyTorch integr
-00002550: 6174 696f 6e2c 2075 7365 7273 2077 696c  ation, users wil
-00002560: 6c20 6265 2061 626c 6520 746f 2073 6561  l be able to sea
-00002570: 6d6c 6573 736c 7920 7574 696c 697a 6520  mlessly utilize 
-00002580: 5079 546f 7263 6820 6d6f 6465 6c73 2066  PyTorch models f
-00002590: 726f 6d20 4875 6767 696e 6720 4661 6365  rom Hugging Face
-000025a0: 0a77 6974 6869 6e20 5869 6e66 6572 656e  .within Xinferen
-000025b0: 6365 2e0a 0a23 2323 204c 616e 6763 6861  ce...### Langcha
-000025c0: 696e 2026 204c 6c61 6d61 496e 6465 7820  in & LlamaIndex 
-000025d0: 696e 7465 6772 6174 696f 6e0a 5769 7468  integration.With
-000025e0: 2058 696e 6665 7265 6e63 652c 2069 7420   Xinference, it 
-000025f0: 7769 6c6c 2062 6520 6d75 6368 2065 6173  will be much eas
-00002600: 6965 7220 666f 7220 7573 6572 7320 746f  ier for users to
-00002610: 2075 7365 2074 6865 7365 206c 6962 7261   use these libra
-00002620: 7269 6573 2061 6e64 2062 7569 6c64 2061  ries and build a
-00002630: 7070 6c69 6361 7469 6f6e 7320 0a77 6974  pplications .wit
-00002640: 6820 4c4c 4d73 2e0a                      h LLMs..
+000009f0: 6769 6629 0a0a 3c64 6976 2061 6c69 676e  gif)..<div align
+00000a00: 3d22 6365 6e74 6572 223e 0a3c 693e 3c61  ="center">.<i><a
+00000a10: 2068 7265 663d 2268 7474 7073 3a2f 2f6a   href="https://j
+00000a20: 6f69 6e2e 736c 6163 6b2e 636f 6d2f 742f  oin.slack.com/t/
+00000a30: 786f 7262 6974 7369 6f2f 7368 6172 6564  xorbitsio/shared
+00000a40: 5f69 6e76 6974 652f 7a74 2d31 7a33 7a73  _invite/zt-1z3zs
+00000a50: 6d39 6570 2d38 3779 4939 595a 5f42 3739  m9ep-87yI9YZ_B79
+00000a60: 484c 4232 6363 5471 3457 4122 3ef0 9f91  HLB2ccTq4WA">...
+00000a70: 8920 4a6f 696e 206f 7572 2053 6c61 636b  . Join our Slack
+00000a80: 2063 6f6d 6d75 6e69 7479 213c 2f61 3e3c   community!</a><
+00000a90: 2f69 3e0a 3c2f 6469 763e 0a0a 2323 204b  /i>.</div>..## K
+00000aa0: 6579 2046 6561 7475 7265 730a f09f 8c9f  ey Features.....
+00000ab0: 202a 2a4d 6f64 656c 2053 6572 7669 6e67   **Model Serving
+00000ac0: 204d 6164 6520 4561 7379 2a2a 3a20 496e   Made Easy**: In
+00000ad0: 6665 7265 6e63 6520 7369 6d70 6c69 6669  ference simplifi
+00000ae0: 6573 2074 6865 2070 726f 6365 7373 206f  es the process o
+00000af0: 6620 7365 7276 696e 6720 6c61 7267 6520  f serving large 
+00000b00: 6c61 6e67 7561 6765 2c20 7370 6565 6368  language, speech
+00000b10: 200a 7265 636f 676e 6974 696f 6e2c 2061   .recognition, a
+00000b20: 6e64 206d 756c 7469 6d6f 6461 6c20 6d6f  nd multimodal mo
+00000b30: 6465 6c73 2e20 596f 7520 6361 6e20 7365  dels. You can se
+00000b40: 7420 7570 2061 6e64 2064 6570 6c6f 7920  t up and deploy 
+00000b50: 796f 7572 206d 6f64 656c 730a 666f 7220  your models.for 
+00000b60: 6578 7065 7269 6d65 6e74 6174 696f 6e20  experimentation 
+00000b70: 616e 6420 7072 6f64 7563 7469 6f6e 2077  and production w
+00000b80: 6974 6820 6120 7369 6e67 6c65 2063 6f6d  ith a single com
+00000b90: 6d61 6e64 2e0a 0ae2 9aa1 efb8 8f20 2a2a  mand......... **
+00000ba0: 5374 6174 652d 6f66 2d74 6865 2d41 7274  State-of-the-Art
+00000bb0: 204d 6f64 656c 732a 2a3a 2045 7870 6572   Models**: Exper
+00000bc0: 696d 656e 7420 7769 7468 2063 7574 7469  iment with cutti
+00000bd0: 6e67 2d65 6467 6520 6275 696c 742d 696e  ng-edge built-in
+00000be0: 206d 6f64 656c 7320 7573 696e 6720 6120   models using a 
+00000bf0: 7369 6e67 6c65 200a 636f 6d6d 616e 642e  single .command.
+00000c00: 2049 6e66 6572 656e 6365 2070 726f 7669   Inference provi
+00000c10: 6465 7320 6163 6365 7373 2074 6f20 7374  des access to st
+00000c20: 6174 652d 6f66 2d74 6865 2d61 7274 206f  ate-of-the-art o
+00000c30: 7065 6e2d 736f 7572 6365 206d 6f64 656c  pen-source model
+00000c40: 7321 0a0a f09f 96a5 202a 2a48 6574 6572  s!...... **Heter
+00000c50: 6f67 656e 656f 7573 2048 6172 6477 6172  ogeneous Hardwar
+00000c60: 6520 5574 696c 697a 6174 696f 6e2a 2a3a  e Utilization**:
+00000c70: 204d 616b 6520 7468 6520 6d6f 7374 206f   Make the most o
+00000c80: 6620 796f 7572 2068 6172 6477 6172 6520  f your hardware 
+00000c90: 7265 736f 7572 6365 732e 2058 6f72 6269  resources. Xorbi
+00000ca0: 7473 200a 496e 6665 7265 6e63 6520 696e  ts .Inference in
+00000cb0: 7465 6c6c 6967 656e 746c 7920 7574 696c  telligently util
+00000cc0: 697a 6573 2068 6574 6572 6f67 656e 656f  izes heterogeneo
+00000cd0: 7573 2068 6172 6477 6172 652c 2069 6e63  us hardware, inc
+00000ce0: 6c75 6469 6e67 2047 5055 7320 616e 6420  luding GPUs and 
+00000cf0: 4350 5573 2c20 746f 206d 6178 696d 697a  CPUs, to maximiz
+00000d00: 650a 7065 7266 6f72 6d61 6e63 6520 616e  e.performance an
+00000d10: 6420 6163 6365 6c65 7261 7465 2079 6f75  d accelerate you
+00000d20: 7220 6d6f 6465 6c20 696e 6665 7265 6e63  r model inferenc
+00000d30: 6520 7461 736b 732e 0a0a e29a 99ef b88f  e tasks.........
+00000d40: 202a 2a46 6c65 7869 626c 6520 4150 4920   **Flexible API 
+00000d50: 616e 6420 496e 7465 7266 6163 6573 2a2a  and Interfaces**
+00000d60: 3a20 586f 7262 6974 7320 496e 6665 7265  : Xorbits Infere
+00000d70: 6e63 6520 6f66 6665 7273 206d 756c 7469  nce offers multi
+00000d80: 706c 6520 696e 7465 7266 6163 6573 2066  ple interfaces f
+00000d90: 6f72 2069 6e74 6572 6163 7469 6e67 0a77  or interacting.w
+00000da0: 6974 6820 796f 7572 206d 6f64 656c 732e  ith your models.
+00000db0: 2059 6f75 2063 616e 2075 7469 6c69 7a65   You can utilize
+00000dc0: 2074 6865 2052 5043 2061 6e64 2052 4553   the RPC and RES
+00000dd0: 5466 756c 2041 5049 2863 6f6d 7061 7469  Tful API(compati
+00000de0: 626c 6520 7769 7468 204f 7065 6e41 4920  ble with OpenAI 
+00000df0: 4150 4929 2074 6f20 696e 7465 6772 6174  API) to integrat
+00000e00: 650a 796f 7572 206d 6f64 656c 7320 7769  e.your models wi
+00000e10: 7468 2065 7869 7374 696e 6720 7379 7374  th existing syst
+00000e20: 656d 7320 6f72 2075 7365 2074 6865 2063  ems or use the c
+00000e30: 6f6d 6d61 6e64 2d6c 696e 6520 696e 7465  ommand-line inte
+00000e40: 7266 6163 6520 2843 4c49 2920 616e 6420  rface (CLI) and 
+00000e50: 7468 6520 696e 7475 6974 6976 6520 5765  the intuitive We
+00000e60: 6255 490a 666f 7220 7365 616d 6c65 7373  bUI.for seamless
+00000e70: 206d 616e 6167 656d 656e 7420 616e 6420   management and 
+00000e80: 6d6f 6e69 746f 7269 6e67 2e0a 0af0 9f8c  monitoring......
+00000e90: 9020 2a2a 4469 7374 7269 6275 7465 6420  . **Distributed 
+00000ea0: 4465 706c 6f79 6d65 6e74 2a2a 3a20 586f  Deployment**: Xo
+00000eb0: 7262 6974 7320 496e 6665 7265 6e63 6520  rbits Inference 
+00000ec0: 6578 6365 6c73 2069 6e20 6469 7374 7269  excels in distri
+00000ed0: 6275 7465 6420 6465 706c 6f79 6d65 6e74  buted deployment
+00000ee0: 2073 6365 6e61 7269 6f73 2c20 0a61 6c6c   scenarios, .all
+00000ef0: 6f77 696e 6720 7468 6520 7365 616d 6c65  owing the seamle
+00000f00: 7373 2064 6973 7472 6962 7574 696f 6e20  ss distribution 
+00000f10: 6f66 206d 6f64 656c 2069 6e66 6572 656e  of model inferen
+00000f20: 6365 2061 6372 6f73 7320 6d75 6c74 6970  ce across multip
+00000f30: 6c65 2064 6576 6963 6573 206f 7220 6d61  le devices or ma
+00000f40: 6368 696e 6573 2e20 4974 0a6c 6576 6572  chines. It.lever
+00000f50: 6167 6573 2064 6973 7472 6962 7574 6564  ages distributed
+00000f60: 2063 6f6d 7075 7469 6e67 2074 6563 686e   computing techn
+00000f70: 6971 7565 7320 746f 2070 6172 616c 6c65  iques to paralle
+00000f80: 6c69 7a65 2061 6e64 2073 6361 6c65 2074  lize and scale t
+00000f90: 6865 2069 6e66 6572 656e 6365 2070 726f  he inference pro
+00000fa0: 6365 7373 2e0a 0af0 9f94 8c20 2a2a 4275  cess....... **Bu
+00000fb0: 696c 742d 696e 2049 6e74 6567 7261 7469  ilt-in Integrati
+00000fc0: 6f6e 2077 6974 6820 5468 6972 642d 5061  on with Third-Pa
+00000fd0: 7274 7920 4c69 6272 6172 6965 732a 2a3a  rty Libraries**:
+00000fe0: 2058 6f72 6269 7473 2049 6e66 6572 656e   Xorbits Inferen
+00000ff0: 6365 2073 6561 6d6c 6573 736c 7920 696e  ce seamlessly in
+00001000: 7465 6772 6174 6573 0a77 6974 6820 706f  tegrates.with po
+00001010: 7075 6c61 7220 7468 6972 642d 7061 7274  pular third-part
+00001020: 7920 6c69 6272 6172 6965 7320 6c69 6b65  y libraries like
+00001030: 204c 616e 6743 6861 696e 2061 6e64 204c   LangChain and L
+00001040: 6c61 6d61 496e 6465 782e 2028 436f 6d69  lamaIndex. (Comi
+00001050: 6e67 2073 6f6f 6e29 0a0a 2323 2047 6574  ng soon)..## Get
+00001060: 7469 6e67 2053 7461 7274 6564 0a58 696e  ting Started.Xin
+00001070: 6665 7265 6e63 6520 6361 6e20 6265 2069  ference can be i
+00001080: 6e73 7461 6c6c 6564 2076 6961 2070 6970  nstalled via pip
+00001090: 2066 726f 6d20 5079 5049 2e20 4974 2069   from PyPI. It i
+000010a0: 7320 6869 6768 6c79 2072 6563 6f6d 6d65  s highly recomme
+000010b0: 6e64 6564 2074 6f20 6372 6561 7465 2061  nded to create a
+000010c0: 206e 6577 2076 6972 7475 616c 0a65 6e76   new virtual.env
+000010d0: 6972 6f6e 6d65 6e74 2074 6f20 6176 6f69  ironment to avoi
+000010e0: 6420 636f 6e66 6c69 6374 732e 0a60 6060  d conflicts..```
+000010f0: 6261 7368 0a24 2070 6970 2069 6e73 7461  bash.$ pip insta
+00001100: 6c6c 2022 7869 6e66 6572 656e 6365 5b61  ll "xinference[a
+00001110: 6c6c 5d22 0a60 6060 0a22 7869 6e66 6572  ll]".```."xinfer
+00001120: 656e 6365 5b61 6c6c 5d22 2069 6e73 7461  ence[all]" insta
+00001130: 6c6c 7320 616c 6c20 7468 6520 6e65 6365  lls all the nece
+00001140: 7373 6172 7920 7061 636b 6167 6573 2066  ssary packages f
+00001150: 6f72 2073 6572 7669 6e67 206d 6f64 656c  or serving model
+00001160: 732e 2049 6620 796f 7520 7761 6e74 2074  s. If you want t
+00001170: 6f20 6163 6869 6576 6520 6163 6365 6c65  o achieve accele
+00001180: 7261 7469 6f6e 206f 6e20 0a64 6966 6665  ration on .diffe
+00001190: 7265 6e74 2068 6172 6477 6172 652c 2072  rent hardware, r
+000011a0: 6566 6572 2074 6f20 7468 6520 696e 7374  efer to the inst
+000011b0: 616c 6c61 7469 6f6e 2064 6f63 756d 656e  allation documen
+000011c0: 7461 7469 6f6e 206f 6620 7468 6520 636f  tation of the co
+000011d0: 7272 6573 706f 6e64 696e 6720 7061 636b  rresponding pack
+000011e0: 6167 652e 0a2d 205b 6c6c 616d 612d 6370  age..- [llama-cp
+000011f0: 702d 7079 7468 6f6e 5d28 6874 7470 733a  p-python](https:
+00001200: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6265  //github.com/abe
+00001210: 746c 656e 2f6c 6c61 6d61 2d63 7070 2d70  tlen/llama-cpp-p
+00001220: 7974 686f 6e23 696e 7374 616c 6c61 7469  ython#installati
+00001230: 6f6e 2d66 726f 6d2d 7079 7069 2d72 6563  on-from-pypi-rec
+00001240: 6f6d 6d65 6e64 6564 2920 6973 2072 6571  ommended) is req
+00001250: 7569 7265 6420 746f 2072 756e 2060 6261  uired to run `ba
+00001260: 6963 6875 616e 602c 2060 7769 7a61 7264  ichuan`, `wizard
+00001270: 6c6d 2d76 312e 3060 2c20 6076 6963 756e  lm-v1.0`, `vicun
+00001280: 612d 7631 2e33 6020 616e 6420 606f 7263  a-v1.3` and `orc
+00001290: 6160 2e0a 2d20 5b63 6861 7467 6c6d 2d63  a`..- [chatglm-c
+000012a0: 7070 2d70 7974 686f 6e5d 2868 7474 7073  pp-python](https
+000012b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6c69  ://github.com/li
+000012c0: 2d70 6c75 732f 6368 6174 676c 6d2e 6370  -plus/chatglm.cp
+000012d0: 7023 6765 7474 696e 672d 7374 6172 7465  p#getting-starte
+000012e0: 6429 2069 7320 7265 7175 6972 6564 2074  d) is required t
+000012f0: 6f20 7275 6e20 6063 6861 7467 6c6d 6020  o run `chatglm` 
+00001300: 616e 6420 6063 6861 7467 6c6d 3260 2e0a  and `chatglm2`..
+00001310: 0a0a 2323 2320 4465 706c 6f79 6d65 6e74  ..### Deployment
+00001320: 0a59 6f75 2063 616e 2064 6570 6c6f 7920  .You can deploy 
+00001330: 5869 6e66 6572 656e 6365 206c 6f63 616c  Xinference local
+00001340: 6c79 2077 6974 6820 6120 7369 6e67 6c65  ly with a single
+00001350: 2063 6f6d 6d61 6e64 206f 7220 6465 706c   command or depl
+00001360: 6f79 2069 7420 696e 2061 2064 6973 7472  oy it in a distr
+00001370: 6962 7574 6564 2063 6c75 7374 6572 2e20  ibuted cluster. 
+00001380: 0a0a 2323 2323 204c 6f63 616c 0a54 6f20  ..#### Local.To 
+00001390: 7374 6172 7420 6120 6c6f 6361 6c20 696e  start a local in
+000013a0: 7374 616e 6365 206f 6620 5869 6e66 6572  stance of Xinfer
+000013b0: 656e 6365 2c20 7275 6e20 7468 6520 666f  ence, run the fo
+000013c0: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
+000013d0: 0a60 6060 6261 7368 0a24 2078 696e 6665  .```bash.$ xinfe
+000013e0: 7265 6e63 650a 6060 600a 0a23 2323 2320  rence.```..#### 
+000013f0: 4469 7374 7269 6275 7465 640a 0a54 6f20  Distributed..To 
+00001400: 6465 706c 6f79 2058 696e 6665 7265 6e63  deploy Xinferenc
+00001410: 6520 696e 2061 2063 6c75 7374 6572 2c20  e in a cluster, 
+00001420: 796f 7520 6e65 6564 2074 6f20 7374 6172  you need to star
+00001430: 7420 6120 5869 6e66 6572 656e 6365 2073  t a Xinference s
+00001440: 7570 6572 7669 736f 7220 6f6e 206f 6e65  upervisor on one
+00001450: 2073 6572 7665 7220 616e 6420 0a58 696e   server and .Xin
+00001460: 6665 7265 6e63 6520 776f 726b 6572 7320  ference workers 
+00001470: 6f6e 2074 6865 206f 7468 6572 2073 6572  on the other ser
+00001480: 7665 7273 2e20 466f 6c6c 6f77 2074 6865  vers. Follow the
+00001490: 2073 7465 7073 2062 656c 6f77 3a0a 0a2a   steps below:..*
+000014a0: 2a53 7461 7274 696e 6720 7468 6520 5375  *Starting the Su
+000014b0: 7065 7276 6973 6f72 2a2a 3a20 4f6e 2074  pervisor**: On t
+000014c0: 6865 2073 6572 7665 7220 7768 6572 6520  he server where 
+000014d0: 796f 7520 7761 6e74 2074 6f20 7275 6e20  you want to run 
+000014e0: 7468 6520 5869 6e66 6572 656e 6365 2073  the Xinference s
+000014f0: 7570 6572 7669 736f 722c 2072 756e 2074  upervisor, run t
+00001500: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00001510: 6d61 6e64 3a0a 6060 6062 6173 680a 2420  mand:.```bash.$ 
+00001520: 7869 6e66 6572 656e 6365 2d73 7570 6572  xinference-super
+00001530: 7669 736f 7220 2d48 2022 247b 7375 7065  visor -H "${supe
+00001540: 7276 6973 6f72 5f68 6f73 747d 220a 6060  rvisor_host}".``
+00001550: 600a 5265 706c 6163 6520 6024 7b73 7570  `.Replace `${sup
+00001560: 6572 7669 736f 725f 686f 7374 7d60 2077  ervisor_host}` w
+00001570: 6974 6820 7468 6520 6163 7475 616c 2068  ith the actual h
+00001580: 6f73 7420 6f66 2079 6f75 7220 7375 7065  ost of your supe
+00001590: 7276 6973 6f72 2073 6572 7665 722e 0a0a  rvisor server...
+000015a0: 2a2a 5374 6172 7469 6e67 2074 6865 2057  **Starting the W
+000015b0: 6f72 6b65 7273 2a2a 3a20 4f6e 2065 6163  orkers**: On eac
+000015c0: 6820 6f66 2074 6865 206f 7468 6572 2073  h of the other s
+000015d0: 6572 7665 7273 2077 6865 7265 2079 6f75  ervers where you
+000015e0: 2077 616e 7420 746f 2072 756e 2058 696e   want to run Xin
+000015f0: 6665 7265 6e63 6520 776f 726b 6572 732c  ference workers,
+00001600: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
+00001610: 6e67 2063 6f6d 6d61 6e64 3a0a 6060 6062  ng command:.```b
+00001620: 6173 680a 2420 7869 6e66 6572 656e 6365  ash.$ xinference
+00001630: 2d77 6f72 6b65 7220 2d65 2022 6874 7470  -worker -e "http
+00001640: 3a2f 2f24 7b73 7570 6572 7669 736f 725f  ://${supervisor_
+00001650: 686f 7374 7d3a 3939 3937 220a 6060 600a  host}:9997".```.
+00001660: 0a4f 6e63 6520 5869 6e66 6572 656e 6365  .Once Xinference
+00001670: 2069 7320 7275 6e6e 696e 672c 2061 6e20   is running, an 
+00001680: 656e 6470 6f69 6e74 2077 696c 6c20 6265  endpoint will be
+00001690: 2061 6363 6573 7369 626c 6520 666f 7220   accessible for 
+000016a0: 6d6f 6465 6c20 6d61 6e61 6765 6d65 6e74  model management
+000016b0: 2076 6961 2043 4c49 206f 720a 5869 6e66   via CLI or.Xinf
+000016c0: 6572 656e 6365 2020 636c 6965 6e74 2e0a  erence  client..
+000016d0: 0a2d 2046 6f72 206c 6f63 616c 2064 6570  .- For local dep
+000016e0: 6c6f 796d 656e 742c 2074 6865 2065 6e64  loyment, the end
+000016f0: 706f 696e 7420 7769 6c6c 2062 6520 6068  point will be `h
+00001700: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+00001710: 3939 3937 602e 0a2d 2046 6f72 2063 6c75  9997`..- For clu
+00001720: 7374 6572 2064 6570 6c6f 796d 656e 742c  ster deployment,
+00001730: 2074 6865 2065 6e64 706f 696e 7420 7769   the endpoint wi
+00001740: 6c6c 2062 6520 6068 7474 703a 2f2f 247b  ll be `http://${
+00001750: 7375 7065 7276 6973 6f72 5f68 6f73 747d  supervisor_host}
+00001760: 3a39 3939 3760 2c20 7768 6572 650a 6024  :9997`, where.`$
+00001770: 7b73 7570 6572 7669 736f 725f 686f 7374  {supervisor_host
+00001780: 7d60 2069 7320 7468 6520 686f 7374 6e61  }` is the hostna
+00001790: 6d65 206f 7220 4950 2061 6464 7265 7373  me or IP address
+000017a0: 206f 6620 7468 6520 7365 7276 6572 2077   of the server w
+000017b0: 6865 7265 2074 6865 2073 7570 6572 7669  here the supervi
+000017c0: 736f 7220 6973 2072 756e 6e69 6e67 2e0a  sor is running..
+000017d0: 0a59 6f75 2063 616e 2061 6c73 6f20 7669  .You can also vi
+000017e0: 6577 2061 2077 6562 2055 4920 7573 696e  ew a web UI usin
+000017f0: 6720 7468 6520 5869 6e66 6572 656e 6365  g the Xinference
+00001800: 2065 6e64 706f 696e 7420 746f 2063 6861   endpoint to cha
+00001810: 7420 7769 7468 2061 6c6c 2074 6865 200a  t with all the .
+00001820: 6275 696c 7469 6e20 6d6f 6465 6c73 2e20  builtin models. 
+00001830: 596f 7520 6361 6e20 6576 656e 202a 2a63  You can even **c
+00001840: 6861 7420 7769 7468 2074 776f 2063 7574  hat with two cut
+00001850: 7469 6e67 2d65 6467 6520 4149 206d 6f64  ting-edge AI mod
+00001860: 656c 7320 7369 6465 2d62 792d 7369 6465  els side-by-side
+00001870: 2074 6f20 636f 6d70 6172 650a 7468 6569   to compare.thei
+00001880: 7220 7065 7266 6f72 6d61 6e63 652a 2a21  r performance**!
+00001890: 0a0a 215b 7765 6220 5549 5d28 6173 7365  ..![web UI](asse
+000018a0: 7473 2f78 696e 6665 7265 6e63 652d 646f  ts/xinference-do
+000018b0: 776e 6c6f 6164 696e 672e 706e 6729 0a0a  wnloading.png)..
+000018c0: 2323 2320 5869 6e66 6572 656e 6365 2043  ### Xinference C
+000018d0: 4c49 0a58 696e 6665 7265 6e63 6520 7072  LI.Xinference pr
+000018e0: 6f76 6964 6573 2061 2063 6f6d 6d61 6e64  ovides a command
+000018f0: 206c 696e 6520 696e 7465 7266 6163 6520   line interface 
+00001900: 2843 4c49 2920 666f 7220 6d6f 6465 6c20  (CLI) for model 
+00001910: 6d61 6e61 6765 6d65 6e74 2e20 4865 7265  management. Here
+00001920: 2061 7265 2073 6f6d 6520 7573 6566 756c   are some useful
+00001930: 200a 636f 6d6d 616e 6473 3a0a 0a2d 204c   .commands:..- L
+00001940: 6175 6e63 6820 6120 6d6f 6465 6c20 2861  aunch a model (a
+00001950: 206d 6f64 656c 2055 4944 2077 696c 6c20   model UID will 
+00001960: 6265 2072 6574 7572 6e65 6429 3a20 6078  be returned): `x
+00001970: 696e 6665 7265 6e63 6520 6c61 756e 6368  inference launch
+00001980: 600a 2d20 4c69 7374 2072 756e 6e69 6e67  `.- List running
+00001990: 206d 6f64 656c 733a 2060 7869 6e66 6572   models: `xinfer
+000019a0: 656e 6365 206c 6973 7460 0a2d 204c 6973  ence list`.- Lis
+000019b0: 7420 616c 6c20 7468 6520 6275 696c 7469  t all the builti
+000019c0: 6e20 6d6f 6465 6c73 3a20 6078 696e 6665  n models: `xinfe
+000019d0: 7265 6e63 6520 6c69 7374 202d 2d61 6c6c  rence list --all
+000019e0: 600a 2d20 5465 726d 696e 6174 6520 6120  `.- Terminate a 
+000019f0: 6d6f 6465 6c3a 2060 7869 6e66 6572 656e  model: `xinferen
+00001a00: 6365 2074 6572 6d69 6e61 7465 202d 2d6d  ce terminate --m
+00001a10: 6f64 656c 2d75 6964 2024 7b6d 6f64 656c  odel-uid ${model
+00001a20: 5f75 6964 7d60 0a0a 2323 2320 5869 6e66  _uid}`..### Xinf
+00001a30: 6572 656e 6365 2043 6c69 656e 740a 5869  erence Client.Xi
+00001a40: 6e66 6572 656e 6365 2061 6c73 6f20 7072  nference also pr
+00001a50: 6f76 6964 6573 2061 2063 6c69 656e 7420  ovides a client 
+00001a60: 666f 7220 6d61 6e61 6769 6e67 2061 6e64  for managing and
+00001a70: 2061 6363 6573 7369 6e67 206d 6f64 656c   accessing model
+00001a80: 7320 7072 6f67 7261 6d6d 6174 6963 616c  s programmatical
+00001a90: 6c79 3a0a 0a60 6060 7079 7468 6f6e 0a66  ly:..```python.f
+00001aa0: 726f 6d20 7869 6e66 6572 656e 6365 2e63  rom xinference.c
+00001ab0: 6c69 656e 7420 696d 706f 7274 2043 6c69  lient import Cli
+00001ac0: 656e 740a 0a63 6c69 656e 7420 3d20 436c  ent..client = Cl
+00001ad0: 6965 6e74 2822 6874 7470 3a2f 2f6c 6f63  ient("http://loc
+00001ae0: 616c 686f 7374 3a39 3939 3722 290a 6d6f  alhost:9997").mo
+00001af0: 6465 6c5f 7569 6420 3d20 636c 6965 6e74  del_uid = client
+00001b00: 2e6c 6175 6e63 685f 6d6f 6465 6c28 6d6f  .launch_model(mo
+00001b10: 6465 6c5f 6e61 6d65 3d22 6368 6174 676c  del_name="chatgl
+00001b20: 6d32 2229 0a6d 6f64 656c 203d 2063 6c69  m2").model = cli
+00001b30: 656e 742e 6765 745f 6d6f 6465 6c28 6d6f  ent.get_model(mo
+00001b40: 6465 6c5f 7569 6429 0a0a 6368 6174 5f68  del_uid)..chat_h
+00001b50: 6973 746f 7279 203d 205b 5d0a 7072 6f6d  istory = [].prom
+00001b60: 7074 203d 2022 5768 6174 2069 7320 7468  pt = "What is th
+00001b70: 6520 6c61 7267 6573 7420 616e 696d 616c  e largest animal
+00001b80: 3f22 0a6d 6f64 656c 2e63 6861 7428 0a20  ?".model.chat(. 
+00001b90: 2020 2020 2020 2020 2020 2070 726f 6d70             promp
+00001ba0: 742c 0a20 2020 2020 2020 2020 2020 2063  t,.            c
+00001bb0: 6861 745f 6869 7374 6f72 792c 0a20 2020  hat_history,.   
+00001bc0: 2020 2020 2020 2020 2067 656e 6572 6174           generat
+00001bd0: 655f 636f 6e66 6967 3d7b 226d 6178 5f74  e_config={"max_t
+00001be0: 6f6b 656e 7322 3a20 3130 3234 7d0a 2020  okens": 1024}.  
+00001bf0: 2020 2020 2020 290a 6060 600a 0a52 6573        ).```..Res
+00001c00: 756c 743a 0a60 6060 6a73 6f6e 0a7b 0a20  ult:.```json.{. 
+00001c10: 2022 6964 223a 2022 6368 6174 636d 706c   "id": "chatcmpl
+00001c20: 2d38 6437 3662 3635 612d 6261 6430 2d34  -8d76b65a-bad0-4
+00001c30: 3265 662d 3931 3264 2d34 6130 3533 3364  2ef-912d-4a0533d
+00001c40: 3930 6436 3122 2c0a 2020 226d 6f64 656c  90d61",.  "model
+00001c50: 223a 2022 3536 6636 3936 3232 2d31 6537  ": "56f69622-1e7
+00001c60: 332d 3131 6565 2d61 3362 642d 3961 6639  3-11ee-a3bd-9af9
+00001c70: 6631 3638 3136 6336 222c 0a20 2022 6f62  f16816c6",.  "ob
+00001c80: 6a65 6374 223a 2022 6368 6174 2e63 6f6d  ject": "chat.com
+00001c90: 706c 6574 696f 6e22 2c0a 2020 2263 7265  pletion",.  "cre
+00001ca0: 6174 6564 223a 2031 3638 3839 3139 3138  ated": 168891918
+00001cb0: 372c 0a20 2022 6368 6f69 6365 7322 3a20  7,.  "choices": 
+00001cc0: 5b0a 2020 2020 7b0a 2020 2020 2020 2269  [.    {.      "i
+00001cd0: 6e64 6578 223a 2030 2c0a 2020 2020 2020  ndex": 0,.      
+00001ce0: 226d 6573 7361 6765 223a 207b 0a20 2020  "message": {.   
+00001cf0: 2020 2020 2022 726f 6c65 223a 2022 6173       "role": "as
+00001d00: 7369 7374 616e 7422 2c0a 2020 2020 2020  sistant",.      
+00001d10: 2020 2263 6f6e 7465 6e74 223a 2022 5468    "content": "Th
+00001d20: 6520 6c61 7267 6573 7420 616e 696d 616c  e largest animal
+00001d30: 2074 6861 7420 6861 7320 6265 656e 2073   that has been s
+00001d40: 6369 656e 7469 6669 6361 6c6c 7920 6d65  cientifically me
+00001d50: 6173 7572 6564 2069 7320 7468 6520 626c  asured is the bl
+00001d60: 7565 2077 6861 6c65 2c20 7768 6963 6820  ue whale, which 
+00001d70: 6861 7320 6120 6d61 7869 6d75 6d20 6c65  has a maximum le
+00001d80: 6e67 7468 206f 6620 6172 6f75 6e64 2032  ngth of around 2
+00001d90: 3320 6d65 7465 7273 2028 3735 2066 6565  3 meters (75 fee
+00001da0: 7429 2066 6f72 2061 6475 6c74 2061 6e69  t) for adult ani
+00001db0: 6d61 6c73 2061 6e64 2063 616e 2077 6569  mals and can wei
+00001dc0: 6768 2075 7020 746f 2031 3530 2c30 3030  gh up to 150,000
+00001dd0: 2070 6f75 6e64 7320 2836 382c 3030 3020   pounds (68,000 
+00001de0: 6b67 292e 2048 6f77 6576 6572 2c20 6974  kg). However, it
+00001df0: 2069 7320 696d 706f 7274 616e 7420 746f   is important to
+00001e00: 206e 6f74 6520 7468 6174 2074 6869 7320   note that this 
+00001e10: 6973 206a 7573 7420 616e 2065 7374 696d  is just an estim
+00001e20: 6174 6520 616e 6420 7468 6174 2074 6865  ate and that the
+00001e30: 206c 6172 6765 7374 2061 6e69 6d61 6c20   largest animal 
+00001e40: 6b6e 6f77 6e20 746f 2073 6369 656e 6365  known to science
+00001e50: 206d 6179 2062 6520 6c61 7267 6572 2073   may be larger s
+00001e60: 7469 6c6c 2e20 536f 6d65 2073 6369 656e  till. Some scien
+00001e70: 7469 7374 7320 6265 6c69 6576 6520 7468  tists believe th
+00001e80: 6174 2074 6865 206c 6172 6765 7374 2061  at the largest a
+00001e90: 6e69 6d61 6c73 206d 6179 206e 6f74 2068  nimals may not h
+00001ea0: 6176 6520 6120 636c 6561 7220 5c22 7369  ave a clear \"si
+00001eb0: 7a65 5c22 2069 6e20 7468 6520 7361 6d65  ze\" in the same
+00001ec0: 2077 6179 2074 6861 7420 6875 6d61 6e73   way that humans
+00001ed0: 2064 6f2c 2061 7320 7468 6569 7220 7369   do, as their si
+00001ee0: 7a65 2063 616e 2076 6172 7920 6465 7065  ze can vary depe
+00001ef0: 6e64 696e 6720 6f6e 2074 6865 2065 6e76  nding on the env
+00001f00: 6972 6f6e 6d65 6e74 2061 6e64 2074 6865  ironment and the
+00001f10: 2073 7461 6765 206f 6620 7468 6569 7220   stage of their 
+00001f20: 6c69 6665 2e22 0a20 2020 2020 207d 2c0a  life.".      },.
+00001f30: 2020 2020 2020 2266 696e 6973 685f 7265        "finish_re
+00001f40: 6173 6f6e 223a 2022 4e6f 6e65 220a 2020  ason": "None".  
+00001f50: 2020 7d0a 2020 5d2c 0a20 2022 7573 6167    }.  ],.  "usag
+00001f60: 6522 3a20 7b0a 2020 2020 2270 726f 6d70  e": {.    "promp
+00001f70: 745f 746f 6b65 6e73 223a 202d 312c 0a20  t_tokens": -1,. 
+00001f80: 2020 2022 636f 6d70 6c65 7469 6f6e 5f74     "completion_t
+00001f90: 6f6b 656e 7322 3a20 2d31 2c0a 2020 2020  okens": -1,.    
+00001fa0: 2274 6f74 616c 5f74 6f6b 656e 7322 3a20  "total_tokens": 
+00001fb0: 2d31 0a20 207d 0a7d 0a60 6060 0a0a 5365  -1.  }.}.```..Se
+00001fc0: 6520 5b65 7861 6d70 6c65 735d 2865 7861  e [examples](exa
+00001fd0: 6d70 6c65 7329 2066 6f72 206d 6f72 6520  mples) for more 
+00001fe0: 6578 616d 706c 6573 2e0a 0a0a 2323 2042  examples....## B
+00001ff0: 7569 6c74 696e 206d 6f64 656c 730a 546f  uiltin models.To
+00002000: 2076 6965 7720 7468 6520 6275 696c 7469   view the builti
+00002010: 6e20 6d6f 6465 6c73 2c20 7275 6e20 7468  n models, run th
+00002020: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00002030: 616e 643a 0a60 6060 6261 7368 0a24 2078  and:.```bash.$ x
+00002040: 696e 6665 7265 6e63 6520 6c69 7374 202d  inference list -
+00002050: 2d61 6c6c 0a60 6060 0a0a 7c20 4e61 6d65  -all.```..| Name
+00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002070: 207c 2054 7970 6520 2020 2020 2020 2020   | Type         
+00002080: 2020 2020 7c20 4c61 6e67 7561 6765 207c      | Language |
+00002090: 2046 6f72 6d61 7420 7c20 5369 7a65 2028   Format | Size (
+000020a0: 696e 2062 696c 6c69 6f6e 7329 207c 2051  in billions) | Q
+000020b0: 7561 6e74 697a 6174 696f 6e20 2020 2020  uantization     
+000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020d0: 2020 2020 2020 7c0a 7c20 2d2d 2d2d 2d2d        |.| ------
+000020e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
+000020f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002100: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  --|----------|--
+00002110: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
+00002120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
+00002130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002150: 2d2d 2d2d 7c0a 7c20 6261 6963 6875 616e  ----|.| baichuan
+00002160: 2020 2020 2020 2020 2020 2020 207c 2046               | F
+00002170: 6f75 6e64 6174 696f 6e20 4d6f 6465 6c20  oundation Model 
+00002180: 7c20 656e 2c20 7a68 2020 207c 2067 676d  | en, zh   | ggm
+00002190: 6c76 3320 7c20 3720 2020 2020 2020 2020  lv3 | 7         
+000021a0: 2020 2020 2020 2020 207c 2027 7132 5f4b           | 'q2_K
+000021b0: 272c 2027 7133 5f4b 5f4c 272c 202e 2e2e  ', 'q3_K_L', ...
+000021c0: 202c 2027 7136 5f4b 272c 2027 7138 5f30   , 'q6_K', 'q8_0
+000021d0: 2720 7c0a 7c20 6368 6174 676c 6d20 2020  ' |.| chatglm   
+000021e0: 2020 2020 2020 2020 2020 207c 2053 4654             | SFT
+000021f0: 204d 6f64 656c 2020 2020 2020 2020 7c20   Model        | 
+00002200: 656e 2c20 7a68 2020 207c 2067 676d 6c76  en, zh   | ggmlv
+00002210: 3320 7c20 3620 2020 2020 2020 2020 2020  3 | 6           
+00002220: 2020 2020 2020 207c 2027 7134 5f30 272c         | 'q4_0',
+00002230: 2027 7134 5f31 272c 2027 7135 5f30 272c   'q4_1', 'q5_0',
+00002240: 2027 7135 5f31 272c 2027 7138 5f30 2720   'q5_1', 'q8_0' 
+00002250: 7c0a 7c20 6368 6174 676c 6d32 2020 2020  |.| chatglm2    
+00002260: 2020 2020 2020 2020 207c 2053 4654 204d           | SFT M
+00002270: 6f64 656c 2020 2020 2020 2020 7c20 656e  odel        | en
+00002280: 2c20 7a68 2020 207c 2067 676d 6c76 3320  , zh   | ggmlv3 
+00002290: 7c20 3620 2020 2020 2020 2020 2020 2020  | 6             
+000022a0: 2020 2020 207c 2027 7134 5f30 272c 2027       | 'q4_0', '
+000022b0: 7134 5f31 272c 2027 7135 5f30 272c 2027  q4_1', 'q5_0', '
+000022c0: 7135 5f31 272c 2027 7138 5f30 2720 7c0a  q5_1', 'q8_0' |.
+000022d0: 7c20 7769 7a61 7264 6c6d 2d76 312e 3020  | wizardlm-v1.0 
+000022e0: 2020 2020 2020 207c 2053 4654 204d 6f64         | SFT Mod
+000022f0: 656c 2020 2020 2020 2020 7c20 656e 2020  el        | en  
+00002300: 2020 2020 207c 2067 676d 6c76 3320 7c20       | ggmlv3 | 
+00002310: 372c 2031 332c 2033 3320 2020 2020 2020  7, 13, 33       
+00002320: 2020 207c 2027 7132 5f4b 272c 2027 7133     | 'q2_K', 'q3
+00002330: 5f4b 5f4c 272c 202e 2e2e 202c 2027 7136  _K_L', ... , 'q6
+00002340: 5f4b 272c 2027 7138 5f30 2720 7c0a 7c20  _K', 'q8_0' |.| 
+00002350: 7669 6375 6e61 2d76 312e 3320 2020 2020  vicuna-v1.3     
+00002360: 2020 2020 207c 2053 4654 204d 6f64 656c       | SFT Model
+00002370: 2020 2020 2020 2020 7c20 656e 2020 2020          | en    
+00002380: 2020 207c 2067 676d 6c76 3320 7c20 372c     | ggmlv3 | 7,
+00002390: 2031 3320 2020 2020 2020 2020 2020 2020   13             
+000023a0: 207c 2027 7132 5f4b 272c 2027 7133 5f4b   | 'q2_K', 'q3_K
+000023b0: 5f4c 272c 202e 2e2e 202c 2027 7136 5f4b  _L', ... , 'q6_K
+000023c0: 272c 2027 7138 5f30 2720 7c0a 7c20 6f72  ', 'q8_0' |.| or
+000023d0: 6361 2020 2020 2020 2020 2020 2020 2020  ca              
+000023e0: 2020 207c 2053 4654 204d 6f64 656c 2020     | SFT Model  
+000023f0: 2020 2020 2020 7c20 656e 2020 2020 2020        | en      
+00002400: 207c 2067 676d 6c76 3320 7c20 332c 2037   | ggmlv3 | 3, 7
+00002410: 2c20 3133 2020 2020 2020 2020 2020 207c  , 13           |
+00002420: 2027 7134 5f30 272c 2027 7134 5f31 272c   'q4_0', 'q4_1',
+00002430: 2027 7135 5f30 272c 2027 7135 5f31 272c   'q5_0', 'q5_1',
+00002440: 2027 7138 5f30 2720 7c0a 0a0a 2a2a 4e4f   'q8_0' |...**NO
+00002450: 5445 2a2a 3a0a 2d20 5869 6e66 6572 656e  TE**:.- Xinferen
+00002460: 6365 2077 696c 6c20 646f 776e 6c6f 6164  ce will download
+00002470: 206d 6f64 656c 7320 6175 746f 6d61 7469   models automati
+00002480: 6361 6c6c 7920 666f 7220 796f 752c 2061  cally for you, a
+00002490: 6e64 2062 7920 6465 6661 756c 7420 7468  nd by default th
+000024a0: 6520 6d6f 6465 6c73 2077 696c 6c20 6265  e models will be
+000024b0: 2073 6176 6564 2075 6e64 6572 2060 247b   saved under `${
+000024c0: 5553 4552 7d2f 2e78 696e 6665 7265 6e63  USER}/.xinferenc
+000024d0: 652f 6361 6368 6560 2e0a 2d20 466f 756e  e/cache`..- Foun
+000024e0: 6461 7469 6f6e 206d 6f64 656c 7320 6f6e  dation models on
+000024f0: 6c79 2070 726f 7669 6465 2069 6e74 6572  ly provide inter
+00002500: 6661 6365 2060 6765 6e65 7261 7465 602e  face `generate`.
+00002510: 0a2d 2053 4654 206d 6f64 656c 7320 7072  .- SFT models pr
+00002520: 6f76 6964 6520 626f 7468 2060 6765 6e65  ovide both `gene
+00002530: 7261 7465 6020 616e 6420 6063 6861 7460  rate` and `chat`
+00002540: 2e0a 0a23 2320 526f 6164 6d61 700a 5869  ...## Roadmap.Xi
+00002550: 6e66 6572 656e 6365 2069 7320 6375 7272  nference is curr
+00002560: 656e 746c 7920 756e 6465 7220 6163 7469  ently under acti
+00002570: 7665 2064 6576 656c 6f70 6d65 6e74 2e20  ve development. 
+00002580: 4865 7265 2773 2061 2072 6f61 646d 6170  Here's a roadmap
+00002590: 206f 7574 6c69 6e69 6e67 206f 7572 2070   outlining our p
+000025a0: 6c61 6e6e 6564 200a 6465 7665 6c6f 706d  lanned .developm
+000025b0: 656e 7473 2066 6f72 2074 6865 206e 6578  ents for the nex
+000025c0: 7420 6665 7720 7765 656b 733a 0a0a 2323  t few weeks:..##
+000025d0: 2320 5079 546f 7263 6820 5375 7070 6f72  # PyTorch Suppor
+000025e0: 740a 5769 7468 2050 7954 6f72 6368 2069  t.With PyTorch i
+000025f0: 6e74 6567 7261 7469 6f6e 2c20 7573 6572  ntegration, user
+00002600: 7320 7769 6c6c 2062 6520 6162 6c65 2074  s will be able t
+00002610: 6f20 7365 616d 6c65 7373 6c79 2075 7469  o seamlessly uti
+00002620: 6c69 7a65 2050 7954 6f72 6368 206d 6f64  lize PyTorch mod
+00002630: 656c 7320 6672 6f6d 2048 7567 6769 6e67  els from Hugging
+00002640: 2046 6163 650a 7769 7468 696e 2058 696e   Face.within Xin
+00002650: 6665 7265 6e63 652e 0a0a 2323 2320 4c61  ference...### La
+00002660: 6e67 6368 6169 6e20 2620 4c6c 616d 6149  ngchain & LlamaI
+00002670: 6e64 6578 2069 6e74 6567 7261 7469 6f6e  ndex integration
+00002680: 0a57 6974 6820 5869 6e66 6572 656e 6365  .With Xinference
+00002690: 2c20 6974 2077 696c 6c20 6265 206d 7563  , it will be muc
+000026a0: 6820 6561 7369 6572 2066 6f72 2075 7365  h easier for use
+000026b0: 7273 2074 6f20 7573 6520 7468 6573 6520  rs to use these 
+000026c0: 6c69 6272 6172 6965 7320 616e 6420 6275  libraries and bu
+000026d0: 696c 6420 6170 706c 6963 6174 696f 6e73  ild applications
+000026e0: 200a 7769 7468 204c 4c4d 732e 0a          .with LLMs..
```

### Comparing `xinference-0.0.2/xinference.egg-info/SOURCES.txt` & `xinference-0.0.3/xinference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

