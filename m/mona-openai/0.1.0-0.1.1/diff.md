# Comparing `tmp/mona-openai-0.1.0.tar.gz` & `tmp/mona-openai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mona-openai-0.1.0.tar", last modified: Mon Jul  3 11:49:23 2023, max compression
+gzip compressed data, was "mona-openai-0.1.1.tar", last modified: Tue Jul 11 10:45:16 2023, max compression
```

## Comparing `mona-openai-0.1.0.tar` & `mona-openai-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.913505 mona-openai-0.1.0/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.1.0/LICENSE
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    12386 2023-07-03 11:49:23.913279 mona-openai-0.1.0/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11792 2023-07-03 07:58:39.000000 mona-openai-0.1.0/README.md
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.908400 mona-openai-0.1.0/mona_openai/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      238 2023-07-02 06:46:47.000000 mona-openai-0.1.0/mona_openai/__init__.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.909467 mona-openai-0.1.0/mona_openai/analysis/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/analysis/privacy.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/analysis/profanity.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3100 2023-07-02 06:46:51.000000 mona-openai-0.1.0/mona_openai/analysis/textual.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.910181 mona-openai-0.1.0/mona_openai/endpoints/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     7750 2023-07-02 06:46:51.000000 mona-openai-0.1.0/mona_openai/endpoints/chat_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     5166 2023-07-02 06:46:51.000000 mona-openai-0.1.0/mona_openai/endpoints/completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/endpoints/endpoint_wrapping.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/endpoints/wrapping_getter.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      225 2023-06-28 08:19:06.000000 mona-openai-0.1.0/mona_openai/exceptions.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.911044 mona-openai-0.1.0/mona_openai/loggers/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      202 2023-07-03 07:53:34.000000 mona-openai-0.1.0/mona_openai/loggers/__init__.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      965 2023-07-02 06:46:47.000000 mona-openai-0.1.0/mona_openai/loggers/file_logger.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      772 2023-07-02 15:33:33.000000 mona-openai-0.1.0/mona_openai/loggers/in_memory_logging.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1411 2023-07-02 15:30:54.000000 mona-openai-0.1.0/mona_openai/loggers/logger.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.911454 mona-openai-0.1.0/mona_openai/loggers/mona_logger/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1381 2023-07-02 06:46:47.000000 mona-openai-0.1.0/mona_openai/loggers/mona_logger/mona_client.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1928 2023-07-02 07:57:33.000000 mona-openai-0.1.0/mona_openai/loggers/mona_logger/mona_logger.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1048 2023-07-02 07:46:00.000000 mona-openai-0.1.0/mona_openai/loggers/standard_logging.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    16828 2023-07-02 06:46:47.000000 mona-openai-0.1.0/mona_openai/mona_openai.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.912524 mona-openai-0.1.0/mona_openai/util/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      946 2023-06-01 06:55:43.000000 mona-openai-0.1.0/mona_openai/util/async_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.1.0/mona_openai/util/func_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/util/oop_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/util/openai_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/util/stream_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/util/tokens_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.1.0/mona_openai/util/validation_util.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.909068 mona-openai-0.1.0/mona_openai.egg-info/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    12386 2023-07-03 11:49:23.000000 mona-openai-0.1.0/mona_openai.egg-info/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1170 2023-07-03 11:49:23.000000 mona-openai-0.1.0/mona_openai.egg-info/SOURCES.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-07-03 11:49:23.000000 mona-openai-0.1.0/mona_openai.egg-info/dependency_links.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-07-03 11:49:23.000000 mona-openai-0.1.0/mona_openai.egg-info/requires.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-07-03 11:49:23.000000 mona-openai-0.1.0/mona_openai.egg-info/top_level.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-07-03 11:49:02.000000 mona-openai-0.1.0/pyproject.toml
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.1.0/requirements.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-07-03 11:49:23.913555 mona-openai-0.1.0/setup.cfg
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.913083 mona-openai-0.1.0/tests/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    17356 2023-07-02 06:46:51.000000 mona-openai-0.1.0/tests/test_chat_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    20107 2023-07-02 06:46:51.000000 mona-openai-0.1.0/tests/test_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.1.0/tests/test_privacy_analyzer.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      975 2023-06-29 11:44:26.000000 mona-openai-0.1.0/tests/test_textual_analyzer.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-11 10:45:16.096766 mona-openai-0.1.1/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.1.1/LICENSE
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    12518 2023-07-11 10:45:16.096604 mona-openai-0.1.1/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11923 2023-07-10 12:44:58.000000 mona-openai-0.1.1/README.md
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-11 10:45:16.092836 mona-openai-0.1.1/mona_openai/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      238 2023-07-05 12:34:59.000000 mona-openai-0.1.1/mona_openai/__init__.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-11 10:45:16.093919 mona-openai-0.1.1/mona_openai/analysis/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.1.1/mona_openai/analysis/privacy.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.1.1/mona_openai/analysis/profanity.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3100 2023-07-02 06:46:51.000000 mona-openai-0.1.1/mona_openai/analysis/textual.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-11 10:45:16.094340 mona-openai-0.1.1/mona_openai/endpoints/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     7750 2023-07-02 06:46:51.000000 mona-openai-0.1.1/mona_openai/endpoints/chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     5166 2023-07-02 06:46:51.000000 mona-openai-0.1.1/mona_openai/endpoints/completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.1.1/mona_openai/endpoints/endpoint_wrapping.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.1.1/mona_openai/endpoints/wrapping_getter.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      225 2023-06-28 08:19:06.000000 mona-openai-0.1.1/mona_openai/exceptions.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-11 10:45:16.094905 mona-openai-0.1.1/mona_openai/loggers/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      202 2023-07-05 12:34:59.000000 mona-openai-0.1.1/mona_openai/loggers/__init__.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      965 2023-07-05 12:34:59.000000 mona-openai-0.1.1/mona_openai/loggers/file_logger.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      772 2023-07-05 12:34:59.000000 mona-openai-0.1.1/mona_openai/loggers/in_memory_logging.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1411 2023-07-05 12:34:59.000000 mona-openai-0.1.1/mona_openai/loggers/logger.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-11 10:45:16.095131 mona-openai-0.1.1/mona_openai/loggers/mona_logger/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1381 2023-07-05 12:34:59.000000 mona-openai-0.1.1/mona_openai/loggers/mona_logger/mona_client.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1928 2023-07-05 12:34:59.000000 mona-openai-0.1.1/mona_openai/loggers/mona_logger/mona_logger.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1048 2023-07-05 12:34:59.000000 mona-openai-0.1.1/mona_openai/loggers/standard_logging.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17203 2023-07-11 03:37:09.000000 mona-openai-0.1.1/mona_openai/mona_openai.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-11 10:45:16.095961 mona-openai-0.1.1/mona_openai/util/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1296 2023-07-10 12:46:59.000000 mona-openai-0.1.1/mona_openai/util/async_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.1.1/mona_openai/util/func_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.1.1/mona_openai/util/oop_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.1.1/mona_openai/util/openai_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.1.1/mona_openai/util/stream_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.1.1/mona_openai/util/tokens_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.1.1/mona_openai/util/validation_util.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-11 10:45:16.093542 mona-openai-0.1.1/mona_openai.egg-info/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    12518 2023-07-11 10:45:16.000000 mona-openai-0.1.1/mona_openai.egg-info/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1170 2023-07-11 10:45:16.000000 mona-openai-0.1.1/mona_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-07-11 10:45:16.000000 mona-openai-0.1.1/mona_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      103 2023-07-11 10:45:16.000000 mona-openai-0.1.1/mona_openai.egg-info/requires.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-07-11 10:45:16.000000 mona-openai-0.1.1/mona_openai.egg-info/top_level.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-07-11 10:31:07.000000 mona-openai-0.1.1/pyproject.toml
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      102 2023-07-10 12:27:13.000000 mona-openai-0.1.1/requirements.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-07-11 10:45:16.096809 mona-openai-0.1.1/setup.cfg
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-11 10:45:16.096439 mona-openai-0.1.1/tests/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17356 2023-07-02 06:46:51.000000 mona-openai-0.1.1/tests/test_chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    20681 2023-07-10 12:46:59.000000 mona-openai-0.1.1/tests/test_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.1.1/tests/test_privacy_analyzer.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      975 2023-06-29 11:44:26.000000 mona-openai-0.1.1/tests/test_textual_analyzer.py
```

### Comparing `mona-openai-0.1.0/LICENSE` & `mona-openai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/PKG-INFO` & `mona-openai-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6f 6e61  : 2.1.Name: mona
 00000020: 2d6f 7065 6e61 690a 5665 7273 696f 6e3a  -openai.Version:
-00000030: 2030 2e31 2e30 0a53 756d 6d61 7279 3a20   0.1.0.Summary: 
+00000030: 2030 2e31 2e31 0a53 756d 6d61 7279 3a20   0.1.1.Summary: 
 00000040: 496e 7465 6772 6174 696f 6e20 636c 6965  Integration clie
 00000050: 6e74 2066 6f72 206d 6f6e 6974 6f72 696e  nt for monitorin
 00000060: 6720 4f70 656e 4149 2075 7361 6765 2077  g OpenAI usage w
 00000070: 6974 6820 4d6f 6e61 0a41 7574 686f 722d  ith Mona.Author-
 00000080: 656d 6169 6c3a 2049 7461 6920 4261 7220  email: Itai Bar 
 00000090: 5369 6e61 6920 3c69 7461 6940 6d6f 6e61  Sinai <itai@mona
 000000a0: 6c61 6273 2e69 6f3e 0a50 726f 6a65 6374  labs.io>.Project
@@ -69,707 +69,715 @@
 00000440: 7574 746f 6e3d 3126 616d 703b 696d 6167  utton=1&amp;imag
 00000450: 655f 706c 6179 5f62 7574 746f 6e5f 636f  e_play_button_co
 00000460: 6c6f 723d 3636 6337 6431 6530 2220 7769  lor=66c7d1e0" wi
 00000470: 6474 683d 2234 3030 2220 6865 6967 6874  dth="400" height
 00000480: 3d22 3232 3522 2073 7479 6c65 3d22 7769  ="225" style="wi
 00000490: 6474 683a 2034 3030 7078 3b20 6865 6967  dth: 400px; heig
 000004a0: 6874 3a20 3232 3570 783b 223e 3c2f 613e  ht: 225px;"></a>
-000004b0: 3c2f 703e 3c70 2061 6c69 676e 3d22 6365  </p><p align="ce
-000004c0: 6e74 6572 223e 3c61 2068 7265 663d 2268  nter"><a href="h
-000004d0: 7474 7073 3a2f 2f6d 6f6e 616c 6162 732e  ttps://monalabs.
-000004e0: 7769 7374 6961 2e63 6f6d 2f6d 6564 6961  wistia.com/media
-000004f0: 732f 6c36 786d 646a 3363 6436 3f77 7669  s/l6xmdj3cd6?wvi
-00000500: 6465 6f3d 6c36 786d 646a 3363 6436 223e  deo=l6xmdj3cd6">
-00000510: 4f70 656e 4149 2047 5054 2049 6e74 6567  OpenAI GPT Integ
-00000520: 7261 7469 6f6e 2054 7574 6f72 6961 6c3c  ration Tutorial<
-00000530: 2f61 3e3c 2f70 3e0a 0a0a 5573 6520 6f6e  /a></p>...Use on
-00000540: 6520 6c69 6e65 206f 6620 636f 6465 2074  e line of code t
-00000550: 6f20 6765 7420 696e 7374 616e 7420 6c69  o get instant li
-00000560: 7665 206d 6f6e 6974 6f72 696e 6720 666f  ve monitoring fo
-00000570: 7220 796f 7572 204f 7065 6e41 4920 7573  r your OpenAI us
-00000580: 6167 6520 696e 636c 7564 696e 673a 0a2a  age including:.*
-00000590: 2054 6f6b 656e 7320 7573 6167 650a 2a20   Tokens usage.* 
-000005a0: 4861 6c6c 7563 696e 6174 696f 6e20 616c  Hallucination al
-000005b0: 6572 7473 0a2a 2050 726f 6661 6e69 7479  erts.* Profanity
-000005c0: 2061 6e64 2070 7269 7661 6379 2061 6e61   and privacy ana
-000005d0: 6c79 7365 730a 2a20 4265 6861 7669 6f72  lyses.* Behavior
-000005e0: 616c 2064 7269 6674 7320 616e 6420 616e  al drifts and an
-000005f0: 6f6d 616c 6965 730a 2a20 4c61 6e67 4368  omalies.* LangCh
-00000600: 6169 6e20 7375 7070 6f72 740a 2a20 4d75  ain support.* Mu
-00000610: 6368 206d 7563 6820 6d6f 7265 0a0a 2323  ch much more..##
-00000620: 2053 6574 7469 6e67 2055 700a 0a60 6060   Setting Up..```
-00000630: 636f 6e73 6f6c 650a 2420 7069 7020 696e  console.$ pip in
-00000640: 7374 616c 6c20 6d6f 6e61 5f6f 7065 6e61  stall mona_opena
-00000650: 690a 6060 600a 0a49 6620 796f 7520 706c  i.```..If you pl
-00000660: 616e 206f 6e20 7573 696e 6720 4d6f 6e61  an on using Mona
-00000670: 2061 7320 796f 7572 206d 6f6e 6974 6f72   as your monitor
-00000680: 696e 6720 7365 7276 6963 652c 205b 7369  ing service, [si
-00000690: 676e 2075 7020 666f 7220 6120 6672 6565  gn up for a free
-000006a0: 2061 6363 6f75 6e74 2068 6572 655d 2868   account here](h
-000006b0: 7474 7073 3a2f 2f77 7777 2e6d 6f6e 616c  ttps://www.monal
-000006c0: 6162 732e 696f 2f6f 7065 6e61 692d 6770  abs.io/openai-gp
-000006d0: 742d 6d6f 6e69 746f 7269 6e67 292e 0a0a  t-monitoring)...
-000006e0: 2323 2051 7569 636b 2053 7461 7274 0a0a  ## Quick Start..
-000006f0: 596f 7520 6361 6e20 6669 6e64 2062 6f69  You can find boi
-00000700: 6c65 7270 6c61 7465 2063 6f64 6520 666f  lerplate code fo
-00000710: 7220 6d61 6e79 2075 7365 2d63 6173 6573  r many use-cases
-00000720: 2075 6e64 6572 205b 7468 6520 2265 7861   under [the "exa
-00000730: 6d70 6c65 7322 2066 6f6c 6465 725d 2868  mples" folder](h
-00000740: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000750: 6d2f 6d6f 6e61 6c61 6273 2f6d 6f6e 612d  m/monalabs/mona-
-00000760: 6f70 656e 6169 2f74 7265 652f 6d61 696e  openai/tree/main
-00000770: 2f65 7861 6d70 6c65 7329 2e0a 0a60 6060  /examples)...```
-00000780: 7079 0a66 726f 6d20 6f73 2069 6d70 6f72  py.from os impor
-00000790: 7420 656e 7669 726f 6e0a 696d 706f 7274  t environ.import
-000007a0: 2061 7379 6e63 696f 0a69 6d70 6f72 7420   asyncio.import 
-000007b0: 6f70 656e 6169 0a66 726f 6d20 6d6f 6e61  openai.from mona
-000007c0: 5f6f 7065 6e61 692e 6c6f 6767 6572 7320  _openai.loggers 
-000007d0: 696d 706f 7274 2053 7461 6e64 6172 644c  import StandardL
-000007e0: 6f67 6765 720a 6672 6f6d 206c 6f67 6769  ogger.from loggi
-000007f0: 6e67 2069 6d70 6f72 7420 5741 524e 494e  ng import WARNIN
-00000800: 470a 0a66 726f 6d20 6d6f 6e61 5f6f 7065  G..from mona_ope
-00000810: 6e61 6920 696d 706f 7274 206d 6f6e 6974  nai import monit
-00000820: 6f72 2c20 6d6f 6e69 746f 725f 7769 7468  or, monitor_with
-00000830: 5f6c 6f67 6765 720a 0a6f 7065 6e61 692e  _logger..openai.
-00000840: 6170 695f 6b65 7920 3d20 656e 7669 726f  api_key = enviro
-00000850: 6e2e 6765 7428 224f 5045 4e5f 4149 5f4b  n.get("OPEN_AI_K
-00000860: 4559 2229 0a0a 2320 5768 656e 2075 7369  EY")..# When usi
-00000870: 6e67 2061 2073 7461 6e64 6172 6420 6c6f  ng a standard lo
-00000880: 6767 6572 2e0a 0a6d 6f6e 6974 6f72 6564  gger...monitored
-00000890: 5f63 6f6d 706c 6574 696f 6e20 3d20 6d6f  _completion = mo
-000008a0: 6e69 746f 725f 7769 7468 5f6c 6f67 6765  nitor_with_logge
-000008b0: 7228 0a20 2020 206f 7065 6e61 692e 436f  r(.    openai.Co
-000008c0: 6d70 6c65 7469 6f6e 2c0a 2020 2020 5374  mpletion,.    St
-000008d0: 616e 6461 7264 4c6f 6767 6572 2857 4152  andardLogger(WAR
-000008e0: 4e49 4e47 292c 0a29 0a0a 7265 7370 6f6e  NING),.)..respon
-000008f0: 7365 203d 206d 6f6e 6974 6f72 6564 5f63  se = monitored_c
-00000900: 6f6d 706c 6574 696f 6e2e 6372 6561 7465  ompletion.create
-00000910: 280a 2020 2020 6d6f 6465 6c3d 2274 6578  (.    model="tex
-00000920: 742d 6164 612d 3030 3122 2c0a 2020 2020  t-ada-001",.    
-00000930: 7072 6f6d 7074 3d22 4920 7761 6e74 2074  prompt="I want t
-00000940: 6f20 6765 6e65 7261 7465 2073 6f6d 6520  o generate some 
-00000950: 7465 7874 2061 626f 7574 2022 2c0a 2020  text about ",.  
-00000960: 2020 6d61 785f 746f 6b65 6e73 3d32 302c    max_tokens=20,
-00000970: 0a20 2020 206e 3d31 2c0a 2020 2020 7465  .    n=1,.    te
-00000980: 6d70 6572 6174 7572 653d 302e 322c 0a20  mperature=0.2,. 
-00000990: 2020 2023 2041 6464 696e 6720 6164 6469     # Adding addi
-000009a0: 7469 6f6e 616c 2069 6e66 6f72 6d61 7469  tional informati
-000009b0: 6f6e 2066 6f72 206d 6f6e 6974 6f72 696e  on for monitorin
-000009c0: 6720 7075 7270 6f73 6573 2c20 756e 7265  g purposes, unre
-000009d0: 6c61 7465 6420 746f 0a20 2020 2023 2069  lated to.    # i
-000009e0: 6e74 6572 6e61 6c20 4f70 656e 4149 2063  nternal OpenAI c
-000009f0: 616c 6c2e 0a20 2020 204d 4f4e 415f 6164  all..    MONA_ad
-00000a00: 6469 7469 6f6e 616c 5f64 6174 613d 7b22  ditional_data={"
-00000a10: 6375 7374 6f6d 6572 5f69 6422 3a20 2241  customer_id": "A
-00000a20: 3533 3132 3531 227d 2c0a 290a 7072 696e  531251"},.).prin
-00000a30: 7428 7265 7370 6f6e 7365 2e63 686f 6963  t(response.choic
-00000a40: 6573 5b30 5d2e 7465 7874 290a 0a0a 2320  es[0].text)...# 
-00000a50: 5768 656e 206d 6f6e 6974 6f72 696e 6720  When monitoring 
-00000a60: 7769 7468 204d 6f6e 612e 0a0a 4d4f 4e41  with Mona...MONA
-00000a70: 5f41 5049 5f4b 4559 203d 2065 6e76 6972  _API_KEY = envir
-00000a80: 6f6e 2e67 6574 2822 4d4f 4e41 5f41 5049  on.get("MONA_API
-00000a90: 5f4b 4559 2229 0a4d 4f4e 415f 5345 4352  _KEY").MONA_SECR
-00000aa0: 4554 203d 2065 6e76 6972 6f6e 2e67 6574  ET = environ.get
-00000ab0: 2822 4d4f 4e41 5f53 4543 5245 5422 290a  ("MONA_SECRET").
-00000ac0: 4d4f 4e41 5f43 5245 4453 203d 207b 0a20  MONA_CREDS = {. 
-00000ad0: 2020 2022 6b65 7922 3a20 4d4f 4e41 5f41     "key": MONA_A
-00000ae0: 5049 5f4b 4559 2c0a 2020 2020 2273 6563  PI_KEY,.    "sec
-00000af0: 7265 7422 3a20 4d4f 4e41 5f53 4543 5245  ret": MONA_SECRE
-00000b00: 542c 0a7d 0a43 4f4e 5445 5854 5f43 4c41  T,.}.CONTEXT_CLA
-00000b10: 5353 5f4e 414d 4520 3d20 2253 4f4d 455f  SS_NAME = "SOME_
-00000b20: 4d4f 4e49 544f 5249 4e47 5f43 4f4e 5445  MONITORING_CONTE
-00000b30: 5854 5f4e 414d 4522 0a0a 0a6d 6f6e 6974  XT_NAME"...monit
-00000b40: 6f72 6564 5f63 6f6d 706c 6574 696f 6e20  ored_completion 
-00000b50: 3d20 6d6f 6e69 746f 7228 0a20 2020 206f  = monitor(.    o
-00000b60: 7065 6e61 692e 436f 6d70 6c65 7469 6f6e  penai.Completion
-00000b70: 2c0a 2020 2020 4d4f 4e41 5f43 5245 4453  ,.    MONA_CREDS
-00000b80: 2c0a 2020 2020 434f 4e54 4558 545f 434c  ,.    CONTEXT_CL
-00000b90: 4153 535f 4e41 4d45 2c0a 290a 0a72 6573  ASS_NAME,.)..res
-00000ba0: 706f 6e73 6520 3d20 6d6f 6e69 746f 7265  ponse = monitore
-00000bb0: 645f 636f 6d70 6c65 7469 6f6e 2e63 7265  d_completion.cre
-00000bc0: 6174 6528 0a20 2020 206d 6f64 656c 3d22  ate(.    model="
-00000bd0: 7465 7874 2d61 6461 2d30 3031 222c 0a20  text-ada-001",. 
-00000be0: 2020 2070 726f 6d70 743d 2249 2077 616e     prompt="I wan
-00000bf0: 7420 746f 2067 656e 6572 6174 6520 736f  t to generate so
-00000c00: 6d65 2074 6578 7420 6162 6f75 7420 222c  me text about ",
-00000c10: 0a20 2020 206d 6178 5f74 6f6b 656e 733d  .    max_tokens=
-00000c20: 3230 2c0a 2020 2020 6e3d 312c 0a20 2020  20,.    n=1,.   
-00000c30: 2074 656d 7065 7261 7475 7265 3d30 2e32   temperature=0.2
-00000c40: 2c0a 2020 2020 2320 4164 6469 6e67 2061  ,.    # Adding a
-00000c50: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
-00000c60: 6174 696f 6e20 666f 7220 6d6f 6e69 746f  ation for monito
-00000c70: 7269 6e67 2070 7572 706f 7365 732c 2075  ring purposes, u
-00000c80: 6e72 656c 6174 6564 2074 6f0a 2020 2020  nrelated to.    
-00000c90: 2320 696e 7465 726e 616c 204f 7065 6e41  # internal OpenA
-00000ca0: 4920 6361 6c6c 2e0a 2020 2020 4d4f 4e41  I call..    MONA
-00000cb0: 5f61 6464 6974 696f 6e61 6c5f 6461 7461  _additional_data
-00000cc0: 3d7b 2263 7573 746f 6d65 725f 6964 223a  ={"customer_id":
-00000cd0: 2022 4135 3331 3235 3122 7d2c 0a29 0a70   "A531251"},.).p
-00000ce0: 7269 6e74 2872 6573 706f 6e73 652e 6368  rint(response.ch
-00000cf0: 6f69 6365 735b 305d 2e74 6578 7429 0a60  oices[0].text).`
-00000d00: 6060 0a23 2320 5375 7070 6f72 7465 6420  ``.## Supported 
-00000d10: 4f70 656e 4149 2041 5049 730a 4375 7272  OpenAI APIs.Curr
-00000d20: 656e 746c 7920 7468 6973 2063 6c69 656e  ently this clien
-00000d30: 7420 7375 7070 6f72 7473 2060 6f70 656e  t supports `open
-00000d40: 6169 2e43 6f6d 706c 6574 696f 6e60 2061  ai.Completion` a
-00000d50: 6e64 2060 6f70 656e 6169 2e43 6861 7443  nd `openai.ChatC
-00000d60: 6f6d 706c 6574 696f 6e60 2e20 4d6f 6e61  ompletion`. Mona
-00000d70: 2063 616e 2073 7570 706f 7274 2070 726f   can support pro
-00000d80: 6365 7373 6573 2062 6173 6564 206f 6e20  cesses based on 
-00000d90: 6f74 6865 7220 4150 4973 2061 6e64 2061  other APIs and a
-00000da0: 6c73 6f20 6e6f 6e2d 4f70 656e 4149 2d62  lso non-OpenAI-b
-00000db0: 6173 6564 2061 7070 732e 0a49 6620 796f  ased apps..If yo
-00000dc0: 7520 6861 7665 2061 2064 6966 6665 7272  u have a differr
-00000dd0: 656e 7420 7573 652d 6361 7365 2c20 7765  ent use-case, we
-00000de0: 2764 206c 6f76 6520 746f 2068 6561 7220  'd love to hear 
-00000df0: 6162 6f75 7420 6974 2120 506c 6561 7365  about it! Please
-00000e00: 2065 6d61 696c 2075 7320 6174 2073 7570   email us at sup
-00000e10: 706f 7274 406d 6f6e 616c 6162 732e 696f  port@monalabs.io
-00000e20: 2e0a 0a23 2320 5573 6167 650a 2323 2320  ...## Usage.### 
-00000e30: 496e 6974 6961 6c69 7a61 7469 6f6e 0a0a  Initialization..
-00000e40: 5468 6520 6d61 696e 2061 6e64 206f 6e6c  The main and onl
-00000e50: 7920 6675 6e63 7469 6f6e 2065 7870 6f73  y function expos
-00000e60: 6564 2069 6e20 7468 6973 2070 6163 6b61  ed in this packa
-00000e70: 6765 2069 7320 606d 6f6e 6974 6f72 602e  ge is `monitor`.
-00000e80: 0a60 6060 7079 0a69 6d70 6f72 7420 6f70  .```py.import op
-00000e90: 656e 6169 0a0a 6672 6f6d 206d 6f6e 615f  enai..from mona_
-00000ea0: 6f70 656e 6169 2069 6d70 6f72 7420 6d6f  openai import mo
-00000eb0: 6e69 746f 720a 0a6f 7065 6e61 692e 6170  nitor..openai.ap
-00000ec0: 695f 6b65 7920 3d20 656e 7669 726f 6e2e  i_key = environ.
-00000ed0: 6765 7428 224f 5045 4e5f 4149 5f4b 4559  get("OPEN_AI_KEY
-00000ee0: 2229 0a0a 6d6f 6e69 746f 7265 645f 636f  ")..monitored_co
-00000ef0: 6d70 6c65 7469 6f6e 203d 206d 6f6e 6974  mpletion = monit
-00000f00: 6f72 280a 2020 2020 6f70 656e 6169 2e43  or(.    openai.C
-00000f10: 6f6d 706c 6574 696f 6e2c 0a20 2020 2028  ompletion,.    (
-00000f20: 0a20 2020 2020 2020 2065 6e76 6972 6f6e  .        environ
-00000f30: 2e67 6574 2822 4d4f 4e41 5f41 5049 5f4b  .get("MONA_API_K
-00000f40: 4559 2229 2c0a 2020 2020 2020 2020 656e  EY"),.        en
-00000f50: 7669 726f 6e2e 6765 7428 224d 4f4e 415f  viron.get("MONA_
-00000f60: 5345 4352 4554 2229 2c0a 2020 2020 292c  SECRET"),.    ),
-00000f70: 0a20 2020 2022 534f 4d45 5f4d 4f4e 4954  .    "SOME_MONIT
-00000f80: 4f52 494e 475f 434f 4e54 4558 545f 4e41  ORING_CONTEXT_NA
-00000f90: 4d45 222c 0a20 2020 207b 2261 6e61 6c79  ME",.    {"analy
-00000fa0: 7369 7322 3a20 7b22 7072 6f66 616e 6974  sis": {"profanit
-00000fb0: 7922 3a20 4661 6c73 657d 7d0a 290a 0a2e  y": False}}.)...
-00000fc0: 2e2e 0a0a 6d6f 6e69 746f 7265 645f 636f  ....monitored_co
-00000fd0: 6d70 6c65 7469 6f6e 2e63 7265 6174 6528  mpletion.create(
-00000fe0: 2e2e 2e29 0a60 6060 0a0a 5468 6520 606d  ...).```..The `m
-00000ff0: 6f6e 6974 6f72 6020 6675 6e63 7469 6f6e  onitor` function
-00001000: 2072 6574 7572 6e73 2074 6f20 796f 7520   returns to you 
-00001010: 6120 636c 6173 7320 7468 6174 2077 7261  a class that wra
-00001020: 7073 2074 6865 206f 7269 6769 6e61 6c20  ps the original 
-00001030: 6f70 656e 6169 2065 6e64 706f 696e 7420  openai endpoint 
-00001040: 636c 6173 7320 796f 7520 7072 6f76 6964  class you provid
-00001050: 652c 2077 6974 6820 616e 2065 7175 6976  e, with an equiv
-00001060: 616c 656e 7420 4150 4920 2862 6573 6964  alent API (besid
-00001070: 6573 2073 6f6d 6520 6164 6469 7469 6f6e  es some addition
-00001080: 7320 6c69 7374 6564 2062 656c 6f77 292e  s listed below).
-00001090: 0a59 6f75 2063 616e 2074 6865 6e20 7573  .You can then us
-000010a0: 6520 7468 6520 7265 7475 726e 6564 2063  e the returned c
-000010b0: 6c61 7373 2720 2263 7265 6174 6522 2061  lass' "create" a
-000010c0: 6e64 2022 6163 7265 6174 6522 2066 756e  nd "acreate" fun
-000010d0: 6374 696f 6e73 206a 7573 7420 6173 2079  ctions just as y
-000010e0: 6f75 2077 6f75 6c64 2062 6566 6f72 652c  ou would before,
-000010f0: 206f 6e6c 7920 6e6f 772c 2062 6573 6964   only now, besid
-00001100: 6573 2067 6574 7469 6e67 2074 6865 2072  es getting the r
-00001110: 6571 7565 7374 6564 206f 7065 6e41 4920  equested openAI 
-00001120: 6675 6e63 7469 6f6e 616c 6974 792c 2074  functionality, t
-00001130: 6869 7320 636c 6965 6e74 2077 696c 6c20  his client will 
-00001140: 6c6f 6720 6f75 7420 746f 204d 6f6e 6127  log out to Mona'
-00001150: 7320 7365 7276 6572 2074 6865 2070 6172  s server the par
-00001160: 616d 6574 6572 7320 796f 7520 7573 6564  ameters you used
-00001170: 2028 652e 672e 2c20 7465 6d70 6572 6174   (e.g., temperat
-00001180: 7572 6529 2c20 6461 7461 2061 626f 7574  ure), data about
-00001190: 2074 6865 2072 6573 706f 6e73 6520 6672   the response fr
-000011a0: 6f6d 204f 7065 6e41 4927 7320 7365 7276  om OpenAI's serv
-000011b0: 6572 2c20 616e 6420 6375 7374 6f6d 2061  er, and custom a
-000011c0: 6e61 6c79 7365 7320 6162 6f75 7420 7468  nalyses about th
-000011d0: 6520 6361 6c6c 2028 652e 672e 2c20 7072  e call (e.g., pr
-000011e0: 6f66 616e 6974 7920 7363 6f72 6573 2c20  ofanity scores, 
-000011f0: 7072 6976 6163 7920 6368 6563 6b73 2066  privacy checks f
-00001200: 6f72 2065 6d61 696c 732f 7068 6f6e 6520  or emails/phone 
-00001210: 6e75 6d62 6572 7320 666f 756e 6420 696e  numbers found in
-00001220: 2074 6865 2074 6578 7473 2c20 7465 7874   the texts, text
-00001230: 7561 6c20 616e 616c 7973 6573 2c20 6574  ual analyses, et
-00001240: 632e 2e2e 290a 0a54 6865 2060 6d6f 6e69  c...)..The `moni
-00001250: 746f 7260 2066 756e 6374 696f 6e20 7265  tor` function re
-00001260: 6365 6976 6573 2074 6865 2066 6f6c 6c6f  ceives the follo
-00001270: 7769 6e67 2061 7267 756d 656e 7473 3a0a  wing arguments:.
-00001280: 6f70 656e 6169 5f63 6c61 7373 3a20 416e  openai_class: An
-00001290: 204f 7065 6e41 4920 4150 4920 636c 6173   OpenAI API clas
-000012a0: 7320 746f 2077 7261 7020 7769 7468 206d  s to wrap with m
-000012b0: 6f6e 6974 6f72 696e 6720 6361 7061 6269  onitoring capabi
-000012c0: 6c74 6965 732e 0a6d 6f6e 615f 6372 6564  lties..mona_cred
-000012d0: 733a 2041 2064 6963 7420 2863 6f6e 7461  s: A dict (conta
-000012e0: 696e 696e 6720 226b 6579 2220 616e 6420  ining "key" and 
-000012f0: 2273 6563 7265 7422 2920 6f72 2070 6169  "secret") or pai
-00001300: 7220 2874 7570 6c65 2920 6f66 204d 6f6e  r (tuple) of Mon
-00001310: 6120 4150 4920 6b65 7920 616e 6420 7365  a API key and se
-00001320: 6372 6574 2074 6f20 7365 7420 7570 204d  cret to set up M
-00001330: 6f6e 6127 7320 636c 6965 6e74 7320 6672  ona's clients fr
-00001340: 6f6d 2069 7473 2053 444b 2e0a 636f 6e74  om its SDK..cont
-00001350: 6578 745f 636c 6173 733a 2054 6865 204d  ext_class: The M
-00001360: 6f6e 6120 636f 6e74 6578 7420 636c 6173  ona context clas
-00001370: 7320 6e61 6d65 2074 6f20 7573 6520 666f  s name to use fo
-00001380: 7220 6d6f 6e69 746f 7269 6e67 2e20 5573  r monitoring. Us
-00001390: 6520 6120 636f 6e73 7461 6e74 206e 616d  e a constant nam
-000013a0: 6520 6f66 2079 6f75 7220 6368 6f69 6365  e of your choice
-000013b0: 2e0a 7370 6563 733a 2041 2064 6963 7469  ..specs: A dicti
-000013c0: 6f6e 6172 7920 6f66 2073 7065 6369 6669  onary of specifi
-000013d0: 6361 7469 6f6e 7320 7375 6368 2061 7320  cations such as 
-000013e0: 6d6f 6e69 746f 7269 6e67 2073 616d 706c  monitoring sampl
-000013f0: 696e 6720 7261 7469 6f2e 0a0a 2323 2323  ing ratio...####
-00001400: 2053 7065 6373 0a54 6865 2073 7065 6373   Specs.The specs
-00001410: 2061 7267 2061 6c6c 6f77 7320 796f 7520   arg allows you 
-00001420: 746f 2063 6f6e 6669 6775 7265 2077 6861  to configure wha
-00001430: 7420 7368 6f75 6c64 2062 6520 6d6f 6e69  t should be moni
-00001440: 746f 7265 642e 2049 7420 6578 7065 6374  tored. It expect
-00001450: 7320 6120 7079 7468 6f6e 2064 6963 7420  s a python dict 
-00001460: 7769 7468 2074 6865 2066 6f6c 6c77 6f69  with the follwoi
-00001470: 6e67 2070 6f73 7369 626c 6520 6b65 7973  ng possible keys
-00001480: 3a0a 2a20 7361 6d70 6c69 6e67 5f72 6174  :.* sampling_rat
-00001490: 696f 2028 3129 3a20 4120 6e75 6d62 6572  io (1): A number
-000014a0: 2062 6574 7765 656e 2030 2061 6e64 2031   between 0 and 1
-000014b0: 2066 6f72 2068 6f77 206f 6674 656e 2073   for how often s
-000014c0: 686f 756c 6420 7468 6520 6361 6c6c 2062  hould the call b
-000014d0: 6520 6c6f 6767 6564 2e0a 2a20 6176 6f69  e logged..* avoi
-000014e0: 645f 6d6f 6e69 746f 7269 6e67 5f65 7863  d_monitoring_exc
-000014f0: 6570 7469 6f6e 7320 2846 616c 7365 293a  eptions (False):
-00001500: 2057 6865 7468 6572 206f 7220 6e6f 7420   Whether or not 
-00001510: 746f 206c 6f67 206f 7574 2074 6f20 4d6f  to log out to Mo
-00001520: 6e61 2077 6865 6e20 7468 6572 6520 6973  na when there is
-00001530: 2061 6e20 4f70 656e 4149 2065 7863 6570   an OpenAI excep
-00001540: 7469 6f6e 2e20 4465 6661 756c 7420 6973  tion. Default is
-00001550: 2074 6f20 7472 6163 6b20 6578 6365 7074   to track except
-00001560: 696f 6e73 202d 2061 6e64 204d 6f6e 6120  ions - and Mona 
-00001570: 7769 6c6c 2061 6c65 7274 2079 6f75 206f  will alert you o
-00001580: 6e20 7468 696e 6773 206c 696b 6520 6120  n things like a 
-00001590: 6a75 6d70 2069 6e20 6e75 6d62 6572 206f  jump in number o
-000015a0: 6620 6578 6365 7074 696f 6e73 0a2a 2065  f exceptions.* e
-000015b0: 7870 6f72 745f 7072 6f6d 7074 2028 4661  xport_prompt (Fa
-000015c0: 6c73 6529 3a20 5768 6574 6865 7220 4d6f  lse): Whether Mo
-000015d0: 6e61 2073 686f 756c 6420 6578 706f 7274  na should export
-000015e0: 2074 6865 2061 6374 7561 6c20 7072 6f6d   the actual prom
-000015f0: 7074 2074 6578 742e 2042 6520 6465 6661  pt text. Be defa
-00001600: 756c 7420 7365 7420 746f 2046 616c 7365  ult set to False
-00001610: 2074 6f20 6176 6f69 6420 7072 6976 6163   to avoid privac
-00001620: 7920 636f 6e63 6572 6e73 2e0a 2a20 6578  y concerns..* ex
-00001630: 706f 7274 5f72 6573 706f 6e73 655f 7465  port_response_te
-00001640: 7874 7320 2846 616c 7365 293a 2057 6865  xts (False): Whe
-00001650: 7468 6572 204d 6f6e 6120 7368 6f75 6c64  ther Mona should
-00001660: 2065 7870 6f72 7420 7468 6520 6163 7475   export the actu
-00001670: 616c 2072 6573 706f 6e73 6520 7465 7874  al response text
-00001680: 732e 2042 6520 6465 6661 756c 7420 7365  s. Be default se
-00001690: 7420 746f 2046 616c 7365 2074 6f20 6176  t to False to av
-000016a0: 6f69 6420 7072 6976 6163 7920 636f 6e63  oid privacy conc
-000016b0: 6572 6e73 2e0a 2a20 616e 616c 7973 6973  erns..* analysis
-000016c0: 3a20 4120 6469 6374 696f 6e61 7279 206d  : A dictionary m
-000016d0: 6170 7069 6e67 2065 6163 6820 616e 616c  apping each anal
-000016e0: 7973 6973 2074 7970 6520 746f 2061 2062  ysis type to a b
-000016f0: 6f6f 6c65 616e 2076 616c 7565 2074 656c  oolean value tel
-00001700: 6c69 6e67 2074 6865 2063 6c69 656e 7420  ling the client 
-00001710: 7768 6574 6865 7220 6f72 206e 6f74 2074  whether or not t
-00001720: 6f20 7275 6e20 7361 6964 2061 6e61 6c79  o run said analy
-00001730: 7369 7320 616e 6420 6c6f 6720 6974 2074  sis and log it t
-00001740: 6f20 4d6f 6e61 2e20 506f 7373 6962 6c65  o Mona. Possible
-00001750: 206f 7074 696f 6e73 2063 7572 7265 6e74   options current
-00001760: 6c79 2061 7265 2022 7072 6976 6163 7922  ly are "privacy"
-00001770: 2c20 2270 726f 6661 6e69 7479 222c 2061  , "profanity", a
-00001780: 6e64 2022 7465 7874 7561 6c22 2e20 4279  nd "textual". By
-00001790: 2064 6566 6175 6c74 2c20 616c 6c20 616e   default, all an
-000017a0: 616c 7973 6573 2074 616b 6520 706c 6163  alyses take plac
-000017b0: 6520 616e 6420 6172 6520 6c6f 6767 6564  e and are logged
-000017c0: 206f 7574 2074 6f20 4d6f 6e61 2e0a 0a23   out to Mona...#
-000017d0: 2323 2055 7369 6e67 2063 7573 746f 6d20  ## Using custom 
-000017e0: 6c6f 6767 6572 730a 596f 7520 646f 6e27  loggers.You don'
-000017f0: 7420 6861 7665 2074 6f20 6861 7665 2061  t have to have a
-00001800: 204d 6f6e 6120 6163 636f 756e 7420 746f   Mona account to
-00001810: 2075 7365 2074 6869 7320 7061 636b 6167   use this packag
-00001820: 652e 2059 6f75 2063 616e 2064 6566 696e  e. You can defin
-00001830: 6520 7370 6563 6966 6963 206c 6f67 6765  e specific logge
-00001840: 7273 2074 6f20 6c6f 6720 6f75 7420 7468  rs to log out th
-00001850: 6520 6461 7461 2074 6f20 6120 6669 6c65  e data to a file
-00001860: 2c20 6d65 6d6f 7279 2c20 6f72 206a 7573  , memory, or jus
-00001870: 7420 6120 6769 7665 6e20 7079 7468 6f6e  t a given python
-00001880: 206c 6f67 6765 722e 2046 6f72 2065 7861   logger. For exa
-00001890: 6d70 6c65 2c20 746f 206c 6f67 206f 7574  mple, to log out
-000018a0: 2074 6865 2072 656c 6576 616e 7420 6d65   the relevant me
-000018b0: 7472 6963 7320 6173 2057 4152 4e49 4e47  trics as WARNING
-000018c0: 3a0a 0a60 6060 7079 0a66 726f 6d20 6f73  :..```py.from os
-000018d0: 2069 6d70 6f72 7420 656e 7669 726f 6e0a   import environ.
-000018e0: 696d 706f 7274 206f 7065 6e61 690a 6672  import openai.fr
-000018f0: 6f6d 206d 6f6e 615f 6f70 656e 6169 2e6c  om mona_openai.l
-00001900: 6f67 6765 7273 2069 6d70 6f72 7420 5374  oggers import St
-00001910: 616e 6461 7264 4c6f 6767 6572 0a66 726f  andardLogger.fro
-00001920: 6d20 6c6f 6767 696e 6720 696d 706f 7274  m logging import
-00001930: 2057 4152 4e49 4e47 0a0a 6672 6f6d 206d   WARNING..from m
-00001940: 6f6e 615f 6f70 656e 6169 2069 6d70 6f72  ona_openai impor
-00001950: 7420 6d6f 6e69 746f 725f 7769 7468 5f6c  t monitor_with_l
-00001960: 6f67 6765 720a 0a6f 7065 6e61 692e 6170  ogger..openai.ap
-00001970: 695f 6b65 7920 3d20 656e 7669 726f 6e2e  i_key = environ.
-00001980: 6765 7428 224f 5045 4e5f 4149 5f4b 4559  get("OPEN_AI_KEY
-00001990: 2229 0a0a 6d6f 6e69 746f 7265 645f 636f  ")..monitored_co
-000019a0: 6d70 6c65 7469 6f6e 203d 206d 6f6e 6974  mpletion = monit
-000019b0: 6f72 5f77 6974 685f 6c6f 6767 6572 280a  or_with_logger(.
-000019c0: 2020 2020 6f70 656e 6169 2e43 6f6d 706c      openai.Compl
-000019d0: 6574 696f 6e2c 0a20 2020 2053 7461 6e64  etion,.    Stand
-000019e0: 6172 644c 6f67 6765 7228 5741 524e 494e  ardLogger(WARNIN
-000019f0: 4729 2c0a 290a 0a72 6573 706f 6e73 6520  G),.)..response 
-00001a00: 3d20 6d6f 6e69 746f 7265 645f 636f 6d70  = monitored_comp
-00001a10: 6c65 7469 6f6e 2e63 7265 6174 6528 0a20  letion.create(. 
-00001a20: 2020 206d 6f64 656c 3d22 7465 7874 2d61     model="text-a
-00001a30: 6461 2d30 3031 222c 0a20 2020 2070 726f  da-001",.    pro
-00001a40: 6d70 743d 2249 2077 616e 7420 746f 2067  mpt="I want to g
-00001a50: 656e 6572 6174 6520 736f 6d65 2074 6578  enerate some tex
-00001a60: 7420 6162 6f75 7420 222c 0a20 2020 206d  t about ",.    m
-00001a70: 6178 5f74 6f6b 656e 733d 3230 2c0a 2020  ax_tokens=20,.  
-00001a80: 2020 6e3d 312c 0a20 2020 2074 656d 7065    n=1,.    tempe
-00001a90: 7261 7475 7265 3d30 2e32 2c0a 2020 2020  rature=0.2,.    
-00001aa0: 2320 4164 6469 6e67 2061 6464 6974 696f  # Adding additio
-00001ab0: 6e61 6c20 696e 666f 726d 6174 696f 6e20  nal information 
-00001ac0: 666f 7220 6d6f 6e69 746f 7269 6e67 2070  for monitoring p
-00001ad0: 7572 706f 7365 732c 2075 6e72 656c 6174  urposes, unrelat
-00001ae0: 6564 2074 6f0a 2020 2020 2320 696e 7465  ed to.    # inte
-00001af0: 726e 616c 204f 7065 6e41 4920 6361 6c6c  rnal OpenAI call
-00001b00: 2e0a 2020 2020 4d4f 4e41 5f61 6464 6974  ..    MONA_addit
-00001b10: 696f 6e61 6c5f 6461 7461 3d7b 2263 7573  ional_data={"cus
-00001b20: 746f 6d65 725f 6964 223a 2022 4135 3331  tomer_id": "A531
-00001b30: 3235 3122 7d2c 0a29 0a60 6060 0a0a 5468  251"},.).```..Th
-00001b40: 6973 2053 444b 2070 726f 7669 6465 7320  is SDK provides 
-00001b50: 6120 7369 6d70 6c65 2069 6e74 6572 6661  a simple interfa
-00001b60: 6365 2074 6f20 696d 706c 656d 656e 7420  ce to implement 
-00001b70: 796f 7572 206f 776e 206c 6f67 6765 7273  your own loggers
-00001b80: 2062 7920 696e 6865 7269 7469 6e67 2066   by inheriting f
-00001b90: 726f 6d20 4c6f 6767 6572 2075 6e64 6572  rom Logger under
-00001ba0: 206c 6f67 6765 7273 2f6c 6f67 6765 722e   loggers/logger.
-00001bb0: 7079 2e0a 416c 7465 726e 6174 6976 656c  py..Alternativel
-00001bc0: 792c 2062 7920 7573 696e 6720 7468 6520  y, by using the 
-00001bd0: 7374 616e 6461 7264 2070 7974 686f 6e20  standard python 
-00001be0: 6c6f 6767 696e 6720 6c69 6272 6172 7920  logging library 
-00001bf0: 6173 2069 6e20 7468 6520 6578 616d 706c  as in the exampl
-00001c00: 652c 2079 6f75 2063 616e 2063 7265 6174  e, you can creat
-00001c10: 6520 6c6f 6767 696e 6720 6861 6e64 6c65  e logging handle
-00001c20: 7273 2074 6f20 6c6f 6720 7468 6520 6461  rs to log the da
-00001c30: 7461 206f 7574 2074 6f20 616e 7920 6d65  ta out to any me
-00001c40: 6368 616e 6973 6d20 796f 7520 6368 6f6f  chanism you choo
-00001c50: 7365 2028 652e 672e 2c20 4b61 666b 612c  se (e.g., Kafka,
-00001c60: 204c 6f67 7374 6173 682c 2065 7463 2e2e   Logstash, etc..
-00001c70: 2e29 0a0a 2323 2320 4361 7061 6269 6c69  .)..### Capabili
-00001c80: 7469 6573 2064 7572 696e 6720 4150 4920  ties during API 
-00001c90: 6361 6c6c 730a 0a41 6674 6572 2077 7261  calls..After wra
-00001ca0: 7070 696e 6720 796f 7572 2065 6e64 706f  pping your endpo
-00001cb0: 696e 7420 7769 7468 2060 6d6f 6e69 746f  int with `monito
-00001cc0: 7260 2c20 796f 7520 7265 616c 6c79 2064  r`, you really d
-00001cd0: 6f6e 2774 206e 6565 6420 746f 2064 6f20  on't need to do 
-00001ce0: 616e 7974 6869 6e67 2065 6c73 652e 2057  anything else. W
-00001cf0: 6865 6e20 7573 696e 6720 6063 7265 6174  hen using `creat
-00001d00: 6560 206f 7220 6061 6372 6561 7465 6020  e` or `acreate` 
-00001d10: 6461 7461 2077 696c 6c20 6265 2074 7261  data will be tra
-00001d20: 636b 6564 2061 6e64 206d 6f6e 6974 6f72  cked and monitor
-00001d30: 696e 6720 7769 6c6c 2074 616b 6520 706c  ing will take pl
-00001d40: 6163 652e 0a0a 5468 6572 6520 6172 652c  ace...There are,
-00001d50: 2068 6f77 6576 6572 2c20 7365 7665 7261   however, severa
-00001d60: 6c20 6361 7061 6269 6c69 7469 6573 2074  l capabilities t
-00001d70: 6861 7420 6172 6520 6164 6465 6420 746f  hat are added to
-00001d80: 2074 6865 7365 2066 756e 6374 696f 6e73   these functions
-00001d90: 2e20 5370 6563 6966 6963 616c 6c79 2c20  . Specifically, 
-00001da0: 796f 7520 6361 6e20 6164 6420 7468 6520  you can add the 
-00001db0: 666f 6c6c 6f77 696e 6720 6172 6775 6d65  following argume
-00001dc0: 6e74 7320 746f 2061 6e79 2063 7265 6174  nts to any creat
-00001dd0: 6520 6361 6c6c 3a0a 2a20 4d4f 4e41 5f63  e call:.* MONA_c
-00001de0: 6f6e 7465 7874 5f69 643a 2054 6865 2075  ontext_id: The u
-00001df0: 6e69 7175 6520 6964 206f 6620 7468 6520  nique id of the 
-00001e00: 636f 6e74 6578 7420 696e 2077 6869 6368  context in which
-00001e10: 2074 6865 2063 616c 6c20 6973 206d 6164   the call is mad
-00001e20: 652e 2042 7920 7573 696e 6720 7468 6973  e. By using this
-00001e30: 2049 4420 796f 7520 6361 6e20 6578 706f   ID you can expo
-00001e40: 7274 206d 6f72 6520 6461 7461 2074 6f20  rt more data to 
-00001e50: 4d6f 6e61 2074 6f20 7468 6520 7361 6d65  Mona to the same
-00001e60: 2063 6f6e 7465 7874 2066 726f 6d20 6f74   context from ot
-00001e70: 6865 7220 706c 6163 6573 2e20 4966 206e  her places. If n
-00001e80: 6f74 2073 7570 706c 6965 642c 2074 6865  ot supplied, the
-00001e90: 2022 6964 2220 6669 656c 6420 6f66 2074   "id" field of t
-00001ea0: 6865 204f 7065 6e41 4920 456e 6470 6f69  he OpenAI Endpoi
-00001eb0: 6e74 2773 2072 6573 706f 6e73 6520 7769  nt's response wi
-00001ec0: 6c6c 2062 6520 7573 6564 2061 7320 7468  ll be used as th
-00001ed0: 6520 4d6f 6e61 2063 6f6e 7465 7874 2049  e Mona context I
-00001ee0: 4420 6175 746f 6d61 7469 6361 6c6c 792e  D automatically.
-00001ef0: 0a2a 204d 4f4e 415f 6578 706f 7274 5f74  .* MONA_export_t
-00001f00: 696d 6573 7461 6d70 3a20 4361 6e20 6265  imestamp: Can be
-00001f10: 2075 7365 6420 746f 2073 696d 756c 6174   used to simulat
-00001f20: 6520 6173 2069 6620 7468 6520 6375 7272  e as if the curr
-00001f30: 656e 7420 6361 6c6c 2077 6173 206d 6164  ent call was mad
-00001f40: 6520 696e 2061 2064 6966 6665 7265 6e74  e in a different
-00001f50: 2074 696d 652c 2061 7320 6661 7220 6173   time, as far as
-00001f60: 204d 6f6e 6120 6973 2063 6f6e 6365 726e   Mona is concern
-00001f70: 6564 2e0a 2a20 4d4f 4e41 5f61 6464 6974  ed..* MONA_addit
-00001f80: 696f 6e61 6c5f 6461 7461 3a20 4120 4a53  ional_data: A JS
-00001f90: 4f4e 2d73 6572 6961 6c69 7a61 626c 6520  ON-serializable 
-00001fa0: 6469 6374 2077 6974 6820 616e 7920 6f74  dict with any ot
-00001fb0: 6865 7220 6461 7461 2079 6f75 2077 616e  her data you wan
-00001fc0: 7420 746f 2061 6464 2074 6f20 7468 6520  t to add to the 
-00001fd0: 6d6f 6e69 746f 7269 6e67 2063 6f6e 7465  monitoring conte
-00001fe0: 7874 2e20 5468 6973 2063 6f6d 6573 2069  xt. This comes i
-00001ff0: 6e20 6861 6e64 7920 6966 2079 6f75 2077  n handy if you w
-00002000: 616e 7420 746f 2061 6464 206d 6f72 6520  ant to add more 
-00002010: 696e 666f 726d 6174 696f 6e20 746f 2074  information to t
-00002020: 6865 206d 6f6e 6974 6f72 696e 6720 636f  he monitoring co
-00002030: 6e74 6578 2074 6861 7420 6973 6e27 7420  ntex that isn't 
-00002040: 7061 7274 206f 6620 7468 6520 6261 7369  part of the basi
-00002050: 6320 4f70 656e 4149 2041 5049 2063 616c  c OpenAI API cal
-00002060: 6c20 696e 666f 726d 6174 696f 6e2e 2046  l information. F
-00002070: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
-00002080: 6f75 2061 7265 2075 7369 6e67 2061 2073  ou are using a s
-00002090: 7065 6369 6669 6320 7465 6d70 6c61 7465  pecific template
-000020a0: 2049 4420 6f72 2069 6620 7468 6973 2063   ID or if this c
-000020b0: 616c 6c20 6973 2062 6569 6e67 206d 6164  all is being mad
-000020c0: 6520 666f 7220 6120 7370 6563 6966 6963  e for a specific
-000020d0: 2063 7573 746f 6d65 7220 4944 2c20 7468   customer ID, th
-000020e0: 6573 6520 6172 6520 6669 656c 6473 2079  ese are fields y
-000020f0: 6f75 2063 616e 2061 6464 2074 6865 7265  ou can add there
-00002100: 2074 6f20 6865 6c70 2067 6574 2066 756c   to help get ful
-00002110: 6c20 636f 6e74 6578 7420 7768 656e 206d  l context when m
-00002120: 6f6e 6974 6f72 696e 6720 7769 7468 204d  onitoring with M
-00002130: 6f6e 612e 0a0a 4578 616d 706c 653a 0a60  ona...Example:.`
-00002140: 6060 7079 0a72 6573 706f 6e73 6520 3d20  ``py.response = 
-00002150: 6173 796e 6369 6f2e 7275 6e28 6d6f 6e69  asyncio.run(moni
-00002160: 746f 7265 645f 636f 6d70 6c65 7469 6f6e  tored_completion
-00002170: 2e61 6372 6561 7465 280a 2020 2020 656e  .acreate(.    en
-00002180: 6769 6e65 3d6d 6f64 656c 2c0a 2020 2020  gine=model,.    
-00002190: 7072 6f6d 7074 3d70 726f 6d70 742c 0a20  prompt=prompt,. 
-000021a0: 2020 206d 6178 5f74 6f6b 656e 733d 6d61     max_tokens=ma
-000021b0: 785f 746f 6b65 6e73 2c0a 2020 2020 6e3d  x_tokens,.    n=
-000021c0: 6e2c 0a20 2020 2074 656d 7065 7261 7475  n,.    temperatu
-000021d0: 7265 3d74 656d 7065 7261 7475 7265 2c0a  re=temperature,.
-000021e0: 2020 2020 4d4f 4e41 5f61 6464 6974 696f      MONA_additio
-000021f0: 6e61 6c5f 6461 7461 3d7b 2263 7573 746f  nal_data={"custo
-00002200: 6d65 725f 6964 223a 2022 4135 3331 3235  mer_id": "A53125
-00002210: 3122 7d2c 0a29 290a 7072 696e 7428 7265  1"},.)).print(re
-00002220: 7370 6f6e 7365 2e63 686f 6963 6573 5b30  sponse.choices[0
-00002230: 5d2e 7465 7874 290a 6060 600a 0a23 2323  ].text).```..###
-00002240: 2055 7369 6e67 204f 7065 6e41 4920 7769   Using OpenAI wi
-00002250: 7468 2052 4553 5420 6361 6c6c 7320 696e  th REST calls in
-00002260: 7374 6561 6420 6f66 204f 7065 6e41 4927  stead of OpenAI'
-00002270: 7320 5079 7468 6f6e 2063 6c69 656e 740a  s Python client.
-00002280: 496e 2073 6f6d 6520 6361 7365 7320 796f  In some cases yo
-00002290: 7520 6d61 7920 6368 6f6f 7365 2074 6f20  u may choose to 
-000022a0: 7573 6520 4f70 656e 4149 2773 2041 5049  use OpenAI's API
-000022b0: 2064 6972 6563 746c 7920 7769 7468 2052   directly with R
-000022c0: 4553 5420 6361 6c6c 7320 616e 6420 6e6f  EST calls and no
-000022d0: 7420 7573 696e 6720 4f70 656e 4149 2773  t using OpenAI's
-000022e0: 2053 444b 2e20 466f 7220 7468 6573 6520   SDK. For these 
-000022f0: 6361 7365 7320 7765 2061 6c6c 6f77 2061  cases we allow a
-00002300: 206d 6f72 6520 6469 7265 6374 2061 7070   more direct app
-00002310: 726f 6163 6820 666f 7220 6c6f 6767 696e  roach for loggin
-00002320: 6720 746f 204d 6f6e 6120 6173 2077 656c  g to Mona as wel
-00002330: 6c2c 2062 7920 7573 696e 6720 7468 6520  l, by using the 
-00002340: 2267 6574 5f72 6573 745f 6d6f 6e69 746f  "get_rest_monito
-00002350: 7222 2066 756e 6374 696f 6e2e 2053 6565  r" function. See
-00002360: 2065 7861 6d70 6c65 2062 656c 6f77 2e0a   example below..
-00002370: 0a60 6060 7079 0a23 2044 6972 6563 7420  .```py.# Direct 
-00002380: 5245 5354 2075 7361 6765 2c20 7769 7468  REST usage, with
-00002390: 6f75 7420 4f70 656e 4149 2063 6c69 656e  out OpenAI clien
-000023a0: 740a 696d 706f 7274 2072 6571 7565 7374  t.import request
-000023b0: 730a 6672 6f6d 206f 7320 696d 706f 7274  s.from os import
-000023c0: 2065 6e76 6972 6f6e 0a66 726f 6d20 6d6f   environ.from mo
-000023d0: 6e61 5f6f 7065 6e61 6920 696d 706f 7274  na_openai import
-000023e0: 2067 6574 5f72 6573 745f 6d6f 6e69 746f   get_rest_monito
-000023f0: 720a 0a0a 4d4f 4e41 5f41 5049 5f4b 4559  r...MONA_API_KEY
-00002400: 203d 2065 6e76 6972 6f6e 2e67 6574 2822   = environ.get("
-00002410: 4d4f 4e41 5f41 5049 5f4b 4559 2229 0a4d  MONA_API_KEY").M
-00002420: 4f4e 415f 5345 4352 4554 203d 2065 6e76  ONA_SECRET = env
-00002430: 6972 6f6e 2e67 6574 2822 4d4f 4e41 5f53  iron.get("MONA_S
-00002440: 4543 5245 5422 290a 4d4f 4e41 5f43 5245  ECRET").MONA_CRE
-00002450: 4453 203d 207b 0a20 2020 2022 6b65 7922  DS = {.    "key"
-00002460: 3a20 4d4f 4e41 5f41 5049 5f4b 4559 2c0a  : MONA_API_KEY,.
-00002470: 2020 2020 2273 6563 7265 7422 3a20 4d4f      "secret": MO
-00002480: 4e41 5f53 4543 5245 542c 0a7d 0a43 4f4e  NA_SECRET,.}.CON
-00002490: 5445 5854 5f43 4c41 5353 5f4e 414d 4520  TEXT_CLASS_NAME 
-000024a0: 3d20 2253 4f4d 455f 4d4f 4e49 544f 5249  = "SOME_MONITORI
-000024b0: 4e47 5f43 4f4e 5445 5854 5f4e 414d 4522  NG_CONTEXT_NAME"
-000024c0: 0a0a 2320 4765 7420 4d6f 6e61 206c 6f67  ..# Get Mona log
-000024d0: 6765 720a 6d6f 6e61 5f6c 6f67 6765 7220  ger.mona_logger 
-000024e0: 3d20 6765 745f 7265 7374 5f6d 6f6e 6974  = get_rest_monit
-000024f0: 6f72 280a 2020 2020 2243 6f6d 706c 6574  or(.    "Complet
-00002500: 696f 6e22 2c0a 2020 2020 4d4f 4e41 5f43  ion",.    MONA_C
-00002510: 5245 4453 2c0a 2020 2020 434f 4e54 4558  REDS,.    CONTEX
-00002520: 545f 434c 4153 535f 4e41 4d45 2c0a 290a  T_CLASS_NAME,.).
-00002530: 0a23 2053 6574 2075 7020 7468 6520 4150  .# Set up the AP
-00002540: 4920 656e 6470 6f69 6e74 2055 524c 2061  I endpoint URL a
-00002550: 6e64 2061 7574 6865 6e74 6963 6174 696f  nd authenticatio
-00002560: 6e20 6865 6164 6572 730a 7572 6c20 3d20  n headers.url = 
-00002570: 2268 7474 7073 3a2f 2f61 7069 2e6f 7065  "https://api.ope
-00002580: 6e61 692e 636f 6d2f 7631 2f63 6f6d 706c  nai.com/v1/compl
-00002590: 6574 696f 6e73 220a 6865 6164 6572 7320  etions".headers 
-000025a0: 3d20 7b0a 2020 2020 2243 6f6e 7465 6e74  = {.    "Content
-000025b0: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
-000025c0: 7469 6f6e 2f6a 736f 6e22 2c0a 2020 2020  tion/json",.    
-000025d0: 2241 7574 686f 7269 7a61 7469 6f6e 223a  "Authorization":
-000025e0: 2066 2242 6561 7265 7220 7b65 6e76 6972   f"Bearer {envir
-000025f0: 6f6e 2e67 6574 2827 4f50 454e 5f41 495f  on.get('OPEN_AI_
-00002600: 4b45 5927 297d 222c 0a7d 0a0a 2320 5365  KEY')}",.}..# Se
-00002610: 7420 7570 2074 6865 2072 6571 7565 7374  t up the request
-00002620: 2064 6174 610a 6461 7461 203d 207b 0a20   data.data = {. 
-00002630: 2020 2022 7072 6f6d 7074 223a 2070 726f     "prompt": pro
-00002640: 6d70 742c 0a20 2020 2022 6d61 785f 746f  mpt,.    "max_to
-00002650: 6b65 6e73 223a 206d 6178 5f74 6f6b 656e  kens": max_token
-00002660: 732c 0a20 2020 2022 7465 6d70 6572 6174  s,.    "temperat
-00002670: 7572 6522 3a20 7465 6d70 6572 6174 7572  ure": temperatur
-00002680: 652c 0a20 2020 2022 6d6f 6465 6c22 3a20  e,.    "model": 
-00002690: 6d6f 6465 6c2c 0a20 2020 2022 6e22 3a20  model,.    "n": 
-000026a0: 6e2c 0a7d 0a0a 2320 5468 6520 6c6f 675f  n,.}..# The log_
-000026b0: 7265 7175 6573 7420 6675 6e63 7469 6f6e  request function
-000026c0: 2072 6574 7572 6e73 2074 776f 206f 7468   returns two oth
-000026d0: 6572 2066 756e 6374 696f 6e20 666f 7220  er function for 
-000026e0: 6c61 7465 7220 6c6f 6767 696e 670a 2320  later logging.# 
-000026f0: 7468 6520 7265 7370 6f6e 7365 206f 7220  the response or 
-00002700: 7468 6520 6578 6365 7074 696f 6e2e 2057  the exception. W
-00002710: 6865 6e20 7765 206c 6174 6572 2064 6f20  hen we later do 
-00002720: 7468 6174 2c20 7468 6520 6c6f 6767 6572  that, the logger
-00002730: 2077 696c 6c0a 2320 6163 7475 616c 6c79   will.# actually
-00002740: 2063 616c 6375 6c61 7465 2061 6c6c 2074   calculate all t
-00002750: 6865 2072 656c 6576 616e 7420 6d65 7472  he relevant metr
-00002760: 6963 7320 616e 6420 7769 6c6c 2073 656e  ics and will sen
-00002770: 6420 7468 656d 2074 6f0a 2320 4d6f 6e61  d them to.# Mona
-00002780: 2e0a 7265 7370 6f6e 7365 5f6c 6f67 6765  ..response_logge
-00002790: 722c 2065 7863 6570 7469 6f6e 5f6c 6f67  r, exception_log
-000027a0: 6765 7220 3d20 6d6f 6e61 5f6c 6f67 6765  ger = mona_logge
-000027b0: 722e 6c6f 675f 7265 7175 6573 7428 0a20  r.log_request(. 
-000027c0: 2020 2064 6174 612c 2061 6464 6974 696f     data, additio
-000027d0: 6e61 6c5f 6461 7461 3d7b 2263 7573 746f  nal_data={"custo
-000027e0: 6d65 725f 6964 223a 2022 4135 3331 3235  mer_id": "A53125
-000027f0: 3122 7d0a 290a 0a74 7279 3a0a 2020 2020  1"}.)..try:.    
-00002800: 2320 5365 6e64 2074 6865 2072 6571 7565  # Send the reque
-00002810: 7374 2074 6f20 7468 6520 4150 490a 2020  st to the API.  
-00002820: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
-00002830: 7565 7374 732e 706f 7374 2875 726c 2c20  uests.post(url, 
-00002840: 6865 6164 6572 733d 6865 6164 6572 732c  headers=headers,
-00002850: 206a 736f 6e3d 6461 7461 290a 0a20 2020   json=data)..   
-00002860: 2023 2043 6865 636b 2066 6f72 2048 5454   # Check for HTT
-00002870: 5020 6572 726f 7273 0a20 2020 2072 6573  P errors.    res
-00002880: 706f 6e73 652e 7261 6973 655f 666f 725f  ponse.raise_for_
-00002890: 7374 6174 7573 2829 0a0a 2020 2020 2320  status()..    # 
-000028a0: 4c6f 6720 7265 7370 6f6e 7365 2074 6f20  Log response to 
-000028b0: 4d6f 6e61 0a20 2020 2072 6573 706f 6e73  Mona.    respons
-000028c0: 655f 6c6f 6767 6572 2872 6573 706f 6e73  e_logger(respons
-000028d0: 652e 6a73 6f6e 2829 290a 2020 2020 7072  e.json()).    pr
-000028e0: 696e 7428 7265 7370 6f6e 7365 2e6a 736f  int(response.jso
-000028f0: 6e28 295b 2263 686f 6963 6573 225d 5b30  n()["choices"][0
-00002900: 5d5b 2274 6578 7422 5d29 0a0a 6578 6365  ]["text"])..exce
-00002910: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00002920: 6572 723a 0a20 2020 2023 204c 6f67 2065  err:.    # Log e
-00002930: 7863 6570 7469 6f6e 2074 6f20 4d6f 6e61  xception to Mona
-00002940: 0a20 2020 2065 7863 6570 7469 6f6e 5f6c  .    exception_l
-00002950: 6f67 6765 7228 290a 6060 600a 0a23 2323  ogger().```..###
-00002960: 2053 7472 6561 6d20 7375 7070 6f72 740a   Stream support.
-00002970: 0a4f 7065 6e41 4920 616c 6c6f 7773 2072  .OpenAI allows r
-00002980: 6563 6569 7669 6e67 2072 6573 706f 6e73  eceiving respons
-00002990: 6573 2061 7320 6120 7374 7265 616d 206f  es as a stream o
-000029a0: 6620 746f 6b65 6e73 2075 7369 6e67 2074  f tokens using t
-000029b0: 6865 2022 7374 7265 616d 2220 7061 7261  he "stream" para
-000029c0: 6d65 7465 722e 2057 6865 6e20 7468 6973  meter. When this
-000029d0: 2069 7320 646f 6e65 2c20 4d6f 6e61 2077   is done, Mona w
-000029e0: 696c 6c20 636f 6c6c 6563 7420 616c 6c20  ill collect all 
-000029f0: 7468 6520 746f 6b65 6e73 2069 6e20 6d65  the tokens in me
-00002a00: 6d6f 7279 2061 6e64 2077 696c 6c20 6372  mory and will cr
-00002a10: 6561 7465 2074 6865 2061 6e61 6c79 7369  eate the analysi
-00002a20: 7320 616e 6420 6c6f 6720 6f75 7420 7468  s and log out th
-00002a30: 6520 6461 7461 2074 6865 206d 6f6d 656e  e data the momen
-00002a40: 7420 7468 6520 7374 7265 616d 2069 7320  t the stream is 
-00002a50: 6f76 6572 2e20 596f 7520 646f 6e27 7420  over. You don't 
-00002a60: 6e65 6564 2074 6f20 646f 2061 6e79 7468  need to do anyth
-00002a70: 696e 6720 746f 206d 616b 6520 7468 6973  ing to make this
-00002a80: 2068 6170 7065 6e2e 0a0a 5369 6e63 6520   happen...Since 
-00002a90: 666f 7220 7374 7265 616d 696e 6720 7265  for streaming re
-00002aa0: 7370 6f6e 7365 7320 4f70 656e 4149 2064  sponses OpenAI d
-00002ab0: 6f65 736e 2774 2073 7570 706c 7920 7468  oesn't supply th
-00002ac0: 6520 6675 6c6c 2075 7361 6765 2074 6f6b  e full usage tok
-00002ad0: 656e 7320 7375 6d6d 6172 792c 204d 6f6e  ens summary, Mon
-00002ae0: 6120 7573 6573 2074 6865 2074 696b 746f  a uses the tikto
-00002af0: 6b65 6e20 7061 636b 6167 6520 746f 2063  ken package to c
-00002b00: 616c 6375 6c61 7465 2074 6865 2074 6f6b  alculate the tok
-00002b10: 656e 7320 6f66 2074 6865 2070 726f 6d70  ens of the promp
-00002b20: 7420 616e 6420 636f 6d70 6c65 7469 6f6e  t and completion
-00002b30: 2061 6e64 206c 6f67 2074 6865 6d20 666f   and log them fo
-00002b40: 7220 6d6f 6e69 746f 7269 6e67 2e0a 0a4e  r monitoring...N
-00002b50: 4f54 453a 2053 7472 6561 6d20 6973 2063  OTE: Stream is c
-00002b60: 7572 7265 6e74 6c79 206f 6e6c 7920 7375  urrently only su
-00002b70: 7070 6f72 7465 6420 7769 7468 2053 444b  pported with SDK
-00002b80: 2075 7361 6765 2c20 616e 6420 6e6f 7420   usage, and not 
-00002b90: 7769 7468 2075 7369 6e67 2052 4553 5420  with using REST 
-00002ba0: 6469 7265 6374 6c79 2e0a 0a23 2320 4c61  directly...## La
-00002bb0: 6e67 4368 6169 6e20 7375 7070 6f72 740a  ngChain support.
-00002bc0: 0a59 6f75 2063 616e 2075 7365 2074 6865  .You can use the
-00002bd0: 2065 7870 6f72 7465 6420 606d 6f6e 6974   exported `monit
-00002be0: 6f72 5f6c 616e 6763 6861 696e 5f6c 6c6d  or_langchain_llm
-00002bf0: 6020 746f 2077 7261 7020 6120 4c61 6e67  ` to wrap a Lang
-00002c00: 4368 6169 6e20 4f70 656e 4149 204c 4c4d  Chain OpenAI LLM
-00002c10: 2028 6368 6174 206f 7220 6e6f 726d 616c   (chat or normal
-00002c20: 2920 7769 7468 204d 6f6e 6127 7320 6d6f  ) with Mona's mo
-00002c30: 6e69 746f 7269 6e67 2063 6170 6162 696c  nitoring capabil
-00002c40: 6974 6965 733a 0a0a 6060 6070 790a 6672  ities:..```py.fr
-00002c50: 6f6d 206d 6f6e 615f 6f70 656e 6169 2069  om mona_openai i
-00002c60: 6d70 6f72 7420 6d6f 6e69 746f 725f 6c61  mport monitor_la
-00002c70: 6e67 6368 6169 6e5f 6c6c 6d0a 0a66 726f  ngchain_llm..fro
-00002c80: 6d20 6c61 6e67 6368 6169 6e2e 6c6c 6d73  m langchain.llms
-00002c90: 2069 6d70 6f72 7420 4f70 656e 4149 0a0a   import OpenAI..
-00002ca0: 2320 5772 6170 2074 6865 204c 4c4d 206f  # Wrap the LLM o
-00002cb0: 626a 6563 7420 7769 7468 204d 6f6e 6120  bject with Mona 
-00002cc0: 6d6f 6e69 746f 7269 6e67 2e0a 6c6c 6d20  monitoring..llm 
-00002cd0: 3d20 6d6f 6e69 746f 725f 6c61 6e67 6368  = monitor_langch
-00002ce0: 6169 6e5f 6c6c 6d28 0a20 2020 204f 7065  ain_llm(.    Ope
-00002cf0: 6e41 4928 4f50 454e 5f41 495f 4b45 5929  nAI(OPEN_AI_KEY)
-00002d00: 2c0a 2020 2020 4d4f 4e41 5f43 5245 4453  ,.    MONA_CREDS
-00002d10: 2c0a 2020 2020 434f 4e54 4558 545f 434c  ,.    CONTEXT_CL
-00002d20: 4153 535f 4e41 4d45 290a 6060 600a 0a53  ASS_NAME).```..S
-00002d30: 6565 2066 756c 6c20 6578 616d 706c 6520  ee full example 
-00002d40: 696e 2063 6f6d 706c 6574 696f 6e5f 6c61  in completion_la
-00002d50: 6e67 6368 6169 6e2e 7079 2069 6e20 7468  ngchain.py in th
-00002d60: 6520 6578 616d 706c 6573 2066 6f6c 6465  e examples folde
-00002d70: 722e 0a0a 2323 204d 6f6e 6120 5344 4b0a  r...## Mona SDK.
-00002d80: 0a54 6869 7320 7061 636b 6167 6520 7573  .This package us
-00002d90: 6573 2074 6865 206d 6f6e 615f 7364 6b20  es the mona_sdk 
-00002da0: 7061 636b 6167 6520 746f 2065 7870 6f72  package to expor
-00002db0: 7420 7468 6520 7265 6c65 7661 6e74 2064  t the relevant d
-00002dc0: 6174 6120 746f 204d 6f6e 612e 2054 6865  ata to Mona. The
-00002dd0: 7265 2061 7265 2073 6576 6572 616c 2065  re are several e
-00002de0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00002df0: 626c 6573 2079 6f75 2063 616e 2075 7365  bles you can use
-00002e00: 2074 6f20 636f 6e66 6967 7572 6520 7468   to configure th
-00002e10: 6520 5344 4b27 7320 6265 6861 7669 6f72  e SDK's behavior
-00002e20: 2e20 466f 7220 6578 616d 706c 652c 2079  . For example, y
-00002e30: 6f75 2063 616e 2073 6574 2069 7420 7570  ou can set it up
-00002e40: 2074 6f20 7261 6973 6520 6578 6365 7074   to raise except
-00002e50: 696f 6e73 2077 6865 6e20 6578 706f 7274  ions when export
-00002e60: 696e 6720 6461 7461 2074 6f20 4d6f 6e61  ing data to Mona
-00002e70: 2066 6169 6c73 2028 6974 2064 6f65 736e   fails (it doesn
-00002e80: 2774 2064 6f20 7468 6174 2062 7920 6465  't do that by de
-00002e90: 6661 756c 7429 2e0a 0a23 2320 4d6f 6e69  fault)...## Moni
-00002ea0: 746f 7269 6e67 2066 6f72 2070 726f 6661  toring for profa
-00002eb0: 6e69 7479 0a0a 4d6f 6e61 2075 7365 7320  nity..Mona uses 
-00002ec0: 7468 6520 616c 742d 7072 6f66 616e 6974  the alt-profanit
-00002ed0: 792d 6368 6563 6b20 7061 6361 6b67 6520  y-check pacakge 
-00002ee0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00002ef0: 672f 7072 6f6a 6563 742f 616c 742d 7072  g/project/alt-pr
-00002f00: 6f66 616e 6974 792d 6368 6563 6b2f 2920  ofanity-check/) 
-00002f10: 746f 2063 7265 6174 6520 626f 7468 2062  to create both b
-00002f20: 6f6f 6c65 616e 2070 7265 6469 6374 696f  oolean predictio
-00002f30: 6e73 2061 6e64 2070 726f 6261 6269 6c74  ns and probabilt
-00002f40: 7920 7363 6f72 6573 2066 6f72 2074 6865  y scores for the
-00002f50: 2065 7869 7374 656e 6365 206f 6620 7072   existence of pr
-00002f60: 6f66 616e 6974 7920 626f 7468 2069 6e20  ofanity both in 
-00002f70: 7468 6520 7072 6f6d 7074 2061 6e64 2069  the prompt and i
-00002f80: 6e20 7468 6520 7265 7370 6f6e 7365 732e  n the responses.
-00002f90: 2057 6520 7573 6520 7468 6520 6275 696c   We use the buil
-00002fa0: 7420 696e 2070 6163 6b61 6765 206d 6574  t in package met
-00002fb0: 686f 6473 2066 6f72 2074 6861 742e 2049  hods for that. I
-00002fc0: 6620 796f 7520 7761 6e74 2c20 666f 7220  f you want, for 
-00002fd0: 6578 616d 706c 652c 2074 6f20 7573 6520  example, to use 
-00002fe0: 6120 6469 6666 6572 656e 7420 7072 6f62  a different prob
-00002ff0: 6162 696c 6974 7920 7468 7265 7368 6f6c  ability threshol
-00003000: 6420 666f 7220 7468 6520 626f 6f6c 6561  d for the boolea
-00003010: 6e20 7072 6564 6963 7469 6f6e 2c20 796f  n prediction, yo
-00003020: 7520 6361 6e20 646f 2074 6861 7420 6279  u can do that by
-00003030: 2063 6861 6e67 696e 6720 796f 7572 204d   changing your M
-00003040: 6f6e 6120 636f 6e66 6967 206f 6e20 7468  ona config on th
-00003050: 6520 4d6f 6e61 2064 6173 6862 6f61 7264  e Mona dashboard
-00003060: 2e0a                                     ..
+000004b0: 3c2f 703e 0a0a 0a55 7365 206f 6e65 206c  </p>...Use one l
+000004c0: 696e 6520 6f66 2063 6f64 6520 746f 2067  ine of code to g
+000004d0: 6574 2069 6e73 7461 6e74 206c 6976 6520  et instant live 
+000004e0: 6d6f 6e69 746f 7269 6e67 2066 6f72 2079  monitoring for y
+000004f0: 6f75 7220 4f70 656e 4149 2075 7361 6765  our OpenAI usage
+00000500: 2069 6e63 6c75 6469 6e67 3a0a 2a20 546f   including:.* To
+00000510: 6b65 6e73 2075 7361 6765 0a2a 2048 616c  kens usage.* Hal
+00000520: 6c75 6369 6e61 7469 6f6e 2061 6c65 7274  lucination alert
+00000530: 730a 2a20 5072 6f66 616e 6974 7920 616e  s.* Profanity an
+00000540: 6420 7072 6976 6163 7920 616e 616c 7973  d privacy analys
+00000550: 6573 0a2a 2042 6568 6176 696f 7261 6c20  es.* Behavioral 
+00000560: 6472 6966 7473 2061 6e64 2061 6e6f 6d61  drifts and anoma
+00000570: 6c69 6573 0a2a 204c 616e 6743 6861 696e  lies.* LangChain
+00000580: 2073 7570 706f 7274 0a2a 204d 7563 6820   support.* Much 
+00000590: 6d75 6368 206d 6f72 650a 0a23 2320 5365  much more..## Se
+000005a0: 7474 696e 6720 5570 0a0a 6060 6063 6f6e  tting Up..```con
+000005b0: 736f 6c65 0a24 2070 6970 2069 6e73 7461  sole.$ pip insta
+000005c0: 6c6c 206d 6f6e 615f 6f70 656e 6169 0a60  ll mona_openai.`
+000005d0: 6060 0a0a 2323 2051 7569 636b 2053 7461  ``..## Quick Sta
+000005e0: 7274 0a0a 596f 7520 6361 6e20 6669 6e64  rt..You can find
+000005f0: 2062 6f69 6c65 7270 6c61 7465 2063 6f64   boilerplate cod
+00000600: 6520 666f 7220 6d61 6e79 2075 7365 2063  e for many use c
+00000610: 6173 6573 2075 6e64 6572 205b 7468 6520  ases under [the 
+00000620: 2265 7861 6d70 6c65 7322 2066 6f6c 6465  "examples" folde
+00000630: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+00000640: 622e 636f 6d2f 6d6f 6e61 6c61 6273 2f6d  b.com/monalabs/m
+00000650: 6f6e 612d 6f70 656e 6169 2f74 7265 652f  ona-openai/tree/
+00000660: 6d61 696e 2f65 7861 6d70 6c65 7329 2e0a  main/examples)..
+00000670: 0a23 2323 2057 6974 6820 5374 616e 6461  .### With Standa
+00000680: 7264 204c 6f67 6769 6e67 0a0a 6060 6070  rd Logging..```p
+00000690: 790a 6672 6f6d 206f 7320 696d 706f 7274  y.from os import
+000006a0: 2065 6e76 6972 6f6e 0a69 6d70 6f72 7420   environ.import 
+000006b0: 6f70 656e 6169 0a66 726f 6d20 6d6f 6e61  openai.from mona
+000006c0: 5f6f 7065 6e61 692e 6c6f 6767 6572 7320  _openai.loggers 
+000006d0: 696d 706f 7274 2053 7461 6e64 6172 644c  import StandardL
+000006e0: 6f67 6765 720a 6672 6f6d 206c 6f67 6769  ogger.from loggi
+000006f0: 6e67 2069 6d70 6f72 7420 5741 524e 494e  ng import WARNIN
+00000700: 470a 0a66 726f 6d20 6d6f 6e61 5f6f 7065  G..from mona_ope
+00000710: 6e61 6920 696d 706f 7274 206d 6f6e 6974  nai import monit
+00000720: 6f72 5f77 6974 685f 6c6f 6767 6572 0a0a  or_with_logger..
+00000730: 6f70 656e 6169 2e61 7069 5f6b 6579 203d  openai.api_key =
+00000740: 2065 6e76 6972 6f6e 2e67 6574 2822 4f50   environ.get("OP
+00000750: 454e 5f41 495f 4b45 5922 290a 0a6d 6f6e  EN_AI_KEY")..mon
+00000760: 6974 6f72 6564 5f63 6f6d 706c 6574 696f  itored_completio
+00000770: 6e20 3d20 6d6f 6e69 746f 725f 7769 7468  n = monitor_with
+00000780: 5f6c 6f67 6765 7228 0a20 2020 206f 7065  _logger(.    ope
+00000790: 6e61 692e 436f 6d70 6c65 7469 6f6e 2c0a  nai.Completion,.
+000007a0: 2020 2020 5374 616e 6461 7264 4c6f 6767      StandardLogg
+000007b0: 6572 2857 4152 4e49 4e47 292c 0a29 0a0a  er(WARNING),.)..
+000007c0: 7265 7370 6f6e 7365 203d 206d 6f6e 6974  response = monit
+000007d0: 6f72 6564 5f63 6f6d 706c 6574 696f 6e2e  ored_completion.
+000007e0: 6372 6561 7465 280a 2020 2020 6d6f 6465  create(.    mode
+000007f0: 6c3d 2274 6578 742d 6164 612d 3030 3122  l="text-ada-001"
+00000800: 2c0a 2020 2020 7072 6f6d 7074 3d22 4920  ,.    prompt="I 
+00000810: 7761 6e74 2074 6f20 6765 6e65 7261 7465  want to generate
+00000820: 2073 6f6d 6520 7465 7874 2061 626f 7574   some text about
+00000830: 2022 2c0a 2020 2020 6d61 785f 746f 6b65   ",.    max_toke
+00000840: 6e73 3d32 302c 0a20 2020 206e 3d31 2c0a  ns=20,.    n=1,.
+00000850: 2020 2020 7465 6d70 6572 6174 7572 653d      temperature=
+00000860: 302e 322c 0a20 2020 2023 2041 6464 696e  0.2,.    # Addin
+00000870: 6720 6164 6469 7469 6f6e 616c 2069 6e66  g additional inf
+00000880: 6f72 6d61 7469 6f6e 2066 6f72 206d 6f6e  ormation for mon
+00000890: 6974 6f72 696e 6720 7075 7270 6f73 6573  itoring purposes
+000008a0: 2c20 756e 7265 6c61 7465 6420 746f 0a20  , unrelated to. 
+000008b0: 2020 2023 2069 6e74 6572 6e61 6c20 4f70     # internal Op
+000008c0: 656e 4149 2063 616c 6c2e 0a20 2020 204d  enAI call..    M
+000008d0: 4f4e 415f 6164 6469 7469 6f6e 616c 5f64  ONA_additional_d
+000008e0: 6174 613d 7b22 6375 7374 6f6d 6572 5f69  ata={"customer_i
+000008f0: 6422 3a20 2241 3533 3132 3531 227d 2c0a  d": "A531251"},.
+00000900: 290a 7072 696e 7428 7265 7370 6f6e 7365  ).print(response
+00000910: 2e63 686f 6963 6573 5b30 5d2e 7465 7874  .choices[0].text
+00000920: 290a 6060 600a 0a23 2323 2057 6974 6820  ).```..### With 
+00000930: 4d6f 6e61 0a0a 5b53 6967 6e20 7570 2066  Mona..[Sign up f
+00000940: 6f72 2061 2066 7265 6520 4d6f 6e61 2061  or a free Mona a
+00000950: 6363 6f75 6e74 2068 6572 655d 2868 7474  ccount here](htt
+00000960: 7073 3a2f 2f77 7777 2e6d 6f6e 616c 6162  ps://www.monalab
+00000970: 732e 696f 2f6f 7065 6e61 692d 6770 742d  s.io/openai-gpt-
+00000980: 6d6f 6e69 746f 7269 6e67 292e 0a0a 6060  monitoring)...``
+00000990: 6070 790a 6672 6f6d 206f 7320 696d 706f  `py.from os impo
+000009a0: 7274 2065 6e76 6972 6f6e 0a69 6d70 6f72  rt environ.impor
+000009b0: 7420 6f70 656e 6169 0a0a 6672 6f6d 206d  t openai..from m
+000009c0: 6f6e 615f 6f70 656e 6169 2069 6d70 6f72  ona_openai impor
+000009d0: 7420 6d6f 6e69 746f 720a 0a6f 7065 6e61  t monitor..opena
+000009e0: 692e 6170 695f 6b65 7920 3d20 656e 7669  i.api_key = envi
+000009f0: 726f 6e2e 6765 7428 224f 5045 4e5f 4149  ron.get("OPEN_AI
+00000a00: 5f4b 4559 2229 0a0a 4d4f 4e41 5f41 5049  _KEY")..MONA_API
+00000a10: 5f4b 4559 203d 2065 6e76 6972 6f6e 2e67  _KEY = environ.g
+00000a20: 6574 2822 4d4f 4e41 5f41 5049 5f4b 4559  et("MONA_API_KEY
+00000a30: 2229 0a4d 4f4e 415f 5345 4352 4554 203d  ").MONA_SECRET =
+00000a40: 2065 6e76 6972 6f6e 2e67 6574 2822 4d4f   environ.get("MO
+00000a50: 4e41 5f53 4543 5245 5422 290a 4d4f 4e41  NA_SECRET").MONA
+00000a60: 5f43 5245 4453 203d 207b 0a20 2020 2022  _CREDS = {.    "
+00000a70: 6b65 7922 3a20 4d4f 4e41 5f41 5049 5f4b  key": MONA_API_K
+00000a80: 4559 2c0a 2020 2020 2273 6563 7265 7422  EY,.    "secret"
+00000a90: 3a20 4d4f 4e41 5f53 4543 5245 542c 0a7d  : MONA_SECRET,.}
+00000aa0: 0a43 4f4e 5445 5854 5f43 4c41 5353 5f4e  .CONTEXT_CLASS_N
+00000ab0: 414d 4520 3d20 2253 4f4d 455f 4d4f 4e49  AME = "SOME_MONI
+00000ac0: 544f 5249 4e47 5f43 4f4e 5445 5854 5f4e  TORING_CONTEXT_N
+00000ad0: 414d 4522 0a0a 0a6d 6f6e 6974 6f72 6564  AME"...monitored
+00000ae0: 5f63 6f6d 706c 6574 696f 6e20 3d20 6d6f  _completion = mo
+00000af0: 6e69 746f 7228 0a20 2020 206f 7065 6e61  nitor(.    opena
+00000b00: 692e 436f 6d70 6c65 7469 6f6e 2c0a 2020  i.Completion,.  
+00000b10: 2020 4d4f 4e41 5f43 5245 4453 2c0a 2020    MONA_CREDS,.  
+00000b20: 2020 434f 4e54 4558 545f 434c 4153 535f    CONTEXT_CLASS_
+00000b30: 4e41 4d45 2c0a 290a 0a72 6573 706f 6e73  NAME,.)..respons
+00000b40: 6520 3d20 6d6f 6e69 746f 7265 645f 636f  e = monitored_co
+00000b50: 6d70 6c65 7469 6f6e 2e63 7265 6174 6528  mpletion.create(
+00000b60: 0a20 2020 206d 6f64 656c 3d22 7465 7874  .    model="text
+00000b70: 2d61 6461 2d30 3031 222c 0a20 2020 2070  -ada-001",.    p
+00000b80: 726f 6d70 743d 2249 2077 616e 7420 746f  rompt="I want to
+00000b90: 2067 656e 6572 6174 6520 736f 6d65 2074   generate some t
+00000ba0: 6578 7420 6162 6f75 7420 222c 0a20 2020  ext about ",.   
+00000bb0: 206d 6178 5f74 6f6b 656e 733d 3230 2c0a   max_tokens=20,.
+00000bc0: 2020 2020 6e3d 312c 0a20 2020 2074 656d      n=1,.    tem
+00000bd0: 7065 7261 7475 7265 3d30 2e32 2c0a 2020  perature=0.2,.  
+00000be0: 2020 2320 4164 6469 6e67 2061 6464 6974    # Adding addit
+00000bf0: 696f 6e61 6c20 696e 666f 726d 6174 696f  ional informatio
+00000c00: 6e20 666f 7220 6d6f 6e69 746f 7269 6e67  n for monitoring
+00000c10: 2070 7572 706f 7365 732c 2075 6e72 656c   purposes, unrel
+00000c20: 6174 6564 2074 6f0a 2020 2020 2320 696e  ated to.    # in
+00000c30: 7465 726e 616c 204f 7065 6e41 4920 6361  ternal OpenAI ca
+00000c40: 6c6c 2e0a 2020 2020 4d4f 4e41 5f61 6464  ll..    MONA_add
+00000c50: 6974 696f 6e61 6c5f 6461 7461 3d7b 2263  itional_data={"c
+00000c60: 7573 746f 6d65 725f 6964 223a 2022 4135  ustomer_id": "A5
+00000c70: 3331 3235 3122 7d2c 0a29 0a70 7269 6e74  31251"},.).print
+00000c80: 2872 6573 706f 6e73 652e 6368 6f69 6365  (response.choice
+00000c90: 735b 305d 2e74 6578 7429 0a60 6060 0a0a  s[0].text).```..
+00000ca0: 2323 2053 7570 706f 7274 6564 204f 7065  ## Supported Ope
+00000cb0: 6e41 4920 4150 4973 0a43 7572 7265 6e74  nAI APIs.Current
+00000cc0: 6c79 2074 6869 7320 636c 6965 6e74 2073  ly this client s
+00000cd0: 7570 706f 7274 7320 606f 7065 6e61 692e  upports `openai.
+00000ce0: 436f 6d70 6c65 7469 6f6e 6020 616e 6420  Completion` and 
+00000cf0: 606f 7065 6e61 692e 4368 6174 436f 6d70  `openai.ChatComp
+00000d00: 6c65 7469 6f6e 602e 204d 6f6e 6120 6361  letion`. Mona ca
+00000d10: 6e20 7375 7070 6f72 7420 7072 6f63 6573  n support proces
+00000d20: 7365 7320 6261 7365 6420 6f6e 206f 7468  ses based on oth
+00000d30: 6572 2041 5049 7320 616e 6420 616c 736f  er APIs and also
+00000d40: 206e 6f6e 2d4f 7065 6e41 492d 6261 7365   non-OpenAI-base
+00000d50: 6420 6170 7073 2e0a 4966 2079 6f75 2068  d apps..If you h
+00000d60: 6176 6520 6120 6469 6666 6572 7265 6e74  ave a differrent
+00000d70: 2075 7365 2d63 6173 652c 2077 6527 6420   use-case, we'd 
+00000d80: 6c6f 7665 2074 6f20 6865 6172 2061 626f  love to hear abo
+00000d90: 7574 2069 7421 2050 6c65 6173 6520 656d  ut it! Please em
+00000da0: 6169 6c20 7573 2061 7420 7375 7070 6f72  ail us at suppor
+00000db0: 7440 6d6f 6e61 6c61 6273 2e69 6f2e 0a0a  t@monalabs.io...
+00000dc0: 2323 2055 7361 6765 0a23 2323 2049 6e69  ## Usage.### Ini
+00000dd0: 7469 616c 697a 6174 696f 6e0a 0a54 6865  tialization..The
+00000de0: 206d 6169 6e20 616e 6420 6f6e 6c79 2066   main and only f
+00000df0: 756e 6374 696f 6e20 6578 706f 7365 6420  unction exposed 
+00000e00: 696e 2074 6869 7320 7061 636b 6167 6520  in this package 
+00000e10: 6973 2060 6d6f 6e69 746f 7260 2e0a 6060  is `monitor`..``
+00000e20: 6070 790a 696d 706f 7274 206f 7065 6e61  `py.import opena
+00000e30: 690a 0a66 726f 6d20 6d6f 6e61 5f6f 7065  i..from mona_ope
+00000e40: 6e61 6920 696d 706f 7274 206d 6f6e 6974  nai import monit
+00000e50: 6f72 0a0a 6f70 656e 6169 2e61 7069 5f6b  or..openai.api_k
+00000e60: 6579 203d 2065 6e76 6972 6f6e 2e67 6574  ey = environ.get
+00000e70: 2822 4f50 454e 5f41 495f 4b45 5922 290a  ("OPEN_AI_KEY").
+00000e80: 0a6d 6f6e 6974 6f72 6564 5f63 6f6d 706c  .monitored_compl
+00000e90: 6574 696f 6e20 3d20 6d6f 6e69 746f 7228  etion = monitor(
+00000ea0: 0a20 2020 206f 7065 6e61 692e 436f 6d70  .    openai.Comp
+00000eb0: 6c65 7469 6f6e 2c0a 2020 2020 280a 2020  letion,.    (.  
+00000ec0: 2020 2020 2020 656e 7669 726f 6e2e 6765        environ.ge
+00000ed0: 7428 224d 4f4e 415f 4150 495f 4b45 5922  t("MONA_API_KEY"
+00000ee0: 292c 0a20 2020 2020 2020 2065 6e76 6972  ),.        envir
+00000ef0: 6f6e 2e67 6574 2822 4d4f 4e41 5f53 4543  on.get("MONA_SEC
+00000f00: 5245 5422 292c 0a20 2020 2029 2c0a 2020  RET"),.    ),.  
+00000f10: 2020 2253 4f4d 455f 4d4f 4e49 544f 5249    "SOME_MONITORI
+00000f20: 4e47 5f43 4f4e 5445 5854 5f4e 414d 4522  NG_CONTEXT_NAME"
+00000f30: 2c0a 2020 2020 7b22 616e 616c 7973 6973  ,.    {"analysis
+00000f40: 223a 207b 2270 726f 6661 6e69 7479 223a  ": {"profanity":
+00000f50: 2046 616c 7365 7d7d 0a29 0a0a 2e2e 2e0a   False}}.)......
+00000f60: 0a6d 6f6e 6974 6f72 6564 5f63 6f6d 706c  .monitored_compl
+00000f70: 6574 696f 6e2e 6372 6561 7465 282e 2e2e  etion.create(...
+00000f80: 290a 6060 600a 0a54 6865 2060 6d6f 6e69  ).```..The `moni
+00000f90: 746f 7260 2066 756e 6374 696f 6e20 7265  tor` function re
+00000fa0: 7475 726e 7320 746f 2079 6f75 2061 2063  turns to you a c
+00000fb0: 6c61 7373 2074 6861 7420 7772 6170 7320  lass that wraps 
+00000fc0: 7468 6520 6f72 6967 696e 616c 206f 7065  the original ope
+00000fd0: 6e61 6920 656e 6470 6f69 6e74 2063 6c61  nai endpoint cla
+00000fe0: 7373 2079 6f75 2070 726f 7669 6465 2c20  ss you provide, 
+00000ff0: 7769 7468 2061 6e20 6571 7569 7661 6c65  with an equivale
+00001000: 6e74 2041 5049 2028 6265 7369 6465 7320  nt API (besides 
+00001010: 736f 6d65 2061 6464 6974 696f 6e73 206c  some additions l
+00001020: 6973 7465 6420 6265 6c6f 7729 2e0a 596f  isted below)..Yo
+00001030: 7520 6361 6e20 7468 656e 2075 7365 2074  u can then use t
+00001040: 6865 2072 6574 7572 6e65 6420 636c 6173  he returned clas
+00001050: 7327 2022 6372 6561 7465 2220 616e 6420  s' "create" and 
+00001060: 2261 6372 6561 7465 2220 6675 6e63 7469  "acreate" functi
+00001070: 6f6e 7320 6a75 7374 2061 7320 796f 7520  ons just as you 
+00001080: 776f 756c 6420 6265 666f 7265 2c20 6f6e  would before, on
+00001090: 6c79 206e 6f77 2c20 6265 7369 6465 7320  ly now, besides 
+000010a0: 6765 7474 696e 6720 7468 6520 7265 7175  getting the requ
+000010b0: 6573 7465 6420 6f70 656e 4149 2066 756e  ested openAI fun
+000010c0: 6374 696f 6e61 6c69 7479 2c20 7468 6973  ctionality, this
+000010d0: 2063 6c69 656e 7420 7769 6c6c 206c 6f67   client will log
+000010e0: 206f 7574 2074 6f20 4d6f 6e61 2773 2073   out to Mona's s
+000010f0: 6572 7665 7220 7468 6520 7061 7261 6d65  erver the parame
+00001100: 7465 7273 2079 6f75 2075 7365 6420 2865  ters you used (e
+00001110: 2e67 2e2c 2074 656d 7065 7261 7475 7265  .g., temperature
+00001120: 292c 2064 6174 6120 6162 6f75 7420 7468  ), data about th
+00001130: 6520 7265 7370 6f6e 7365 2066 726f 6d20  e response from 
+00001140: 4f70 656e 4149 2773 2073 6572 7665 722c  OpenAI's server,
+00001150: 2061 6e64 2063 7573 746f 6d20 616e 616c   and custom anal
+00001160: 7973 6573 2061 626f 7574 2074 6865 2063  yses about the c
+00001170: 616c 6c20 2865 2e67 2e2c 2070 726f 6661  all (e.g., profa
+00001180: 6e69 7479 2073 636f 7265 732c 2070 7269  nity scores, pri
+00001190: 7661 6379 2063 6865 636b 7320 666f 7220  vacy checks for 
+000011a0: 656d 6169 6c73 2f70 686f 6e65 206e 756d  emails/phone num
+000011b0: 6265 7273 2066 6f75 6e64 2069 6e20 7468  bers found in th
+000011c0: 6520 7465 7874 732c 2074 6578 7475 616c  e texts, textual
+000011d0: 2061 6e61 6c79 7365 732c 2065 7463 2e2e   analyses, etc..
+000011e0: 2e29 0a0a 5468 6520 606d 6f6e 6974 6f72  .)..The `monitor
+000011f0: 6020 6675 6e63 7469 6f6e 2072 6563 6569  ` function recei
+00001200: 7665 7320 7468 6520 666f 6c6c 6f77 696e  ves the followin
+00001210: 6720 6172 6775 6d65 6e74 733a 0a6f 7065  g arguments:.ope
+00001220: 6e61 695f 636c 6173 733a 2041 6e20 4f70  nai_class: An Op
+00001230: 656e 4149 2041 5049 2063 6c61 7373 2074  enAI API class t
+00001240: 6f20 7772 6170 2077 6974 6820 6d6f 6e69  o wrap with moni
+00001250: 746f 7269 6e67 2063 6170 6162 696c 7469  toring capabilti
+00001260: 6573 2e0a 6d6f 6e61 5f63 7265 6473 3a20  es..mona_creds: 
+00001270: 4120 6469 6374 2028 636f 6e74 6169 6e69  A dict (containi
+00001280: 6e67 2022 6b65 7922 2061 6e64 2022 7365  ng "key" and "se
+00001290: 6372 6574 2229 206f 7220 7061 6972 2028  cret") or pair (
+000012a0: 7475 706c 6529 206f 6620 4d6f 6e61 2041  tuple) of Mona A
+000012b0: 5049 206b 6579 2061 6e64 2073 6563 7265  PI key and secre
+000012c0: 7420 746f 2073 6574 2075 7020 4d6f 6e61  t to set up Mona
+000012d0: 2773 2063 6c69 656e 7473 2066 726f 6d20  's clients from 
+000012e0: 6974 7320 5344 4b2e 0a63 6f6e 7465 7874  its SDK..context
+000012f0: 5f63 6c61 7373 3a20 5468 6520 4d6f 6e61  _class: The Mona
+00001300: 2063 6f6e 7465 7874 2063 6c61 7373 206e   context class n
+00001310: 616d 6520 746f 2075 7365 2066 6f72 206d  ame to use for m
+00001320: 6f6e 6974 6f72 696e 672e 2055 7365 2061  onitoring. Use a
+00001330: 2063 6f6e 7374 616e 7420 6e61 6d65 206f   constant name o
+00001340: 6620 796f 7572 2063 686f 6963 652e 0a73  f your choice..s
+00001350: 7065 6373 3a20 4120 6469 6374 696f 6e61  pecs: A dictiona
+00001360: 7279 206f 6620 7370 6563 6966 6963 6174  ry of specificat
+00001370: 696f 6e73 2073 7563 6820 6173 206d 6f6e  ions such as mon
+00001380: 6974 6f72 696e 6720 7361 6d70 6c69 6e67  itoring sampling
+00001390: 2072 6174 696f 2e0a 0a23 2323 2320 5370   ratio...#### Sp
+000013a0: 6563 730a 5468 6520 7370 6563 7320 6172  ecs.The specs ar
+000013b0: 6720 616c 6c6f 7773 2079 6f75 2074 6f20  g allows you to 
+000013c0: 636f 6e66 6967 7572 6520 7768 6174 2073  configure what s
+000013d0: 686f 756c 6420 6265 206d 6f6e 6974 6f72  hould be monitor
+000013e0: 6564 2e20 4974 2065 7870 6563 7473 2061  ed. It expects a
+000013f0: 2070 7974 686f 6e20 6469 6374 2077 6974   python dict wit
+00001400: 6820 7468 6520 666f 6c6c 776f 696e 6720  h the follwoing 
+00001410: 706f 7373 6962 6c65 206b 6579 733a 0a2a  possible keys:.*
+00001420: 2073 616d 706c 696e 675f 7261 7469 6f20   sampling_ratio 
+00001430: 2831 293a 2041 206e 756d 6265 7220 6265  (1): A number be
+00001440: 7477 6565 6e20 3020 616e 6420 3120 666f  tween 0 and 1 fo
+00001450: 7220 686f 7720 6f66 7465 6e20 7368 6f75  r how often shou
+00001460: 6c64 2074 6865 2063 616c 6c20 6265 206c  ld the call be l
+00001470: 6f67 6765 642e 0a2a 2061 766f 6964 5f6d  ogged..* avoid_m
+00001480: 6f6e 6974 6f72 696e 675f 6578 6365 7074  onitoring_except
+00001490: 696f 6e73 2028 4661 6c73 6529 3a20 5768  ions (False): Wh
+000014a0: 6574 6865 7220 6f72 206e 6f74 2074 6f20  ether or not to 
+000014b0: 6c6f 6720 6f75 7420 746f 204d 6f6e 6120  log out to Mona 
+000014c0: 7768 656e 2074 6865 7265 2069 7320 616e  when there is an
+000014d0: 204f 7065 6e41 4920 6578 6365 7074 696f   OpenAI exceptio
+000014e0: 6e2e 2044 6566 6175 6c74 2069 7320 746f  n. Default is to
+000014f0: 2074 7261 636b 2065 7863 6570 7469 6f6e   track exception
+00001500: 7320 2d20 616e 6420 4d6f 6e61 2077 696c  s - and Mona wil
+00001510: 6c20 616c 6572 7420 796f 7520 6f6e 2074  l alert you on t
+00001520: 6869 6e67 7320 6c69 6b65 2061 206a 756d  hings like a jum
+00001530: 7020 696e 206e 756d 6265 7220 6f66 2065  p in number of e
+00001540: 7863 6570 7469 6f6e 730a 2a20 6578 706f  xceptions.* expo
+00001550: 7274 5f70 726f 6d70 7420 2846 616c 7365  rt_prompt (False
+00001560: 293a 2057 6865 7468 6572 204d 6f6e 6120  ): Whether Mona 
+00001570: 7368 6f75 6c64 2065 7870 6f72 7420 7468  should export th
+00001580: 6520 6163 7475 616c 2070 726f 6d70 7420  e actual prompt 
+00001590: 7465 7874 2e20 4265 2064 6566 6175 6c74  text. Be default
+000015a0: 2073 6574 2074 6f20 4661 6c73 6520 746f   set to False to
+000015b0: 2061 766f 6964 2070 7269 7661 6379 2063   avoid privacy c
+000015c0: 6f6e 6365 726e 732e 0a2a 2065 7870 6f72  oncerns..* expor
+000015d0: 745f 7265 7370 6f6e 7365 5f74 6578 7473  t_response_texts
+000015e0: 2028 4661 6c73 6529 3a20 5768 6574 6865   (False): Whethe
+000015f0: 7220 4d6f 6e61 2073 686f 756c 6420 6578  r Mona should ex
+00001600: 706f 7274 2074 6865 2061 6374 7561 6c20  port the actual 
+00001610: 7265 7370 6f6e 7365 2074 6578 7473 2e20  response texts. 
+00001620: 4265 2064 6566 6175 6c74 2073 6574 2074  Be default set t
+00001630: 6f20 4661 6c73 6520 746f 2061 766f 6964  o False to avoid
+00001640: 2070 7269 7661 6379 2063 6f6e 6365 726e   privacy concern
+00001650: 732e 0a2a 2061 6e61 6c79 7369 733a 2041  s..* analysis: A
+00001660: 2064 6963 7469 6f6e 6172 7920 6d61 7070   dictionary mapp
+00001670: 696e 6720 6561 6368 2061 6e61 6c79 7369  ing each analysi
+00001680: 7320 7479 7065 2074 6f20 6120 626f 6f6c  s type to a bool
+00001690: 6561 6e20 7661 6c75 6520 7465 6c6c 696e  ean value tellin
+000016a0: 6720 7468 6520 636c 6965 6e74 2077 6865  g the client whe
+000016b0: 7468 6572 206f 7220 6e6f 7420 746f 2072  ther or not to r
+000016c0: 756e 2073 6169 6420 616e 616c 7973 6973  un said analysis
+000016d0: 2061 6e64 206c 6f67 2069 7420 746f 204d   and log it to M
+000016e0: 6f6e 612e 2050 6f73 7369 626c 6520 6f70  ona. Possible op
+000016f0: 7469 6f6e 7320 6375 7272 656e 746c 7920  tions currently 
+00001700: 6172 6520 2270 7269 7661 6379 222c 2022  are "privacy", "
+00001710: 7072 6f66 616e 6974 7922 2c20 616e 6420  profanity", and 
+00001720: 2274 6578 7475 616c 222e 2042 7920 6465  "textual". By de
+00001730: 6661 756c 742c 2061 6c6c 2061 6e61 6c79  fault, all analy
+00001740: 7365 7320 7461 6b65 2070 6c61 6365 2061  ses take place a
+00001750: 6e64 2061 7265 206c 6f67 6765 6420 6f75  nd are logged ou
+00001760: 7420 746f 204d 6f6e 612e 0a0a 2323 2320  t to Mona...### 
+00001770: 5573 696e 6720 6375 7374 6f6d 206c 6f67  Using custom log
+00001780: 6765 7273 0a59 6f75 2064 6f6e 2774 2068  gers.You don't h
+00001790: 6176 6520 746f 2068 6176 6520 6120 4d6f  ave to have a Mo
+000017a0: 6e61 2061 6363 6f75 6e74 2074 6f20 7573  na account to us
+000017b0: 6520 7468 6973 2070 6163 6b61 6765 2e20  e this package. 
+000017c0: 596f 7520 6361 6e20 6465 6669 6e65 2073  You can define s
+000017d0: 7065 6369 6669 6320 6c6f 6767 6572 7320  pecific loggers 
+000017e0: 746f 206c 6f67 206f 7574 2074 6865 2064  to log out the d
+000017f0: 6174 6120 746f 2061 2066 696c 652c 206d  ata to a file, m
+00001800: 656d 6f72 792c 206f 7220 6a75 7374 2061  emory, or just a
+00001810: 2067 6976 656e 2070 7974 686f 6e20 6c6f   given python lo
+00001820: 6767 6572 2e20 466f 7220 6578 616d 706c  gger. For exampl
+00001830: 652c 2074 6f20 6c6f 6720 6f75 7420 7468  e, to log out th
+00001840: 6520 7265 6c65 7661 6e74 206d 6574 7269  e relevant metri
+00001850: 6373 2061 7320 5741 524e 494e 473a 0a0a  cs as WARNING:..
+00001860: 6060 6070 790a 6672 6f6d 206f 7320 696d  ```py.from os im
+00001870: 706f 7274 2065 6e76 6972 6f6e 0a69 6d70  port environ.imp
+00001880: 6f72 7420 6f70 656e 6169 0a66 726f 6d20  ort openai.from 
+00001890: 6d6f 6e61 5f6f 7065 6e61 692e 6c6f 6767  mona_openai.logg
+000018a0: 6572 7320 696d 706f 7274 2053 7461 6e64  ers import Stand
+000018b0: 6172 644c 6f67 6765 720a 6672 6f6d 206c  ardLogger.from l
+000018c0: 6f67 6769 6e67 2069 6d70 6f72 7420 5741  ogging import WA
+000018d0: 524e 494e 470a 0a66 726f 6d20 6d6f 6e61  RNING..from mona
+000018e0: 5f6f 7065 6e61 6920 696d 706f 7274 206d  _openai import m
+000018f0: 6f6e 6974 6f72 5f77 6974 685f 6c6f 6767  onitor_with_logg
+00001900: 6572 0a0a 6f70 656e 6169 2e61 7069 5f6b  er..openai.api_k
+00001910: 6579 203d 2065 6e76 6972 6f6e 2e67 6574  ey = environ.get
+00001920: 2822 4f50 454e 5f41 495f 4b45 5922 290a  ("OPEN_AI_KEY").
+00001930: 0a6d 6f6e 6974 6f72 6564 5f63 6f6d 706c  .monitored_compl
+00001940: 6574 696f 6e20 3d20 6d6f 6e69 746f 725f  etion = monitor_
+00001950: 7769 7468 5f6c 6f67 6765 7228 0a20 2020  with_logger(.   
+00001960: 206f 7065 6e61 692e 436f 6d70 6c65 7469   openai.Completi
+00001970: 6f6e 2c0a 2020 2020 5374 616e 6461 7264  on,.    Standard
+00001980: 4c6f 6767 6572 2857 4152 4e49 4e47 292c  Logger(WARNING),
+00001990: 0a29 0a0a 7265 7370 6f6e 7365 203d 206d  .)..response = m
+000019a0: 6f6e 6974 6f72 6564 5f63 6f6d 706c 6574  onitored_complet
+000019b0: 696f 6e2e 6372 6561 7465 280a 2020 2020  ion.create(.    
+000019c0: 6d6f 6465 6c3d 2274 6578 742d 6164 612d  model="text-ada-
+000019d0: 3030 3122 2c0a 2020 2020 7072 6f6d 7074  001",.    prompt
+000019e0: 3d22 4920 7761 6e74 2074 6f20 6765 6e65  ="I want to gene
+000019f0: 7261 7465 2073 6f6d 6520 7465 7874 2061  rate some text a
+00001a00: 626f 7574 2022 2c0a 2020 2020 6d61 785f  bout ",.    max_
+00001a10: 746f 6b65 6e73 3d32 302c 0a20 2020 206e  tokens=20,.    n
+00001a20: 3d31 2c0a 2020 2020 7465 6d70 6572 6174  =1,.    temperat
+00001a30: 7572 653d 302e 322c 0a20 2020 2023 2041  ure=0.2,.    # A
+00001a40: 6464 696e 6720 6164 6469 7469 6f6e 616c  dding additional
+00001a50: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f72   information for
+00001a60: 206d 6f6e 6974 6f72 696e 6720 7075 7270   monitoring purp
+00001a70: 6f73 6573 2c20 756e 7265 6c61 7465 6420  oses, unrelated 
+00001a80: 746f 0a20 2020 2023 2069 6e74 6572 6e61  to.    # interna
+00001a90: 6c20 4f70 656e 4149 2063 616c 6c2e 0a20  l OpenAI call.. 
+00001aa0: 2020 204d 4f4e 415f 6164 6469 7469 6f6e     MONA_addition
+00001ab0: 616c 5f64 6174 613d 7b22 6375 7374 6f6d  al_data={"custom
+00001ac0: 6572 5f69 6422 3a20 2241 3533 3132 3531  er_id": "A531251
+00001ad0: 227d 2c0a 290a 6060 600a 0a54 6869 7320  "},.).```..This 
+00001ae0: 5344 4b20 7072 6f76 6964 6573 2061 2073  SDK provides a s
+00001af0: 696d 706c 6520 696e 7465 7266 6163 6520  imple interface 
+00001b00: 746f 2069 6d70 6c65 6d65 6e74 2079 6f75  to implement you
+00001b10: 7220 6f77 6e20 6c6f 6767 6572 7320 6279  r own loggers by
+00001b20: 2069 6e68 6572 6974 696e 6720 6672 6f6d   inheriting from
+00001b30: 204c 6f67 6765 7220 756e 6465 7220 6c6f   Logger under lo
+00001b40: 6767 6572 732f 6c6f 6767 6572 2e70 792e  ggers/logger.py.
+00001b50: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
+00001b60: 6279 2075 7369 6e67 2074 6865 2073 7461  by using the sta
+00001b70: 6e64 6172 6420 7079 7468 6f6e 206c 6f67  ndard python log
+00001b80: 6769 6e67 206c 6962 7261 7279 2061 7320  ging library as 
+00001b90: 696e 2074 6865 2065 7861 6d70 6c65 2c20  in the example, 
+00001ba0: 796f 7520 6361 6e20 6372 6561 7465 206c  you can create l
+00001bb0: 6f67 6769 6e67 2068 616e 646c 6572 7320  ogging handlers 
+00001bc0: 746f 206c 6f67 2074 6865 2064 6174 6120  to log the data 
+00001bd0: 6f75 7420 746f 2061 6e79 206d 6563 6861  out to any mecha
+00001be0: 6e69 736d 2079 6f75 2063 686f 6f73 6520  nism you choose 
+00001bf0: 2865 2e67 2e2c 204b 6166 6b61 2c20 4c6f  (e.g., Kafka, Lo
+00001c00: 6773 7461 7368 2c20 6574 632e 2e2e 290a  gstash, etc...).
+00001c10: 0a23 2323 2043 6170 6162 696c 6974 6965  .### Capabilitie
+00001c20: 7320 6475 7269 6e67 2041 5049 2063 616c  s during API cal
+00001c30: 6c73 0a0a 4166 7465 7220 7772 6170 7069  ls..After wrappi
+00001c40: 6e67 2079 6f75 7220 656e 6470 6f69 6e74  ng your endpoint
+00001c50: 2077 6974 6820 606d 6f6e 6974 6f72 602c   with `monitor`,
+00001c60: 2079 6f75 2072 6561 6c6c 7920 646f 6e27   you really don'
+00001c70: 7420 6e65 6564 2074 6f20 646f 2061 6e79  t need to do any
+00001c80: 7468 696e 6720 656c 7365 2e20 5768 656e  thing else. When
+00001c90: 2075 7369 6e67 2060 6372 6561 7465 6020   using `create` 
+00001ca0: 6f72 2060 6163 7265 6174 6560 2064 6174  or `acreate` dat
+00001cb0: 6120 7769 6c6c 2062 6520 7472 6163 6b65  a will be tracke
+00001cc0: 6420 616e 6420 6d6f 6e69 746f 7269 6e67  d and monitoring
+00001cd0: 2077 696c 6c20 7461 6b65 2070 6c61 6365   will take place
+00001ce0: 2e0a 0a54 6865 7265 2061 7265 2c20 686f  ...There are, ho
+00001cf0: 7765 7665 722c 2073 6576 6572 616c 2063  wever, several c
+00001d00: 6170 6162 696c 6974 6965 7320 7468 6174  apabilities that
+00001d10: 2061 7265 2061 6464 6564 2074 6f20 7468   are added to th
+00001d20: 6573 6520 6675 6e63 7469 6f6e 732e 2053  ese functions. S
+00001d30: 7065 6369 6669 6361 6c6c 792c 2079 6f75  pecifically, you
+00001d40: 2063 616e 2061 6464 2074 6865 2066 6f6c   can add the fol
+00001d50: 6c6f 7769 6e67 2061 7267 756d 656e 7473  lowing arguments
+00001d60: 2074 6f20 616e 7920 6372 6561 7465 2063   to any create c
+00001d70: 616c 6c3a 0a2a 204d 4f4e 415f 636f 6e74  all:.* MONA_cont
+00001d80: 6578 745f 6964 3a20 5468 6520 756e 6971  ext_id: The uniq
+00001d90: 7565 2069 6420 6f66 2074 6865 2063 6f6e  ue id of the con
+00001da0: 7465 7874 2069 6e20 7768 6963 6820 7468  text in which th
+00001db0: 6520 6361 6c6c 2069 7320 6d61 6465 2e20  e call is made. 
+00001dc0: 4279 2075 7369 6e67 2074 6869 7320 4944  By using this ID
+00001dd0: 2079 6f75 2063 616e 2065 7870 6f72 7420   you can export 
+00001de0: 6d6f 7265 2064 6174 6120 746f 204d 6f6e  more data to Mon
+00001df0: 6120 746f 2074 6865 2073 616d 6520 636f  a to the same co
+00001e00: 6e74 6578 7420 6672 6f6d 206f 7468 6572  ntext from other
+00001e10: 2070 6c61 6365 732e 2049 6620 6e6f 7420   places. If not 
+00001e20: 7375 7070 6c69 6564 2c20 7468 6520 2269  supplied, the "i
+00001e30: 6422 2066 6965 6c64 206f 6620 7468 6520  d" field of the 
+00001e40: 4f70 656e 4149 2045 6e64 706f 696e 7427  OpenAI Endpoint'
+00001e50: 7320 7265 7370 6f6e 7365 2077 696c 6c20  s response will 
+00001e60: 6265 2075 7365 6420 6173 2074 6865 204d  be used as the M
+00001e70: 6f6e 6120 636f 6e74 6578 7420 4944 2061  ona context ID a
+00001e80: 7574 6f6d 6174 6963 616c 6c79 2e0a 2a20  utomatically..* 
+00001e90: 4d4f 4e41 5f65 7870 6f72 745f 7469 6d65  MONA_export_time
+00001ea0: 7374 616d 703a 2043 616e 2062 6520 7573  stamp: Can be us
+00001eb0: 6564 2074 6f20 7369 6d75 6c61 7465 2061  ed to simulate a
+00001ec0: 7320 6966 2074 6865 2063 7572 7265 6e74  s if the current
+00001ed0: 2063 616c 6c20 7761 7320 6d61 6465 2069   call was made i
+00001ee0: 6e20 6120 6469 6666 6572 656e 7420 7469  n a different ti
+00001ef0: 6d65 2c20 6173 2066 6172 2061 7320 4d6f  me, as far as Mo
+00001f00: 6e61 2069 7320 636f 6e63 6572 6e65 642e  na is concerned.
+00001f10: 0a2a 204d 4f4e 415f 6164 6469 7469 6f6e  .* MONA_addition
+00001f20: 616c 5f64 6174 613a 2041 204a 534f 4e2d  al_data: A JSON-
+00001f30: 7365 7269 616c 697a 6162 6c65 2064 6963  serializable dic
+00001f40: 7420 7769 7468 2061 6e79 206f 7468 6572  t with any other
+00001f50: 2064 6174 6120 796f 7520 7761 6e74 2074   data you want t
+00001f60: 6f20 6164 6420 746f 2074 6865 206d 6f6e  o add to the mon
+00001f70: 6974 6f72 696e 6720 636f 6e74 6578 742e  itoring context.
+00001f80: 2054 6869 7320 636f 6d65 7320 696e 2068   This comes in h
+00001f90: 616e 6479 2069 6620 796f 7520 7761 6e74  andy if you want
+00001fa0: 2074 6f20 6164 6420 6d6f 7265 2069 6e66   to add more inf
+00001fb0: 6f72 6d61 7469 6f6e 2074 6f20 7468 6520  ormation to the 
+00001fc0: 6d6f 6e69 746f 7269 6e67 2063 6f6e 7465  monitoring conte
+00001fd0: 7820 7468 6174 2069 736e 2774 2070 6172  x that isn't par
+00001fe0: 7420 6f66 2074 6865 2062 6173 6963 204f  t of the basic O
+00001ff0: 7065 6e41 4920 4150 4920 6361 6c6c 2069  penAI API call i
+00002000: 6e66 6f72 6d61 7469 6f6e 2e20 466f 7220  nformation. For 
+00002010: 6578 616d 706c 652c 2069 6620 796f 7520  example, if you 
+00002020: 6172 6520 7573 696e 6720 6120 7370 6563  are using a spec
+00002030: 6966 6963 2074 656d 706c 6174 6520 4944  ific template ID
+00002040: 206f 7220 6966 2074 6869 7320 6361 6c6c   or if this call
+00002050: 2069 7320 6265 696e 6720 6d61 6465 2066   is being made f
+00002060: 6f72 2061 2073 7065 6369 6669 6320 6375  or a specific cu
+00002070: 7374 6f6d 6572 2049 442c 2074 6865 7365  stomer ID, these
+00002080: 2061 7265 2066 6965 6c64 7320 796f 7520   are fields you 
+00002090: 6361 6e20 6164 6420 7468 6572 6520 746f  can add there to
+000020a0: 2068 656c 7020 6765 7420 6675 6c6c 2063   help get full c
+000020b0: 6f6e 7465 7874 2077 6865 6e20 6d6f 6e69  ontext when moni
+000020c0: 746f 7269 6e67 2077 6974 6820 4d6f 6e61  toring with Mona
+000020d0: 2e0a 0a45 7861 6d70 6c65 3a0a 6060 6070  ...Example:.```p
+000020e0: 790a 7265 7370 6f6e 7365 203d 2061 7379  y.response = asy
+000020f0: 6e63 696f 2e72 756e 286d 6f6e 6974 6f72  ncio.run(monitor
+00002100: 6564 5f63 6f6d 706c 6574 696f 6e2e 6163  ed_completion.ac
+00002110: 7265 6174 6528 0a20 2020 2065 6e67 696e  reate(.    engin
+00002120: 653d 6d6f 6465 6c2c 0a20 2020 2070 726f  e=model,.    pro
+00002130: 6d70 743d 7072 6f6d 7074 2c0a 2020 2020  mpt=prompt,.    
+00002140: 6d61 785f 746f 6b65 6e73 3d6d 6178 5f74  max_tokens=max_t
+00002150: 6f6b 656e 732c 0a20 2020 206e 3d6e 2c0a  okens,.    n=n,.
+00002160: 2020 2020 7465 6d70 6572 6174 7572 653d      temperature=
+00002170: 7465 6d70 6572 6174 7572 652c 0a20 2020  temperature,.   
+00002180: 204d 4f4e 415f 6164 6469 7469 6f6e 616c   MONA_additional
+00002190: 5f64 6174 613d 7b22 6375 7374 6f6d 6572  _data={"customer
+000021a0: 5f69 6422 3a20 2241 3533 3132 3531 227d  _id": "A531251"}
+000021b0: 2c0a 2929 0a70 7269 6e74 2872 6573 706f  ,.)).print(respo
+000021c0: 6e73 652e 6368 6f69 6365 735b 305d 2e74  nse.choices[0].t
+000021d0: 6578 7429 0a60 6060 0a0a 2323 2320 5573  ext).```..### Us
+000021e0: 696e 6720 4f70 656e 4149 2077 6974 6820  ing OpenAI with 
+000021f0: 5245 5354 2063 616c 6c73 2069 6e73 7465  REST calls inste
+00002200: 6164 206f 6620 4f70 656e 4149 2773 2050  ad of OpenAI's P
+00002210: 7974 686f 6e20 636c 6965 6e74 0a49 6e20  ython client.In 
+00002220: 736f 6d65 2063 6173 6573 2079 6f75 206d  some cases you m
+00002230: 6179 2063 686f 6f73 6520 746f 2075 7365  ay choose to use
+00002240: 204f 7065 6e41 4927 7320 4150 4920 6469   OpenAI's API di
+00002250: 7265 6374 6c79 2077 6974 6820 5245 5354  rectly with REST
+00002260: 2063 616c 6c73 2061 6e64 206e 6f74 2075   calls and not u
+00002270: 7369 6e67 204f 7065 6e41 4927 7320 5344  sing OpenAI's SD
+00002280: 4b2e 2046 6f72 2074 6865 7365 2063 6173  K. For these cas
+00002290: 6573 2077 6520 616c 6c6f 7720 6120 6d6f  es we allow a mo
+000022a0: 7265 2064 6972 6563 7420 6170 7072 6f61  re direct approa
+000022b0: 6368 2066 6f72 206c 6f67 6769 6e67 2074  ch for logging t
+000022c0: 6f20 4d6f 6e61 2061 7320 7765 6c6c 2c20  o Mona as well, 
+000022d0: 6279 2075 7369 6e67 2074 6865 2022 6765  by using the "ge
+000022e0: 745f 7265 7374 5f6d 6f6e 6974 6f72 2220  t_rest_monitor" 
+000022f0: 6675 6e63 7469 6f6e 2e20 5365 6520 6578  function. See ex
+00002300: 616d 706c 6520 6265 6c6f 772e 0a0a 6060  ample below...``
+00002310: 6070 790a 2320 4469 7265 6374 2052 4553  `py.# Direct RES
+00002320: 5420 7573 6167 652c 2077 6974 686f 7574  T usage, without
+00002330: 204f 7065 6e41 4920 636c 6965 6e74 0a69   OpenAI client.i
+00002340: 6d70 6f72 7420 7265 7175 6573 7473 0a66  mport requests.f
+00002350: 726f 6d20 6f73 2069 6d70 6f72 7420 656e  rom os import en
+00002360: 7669 726f 6e0a 6672 6f6d 206d 6f6e 615f  viron.from mona_
+00002370: 6f70 656e 6169 2069 6d70 6f72 7420 6765  openai import ge
+00002380: 745f 7265 7374 5f6d 6f6e 6974 6f72 0a0a  t_rest_monitor..
+00002390: 0a4d 4f4e 415f 4150 495f 4b45 5920 3d20  .MONA_API_KEY = 
+000023a0: 656e 7669 726f 6e2e 6765 7428 224d 4f4e  environ.get("MON
+000023b0: 415f 4150 495f 4b45 5922 290a 4d4f 4e41  A_API_KEY").MONA
+000023c0: 5f53 4543 5245 5420 3d20 656e 7669 726f  _SECRET = enviro
+000023d0: 6e2e 6765 7428 224d 4f4e 415f 5345 4352  n.get("MONA_SECR
+000023e0: 4554 2229 0a4d 4f4e 415f 4352 4544 5320  ET").MONA_CREDS 
+000023f0: 3d20 7b0a 2020 2020 226b 6579 223a 204d  = {.    "key": M
+00002400: 4f4e 415f 4150 495f 4b45 592c 0a20 2020  ONA_API_KEY,.   
+00002410: 2022 7365 6372 6574 223a 204d 4f4e 415f   "secret": MONA_
+00002420: 5345 4352 4554 2c0a 7d0a 434f 4e54 4558  SECRET,.}.CONTEX
+00002430: 545f 434c 4153 535f 4e41 4d45 203d 2022  T_CLASS_NAME = "
+00002440: 534f 4d45 5f4d 4f4e 4954 4f52 494e 475f  SOME_MONITORING_
+00002450: 434f 4e54 4558 545f 4e41 4d45 220a 0a23  CONTEXT_NAME"..#
+00002460: 2047 6574 204d 6f6e 6120 6c6f 6767 6572   Get Mona logger
+00002470: 0a6d 6f6e 615f 6c6f 6767 6572 203d 2067  .mona_logger = g
+00002480: 6574 5f72 6573 745f 6d6f 6e69 746f 7228  et_rest_monitor(
+00002490: 0a20 2020 2022 436f 6d70 6c65 7469 6f6e  .    "Completion
+000024a0: 222c 0a20 2020 204d 4f4e 415f 4352 4544  ",.    MONA_CRED
+000024b0: 532c 0a20 2020 2043 4f4e 5445 5854 5f43  S,.    CONTEXT_C
+000024c0: 4c41 5353 5f4e 414d 452c 0a29 0a0a 2320  LASS_NAME,.)..# 
+000024d0: 5365 7420 7570 2074 6865 2041 5049 2065  Set up the API e
+000024e0: 6e64 706f 696e 7420 5552 4c20 616e 6420  ndpoint URL and 
+000024f0: 6175 7468 656e 7469 6361 7469 6f6e 2068  authentication h
+00002500: 6561 6465 7273 0a75 726c 203d 2022 6874  eaders.url = "ht
+00002510: 7470 733a 2f2f 6170 692e 6f70 656e 6169  tps://api.openai
+00002520: 2e63 6f6d 2f76 312f 636f 6d70 6c65 7469  .com/v1/completi
+00002530: 6f6e 7322 0a68 6561 6465 7273 203d 207b  ons".headers = {
+00002540: 0a20 2020 2022 436f 6e74 656e 742d 5479  .    "Content-Ty
+00002550: 7065 223a 2022 6170 706c 6963 6174 696f  pe": "applicatio
+00002560: 6e2f 6a73 6f6e 222c 0a20 2020 2022 4175  n/json",.    "Au
+00002570: 7468 6f72 697a 6174 696f 6e22 3a20 6622  thorization": f"
+00002580: 4265 6172 6572 207b 656e 7669 726f 6e2e  Bearer {environ.
+00002590: 6765 7428 274f 5045 4e5f 4149 5f4b 4559  get('OPEN_AI_KEY
+000025a0: 2729 7d22 2c0a 7d0a 0a23 2053 6574 2075  ')}",.}..# Set u
+000025b0: 7020 7468 6520 7265 7175 6573 7420 6461  p the request da
+000025c0: 7461 0a64 6174 6120 3d20 7b0a 2020 2020  ta.data = {.    
+000025d0: 2270 726f 6d70 7422 3a20 7072 6f6d 7074  "prompt": prompt
+000025e0: 2c0a 2020 2020 226d 6178 5f74 6f6b 656e  ,.    "max_token
+000025f0: 7322 3a20 6d61 785f 746f 6b65 6e73 2c0a  s": max_tokens,.
+00002600: 2020 2020 2274 656d 7065 7261 7475 7265      "temperature
+00002610: 223a 2074 656d 7065 7261 7475 7265 2c0a  ": temperature,.
+00002620: 2020 2020 226d 6f64 656c 223a 206d 6f64      "model": mod
+00002630: 656c 2c0a 2020 2020 226e 223a 206e 2c0a  el,.    "n": n,.
+00002640: 7d0a 0a23 2054 6865 206c 6f67 5f72 6571  }..# The log_req
+00002650: 7565 7374 2066 756e 6374 696f 6e20 7265  uest function re
+00002660: 7475 726e 7320 7477 6f20 6f74 6865 7220  turns two other 
+00002670: 6675 6e63 7469 6f6e 2066 6f72 206c 6174  function for lat
+00002680: 6572 206c 6f67 6769 6e67 0a23 2074 6865  er logging.# the
+00002690: 2072 6573 706f 6e73 6520 6f72 2074 6865   response or the
+000026a0: 2065 7863 6570 7469 6f6e 2e20 5768 656e   exception. When
+000026b0: 2077 6520 6c61 7465 7220 646f 2074 6861   we later do tha
+000026c0: 742c 2074 6865 206c 6f67 6765 7220 7769  t, the logger wi
+000026d0: 6c6c 0a23 2061 6374 7561 6c6c 7920 6361  ll.# actually ca
+000026e0: 6c63 756c 6174 6520 616c 6c20 7468 6520  lculate all the 
+000026f0: 7265 6c65 7661 6e74 206d 6574 7269 6373  relevant metrics
+00002700: 2061 6e64 2077 696c 6c20 7365 6e64 2074   and will send t
+00002710: 6865 6d20 746f 0a23 204d 6f6e 612e 0a72  hem to.# Mona..r
+00002720: 6573 706f 6e73 655f 6c6f 6767 6572 2c20  esponse_logger, 
+00002730: 6578 6365 7074 696f 6e5f 6c6f 6767 6572  exception_logger
+00002740: 203d 206d 6f6e 615f 6c6f 6767 6572 2e6c   = mona_logger.l
+00002750: 6f67 5f72 6571 7565 7374 280a 2020 2020  og_request(.    
+00002760: 6461 7461 2c20 6164 6469 7469 6f6e 616c  data, additional
+00002770: 5f64 6174 613d 7b22 6375 7374 6f6d 6572  _data={"customer
+00002780: 5f69 6422 3a20 2241 3533 3132 3531 227d  _id": "A531251"}
+00002790: 0a29 0a0a 7472 793a 0a20 2020 2023 2053  .)..try:.    # S
+000027a0: 656e 6420 7468 6520 7265 7175 6573 7420  end the request 
+000027b0: 746f 2074 6865 2041 5049 0a20 2020 2072  to the API.    r
+000027c0: 6573 706f 6e73 6520 3d20 7265 7175 6573  esponse = reques
+000027d0: 7473 2e70 6f73 7428 7572 6c2c 2068 6561  ts.post(url, hea
+000027e0: 6465 7273 3d68 6561 6465 7273 2c20 6a73  ders=headers, js
+000027f0: 6f6e 3d64 6174 6129 0a0a 2020 2020 2320  on=data)..    # 
+00002800: 4368 6563 6b20 666f 7220 4854 5450 2065  Check for HTTP e
+00002810: 7272 6f72 730a 2020 2020 7265 7370 6f6e  rrors.    respon
+00002820: 7365 2e72 6169 7365 5f66 6f72 5f73 7461  se.raise_for_sta
+00002830: 7475 7328 290a 0a20 2020 2023 204c 6f67  tus()..    # Log
+00002840: 2072 6573 706f 6e73 6520 746f 204d 6f6e   response to Mon
+00002850: 610a 2020 2020 7265 7370 6f6e 7365 5f6c  a.    response_l
+00002860: 6f67 6765 7228 7265 7370 6f6e 7365 2e6a  ogger(response.j
+00002870: 736f 6e28 2929 0a20 2020 2070 7269 6e74  son()).    print
+00002880: 2872 6573 706f 6e73 652e 6a73 6f6e 2829  (response.json()
+00002890: 5b22 6368 6f69 6365 7322 5d5b 305d 5b22  ["choices"][0]["
+000028a0: 7465 7874 225d 290a 0a65 7863 6570 7420  text"])..except 
+000028b0: 4578 6365 7074 696f 6e20 6173 2065 7272  Exception as err
+000028c0: 3a0a 2020 2020 2320 4c6f 6720 6578 6365  :.    # Log exce
+000028d0: 7074 696f 6e20 746f 204d 6f6e 610a 2020  ption to Mona.  
+000028e0: 2020 6578 6365 7074 696f 6e5f 6c6f 6767    exception_logg
+000028f0: 6572 2829 0a60 6060 0a0a 2323 2320 5374  er().```..### St
+00002900: 7265 616d 2073 7570 706f 7274 0a0a 4f70  ream support..Op
+00002910: 656e 4149 2061 6c6c 6f77 7320 7265 6365  enAI allows rece
+00002920: 6976 696e 6720 7265 7370 6f6e 7365 7320  iving responses 
+00002930: 6173 2061 2073 7472 6561 6d20 6f66 2074  as a stream of t
+00002940: 6f6b 656e 7320 7573 696e 6720 7468 6520  okens using the 
+00002950: 2273 7472 6561 6d22 2070 6172 616d 6574  "stream" paramet
+00002960: 6572 2e20 5768 656e 2074 6869 7320 6973  er. When this is
+00002970: 2064 6f6e 652c 204d 6f6e 6120 7769 6c6c   done, Mona will
+00002980: 2063 6f6c 6c65 6374 2061 6c6c 2074 6865   collect all the
+00002990: 2074 6f6b 656e 7320 696e 206d 656d 6f72   tokens in memor
+000029a0: 7920 616e 6420 7769 6c6c 2063 7265 6174  y and will creat
+000029b0: 6520 7468 6520 616e 616c 7973 6973 2061  e the analysis a
+000029c0: 6e64 206c 6f67 206f 7574 2074 6865 2064  nd log out the d
+000029d0: 6174 6120 7468 6520 6d6f 6d65 6e74 2074  ata the moment t
+000029e0: 6865 2073 7472 6561 6d20 6973 206f 7665  he stream is ove
+000029f0: 722e 2059 6f75 2064 6f6e 2774 206e 6565  r. You don't nee
+00002a00: 6420 746f 2064 6f20 616e 7974 6869 6e67  d to do anything
+00002a10: 2074 6f20 6d61 6b65 2074 6869 7320 6861   to make this ha
+00002a20: 7070 656e 2e0a 0a53 696e 6365 2066 6f72  ppen...Since for
+00002a30: 2073 7472 6561 6d69 6e67 2072 6573 706f   streaming respo
+00002a40: 6e73 6573 204f 7065 6e41 4920 646f 6573  nses OpenAI does
+00002a50: 6e27 7420 7375 7070 6c79 2074 6865 2066  n't supply the f
+00002a60: 756c 6c20 7573 6167 6520 746f 6b65 6e73  ull usage tokens
+00002a70: 2073 756d 6d61 7279 2c20 4d6f 6e61 2075   summary, Mona u
+00002a80: 7365 7320 7468 6520 7469 6b74 6f6b 656e  ses the tiktoken
+00002a90: 2070 6163 6b61 6765 2074 6f20 6361 6c63   package to calc
+00002aa0: 756c 6174 6520 7468 6520 746f 6b65 6e73  ulate the tokens
+00002ab0: 206f 6620 7468 6520 7072 6f6d 7074 2061   of the prompt a
+00002ac0: 6e64 2063 6f6d 706c 6574 696f 6e20 616e  nd completion an
+00002ad0: 6420 6c6f 6720 7468 656d 2066 6f72 206d  d log them for m
+00002ae0: 6f6e 6974 6f72 696e 672e 0a0a 4e4f 5445  onitoring...NOTE
+00002af0: 3a20 5374 7265 616d 2069 7320 6375 7272  : Stream is curr
+00002b00: 656e 746c 7920 6f6e 6c79 2073 7570 706f  ently only suppo
+00002b10: 7274 6564 2077 6974 6820 5344 4b20 7573  rted with SDK us
+00002b20: 6167 652c 2061 6e64 206e 6f74 2077 6974  age, and not wit
+00002b30: 6820 7573 696e 6720 5245 5354 2064 6972  h using REST dir
+00002b40: 6563 746c 792e 0a0a 2323 204c 616e 6743  ectly...## LangC
+00002b50: 6861 696e 2073 7570 706f 7274 0a0a 596f  hain support..Yo
+00002b60: 7520 6361 6e20 7573 6520 7468 6520 6578  u can use the ex
+00002b70: 706f 7274 6564 2060 6d6f 6e69 746f 725f  ported `monitor_
+00002b80: 6c61 6e67 6368 6169 6e5f 6c6c 6d60 2074  langchain_llm` t
+00002b90: 6f20 7772 6170 2061 204c 616e 6743 6861  o wrap a LangCha
+00002ba0: 696e 204f 7065 6e41 4920 4c4c 4d20 2863  in OpenAI LLM (c
+00002bb0: 6861 7420 6f72 206e 6f72 6d61 6c29 2077  hat or normal) w
+00002bc0: 6974 6820 4d6f 6e61 2773 206d 6f6e 6974  ith Mona's monit
+00002bd0: 6f72 696e 6720 6361 7061 6269 6c69 7469  oring capabiliti
+00002be0: 6573 3a0a 0a60 6060 7079 0a66 726f 6d20  es:..```py.from 
+00002bf0: 6d6f 6e61 5f6f 7065 6e61 6920 696d 706f  mona_openai impo
+00002c00: 7274 206d 6f6e 6974 6f72 5f6c 616e 6763  rt monitor_langc
+00002c10: 6861 696e 5f6c 6c6d 0a0a 6672 6f6d 206c  hain_llm..from l
+00002c20: 616e 6763 6861 696e 2e6c 6c6d 7320 696d  angchain.llms im
+00002c30: 706f 7274 204f 7065 6e41 490a 0a23 2057  port OpenAI..# W
+00002c40: 7261 7020 7468 6520 4c4c 4d20 6f62 6a65  rap the LLM obje
+00002c50: 6374 2077 6974 6820 4d6f 6e61 206d 6f6e  ct with Mona mon
+00002c60: 6974 6f72 696e 672e 0a6c 6c6d 203d 206d  itoring..llm = m
+00002c70: 6f6e 6974 6f72 5f6c 616e 6763 6861 696e  onitor_langchain
+00002c80: 5f6c 6c6d 280a 2020 2020 4f70 656e 4149  _llm(.    OpenAI
+00002c90: 284f 5045 4e5f 4149 5f4b 4559 292c 0a20  (OPEN_AI_KEY),. 
+00002ca0: 2020 204d 4f4e 415f 4352 4544 532c 0a20     MONA_CREDS,. 
+00002cb0: 2020 2043 4f4e 5445 5854 5f43 4c41 5353     CONTEXT_CLASS
+00002cc0: 5f4e 414d 4529 0a60 6060 0a0a 5365 6520  _NAME).```..See 
+00002cd0: 6675 6c6c 2065 7861 6d70 6c65 2069 6e20  full example in 
+00002ce0: 636f 6d70 6c65 7469 6f6e 5f6c 616e 6763  completion_langc
+00002cf0: 6861 696e 2e70 7920 696e 2074 6865 2065  hain.py in the e
+00002d00: 7861 6d70 6c65 7320 666f 6c64 6572 2e0a  xamples folder..
+00002d10: 0a23 2320 4d6f 6e61 2053 444b 0a0a 5468  .## Mona SDK..Th
+00002d20: 6973 2070 6163 6b61 6765 2075 7365 7320  is package uses 
+00002d30: 7468 6520 6d6f 6e61 5f73 646b 2070 6163  the mona_sdk pac
+00002d40: 6b61 6765 2074 6f20 6578 706f 7274 2074  kage to export t
+00002d50: 6865 2072 656c 6576 616e 7420 6461 7461  he relevant data
+00002d60: 2074 6f20 4d6f 6e61 2e20 5468 6572 6520   to Mona. There 
+00002d70: 6172 6520 7365 7665 7261 6c20 656e 7669  are several envi
+00002d80: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00002d90: 7320 796f 7520 6361 6e20 7573 6520 746f  s you can use to
+00002da0: 2063 6f6e 6669 6775 7265 2074 6865 2053   configure the S
+00002db0: 444b 2773 2062 6568 6176 696f 722e 2046  DK's behavior. F
+00002dc0: 6f72 2065 7861 6d70 6c65 2c20 796f 7520  or example, you 
+00002dd0: 6361 6e20 7365 7420 6974 2075 7020 746f  can set it up to
+00002de0: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
+00002df0: 7320 7768 656e 2065 7870 6f72 7469 6e67  s when exporting
+00002e00: 2064 6174 6120 746f 204d 6f6e 6120 6661   data to Mona fa
+00002e10: 696c 7320 2869 7420 646f 6573 6e27 7420  ils (it doesn't 
+00002e20: 646f 2074 6861 7420 6279 2064 6566 6175  do that by defau
+00002e30: 6c74 292e 0a0a 2323 204d 6f6e 6974 6f72  lt)...## Monitor
+00002e40: 696e 6720 666f 7220 7072 6f66 616e 6974  ing for profanit
+00002e50: 790a 0a4d 6f6e 6120 7573 6573 2074 6865  y..Mona uses the
+00002e60: 2061 6c74 2d70 726f 6661 6e69 7479 2d63   alt-profanity-c
+00002e70: 6865 636b 2070 6163 616b 6765 2028 6874  heck pacakge (ht
+00002e80: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00002e90: 726f 6a65 6374 2f61 6c74 2d70 726f 6661  roject/alt-profa
+00002ea0: 6e69 7479 2d63 6865 636b 2f29 2074 6f20  nity-check/) to 
+00002eb0: 6372 6561 7465 2062 6f74 6820 626f 6f6c  create both bool
+00002ec0: 6561 6e20 7072 6564 6963 7469 6f6e 7320  ean predictions 
+00002ed0: 616e 6420 7072 6f62 6162 696c 7479 2073  and probabilty s
+00002ee0: 636f 7265 7320 666f 7220 7468 6520 6578  cores for the ex
+00002ef0: 6973 7465 6e63 6520 6f66 2070 726f 6661  istence of profa
+00002f00: 6e69 7479 2062 6f74 6820 696e 2074 6865  nity both in the
+00002f10: 2070 726f 6d70 7420 616e 6420 696e 2074   prompt and in t
+00002f20: 6865 2072 6573 706f 6e73 6573 2e20 5765  he responses. We
+00002f30: 2075 7365 2074 6865 2062 7569 6c74 2069   use the built i
+00002f40: 6e20 7061 636b 6167 6520 6d65 7468 6f64  n package method
+00002f50: 7320 666f 7220 7468 6174 2e20 4966 2079  s for that. If y
+00002f60: 6f75 2077 616e 742c 2066 6f72 2065 7861  ou want, for exa
+00002f70: 6d70 6c65 2c20 746f 2075 7365 2061 2064  mple, to use a d
+00002f80: 6966 6665 7265 6e74 2070 726f 6261 6269  ifferent probabi
+00002f90: 6c69 7479 2074 6872 6573 686f 6c64 2066  lity threshold f
+00002fa0: 6f72 2074 6865 2062 6f6f 6c65 616e 2070  or the boolean p
+00002fb0: 7265 6469 6374 696f 6e2c 2079 6f75 2063  rediction, you c
+00002fc0: 616e 2064 6f20 7468 6174 2062 7920 6368  an do that by ch
+00002fd0: 616e 6769 6e67 2079 6f75 7220 4d6f 6e61  anging your Mona
+00002fe0: 2063 6f6e 6669 6720 6f6e 2074 6865 204d   config on the M
+00002ff0: 6f6e 6120 6461 7368 626f 6172 642e 0a0a  ona dashboard...
+00003000: 2323 2055 7369 6e67 206e 6573 742d 6173  ## Using nest-as
+00003010: 796e 6369 6f0a 0a49 6e20 656e 7669 726f  yncio..In enviro
+00003020: 6e6d 656e 7473 2069 6e20 7768 6963 6820  nments in which 
+00003030: 7468 6572 6527 7320 6120 666f 7265 7665  there's a foreve
+00003040: 7220 7275 6e6e 696e 6720 6576 656e 7420  r running event 
+00003050: 6c6f 6f70 2028 652e 672e 2c20 4a75 7079  loop (e.g., Jupy
+00003060: 7465 7220 6e6f 7465 626f 6f6b 7329 2c20  ter notebooks), 
+00003070: 7468 6520 636c 6965 6e74 206d 6967 6874  the client might
+00003080: 2075 7365 205b 6e65 7374 5f61 7379 6e63   use [nest_async
+00003090: 696f 2e61 7070 6c79 2829 5d28 6874 7470  io.apply()](http
+000030a0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000030b0: 6a65 6374 2f6e 6573 742d 6173 796e 6369  ject/nest-asynci
+000030c0: 6f2f 2920 746f 2072 756e 206a 6f69 6e74  o/) to run joint
+000030d0: 2073 796e 6320 616e 6420 6173 796e 6320   sync and async 
+000030e0: 636f 6465 2e0a                           code..
```

### Comparing `mona-openai-0.1.0/README.md` & `mona-openai-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,706 +32,715 @@
 000001f0: 746f 6e3d 3126 616d 703b 696d 6167 655f  ton=1&amp;image_
 00000200: 706c 6179 5f62 7574 746f 6e5f 636f 6c6f  play_button_colo
 00000210: 723d 3636 6337 6431 6530 2220 7769 6474  r=66c7d1e0" widt
 00000220: 683d 2234 3030 2220 6865 6967 6874 3d22  h="400" height="
 00000230: 3232 3522 2073 7479 6c65 3d22 7769 6474  225" style="widt
 00000240: 683a 2034 3030 7078 3b20 6865 6967 6874  h: 400px; height
 00000250: 3a20 3232 3570 783b 223e 3c2f 613e 3c2f  : 225px;"></a></
-00000260: 703e 3c70 2061 6c69 676e 3d22 6365 6e74  p><p align="cent
-00000270: 6572 223e 3c61 2068 7265 663d 2268 7474  er"><a href="htt
-00000280: 7073 3a2f 2f6d 6f6e 616c 6162 732e 7769  ps://monalabs.wi
-00000290: 7374 6961 2e63 6f6d 2f6d 6564 6961 732f  stia.com/medias/
-000002a0: 6c36 786d 646a 3363 6436 3f77 7669 6465  l6xmdj3cd6?wvide
-000002b0: 6f3d 6c36 786d 646a 3363 6436 223e 4f70  o=l6xmdj3cd6">Op
-000002c0: 656e 4149 2047 5054 2049 6e74 6567 7261  enAI GPT Integra
-000002d0: 7469 6f6e 2054 7574 6f72 6961 6c3c 2f61  tion Tutorial</a
-000002e0: 3e3c 2f70 3e0a 0a0a 5573 6520 6f6e 6520  ></p>...Use one 
-000002f0: 6c69 6e65 206f 6620 636f 6465 2074 6f20  line of code to 
-00000300: 6765 7420 696e 7374 616e 7420 6c69 7665  get instant live
-00000310: 206d 6f6e 6974 6f72 696e 6720 666f 7220   monitoring for 
-00000320: 796f 7572 204f 7065 6e41 4920 7573 6167  your OpenAI usag
-00000330: 6520 696e 636c 7564 696e 673a 0a2a 2054  e including:.* T
-00000340: 6f6b 656e 7320 7573 6167 650a 2a20 4861  okens usage.* Ha
-00000350: 6c6c 7563 696e 6174 696f 6e20 616c 6572  llucination aler
-00000360: 7473 0a2a 2050 726f 6661 6e69 7479 2061  ts.* Profanity a
-00000370: 6e64 2070 7269 7661 6379 2061 6e61 6c79  nd privacy analy
-00000380: 7365 730a 2a20 4265 6861 7669 6f72 616c  ses.* Behavioral
-00000390: 2064 7269 6674 7320 616e 6420 616e 6f6d   drifts and anom
-000003a0: 616c 6965 730a 2a20 4c61 6e67 4368 6169  alies.* LangChai
-000003b0: 6e20 7375 7070 6f72 740a 2a20 4d75 6368  n support.* Much
-000003c0: 206d 7563 6820 6d6f 7265 0a0a 2323 2053   much more..## S
-000003d0: 6574 7469 6e67 2055 700a 0a60 6060 636f  etting Up..```co
-000003e0: 6e73 6f6c 650a 2420 7069 7020 696e 7374  nsole.$ pip inst
-000003f0: 616c 6c20 6d6f 6e61 5f6f 7065 6e61 690a  all mona_openai.
-00000400: 6060 600a 0a49 6620 796f 7520 706c 616e  ```..If you plan
-00000410: 206f 6e20 7573 696e 6720 4d6f 6e61 2061   on using Mona a
-00000420: 7320 796f 7572 206d 6f6e 6974 6f72 696e  s your monitorin
-00000430: 6720 7365 7276 6963 652c 205b 7369 676e  g service, [sign
-00000440: 2075 7020 666f 7220 6120 6672 6565 2061   up for a free a
-00000450: 6363 6f75 6e74 2068 6572 655d 2868 7474  ccount here](htt
-00000460: 7073 3a2f 2f77 7777 2e6d 6f6e 616c 6162  ps://www.monalab
-00000470: 732e 696f 2f6f 7065 6e61 692d 6770 742d  s.io/openai-gpt-
-00000480: 6d6f 6e69 746f 7269 6e67 292e 0a0a 2323  monitoring)...##
-00000490: 2051 7569 636b 2053 7461 7274 0a0a 596f   Quick Start..Yo
-000004a0: 7520 6361 6e20 6669 6e64 2062 6f69 6c65  u can find boile
-000004b0: 7270 6c61 7465 2063 6f64 6520 666f 7220  rplate code for 
-000004c0: 6d61 6e79 2075 7365 2d63 6173 6573 2075  many use-cases u
-000004d0: 6e64 6572 205b 7468 6520 2265 7861 6d70  nder [the "examp
-000004e0: 6c65 7322 2066 6f6c 6465 725d 2868 7474  les" folder](htt
-000004f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000500: 6d6f 6e61 6c61 6273 2f6d 6f6e 612d 6f70  monalabs/mona-op
-00000510: 656e 6169 2f74 7265 652f 6d61 696e 2f65  enai/tree/main/e
-00000520: 7861 6d70 6c65 7329 2e0a 0a60 6060 7079  xamples)...```py
-00000530: 0a66 726f 6d20 6f73 2069 6d70 6f72 7420  .from os import 
-00000540: 656e 7669 726f 6e0a 696d 706f 7274 2061  environ.import a
-00000550: 7379 6e63 696f 0a69 6d70 6f72 7420 6f70  syncio.import op
-00000560: 656e 6169 0a66 726f 6d20 6d6f 6e61 5f6f  enai.from mona_o
-00000570: 7065 6e61 692e 6c6f 6767 6572 7320 696d  penai.loggers im
-00000580: 706f 7274 2053 7461 6e64 6172 644c 6f67  port StandardLog
-00000590: 6765 720a 6672 6f6d 206c 6f67 6769 6e67  ger.from logging
-000005a0: 2069 6d70 6f72 7420 5741 524e 494e 470a   import WARNING.
-000005b0: 0a66 726f 6d20 6d6f 6e61 5f6f 7065 6e61  .from mona_opena
-000005c0: 6920 696d 706f 7274 206d 6f6e 6974 6f72  i import monitor
-000005d0: 2c20 6d6f 6e69 746f 725f 7769 7468 5f6c  , monitor_with_l
-000005e0: 6f67 6765 720a 0a6f 7065 6e61 692e 6170  ogger..openai.ap
-000005f0: 695f 6b65 7920 3d20 656e 7669 726f 6e2e  i_key = environ.
-00000600: 6765 7428 224f 5045 4e5f 4149 5f4b 4559  get("OPEN_AI_KEY
-00000610: 2229 0a0a 2320 5768 656e 2075 7369 6e67  ")..# When using
-00000620: 2061 2073 7461 6e64 6172 6420 6c6f 6767   a standard logg
-00000630: 6572 2e0a 0a6d 6f6e 6974 6f72 6564 5f63  er...monitored_c
-00000640: 6f6d 706c 6574 696f 6e20 3d20 6d6f 6e69  ompletion = moni
-00000650: 746f 725f 7769 7468 5f6c 6f67 6765 7228  tor_with_logger(
-00000660: 0a20 2020 206f 7065 6e61 692e 436f 6d70  .    openai.Comp
-00000670: 6c65 7469 6f6e 2c0a 2020 2020 5374 616e  letion,.    Stan
-00000680: 6461 7264 4c6f 6767 6572 2857 4152 4e49  dardLogger(WARNI
-00000690: 4e47 292c 0a29 0a0a 7265 7370 6f6e 7365  NG),.)..response
-000006a0: 203d 206d 6f6e 6974 6f72 6564 5f63 6f6d   = monitored_com
-000006b0: 706c 6574 696f 6e2e 6372 6561 7465 280a  pletion.create(.
-000006c0: 2020 2020 6d6f 6465 6c3d 2274 6578 742d      model="text-
-000006d0: 6164 612d 3030 3122 2c0a 2020 2020 7072  ada-001",.    pr
-000006e0: 6f6d 7074 3d22 4920 7761 6e74 2074 6f20  ompt="I want to 
-000006f0: 6765 6e65 7261 7465 2073 6f6d 6520 7465  generate some te
-00000700: 7874 2061 626f 7574 2022 2c0a 2020 2020  xt about ",.    
-00000710: 6d61 785f 746f 6b65 6e73 3d32 302c 0a20  max_tokens=20,. 
-00000720: 2020 206e 3d31 2c0a 2020 2020 7465 6d70     n=1,.    temp
-00000730: 6572 6174 7572 653d 302e 322c 0a20 2020  erature=0.2,.   
-00000740: 2023 2041 6464 696e 6720 6164 6469 7469   # Adding additi
-00000750: 6f6e 616c 2069 6e66 6f72 6d61 7469 6f6e  onal information
-00000760: 2066 6f72 206d 6f6e 6974 6f72 696e 6720   for monitoring 
-00000770: 7075 7270 6f73 6573 2c20 756e 7265 6c61  purposes, unrela
-00000780: 7465 6420 746f 0a20 2020 2023 2069 6e74  ted to.    # int
-00000790: 6572 6e61 6c20 4f70 656e 4149 2063 616c  ernal OpenAI cal
-000007a0: 6c2e 0a20 2020 204d 4f4e 415f 6164 6469  l..    MONA_addi
-000007b0: 7469 6f6e 616c 5f64 6174 613d 7b22 6375  tional_data={"cu
-000007c0: 7374 6f6d 6572 5f69 6422 3a20 2241 3533  stomer_id": "A53
-000007d0: 3132 3531 227d 2c0a 290a 7072 696e 7428  1251"},.).print(
-000007e0: 7265 7370 6f6e 7365 2e63 686f 6963 6573  response.choices
-000007f0: 5b30 5d2e 7465 7874 290a 0a0a 2320 5768  [0].text)...# Wh
-00000800: 656e 206d 6f6e 6974 6f72 696e 6720 7769  en monitoring wi
-00000810: 7468 204d 6f6e 612e 0a0a 4d4f 4e41 5f41  th Mona...MONA_A
-00000820: 5049 5f4b 4559 203d 2065 6e76 6972 6f6e  PI_KEY = environ
-00000830: 2e67 6574 2822 4d4f 4e41 5f41 5049 5f4b  .get("MONA_API_K
-00000840: 4559 2229 0a4d 4f4e 415f 5345 4352 4554  EY").MONA_SECRET
-00000850: 203d 2065 6e76 6972 6f6e 2e67 6574 2822   = environ.get("
-00000860: 4d4f 4e41 5f53 4543 5245 5422 290a 4d4f  MONA_SECRET").MO
-00000870: 4e41 5f43 5245 4453 203d 207b 0a20 2020  NA_CREDS = {.   
-00000880: 2022 6b65 7922 3a20 4d4f 4e41 5f41 5049   "key": MONA_API
-00000890: 5f4b 4559 2c0a 2020 2020 2273 6563 7265  _KEY,.    "secre
-000008a0: 7422 3a20 4d4f 4e41 5f53 4543 5245 542c  t": MONA_SECRET,
-000008b0: 0a7d 0a43 4f4e 5445 5854 5f43 4c41 5353  .}.CONTEXT_CLASS
-000008c0: 5f4e 414d 4520 3d20 2253 4f4d 455f 4d4f  _NAME = "SOME_MO
-000008d0: 4e49 544f 5249 4e47 5f43 4f4e 5445 5854  NITORING_CONTEXT
-000008e0: 5f4e 414d 4522 0a0a 0a6d 6f6e 6974 6f72  _NAME"...monitor
-000008f0: 6564 5f63 6f6d 706c 6574 696f 6e20 3d20  ed_completion = 
-00000900: 6d6f 6e69 746f 7228 0a20 2020 206f 7065  monitor(.    ope
-00000910: 6e61 692e 436f 6d70 6c65 7469 6f6e 2c0a  nai.Completion,.
-00000920: 2020 2020 4d4f 4e41 5f43 5245 4453 2c0a      MONA_CREDS,.
-00000930: 2020 2020 434f 4e54 4558 545f 434c 4153      CONTEXT_CLAS
-00000940: 535f 4e41 4d45 2c0a 290a 0a72 6573 706f  S_NAME,.)..respo
-00000950: 6e73 6520 3d20 6d6f 6e69 746f 7265 645f  nse = monitored_
-00000960: 636f 6d70 6c65 7469 6f6e 2e63 7265 6174  completion.creat
-00000970: 6528 0a20 2020 206d 6f64 656c 3d22 7465  e(.    model="te
-00000980: 7874 2d61 6461 2d30 3031 222c 0a20 2020  xt-ada-001",.   
-00000990: 2070 726f 6d70 743d 2249 2077 616e 7420   prompt="I want 
-000009a0: 746f 2067 656e 6572 6174 6520 736f 6d65  to generate some
-000009b0: 2074 6578 7420 6162 6f75 7420 222c 0a20   text about ",. 
-000009c0: 2020 206d 6178 5f74 6f6b 656e 733d 3230     max_tokens=20
-000009d0: 2c0a 2020 2020 6e3d 312c 0a20 2020 2074  ,.    n=1,.    t
-000009e0: 656d 7065 7261 7475 7265 3d30 2e32 2c0a  emperature=0.2,.
-000009f0: 2020 2020 2320 4164 6469 6e67 2061 6464      # Adding add
-00000a00: 6974 696f 6e61 6c20 696e 666f 726d 6174  itional informat
-00000a10: 696f 6e20 666f 7220 6d6f 6e69 746f 7269  ion for monitori
-00000a20: 6e67 2070 7572 706f 7365 732c 2075 6e72  ng purposes, unr
-00000a30: 656c 6174 6564 2074 6f0a 2020 2020 2320  elated to.    # 
-00000a40: 696e 7465 726e 616c 204f 7065 6e41 4920  internal OpenAI 
-00000a50: 6361 6c6c 2e0a 2020 2020 4d4f 4e41 5f61  call..    MONA_a
-00000a60: 6464 6974 696f 6e61 6c5f 6461 7461 3d7b  dditional_data={
-00000a70: 2263 7573 746f 6d65 725f 6964 223a 2022  "customer_id": "
-00000a80: 4135 3331 3235 3122 7d2c 0a29 0a70 7269  A531251"},.).pri
-00000a90: 6e74 2872 6573 706f 6e73 652e 6368 6f69  nt(response.choi
-00000aa0: 6365 735b 305d 2e74 6578 7429 0a60 6060  ces[0].text).```
-00000ab0: 0a23 2320 5375 7070 6f72 7465 6420 4f70  .## Supported Op
-00000ac0: 656e 4149 2041 5049 730a 4375 7272 656e  enAI APIs.Curren
-00000ad0: 746c 7920 7468 6973 2063 6c69 656e 7420  tly this client 
-00000ae0: 7375 7070 6f72 7473 2060 6f70 656e 6169  supports `openai
-00000af0: 2e43 6f6d 706c 6574 696f 6e60 2061 6e64  .Completion` and
-00000b00: 2060 6f70 656e 6169 2e43 6861 7443 6f6d   `openai.ChatCom
-00000b10: 706c 6574 696f 6e60 2e20 4d6f 6e61 2063  pletion`. Mona c
-00000b20: 616e 2073 7570 706f 7274 2070 726f 6365  an support proce
-00000b30: 7373 6573 2062 6173 6564 206f 6e20 6f74  sses based on ot
-00000b40: 6865 7220 4150 4973 2061 6e64 2061 6c73  her APIs and als
-00000b50: 6f20 6e6f 6e2d 4f70 656e 4149 2d62 6173  o non-OpenAI-bas
-00000b60: 6564 2061 7070 732e 0a49 6620 796f 7520  ed apps..If you 
-00000b70: 6861 7665 2061 2064 6966 6665 7272 656e  have a differren
-00000b80: 7420 7573 652d 6361 7365 2c20 7765 2764  t use-case, we'd
-00000b90: 206c 6f76 6520 746f 2068 6561 7220 6162   love to hear ab
-00000ba0: 6f75 7420 6974 2120 506c 6561 7365 2065  out it! Please e
-00000bb0: 6d61 696c 2075 7320 6174 2073 7570 706f  mail us at suppo
-00000bc0: 7274 406d 6f6e 616c 6162 732e 696f 2e0a  rt@monalabs.io..
-00000bd0: 0a23 2320 5573 6167 650a 2323 2320 496e  .## Usage.### In
-00000be0: 6974 6961 6c69 7a61 7469 6f6e 0a0a 5468  itialization..Th
-00000bf0: 6520 6d61 696e 2061 6e64 206f 6e6c 7920  e main and only 
-00000c00: 6675 6e63 7469 6f6e 2065 7870 6f73 6564  function exposed
-00000c10: 2069 6e20 7468 6973 2070 6163 6b61 6765   in this package
-00000c20: 2069 7320 606d 6f6e 6974 6f72 602e 0a60   is `monitor`..`
-00000c30: 6060 7079 0a69 6d70 6f72 7420 6f70 656e  ``py.import open
-00000c40: 6169 0a0a 6672 6f6d 206d 6f6e 615f 6f70  ai..from mona_op
-00000c50: 656e 6169 2069 6d70 6f72 7420 6d6f 6e69  enai import moni
-00000c60: 746f 720a 0a6f 7065 6e61 692e 6170 695f  tor..openai.api_
-00000c70: 6b65 7920 3d20 656e 7669 726f 6e2e 6765  key = environ.ge
-00000c80: 7428 224f 5045 4e5f 4149 5f4b 4559 2229  t("OPEN_AI_KEY")
-00000c90: 0a0a 6d6f 6e69 746f 7265 645f 636f 6d70  ..monitored_comp
-00000ca0: 6c65 7469 6f6e 203d 206d 6f6e 6974 6f72  letion = monitor
-00000cb0: 280a 2020 2020 6f70 656e 6169 2e43 6f6d  (.    openai.Com
-00000cc0: 706c 6574 696f 6e2c 0a20 2020 2028 0a20  pletion,.    (. 
-00000cd0: 2020 2020 2020 2065 6e76 6972 6f6e 2e67         environ.g
-00000ce0: 6574 2822 4d4f 4e41 5f41 5049 5f4b 4559  et("MONA_API_KEY
-00000cf0: 2229 2c0a 2020 2020 2020 2020 656e 7669  "),.        envi
-00000d00: 726f 6e2e 6765 7428 224d 4f4e 415f 5345  ron.get("MONA_SE
-00000d10: 4352 4554 2229 2c0a 2020 2020 292c 0a20  CRET"),.    ),. 
-00000d20: 2020 2022 534f 4d45 5f4d 4f4e 4954 4f52     "SOME_MONITOR
-00000d30: 494e 475f 434f 4e54 4558 545f 4e41 4d45  ING_CONTEXT_NAME
-00000d40: 222c 0a20 2020 207b 2261 6e61 6c79 7369  ",.    {"analysi
-00000d50: 7322 3a20 7b22 7072 6f66 616e 6974 7922  s": {"profanity"
-00000d60: 3a20 4661 6c73 657d 7d0a 290a 0a2e 2e2e  : False}}.).....
-00000d70: 0a0a 6d6f 6e69 746f 7265 645f 636f 6d70  ..monitored_comp
-00000d80: 6c65 7469 6f6e 2e63 7265 6174 6528 2e2e  letion.create(..
-00000d90: 2e29 0a60 6060 0a0a 5468 6520 606d 6f6e  .).```..The `mon
-00000da0: 6974 6f72 6020 6675 6e63 7469 6f6e 2072  itor` function r
-00000db0: 6574 7572 6e73 2074 6f20 796f 7520 6120  eturns to you a 
-00000dc0: 636c 6173 7320 7468 6174 2077 7261 7073  class that wraps
-00000dd0: 2074 6865 206f 7269 6769 6e61 6c20 6f70   the original op
-00000de0: 656e 6169 2065 6e64 706f 696e 7420 636c  enai endpoint cl
-00000df0: 6173 7320 796f 7520 7072 6f76 6964 652c  ass you provide,
-00000e00: 2077 6974 6820 616e 2065 7175 6976 616c   with an equival
-00000e10: 656e 7420 4150 4920 2862 6573 6964 6573  ent API (besides
-00000e20: 2073 6f6d 6520 6164 6469 7469 6f6e 7320   some additions 
-00000e30: 6c69 7374 6564 2062 656c 6f77 292e 0a59  listed below)..Y
-00000e40: 6f75 2063 616e 2074 6865 6e20 7573 6520  ou can then use 
-00000e50: 7468 6520 7265 7475 726e 6564 2063 6c61  the returned cla
-00000e60: 7373 2720 2263 7265 6174 6522 2061 6e64  ss' "create" and
-00000e70: 2022 6163 7265 6174 6522 2066 756e 6374   "acreate" funct
-00000e80: 696f 6e73 206a 7573 7420 6173 2079 6f75  ions just as you
-00000e90: 2077 6f75 6c64 2062 6566 6f72 652c 206f   would before, o
-00000ea0: 6e6c 7920 6e6f 772c 2062 6573 6964 6573  nly now, besides
-00000eb0: 2067 6574 7469 6e67 2074 6865 2072 6571   getting the req
-00000ec0: 7565 7374 6564 206f 7065 6e41 4920 6675  uested openAI fu
-00000ed0: 6e63 7469 6f6e 616c 6974 792c 2074 6869  nctionality, thi
-00000ee0: 7320 636c 6965 6e74 2077 696c 6c20 6c6f  s client will lo
-00000ef0: 6720 6f75 7420 746f 204d 6f6e 6127 7320  g out to Mona's 
-00000f00: 7365 7276 6572 2074 6865 2070 6172 616d  server the param
-00000f10: 6574 6572 7320 796f 7520 7573 6564 2028  eters you used (
-00000f20: 652e 672e 2c20 7465 6d70 6572 6174 7572  e.g., temperatur
-00000f30: 6529 2c20 6461 7461 2061 626f 7574 2074  e), data about t
-00000f40: 6865 2072 6573 706f 6e73 6520 6672 6f6d  he response from
-00000f50: 204f 7065 6e41 4927 7320 7365 7276 6572   OpenAI's server
-00000f60: 2c20 616e 6420 6375 7374 6f6d 2061 6e61  , and custom ana
-00000f70: 6c79 7365 7320 6162 6f75 7420 7468 6520  lyses about the 
-00000f80: 6361 6c6c 2028 652e 672e 2c20 7072 6f66  call (e.g., prof
-00000f90: 616e 6974 7920 7363 6f72 6573 2c20 7072  anity scores, pr
-00000fa0: 6976 6163 7920 6368 6563 6b73 2066 6f72  ivacy checks for
-00000fb0: 2065 6d61 696c 732f 7068 6f6e 6520 6e75   emails/phone nu
-00000fc0: 6d62 6572 7320 666f 756e 6420 696e 2074  mbers found in t
-00000fd0: 6865 2074 6578 7473 2c20 7465 7874 7561  he texts, textua
-00000fe0: 6c20 616e 616c 7973 6573 2c20 6574 632e  l analyses, etc.
-00000ff0: 2e2e 290a 0a54 6865 2060 6d6f 6e69 746f  ..)..The `monito
-00001000: 7260 2066 756e 6374 696f 6e20 7265 6365  r` function rece
-00001010: 6976 6573 2074 6865 2066 6f6c 6c6f 7769  ives the followi
-00001020: 6e67 2061 7267 756d 656e 7473 3a0a 6f70  ng arguments:.op
-00001030: 656e 6169 5f63 6c61 7373 3a20 416e 204f  enai_class: An O
-00001040: 7065 6e41 4920 4150 4920 636c 6173 7320  penAI API class 
-00001050: 746f 2077 7261 7020 7769 7468 206d 6f6e  to wrap with mon
-00001060: 6974 6f72 696e 6720 6361 7061 6269 6c74  itoring capabilt
-00001070: 6965 732e 0a6d 6f6e 615f 6372 6564 733a  ies..mona_creds:
-00001080: 2041 2064 6963 7420 2863 6f6e 7461 696e   A dict (contain
-00001090: 696e 6720 226b 6579 2220 616e 6420 2273  ing "key" and "s
-000010a0: 6563 7265 7422 2920 6f72 2070 6169 7220  ecret") or pair 
-000010b0: 2874 7570 6c65 2920 6f66 204d 6f6e 6120  (tuple) of Mona 
-000010c0: 4150 4920 6b65 7920 616e 6420 7365 6372  API key and secr
-000010d0: 6574 2074 6f20 7365 7420 7570 204d 6f6e  et to set up Mon
-000010e0: 6127 7320 636c 6965 6e74 7320 6672 6f6d  a's clients from
-000010f0: 2069 7473 2053 444b 2e0a 636f 6e74 6578   its SDK..contex
-00001100: 745f 636c 6173 733a 2054 6865 204d 6f6e  t_class: The Mon
-00001110: 6120 636f 6e74 6578 7420 636c 6173 7320  a context class 
-00001120: 6e61 6d65 2074 6f20 7573 6520 666f 7220  name to use for 
-00001130: 6d6f 6e69 746f 7269 6e67 2e20 5573 6520  monitoring. Use 
-00001140: 6120 636f 6e73 7461 6e74 206e 616d 6520  a constant name 
-00001150: 6f66 2079 6f75 7220 6368 6f69 6365 2e0a  of your choice..
-00001160: 7370 6563 733a 2041 2064 6963 7469 6f6e  specs: A diction
-00001170: 6172 7920 6f66 2073 7065 6369 6669 6361  ary of specifica
-00001180: 7469 6f6e 7320 7375 6368 2061 7320 6d6f  tions such as mo
-00001190: 6e69 746f 7269 6e67 2073 616d 706c 696e  nitoring samplin
-000011a0: 6720 7261 7469 6f2e 0a0a 2323 2323 2053  g ratio...#### S
-000011b0: 7065 6373 0a54 6865 2073 7065 6373 2061  pecs.The specs a
-000011c0: 7267 2061 6c6c 6f77 7320 796f 7520 746f  rg allows you to
-000011d0: 2063 6f6e 6669 6775 7265 2077 6861 7420   configure what 
-000011e0: 7368 6f75 6c64 2062 6520 6d6f 6e69 746f  should be monito
-000011f0: 7265 642e 2049 7420 6578 7065 6374 7320  red. It expects 
-00001200: 6120 7079 7468 6f6e 2064 6963 7420 7769  a python dict wi
-00001210: 7468 2074 6865 2066 6f6c 6c77 6f69 6e67  th the follwoing
-00001220: 2070 6f73 7369 626c 6520 6b65 7973 3a0a   possible keys:.
-00001230: 2a20 7361 6d70 6c69 6e67 5f72 6174 696f  * sampling_ratio
-00001240: 2028 3129 3a20 4120 6e75 6d62 6572 2062   (1): A number b
-00001250: 6574 7765 656e 2030 2061 6e64 2031 2066  etween 0 and 1 f
-00001260: 6f72 2068 6f77 206f 6674 656e 2073 686f  or how often sho
-00001270: 756c 6420 7468 6520 6361 6c6c 2062 6520  uld the call be 
-00001280: 6c6f 6767 6564 2e0a 2a20 6176 6f69 645f  logged..* avoid_
-00001290: 6d6f 6e69 746f 7269 6e67 5f65 7863 6570  monitoring_excep
-000012a0: 7469 6f6e 7320 2846 616c 7365 293a 2057  tions (False): W
-000012b0: 6865 7468 6572 206f 7220 6e6f 7420 746f  hether or not to
-000012c0: 206c 6f67 206f 7574 2074 6f20 4d6f 6e61   log out to Mona
-000012d0: 2077 6865 6e20 7468 6572 6520 6973 2061   when there is a
-000012e0: 6e20 4f70 656e 4149 2065 7863 6570 7469  n OpenAI excepti
-000012f0: 6f6e 2e20 4465 6661 756c 7420 6973 2074  on. Default is t
-00001300: 6f20 7472 6163 6b20 6578 6365 7074 696f  o track exceptio
-00001310: 6e73 202d 2061 6e64 204d 6f6e 6120 7769  ns - and Mona wi
-00001320: 6c6c 2061 6c65 7274 2079 6f75 206f 6e20  ll alert you on 
-00001330: 7468 696e 6773 206c 696b 6520 6120 6a75  things like a ju
-00001340: 6d70 2069 6e20 6e75 6d62 6572 206f 6620  mp in number of 
-00001350: 6578 6365 7074 696f 6e73 0a2a 2065 7870  exceptions.* exp
-00001360: 6f72 745f 7072 6f6d 7074 2028 4661 6c73  ort_prompt (Fals
-00001370: 6529 3a20 5768 6574 6865 7220 4d6f 6e61  e): Whether Mona
-00001380: 2073 686f 756c 6420 6578 706f 7274 2074   should export t
-00001390: 6865 2061 6374 7561 6c20 7072 6f6d 7074  he actual prompt
-000013a0: 2074 6578 742e 2042 6520 6465 6661 756c   text. Be defaul
-000013b0: 7420 7365 7420 746f 2046 616c 7365 2074  t set to False t
-000013c0: 6f20 6176 6f69 6420 7072 6976 6163 7920  o avoid privacy 
-000013d0: 636f 6e63 6572 6e73 2e0a 2a20 6578 706f  concerns..* expo
-000013e0: 7274 5f72 6573 706f 6e73 655f 7465 7874  rt_response_text
-000013f0: 7320 2846 616c 7365 293a 2057 6865 7468  s (False): Wheth
-00001400: 6572 204d 6f6e 6120 7368 6f75 6c64 2065  er Mona should e
-00001410: 7870 6f72 7420 7468 6520 6163 7475 616c  xport the actual
-00001420: 2072 6573 706f 6e73 6520 7465 7874 732e   response texts.
-00001430: 2042 6520 6465 6661 756c 7420 7365 7420   Be default set 
-00001440: 746f 2046 616c 7365 2074 6f20 6176 6f69  to False to avoi
-00001450: 6420 7072 6976 6163 7920 636f 6e63 6572  d privacy concer
-00001460: 6e73 2e0a 2a20 616e 616c 7973 6973 3a20  ns..* analysis: 
-00001470: 4120 6469 6374 696f 6e61 7279 206d 6170  A dictionary map
-00001480: 7069 6e67 2065 6163 6820 616e 616c 7973  ping each analys
-00001490: 6973 2074 7970 6520 746f 2061 2062 6f6f  is type to a boo
-000014a0: 6c65 616e 2076 616c 7565 2074 656c 6c69  lean value telli
-000014b0: 6e67 2074 6865 2063 6c69 656e 7420 7768  ng the client wh
-000014c0: 6574 6865 7220 6f72 206e 6f74 2074 6f20  ether or not to 
-000014d0: 7275 6e20 7361 6964 2061 6e61 6c79 7369  run said analysi
-000014e0: 7320 616e 6420 6c6f 6720 6974 2074 6f20  s and log it to 
-000014f0: 4d6f 6e61 2e20 506f 7373 6962 6c65 206f  Mona. Possible o
-00001500: 7074 696f 6e73 2063 7572 7265 6e74 6c79  ptions currently
-00001510: 2061 7265 2022 7072 6976 6163 7922 2c20   are "privacy", 
-00001520: 2270 726f 6661 6e69 7479 222c 2061 6e64  "profanity", and
-00001530: 2022 7465 7874 7561 6c22 2e20 4279 2064   "textual". By d
-00001540: 6566 6175 6c74 2c20 616c 6c20 616e 616c  efault, all anal
-00001550: 7973 6573 2074 616b 6520 706c 6163 6520  yses take place 
-00001560: 616e 6420 6172 6520 6c6f 6767 6564 206f  and are logged o
-00001570: 7574 2074 6f20 4d6f 6e61 2e0a 0a23 2323  ut to Mona...###
-00001580: 2055 7369 6e67 2063 7573 746f 6d20 6c6f   Using custom lo
-00001590: 6767 6572 730a 596f 7520 646f 6e27 7420  ggers.You don't 
-000015a0: 6861 7665 2074 6f20 6861 7665 2061 204d  have to have a M
-000015b0: 6f6e 6120 6163 636f 756e 7420 746f 2075  ona account to u
-000015c0: 7365 2074 6869 7320 7061 636b 6167 652e  se this package.
-000015d0: 2059 6f75 2063 616e 2064 6566 696e 6520   You can define 
-000015e0: 7370 6563 6966 6963 206c 6f67 6765 7273  specific loggers
-000015f0: 2074 6f20 6c6f 6720 6f75 7420 7468 6520   to log out the 
-00001600: 6461 7461 2074 6f20 6120 6669 6c65 2c20  data to a file, 
-00001610: 6d65 6d6f 7279 2c20 6f72 206a 7573 7420  memory, or just 
-00001620: 6120 6769 7665 6e20 7079 7468 6f6e 206c  a given python l
-00001630: 6f67 6765 722e 2046 6f72 2065 7861 6d70  ogger. For examp
-00001640: 6c65 2c20 746f 206c 6f67 206f 7574 2074  le, to log out t
-00001650: 6865 2072 656c 6576 616e 7420 6d65 7472  he relevant metr
-00001660: 6963 7320 6173 2057 4152 4e49 4e47 3a0a  ics as WARNING:.
-00001670: 0a60 6060 7079 0a66 726f 6d20 6f73 2069  .```py.from os i
-00001680: 6d70 6f72 7420 656e 7669 726f 6e0a 696d  mport environ.im
-00001690: 706f 7274 206f 7065 6e61 690a 6672 6f6d  port openai.from
-000016a0: 206d 6f6e 615f 6f70 656e 6169 2e6c 6f67   mona_openai.log
-000016b0: 6765 7273 2069 6d70 6f72 7420 5374 616e  gers import Stan
-000016c0: 6461 7264 4c6f 6767 6572 0a66 726f 6d20  dardLogger.from 
-000016d0: 6c6f 6767 696e 6720 696d 706f 7274 2057  logging import W
-000016e0: 4152 4e49 4e47 0a0a 6672 6f6d 206d 6f6e  ARNING..from mon
-000016f0: 615f 6f70 656e 6169 2069 6d70 6f72 7420  a_openai import 
-00001700: 6d6f 6e69 746f 725f 7769 7468 5f6c 6f67  monitor_with_log
-00001710: 6765 720a 0a6f 7065 6e61 692e 6170 695f  ger..openai.api_
-00001720: 6b65 7920 3d20 656e 7669 726f 6e2e 6765  key = environ.ge
-00001730: 7428 224f 5045 4e5f 4149 5f4b 4559 2229  t("OPEN_AI_KEY")
-00001740: 0a0a 6d6f 6e69 746f 7265 645f 636f 6d70  ..monitored_comp
-00001750: 6c65 7469 6f6e 203d 206d 6f6e 6974 6f72  letion = monitor
-00001760: 5f77 6974 685f 6c6f 6767 6572 280a 2020  _with_logger(.  
-00001770: 2020 6f70 656e 6169 2e43 6f6d 706c 6574    openai.Complet
-00001780: 696f 6e2c 0a20 2020 2053 7461 6e64 6172  ion,.    Standar
-00001790: 644c 6f67 6765 7228 5741 524e 494e 4729  dLogger(WARNING)
-000017a0: 2c0a 290a 0a72 6573 706f 6e73 6520 3d20  ,.)..response = 
-000017b0: 6d6f 6e69 746f 7265 645f 636f 6d70 6c65  monitored_comple
-000017c0: 7469 6f6e 2e63 7265 6174 6528 0a20 2020  tion.create(.   
-000017d0: 206d 6f64 656c 3d22 7465 7874 2d61 6461   model="text-ada
-000017e0: 2d30 3031 222c 0a20 2020 2070 726f 6d70  -001",.    promp
-000017f0: 743d 2249 2077 616e 7420 746f 2067 656e  t="I want to gen
-00001800: 6572 6174 6520 736f 6d65 2074 6578 7420  erate some text 
-00001810: 6162 6f75 7420 222c 0a20 2020 206d 6178  about ",.    max
-00001820: 5f74 6f6b 656e 733d 3230 2c0a 2020 2020  _tokens=20,.    
-00001830: 6e3d 312c 0a20 2020 2074 656d 7065 7261  n=1,.    tempera
-00001840: 7475 7265 3d30 2e32 2c0a 2020 2020 2320  ture=0.2,.    # 
-00001850: 4164 6469 6e67 2061 6464 6974 696f 6e61  Adding additiona
-00001860: 6c20 696e 666f 726d 6174 696f 6e20 666f  l information fo
-00001870: 7220 6d6f 6e69 746f 7269 6e67 2070 7572  r monitoring pur
-00001880: 706f 7365 732c 2075 6e72 656c 6174 6564  poses, unrelated
-00001890: 2074 6f0a 2020 2020 2320 696e 7465 726e   to.    # intern
-000018a0: 616c 204f 7065 6e41 4920 6361 6c6c 2e0a  al OpenAI call..
-000018b0: 2020 2020 4d4f 4e41 5f61 6464 6974 696f      MONA_additio
-000018c0: 6e61 6c5f 6461 7461 3d7b 2263 7573 746f  nal_data={"custo
-000018d0: 6d65 725f 6964 223a 2022 4135 3331 3235  mer_id": "A53125
-000018e0: 3122 7d2c 0a29 0a60 6060 0a0a 5468 6973  1"},.).```..This
-000018f0: 2053 444b 2070 726f 7669 6465 7320 6120   SDK provides a 
-00001900: 7369 6d70 6c65 2069 6e74 6572 6661 6365  simple interface
-00001910: 2074 6f20 696d 706c 656d 656e 7420 796f   to implement yo
-00001920: 7572 206f 776e 206c 6f67 6765 7273 2062  ur own loggers b
-00001930: 7920 696e 6865 7269 7469 6e67 2066 726f  y inheriting fro
-00001940: 6d20 4c6f 6767 6572 2075 6e64 6572 206c  m Logger under l
-00001950: 6f67 6765 7273 2f6c 6f67 6765 722e 7079  oggers/logger.py
-00001960: 2e0a 416c 7465 726e 6174 6976 656c 792c  ..Alternatively,
-00001970: 2062 7920 7573 696e 6720 7468 6520 7374   by using the st
-00001980: 616e 6461 7264 2070 7974 686f 6e20 6c6f  andard python lo
-00001990: 6767 696e 6720 6c69 6272 6172 7920 6173  gging library as
-000019a0: 2069 6e20 7468 6520 6578 616d 706c 652c   in the example,
-000019b0: 2079 6f75 2063 616e 2063 7265 6174 6520   you can create 
-000019c0: 6c6f 6767 696e 6720 6861 6e64 6c65 7273  logging handlers
-000019d0: 2074 6f20 6c6f 6720 7468 6520 6461 7461   to log the data
-000019e0: 206f 7574 2074 6f20 616e 7920 6d65 6368   out to any mech
-000019f0: 616e 6973 6d20 796f 7520 6368 6f6f 7365  anism you choose
-00001a00: 2028 652e 672e 2c20 4b61 666b 612c 204c   (e.g., Kafka, L
-00001a10: 6f67 7374 6173 682c 2065 7463 2e2e 2e29  ogstash, etc...)
-00001a20: 0a0a 2323 2320 4361 7061 6269 6c69 7469  ..### Capabiliti
-00001a30: 6573 2064 7572 696e 6720 4150 4920 6361  es during API ca
-00001a40: 6c6c 730a 0a41 6674 6572 2077 7261 7070  lls..After wrapp
-00001a50: 696e 6720 796f 7572 2065 6e64 706f 696e  ing your endpoin
-00001a60: 7420 7769 7468 2060 6d6f 6e69 746f 7260  t with `monitor`
-00001a70: 2c20 796f 7520 7265 616c 6c79 2064 6f6e  , you really don
-00001a80: 2774 206e 6565 6420 746f 2064 6f20 616e  't need to do an
-00001a90: 7974 6869 6e67 2065 6c73 652e 2057 6865  ything else. Whe
-00001aa0: 6e20 7573 696e 6720 6063 7265 6174 6560  n using `create`
-00001ab0: 206f 7220 6061 6372 6561 7465 6020 6461   or `acreate` da
-00001ac0: 7461 2077 696c 6c20 6265 2074 7261 636b  ta will be track
-00001ad0: 6564 2061 6e64 206d 6f6e 6974 6f72 696e  ed and monitorin
-00001ae0: 6720 7769 6c6c 2074 616b 6520 706c 6163  g will take plac
-00001af0: 652e 0a0a 5468 6572 6520 6172 652c 2068  e...There are, h
-00001b00: 6f77 6576 6572 2c20 7365 7665 7261 6c20  owever, several 
-00001b10: 6361 7061 6269 6c69 7469 6573 2074 6861  capabilities tha
-00001b20: 7420 6172 6520 6164 6465 6420 746f 2074  t are added to t
-00001b30: 6865 7365 2066 756e 6374 696f 6e73 2e20  hese functions. 
-00001b40: 5370 6563 6966 6963 616c 6c79 2c20 796f  Specifically, yo
-00001b50: 7520 6361 6e20 6164 6420 7468 6520 666f  u can add the fo
-00001b60: 6c6c 6f77 696e 6720 6172 6775 6d65 6e74  llowing argument
-00001b70: 7320 746f 2061 6e79 2063 7265 6174 6520  s to any create 
-00001b80: 6361 6c6c 3a0a 2a20 4d4f 4e41 5f63 6f6e  call:.* MONA_con
-00001b90: 7465 7874 5f69 643a 2054 6865 2075 6e69  text_id: The uni
-00001ba0: 7175 6520 6964 206f 6620 7468 6520 636f  que id of the co
-00001bb0: 6e74 6578 7420 696e 2077 6869 6368 2074  ntext in which t
-00001bc0: 6865 2063 616c 6c20 6973 206d 6164 652e  he call is made.
-00001bd0: 2042 7920 7573 696e 6720 7468 6973 2049   By using this I
-00001be0: 4420 796f 7520 6361 6e20 6578 706f 7274  D you can export
-00001bf0: 206d 6f72 6520 6461 7461 2074 6f20 4d6f   more data to Mo
-00001c00: 6e61 2074 6f20 7468 6520 7361 6d65 2063  na to the same c
-00001c10: 6f6e 7465 7874 2066 726f 6d20 6f74 6865  ontext from othe
-00001c20: 7220 706c 6163 6573 2e20 4966 206e 6f74  r places. If not
-00001c30: 2073 7570 706c 6965 642c 2074 6865 2022   supplied, the "
-00001c40: 6964 2220 6669 656c 6420 6f66 2074 6865  id" field of the
-00001c50: 204f 7065 6e41 4920 456e 6470 6f69 6e74   OpenAI Endpoint
-00001c60: 2773 2072 6573 706f 6e73 6520 7769 6c6c  's response will
-00001c70: 2062 6520 7573 6564 2061 7320 7468 6520   be used as the 
-00001c80: 4d6f 6e61 2063 6f6e 7465 7874 2049 4420  Mona context ID 
-00001c90: 6175 746f 6d61 7469 6361 6c6c 792e 0a2a  automatically..*
-00001ca0: 204d 4f4e 415f 6578 706f 7274 5f74 696d   MONA_export_tim
-00001cb0: 6573 7461 6d70 3a20 4361 6e20 6265 2075  estamp: Can be u
-00001cc0: 7365 6420 746f 2073 696d 756c 6174 6520  sed to simulate 
-00001cd0: 6173 2069 6620 7468 6520 6375 7272 656e  as if the curren
-00001ce0: 7420 6361 6c6c 2077 6173 206d 6164 6520  t call was made 
-00001cf0: 696e 2061 2064 6966 6665 7265 6e74 2074  in a different t
-00001d00: 696d 652c 2061 7320 6661 7220 6173 204d  ime, as far as M
-00001d10: 6f6e 6120 6973 2063 6f6e 6365 726e 6564  ona is concerned
-00001d20: 2e0a 2a20 4d4f 4e41 5f61 6464 6974 696f  ..* MONA_additio
-00001d30: 6e61 6c5f 6461 7461 3a20 4120 4a53 4f4e  nal_data: A JSON
-00001d40: 2d73 6572 6961 6c69 7a61 626c 6520 6469  -serializable di
-00001d50: 6374 2077 6974 6820 616e 7920 6f74 6865  ct with any othe
-00001d60: 7220 6461 7461 2079 6f75 2077 616e 7420  r data you want 
-00001d70: 746f 2061 6464 2074 6f20 7468 6520 6d6f  to add to the mo
-00001d80: 6e69 746f 7269 6e67 2063 6f6e 7465 7874  nitoring context
-00001d90: 2e20 5468 6973 2063 6f6d 6573 2069 6e20  . This comes in 
-00001da0: 6861 6e64 7920 6966 2079 6f75 2077 616e  handy if you wan
-00001db0: 7420 746f 2061 6464 206d 6f72 6520 696e  t to add more in
-00001dc0: 666f 726d 6174 696f 6e20 746f 2074 6865  formation to the
-00001dd0: 206d 6f6e 6974 6f72 696e 6720 636f 6e74   monitoring cont
-00001de0: 6578 2074 6861 7420 6973 6e27 7420 7061  ex that isn't pa
-00001df0: 7274 206f 6620 7468 6520 6261 7369 6320  rt of the basic 
-00001e00: 4f70 656e 4149 2041 5049 2063 616c 6c20  OpenAI API call 
-00001e10: 696e 666f 726d 6174 696f 6e2e 2046 6f72  information. For
-00001e20: 2065 7861 6d70 6c65 2c20 6966 2079 6f75   example, if you
-00001e30: 2061 7265 2075 7369 6e67 2061 2073 7065   are using a spe
-00001e40: 6369 6669 6320 7465 6d70 6c61 7465 2049  cific template I
-00001e50: 4420 6f72 2069 6620 7468 6973 2063 616c  D or if this cal
-00001e60: 6c20 6973 2062 6569 6e67 206d 6164 6520  l is being made 
-00001e70: 666f 7220 6120 7370 6563 6966 6963 2063  for a specific c
-00001e80: 7573 746f 6d65 7220 4944 2c20 7468 6573  ustomer ID, thes
-00001e90: 6520 6172 6520 6669 656c 6473 2079 6f75  e are fields you
-00001ea0: 2063 616e 2061 6464 2074 6865 7265 2074   can add there t
-00001eb0: 6f20 6865 6c70 2067 6574 2066 756c 6c20  o help get full 
-00001ec0: 636f 6e74 6578 7420 7768 656e 206d 6f6e  context when mon
-00001ed0: 6974 6f72 696e 6720 7769 7468 204d 6f6e  itoring with Mon
-00001ee0: 612e 0a0a 4578 616d 706c 653a 0a60 6060  a...Example:.```
-00001ef0: 7079 0a72 6573 706f 6e73 6520 3d20 6173  py.response = as
-00001f00: 796e 6369 6f2e 7275 6e28 6d6f 6e69 746f  yncio.run(monito
-00001f10: 7265 645f 636f 6d70 6c65 7469 6f6e 2e61  red_completion.a
-00001f20: 6372 6561 7465 280a 2020 2020 656e 6769  create(.    engi
-00001f30: 6e65 3d6d 6f64 656c 2c0a 2020 2020 7072  ne=model,.    pr
-00001f40: 6f6d 7074 3d70 726f 6d70 742c 0a20 2020  ompt=prompt,.   
-00001f50: 206d 6178 5f74 6f6b 656e 733d 6d61 785f   max_tokens=max_
-00001f60: 746f 6b65 6e73 2c0a 2020 2020 6e3d 6e2c  tokens,.    n=n,
-00001f70: 0a20 2020 2074 656d 7065 7261 7475 7265  .    temperature
-00001f80: 3d74 656d 7065 7261 7475 7265 2c0a 2020  =temperature,.  
-00001f90: 2020 4d4f 4e41 5f61 6464 6974 696f 6e61    MONA_additiona
-00001fa0: 6c5f 6461 7461 3d7b 2263 7573 746f 6d65  l_data={"custome
-00001fb0: 725f 6964 223a 2022 4135 3331 3235 3122  r_id": "A531251"
-00001fc0: 7d2c 0a29 290a 7072 696e 7428 7265 7370  },.)).print(resp
-00001fd0: 6f6e 7365 2e63 686f 6963 6573 5b30 5d2e  onse.choices[0].
-00001fe0: 7465 7874 290a 6060 600a 0a23 2323 2055  text).```..### U
-00001ff0: 7369 6e67 204f 7065 6e41 4920 7769 7468  sing OpenAI with
-00002000: 2052 4553 5420 6361 6c6c 7320 696e 7374   REST calls inst
-00002010: 6561 6420 6f66 204f 7065 6e41 4927 7320  ead of OpenAI's 
-00002020: 5079 7468 6f6e 2063 6c69 656e 740a 496e  Python client.In
-00002030: 2073 6f6d 6520 6361 7365 7320 796f 7520   some cases you 
-00002040: 6d61 7920 6368 6f6f 7365 2074 6f20 7573  may choose to us
-00002050: 6520 4f70 656e 4149 2773 2041 5049 2064  e OpenAI's API d
-00002060: 6972 6563 746c 7920 7769 7468 2052 4553  irectly with RES
-00002070: 5420 6361 6c6c 7320 616e 6420 6e6f 7420  T calls and not 
-00002080: 7573 696e 6720 4f70 656e 4149 2773 2053  using OpenAI's S
-00002090: 444b 2e20 466f 7220 7468 6573 6520 6361  DK. For these ca
-000020a0: 7365 7320 7765 2061 6c6c 6f77 2061 206d  ses we allow a m
-000020b0: 6f72 6520 6469 7265 6374 2061 7070 726f  ore direct appro
-000020c0: 6163 6820 666f 7220 6c6f 6767 696e 6720  ach for logging 
-000020d0: 746f 204d 6f6e 6120 6173 2077 656c 6c2c  to Mona as well,
-000020e0: 2062 7920 7573 696e 6720 7468 6520 2267   by using the "g
-000020f0: 6574 5f72 6573 745f 6d6f 6e69 746f 7222  et_rest_monitor"
-00002100: 2066 756e 6374 696f 6e2e 2053 6565 2065   function. See e
-00002110: 7861 6d70 6c65 2062 656c 6f77 2e0a 0a60  xample below...`
-00002120: 6060 7079 0a23 2044 6972 6563 7420 5245  ``py.# Direct RE
-00002130: 5354 2075 7361 6765 2c20 7769 7468 6f75  ST usage, withou
-00002140: 7420 4f70 656e 4149 2063 6c69 656e 740a  t OpenAI client.
-00002150: 696d 706f 7274 2072 6571 7565 7374 730a  import requests.
-00002160: 6672 6f6d 206f 7320 696d 706f 7274 2065  from os import e
-00002170: 6e76 6972 6f6e 0a66 726f 6d20 6d6f 6e61  nviron.from mona
-00002180: 5f6f 7065 6e61 6920 696d 706f 7274 2067  _openai import g
-00002190: 6574 5f72 6573 745f 6d6f 6e69 746f 720a  et_rest_monitor.
-000021a0: 0a0a 4d4f 4e41 5f41 5049 5f4b 4559 203d  ..MONA_API_KEY =
-000021b0: 2065 6e76 6972 6f6e 2e67 6574 2822 4d4f   environ.get("MO
-000021c0: 4e41 5f41 5049 5f4b 4559 2229 0a4d 4f4e  NA_API_KEY").MON
-000021d0: 415f 5345 4352 4554 203d 2065 6e76 6972  A_SECRET = envir
-000021e0: 6f6e 2e67 6574 2822 4d4f 4e41 5f53 4543  on.get("MONA_SEC
-000021f0: 5245 5422 290a 4d4f 4e41 5f43 5245 4453  RET").MONA_CREDS
-00002200: 203d 207b 0a20 2020 2022 6b65 7922 3a20   = {.    "key": 
-00002210: 4d4f 4e41 5f41 5049 5f4b 4559 2c0a 2020  MONA_API_KEY,.  
-00002220: 2020 2273 6563 7265 7422 3a20 4d4f 4e41    "secret": MONA
-00002230: 5f53 4543 5245 542c 0a7d 0a43 4f4e 5445  _SECRET,.}.CONTE
-00002240: 5854 5f43 4c41 5353 5f4e 414d 4520 3d20  XT_CLASS_NAME = 
-00002250: 2253 4f4d 455f 4d4f 4e49 544f 5249 4e47  "SOME_MONITORING
-00002260: 5f43 4f4e 5445 5854 5f4e 414d 4522 0a0a  _CONTEXT_NAME"..
-00002270: 2320 4765 7420 4d6f 6e61 206c 6f67 6765  # Get Mona logge
-00002280: 720a 6d6f 6e61 5f6c 6f67 6765 7220 3d20  r.mona_logger = 
-00002290: 6765 745f 7265 7374 5f6d 6f6e 6974 6f72  get_rest_monitor
-000022a0: 280a 2020 2020 2243 6f6d 706c 6574 696f  (.    "Completio
-000022b0: 6e22 2c0a 2020 2020 4d4f 4e41 5f43 5245  n",.    MONA_CRE
-000022c0: 4453 2c0a 2020 2020 434f 4e54 4558 545f  DS,.    CONTEXT_
-000022d0: 434c 4153 535f 4e41 4d45 2c0a 290a 0a23  CLASS_NAME,.)..#
-000022e0: 2053 6574 2075 7020 7468 6520 4150 4920   Set up the API 
-000022f0: 656e 6470 6f69 6e74 2055 524c 2061 6e64  endpoint URL and
-00002300: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
-00002310: 6865 6164 6572 730a 7572 6c20 3d20 2268  headers.url = "h
-00002320: 7474 7073 3a2f 2f61 7069 2e6f 7065 6e61  ttps://api.opena
-00002330: 692e 636f 6d2f 7631 2f63 6f6d 706c 6574  i.com/v1/complet
-00002340: 696f 6e73 220a 6865 6164 6572 7320 3d20  ions".headers = 
-00002350: 7b0a 2020 2020 2243 6f6e 7465 6e74 2d54  {.    "Content-T
-00002360: 7970 6522 3a20 2261 7070 6c69 6361 7469  ype": "applicati
-00002370: 6f6e 2f6a 736f 6e22 2c0a 2020 2020 2241  on/json",.    "A
-00002380: 7574 686f 7269 7a61 7469 6f6e 223a 2066  uthorization": f
-00002390: 2242 6561 7265 7220 7b65 6e76 6972 6f6e  "Bearer {environ
-000023a0: 2e67 6574 2827 4f50 454e 5f41 495f 4b45  .get('OPEN_AI_KE
-000023b0: 5927 297d 222c 0a7d 0a0a 2320 5365 7420  Y')}",.}..# Set 
-000023c0: 7570 2074 6865 2072 6571 7565 7374 2064  up the request d
-000023d0: 6174 610a 6461 7461 203d 207b 0a20 2020  ata.data = {.   
-000023e0: 2022 7072 6f6d 7074 223a 2070 726f 6d70   "prompt": promp
-000023f0: 742c 0a20 2020 2022 6d61 785f 746f 6b65  t,.    "max_toke
-00002400: 6e73 223a 206d 6178 5f74 6f6b 656e 732c  ns": max_tokens,
-00002410: 0a20 2020 2022 7465 6d70 6572 6174 7572  .    "temperatur
-00002420: 6522 3a20 7465 6d70 6572 6174 7572 652c  e": temperature,
-00002430: 0a20 2020 2022 6d6f 6465 6c22 3a20 6d6f  .    "model": mo
-00002440: 6465 6c2c 0a20 2020 2022 6e22 3a20 6e2c  del,.    "n": n,
-00002450: 0a7d 0a0a 2320 5468 6520 6c6f 675f 7265  .}..# The log_re
-00002460: 7175 6573 7420 6675 6e63 7469 6f6e 2072  quest function r
-00002470: 6574 7572 6e73 2074 776f 206f 7468 6572  eturns two other
-00002480: 2066 756e 6374 696f 6e20 666f 7220 6c61   function for la
-00002490: 7465 7220 6c6f 6767 696e 670a 2320 7468  ter logging.# th
-000024a0: 6520 7265 7370 6f6e 7365 206f 7220 7468  e response or th
-000024b0: 6520 6578 6365 7074 696f 6e2e 2057 6865  e exception. Whe
-000024c0: 6e20 7765 206c 6174 6572 2064 6f20 7468  n we later do th
-000024d0: 6174 2c20 7468 6520 6c6f 6767 6572 2077  at, the logger w
-000024e0: 696c 6c0a 2320 6163 7475 616c 6c79 2063  ill.# actually c
-000024f0: 616c 6375 6c61 7465 2061 6c6c 2074 6865  alculate all the
-00002500: 2072 656c 6576 616e 7420 6d65 7472 6963   relevant metric
-00002510: 7320 616e 6420 7769 6c6c 2073 656e 6420  s and will send 
-00002520: 7468 656d 2074 6f0a 2320 4d6f 6e61 2e0a  them to.# Mona..
-00002530: 7265 7370 6f6e 7365 5f6c 6f67 6765 722c  response_logger,
-00002540: 2065 7863 6570 7469 6f6e 5f6c 6f67 6765   exception_logge
-00002550: 7220 3d20 6d6f 6e61 5f6c 6f67 6765 722e  r = mona_logger.
-00002560: 6c6f 675f 7265 7175 6573 7428 0a20 2020  log_request(.   
-00002570: 2064 6174 612c 2061 6464 6974 696f 6e61   data, additiona
-00002580: 6c5f 6461 7461 3d7b 2263 7573 746f 6d65  l_data={"custome
-00002590: 725f 6964 223a 2022 4135 3331 3235 3122  r_id": "A531251"
-000025a0: 7d0a 290a 0a74 7279 3a0a 2020 2020 2320  }.)..try:.    # 
-000025b0: 5365 6e64 2074 6865 2072 6571 7565 7374  Send the request
-000025c0: 2074 6f20 7468 6520 4150 490a 2020 2020   to the API.    
-000025d0: 7265 7370 6f6e 7365 203d 2072 6571 7565  response = reque
-000025e0: 7374 732e 706f 7374 2875 726c 2c20 6865  sts.post(url, he
-000025f0: 6164 6572 733d 6865 6164 6572 732c 206a  aders=headers, j
-00002600: 736f 6e3d 6461 7461 290a 0a20 2020 2023  son=data)..    #
-00002610: 2043 6865 636b 2066 6f72 2048 5454 5020   Check for HTTP 
-00002620: 6572 726f 7273 0a20 2020 2072 6573 706f  errors.    respo
-00002630: 6e73 652e 7261 6973 655f 666f 725f 7374  nse.raise_for_st
-00002640: 6174 7573 2829 0a0a 2020 2020 2320 4c6f  atus()..    # Lo
-00002650: 6720 7265 7370 6f6e 7365 2074 6f20 4d6f  g response to Mo
-00002660: 6e61 0a20 2020 2072 6573 706f 6e73 655f  na.    response_
-00002670: 6c6f 6767 6572 2872 6573 706f 6e73 652e  logger(response.
-00002680: 6a73 6f6e 2829 290a 2020 2020 7072 696e  json()).    prin
-00002690: 7428 7265 7370 6f6e 7365 2e6a 736f 6e28  t(response.json(
-000026a0: 295b 2263 686f 6963 6573 225d 5b30 5d5b  )["choices"][0][
-000026b0: 2274 6578 7422 5d29 0a0a 6578 6365 7074  "text"])..except
-000026c0: 2045 7863 6570 7469 6f6e 2061 7320 6572   Exception as er
-000026d0: 723a 0a20 2020 2023 204c 6f67 2065 7863  r:.    # Log exc
-000026e0: 6570 7469 6f6e 2074 6f20 4d6f 6e61 0a20  eption to Mona. 
-000026f0: 2020 2065 7863 6570 7469 6f6e 5f6c 6f67     exception_log
-00002700: 6765 7228 290a 6060 600a 0a23 2323 2053  ger().```..### S
-00002710: 7472 6561 6d20 7375 7070 6f72 740a 0a4f  tream support..O
-00002720: 7065 6e41 4920 616c 6c6f 7773 2072 6563  penAI allows rec
-00002730: 6569 7669 6e67 2072 6573 706f 6e73 6573  eiving responses
-00002740: 2061 7320 6120 7374 7265 616d 206f 6620   as a stream of 
-00002750: 746f 6b65 6e73 2075 7369 6e67 2074 6865  tokens using the
-00002760: 2022 7374 7265 616d 2220 7061 7261 6d65   "stream" parame
-00002770: 7465 722e 2057 6865 6e20 7468 6973 2069  ter. When this i
-00002780: 7320 646f 6e65 2c20 4d6f 6e61 2077 696c  s done, Mona wil
-00002790: 6c20 636f 6c6c 6563 7420 616c 6c20 7468  l collect all th
-000027a0: 6520 746f 6b65 6e73 2069 6e20 6d65 6d6f  e tokens in memo
-000027b0: 7279 2061 6e64 2077 696c 6c20 6372 6561  ry and will crea
-000027c0: 7465 2074 6865 2061 6e61 6c79 7369 7320  te the analysis 
-000027d0: 616e 6420 6c6f 6720 6f75 7420 7468 6520  and log out the 
-000027e0: 6461 7461 2074 6865 206d 6f6d 656e 7420  data the moment 
-000027f0: 7468 6520 7374 7265 616d 2069 7320 6f76  the stream is ov
-00002800: 6572 2e20 596f 7520 646f 6e27 7420 6e65  er. You don't ne
-00002810: 6564 2074 6f20 646f 2061 6e79 7468 696e  ed to do anythin
-00002820: 6720 746f 206d 616b 6520 7468 6973 2068  g to make this h
-00002830: 6170 7065 6e2e 0a0a 5369 6e63 6520 666f  appen...Since fo
-00002840: 7220 7374 7265 616d 696e 6720 7265 7370  r streaming resp
-00002850: 6f6e 7365 7320 4f70 656e 4149 2064 6f65  onses OpenAI doe
-00002860: 736e 2774 2073 7570 706c 7920 7468 6520  sn't supply the 
-00002870: 6675 6c6c 2075 7361 6765 2074 6f6b 656e  full usage token
-00002880: 7320 7375 6d6d 6172 792c 204d 6f6e 6120  s summary, Mona 
-00002890: 7573 6573 2074 6865 2074 696b 746f 6b65  uses the tiktoke
-000028a0: 6e20 7061 636b 6167 6520 746f 2063 616c  n package to cal
-000028b0: 6375 6c61 7465 2074 6865 2074 6f6b 656e  culate the token
-000028c0: 7320 6f66 2074 6865 2070 726f 6d70 7420  s of the prompt 
-000028d0: 616e 6420 636f 6d70 6c65 7469 6f6e 2061  and completion a
-000028e0: 6e64 206c 6f67 2074 6865 6d20 666f 7220  nd log them for 
-000028f0: 6d6f 6e69 746f 7269 6e67 2e0a 0a4e 4f54  monitoring...NOT
-00002900: 453a 2053 7472 6561 6d20 6973 2063 7572  E: Stream is cur
-00002910: 7265 6e74 6c79 206f 6e6c 7920 7375 7070  rently only supp
-00002920: 6f72 7465 6420 7769 7468 2053 444b 2075  orted with SDK u
-00002930: 7361 6765 2c20 616e 6420 6e6f 7420 7769  sage, and not wi
-00002940: 7468 2075 7369 6e67 2052 4553 5420 6469  th using REST di
-00002950: 7265 6374 6c79 2e0a 0a23 2320 4c61 6e67  rectly...## Lang
-00002960: 4368 6169 6e20 7375 7070 6f72 740a 0a59  Chain support..Y
-00002970: 6f75 2063 616e 2075 7365 2074 6865 2065  ou can use the e
-00002980: 7870 6f72 7465 6420 606d 6f6e 6974 6f72  xported `monitor
-00002990: 5f6c 616e 6763 6861 696e 5f6c 6c6d 6020  _langchain_llm` 
-000029a0: 746f 2077 7261 7020 6120 4c61 6e67 4368  to wrap a LangCh
-000029b0: 6169 6e20 4f70 656e 4149 204c 4c4d 2028  ain OpenAI LLM (
-000029c0: 6368 6174 206f 7220 6e6f 726d 616c 2920  chat or normal) 
-000029d0: 7769 7468 204d 6f6e 6127 7320 6d6f 6e69  with Mona's moni
-000029e0: 746f 7269 6e67 2063 6170 6162 696c 6974  toring capabilit
-000029f0: 6965 733a 0a0a 6060 6070 790a 6672 6f6d  ies:..```py.from
-00002a00: 206d 6f6e 615f 6f70 656e 6169 2069 6d70   mona_openai imp
-00002a10: 6f72 7420 6d6f 6e69 746f 725f 6c61 6e67  ort monitor_lang
-00002a20: 6368 6169 6e5f 6c6c 6d0a 0a66 726f 6d20  chain_llm..from 
-00002a30: 6c61 6e67 6368 6169 6e2e 6c6c 6d73 2069  langchain.llms i
-00002a40: 6d70 6f72 7420 4f70 656e 4149 0a0a 2320  mport OpenAI..# 
-00002a50: 5772 6170 2074 6865 204c 4c4d 206f 626a  Wrap the LLM obj
-00002a60: 6563 7420 7769 7468 204d 6f6e 6120 6d6f  ect with Mona mo
-00002a70: 6e69 746f 7269 6e67 2e0a 6c6c 6d20 3d20  nitoring..llm = 
-00002a80: 6d6f 6e69 746f 725f 6c61 6e67 6368 6169  monitor_langchai
-00002a90: 6e5f 6c6c 6d28 0a20 2020 204f 7065 6e41  n_llm(.    OpenA
-00002aa0: 4928 4f50 454e 5f41 495f 4b45 5929 2c0a  I(OPEN_AI_KEY),.
-00002ab0: 2020 2020 4d4f 4e41 5f43 5245 4453 2c0a      MONA_CREDS,.
-00002ac0: 2020 2020 434f 4e54 4558 545f 434c 4153      CONTEXT_CLAS
-00002ad0: 535f 4e41 4d45 290a 6060 600a 0a53 6565  S_NAME).```..See
-00002ae0: 2066 756c 6c20 6578 616d 706c 6520 696e   full example in
-00002af0: 2063 6f6d 706c 6574 696f 6e5f 6c61 6e67   completion_lang
-00002b00: 6368 6169 6e2e 7079 2069 6e20 7468 6520  chain.py in the 
-00002b10: 6578 616d 706c 6573 2066 6f6c 6465 722e  examples folder.
-00002b20: 0a0a 2323 204d 6f6e 6120 5344 4b0a 0a54  ..## Mona SDK..T
-00002b30: 6869 7320 7061 636b 6167 6520 7573 6573  his package uses
-00002b40: 2074 6865 206d 6f6e 615f 7364 6b20 7061   the mona_sdk pa
-00002b50: 636b 6167 6520 746f 2065 7870 6f72 7420  ckage to export 
-00002b60: 7468 6520 7265 6c65 7661 6e74 2064 6174  the relevant dat
-00002b70: 6120 746f 204d 6f6e 612e 2054 6865 7265  a to Mona. There
-00002b80: 2061 7265 2073 6576 6572 616c 2065 6e76   are several env
-00002b90: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00002ba0: 6573 2079 6f75 2063 616e 2075 7365 2074  es you can use t
-00002bb0: 6f20 636f 6e66 6967 7572 6520 7468 6520  o configure the 
-00002bc0: 5344 4b27 7320 6265 6861 7669 6f72 2e20  SDK's behavior. 
-00002bd0: 466f 7220 6578 616d 706c 652c 2079 6f75  For example, you
-00002be0: 2063 616e 2073 6574 2069 7420 7570 2074   can set it up t
-00002bf0: 6f20 7261 6973 6520 6578 6365 7074 696f  o raise exceptio
-00002c00: 6e73 2077 6865 6e20 6578 706f 7274 696e  ns when exportin
-00002c10: 6720 6461 7461 2074 6f20 4d6f 6e61 2066  g data to Mona f
-00002c20: 6169 6c73 2028 6974 2064 6f65 736e 2774  ails (it doesn't
-00002c30: 2064 6f20 7468 6174 2062 7920 6465 6661   do that by defa
-00002c40: 756c 7429 2e0a 0a23 2320 4d6f 6e69 746f  ult)...## Monito
-00002c50: 7269 6e67 2066 6f72 2070 726f 6661 6e69  ring for profani
-00002c60: 7479 0a0a 4d6f 6e61 2075 7365 7320 7468  ty..Mona uses th
-00002c70: 6520 616c 742d 7072 6f66 616e 6974 792d  e alt-profanity-
-00002c80: 6368 6563 6b20 7061 6361 6b67 6520 2868  check pacakge (h
-00002c90: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00002ca0: 7072 6f6a 6563 742f 616c 742d 7072 6f66  project/alt-prof
-00002cb0: 616e 6974 792d 6368 6563 6b2f 2920 746f  anity-check/) to
-00002cc0: 2063 7265 6174 6520 626f 7468 2062 6f6f   create both boo
-00002cd0: 6c65 616e 2070 7265 6469 6374 696f 6e73  lean predictions
-00002ce0: 2061 6e64 2070 726f 6261 6269 6c74 7920   and probabilty 
-00002cf0: 7363 6f72 6573 2066 6f72 2074 6865 2065  scores for the e
-00002d00: 7869 7374 656e 6365 206f 6620 7072 6f66  xistence of prof
-00002d10: 616e 6974 7920 626f 7468 2069 6e20 7468  anity both in th
-00002d20: 6520 7072 6f6d 7074 2061 6e64 2069 6e20  e prompt and in 
-00002d30: 7468 6520 7265 7370 6f6e 7365 732e 2057  the responses. W
-00002d40: 6520 7573 6520 7468 6520 6275 696c 7420  e use the built 
-00002d50: 696e 2070 6163 6b61 6765 206d 6574 686f  in package metho
-00002d60: 6473 2066 6f72 2074 6861 742e 2049 6620  ds for that. If 
-00002d70: 796f 7520 7761 6e74 2c20 666f 7220 6578  you want, for ex
-00002d80: 616d 706c 652c 2074 6f20 7573 6520 6120  ample, to use a 
-00002d90: 6469 6666 6572 656e 7420 7072 6f62 6162  different probab
-00002da0: 696c 6974 7920 7468 7265 7368 6f6c 6420  ility threshold 
-00002db0: 666f 7220 7468 6520 626f 6f6c 6561 6e20  for the boolean 
-00002dc0: 7072 6564 6963 7469 6f6e 2c20 796f 7520  prediction, you 
-00002dd0: 6361 6e20 646f 2074 6861 7420 6279 2063  can do that by c
-00002de0: 6861 6e67 696e 6720 796f 7572 204d 6f6e  hanging your Mon
-00002df0: 6120 636f 6e66 6967 206f 6e20 7468 6520  a config on the 
-00002e00: 4d6f 6e61 2064 6173 6862 6f61 7264 2e0a  Mona dashboard..
+00000260: 703e 0a0a 0a55 7365 206f 6e65 206c 696e  p>...Use one lin
+00000270: 6520 6f66 2063 6f64 6520 746f 2067 6574  e of code to get
+00000280: 2069 6e73 7461 6e74 206c 6976 6520 6d6f   instant live mo
+00000290: 6e69 746f 7269 6e67 2066 6f72 2079 6f75  nitoring for you
+000002a0: 7220 4f70 656e 4149 2075 7361 6765 2069  r OpenAI usage i
+000002b0: 6e63 6c75 6469 6e67 3a0a 2a20 546f 6b65  ncluding:.* Toke
+000002c0: 6e73 2075 7361 6765 0a2a 2048 616c 6c75  ns usage.* Hallu
+000002d0: 6369 6e61 7469 6f6e 2061 6c65 7274 730a  cination alerts.
+000002e0: 2a20 5072 6f66 616e 6974 7920 616e 6420  * Profanity and 
+000002f0: 7072 6976 6163 7920 616e 616c 7973 6573  privacy analyses
+00000300: 0a2a 2042 6568 6176 696f 7261 6c20 6472  .* Behavioral dr
+00000310: 6966 7473 2061 6e64 2061 6e6f 6d61 6c69  ifts and anomali
+00000320: 6573 0a2a 204c 616e 6743 6861 696e 2073  es.* LangChain s
+00000330: 7570 706f 7274 0a2a 204d 7563 6820 6d75  upport.* Much mu
+00000340: 6368 206d 6f72 650a 0a23 2320 5365 7474  ch more..## Sett
+00000350: 696e 6720 5570 0a0a 6060 6063 6f6e 736f  ing Up..```conso
+00000360: 6c65 0a24 2070 6970 2069 6e73 7461 6c6c  le.$ pip install
+00000370: 206d 6f6e 615f 6f70 656e 6169 0a60 6060   mona_openai.```
+00000380: 0a0a 2323 2051 7569 636b 2053 7461 7274  ..## Quick Start
+00000390: 0a0a 596f 7520 6361 6e20 6669 6e64 2062  ..You can find b
+000003a0: 6f69 6c65 7270 6c61 7465 2063 6f64 6520  oilerplate code 
+000003b0: 666f 7220 6d61 6e79 2075 7365 2063 6173  for many use cas
+000003c0: 6573 2075 6e64 6572 205b 7468 6520 2265  es under [the "e
+000003d0: 7861 6d70 6c65 7322 2066 6f6c 6465 725d  xamples" folder]
+000003e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000003f0: 636f 6d2f 6d6f 6e61 6c61 6273 2f6d 6f6e  com/monalabs/mon
+00000400: 612d 6f70 656e 6169 2f74 7265 652f 6d61  a-openai/tree/ma
+00000410: 696e 2f65 7861 6d70 6c65 7329 2e0a 0a23  in/examples)...#
+00000420: 2323 2057 6974 6820 5374 616e 6461 7264  ## With Standard
+00000430: 204c 6f67 6769 6e67 0a0a 6060 6070 790a   Logging..```py.
+00000440: 6672 6f6d 206f 7320 696d 706f 7274 2065  from os import e
+00000450: 6e76 6972 6f6e 0a69 6d70 6f72 7420 6f70  nviron.import op
+00000460: 656e 6169 0a66 726f 6d20 6d6f 6e61 5f6f  enai.from mona_o
+00000470: 7065 6e61 692e 6c6f 6767 6572 7320 696d  penai.loggers im
+00000480: 706f 7274 2053 7461 6e64 6172 644c 6f67  port StandardLog
+00000490: 6765 720a 6672 6f6d 206c 6f67 6769 6e67  ger.from logging
+000004a0: 2069 6d70 6f72 7420 5741 524e 494e 470a   import WARNING.
+000004b0: 0a66 726f 6d20 6d6f 6e61 5f6f 7065 6e61  .from mona_opena
+000004c0: 6920 696d 706f 7274 206d 6f6e 6974 6f72  i import monitor
+000004d0: 5f77 6974 685f 6c6f 6767 6572 0a0a 6f70  _with_logger..op
+000004e0: 656e 6169 2e61 7069 5f6b 6579 203d 2065  enai.api_key = e
+000004f0: 6e76 6972 6f6e 2e67 6574 2822 4f50 454e  nviron.get("OPEN
+00000500: 5f41 495f 4b45 5922 290a 0a6d 6f6e 6974  _AI_KEY")..monit
+00000510: 6f72 6564 5f63 6f6d 706c 6574 696f 6e20  ored_completion 
+00000520: 3d20 6d6f 6e69 746f 725f 7769 7468 5f6c  = monitor_with_l
+00000530: 6f67 6765 7228 0a20 2020 206f 7065 6e61  ogger(.    opena
+00000540: 692e 436f 6d70 6c65 7469 6f6e 2c0a 2020  i.Completion,.  
+00000550: 2020 5374 616e 6461 7264 4c6f 6767 6572    StandardLogger
+00000560: 2857 4152 4e49 4e47 292c 0a29 0a0a 7265  (WARNING),.)..re
+00000570: 7370 6f6e 7365 203d 206d 6f6e 6974 6f72  sponse = monitor
+00000580: 6564 5f63 6f6d 706c 6574 696f 6e2e 6372  ed_completion.cr
+00000590: 6561 7465 280a 2020 2020 6d6f 6465 6c3d  eate(.    model=
+000005a0: 2274 6578 742d 6164 612d 3030 3122 2c0a  "text-ada-001",.
+000005b0: 2020 2020 7072 6f6d 7074 3d22 4920 7761      prompt="I wa
+000005c0: 6e74 2074 6f20 6765 6e65 7261 7465 2073  nt to generate s
+000005d0: 6f6d 6520 7465 7874 2061 626f 7574 2022  ome text about "
+000005e0: 2c0a 2020 2020 6d61 785f 746f 6b65 6e73  ,.    max_tokens
+000005f0: 3d32 302c 0a20 2020 206e 3d31 2c0a 2020  =20,.    n=1,.  
+00000600: 2020 7465 6d70 6572 6174 7572 653d 302e    temperature=0.
+00000610: 322c 0a20 2020 2023 2041 6464 696e 6720  2,.    # Adding 
+00000620: 6164 6469 7469 6f6e 616c 2069 6e66 6f72  additional infor
+00000630: 6d61 7469 6f6e 2066 6f72 206d 6f6e 6974  mation for monit
+00000640: 6f72 696e 6720 7075 7270 6f73 6573 2c20  oring purposes, 
+00000650: 756e 7265 6c61 7465 6420 746f 0a20 2020  unrelated to.   
+00000660: 2023 2069 6e74 6572 6e61 6c20 4f70 656e   # internal Open
+00000670: 4149 2063 616c 6c2e 0a20 2020 204d 4f4e  AI call..    MON
+00000680: 415f 6164 6469 7469 6f6e 616c 5f64 6174  A_additional_dat
+00000690: 613d 7b22 6375 7374 6f6d 6572 5f69 6422  a={"customer_id"
+000006a0: 3a20 2241 3533 3132 3531 227d 2c0a 290a  : "A531251"},.).
+000006b0: 7072 696e 7428 7265 7370 6f6e 7365 2e63  print(response.c
+000006c0: 686f 6963 6573 5b30 5d2e 7465 7874 290a  hoices[0].text).
+000006d0: 6060 600a 0a23 2323 2057 6974 6820 4d6f  ```..### With Mo
+000006e0: 6e61 0a0a 5b53 6967 6e20 7570 2066 6f72  na..[Sign up for
+000006f0: 2061 2066 7265 6520 4d6f 6e61 2061 6363   a free Mona acc
+00000700: 6f75 6e74 2068 6572 655d 2868 7474 7073  ount here](https
+00000710: 3a2f 2f77 7777 2e6d 6f6e 616c 6162 732e  ://www.monalabs.
+00000720: 696f 2f6f 7065 6e61 692d 6770 742d 6d6f  io/openai-gpt-mo
+00000730: 6e69 746f 7269 6e67 292e 0a0a 6060 6070  nitoring)...```p
+00000740: 790a 6672 6f6d 206f 7320 696d 706f 7274  y.from os import
+00000750: 2065 6e76 6972 6f6e 0a69 6d70 6f72 7420   environ.import 
+00000760: 6f70 656e 6169 0a0a 6672 6f6d 206d 6f6e  openai..from mon
+00000770: 615f 6f70 656e 6169 2069 6d70 6f72 7420  a_openai import 
+00000780: 6d6f 6e69 746f 720a 0a6f 7065 6e61 692e  monitor..openai.
+00000790: 6170 695f 6b65 7920 3d20 656e 7669 726f  api_key = enviro
+000007a0: 6e2e 6765 7428 224f 5045 4e5f 4149 5f4b  n.get("OPEN_AI_K
+000007b0: 4559 2229 0a0a 4d4f 4e41 5f41 5049 5f4b  EY")..MONA_API_K
+000007c0: 4559 203d 2065 6e76 6972 6f6e 2e67 6574  EY = environ.get
+000007d0: 2822 4d4f 4e41 5f41 5049 5f4b 4559 2229  ("MONA_API_KEY")
+000007e0: 0a4d 4f4e 415f 5345 4352 4554 203d 2065  .MONA_SECRET = e
+000007f0: 6e76 6972 6f6e 2e67 6574 2822 4d4f 4e41  nviron.get("MONA
+00000800: 5f53 4543 5245 5422 290a 4d4f 4e41 5f43  _SECRET").MONA_C
+00000810: 5245 4453 203d 207b 0a20 2020 2022 6b65  REDS = {.    "ke
+00000820: 7922 3a20 4d4f 4e41 5f41 5049 5f4b 4559  y": MONA_API_KEY
+00000830: 2c0a 2020 2020 2273 6563 7265 7422 3a20  ,.    "secret": 
+00000840: 4d4f 4e41 5f53 4543 5245 542c 0a7d 0a43  MONA_SECRET,.}.C
+00000850: 4f4e 5445 5854 5f43 4c41 5353 5f4e 414d  ONTEXT_CLASS_NAM
+00000860: 4520 3d20 2253 4f4d 455f 4d4f 4e49 544f  E = "SOME_MONITO
+00000870: 5249 4e47 5f43 4f4e 5445 5854 5f4e 414d  RING_CONTEXT_NAM
+00000880: 4522 0a0a 0a6d 6f6e 6974 6f72 6564 5f63  E"...monitored_c
+00000890: 6f6d 706c 6574 696f 6e20 3d20 6d6f 6e69  ompletion = moni
+000008a0: 746f 7228 0a20 2020 206f 7065 6e61 692e  tor(.    openai.
+000008b0: 436f 6d70 6c65 7469 6f6e 2c0a 2020 2020  Completion,.    
+000008c0: 4d4f 4e41 5f43 5245 4453 2c0a 2020 2020  MONA_CREDS,.    
+000008d0: 434f 4e54 4558 545f 434c 4153 535f 4e41  CONTEXT_CLASS_NA
+000008e0: 4d45 2c0a 290a 0a72 6573 706f 6e73 6520  ME,.)..response 
+000008f0: 3d20 6d6f 6e69 746f 7265 645f 636f 6d70  = monitored_comp
+00000900: 6c65 7469 6f6e 2e63 7265 6174 6528 0a20  letion.create(. 
+00000910: 2020 206d 6f64 656c 3d22 7465 7874 2d61     model="text-a
+00000920: 6461 2d30 3031 222c 0a20 2020 2070 726f  da-001",.    pro
+00000930: 6d70 743d 2249 2077 616e 7420 746f 2067  mpt="I want to g
+00000940: 656e 6572 6174 6520 736f 6d65 2074 6578  enerate some tex
+00000950: 7420 6162 6f75 7420 222c 0a20 2020 206d  t about ",.    m
+00000960: 6178 5f74 6f6b 656e 733d 3230 2c0a 2020  ax_tokens=20,.  
+00000970: 2020 6e3d 312c 0a20 2020 2074 656d 7065    n=1,.    tempe
+00000980: 7261 7475 7265 3d30 2e32 2c0a 2020 2020  rature=0.2,.    
+00000990: 2320 4164 6469 6e67 2061 6464 6974 696f  # Adding additio
+000009a0: 6e61 6c20 696e 666f 726d 6174 696f 6e20  nal information 
+000009b0: 666f 7220 6d6f 6e69 746f 7269 6e67 2070  for monitoring p
+000009c0: 7572 706f 7365 732c 2075 6e72 656c 6174  urposes, unrelat
+000009d0: 6564 2074 6f0a 2020 2020 2320 696e 7465  ed to.    # inte
+000009e0: 726e 616c 204f 7065 6e41 4920 6361 6c6c  rnal OpenAI call
+000009f0: 2e0a 2020 2020 4d4f 4e41 5f61 6464 6974  ..    MONA_addit
+00000a00: 696f 6e61 6c5f 6461 7461 3d7b 2263 7573  ional_data={"cus
+00000a10: 746f 6d65 725f 6964 223a 2022 4135 3331  tomer_id": "A531
+00000a20: 3235 3122 7d2c 0a29 0a70 7269 6e74 2872  251"},.).print(r
+00000a30: 6573 706f 6e73 652e 6368 6f69 6365 735b  esponse.choices[
+00000a40: 305d 2e74 6578 7429 0a60 6060 0a0a 2323  0].text).```..##
+00000a50: 2053 7570 706f 7274 6564 204f 7065 6e41   Supported OpenA
+00000a60: 4920 4150 4973 0a43 7572 7265 6e74 6c79  I APIs.Currently
+00000a70: 2074 6869 7320 636c 6965 6e74 2073 7570   this client sup
+00000a80: 706f 7274 7320 606f 7065 6e61 692e 436f  ports `openai.Co
+00000a90: 6d70 6c65 7469 6f6e 6020 616e 6420 606f  mpletion` and `o
+00000aa0: 7065 6e61 692e 4368 6174 436f 6d70 6c65  penai.ChatComple
+00000ab0: 7469 6f6e 602e 204d 6f6e 6120 6361 6e20  tion`. Mona can 
+00000ac0: 7375 7070 6f72 7420 7072 6f63 6573 7365  support processe
+00000ad0: 7320 6261 7365 6420 6f6e 206f 7468 6572  s based on other
+00000ae0: 2041 5049 7320 616e 6420 616c 736f 206e   APIs and also n
+00000af0: 6f6e 2d4f 7065 6e41 492d 6261 7365 6420  on-OpenAI-based 
+00000b00: 6170 7073 2e0a 4966 2079 6f75 2068 6176  apps..If you hav
+00000b10: 6520 6120 6469 6666 6572 7265 6e74 2075  e a differrent u
+00000b20: 7365 2d63 6173 652c 2077 6527 6420 6c6f  se-case, we'd lo
+00000b30: 7665 2074 6f20 6865 6172 2061 626f 7574  ve to hear about
+00000b40: 2069 7421 2050 6c65 6173 6520 656d 6169   it! Please emai
+00000b50: 6c20 7573 2061 7420 7375 7070 6f72 7440  l us at support@
+00000b60: 6d6f 6e61 6c61 6273 2e69 6f2e 0a0a 2323  monalabs.io...##
+00000b70: 2055 7361 6765 0a23 2323 2049 6e69 7469   Usage.### Initi
+00000b80: 616c 697a 6174 696f 6e0a 0a54 6865 206d  alization..The m
+00000b90: 6169 6e20 616e 6420 6f6e 6c79 2066 756e  ain and only fun
+00000ba0: 6374 696f 6e20 6578 706f 7365 6420 696e  ction exposed in
+00000bb0: 2074 6869 7320 7061 636b 6167 6520 6973   this package is
+00000bc0: 2060 6d6f 6e69 746f 7260 2e0a 6060 6070   `monitor`..```p
+00000bd0: 790a 696d 706f 7274 206f 7065 6e61 690a  y.import openai.
+00000be0: 0a66 726f 6d20 6d6f 6e61 5f6f 7065 6e61  .from mona_opena
+00000bf0: 6920 696d 706f 7274 206d 6f6e 6974 6f72  i import monitor
+00000c00: 0a0a 6f70 656e 6169 2e61 7069 5f6b 6579  ..openai.api_key
+00000c10: 203d 2065 6e76 6972 6f6e 2e67 6574 2822   = environ.get("
+00000c20: 4f50 454e 5f41 495f 4b45 5922 290a 0a6d  OPEN_AI_KEY")..m
+00000c30: 6f6e 6974 6f72 6564 5f63 6f6d 706c 6574  onitored_complet
+00000c40: 696f 6e20 3d20 6d6f 6e69 746f 7228 0a20  ion = monitor(. 
+00000c50: 2020 206f 7065 6e61 692e 436f 6d70 6c65     openai.Comple
+00000c60: 7469 6f6e 2c0a 2020 2020 280a 2020 2020  tion,.    (.    
+00000c70: 2020 2020 656e 7669 726f 6e2e 6765 7428      environ.get(
+00000c80: 224d 4f4e 415f 4150 495f 4b45 5922 292c  "MONA_API_KEY"),
+00000c90: 0a20 2020 2020 2020 2065 6e76 6972 6f6e  .        environ
+00000ca0: 2e67 6574 2822 4d4f 4e41 5f53 4543 5245  .get("MONA_SECRE
+00000cb0: 5422 292c 0a20 2020 2029 2c0a 2020 2020  T"),.    ),.    
+00000cc0: 2253 4f4d 455f 4d4f 4e49 544f 5249 4e47  "SOME_MONITORING
+00000cd0: 5f43 4f4e 5445 5854 5f4e 414d 4522 2c0a  _CONTEXT_NAME",.
+00000ce0: 2020 2020 7b22 616e 616c 7973 6973 223a      {"analysis":
+00000cf0: 207b 2270 726f 6661 6e69 7479 223a 2046   {"profanity": F
+00000d00: 616c 7365 7d7d 0a29 0a0a 2e2e 2e0a 0a6d  alse}}.).......m
+00000d10: 6f6e 6974 6f72 6564 5f63 6f6d 706c 6574  onitored_complet
+00000d20: 696f 6e2e 6372 6561 7465 282e 2e2e 290a  ion.create(...).
+00000d30: 6060 600a 0a54 6865 2060 6d6f 6e69 746f  ```..The `monito
+00000d40: 7260 2066 756e 6374 696f 6e20 7265 7475  r` function retu
+00000d50: 726e 7320 746f 2079 6f75 2061 2063 6c61  rns to you a cla
+00000d60: 7373 2074 6861 7420 7772 6170 7320 7468  ss that wraps th
+00000d70: 6520 6f72 6967 696e 616c 206f 7065 6e61  e original opena
+00000d80: 6920 656e 6470 6f69 6e74 2063 6c61 7373  i endpoint class
+00000d90: 2079 6f75 2070 726f 7669 6465 2c20 7769   you provide, wi
+00000da0: 7468 2061 6e20 6571 7569 7661 6c65 6e74  th an equivalent
+00000db0: 2041 5049 2028 6265 7369 6465 7320 736f   API (besides so
+00000dc0: 6d65 2061 6464 6974 696f 6e73 206c 6973  me additions lis
+00000dd0: 7465 6420 6265 6c6f 7729 2e0a 596f 7520  ted below)..You 
+00000de0: 6361 6e20 7468 656e 2075 7365 2074 6865  can then use the
+00000df0: 2072 6574 7572 6e65 6420 636c 6173 7327   returned class'
+00000e00: 2022 6372 6561 7465 2220 616e 6420 2261   "create" and "a
+00000e10: 6372 6561 7465 2220 6675 6e63 7469 6f6e  create" function
+00000e20: 7320 6a75 7374 2061 7320 796f 7520 776f  s just as you wo
+00000e30: 756c 6420 6265 666f 7265 2c20 6f6e 6c79  uld before, only
+00000e40: 206e 6f77 2c20 6265 7369 6465 7320 6765   now, besides ge
+00000e50: 7474 696e 6720 7468 6520 7265 7175 6573  tting the reques
+00000e60: 7465 6420 6f70 656e 4149 2066 756e 6374  ted openAI funct
+00000e70: 696f 6e61 6c69 7479 2c20 7468 6973 2063  ionality, this c
+00000e80: 6c69 656e 7420 7769 6c6c 206c 6f67 206f  lient will log o
+00000e90: 7574 2074 6f20 4d6f 6e61 2773 2073 6572  ut to Mona's ser
+00000ea0: 7665 7220 7468 6520 7061 7261 6d65 7465  ver the paramete
+00000eb0: 7273 2079 6f75 2075 7365 6420 2865 2e67  rs you used (e.g
+00000ec0: 2e2c 2074 656d 7065 7261 7475 7265 292c  ., temperature),
+00000ed0: 2064 6174 6120 6162 6f75 7420 7468 6520   data about the 
+00000ee0: 7265 7370 6f6e 7365 2066 726f 6d20 4f70  response from Op
+00000ef0: 656e 4149 2773 2073 6572 7665 722c 2061  enAI's server, a
+00000f00: 6e64 2063 7573 746f 6d20 616e 616c 7973  nd custom analys
+00000f10: 6573 2061 626f 7574 2074 6865 2063 616c  es about the cal
+00000f20: 6c20 2865 2e67 2e2c 2070 726f 6661 6e69  l (e.g., profani
+00000f30: 7479 2073 636f 7265 732c 2070 7269 7661  ty scores, priva
+00000f40: 6379 2063 6865 636b 7320 666f 7220 656d  cy checks for em
+00000f50: 6169 6c73 2f70 686f 6e65 206e 756d 6265  ails/phone numbe
+00000f60: 7273 2066 6f75 6e64 2069 6e20 7468 6520  rs found in the 
+00000f70: 7465 7874 732c 2074 6578 7475 616c 2061  texts, textual a
+00000f80: 6e61 6c79 7365 732c 2065 7463 2e2e 2e29  nalyses, etc...)
+00000f90: 0a0a 5468 6520 606d 6f6e 6974 6f72 6020  ..The `monitor` 
+00000fa0: 6675 6e63 7469 6f6e 2072 6563 6569 7665  function receive
+00000fb0: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
+00000fc0: 6172 6775 6d65 6e74 733a 0a6f 7065 6e61  arguments:.opena
+00000fd0: 695f 636c 6173 733a 2041 6e20 4f70 656e  i_class: An Open
+00000fe0: 4149 2041 5049 2063 6c61 7373 2074 6f20  AI API class to 
+00000ff0: 7772 6170 2077 6974 6820 6d6f 6e69 746f  wrap with monito
+00001000: 7269 6e67 2063 6170 6162 696c 7469 6573  ring capabilties
+00001010: 2e0a 6d6f 6e61 5f63 7265 6473 3a20 4120  ..mona_creds: A 
+00001020: 6469 6374 2028 636f 6e74 6169 6e69 6e67  dict (containing
+00001030: 2022 6b65 7922 2061 6e64 2022 7365 6372   "key" and "secr
+00001040: 6574 2229 206f 7220 7061 6972 2028 7475  et") or pair (tu
+00001050: 706c 6529 206f 6620 4d6f 6e61 2041 5049  ple) of Mona API
+00001060: 206b 6579 2061 6e64 2073 6563 7265 7420   key and secret 
+00001070: 746f 2073 6574 2075 7020 4d6f 6e61 2773  to set up Mona's
+00001080: 2063 6c69 656e 7473 2066 726f 6d20 6974   clients from it
+00001090: 7320 5344 4b2e 0a63 6f6e 7465 7874 5f63  s SDK..context_c
+000010a0: 6c61 7373 3a20 5468 6520 4d6f 6e61 2063  lass: The Mona c
+000010b0: 6f6e 7465 7874 2063 6c61 7373 206e 616d  ontext class nam
+000010c0: 6520 746f 2075 7365 2066 6f72 206d 6f6e  e to use for mon
+000010d0: 6974 6f72 696e 672e 2055 7365 2061 2063  itoring. Use a c
+000010e0: 6f6e 7374 616e 7420 6e61 6d65 206f 6620  onstant name of 
+000010f0: 796f 7572 2063 686f 6963 652e 0a73 7065  your choice..spe
+00001100: 6373 3a20 4120 6469 6374 696f 6e61 7279  cs: A dictionary
+00001110: 206f 6620 7370 6563 6966 6963 6174 696f   of specificatio
+00001120: 6e73 2073 7563 6820 6173 206d 6f6e 6974  ns such as monit
+00001130: 6f72 696e 6720 7361 6d70 6c69 6e67 2072  oring sampling r
+00001140: 6174 696f 2e0a 0a23 2323 2320 5370 6563  atio...#### Spec
+00001150: 730a 5468 6520 7370 6563 7320 6172 6720  s.The specs arg 
+00001160: 616c 6c6f 7773 2079 6f75 2074 6f20 636f  allows you to co
+00001170: 6e66 6967 7572 6520 7768 6174 2073 686f  nfigure what sho
+00001180: 756c 6420 6265 206d 6f6e 6974 6f72 6564  uld be monitored
+00001190: 2e20 4974 2065 7870 6563 7473 2061 2070  . It expects a p
+000011a0: 7974 686f 6e20 6469 6374 2077 6974 6820  ython dict with 
+000011b0: 7468 6520 666f 6c6c 776f 696e 6720 706f  the follwoing po
+000011c0: 7373 6962 6c65 206b 6579 733a 0a2a 2073  ssible keys:.* s
+000011d0: 616d 706c 696e 675f 7261 7469 6f20 2831  ampling_ratio (1
+000011e0: 293a 2041 206e 756d 6265 7220 6265 7477  ): A number betw
+000011f0: 6565 6e20 3020 616e 6420 3120 666f 7220  een 0 and 1 for 
+00001200: 686f 7720 6f66 7465 6e20 7368 6f75 6c64  how often should
+00001210: 2074 6865 2063 616c 6c20 6265 206c 6f67   the call be log
+00001220: 6765 642e 0a2a 2061 766f 6964 5f6d 6f6e  ged..* avoid_mon
+00001230: 6974 6f72 696e 675f 6578 6365 7074 696f  itoring_exceptio
+00001240: 6e73 2028 4661 6c73 6529 3a20 5768 6574  ns (False): Whet
+00001250: 6865 7220 6f72 206e 6f74 2074 6f20 6c6f  her or not to lo
+00001260: 6720 6f75 7420 746f 204d 6f6e 6120 7768  g out to Mona wh
+00001270: 656e 2074 6865 7265 2069 7320 616e 204f  en there is an O
+00001280: 7065 6e41 4920 6578 6365 7074 696f 6e2e  penAI exception.
+00001290: 2044 6566 6175 6c74 2069 7320 746f 2074   Default is to t
+000012a0: 7261 636b 2065 7863 6570 7469 6f6e 7320  rack exceptions 
+000012b0: 2d20 616e 6420 4d6f 6e61 2077 696c 6c20  - and Mona will 
+000012c0: 616c 6572 7420 796f 7520 6f6e 2074 6869  alert you on thi
+000012d0: 6e67 7320 6c69 6b65 2061 206a 756d 7020  ngs like a jump 
+000012e0: 696e 206e 756d 6265 7220 6f66 2065 7863  in number of exc
+000012f0: 6570 7469 6f6e 730a 2a20 6578 706f 7274  eptions.* export
+00001300: 5f70 726f 6d70 7420 2846 616c 7365 293a  _prompt (False):
+00001310: 2057 6865 7468 6572 204d 6f6e 6120 7368   Whether Mona sh
+00001320: 6f75 6c64 2065 7870 6f72 7420 7468 6520  ould export the 
+00001330: 6163 7475 616c 2070 726f 6d70 7420 7465  actual prompt te
+00001340: 7874 2e20 4265 2064 6566 6175 6c74 2073  xt. Be default s
+00001350: 6574 2074 6f20 4661 6c73 6520 746f 2061  et to False to a
+00001360: 766f 6964 2070 7269 7661 6379 2063 6f6e  void privacy con
+00001370: 6365 726e 732e 0a2a 2065 7870 6f72 745f  cerns..* export_
+00001380: 7265 7370 6f6e 7365 5f74 6578 7473 2028  response_texts (
+00001390: 4661 6c73 6529 3a20 5768 6574 6865 7220  False): Whether 
+000013a0: 4d6f 6e61 2073 686f 756c 6420 6578 706f  Mona should expo
+000013b0: 7274 2074 6865 2061 6374 7561 6c20 7265  rt the actual re
+000013c0: 7370 6f6e 7365 2074 6578 7473 2e20 4265  sponse texts. Be
+000013d0: 2064 6566 6175 6c74 2073 6574 2074 6f20   default set to 
+000013e0: 4661 6c73 6520 746f 2061 766f 6964 2070  False to avoid p
+000013f0: 7269 7661 6379 2063 6f6e 6365 726e 732e  rivacy concerns.
+00001400: 0a2a 2061 6e61 6c79 7369 733a 2041 2064  .* analysis: A d
+00001410: 6963 7469 6f6e 6172 7920 6d61 7070 696e  ictionary mappin
+00001420: 6720 6561 6368 2061 6e61 6c79 7369 7320  g each analysis 
+00001430: 7479 7065 2074 6f20 6120 626f 6f6c 6561  type to a boolea
+00001440: 6e20 7661 6c75 6520 7465 6c6c 696e 6720  n value telling 
+00001450: 7468 6520 636c 6965 6e74 2077 6865 7468  the client wheth
+00001460: 6572 206f 7220 6e6f 7420 746f 2072 756e  er or not to run
+00001470: 2073 6169 6420 616e 616c 7973 6973 2061   said analysis a
+00001480: 6e64 206c 6f67 2069 7420 746f 204d 6f6e  nd log it to Mon
+00001490: 612e 2050 6f73 7369 626c 6520 6f70 7469  a. Possible opti
+000014a0: 6f6e 7320 6375 7272 656e 746c 7920 6172  ons currently ar
+000014b0: 6520 2270 7269 7661 6379 222c 2022 7072  e "privacy", "pr
+000014c0: 6f66 616e 6974 7922 2c20 616e 6420 2274  ofanity", and "t
+000014d0: 6578 7475 616c 222e 2042 7920 6465 6661  extual". By defa
+000014e0: 756c 742c 2061 6c6c 2061 6e61 6c79 7365  ult, all analyse
+000014f0: 7320 7461 6b65 2070 6c61 6365 2061 6e64  s take place and
+00001500: 2061 7265 206c 6f67 6765 6420 6f75 7420   are logged out 
+00001510: 746f 204d 6f6e 612e 0a0a 2323 2320 5573  to Mona...### Us
+00001520: 696e 6720 6375 7374 6f6d 206c 6f67 6765  ing custom logge
+00001530: 7273 0a59 6f75 2064 6f6e 2774 2068 6176  rs.You don't hav
+00001540: 6520 746f 2068 6176 6520 6120 4d6f 6e61  e to have a Mona
+00001550: 2061 6363 6f75 6e74 2074 6f20 7573 6520   account to use 
+00001560: 7468 6973 2070 6163 6b61 6765 2e20 596f  this package. Yo
+00001570: 7520 6361 6e20 6465 6669 6e65 2073 7065  u can define spe
+00001580: 6369 6669 6320 6c6f 6767 6572 7320 746f  cific loggers to
+00001590: 206c 6f67 206f 7574 2074 6865 2064 6174   log out the dat
+000015a0: 6120 746f 2061 2066 696c 652c 206d 656d  a to a file, mem
+000015b0: 6f72 792c 206f 7220 6a75 7374 2061 2067  ory, or just a g
+000015c0: 6976 656e 2070 7974 686f 6e20 6c6f 6767  iven python logg
+000015d0: 6572 2e20 466f 7220 6578 616d 706c 652c  er. For example,
+000015e0: 2074 6f20 6c6f 6720 6f75 7420 7468 6520   to log out the 
+000015f0: 7265 6c65 7661 6e74 206d 6574 7269 6373  relevant metrics
+00001600: 2061 7320 5741 524e 494e 473a 0a0a 6060   as WARNING:..``
+00001610: 6070 790a 6672 6f6d 206f 7320 696d 706f  `py.from os impo
+00001620: 7274 2065 6e76 6972 6f6e 0a69 6d70 6f72  rt environ.impor
+00001630: 7420 6f70 656e 6169 0a66 726f 6d20 6d6f  t openai.from mo
+00001640: 6e61 5f6f 7065 6e61 692e 6c6f 6767 6572  na_openai.logger
+00001650: 7320 696d 706f 7274 2053 7461 6e64 6172  s import Standar
+00001660: 644c 6f67 6765 720a 6672 6f6d 206c 6f67  dLogger.from log
+00001670: 6769 6e67 2069 6d70 6f72 7420 5741 524e  ging import WARN
+00001680: 494e 470a 0a66 726f 6d20 6d6f 6e61 5f6f  ING..from mona_o
+00001690: 7065 6e61 6920 696d 706f 7274 206d 6f6e  penai import mon
+000016a0: 6974 6f72 5f77 6974 685f 6c6f 6767 6572  itor_with_logger
+000016b0: 0a0a 6f70 656e 6169 2e61 7069 5f6b 6579  ..openai.api_key
+000016c0: 203d 2065 6e76 6972 6f6e 2e67 6574 2822   = environ.get("
+000016d0: 4f50 454e 5f41 495f 4b45 5922 290a 0a6d  OPEN_AI_KEY")..m
+000016e0: 6f6e 6974 6f72 6564 5f63 6f6d 706c 6574  onitored_complet
+000016f0: 696f 6e20 3d20 6d6f 6e69 746f 725f 7769  ion = monitor_wi
+00001700: 7468 5f6c 6f67 6765 7228 0a20 2020 206f  th_logger(.    o
+00001710: 7065 6e61 692e 436f 6d70 6c65 7469 6f6e  penai.Completion
+00001720: 2c0a 2020 2020 5374 616e 6461 7264 4c6f  ,.    StandardLo
+00001730: 6767 6572 2857 4152 4e49 4e47 292c 0a29  gger(WARNING),.)
+00001740: 0a0a 7265 7370 6f6e 7365 203d 206d 6f6e  ..response = mon
+00001750: 6974 6f72 6564 5f63 6f6d 706c 6574 696f  itored_completio
+00001760: 6e2e 6372 6561 7465 280a 2020 2020 6d6f  n.create(.    mo
+00001770: 6465 6c3d 2274 6578 742d 6164 612d 3030  del="text-ada-00
+00001780: 3122 2c0a 2020 2020 7072 6f6d 7074 3d22  1",.    prompt="
+00001790: 4920 7761 6e74 2074 6f20 6765 6e65 7261  I want to genera
+000017a0: 7465 2073 6f6d 6520 7465 7874 2061 626f  te some text abo
+000017b0: 7574 2022 2c0a 2020 2020 6d61 785f 746f  ut ",.    max_to
+000017c0: 6b65 6e73 3d32 302c 0a20 2020 206e 3d31  kens=20,.    n=1
+000017d0: 2c0a 2020 2020 7465 6d70 6572 6174 7572  ,.    temperatur
+000017e0: 653d 302e 322c 0a20 2020 2023 2041 6464  e=0.2,.    # Add
+000017f0: 696e 6720 6164 6469 7469 6f6e 616c 2069  ing additional i
+00001800: 6e66 6f72 6d61 7469 6f6e 2066 6f72 206d  nformation for m
+00001810: 6f6e 6974 6f72 696e 6720 7075 7270 6f73  onitoring purpos
+00001820: 6573 2c20 756e 7265 6c61 7465 6420 746f  es, unrelated to
+00001830: 0a20 2020 2023 2069 6e74 6572 6e61 6c20  .    # internal 
+00001840: 4f70 656e 4149 2063 616c 6c2e 0a20 2020  OpenAI call..   
+00001850: 204d 4f4e 415f 6164 6469 7469 6f6e 616c   MONA_additional
+00001860: 5f64 6174 613d 7b22 6375 7374 6f6d 6572  _data={"customer
+00001870: 5f69 6422 3a20 2241 3533 3132 3531 227d  _id": "A531251"}
+00001880: 2c0a 290a 6060 600a 0a54 6869 7320 5344  ,.).```..This SD
+00001890: 4b20 7072 6f76 6964 6573 2061 2073 696d  K provides a sim
+000018a0: 706c 6520 696e 7465 7266 6163 6520 746f  ple interface to
+000018b0: 2069 6d70 6c65 6d65 6e74 2079 6f75 7220   implement your 
+000018c0: 6f77 6e20 6c6f 6767 6572 7320 6279 2069  own loggers by i
+000018d0: 6e68 6572 6974 696e 6720 6672 6f6d 204c  nheriting from L
+000018e0: 6f67 6765 7220 756e 6465 7220 6c6f 6767  ogger under logg
+000018f0: 6572 732f 6c6f 6767 6572 2e70 792e 0a41  ers/logger.py..A
+00001900: 6c74 6572 6e61 7469 7665 6c79 2c20 6279  lternatively, by
+00001910: 2075 7369 6e67 2074 6865 2073 7461 6e64   using the stand
+00001920: 6172 6420 7079 7468 6f6e 206c 6f67 6769  ard python loggi
+00001930: 6e67 206c 6962 7261 7279 2061 7320 696e  ng library as in
+00001940: 2074 6865 2065 7861 6d70 6c65 2c20 796f   the example, yo
+00001950: 7520 6361 6e20 6372 6561 7465 206c 6f67  u can create log
+00001960: 6769 6e67 2068 616e 646c 6572 7320 746f  ging handlers to
+00001970: 206c 6f67 2074 6865 2064 6174 6120 6f75   log the data ou
+00001980: 7420 746f 2061 6e79 206d 6563 6861 6e69  t to any mechani
+00001990: 736d 2079 6f75 2063 686f 6f73 6520 2865  sm you choose (e
+000019a0: 2e67 2e2c 204b 6166 6b61 2c20 4c6f 6773  .g., Kafka, Logs
+000019b0: 7461 7368 2c20 6574 632e 2e2e 290a 0a23  tash, etc...)..#
+000019c0: 2323 2043 6170 6162 696c 6974 6965 7320  ## Capabilities 
+000019d0: 6475 7269 6e67 2041 5049 2063 616c 6c73  during API calls
+000019e0: 0a0a 4166 7465 7220 7772 6170 7069 6e67  ..After wrapping
+000019f0: 2079 6f75 7220 656e 6470 6f69 6e74 2077   your endpoint w
+00001a00: 6974 6820 606d 6f6e 6974 6f72 602c 2079  ith `monitor`, y
+00001a10: 6f75 2072 6561 6c6c 7920 646f 6e27 7420  ou really don't 
+00001a20: 6e65 6564 2074 6f20 646f 2061 6e79 7468  need to do anyth
+00001a30: 696e 6720 656c 7365 2e20 5768 656e 2075  ing else. When u
+00001a40: 7369 6e67 2060 6372 6561 7465 6020 6f72  sing `create` or
+00001a50: 2060 6163 7265 6174 6560 2064 6174 6120   `acreate` data 
+00001a60: 7769 6c6c 2062 6520 7472 6163 6b65 6420  will be tracked 
+00001a70: 616e 6420 6d6f 6e69 746f 7269 6e67 2077  and monitoring w
+00001a80: 696c 6c20 7461 6b65 2070 6c61 6365 2e0a  ill take place..
+00001a90: 0a54 6865 7265 2061 7265 2c20 686f 7765  .There are, howe
+00001aa0: 7665 722c 2073 6576 6572 616c 2063 6170  ver, several cap
+00001ab0: 6162 696c 6974 6965 7320 7468 6174 2061  abilities that a
+00001ac0: 7265 2061 6464 6564 2074 6f20 7468 6573  re added to thes
+00001ad0: 6520 6675 6e63 7469 6f6e 732e 2053 7065  e functions. Spe
+00001ae0: 6369 6669 6361 6c6c 792c 2079 6f75 2063  cifically, you c
+00001af0: 616e 2061 6464 2074 6865 2066 6f6c 6c6f  an add the follo
+00001b00: 7769 6e67 2061 7267 756d 656e 7473 2074  wing arguments t
+00001b10: 6f20 616e 7920 6372 6561 7465 2063 616c  o any create cal
+00001b20: 6c3a 0a2a 204d 4f4e 415f 636f 6e74 6578  l:.* MONA_contex
+00001b30: 745f 6964 3a20 5468 6520 756e 6971 7565  t_id: The unique
+00001b40: 2069 6420 6f66 2074 6865 2063 6f6e 7465   id of the conte
+00001b50: 7874 2069 6e20 7768 6963 6820 7468 6520  xt in which the 
+00001b60: 6361 6c6c 2069 7320 6d61 6465 2e20 4279  call is made. By
+00001b70: 2075 7369 6e67 2074 6869 7320 4944 2079   using this ID y
+00001b80: 6f75 2063 616e 2065 7870 6f72 7420 6d6f  ou can export mo
+00001b90: 7265 2064 6174 6120 746f 204d 6f6e 6120  re data to Mona 
+00001ba0: 746f 2074 6865 2073 616d 6520 636f 6e74  to the same cont
+00001bb0: 6578 7420 6672 6f6d 206f 7468 6572 2070  ext from other p
+00001bc0: 6c61 6365 732e 2049 6620 6e6f 7420 7375  laces. If not su
+00001bd0: 7070 6c69 6564 2c20 7468 6520 2269 6422  pplied, the "id"
+00001be0: 2066 6965 6c64 206f 6620 7468 6520 4f70   field of the Op
+00001bf0: 656e 4149 2045 6e64 706f 696e 7427 7320  enAI Endpoint's 
+00001c00: 7265 7370 6f6e 7365 2077 696c 6c20 6265  response will be
+00001c10: 2075 7365 6420 6173 2074 6865 204d 6f6e   used as the Mon
+00001c20: 6120 636f 6e74 6578 7420 4944 2061 7574  a context ID aut
+00001c30: 6f6d 6174 6963 616c 6c79 2e0a 2a20 4d4f  omatically..* MO
+00001c40: 4e41 5f65 7870 6f72 745f 7469 6d65 7374  NA_export_timest
+00001c50: 616d 703a 2043 616e 2062 6520 7573 6564  amp: Can be used
+00001c60: 2074 6f20 7369 6d75 6c61 7465 2061 7320   to simulate as 
+00001c70: 6966 2074 6865 2063 7572 7265 6e74 2063  if the current c
+00001c80: 616c 6c20 7761 7320 6d61 6465 2069 6e20  all was made in 
+00001c90: 6120 6469 6666 6572 656e 7420 7469 6d65  a different time
+00001ca0: 2c20 6173 2066 6172 2061 7320 4d6f 6e61  , as far as Mona
+00001cb0: 2069 7320 636f 6e63 6572 6e65 642e 0a2a   is concerned..*
+00001cc0: 204d 4f4e 415f 6164 6469 7469 6f6e 616c   MONA_additional
+00001cd0: 5f64 6174 613a 2041 204a 534f 4e2d 7365  _data: A JSON-se
+00001ce0: 7269 616c 697a 6162 6c65 2064 6963 7420  rializable dict 
+00001cf0: 7769 7468 2061 6e79 206f 7468 6572 2064  with any other d
+00001d00: 6174 6120 796f 7520 7761 6e74 2074 6f20  ata you want to 
+00001d10: 6164 6420 746f 2074 6865 206d 6f6e 6974  add to the monit
+00001d20: 6f72 696e 6720 636f 6e74 6578 742e 2054  oring context. T
+00001d30: 6869 7320 636f 6d65 7320 696e 2068 616e  his comes in han
+00001d40: 6479 2069 6620 796f 7520 7761 6e74 2074  dy if you want t
+00001d50: 6f20 6164 6420 6d6f 7265 2069 6e66 6f72  o add more infor
+00001d60: 6d61 7469 6f6e 2074 6f20 7468 6520 6d6f  mation to the mo
+00001d70: 6e69 746f 7269 6e67 2063 6f6e 7465 7820  nitoring contex 
+00001d80: 7468 6174 2069 736e 2774 2070 6172 7420  that isn't part 
+00001d90: 6f66 2074 6865 2062 6173 6963 204f 7065  of the basic Ope
+00001da0: 6e41 4920 4150 4920 6361 6c6c 2069 6e66  nAI API call inf
+00001db0: 6f72 6d61 7469 6f6e 2e20 466f 7220 6578  ormation. For ex
+00001dc0: 616d 706c 652c 2069 6620 796f 7520 6172  ample, if you ar
+00001dd0: 6520 7573 696e 6720 6120 7370 6563 6966  e using a specif
+00001de0: 6963 2074 656d 706c 6174 6520 4944 206f  ic template ID o
+00001df0: 7220 6966 2074 6869 7320 6361 6c6c 2069  r if this call i
+00001e00: 7320 6265 696e 6720 6d61 6465 2066 6f72  s being made for
+00001e10: 2061 2073 7065 6369 6669 6320 6375 7374   a specific cust
+00001e20: 6f6d 6572 2049 442c 2074 6865 7365 2061  omer ID, these a
+00001e30: 7265 2066 6965 6c64 7320 796f 7520 6361  re fields you ca
+00001e40: 6e20 6164 6420 7468 6572 6520 746f 2068  n add there to h
+00001e50: 656c 7020 6765 7420 6675 6c6c 2063 6f6e  elp get full con
+00001e60: 7465 7874 2077 6865 6e20 6d6f 6e69 746f  text when monito
+00001e70: 7269 6e67 2077 6974 6820 4d6f 6e61 2e0a  ring with Mona..
+00001e80: 0a45 7861 6d70 6c65 3a0a 6060 6070 790a  .Example:.```py.
+00001e90: 7265 7370 6f6e 7365 203d 2061 7379 6e63  response = async
+00001ea0: 696f 2e72 756e 286d 6f6e 6974 6f72 6564  io.run(monitored
+00001eb0: 5f63 6f6d 706c 6574 696f 6e2e 6163 7265  _completion.acre
+00001ec0: 6174 6528 0a20 2020 2065 6e67 696e 653d  ate(.    engine=
+00001ed0: 6d6f 6465 6c2c 0a20 2020 2070 726f 6d70  model,.    promp
+00001ee0: 743d 7072 6f6d 7074 2c0a 2020 2020 6d61  t=prompt,.    ma
+00001ef0: 785f 746f 6b65 6e73 3d6d 6178 5f74 6f6b  x_tokens=max_tok
+00001f00: 656e 732c 0a20 2020 206e 3d6e 2c0a 2020  ens,.    n=n,.  
+00001f10: 2020 7465 6d70 6572 6174 7572 653d 7465    temperature=te
+00001f20: 6d70 6572 6174 7572 652c 0a20 2020 204d  mperature,.    M
+00001f30: 4f4e 415f 6164 6469 7469 6f6e 616c 5f64  ONA_additional_d
+00001f40: 6174 613d 7b22 6375 7374 6f6d 6572 5f69  ata={"customer_i
+00001f50: 6422 3a20 2241 3533 3132 3531 227d 2c0a  d": "A531251"},.
+00001f60: 2929 0a70 7269 6e74 2872 6573 706f 6e73  )).print(respons
+00001f70: 652e 6368 6f69 6365 735b 305d 2e74 6578  e.choices[0].tex
+00001f80: 7429 0a60 6060 0a0a 2323 2320 5573 696e  t).```..### Usin
+00001f90: 6720 4f70 656e 4149 2077 6974 6820 5245  g OpenAI with RE
+00001fa0: 5354 2063 616c 6c73 2069 6e73 7465 6164  ST calls instead
+00001fb0: 206f 6620 4f70 656e 4149 2773 2050 7974   of OpenAI's Pyt
+00001fc0: 686f 6e20 636c 6965 6e74 0a49 6e20 736f  hon client.In so
+00001fd0: 6d65 2063 6173 6573 2079 6f75 206d 6179  me cases you may
+00001fe0: 2063 686f 6f73 6520 746f 2075 7365 204f   choose to use O
+00001ff0: 7065 6e41 4927 7320 4150 4920 6469 7265  penAI's API dire
+00002000: 6374 6c79 2077 6974 6820 5245 5354 2063  ctly with REST c
+00002010: 616c 6c73 2061 6e64 206e 6f74 2075 7369  alls and not usi
+00002020: 6e67 204f 7065 6e41 4927 7320 5344 4b2e  ng OpenAI's SDK.
+00002030: 2046 6f72 2074 6865 7365 2063 6173 6573   For these cases
+00002040: 2077 6520 616c 6c6f 7720 6120 6d6f 7265   we allow a more
+00002050: 2064 6972 6563 7420 6170 7072 6f61 6368   direct approach
+00002060: 2066 6f72 206c 6f67 6769 6e67 2074 6f20   for logging to 
+00002070: 4d6f 6e61 2061 7320 7765 6c6c 2c20 6279  Mona as well, by
+00002080: 2075 7369 6e67 2074 6865 2022 6765 745f   using the "get_
+00002090: 7265 7374 5f6d 6f6e 6974 6f72 2220 6675  rest_monitor" fu
+000020a0: 6e63 7469 6f6e 2e20 5365 6520 6578 616d  nction. See exam
+000020b0: 706c 6520 6265 6c6f 772e 0a0a 6060 6070  ple below...```p
+000020c0: 790a 2320 4469 7265 6374 2052 4553 5420  y.# Direct REST 
+000020d0: 7573 6167 652c 2077 6974 686f 7574 204f  usage, without O
+000020e0: 7065 6e41 4920 636c 6965 6e74 0a69 6d70  penAI client.imp
+000020f0: 6f72 7420 7265 7175 6573 7473 0a66 726f  ort requests.fro
+00002100: 6d20 6f73 2069 6d70 6f72 7420 656e 7669  m os import envi
+00002110: 726f 6e0a 6672 6f6d 206d 6f6e 615f 6f70  ron.from mona_op
+00002120: 656e 6169 2069 6d70 6f72 7420 6765 745f  enai import get_
+00002130: 7265 7374 5f6d 6f6e 6974 6f72 0a0a 0a4d  rest_monitor...M
+00002140: 4f4e 415f 4150 495f 4b45 5920 3d20 656e  ONA_API_KEY = en
+00002150: 7669 726f 6e2e 6765 7428 224d 4f4e 415f  viron.get("MONA_
+00002160: 4150 495f 4b45 5922 290a 4d4f 4e41 5f53  API_KEY").MONA_S
+00002170: 4543 5245 5420 3d20 656e 7669 726f 6e2e  ECRET = environ.
+00002180: 6765 7428 224d 4f4e 415f 5345 4352 4554  get("MONA_SECRET
+00002190: 2229 0a4d 4f4e 415f 4352 4544 5320 3d20  ").MONA_CREDS = 
+000021a0: 7b0a 2020 2020 226b 6579 223a 204d 4f4e  {.    "key": MON
+000021b0: 415f 4150 495f 4b45 592c 0a20 2020 2022  A_API_KEY,.    "
+000021c0: 7365 6372 6574 223a 204d 4f4e 415f 5345  secret": MONA_SE
+000021d0: 4352 4554 2c0a 7d0a 434f 4e54 4558 545f  CRET,.}.CONTEXT_
+000021e0: 434c 4153 535f 4e41 4d45 203d 2022 534f  CLASS_NAME = "SO
+000021f0: 4d45 5f4d 4f4e 4954 4f52 494e 475f 434f  ME_MONITORING_CO
+00002200: 4e54 4558 545f 4e41 4d45 220a 0a23 2047  NTEXT_NAME"..# G
+00002210: 6574 204d 6f6e 6120 6c6f 6767 6572 0a6d  et Mona logger.m
+00002220: 6f6e 615f 6c6f 6767 6572 203d 2067 6574  ona_logger = get
+00002230: 5f72 6573 745f 6d6f 6e69 746f 7228 0a20  _rest_monitor(. 
+00002240: 2020 2022 436f 6d70 6c65 7469 6f6e 222c     "Completion",
+00002250: 0a20 2020 204d 4f4e 415f 4352 4544 532c  .    MONA_CREDS,
+00002260: 0a20 2020 2043 4f4e 5445 5854 5f43 4c41  .    CONTEXT_CLA
+00002270: 5353 5f4e 414d 452c 0a29 0a0a 2320 5365  SS_NAME,.)..# Se
+00002280: 7420 7570 2074 6865 2041 5049 2065 6e64  t up the API end
+00002290: 706f 696e 7420 5552 4c20 616e 6420 6175  point URL and au
+000022a0: 7468 656e 7469 6361 7469 6f6e 2068 6561  thentication hea
+000022b0: 6465 7273 0a75 726c 203d 2022 6874 7470  ders.url = "http
+000022c0: 733a 2f2f 6170 692e 6f70 656e 6169 2e63  s://api.openai.c
+000022d0: 6f6d 2f76 312f 636f 6d70 6c65 7469 6f6e  om/v1/completion
+000022e0: 7322 0a68 6561 6465 7273 203d 207b 0a20  s".headers = {. 
+000022f0: 2020 2022 436f 6e74 656e 742d 5479 7065     "Content-Type
+00002300: 223a 2022 6170 706c 6963 6174 696f 6e2f  ": "application/
+00002310: 6a73 6f6e 222c 0a20 2020 2022 4175 7468  json",.    "Auth
+00002320: 6f72 697a 6174 696f 6e22 3a20 6622 4265  orization": f"Be
+00002330: 6172 6572 207b 656e 7669 726f 6e2e 6765  arer {environ.ge
+00002340: 7428 274f 5045 4e5f 4149 5f4b 4559 2729  t('OPEN_AI_KEY')
+00002350: 7d22 2c0a 7d0a 0a23 2053 6574 2075 7020  }",.}..# Set up 
+00002360: 7468 6520 7265 7175 6573 7420 6461 7461  the request data
+00002370: 0a64 6174 6120 3d20 7b0a 2020 2020 2270  .data = {.    "p
+00002380: 726f 6d70 7422 3a20 7072 6f6d 7074 2c0a  rompt": prompt,.
+00002390: 2020 2020 226d 6178 5f74 6f6b 656e 7322      "max_tokens"
+000023a0: 3a20 6d61 785f 746f 6b65 6e73 2c0a 2020  : max_tokens,.  
+000023b0: 2020 2274 656d 7065 7261 7475 7265 223a    "temperature":
+000023c0: 2074 656d 7065 7261 7475 7265 2c0a 2020   temperature,.  
+000023d0: 2020 226d 6f64 656c 223a 206d 6f64 656c    "model": model
+000023e0: 2c0a 2020 2020 226e 223a 206e 2c0a 7d0a  ,.    "n": n,.}.
+000023f0: 0a23 2054 6865 206c 6f67 5f72 6571 7565  .# The log_reque
+00002400: 7374 2066 756e 6374 696f 6e20 7265 7475  st function retu
+00002410: 726e 7320 7477 6f20 6f74 6865 7220 6675  rns two other fu
+00002420: 6e63 7469 6f6e 2066 6f72 206c 6174 6572  nction for later
+00002430: 206c 6f67 6769 6e67 0a23 2074 6865 2072   logging.# the r
+00002440: 6573 706f 6e73 6520 6f72 2074 6865 2065  esponse or the e
+00002450: 7863 6570 7469 6f6e 2e20 5768 656e 2077  xception. When w
+00002460: 6520 6c61 7465 7220 646f 2074 6861 742c  e later do that,
+00002470: 2074 6865 206c 6f67 6765 7220 7769 6c6c   the logger will
+00002480: 0a23 2061 6374 7561 6c6c 7920 6361 6c63  .# actually calc
+00002490: 756c 6174 6520 616c 6c20 7468 6520 7265  ulate all the re
+000024a0: 6c65 7661 6e74 206d 6574 7269 6373 2061  levant metrics a
+000024b0: 6e64 2077 696c 6c20 7365 6e64 2074 6865  nd will send the
+000024c0: 6d20 746f 0a23 204d 6f6e 612e 0a72 6573  m to.# Mona..res
+000024d0: 706f 6e73 655f 6c6f 6767 6572 2c20 6578  ponse_logger, ex
+000024e0: 6365 7074 696f 6e5f 6c6f 6767 6572 203d  ception_logger =
+000024f0: 206d 6f6e 615f 6c6f 6767 6572 2e6c 6f67   mona_logger.log
+00002500: 5f72 6571 7565 7374 280a 2020 2020 6461  _request(.    da
+00002510: 7461 2c20 6164 6469 7469 6f6e 616c 5f64  ta, additional_d
+00002520: 6174 613d 7b22 6375 7374 6f6d 6572 5f69  ata={"customer_i
+00002530: 6422 3a20 2241 3533 3132 3531 227d 0a29  d": "A531251"}.)
+00002540: 0a0a 7472 793a 0a20 2020 2023 2053 656e  ..try:.    # Sen
+00002550: 6420 7468 6520 7265 7175 6573 7420 746f  d the request to
+00002560: 2074 6865 2041 5049 0a20 2020 2072 6573   the API.    res
+00002570: 706f 6e73 6520 3d20 7265 7175 6573 7473  ponse = requests
+00002580: 2e70 6f73 7428 7572 6c2c 2068 6561 6465  .post(url, heade
+00002590: 7273 3d68 6561 6465 7273 2c20 6a73 6f6e  rs=headers, json
+000025a0: 3d64 6174 6129 0a0a 2020 2020 2320 4368  =data)..    # Ch
+000025b0: 6563 6b20 666f 7220 4854 5450 2065 7272  eck for HTTP err
+000025c0: 6f72 730a 2020 2020 7265 7370 6f6e 7365  ors.    response
+000025d0: 2e72 6169 7365 5f66 6f72 5f73 7461 7475  .raise_for_statu
+000025e0: 7328 290a 0a20 2020 2023 204c 6f67 2072  s()..    # Log r
+000025f0: 6573 706f 6e73 6520 746f 204d 6f6e 610a  esponse to Mona.
+00002600: 2020 2020 7265 7370 6f6e 7365 5f6c 6f67      response_log
+00002610: 6765 7228 7265 7370 6f6e 7365 2e6a 736f  ger(response.jso
+00002620: 6e28 2929 0a20 2020 2070 7269 6e74 2872  n()).    print(r
+00002630: 6573 706f 6e73 652e 6a73 6f6e 2829 5b22  esponse.json()["
+00002640: 6368 6f69 6365 7322 5d5b 305d 5b22 7465  choices"][0]["te
+00002650: 7874 225d 290a 0a65 7863 6570 7420 4578  xt"])..except Ex
+00002660: 6365 7074 696f 6e20 6173 2065 7272 3a0a  ception as err:.
+00002670: 2020 2020 2320 4c6f 6720 6578 6365 7074      # Log except
+00002680: 696f 6e20 746f 204d 6f6e 610a 2020 2020  ion to Mona.    
+00002690: 6578 6365 7074 696f 6e5f 6c6f 6767 6572  exception_logger
+000026a0: 2829 0a60 6060 0a0a 2323 2320 5374 7265  ().```..### Stre
+000026b0: 616d 2073 7570 706f 7274 0a0a 4f70 656e  am support..Open
+000026c0: 4149 2061 6c6c 6f77 7320 7265 6365 6976  AI allows receiv
+000026d0: 696e 6720 7265 7370 6f6e 7365 7320 6173  ing responses as
+000026e0: 2061 2073 7472 6561 6d20 6f66 2074 6f6b   a stream of tok
+000026f0: 656e 7320 7573 696e 6720 7468 6520 2273  ens using the "s
+00002700: 7472 6561 6d22 2070 6172 616d 6574 6572  tream" parameter
+00002710: 2e20 5768 656e 2074 6869 7320 6973 2064  . When this is d
+00002720: 6f6e 652c 204d 6f6e 6120 7769 6c6c 2063  one, Mona will c
+00002730: 6f6c 6c65 6374 2061 6c6c 2074 6865 2074  ollect all the t
+00002740: 6f6b 656e 7320 696e 206d 656d 6f72 7920  okens in memory 
+00002750: 616e 6420 7769 6c6c 2063 7265 6174 6520  and will create 
+00002760: 7468 6520 616e 616c 7973 6973 2061 6e64  the analysis and
+00002770: 206c 6f67 206f 7574 2074 6865 2064 6174   log out the dat
+00002780: 6120 7468 6520 6d6f 6d65 6e74 2074 6865  a the moment the
+00002790: 2073 7472 6561 6d20 6973 206f 7665 722e   stream is over.
+000027a0: 2059 6f75 2064 6f6e 2774 206e 6565 6420   You don't need 
+000027b0: 746f 2064 6f20 616e 7974 6869 6e67 2074  to do anything t
+000027c0: 6f20 6d61 6b65 2074 6869 7320 6861 7070  o make this happ
+000027d0: 656e 2e0a 0a53 696e 6365 2066 6f72 2073  en...Since for s
+000027e0: 7472 6561 6d69 6e67 2072 6573 706f 6e73  treaming respons
+000027f0: 6573 204f 7065 6e41 4920 646f 6573 6e27  es OpenAI doesn'
+00002800: 7420 7375 7070 6c79 2074 6865 2066 756c  t supply the ful
+00002810: 6c20 7573 6167 6520 746f 6b65 6e73 2073  l usage tokens s
+00002820: 756d 6d61 7279 2c20 4d6f 6e61 2075 7365  ummary, Mona use
+00002830: 7320 7468 6520 7469 6b74 6f6b 656e 2070  s the tiktoken p
+00002840: 6163 6b61 6765 2074 6f20 6361 6c63 756c  ackage to calcul
+00002850: 6174 6520 7468 6520 746f 6b65 6e73 206f  ate the tokens o
+00002860: 6620 7468 6520 7072 6f6d 7074 2061 6e64  f the prompt and
+00002870: 2063 6f6d 706c 6574 696f 6e20 616e 6420   completion and 
+00002880: 6c6f 6720 7468 656d 2066 6f72 206d 6f6e  log them for mon
+00002890: 6974 6f72 696e 672e 0a0a 4e4f 5445 3a20  itoring...NOTE: 
+000028a0: 5374 7265 616d 2069 7320 6375 7272 656e  Stream is curren
+000028b0: 746c 7920 6f6e 6c79 2073 7570 706f 7274  tly only support
+000028c0: 6564 2077 6974 6820 5344 4b20 7573 6167  ed with SDK usag
+000028d0: 652c 2061 6e64 206e 6f74 2077 6974 6820  e, and not with 
+000028e0: 7573 696e 6720 5245 5354 2064 6972 6563  using REST direc
+000028f0: 746c 792e 0a0a 2323 204c 616e 6743 6861  tly...## LangCha
+00002900: 696e 2073 7570 706f 7274 0a0a 596f 7520  in support..You 
+00002910: 6361 6e20 7573 6520 7468 6520 6578 706f  can use the expo
+00002920: 7274 6564 2060 6d6f 6e69 746f 725f 6c61  rted `monitor_la
+00002930: 6e67 6368 6169 6e5f 6c6c 6d60 2074 6f20  ngchain_llm` to 
+00002940: 7772 6170 2061 204c 616e 6743 6861 696e  wrap a LangChain
+00002950: 204f 7065 6e41 4920 4c4c 4d20 2863 6861   OpenAI LLM (cha
+00002960: 7420 6f72 206e 6f72 6d61 6c29 2077 6974  t or normal) wit
+00002970: 6820 4d6f 6e61 2773 206d 6f6e 6974 6f72  h Mona's monitor
+00002980: 696e 6720 6361 7061 6269 6c69 7469 6573  ing capabilities
+00002990: 3a0a 0a60 6060 7079 0a66 726f 6d20 6d6f  :..```py.from mo
+000029a0: 6e61 5f6f 7065 6e61 6920 696d 706f 7274  na_openai import
+000029b0: 206d 6f6e 6974 6f72 5f6c 616e 6763 6861   monitor_langcha
+000029c0: 696e 5f6c 6c6d 0a0a 6672 6f6d 206c 616e  in_llm..from lan
+000029d0: 6763 6861 696e 2e6c 6c6d 7320 696d 706f  gchain.llms impo
+000029e0: 7274 204f 7065 6e41 490a 0a23 2057 7261  rt OpenAI..# Wra
+000029f0: 7020 7468 6520 4c4c 4d20 6f62 6a65 6374  p the LLM object
+00002a00: 2077 6974 6820 4d6f 6e61 206d 6f6e 6974   with Mona monit
+00002a10: 6f72 696e 672e 0a6c 6c6d 203d 206d 6f6e  oring..llm = mon
+00002a20: 6974 6f72 5f6c 616e 6763 6861 696e 5f6c  itor_langchain_l
+00002a30: 6c6d 280a 2020 2020 4f70 656e 4149 284f  lm(.    OpenAI(O
+00002a40: 5045 4e5f 4149 5f4b 4559 292c 0a20 2020  PEN_AI_KEY),.   
+00002a50: 204d 4f4e 415f 4352 4544 532c 0a20 2020   MONA_CREDS,.   
+00002a60: 2043 4f4e 5445 5854 5f43 4c41 5353 5f4e   CONTEXT_CLASS_N
+00002a70: 414d 4529 0a60 6060 0a0a 5365 6520 6675  AME).```..See fu
+00002a80: 6c6c 2065 7861 6d70 6c65 2069 6e20 636f  ll example in co
+00002a90: 6d70 6c65 7469 6f6e 5f6c 616e 6763 6861  mpletion_langcha
+00002aa0: 696e 2e70 7920 696e 2074 6865 2065 7861  in.py in the exa
+00002ab0: 6d70 6c65 7320 666f 6c64 6572 2e0a 0a23  mples folder...#
+00002ac0: 2320 4d6f 6e61 2053 444b 0a0a 5468 6973  # Mona SDK..This
+00002ad0: 2070 6163 6b61 6765 2075 7365 7320 7468   package uses th
+00002ae0: 6520 6d6f 6e61 5f73 646b 2070 6163 6b61  e mona_sdk packa
+00002af0: 6765 2074 6f20 6578 706f 7274 2074 6865  ge to export the
+00002b00: 2072 656c 6576 616e 7420 6461 7461 2074   relevant data t
+00002b10: 6f20 4d6f 6e61 2e20 5468 6572 6520 6172  o Mona. There ar
+00002b20: 6520 7365 7665 7261 6c20 656e 7669 726f  e several enviro
+00002b30: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
+00002b40: 796f 7520 6361 6e20 7573 6520 746f 2063  you can use to c
+00002b50: 6f6e 6669 6775 7265 2074 6865 2053 444b  onfigure the SDK
+00002b60: 2773 2062 6568 6176 696f 722e 2046 6f72  's behavior. For
+00002b70: 2065 7861 6d70 6c65 2c20 796f 7520 6361   example, you ca
+00002b80: 6e20 7365 7420 6974 2075 7020 746f 2072  n set it up to r
+00002b90: 6169 7365 2065 7863 6570 7469 6f6e 7320  aise exceptions 
+00002ba0: 7768 656e 2065 7870 6f72 7469 6e67 2064  when exporting d
+00002bb0: 6174 6120 746f 204d 6f6e 6120 6661 696c  ata to Mona fail
+00002bc0: 7320 2869 7420 646f 6573 6e27 7420 646f  s (it doesn't do
+00002bd0: 2074 6861 7420 6279 2064 6566 6175 6c74   that by default
+00002be0: 292e 0a0a 2323 204d 6f6e 6974 6f72 696e  )...## Monitorin
+00002bf0: 6720 666f 7220 7072 6f66 616e 6974 790a  g for profanity.
+00002c00: 0a4d 6f6e 6120 7573 6573 2074 6865 2061  .Mona uses the a
+00002c10: 6c74 2d70 726f 6661 6e69 7479 2d63 6865  lt-profanity-che
+00002c20: 636b 2070 6163 616b 6765 2028 6874 7470  ck pacakge (http
+00002c30: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00002c40: 6a65 6374 2f61 6c74 2d70 726f 6661 6e69  ject/alt-profani
+00002c50: 7479 2d63 6865 636b 2f29 2074 6f20 6372  ty-check/) to cr
+00002c60: 6561 7465 2062 6f74 6820 626f 6f6c 6561  eate both boolea
+00002c70: 6e20 7072 6564 6963 7469 6f6e 7320 616e  n predictions an
+00002c80: 6420 7072 6f62 6162 696c 7479 2073 636f  d probabilty sco
+00002c90: 7265 7320 666f 7220 7468 6520 6578 6973  res for the exis
+00002ca0: 7465 6e63 6520 6f66 2070 726f 6661 6e69  tence of profani
+00002cb0: 7479 2062 6f74 6820 696e 2074 6865 2070  ty both in the p
+00002cc0: 726f 6d70 7420 616e 6420 696e 2074 6865  rompt and in the
+00002cd0: 2072 6573 706f 6e73 6573 2e20 5765 2075   responses. We u
+00002ce0: 7365 2074 6865 2062 7569 6c74 2069 6e20  se the built in 
+00002cf0: 7061 636b 6167 6520 6d65 7468 6f64 7320  package methods 
+00002d00: 666f 7220 7468 6174 2e20 4966 2079 6f75  for that. If you
+00002d10: 2077 616e 742c 2066 6f72 2065 7861 6d70   want, for examp
+00002d20: 6c65 2c20 746f 2075 7365 2061 2064 6966  le, to use a dif
+00002d30: 6665 7265 6e74 2070 726f 6261 6269 6c69  ferent probabili
+00002d40: 7479 2074 6872 6573 686f 6c64 2066 6f72  ty threshold for
+00002d50: 2074 6865 2062 6f6f 6c65 616e 2070 7265   the boolean pre
+00002d60: 6469 6374 696f 6e2c 2079 6f75 2063 616e  diction, you can
+00002d70: 2064 6f20 7468 6174 2062 7920 6368 616e   do that by chan
+00002d80: 6769 6e67 2079 6f75 7220 4d6f 6e61 2063  ging your Mona c
+00002d90: 6f6e 6669 6720 6f6e 2074 6865 204d 6f6e  onfig on the Mon
+00002da0: 6120 6461 7368 626f 6172 642e 0a0a 2323  a dashboard...##
+00002db0: 2055 7369 6e67 206e 6573 742d 6173 796e   Using nest-asyn
+00002dc0: 6369 6f0a 0a49 6e20 656e 7669 726f 6e6d  cio..In environm
+00002dd0: 656e 7473 2069 6e20 7768 6963 6820 7468  ents in which th
+00002de0: 6572 6527 7320 6120 666f 7265 7665 7220  ere's a forever 
+00002df0: 7275 6e6e 696e 6720 6576 656e 7420 6c6f  running event lo
+00002e00: 6f70 2028 652e 672e 2c20 4a75 7079 7465  op (e.g., Jupyte
+00002e10: 7220 6e6f 7465 626f 6f6b 7329 2c20 7468  r notebooks), th
+00002e20: 6520 636c 6965 6e74 206d 6967 6874 2075  e client might u
+00002e30: 7365 205b 6e65 7374 5f61 7379 6e63 696f  se [nest_asyncio
+00002e40: 2e61 7070 6c79 2829 5d28 6874 7470 733a  .apply()](https:
+00002e50: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00002e60: 6374 2f6e 6573 742d 6173 796e 6369 6f2f  ct/nest-asyncio/
+00002e70: 2920 746f 2072 756e 206a 6f69 6e74 2073  ) to run joint s
+00002e80: 796e 6320 616e 6420 6173 796e 6320 636f  ync and async co
+00002e90: 6465 2e                                  de.
```

### Comparing `mona-openai-0.1.0/mona_openai/analysis/privacy.py` & `mona-openai-0.1.1/mona_openai/analysis/privacy.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/analysis/textual.py` & `mona-openai-0.1.1/mona_openai/analysis/textual.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/endpoints/chat_completion.py` & `mona-openai-0.1.1/mona_openai/endpoints/chat_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/endpoints/completion.py` & `mona-openai-0.1.1/mona_openai/endpoints/completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/endpoints/endpoint_wrapping.py` & `mona-openai-0.1.1/mona_openai/endpoints/endpoint_wrapping.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/endpoints/wrapping_getter.py` & `mona-openai-0.1.1/mona_openai/endpoints/wrapping_getter.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/loggers/file_logger.py` & `mona-openai-0.1.1/mona_openai/loggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/loggers/in_memory_logging.py` & `mona-openai-0.1.1/mona_openai/loggers/in_memory_logging.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/loggers/logger.py` & `mona-openai-0.1.1/mona_openai/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/loggers/mona_logger/mona_client.py` & `mona-openai-0.1.1/mona_openai/loggers/mona_logger/mona_client.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/loggers/mona_logger/mona_logger.py` & `mona-openai-0.1.1/mona_openai/loggers/mona_logger/mona_logger.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/loggers/standard_logging.py` & `mona-openai-0.1.1/mona_openai/loggers/standard_logging.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/mona_openai.py` & `mona-openai-0.1.1/mona_openai/mona_openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -369,62 +369,70 @@
         """
 
         @classmethod
         def _inner_log_request(
             cls,
             message_logging_function,
             request_dict,
-            additional_data=None,
+            additional_data=EMPTY_DICT,
             context_id=None,
             export_timestamp=None,
         ):
             """
             Actual logic for logging requests, responses and exceptions.
             """
             start_time = time.time()
 
-            inner_response = None
+            if additional_data is None:
+                additional_data = EMPTY_DICT
 
-            def _inner_log_message(is_exception):
+            def _inner_log_message(
+                is_exception, more_additional_data, response=None
+            ):
                 return message_logging_function(
                     _get_logging_message(
                         api_name=openai_endpoint_name,
                         request_input=request_dict,
                         start_time=start_time,
                         is_exception=is_exception,
                         is_async=False,
                         # TODO(itai): Support stream in REST as well.
                         stream_start_time=None,
-                        response=inner_response,
+                        response=response,
                         analysis_getter=wrapping_logic.get_full_analysis,
                         message_cleaner=wrapping_logic.get_clean_message,
-                        additional_data=additional_data,
+                        additional_data={
+                            **additional_data,
+                            **more_additional_data,
+                        },
                     ),
                     context_id,
                     export_timestamp,
                 )
 
             log_message = add_conditional_sampling(
                 _inner_log_message, sampling_ratio
             )
 
-            def log_response(response):
+            def log_response(response, additional_data=EMPTY_DICT):
                 """
                 Only when this function is called, will data be logged
                 out. This function should be called with a
                 response object from the OpenAI API as close as
                 possible to when it is received to allow accurate
                 latency logging.
                 """
-                nonlocal inner_response
-                inner_response = response
-                return log_message(False)
+                return log_message(
+                    False,
+                    more_additional_data=additional_data,
+                    response=response,
+                )
 
-            def log_exception():
-                return log_message(True)
+            def log_exception(additional_data=EMPTY_DICT):
+                return log_message(True, more_additional_data=additional_data)
 
             return log_response, log_exception
 
         @classmethod
         def log_request(
             cls,
             request_dict,
```

### Comparing `mona-openai-0.1.0/mona_openai/util/func_util.py` & `mona-openai-0.1.1/mona_openai/util/func_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/util/oop_util.py` & `mona-openai-0.1.1/mona_openai/util/oop_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/util/stream_util.py` & `mona-openai-0.1.1/mona_openai/util/stream_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/util/tokens_util.py` & `mona-openai-0.1.1/mona_openai/util/tokens_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai/util/validation_util.py` & `mona-openai-0.1.1/mona_openai/util/validation_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/mona_openai.egg-info/PKG-INFO` & `mona-openai-0.1.1/mona_openai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6f 6e61  : 2.1.Name: mona
 00000020: 2d6f 7065 6e61 690a 5665 7273 696f 6e3a  -openai.Version:
-00000030: 2030 2e31 2e30 0a53 756d 6d61 7279 3a20   0.1.0.Summary: 
+00000030: 2030 2e31 2e31 0a53 756d 6d61 7279 3a20   0.1.1.Summary: 
 00000040: 496e 7465 6772 6174 696f 6e20 636c 6965  Integration clie
 00000050: 6e74 2066 6f72 206d 6f6e 6974 6f72 696e  nt for monitorin
 00000060: 6720 4f70 656e 4149 2075 7361 6765 2077  g OpenAI usage w
 00000070: 6974 6820 4d6f 6e61 0a41 7574 686f 722d  ith Mona.Author-
 00000080: 656d 6169 6c3a 2049 7461 6920 4261 7220  email: Itai Bar 
 00000090: 5369 6e61 6920 3c69 7461 6940 6d6f 6e61  Sinai <itai@mona
 000000a0: 6c61 6273 2e69 6f3e 0a50 726f 6a65 6374  labs.io>.Project
@@ -69,707 +69,715 @@
 00000440: 7574 746f 6e3d 3126 616d 703b 696d 6167  utton=1&amp;imag
 00000450: 655f 706c 6179 5f62 7574 746f 6e5f 636f  e_play_button_co
 00000460: 6c6f 723d 3636 6337 6431 6530 2220 7769  lor=66c7d1e0" wi
 00000470: 6474 683d 2234 3030 2220 6865 6967 6874  dth="400" height
 00000480: 3d22 3232 3522 2073 7479 6c65 3d22 7769  ="225" style="wi
 00000490: 6474 683a 2034 3030 7078 3b20 6865 6967  dth: 400px; heig
 000004a0: 6874 3a20 3232 3570 783b 223e 3c2f 613e  ht: 225px;"></a>
-000004b0: 3c2f 703e 3c70 2061 6c69 676e 3d22 6365  </p><p align="ce
-000004c0: 6e74 6572 223e 3c61 2068 7265 663d 2268  nter"><a href="h
-000004d0: 7474 7073 3a2f 2f6d 6f6e 616c 6162 732e  ttps://monalabs.
-000004e0: 7769 7374 6961 2e63 6f6d 2f6d 6564 6961  wistia.com/media
-000004f0: 732f 6c36 786d 646a 3363 6436 3f77 7669  s/l6xmdj3cd6?wvi
-00000500: 6465 6f3d 6c36 786d 646a 3363 6436 223e  deo=l6xmdj3cd6">
-00000510: 4f70 656e 4149 2047 5054 2049 6e74 6567  OpenAI GPT Integ
-00000520: 7261 7469 6f6e 2054 7574 6f72 6961 6c3c  ration Tutorial<
-00000530: 2f61 3e3c 2f70 3e0a 0a0a 5573 6520 6f6e  /a></p>...Use on
-00000540: 6520 6c69 6e65 206f 6620 636f 6465 2074  e line of code t
-00000550: 6f20 6765 7420 696e 7374 616e 7420 6c69  o get instant li
-00000560: 7665 206d 6f6e 6974 6f72 696e 6720 666f  ve monitoring fo
-00000570: 7220 796f 7572 204f 7065 6e41 4920 7573  r your OpenAI us
-00000580: 6167 6520 696e 636c 7564 696e 673a 0a2a  age including:.*
-00000590: 2054 6f6b 656e 7320 7573 6167 650a 2a20   Tokens usage.* 
-000005a0: 4861 6c6c 7563 696e 6174 696f 6e20 616c  Hallucination al
-000005b0: 6572 7473 0a2a 2050 726f 6661 6e69 7479  erts.* Profanity
-000005c0: 2061 6e64 2070 7269 7661 6379 2061 6e61   and privacy ana
-000005d0: 6c79 7365 730a 2a20 4265 6861 7669 6f72  lyses.* Behavior
-000005e0: 616c 2064 7269 6674 7320 616e 6420 616e  al drifts and an
-000005f0: 6f6d 616c 6965 730a 2a20 4c61 6e67 4368  omalies.* LangCh
-00000600: 6169 6e20 7375 7070 6f72 740a 2a20 4d75  ain support.* Mu
-00000610: 6368 206d 7563 6820 6d6f 7265 0a0a 2323  ch much more..##
-00000620: 2053 6574 7469 6e67 2055 700a 0a60 6060   Setting Up..```
-00000630: 636f 6e73 6f6c 650a 2420 7069 7020 696e  console.$ pip in
-00000640: 7374 616c 6c20 6d6f 6e61 5f6f 7065 6e61  stall mona_opena
-00000650: 690a 6060 600a 0a49 6620 796f 7520 706c  i.```..If you pl
-00000660: 616e 206f 6e20 7573 696e 6720 4d6f 6e61  an on using Mona
-00000670: 2061 7320 796f 7572 206d 6f6e 6974 6f72   as your monitor
-00000680: 696e 6720 7365 7276 6963 652c 205b 7369  ing service, [si
-00000690: 676e 2075 7020 666f 7220 6120 6672 6565  gn up for a free
-000006a0: 2061 6363 6f75 6e74 2068 6572 655d 2868   account here](h
-000006b0: 7474 7073 3a2f 2f77 7777 2e6d 6f6e 616c  ttps://www.monal
-000006c0: 6162 732e 696f 2f6f 7065 6e61 692d 6770  abs.io/openai-gp
-000006d0: 742d 6d6f 6e69 746f 7269 6e67 292e 0a0a  t-monitoring)...
-000006e0: 2323 2051 7569 636b 2053 7461 7274 0a0a  ## Quick Start..
-000006f0: 596f 7520 6361 6e20 6669 6e64 2062 6f69  You can find boi
-00000700: 6c65 7270 6c61 7465 2063 6f64 6520 666f  lerplate code fo
-00000710: 7220 6d61 6e79 2075 7365 2d63 6173 6573  r many use-cases
-00000720: 2075 6e64 6572 205b 7468 6520 2265 7861   under [the "exa
-00000730: 6d70 6c65 7322 2066 6f6c 6465 725d 2868  mples" folder](h
-00000740: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000750: 6d2f 6d6f 6e61 6c61 6273 2f6d 6f6e 612d  m/monalabs/mona-
-00000760: 6f70 656e 6169 2f74 7265 652f 6d61 696e  openai/tree/main
-00000770: 2f65 7861 6d70 6c65 7329 2e0a 0a60 6060  /examples)...```
-00000780: 7079 0a66 726f 6d20 6f73 2069 6d70 6f72  py.from os impor
-00000790: 7420 656e 7669 726f 6e0a 696d 706f 7274  t environ.import
-000007a0: 2061 7379 6e63 696f 0a69 6d70 6f72 7420   asyncio.import 
-000007b0: 6f70 656e 6169 0a66 726f 6d20 6d6f 6e61  openai.from mona
-000007c0: 5f6f 7065 6e61 692e 6c6f 6767 6572 7320  _openai.loggers 
-000007d0: 696d 706f 7274 2053 7461 6e64 6172 644c  import StandardL
-000007e0: 6f67 6765 720a 6672 6f6d 206c 6f67 6769  ogger.from loggi
-000007f0: 6e67 2069 6d70 6f72 7420 5741 524e 494e  ng import WARNIN
-00000800: 470a 0a66 726f 6d20 6d6f 6e61 5f6f 7065  G..from mona_ope
-00000810: 6e61 6920 696d 706f 7274 206d 6f6e 6974  nai import monit
-00000820: 6f72 2c20 6d6f 6e69 746f 725f 7769 7468  or, monitor_with
-00000830: 5f6c 6f67 6765 720a 0a6f 7065 6e61 692e  _logger..openai.
-00000840: 6170 695f 6b65 7920 3d20 656e 7669 726f  api_key = enviro
-00000850: 6e2e 6765 7428 224f 5045 4e5f 4149 5f4b  n.get("OPEN_AI_K
-00000860: 4559 2229 0a0a 2320 5768 656e 2075 7369  EY")..# When usi
-00000870: 6e67 2061 2073 7461 6e64 6172 6420 6c6f  ng a standard lo
-00000880: 6767 6572 2e0a 0a6d 6f6e 6974 6f72 6564  gger...monitored
-00000890: 5f63 6f6d 706c 6574 696f 6e20 3d20 6d6f  _completion = mo
-000008a0: 6e69 746f 725f 7769 7468 5f6c 6f67 6765  nitor_with_logge
-000008b0: 7228 0a20 2020 206f 7065 6e61 692e 436f  r(.    openai.Co
-000008c0: 6d70 6c65 7469 6f6e 2c0a 2020 2020 5374  mpletion,.    St
-000008d0: 616e 6461 7264 4c6f 6767 6572 2857 4152  andardLogger(WAR
-000008e0: 4e49 4e47 292c 0a29 0a0a 7265 7370 6f6e  NING),.)..respon
-000008f0: 7365 203d 206d 6f6e 6974 6f72 6564 5f63  se = monitored_c
-00000900: 6f6d 706c 6574 696f 6e2e 6372 6561 7465  ompletion.create
-00000910: 280a 2020 2020 6d6f 6465 6c3d 2274 6578  (.    model="tex
-00000920: 742d 6164 612d 3030 3122 2c0a 2020 2020  t-ada-001",.    
-00000930: 7072 6f6d 7074 3d22 4920 7761 6e74 2074  prompt="I want t
-00000940: 6f20 6765 6e65 7261 7465 2073 6f6d 6520  o generate some 
-00000950: 7465 7874 2061 626f 7574 2022 2c0a 2020  text about ",.  
-00000960: 2020 6d61 785f 746f 6b65 6e73 3d32 302c    max_tokens=20,
-00000970: 0a20 2020 206e 3d31 2c0a 2020 2020 7465  .    n=1,.    te
-00000980: 6d70 6572 6174 7572 653d 302e 322c 0a20  mperature=0.2,. 
-00000990: 2020 2023 2041 6464 696e 6720 6164 6469     # Adding addi
-000009a0: 7469 6f6e 616c 2069 6e66 6f72 6d61 7469  tional informati
-000009b0: 6f6e 2066 6f72 206d 6f6e 6974 6f72 696e  on for monitorin
-000009c0: 6720 7075 7270 6f73 6573 2c20 756e 7265  g purposes, unre
-000009d0: 6c61 7465 6420 746f 0a20 2020 2023 2069  lated to.    # i
-000009e0: 6e74 6572 6e61 6c20 4f70 656e 4149 2063  nternal OpenAI c
-000009f0: 616c 6c2e 0a20 2020 204d 4f4e 415f 6164  all..    MONA_ad
-00000a00: 6469 7469 6f6e 616c 5f64 6174 613d 7b22  ditional_data={"
-00000a10: 6375 7374 6f6d 6572 5f69 6422 3a20 2241  customer_id": "A
-00000a20: 3533 3132 3531 227d 2c0a 290a 7072 696e  531251"},.).prin
-00000a30: 7428 7265 7370 6f6e 7365 2e63 686f 6963  t(response.choic
-00000a40: 6573 5b30 5d2e 7465 7874 290a 0a0a 2320  es[0].text)...# 
-00000a50: 5768 656e 206d 6f6e 6974 6f72 696e 6720  When monitoring 
-00000a60: 7769 7468 204d 6f6e 612e 0a0a 4d4f 4e41  with Mona...MONA
-00000a70: 5f41 5049 5f4b 4559 203d 2065 6e76 6972  _API_KEY = envir
-00000a80: 6f6e 2e67 6574 2822 4d4f 4e41 5f41 5049  on.get("MONA_API
-00000a90: 5f4b 4559 2229 0a4d 4f4e 415f 5345 4352  _KEY").MONA_SECR
-00000aa0: 4554 203d 2065 6e76 6972 6f6e 2e67 6574  ET = environ.get
-00000ab0: 2822 4d4f 4e41 5f53 4543 5245 5422 290a  ("MONA_SECRET").
-00000ac0: 4d4f 4e41 5f43 5245 4453 203d 207b 0a20  MONA_CREDS = {. 
-00000ad0: 2020 2022 6b65 7922 3a20 4d4f 4e41 5f41     "key": MONA_A
-00000ae0: 5049 5f4b 4559 2c0a 2020 2020 2273 6563  PI_KEY,.    "sec
-00000af0: 7265 7422 3a20 4d4f 4e41 5f53 4543 5245  ret": MONA_SECRE
-00000b00: 542c 0a7d 0a43 4f4e 5445 5854 5f43 4c41  T,.}.CONTEXT_CLA
-00000b10: 5353 5f4e 414d 4520 3d20 2253 4f4d 455f  SS_NAME = "SOME_
-00000b20: 4d4f 4e49 544f 5249 4e47 5f43 4f4e 5445  MONITORING_CONTE
-00000b30: 5854 5f4e 414d 4522 0a0a 0a6d 6f6e 6974  XT_NAME"...monit
-00000b40: 6f72 6564 5f63 6f6d 706c 6574 696f 6e20  ored_completion 
-00000b50: 3d20 6d6f 6e69 746f 7228 0a20 2020 206f  = monitor(.    o
-00000b60: 7065 6e61 692e 436f 6d70 6c65 7469 6f6e  penai.Completion
-00000b70: 2c0a 2020 2020 4d4f 4e41 5f43 5245 4453  ,.    MONA_CREDS
-00000b80: 2c0a 2020 2020 434f 4e54 4558 545f 434c  ,.    CONTEXT_CL
-00000b90: 4153 535f 4e41 4d45 2c0a 290a 0a72 6573  ASS_NAME,.)..res
-00000ba0: 706f 6e73 6520 3d20 6d6f 6e69 746f 7265  ponse = monitore
-00000bb0: 645f 636f 6d70 6c65 7469 6f6e 2e63 7265  d_completion.cre
-00000bc0: 6174 6528 0a20 2020 206d 6f64 656c 3d22  ate(.    model="
-00000bd0: 7465 7874 2d61 6461 2d30 3031 222c 0a20  text-ada-001",. 
-00000be0: 2020 2070 726f 6d70 743d 2249 2077 616e     prompt="I wan
-00000bf0: 7420 746f 2067 656e 6572 6174 6520 736f  t to generate so
-00000c00: 6d65 2074 6578 7420 6162 6f75 7420 222c  me text about ",
-00000c10: 0a20 2020 206d 6178 5f74 6f6b 656e 733d  .    max_tokens=
-00000c20: 3230 2c0a 2020 2020 6e3d 312c 0a20 2020  20,.    n=1,.   
-00000c30: 2074 656d 7065 7261 7475 7265 3d30 2e32   temperature=0.2
-00000c40: 2c0a 2020 2020 2320 4164 6469 6e67 2061  ,.    # Adding a
-00000c50: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
-00000c60: 6174 696f 6e20 666f 7220 6d6f 6e69 746f  ation for monito
-00000c70: 7269 6e67 2070 7572 706f 7365 732c 2075  ring purposes, u
-00000c80: 6e72 656c 6174 6564 2074 6f0a 2020 2020  nrelated to.    
-00000c90: 2320 696e 7465 726e 616c 204f 7065 6e41  # internal OpenA
-00000ca0: 4920 6361 6c6c 2e0a 2020 2020 4d4f 4e41  I call..    MONA
-00000cb0: 5f61 6464 6974 696f 6e61 6c5f 6461 7461  _additional_data
-00000cc0: 3d7b 2263 7573 746f 6d65 725f 6964 223a  ={"customer_id":
-00000cd0: 2022 4135 3331 3235 3122 7d2c 0a29 0a70   "A531251"},.).p
-00000ce0: 7269 6e74 2872 6573 706f 6e73 652e 6368  rint(response.ch
-00000cf0: 6f69 6365 735b 305d 2e74 6578 7429 0a60  oices[0].text).`
-00000d00: 6060 0a23 2320 5375 7070 6f72 7465 6420  ``.## Supported 
-00000d10: 4f70 656e 4149 2041 5049 730a 4375 7272  OpenAI APIs.Curr
-00000d20: 656e 746c 7920 7468 6973 2063 6c69 656e  ently this clien
-00000d30: 7420 7375 7070 6f72 7473 2060 6f70 656e  t supports `open
-00000d40: 6169 2e43 6f6d 706c 6574 696f 6e60 2061  ai.Completion` a
-00000d50: 6e64 2060 6f70 656e 6169 2e43 6861 7443  nd `openai.ChatC
-00000d60: 6f6d 706c 6574 696f 6e60 2e20 4d6f 6e61  ompletion`. Mona
-00000d70: 2063 616e 2073 7570 706f 7274 2070 726f   can support pro
-00000d80: 6365 7373 6573 2062 6173 6564 206f 6e20  cesses based on 
-00000d90: 6f74 6865 7220 4150 4973 2061 6e64 2061  other APIs and a
-00000da0: 6c73 6f20 6e6f 6e2d 4f70 656e 4149 2d62  lso non-OpenAI-b
-00000db0: 6173 6564 2061 7070 732e 0a49 6620 796f  ased apps..If yo
-00000dc0: 7520 6861 7665 2061 2064 6966 6665 7272  u have a differr
-00000dd0: 656e 7420 7573 652d 6361 7365 2c20 7765  ent use-case, we
-00000de0: 2764 206c 6f76 6520 746f 2068 6561 7220  'd love to hear 
-00000df0: 6162 6f75 7420 6974 2120 506c 6561 7365  about it! Please
-00000e00: 2065 6d61 696c 2075 7320 6174 2073 7570   email us at sup
-00000e10: 706f 7274 406d 6f6e 616c 6162 732e 696f  port@monalabs.io
-00000e20: 2e0a 0a23 2320 5573 6167 650a 2323 2320  ...## Usage.### 
-00000e30: 496e 6974 6961 6c69 7a61 7469 6f6e 0a0a  Initialization..
-00000e40: 5468 6520 6d61 696e 2061 6e64 206f 6e6c  The main and onl
-00000e50: 7920 6675 6e63 7469 6f6e 2065 7870 6f73  y function expos
-00000e60: 6564 2069 6e20 7468 6973 2070 6163 6b61  ed in this packa
-00000e70: 6765 2069 7320 606d 6f6e 6974 6f72 602e  ge is `monitor`.
-00000e80: 0a60 6060 7079 0a69 6d70 6f72 7420 6f70  .```py.import op
-00000e90: 656e 6169 0a0a 6672 6f6d 206d 6f6e 615f  enai..from mona_
-00000ea0: 6f70 656e 6169 2069 6d70 6f72 7420 6d6f  openai import mo
-00000eb0: 6e69 746f 720a 0a6f 7065 6e61 692e 6170  nitor..openai.ap
-00000ec0: 695f 6b65 7920 3d20 656e 7669 726f 6e2e  i_key = environ.
-00000ed0: 6765 7428 224f 5045 4e5f 4149 5f4b 4559  get("OPEN_AI_KEY
-00000ee0: 2229 0a0a 6d6f 6e69 746f 7265 645f 636f  ")..monitored_co
-00000ef0: 6d70 6c65 7469 6f6e 203d 206d 6f6e 6974  mpletion = monit
-00000f00: 6f72 280a 2020 2020 6f70 656e 6169 2e43  or(.    openai.C
-00000f10: 6f6d 706c 6574 696f 6e2c 0a20 2020 2028  ompletion,.    (
-00000f20: 0a20 2020 2020 2020 2065 6e76 6972 6f6e  .        environ
-00000f30: 2e67 6574 2822 4d4f 4e41 5f41 5049 5f4b  .get("MONA_API_K
-00000f40: 4559 2229 2c0a 2020 2020 2020 2020 656e  EY"),.        en
-00000f50: 7669 726f 6e2e 6765 7428 224d 4f4e 415f  viron.get("MONA_
-00000f60: 5345 4352 4554 2229 2c0a 2020 2020 292c  SECRET"),.    ),
-00000f70: 0a20 2020 2022 534f 4d45 5f4d 4f4e 4954  .    "SOME_MONIT
-00000f80: 4f52 494e 475f 434f 4e54 4558 545f 4e41  ORING_CONTEXT_NA
-00000f90: 4d45 222c 0a20 2020 207b 2261 6e61 6c79  ME",.    {"analy
-00000fa0: 7369 7322 3a20 7b22 7072 6f66 616e 6974  sis": {"profanit
-00000fb0: 7922 3a20 4661 6c73 657d 7d0a 290a 0a2e  y": False}}.)...
-00000fc0: 2e2e 0a0a 6d6f 6e69 746f 7265 645f 636f  ....monitored_co
-00000fd0: 6d70 6c65 7469 6f6e 2e63 7265 6174 6528  mpletion.create(
-00000fe0: 2e2e 2e29 0a60 6060 0a0a 5468 6520 606d  ...).```..The `m
-00000ff0: 6f6e 6974 6f72 6020 6675 6e63 7469 6f6e  onitor` function
-00001000: 2072 6574 7572 6e73 2074 6f20 796f 7520   returns to you 
-00001010: 6120 636c 6173 7320 7468 6174 2077 7261  a class that wra
-00001020: 7073 2074 6865 206f 7269 6769 6e61 6c20  ps the original 
-00001030: 6f70 656e 6169 2065 6e64 706f 696e 7420  openai endpoint 
-00001040: 636c 6173 7320 796f 7520 7072 6f76 6964  class you provid
-00001050: 652c 2077 6974 6820 616e 2065 7175 6976  e, with an equiv
-00001060: 616c 656e 7420 4150 4920 2862 6573 6964  alent API (besid
-00001070: 6573 2073 6f6d 6520 6164 6469 7469 6f6e  es some addition
-00001080: 7320 6c69 7374 6564 2062 656c 6f77 292e  s listed below).
-00001090: 0a59 6f75 2063 616e 2074 6865 6e20 7573  .You can then us
-000010a0: 6520 7468 6520 7265 7475 726e 6564 2063  e the returned c
-000010b0: 6c61 7373 2720 2263 7265 6174 6522 2061  lass' "create" a
-000010c0: 6e64 2022 6163 7265 6174 6522 2066 756e  nd "acreate" fun
-000010d0: 6374 696f 6e73 206a 7573 7420 6173 2079  ctions just as y
-000010e0: 6f75 2077 6f75 6c64 2062 6566 6f72 652c  ou would before,
-000010f0: 206f 6e6c 7920 6e6f 772c 2062 6573 6964   only now, besid
-00001100: 6573 2067 6574 7469 6e67 2074 6865 2072  es getting the r
-00001110: 6571 7565 7374 6564 206f 7065 6e41 4920  equested openAI 
-00001120: 6675 6e63 7469 6f6e 616c 6974 792c 2074  functionality, t
-00001130: 6869 7320 636c 6965 6e74 2077 696c 6c20  his client will 
-00001140: 6c6f 6720 6f75 7420 746f 204d 6f6e 6127  log out to Mona'
-00001150: 7320 7365 7276 6572 2074 6865 2070 6172  s server the par
-00001160: 616d 6574 6572 7320 796f 7520 7573 6564  ameters you used
-00001170: 2028 652e 672e 2c20 7465 6d70 6572 6174   (e.g., temperat
-00001180: 7572 6529 2c20 6461 7461 2061 626f 7574  ure), data about
-00001190: 2074 6865 2072 6573 706f 6e73 6520 6672   the response fr
-000011a0: 6f6d 204f 7065 6e41 4927 7320 7365 7276  om OpenAI's serv
-000011b0: 6572 2c20 616e 6420 6375 7374 6f6d 2061  er, and custom a
-000011c0: 6e61 6c79 7365 7320 6162 6f75 7420 7468  nalyses about th
-000011d0: 6520 6361 6c6c 2028 652e 672e 2c20 7072  e call (e.g., pr
-000011e0: 6f66 616e 6974 7920 7363 6f72 6573 2c20  ofanity scores, 
-000011f0: 7072 6976 6163 7920 6368 6563 6b73 2066  privacy checks f
-00001200: 6f72 2065 6d61 696c 732f 7068 6f6e 6520  or emails/phone 
-00001210: 6e75 6d62 6572 7320 666f 756e 6420 696e  numbers found in
-00001220: 2074 6865 2074 6578 7473 2c20 7465 7874   the texts, text
-00001230: 7561 6c20 616e 616c 7973 6573 2c20 6574  ual analyses, et
-00001240: 632e 2e2e 290a 0a54 6865 2060 6d6f 6e69  c...)..The `moni
-00001250: 746f 7260 2066 756e 6374 696f 6e20 7265  tor` function re
-00001260: 6365 6976 6573 2074 6865 2066 6f6c 6c6f  ceives the follo
-00001270: 7769 6e67 2061 7267 756d 656e 7473 3a0a  wing arguments:.
-00001280: 6f70 656e 6169 5f63 6c61 7373 3a20 416e  openai_class: An
-00001290: 204f 7065 6e41 4920 4150 4920 636c 6173   OpenAI API clas
-000012a0: 7320 746f 2077 7261 7020 7769 7468 206d  s to wrap with m
-000012b0: 6f6e 6974 6f72 696e 6720 6361 7061 6269  onitoring capabi
-000012c0: 6c74 6965 732e 0a6d 6f6e 615f 6372 6564  lties..mona_cred
-000012d0: 733a 2041 2064 6963 7420 2863 6f6e 7461  s: A dict (conta
-000012e0: 696e 696e 6720 226b 6579 2220 616e 6420  ining "key" and 
-000012f0: 2273 6563 7265 7422 2920 6f72 2070 6169  "secret") or pai
-00001300: 7220 2874 7570 6c65 2920 6f66 204d 6f6e  r (tuple) of Mon
-00001310: 6120 4150 4920 6b65 7920 616e 6420 7365  a API key and se
-00001320: 6372 6574 2074 6f20 7365 7420 7570 204d  cret to set up M
-00001330: 6f6e 6127 7320 636c 6965 6e74 7320 6672  ona's clients fr
-00001340: 6f6d 2069 7473 2053 444b 2e0a 636f 6e74  om its SDK..cont
-00001350: 6578 745f 636c 6173 733a 2054 6865 204d  ext_class: The M
-00001360: 6f6e 6120 636f 6e74 6578 7420 636c 6173  ona context clas
-00001370: 7320 6e61 6d65 2074 6f20 7573 6520 666f  s name to use fo
-00001380: 7220 6d6f 6e69 746f 7269 6e67 2e20 5573  r monitoring. Us
-00001390: 6520 6120 636f 6e73 7461 6e74 206e 616d  e a constant nam
-000013a0: 6520 6f66 2079 6f75 7220 6368 6f69 6365  e of your choice
-000013b0: 2e0a 7370 6563 733a 2041 2064 6963 7469  ..specs: A dicti
-000013c0: 6f6e 6172 7920 6f66 2073 7065 6369 6669  onary of specifi
-000013d0: 6361 7469 6f6e 7320 7375 6368 2061 7320  cations such as 
-000013e0: 6d6f 6e69 746f 7269 6e67 2073 616d 706c  monitoring sampl
-000013f0: 696e 6720 7261 7469 6f2e 0a0a 2323 2323  ing ratio...####
-00001400: 2053 7065 6373 0a54 6865 2073 7065 6373   Specs.The specs
-00001410: 2061 7267 2061 6c6c 6f77 7320 796f 7520   arg allows you 
-00001420: 746f 2063 6f6e 6669 6775 7265 2077 6861  to configure wha
-00001430: 7420 7368 6f75 6c64 2062 6520 6d6f 6e69  t should be moni
-00001440: 746f 7265 642e 2049 7420 6578 7065 6374  tored. It expect
-00001450: 7320 6120 7079 7468 6f6e 2064 6963 7420  s a python dict 
-00001460: 7769 7468 2074 6865 2066 6f6c 6c77 6f69  with the follwoi
-00001470: 6e67 2070 6f73 7369 626c 6520 6b65 7973  ng possible keys
-00001480: 3a0a 2a20 7361 6d70 6c69 6e67 5f72 6174  :.* sampling_rat
-00001490: 696f 2028 3129 3a20 4120 6e75 6d62 6572  io (1): A number
-000014a0: 2062 6574 7765 656e 2030 2061 6e64 2031   between 0 and 1
-000014b0: 2066 6f72 2068 6f77 206f 6674 656e 2073   for how often s
-000014c0: 686f 756c 6420 7468 6520 6361 6c6c 2062  hould the call b
-000014d0: 6520 6c6f 6767 6564 2e0a 2a20 6176 6f69  e logged..* avoi
-000014e0: 645f 6d6f 6e69 746f 7269 6e67 5f65 7863  d_monitoring_exc
-000014f0: 6570 7469 6f6e 7320 2846 616c 7365 293a  eptions (False):
-00001500: 2057 6865 7468 6572 206f 7220 6e6f 7420   Whether or not 
-00001510: 746f 206c 6f67 206f 7574 2074 6f20 4d6f  to log out to Mo
-00001520: 6e61 2077 6865 6e20 7468 6572 6520 6973  na when there is
-00001530: 2061 6e20 4f70 656e 4149 2065 7863 6570   an OpenAI excep
-00001540: 7469 6f6e 2e20 4465 6661 756c 7420 6973  tion. Default is
-00001550: 2074 6f20 7472 6163 6b20 6578 6365 7074   to track except
-00001560: 696f 6e73 202d 2061 6e64 204d 6f6e 6120  ions - and Mona 
-00001570: 7769 6c6c 2061 6c65 7274 2079 6f75 206f  will alert you o
-00001580: 6e20 7468 696e 6773 206c 696b 6520 6120  n things like a 
-00001590: 6a75 6d70 2069 6e20 6e75 6d62 6572 206f  jump in number o
-000015a0: 6620 6578 6365 7074 696f 6e73 0a2a 2065  f exceptions.* e
-000015b0: 7870 6f72 745f 7072 6f6d 7074 2028 4661  xport_prompt (Fa
-000015c0: 6c73 6529 3a20 5768 6574 6865 7220 4d6f  lse): Whether Mo
-000015d0: 6e61 2073 686f 756c 6420 6578 706f 7274  na should export
-000015e0: 2074 6865 2061 6374 7561 6c20 7072 6f6d   the actual prom
-000015f0: 7074 2074 6578 742e 2042 6520 6465 6661  pt text. Be defa
-00001600: 756c 7420 7365 7420 746f 2046 616c 7365  ult set to False
-00001610: 2074 6f20 6176 6f69 6420 7072 6976 6163   to avoid privac
-00001620: 7920 636f 6e63 6572 6e73 2e0a 2a20 6578  y concerns..* ex
-00001630: 706f 7274 5f72 6573 706f 6e73 655f 7465  port_response_te
-00001640: 7874 7320 2846 616c 7365 293a 2057 6865  xts (False): Whe
-00001650: 7468 6572 204d 6f6e 6120 7368 6f75 6c64  ther Mona should
-00001660: 2065 7870 6f72 7420 7468 6520 6163 7475   export the actu
-00001670: 616c 2072 6573 706f 6e73 6520 7465 7874  al response text
-00001680: 732e 2042 6520 6465 6661 756c 7420 7365  s. Be default se
-00001690: 7420 746f 2046 616c 7365 2074 6f20 6176  t to False to av
-000016a0: 6f69 6420 7072 6976 6163 7920 636f 6e63  oid privacy conc
-000016b0: 6572 6e73 2e0a 2a20 616e 616c 7973 6973  erns..* analysis
-000016c0: 3a20 4120 6469 6374 696f 6e61 7279 206d  : A dictionary m
-000016d0: 6170 7069 6e67 2065 6163 6820 616e 616c  apping each anal
-000016e0: 7973 6973 2074 7970 6520 746f 2061 2062  ysis type to a b
-000016f0: 6f6f 6c65 616e 2076 616c 7565 2074 656c  oolean value tel
-00001700: 6c69 6e67 2074 6865 2063 6c69 656e 7420  ling the client 
-00001710: 7768 6574 6865 7220 6f72 206e 6f74 2074  whether or not t
-00001720: 6f20 7275 6e20 7361 6964 2061 6e61 6c79  o run said analy
-00001730: 7369 7320 616e 6420 6c6f 6720 6974 2074  sis and log it t
-00001740: 6f20 4d6f 6e61 2e20 506f 7373 6962 6c65  o Mona. Possible
-00001750: 206f 7074 696f 6e73 2063 7572 7265 6e74   options current
-00001760: 6c79 2061 7265 2022 7072 6976 6163 7922  ly are "privacy"
-00001770: 2c20 2270 726f 6661 6e69 7479 222c 2061  , "profanity", a
-00001780: 6e64 2022 7465 7874 7561 6c22 2e20 4279  nd "textual". By
-00001790: 2064 6566 6175 6c74 2c20 616c 6c20 616e   default, all an
-000017a0: 616c 7973 6573 2074 616b 6520 706c 6163  alyses take plac
-000017b0: 6520 616e 6420 6172 6520 6c6f 6767 6564  e and are logged
-000017c0: 206f 7574 2074 6f20 4d6f 6e61 2e0a 0a23   out to Mona...#
-000017d0: 2323 2055 7369 6e67 2063 7573 746f 6d20  ## Using custom 
-000017e0: 6c6f 6767 6572 730a 596f 7520 646f 6e27  loggers.You don'
-000017f0: 7420 6861 7665 2074 6f20 6861 7665 2061  t have to have a
-00001800: 204d 6f6e 6120 6163 636f 756e 7420 746f   Mona account to
-00001810: 2075 7365 2074 6869 7320 7061 636b 6167   use this packag
-00001820: 652e 2059 6f75 2063 616e 2064 6566 696e  e. You can defin
-00001830: 6520 7370 6563 6966 6963 206c 6f67 6765  e specific logge
-00001840: 7273 2074 6f20 6c6f 6720 6f75 7420 7468  rs to log out th
-00001850: 6520 6461 7461 2074 6f20 6120 6669 6c65  e data to a file
-00001860: 2c20 6d65 6d6f 7279 2c20 6f72 206a 7573  , memory, or jus
-00001870: 7420 6120 6769 7665 6e20 7079 7468 6f6e  t a given python
-00001880: 206c 6f67 6765 722e 2046 6f72 2065 7861   logger. For exa
-00001890: 6d70 6c65 2c20 746f 206c 6f67 206f 7574  mple, to log out
-000018a0: 2074 6865 2072 656c 6576 616e 7420 6d65   the relevant me
-000018b0: 7472 6963 7320 6173 2057 4152 4e49 4e47  trics as WARNING
-000018c0: 3a0a 0a60 6060 7079 0a66 726f 6d20 6f73  :..```py.from os
-000018d0: 2069 6d70 6f72 7420 656e 7669 726f 6e0a   import environ.
-000018e0: 696d 706f 7274 206f 7065 6e61 690a 6672  import openai.fr
-000018f0: 6f6d 206d 6f6e 615f 6f70 656e 6169 2e6c  om mona_openai.l
-00001900: 6f67 6765 7273 2069 6d70 6f72 7420 5374  oggers import St
-00001910: 616e 6461 7264 4c6f 6767 6572 0a66 726f  andardLogger.fro
-00001920: 6d20 6c6f 6767 696e 6720 696d 706f 7274  m logging import
-00001930: 2057 4152 4e49 4e47 0a0a 6672 6f6d 206d   WARNING..from m
-00001940: 6f6e 615f 6f70 656e 6169 2069 6d70 6f72  ona_openai impor
-00001950: 7420 6d6f 6e69 746f 725f 7769 7468 5f6c  t monitor_with_l
-00001960: 6f67 6765 720a 0a6f 7065 6e61 692e 6170  ogger..openai.ap
-00001970: 695f 6b65 7920 3d20 656e 7669 726f 6e2e  i_key = environ.
-00001980: 6765 7428 224f 5045 4e5f 4149 5f4b 4559  get("OPEN_AI_KEY
-00001990: 2229 0a0a 6d6f 6e69 746f 7265 645f 636f  ")..monitored_co
-000019a0: 6d70 6c65 7469 6f6e 203d 206d 6f6e 6974  mpletion = monit
-000019b0: 6f72 5f77 6974 685f 6c6f 6767 6572 280a  or_with_logger(.
-000019c0: 2020 2020 6f70 656e 6169 2e43 6f6d 706c      openai.Compl
-000019d0: 6574 696f 6e2c 0a20 2020 2053 7461 6e64  etion,.    Stand
-000019e0: 6172 644c 6f67 6765 7228 5741 524e 494e  ardLogger(WARNIN
-000019f0: 4729 2c0a 290a 0a72 6573 706f 6e73 6520  G),.)..response 
-00001a00: 3d20 6d6f 6e69 746f 7265 645f 636f 6d70  = monitored_comp
-00001a10: 6c65 7469 6f6e 2e63 7265 6174 6528 0a20  letion.create(. 
-00001a20: 2020 206d 6f64 656c 3d22 7465 7874 2d61     model="text-a
-00001a30: 6461 2d30 3031 222c 0a20 2020 2070 726f  da-001",.    pro
-00001a40: 6d70 743d 2249 2077 616e 7420 746f 2067  mpt="I want to g
-00001a50: 656e 6572 6174 6520 736f 6d65 2074 6578  enerate some tex
-00001a60: 7420 6162 6f75 7420 222c 0a20 2020 206d  t about ",.    m
-00001a70: 6178 5f74 6f6b 656e 733d 3230 2c0a 2020  ax_tokens=20,.  
-00001a80: 2020 6e3d 312c 0a20 2020 2074 656d 7065    n=1,.    tempe
-00001a90: 7261 7475 7265 3d30 2e32 2c0a 2020 2020  rature=0.2,.    
-00001aa0: 2320 4164 6469 6e67 2061 6464 6974 696f  # Adding additio
-00001ab0: 6e61 6c20 696e 666f 726d 6174 696f 6e20  nal information 
-00001ac0: 666f 7220 6d6f 6e69 746f 7269 6e67 2070  for monitoring p
-00001ad0: 7572 706f 7365 732c 2075 6e72 656c 6174  urposes, unrelat
-00001ae0: 6564 2074 6f0a 2020 2020 2320 696e 7465  ed to.    # inte
-00001af0: 726e 616c 204f 7065 6e41 4920 6361 6c6c  rnal OpenAI call
-00001b00: 2e0a 2020 2020 4d4f 4e41 5f61 6464 6974  ..    MONA_addit
-00001b10: 696f 6e61 6c5f 6461 7461 3d7b 2263 7573  ional_data={"cus
-00001b20: 746f 6d65 725f 6964 223a 2022 4135 3331  tomer_id": "A531
-00001b30: 3235 3122 7d2c 0a29 0a60 6060 0a0a 5468  251"},.).```..Th
-00001b40: 6973 2053 444b 2070 726f 7669 6465 7320  is SDK provides 
-00001b50: 6120 7369 6d70 6c65 2069 6e74 6572 6661  a simple interfa
-00001b60: 6365 2074 6f20 696d 706c 656d 656e 7420  ce to implement 
-00001b70: 796f 7572 206f 776e 206c 6f67 6765 7273  your own loggers
-00001b80: 2062 7920 696e 6865 7269 7469 6e67 2066   by inheriting f
-00001b90: 726f 6d20 4c6f 6767 6572 2075 6e64 6572  rom Logger under
-00001ba0: 206c 6f67 6765 7273 2f6c 6f67 6765 722e   loggers/logger.
-00001bb0: 7079 2e0a 416c 7465 726e 6174 6976 656c  py..Alternativel
-00001bc0: 792c 2062 7920 7573 696e 6720 7468 6520  y, by using the 
-00001bd0: 7374 616e 6461 7264 2070 7974 686f 6e20  standard python 
-00001be0: 6c6f 6767 696e 6720 6c69 6272 6172 7920  logging library 
-00001bf0: 6173 2069 6e20 7468 6520 6578 616d 706c  as in the exampl
-00001c00: 652c 2079 6f75 2063 616e 2063 7265 6174  e, you can creat
-00001c10: 6520 6c6f 6767 696e 6720 6861 6e64 6c65  e logging handle
-00001c20: 7273 2074 6f20 6c6f 6720 7468 6520 6461  rs to log the da
-00001c30: 7461 206f 7574 2074 6f20 616e 7920 6d65  ta out to any me
-00001c40: 6368 616e 6973 6d20 796f 7520 6368 6f6f  chanism you choo
-00001c50: 7365 2028 652e 672e 2c20 4b61 666b 612c  se (e.g., Kafka,
-00001c60: 204c 6f67 7374 6173 682c 2065 7463 2e2e   Logstash, etc..
-00001c70: 2e29 0a0a 2323 2320 4361 7061 6269 6c69  .)..### Capabili
-00001c80: 7469 6573 2064 7572 696e 6720 4150 4920  ties during API 
-00001c90: 6361 6c6c 730a 0a41 6674 6572 2077 7261  calls..After wra
-00001ca0: 7070 696e 6720 796f 7572 2065 6e64 706f  pping your endpo
-00001cb0: 696e 7420 7769 7468 2060 6d6f 6e69 746f  int with `monito
-00001cc0: 7260 2c20 796f 7520 7265 616c 6c79 2064  r`, you really d
-00001cd0: 6f6e 2774 206e 6565 6420 746f 2064 6f20  on't need to do 
-00001ce0: 616e 7974 6869 6e67 2065 6c73 652e 2057  anything else. W
-00001cf0: 6865 6e20 7573 696e 6720 6063 7265 6174  hen using `creat
-00001d00: 6560 206f 7220 6061 6372 6561 7465 6020  e` or `acreate` 
-00001d10: 6461 7461 2077 696c 6c20 6265 2074 7261  data will be tra
-00001d20: 636b 6564 2061 6e64 206d 6f6e 6974 6f72  cked and monitor
-00001d30: 696e 6720 7769 6c6c 2074 616b 6520 706c  ing will take pl
-00001d40: 6163 652e 0a0a 5468 6572 6520 6172 652c  ace...There are,
-00001d50: 2068 6f77 6576 6572 2c20 7365 7665 7261   however, severa
-00001d60: 6c20 6361 7061 6269 6c69 7469 6573 2074  l capabilities t
-00001d70: 6861 7420 6172 6520 6164 6465 6420 746f  hat are added to
-00001d80: 2074 6865 7365 2066 756e 6374 696f 6e73   these functions
-00001d90: 2e20 5370 6563 6966 6963 616c 6c79 2c20  . Specifically, 
-00001da0: 796f 7520 6361 6e20 6164 6420 7468 6520  you can add the 
-00001db0: 666f 6c6c 6f77 696e 6720 6172 6775 6d65  following argume
-00001dc0: 6e74 7320 746f 2061 6e79 2063 7265 6174  nts to any creat
-00001dd0: 6520 6361 6c6c 3a0a 2a20 4d4f 4e41 5f63  e call:.* MONA_c
-00001de0: 6f6e 7465 7874 5f69 643a 2054 6865 2075  ontext_id: The u
-00001df0: 6e69 7175 6520 6964 206f 6620 7468 6520  nique id of the 
-00001e00: 636f 6e74 6578 7420 696e 2077 6869 6368  context in which
-00001e10: 2074 6865 2063 616c 6c20 6973 206d 6164   the call is mad
-00001e20: 652e 2042 7920 7573 696e 6720 7468 6973  e. By using this
-00001e30: 2049 4420 796f 7520 6361 6e20 6578 706f   ID you can expo
-00001e40: 7274 206d 6f72 6520 6461 7461 2074 6f20  rt more data to 
-00001e50: 4d6f 6e61 2074 6f20 7468 6520 7361 6d65  Mona to the same
-00001e60: 2063 6f6e 7465 7874 2066 726f 6d20 6f74   context from ot
-00001e70: 6865 7220 706c 6163 6573 2e20 4966 206e  her places. If n
-00001e80: 6f74 2073 7570 706c 6965 642c 2074 6865  ot supplied, the
-00001e90: 2022 6964 2220 6669 656c 6420 6f66 2074   "id" field of t
-00001ea0: 6865 204f 7065 6e41 4920 456e 6470 6f69  he OpenAI Endpoi
-00001eb0: 6e74 2773 2072 6573 706f 6e73 6520 7769  nt's response wi
-00001ec0: 6c6c 2062 6520 7573 6564 2061 7320 7468  ll be used as th
-00001ed0: 6520 4d6f 6e61 2063 6f6e 7465 7874 2049  e Mona context I
-00001ee0: 4420 6175 746f 6d61 7469 6361 6c6c 792e  D automatically.
-00001ef0: 0a2a 204d 4f4e 415f 6578 706f 7274 5f74  .* MONA_export_t
-00001f00: 696d 6573 7461 6d70 3a20 4361 6e20 6265  imestamp: Can be
-00001f10: 2075 7365 6420 746f 2073 696d 756c 6174   used to simulat
-00001f20: 6520 6173 2069 6620 7468 6520 6375 7272  e as if the curr
-00001f30: 656e 7420 6361 6c6c 2077 6173 206d 6164  ent call was mad
-00001f40: 6520 696e 2061 2064 6966 6665 7265 6e74  e in a different
-00001f50: 2074 696d 652c 2061 7320 6661 7220 6173   time, as far as
-00001f60: 204d 6f6e 6120 6973 2063 6f6e 6365 726e   Mona is concern
-00001f70: 6564 2e0a 2a20 4d4f 4e41 5f61 6464 6974  ed..* MONA_addit
-00001f80: 696f 6e61 6c5f 6461 7461 3a20 4120 4a53  ional_data: A JS
-00001f90: 4f4e 2d73 6572 6961 6c69 7a61 626c 6520  ON-serializable 
-00001fa0: 6469 6374 2077 6974 6820 616e 7920 6f74  dict with any ot
-00001fb0: 6865 7220 6461 7461 2079 6f75 2077 616e  her data you wan
-00001fc0: 7420 746f 2061 6464 2074 6f20 7468 6520  t to add to the 
-00001fd0: 6d6f 6e69 746f 7269 6e67 2063 6f6e 7465  monitoring conte
-00001fe0: 7874 2e20 5468 6973 2063 6f6d 6573 2069  xt. This comes i
-00001ff0: 6e20 6861 6e64 7920 6966 2079 6f75 2077  n handy if you w
-00002000: 616e 7420 746f 2061 6464 206d 6f72 6520  ant to add more 
-00002010: 696e 666f 726d 6174 696f 6e20 746f 2074  information to t
-00002020: 6865 206d 6f6e 6974 6f72 696e 6720 636f  he monitoring co
-00002030: 6e74 6578 2074 6861 7420 6973 6e27 7420  ntex that isn't 
-00002040: 7061 7274 206f 6620 7468 6520 6261 7369  part of the basi
-00002050: 6320 4f70 656e 4149 2041 5049 2063 616c  c OpenAI API cal
-00002060: 6c20 696e 666f 726d 6174 696f 6e2e 2046  l information. F
-00002070: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
-00002080: 6f75 2061 7265 2075 7369 6e67 2061 2073  ou are using a s
-00002090: 7065 6369 6669 6320 7465 6d70 6c61 7465  pecific template
-000020a0: 2049 4420 6f72 2069 6620 7468 6973 2063   ID or if this c
-000020b0: 616c 6c20 6973 2062 6569 6e67 206d 6164  all is being mad
-000020c0: 6520 666f 7220 6120 7370 6563 6966 6963  e for a specific
-000020d0: 2063 7573 746f 6d65 7220 4944 2c20 7468   customer ID, th
-000020e0: 6573 6520 6172 6520 6669 656c 6473 2079  ese are fields y
-000020f0: 6f75 2063 616e 2061 6464 2074 6865 7265  ou can add there
-00002100: 2074 6f20 6865 6c70 2067 6574 2066 756c   to help get ful
-00002110: 6c20 636f 6e74 6578 7420 7768 656e 206d  l context when m
-00002120: 6f6e 6974 6f72 696e 6720 7769 7468 204d  onitoring with M
-00002130: 6f6e 612e 0a0a 4578 616d 706c 653a 0a60  ona...Example:.`
-00002140: 6060 7079 0a72 6573 706f 6e73 6520 3d20  ``py.response = 
-00002150: 6173 796e 6369 6f2e 7275 6e28 6d6f 6e69  asyncio.run(moni
-00002160: 746f 7265 645f 636f 6d70 6c65 7469 6f6e  tored_completion
-00002170: 2e61 6372 6561 7465 280a 2020 2020 656e  .acreate(.    en
-00002180: 6769 6e65 3d6d 6f64 656c 2c0a 2020 2020  gine=model,.    
-00002190: 7072 6f6d 7074 3d70 726f 6d70 742c 0a20  prompt=prompt,. 
-000021a0: 2020 206d 6178 5f74 6f6b 656e 733d 6d61     max_tokens=ma
-000021b0: 785f 746f 6b65 6e73 2c0a 2020 2020 6e3d  x_tokens,.    n=
-000021c0: 6e2c 0a20 2020 2074 656d 7065 7261 7475  n,.    temperatu
-000021d0: 7265 3d74 656d 7065 7261 7475 7265 2c0a  re=temperature,.
-000021e0: 2020 2020 4d4f 4e41 5f61 6464 6974 696f      MONA_additio
-000021f0: 6e61 6c5f 6461 7461 3d7b 2263 7573 746f  nal_data={"custo
-00002200: 6d65 725f 6964 223a 2022 4135 3331 3235  mer_id": "A53125
-00002210: 3122 7d2c 0a29 290a 7072 696e 7428 7265  1"},.)).print(re
-00002220: 7370 6f6e 7365 2e63 686f 6963 6573 5b30  sponse.choices[0
-00002230: 5d2e 7465 7874 290a 6060 600a 0a23 2323  ].text).```..###
-00002240: 2055 7369 6e67 204f 7065 6e41 4920 7769   Using OpenAI wi
-00002250: 7468 2052 4553 5420 6361 6c6c 7320 696e  th REST calls in
-00002260: 7374 6561 6420 6f66 204f 7065 6e41 4927  stead of OpenAI'
-00002270: 7320 5079 7468 6f6e 2063 6c69 656e 740a  s Python client.
-00002280: 496e 2073 6f6d 6520 6361 7365 7320 796f  In some cases yo
-00002290: 7520 6d61 7920 6368 6f6f 7365 2074 6f20  u may choose to 
-000022a0: 7573 6520 4f70 656e 4149 2773 2041 5049  use OpenAI's API
-000022b0: 2064 6972 6563 746c 7920 7769 7468 2052   directly with R
-000022c0: 4553 5420 6361 6c6c 7320 616e 6420 6e6f  EST calls and no
-000022d0: 7420 7573 696e 6720 4f70 656e 4149 2773  t using OpenAI's
-000022e0: 2053 444b 2e20 466f 7220 7468 6573 6520   SDK. For these 
-000022f0: 6361 7365 7320 7765 2061 6c6c 6f77 2061  cases we allow a
-00002300: 206d 6f72 6520 6469 7265 6374 2061 7070   more direct app
-00002310: 726f 6163 6820 666f 7220 6c6f 6767 696e  roach for loggin
-00002320: 6720 746f 204d 6f6e 6120 6173 2077 656c  g to Mona as wel
-00002330: 6c2c 2062 7920 7573 696e 6720 7468 6520  l, by using the 
-00002340: 2267 6574 5f72 6573 745f 6d6f 6e69 746f  "get_rest_monito
-00002350: 7222 2066 756e 6374 696f 6e2e 2053 6565  r" function. See
-00002360: 2065 7861 6d70 6c65 2062 656c 6f77 2e0a   example below..
-00002370: 0a60 6060 7079 0a23 2044 6972 6563 7420  .```py.# Direct 
-00002380: 5245 5354 2075 7361 6765 2c20 7769 7468  REST usage, with
-00002390: 6f75 7420 4f70 656e 4149 2063 6c69 656e  out OpenAI clien
-000023a0: 740a 696d 706f 7274 2072 6571 7565 7374  t.import request
-000023b0: 730a 6672 6f6d 206f 7320 696d 706f 7274  s.from os import
-000023c0: 2065 6e76 6972 6f6e 0a66 726f 6d20 6d6f   environ.from mo
-000023d0: 6e61 5f6f 7065 6e61 6920 696d 706f 7274  na_openai import
-000023e0: 2067 6574 5f72 6573 745f 6d6f 6e69 746f   get_rest_monito
-000023f0: 720a 0a0a 4d4f 4e41 5f41 5049 5f4b 4559  r...MONA_API_KEY
-00002400: 203d 2065 6e76 6972 6f6e 2e67 6574 2822   = environ.get("
-00002410: 4d4f 4e41 5f41 5049 5f4b 4559 2229 0a4d  MONA_API_KEY").M
-00002420: 4f4e 415f 5345 4352 4554 203d 2065 6e76  ONA_SECRET = env
-00002430: 6972 6f6e 2e67 6574 2822 4d4f 4e41 5f53  iron.get("MONA_S
-00002440: 4543 5245 5422 290a 4d4f 4e41 5f43 5245  ECRET").MONA_CRE
-00002450: 4453 203d 207b 0a20 2020 2022 6b65 7922  DS = {.    "key"
-00002460: 3a20 4d4f 4e41 5f41 5049 5f4b 4559 2c0a  : MONA_API_KEY,.
-00002470: 2020 2020 2273 6563 7265 7422 3a20 4d4f      "secret": MO
-00002480: 4e41 5f53 4543 5245 542c 0a7d 0a43 4f4e  NA_SECRET,.}.CON
-00002490: 5445 5854 5f43 4c41 5353 5f4e 414d 4520  TEXT_CLASS_NAME 
-000024a0: 3d20 2253 4f4d 455f 4d4f 4e49 544f 5249  = "SOME_MONITORI
-000024b0: 4e47 5f43 4f4e 5445 5854 5f4e 414d 4522  NG_CONTEXT_NAME"
-000024c0: 0a0a 2320 4765 7420 4d6f 6e61 206c 6f67  ..# Get Mona log
-000024d0: 6765 720a 6d6f 6e61 5f6c 6f67 6765 7220  ger.mona_logger 
-000024e0: 3d20 6765 745f 7265 7374 5f6d 6f6e 6974  = get_rest_monit
-000024f0: 6f72 280a 2020 2020 2243 6f6d 706c 6574  or(.    "Complet
-00002500: 696f 6e22 2c0a 2020 2020 4d4f 4e41 5f43  ion",.    MONA_C
-00002510: 5245 4453 2c0a 2020 2020 434f 4e54 4558  REDS,.    CONTEX
-00002520: 545f 434c 4153 535f 4e41 4d45 2c0a 290a  T_CLASS_NAME,.).
-00002530: 0a23 2053 6574 2075 7020 7468 6520 4150  .# Set up the AP
-00002540: 4920 656e 6470 6f69 6e74 2055 524c 2061  I endpoint URL a
-00002550: 6e64 2061 7574 6865 6e74 6963 6174 696f  nd authenticatio
-00002560: 6e20 6865 6164 6572 730a 7572 6c20 3d20  n headers.url = 
-00002570: 2268 7474 7073 3a2f 2f61 7069 2e6f 7065  "https://api.ope
-00002580: 6e61 692e 636f 6d2f 7631 2f63 6f6d 706c  nai.com/v1/compl
-00002590: 6574 696f 6e73 220a 6865 6164 6572 7320  etions".headers 
-000025a0: 3d20 7b0a 2020 2020 2243 6f6e 7465 6e74  = {.    "Content
-000025b0: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
-000025c0: 7469 6f6e 2f6a 736f 6e22 2c0a 2020 2020  tion/json",.    
-000025d0: 2241 7574 686f 7269 7a61 7469 6f6e 223a  "Authorization":
-000025e0: 2066 2242 6561 7265 7220 7b65 6e76 6972   f"Bearer {envir
-000025f0: 6f6e 2e67 6574 2827 4f50 454e 5f41 495f  on.get('OPEN_AI_
-00002600: 4b45 5927 297d 222c 0a7d 0a0a 2320 5365  KEY')}",.}..# Se
-00002610: 7420 7570 2074 6865 2072 6571 7565 7374  t up the request
-00002620: 2064 6174 610a 6461 7461 203d 207b 0a20   data.data = {. 
-00002630: 2020 2022 7072 6f6d 7074 223a 2070 726f     "prompt": pro
-00002640: 6d70 742c 0a20 2020 2022 6d61 785f 746f  mpt,.    "max_to
-00002650: 6b65 6e73 223a 206d 6178 5f74 6f6b 656e  kens": max_token
-00002660: 732c 0a20 2020 2022 7465 6d70 6572 6174  s,.    "temperat
-00002670: 7572 6522 3a20 7465 6d70 6572 6174 7572  ure": temperatur
-00002680: 652c 0a20 2020 2022 6d6f 6465 6c22 3a20  e,.    "model": 
-00002690: 6d6f 6465 6c2c 0a20 2020 2022 6e22 3a20  model,.    "n": 
-000026a0: 6e2c 0a7d 0a0a 2320 5468 6520 6c6f 675f  n,.}..# The log_
-000026b0: 7265 7175 6573 7420 6675 6e63 7469 6f6e  request function
-000026c0: 2072 6574 7572 6e73 2074 776f 206f 7468   returns two oth
-000026d0: 6572 2066 756e 6374 696f 6e20 666f 7220  er function for 
-000026e0: 6c61 7465 7220 6c6f 6767 696e 670a 2320  later logging.# 
-000026f0: 7468 6520 7265 7370 6f6e 7365 206f 7220  the response or 
-00002700: 7468 6520 6578 6365 7074 696f 6e2e 2057  the exception. W
-00002710: 6865 6e20 7765 206c 6174 6572 2064 6f20  hen we later do 
-00002720: 7468 6174 2c20 7468 6520 6c6f 6767 6572  that, the logger
-00002730: 2077 696c 6c0a 2320 6163 7475 616c 6c79   will.# actually
-00002740: 2063 616c 6375 6c61 7465 2061 6c6c 2074   calculate all t
-00002750: 6865 2072 656c 6576 616e 7420 6d65 7472  he relevant metr
-00002760: 6963 7320 616e 6420 7769 6c6c 2073 656e  ics and will sen
-00002770: 6420 7468 656d 2074 6f0a 2320 4d6f 6e61  d them to.# Mona
-00002780: 2e0a 7265 7370 6f6e 7365 5f6c 6f67 6765  ..response_logge
-00002790: 722c 2065 7863 6570 7469 6f6e 5f6c 6f67  r, exception_log
-000027a0: 6765 7220 3d20 6d6f 6e61 5f6c 6f67 6765  ger = mona_logge
-000027b0: 722e 6c6f 675f 7265 7175 6573 7428 0a20  r.log_request(. 
-000027c0: 2020 2064 6174 612c 2061 6464 6974 696f     data, additio
-000027d0: 6e61 6c5f 6461 7461 3d7b 2263 7573 746f  nal_data={"custo
-000027e0: 6d65 725f 6964 223a 2022 4135 3331 3235  mer_id": "A53125
-000027f0: 3122 7d0a 290a 0a74 7279 3a0a 2020 2020  1"}.)..try:.    
-00002800: 2320 5365 6e64 2074 6865 2072 6571 7565  # Send the reque
-00002810: 7374 2074 6f20 7468 6520 4150 490a 2020  st to the API.  
-00002820: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
-00002830: 7565 7374 732e 706f 7374 2875 726c 2c20  uests.post(url, 
-00002840: 6865 6164 6572 733d 6865 6164 6572 732c  headers=headers,
-00002850: 206a 736f 6e3d 6461 7461 290a 0a20 2020   json=data)..   
-00002860: 2023 2043 6865 636b 2066 6f72 2048 5454   # Check for HTT
-00002870: 5020 6572 726f 7273 0a20 2020 2072 6573  P errors.    res
-00002880: 706f 6e73 652e 7261 6973 655f 666f 725f  ponse.raise_for_
-00002890: 7374 6174 7573 2829 0a0a 2020 2020 2320  status()..    # 
-000028a0: 4c6f 6720 7265 7370 6f6e 7365 2074 6f20  Log response to 
-000028b0: 4d6f 6e61 0a20 2020 2072 6573 706f 6e73  Mona.    respons
-000028c0: 655f 6c6f 6767 6572 2872 6573 706f 6e73  e_logger(respons
-000028d0: 652e 6a73 6f6e 2829 290a 2020 2020 7072  e.json()).    pr
-000028e0: 696e 7428 7265 7370 6f6e 7365 2e6a 736f  int(response.jso
-000028f0: 6e28 295b 2263 686f 6963 6573 225d 5b30  n()["choices"][0
-00002900: 5d5b 2274 6578 7422 5d29 0a0a 6578 6365  ]["text"])..exce
-00002910: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00002920: 6572 723a 0a20 2020 2023 204c 6f67 2065  err:.    # Log e
-00002930: 7863 6570 7469 6f6e 2074 6f20 4d6f 6e61  xception to Mona
-00002940: 0a20 2020 2065 7863 6570 7469 6f6e 5f6c  .    exception_l
-00002950: 6f67 6765 7228 290a 6060 600a 0a23 2323  ogger().```..###
-00002960: 2053 7472 6561 6d20 7375 7070 6f72 740a   Stream support.
-00002970: 0a4f 7065 6e41 4920 616c 6c6f 7773 2072  .OpenAI allows r
-00002980: 6563 6569 7669 6e67 2072 6573 706f 6e73  eceiving respons
-00002990: 6573 2061 7320 6120 7374 7265 616d 206f  es as a stream o
-000029a0: 6620 746f 6b65 6e73 2075 7369 6e67 2074  f tokens using t
-000029b0: 6865 2022 7374 7265 616d 2220 7061 7261  he "stream" para
-000029c0: 6d65 7465 722e 2057 6865 6e20 7468 6973  meter. When this
-000029d0: 2069 7320 646f 6e65 2c20 4d6f 6e61 2077   is done, Mona w
-000029e0: 696c 6c20 636f 6c6c 6563 7420 616c 6c20  ill collect all 
-000029f0: 7468 6520 746f 6b65 6e73 2069 6e20 6d65  the tokens in me
-00002a00: 6d6f 7279 2061 6e64 2077 696c 6c20 6372  mory and will cr
-00002a10: 6561 7465 2074 6865 2061 6e61 6c79 7369  eate the analysi
-00002a20: 7320 616e 6420 6c6f 6720 6f75 7420 7468  s and log out th
-00002a30: 6520 6461 7461 2074 6865 206d 6f6d 656e  e data the momen
-00002a40: 7420 7468 6520 7374 7265 616d 2069 7320  t the stream is 
-00002a50: 6f76 6572 2e20 596f 7520 646f 6e27 7420  over. You don't 
-00002a60: 6e65 6564 2074 6f20 646f 2061 6e79 7468  need to do anyth
-00002a70: 696e 6720 746f 206d 616b 6520 7468 6973  ing to make this
-00002a80: 2068 6170 7065 6e2e 0a0a 5369 6e63 6520   happen...Since 
-00002a90: 666f 7220 7374 7265 616d 696e 6720 7265  for streaming re
-00002aa0: 7370 6f6e 7365 7320 4f70 656e 4149 2064  sponses OpenAI d
-00002ab0: 6f65 736e 2774 2073 7570 706c 7920 7468  oesn't supply th
-00002ac0: 6520 6675 6c6c 2075 7361 6765 2074 6f6b  e full usage tok
-00002ad0: 656e 7320 7375 6d6d 6172 792c 204d 6f6e  ens summary, Mon
-00002ae0: 6120 7573 6573 2074 6865 2074 696b 746f  a uses the tikto
-00002af0: 6b65 6e20 7061 636b 6167 6520 746f 2063  ken package to c
-00002b00: 616c 6375 6c61 7465 2074 6865 2074 6f6b  alculate the tok
-00002b10: 656e 7320 6f66 2074 6865 2070 726f 6d70  ens of the promp
-00002b20: 7420 616e 6420 636f 6d70 6c65 7469 6f6e  t and completion
-00002b30: 2061 6e64 206c 6f67 2074 6865 6d20 666f   and log them fo
-00002b40: 7220 6d6f 6e69 746f 7269 6e67 2e0a 0a4e  r monitoring...N
-00002b50: 4f54 453a 2053 7472 6561 6d20 6973 2063  OTE: Stream is c
-00002b60: 7572 7265 6e74 6c79 206f 6e6c 7920 7375  urrently only su
-00002b70: 7070 6f72 7465 6420 7769 7468 2053 444b  pported with SDK
-00002b80: 2075 7361 6765 2c20 616e 6420 6e6f 7420   usage, and not 
-00002b90: 7769 7468 2075 7369 6e67 2052 4553 5420  with using REST 
-00002ba0: 6469 7265 6374 6c79 2e0a 0a23 2320 4c61  directly...## La
-00002bb0: 6e67 4368 6169 6e20 7375 7070 6f72 740a  ngChain support.
-00002bc0: 0a59 6f75 2063 616e 2075 7365 2074 6865  .You can use the
-00002bd0: 2065 7870 6f72 7465 6420 606d 6f6e 6974   exported `monit
-00002be0: 6f72 5f6c 616e 6763 6861 696e 5f6c 6c6d  or_langchain_llm
-00002bf0: 6020 746f 2077 7261 7020 6120 4c61 6e67  ` to wrap a Lang
-00002c00: 4368 6169 6e20 4f70 656e 4149 204c 4c4d  Chain OpenAI LLM
-00002c10: 2028 6368 6174 206f 7220 6e6f 726d 616c   (chat or normal
-00002c20: 2920 7769 7468 204d 6f6e 6127 7320 6d6f  ) with Mona's mo
-00002c30: 6e69 746f 7269 6e67 2063 6170 6162 696c  nitoring capabil
-00002c40: 6974 6965 733a 0a0a 6060 6070 790a 6672  ities:..```py.fr
-00002c50: 6f6d 206d 6f6e 615f 6f70 656e 6169 2069  om mona_openai i
-00002c60: 6d70 6f72 7420 6d6f 6e69 746f 725f 6c61  mport monitor_la
-00002c70: 6e67 6368 6169 6e5f 6c6c 6d0a 0a66 726f  ngchain_llm..fro
-00002c80: 6d20 6c61 6e67 6368 6169 6e2e 6c6c 6d73  m langchain.llms
-00002c90: 2069 6d70 6f72 7420 4f70 656e 4149 0a0a   import OpenAI..
-00002ca0: 2320 5772 6170 2074 6865 204c 4c4d 206f  # Wrap the LLM o
-00002cb0: 626a 6563 7420 7769 7468 204d 6f6e 6120  bject with Mona 
-00002cc0: 6d6f 6e69 746f 7269 6e67 2e0a 6c6c 6d20  monitoring..llm 
-00002cd0: 3d20 6d6f 6e69 746f 725f 6c61 6e67 6368  = monitor_langch
-00002ce0: 6169 6e5f 6c6c 6d28 0a20 2020 204f 7065  ain_llm(.    Ope
-00002cf0: 6e41 4928 4f50 454e 5f41 495f 4b45 5929  nAI(OPEN_AI_KEY)
-00002d00: 2c0a 2020 2020 4d4f 4e41 5f43 5245 4453  ,.    MONA_CREDS
-00002d10: 2c0a 2020 2020 434f 4e54 4558 545f 434c  ,.    CONTEXT_CL
-00002d20: 4153 535f 4e41 4d45 290a 6060 600a 0a53  ASS_NAME).```..S
-00002d30: 6565 2066 756c 6c20 6578 616d 706c 6520  ee full example 
-00002d40: 696e 2063 6f6d 706c 6574 696f 6e5f 6c61  in completion_la
-00002d50: 6e67 6368 6169 6e2e 7079 2069 6e20 7468  ngchain.py in th
-00002d60: 6520 6578 616d 706c 6573 2066 6f6c 6465  e examples folde
-00002d70: 722e 0a0a 2323 204d 6f6e 6120 5344 4b0a  r...## Mona SDK.
-00002d80: 0a54 6869 7320 7061 636b 6167 6520 7573  .This package us
-00002d90: 6573 2074 6865 206d 6f6e 615f 7364 6b20  es the mona_sdk 
-00002da0: 7061 636b 6167 6520 746f 2065 7870 6f72  package to expor
-00002db0: 7420 7468 6520 7265 6c65 7661 6e74 2064  t the relevant d
-00002dc0: 6174 6120 746f 204d 6f6e 612e 2054 6865  ata to Mona. The
-00002dd0: 7265 2061 7265 2073 6576 6572 616c 2065  re are several e
-00002de0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00002df0: 626c 6573 2079 6f75 2063 616e 2075 7365  bles you can use
-00002e00: 2074 6f20 636f 6e66 6967 7572 6520 7468   to configure th
-00002e10: 6520 5344 4b27 7320 6265 6861 7669 6f72  e SDK's behavior
-00002e20: 2e20 466f 7220 6578 616d 706c 652c 2079  . For example, y
-00002e30: 6f75 2063 616e 2073 6574 2069 7420 7570  ou can set it up
-00002e40: 2074 6f20 7261 6973 6520 6578 6365 7074   to raise except
-00002e50: 696f 6e73 2077 6865 6e20 6578 706f 7274  ions when export
-00002e60: 696e 6720 6461 7461 2074 6f20 4d6f 6e61  ing data to Mona
-00002e70: 2066 6169 6c73 2028 6974 2064 6f65 736e   fails (it doesn
-00002e80: 2774 2064 6f20 7468 6174 2062 7920 6465  't do that by de
-00002e90: 6661 756c 7429 2e0a 0a23 2320 4d6f 6e69  fault)...## Moni
-00002ea0: 746f 7269 6e67 2066 6f72 2070 726f 6661  toring for profa
-00002eb0: 6e69 7479 0a0a 4d6f 6e61 2075 7365 7320  nity..Mona uses 
-00002ec0: 7468 6520 616c 742d 7072 6f66 616e 6974  the alt-profanit
-00002ed0: 792d 6368 6563 6b20 7061 6361 6b67 6520  y-check pacakge 
-00002ee0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00002ef0: 672f 7072 6f6a 6563 742f 616c 742d 7072  g/project/alt-pr
-00002f00: 6f66 616e 6974 792d 6368 6563 6b2f 2920  ofanity-check/) 
-00002f10: 746f 2063 7265 6174 6520 626f 7468 2062  to create both b
-00002f20: 6f6f 6c65 616e 2070 7265 6469 6374 696f  oolean predictio
-00002f30: 6e73 2061 6e64 2070 726f 6261 6269 6c74  ns and probabilt
-00002f40: 7920 7363 6f72 6573 2066 6f72 2074 6865  y scores for the
-00002f50: 2065 7869 7374 656e 6365 206f 6620 7072   existence of pr
-00002f60: 6f66 616e 6974 7920 626f 7468 2069 6e20  ofanity both in 
-00002f70: 7468 6520 7072 6f6d 7074 2061 6e64 2069  the prompt and i
-00002f80: 6e20 7468 6520 7265 7370 6f6e 7365 732e  n the responses.
-00002f90: 2057 6520 7573 6520 7468 6520 6275 696c   We use the buil
-00002fa0: 7420 696e 2070 6163 6b61 6765 206d 6574  t in package met
-00002fb0: 686f 6473 2066 6f72 2074 6861 742e 2049  hods for that. I
-00002fc0: 6620 796f 7520 7761 6e74 2c20 666f 7220  f you want, for 
-00002fd0: 6578 616d 706c 652c 2074 6f20 7573 6520  example, to use 
-00002fe0: 6120 6469 6666 6572 656e 7420 7072 6f62  a different prob
-00002ff0: 6162 696c 6974 7920 7468 7265 7368 6f6c  ability threshol
-00003000: 6420 666f 7220 7468 6520 626f 6f6c 6561  d for the boolea
-00003010: 6e20 7072 6564 6963 7469 6f6e 2c20 796f  n prediction, yo
-00003020: 7520 6361 6e20 646f 2074 6861 7420 6279  u can do that by
-00003030: 2063 6861 6e67 696e 6720 796f 7572 204d   changing your M
-00003040: 6f6e 6120 636f 6e66 6967 206f 6e20 7468  ona config on th
-00003050: 6520 4d6f 6e61 2064 6173 6862 6f61 7264  e Mona dashboard
-00003060: 2e0a                                     ..
+000004b0: 3c2f 703e 0a0a 0a55 7365 206f 6e65 206c  </p>...Use one l
+000004c0: 696e 6520 6f66 2063 6f64 6520 746f 2067  ine of code to g
+000004d0: 6574 2069 6e73 7461 6e74 206c 6976 6520  et instant live 
+000004e0: 6d6f 6e69 746f 7269 6e67 2066 6f72 2079  monitoring for y
+000004f0: 6f75 7220 4f70 656e 4149 2075 7361 6765  our OpenAI usage
+00000500: 2069 6e63 6c75 6469 6e67 3a0a 2a20 546f   including:.* To
+00000510: 6b65 6e73 2075 7361 6765 0a2a 2048 616c  kens usage.* Hal
+00000520: 6c75 6369 6e61 7469 6f6e 2061 6c65 7274  lucination alert
+00000530: 730a 2a20 5072 6f66 616e 6974 7920 616e  s.* Profanity an
+00000540: 6420 7072 6976 6163 7920 616e 616c 7973  d privacy analys
+00000550: 6573 0a2a 2042 6568 6176 696f 7261 6c20  es.* Behavioral 
+00000560: 6472 6966 7473 2061 6e64 2061 6e6f 6d61  drifts and anoma
+00000570: 6c69 6573 0a2a 204c 616e 6743 6861 696e  lies.* LangChain
+00000580: 2073 7570 706f 7274 0a2a 204d 7563 6820   support.* Much 
+00000590: 6d75 6368 206d 6f72 650a 0a23 2320 5365  much more..## Se
+000005a0: 7474 696e 6720 5570 0a0a 6060 6063 6f6e  tting Up..```con
+000005b0: 736f 6c65 0a24 2070 6970 2069 6e73 7461  sole.$ pip insta
+000005c0: 6c6c 206d 6f6e 615f 6f70 656e 6169 0a60  ll mona_openai.`
+000005d0: 6060 0a0a 2323 2051 7569 636b 2053 7461  ``..## Quick Sta
+000005e0: 7274 0a0a 596f 7520 6361 6e20 6669 6e64  rt..You can find
+000005f0: 2062 6f69 6c65 7270 6c61 7465 2063 6f64   boilerplate cod
+00000600: 6520 666f 7220 6d61 6e79 2075 7365 2063  e for many use c
+00000610: 6173 6573 2075 6e64 6572 205b 7468 6520  ases under [the 
+00000620: 2265 7861 6d70 6c65 7322 2066 6f6c 6465  "examples" folde
+00000630: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+00000640: 622e 636f 6d2f 6d6f 6e61 6c61 6273 2f6d  b.com/monalabs/m
+00000650: 6f6e 612d 6f70 656e 6169 2f74 7265 652f  ona-openai/tree/
+00000660: 6d61 696e 2f65 7861 6d70 6c65 7329 2e0a  main/examples)..
+00000670: 0a23 2323 2057 6974 6820 5374 616e 6461  .### With Standa
+00000680: 7264 204c 6f67 6769 6e67 0a0a 6060 6070  rd Logging..```p
+00000690: 790a 6672 6f6d 206f 7320 696d 706f 7274  y.from os import
+000006a0: 2065 6e76 6972 6f6e 0a69 6d70 6f72 7420   environ.import 
+000006b0: 6f70 656e 6169 0a66 726f 6d20 6d6f 6e61  openai.from mona
+000006c0: 5f6f 7065 6e61 692e 6c6f 6767 6572 7320  _openai.loggers 
+000006d0: 696d 706f 7274 2053 7461 6e64 6172 644c  import StandardL
+000006e0: 6f67 6765 720a 6672 6f6d 206c 6f67 6769  ogger.from loggi
+000006f0: 6e67 2069 6d70 6f72 7420 5741 524e 494e  ng import WARNIN
+00000700: 470a 0a66 726f 6d20 6d6f 6e61 5f6f 7065  G..from mona_ope
+00000710: 6e61 6920 696d 706f 7274 206d 6f6e 6974  nai import monit
+00000720: 6f72 5f77 6974 685f 6c6f 6767 6572 0a0a  or_with_logger..
+00000730: 6f70 656e 6169 2e61 7069 5f6b 6579 203d  openai.api_key =
+00000740: 2065 6e76 6972 6f6e 2e67 6574 2822 4f50   environ.get("OP
+00000750: 454e 5f41 495f 4b45 5922 290a 0a6d 6f6e  EN_AI_KEY")..mon
+00000760: 6974 6f72 6564 5f63 6f6d 706c 6574 696f  itored_completio
+00000770: 6e20 3d20 6d6f 6e69 746f 725f 7769 7468  n = monitor_with
+00000780: 5f6c 6f67 6765 7228 0a20 2020 206f 7065  _logger(.    ope
+00000790: 6e61 692e 436f 6d70 6c65 7469 6f6e 2c0a  nai.Completion,.
+000007a0: 2020 2020 5374 616e 6461 7264 4c6f 6767      StandardLogg
+000007b0: 6572 2857 4152 4e49 4e47 292c 0a29 0a0a  er(WARNING),.)..
+000007c0: 7265 7370 6f6e 7365 203d 206d 6f6e 6974  response = monit
+000007d0: 6f72 6564 5f63 6f6d 706c 6574 696f 6e2e  ored_completion.
+000007e0: 6372 6561 7465 280a 2020 2020 6d6f 6465  create(.    mode
+000007f0: 6c3d 2274 6578 742d 6164 612d 3030 3122  l="text-ada-001"
+00000800: 2c0a 2020 2020 7072 6f6d 7074 3d22 4920  ,.    prompt="I 
+00000810: 7761 6e74 2074 6f20 6765 6e65 7261 7465  want to generate
+00000820: 2073 6f6d 6520 7465 7874 2061 626f 7574   some text about
+00000830: 2022 2c0a 2020 2020 6d61 785f 746f 6b65   ",.    max_toke
+00000840: 6e73 3d32 302c 0a20 2020 206e 3d31 2c0a  ns=20,.    n=1,.
+00000850: 2020 2020 7465 6d70 6572 6174 7572 653d      temperature=
+00000860: 302e 322c 0a20 2020 2023 2041 6464 696e  0.2,.    # Addin
+00000870: 6720 6164 6469 7469 6f6e 616c 2069 6e66  g additional inf
+00000880: 6f72 6d61 7469 6f6e 2066 6f72 206d 6f6e  ormation for mon
+00000890: 6974 6f72 696e 6720 7075 7270 6f73 6573  itoring purposes
+000008a0: 2c20 756e 7265 6c61 7465 6420 746f 0a20  , unrelated to. 
+000008b0: 2020 2023 2069 6e74 6572 6e61 6c20 4f70     # internal Op
+000008c0: 656e 4149 2063 616c 6c2e 0a20 2020 204d  enAI call..    M
+000008d0: 4f4e 415f 6164 6469 7469 6f6e 616c 5f64  ONA_additional_d
+000008e0: 6174 613d 7b22 6375 7374 6f6d 6572 5f69  ata={"customer_i
+000008f0: 6422 3a20 2241 3533 3132 3531 227d 2c0a  d": "A531251"},.
+00000900: 290a 7072 696e 7428 7265 7370 6f6e 7365  ).print(response
+00000910: 2e63 686f 6963 6573 5b30 5d2e 7465 7874  .choices[0].text
+00000920: 290a 6060 600a 0a23 2323 2057 6974 6820  ).```..### With 
+00000930: 4d6f 6e61 0a0a 5b53 6967 6e20 7570 2066  Mona..[Sign up f
+00000940: 6f72 2061 2066 7265 6520 4d6f 6e61 2061  or a free Mona a
+00000950: 6363 6f75 6e74 2068 6572 655d 2868 7474  ccount here](htt
+00000960: 7073 3a2f 2f77 7777 2e6d 6f6e 616c 6162  ps://www.monalab
+00000970: 732e 696f 2f6f 7065 6e61 692d 6770 742d  s.io/openai-gpt-
+00000980: 6d6f 6e69 746f 7269 6e67 292e 0a0a 6060  monitoring)...``
+00000990: 6070 790a 6672 6f6d 206f 7320 696d 706f  `py.from os impo
+000009a0: 7274 2065 6e76 6972 6f6e 0a69 6d70 6f72  rt environ.impor
+000009b0: 7420 6f70 656e 6169 0a0a 6672 6f6d 206d  t openai..from m
+000009c0: 6f6e 615f 6f70 656e 6169 2069 6d70 6f72  ona_openai impor
+000009d0: 7420 6d6f 6e69 746f 720a 0a6f 7065 6e61  t monitor..opena
+000009e0: 692e 6170 695f 6b65 7920 3d20 656e 7669  i.api_key = envi
+000009f0: 726f 6e2e 6765 7428 224f 5045 4e5f 4149  ron.get("OPEN_AI
+00000a00: 5f4b 4559 2229 0a0a 4d4f 4e41 5f41 5049  _KEY")..MONA_API
+00000a10: 5f4b 4559 203d 2065 6e76 6972 6f6e 2e67  _KEY = environ.g
+00000a20: 6574 2822 4d4f 4e41 5f41 5049 5f4b 4559  et("MONA_API_KEY
+00000a30: 2229 0a4d 4f4e 415f 5345 4352 4554 203d  ").MONA_SECRET =
+00000a40: 2065 6e76 6972 6f6e 2e67 6574 2822 4d4f   environ.get("MO
+00000a50: 4e41 5f53 4543 5245 5422 290a 4d4f 4e41  NA_SECRET").MONA
+00000a60: 5f43 5245 4453 203d 207b 0a20 2020 2022  _CREDS = {.    "
+00000a70: 6b65 7922 3a20 4d4f 4e41 5f41 5049 5f4b  key": MONA_API_K
+00000a80: 4559 2c0a 2020 2020 2273 6563 7265 7422  EY,.    "secret"
+00000a90: 3a20 4d4f 4e41 5f53 4543 5245 542c 0a7d  : MONA_SECRET,.}
+00000aa0: 0a43 4f4e 5445 5854 5f43 4c41 5353 5f4e  .CONTEXT_CLASS_N
+00000ab0: 414d 4520 3d20 2253 4f4d 455f 4d4f 4e49  AME = "SOME_MONI
+00000ac0: 544f 5249 4e47 5f43 4f4e 5445 5854 5f4e  TORING_CONTEXT_N
+00000ad0: 414d 4522 0a0a 0a6d 6f6e 6974 6f72 6564  AME"...monitored
+00000ae0: 5f63 6f6d 706c 6574 696f 6e20 3d20 6d6f  _completion = mo
+00000af0: 6e69 746f 7228 0a20 2020 206f 7065 6e61  nitor(.    opena
+00000b00: 692e 436f 6d70 6c65 7469 6f6e 2c0a 2020  i.Completion,.  
+00000b10: 2020 4d4f 4e41 5f43 5245 4453 2c0a 2020    MONA_CREDS,.  
+00000b20: 2020 434f 4e54 4558 545f 434c 4153 535f    CONTEXT_CLASS_
+00000b30: 4e41 4d45 2c0a 290a 0a72 6573 706f 6e73  NAME,.)..respons
+00000b40: 6520 3d20 6d6f 6e69 746f 7265 645f 636f  e = monitored_co
+00000b50: 6d70 6c65 7469 6f6e 2e63 7265 6174 6528  mpletion.create(
+00000b60: 0a20 2020 206d 6f64 656c 3d22 7465 7874  .    model="text
+00000b70: 2d61 6461 2d30 3031 222c 0a20 2020 2070  -ada-001",.    p
+00000b80: 726f 6d70 743d 2249 2077 616e 7420 746f  rompt="I want to
+00000b90: 2067 656e 6572 6174 6520 736f 6d65 2074   generate some t
+00000ba0: 6578 7420 6162 6f75 7420 222c 0a20 2020  ext about ",.   
+00000bb0: 206d 6178 5f74 6f6b 656e 733d 3230 2c0a   max_tokens=20,.
+00000bc0: 2020 2020 6e3d 312c 0a20 2020 2074 656d      n=1,.    tem
+00000bd0: 7065 7261 7475 7265 3d30 2e32 2c0a 2020  perature=0.2,.  
+00000be0: 2020 2320 4164 6469 6e67 2061 6464 6974    # Adding addit
+00000bf0: 696f 6e61 6c20 696e 666f 726d 6174 696f  ional informatio
+00000c00: 6e20 666f 7220 6d6f 6e69 746f 7269 6e67  n for monitoring
+00000c10: 2070 7572 706f 7365 732c 2075 6e72 656c   purposes, unrel
+00000c20: 6174 6564 2074 6f0a 2020 2020 2320 696e  ated to.    # in
+00000c30: 7465 726e 616c 204f 7065 6e41 4920 6361  ternal OpenAI ca
+00000c40: 6c6c 2e0a 2020 2020 4d4f 4e41 5f61 6464  ll..    MONA_add
+00000c50: 6974 696f 6e61 6c5f 6461 7461 3d7b 2263  itional_data={"c
+00000c60: 7573 746f 6d65 725f 6964 223a 2022 4135  ustomer_id": "A5
+00000c70: 3331 3235 3122 7d2c 0a29 0a70 7269 6e74  31251"},.).print
+00000c80: 2872 6573 706f 6e73 652e 6368 6f69 6365  (response.choice
+00000c90: 735b 305d 2e74 6578 7429 0a60 6060 0a0a  s[0].text).```..
+00000ca0: 2323 2053 7570 706f 7274 6564 204f 7065  ## Supported Ope
+00000cb0: 6e41 4920 4150 4973 0a43 7572 7265 6e74  nAI APIs.Current
+00000cc0: 6c79 2074 6869 7320 636c 6965 6e74 2073  ly this client s
+00000cd0: 7570 706f 7274 7320 606f 7065 6e61 692e  upports `openai.
+00000ce0: 436f 6d70 6c65 7469 6f6e 6020 616e 6420  Completion` and 
+00000cf0: 606f 7065 6e61 692e 4368 6174 436f 6d70  `openai.ChatComp
+00000d00: 6c65 7469 6f6e 602e 204d 6f6e 6120 6361  letion`. Mona ca
+00000d10: 6e20 7375 7070 6f72 7420 7072 6f63 6573  n support proces
+00000d20: 7365 7320 6261 7365 6420 6f6e 206f 7468  ses based on oth
+00000d30: 6572 2041 5049 7320 616e 6420 616c 736f  er APIs and also
+00000d40: 206e 6f6e 2d4f 7065 6e41 492d 6261 7365   non-OpenAI-base
+00000d50: 6420 6170 7073 2e0a 4966 2079 6f75 2068  d apps..If you h
+00000d60: 6176 6520 6120 6469 6666 6572 7265 6e74  ave a differrent
+00000d70: 2075 7365 2d63 6173 652c 2077 6527 6420   use-case, we'd 
+00000d80: 6c6f 7665 2074 6f20 6865 6172 2061 626f  love to hear abo
+00000d90: 7574 2069 7421 2050 6c65 6173 6520 656d  ut it! Please em
+00000da0: 6169 6c20 7573 2061 7420 7375 7070 6f72  ail us at suppor
+00000db0: 7440 6d6f 6e61 6c61 6273 2e69 6f2e 0a0a  t@monalabs.io...
+00000dc0: 2323 2055 7361 6765 0a23 2323 2049 6e69  ## Usage.### Ini
+00000dd0: 7469 616c 697a 6174 696f 6e0a 0a54 6865  tialization..The
+00000de0: 206d 6169 6e20 616e 6420 6f6e 6c79 2066   main and only f
+00000df0: 756e 6374 696f 6e20 6578 706f 7365 6420  unction exposed 
+00000e00: 696e 2074 6869 7320 7061 636b 6167 6520  in this package 
+00000e10: 6973 2060 6d6f 6e69 746f 7260 2e0a 6060  is `monitor`..``
+00000e20: 6070 790a 696d 706f 7274 206f 7065 6e61  `py.import opena
+00000e30: 690a 0a66 726f 6d20 6d6f 6e61 5f6f 7065  i..from mona_ope
+00000e40: 6e61 6920 696d 706f 7274 206d 6f6e 6974  nai import monit
+00000e50: 6f72 0a0a 6f70 656e 6169 2e61 7069 5f6b  or..openai.api_k
+00000e60: 6579 203d 2065 6e76 6972 6f6e 2e67 6574  ey = environ.get
+00000e70: 2822 4f50 454e 5f41 495f 4b45 5922 290a  ("OPEN_AI_KEY").
+00000e80: 0a6d 6f6e 6974 6f72 6564 5f63 6f6d 706c  .monitored_compl
+00000e90: 6574 696f 6e20 3d20 6d6f 6e69 746f 7228  etion = monitor(
+00000ea0: 0a20 2020 206f 7065 6e61 692e 436f 6d70  .    openai.Comp
+00000eb0: 6c65 7469 6f6e 2c0a 2020 2020 280a 2020  letion,.    (.  
+00000ec0: 2020 2020 2020 656e 7669 726f 6e2e 6765        environ.ge
+00000ed0: 7428 224d 4f4e 415f 4150 495f 4b45 5922  t("MONA_API_KEY"
+00000ee0: 292c 0a20 2020 2020 2020 2065 6e76 6972  ),.        envir
+00000ef0: 6f6e 2e67 6574 2822 4d4f 4e41 5f53 4543  on.get("MONA_SEC
+00000f00: 5245 5422 292c 0a20 2020 2029 2c0a 2020  RET"),.    ),.  
+00000f10: 2020 2253 4f4d 455f 4d4f 4e49 544f 5249    "SOME_MONITORI
+00000f20: 4e47 5f43 4f4e 5445 5854 5f4e 414d 4522  NG_CONTEXT_NAME"
+00000f30: 2c0a 2020 2020 7b22 616e 616c 7973 6973  ,.    {"analysis
+00000f40: 223a 207b 2270 726f 6661 6e69 7479 223a  ": {"profanity":
+00000f50: 2046 616c 7365 7d7d 0a29 0a0a 2e2e 2e0a   False}}.)......
+00000f60: 0a6d 6f6e 6974 6f72 6564 5f63 6f6d 706c  .monitored_compl
+00000f70: 6574 696f 6e2e 6372 6561 7465 282e 2e2e  etion.create(...
+00000f80: 290a 6060 600a 0a54 6865 2060 6d6f 6e69  ).```..The `moni
+00000f90: 746f 7260 2066 756e 6374 696f 6e20 7265  tor` function re
+00000fa0: 7475 726e 7320 746f 2079 6f75 2061 2063  turns to you a c
+00000fb0: 6c61 7373 2074 6861 7420 7772 6170 7320  lass that wraps 
+00000fc0: 7468 6520 6f72 6967 696e 616c 206f 7065  the original ope
+00000fd0: 6e61 6920 656e 6470 6f69 6e74 2063 6c61  nai endpoint cla
+00000fe0: 7373 2079 6f75 2070 726f 7669 6465 2c20  ss you provide, 
+00000ff0: 7769 7468 2061 6e20 6571 7569 7661 6c65  with an equivale
+00001000: 6e74 2041 5049 2028 6265 7369 6465 7320  nt API (besides 
+00001010: 736f 6d65 2061 6464 6974 696f 6e73 206c  some additions l
+00001020: 6973 7465 6420 6265 6c6f 7729 2e0a 596f  isted below)..Yo
+00001030: 7520 6361 6e20 7468 656e 2075 7365 2074  u can then use t
+00001040: 6865 2072 6574 7572 6e65 6420 636c 6173  he returned clas
+00001050: 7327 2022 6372 6561 7465 2220 616e 6420  s' "create" and 
+00001060: 2261 6372 6561 7465 2220 6675 6e63 7469  "acreate" functi
+00001070: 6f6e 7320 6a75 7374 2061 7320 796f 7520  ons just as you 
+00001080: 776f 756c 6420 6265 666f 7265 2c20 6f6e  would before, on
+00001090: 6c79 206e 6f77 2c20 6265 7369 6465 7320  ly now, besides 
+000010a0: 6765 7474 696e 6720 7468 6520 7265 7175  getting the requ
+000010b0: 6573 7465 6420 6f70 656e 4149 2066 756e  ested openAI fun
+000010c0: 6374 696f 6e61 6c69 7479 2c20 7468 6973  ctionality, this
+000010d0: 2063 6c69 656e 7420 7769 6c6c 206c 6f67   client will log
+000010e0: 206f 7574 2074 6f20 4d6f 6e61 2773 2073   out to Mona's s
+000010f0: 6572 7665 7220 7468 6520 7061 7261 6d65  erver the parame
+00001100: 7465 7273 2079 6f75 2075 7365 6420 2865  ters you used (e
+00001110: 2e67 2e2c 2074 656d 7065 7261 7475 7265  .g., temperature
+00001120: 292c 2064 6174 6120 6162 6f75 7420 7468  ), data about th
+00001130: 6520 7265 7370 6f6e 7365 2066 726f 6d20  e response from 
+00001140: 4f70 656e 4149 2773 2073 6572 7665 722c  OpenAI's server,
+00001150: 2061 6e64 2063 7573 746f 6d20 616e 616c   and custom anal
+00001160: 7973 6573 2061 626f 7574 2074 6865 2063  yses about the c
+00001170: 616c 6c20 2865 2e67 2e2c 2070 726f 6661  all (e.g., profa
+00001180: 6e69 7479 2073 636f 7265 732c 2070 7269  nity scores, pri
+00001190: 7661 6379 2063 6865 636b 7320 666f 7220  vacy checks for 
+000011a0: 656d 6169 6c73 2f70 686f 6e65 206e 756d  emails/phone num
+000011b0: 6265 7273 2066 6f75 6e64 2069 6e20 7468  bers found in th
+000011c0: 6520 7465 7874 732c 2074 6578 7475 616c  e texts, textual
+000011d0: 2061 6e61 6c79 7365 732c 2065 7463 2e2e   analyses, etc..
+000011e0: 2e29 0a0a 5468 6520 606d 6f6e 6974 6f72  .)..The `monitor
+000011f0: 6020 6675 6e63 7469 6f6e 2072 6563 6569  ` function recei
+00001200: 7665 7320 7468 6520 666f 6c6c 6f77 696e  ves the followin
+00001210: 6720 6172 6775 6d65 6e74 733a 0a6f 7065  g arguments:.ope
+00001220: 6e61 695f 636c 6173 733a 2041 6e20 4f70  nai_class: An Op
+00001230: 656e 4149 2041 5049 2063 6c61 7373 2074  enAI API class t
+00001240: 6f20 7772 6170 2077 6974 6820 6d6f 6e69  o wrap with moni
+00001250: 746f 7269 6e67 2063 6170 6162 696c 7469  toring capabilti
+00001260: 6573 2e0a 6d6f 6e61 5f63 7265 6473 3a20  es..mona_creds: 
+00001270: 4120 6469 6374 2028 636f 6e74 6169 6e69  A dict (containi
+00001280: 6e67 2022 6b65 7922 2061 6e64 2022 7365  ng "key" and "se
+00001290: 6372 6574 2229 206f 7220 7061 6972 2028  cret") or pair (
+000012a0: 7475 706c 6529 206f 6620 4d6f 6e61 2041  tuple) of Mona A
+000012b0: 5049 206b 6579 2061 6e64 2073 6563 7265  PI key and secre
+000012c0: 7420 746f 2073 6574 2075 7020 4d6f 6e61  t to set up Mona
+000012d0: 2773 2063 6c69 656e 7473 2066 726f 6d20  's clients from 
+000012e0: 6974 7320 5344 4b2e 0a63 6f6e 7465 7874  its SDK..context
+000012f0: 5f63 6c61 7373 3a20 5468 6520 4d6f 6e61  _class: The Mona
+00001300: 2063 6f6e 7465 7874 2063 6c61 7373 206e   context class n
+00001310: 616d 6520 746f 2075 7365 2066 6f72 206d  ame to use for m
+00001320: 6f6e 6974 6f72 696e 672e 2055 7365 2061  onitoring. Use a
+00001330: 2063 6f6e 7374 616e 7420 6e61 6d65 206f   constant name o
+00001340: 6620 796f 7572 2063 686f 6963 652e 0a73  f your choice..s
+00001350: 7065 6373 3a20 4120 6469 6374 696f 6e61  pecs: A dictiona
+00001360: 7279 206f 6620 7370 6563 6966 6963 6174  ry of specificat
+00001370: 696f 6e73 2073 7563 6820 6173 206d 6f6e  ions such as mon
+00001380: 6974 6f72 696e 6720 7361 6d70 6c69 6e67  itoring sampling
+00001390: 2072 6174 696f 2e0a 0a23 2323 2320 5370   ratio...#### Sp
+000013a0: 6563 730a 5468 6520 7370 6563 7320 6172  ecs.The specs ar
+000013b0: 6720 616c 6c6f 7773 2079 6f75 2074 6f20  g allows you to 
+000013c0: 636f 6e66 6967 7572 6520 7768 6174 2073  configure what s
+000013d0: 686f 756c 6420 6265 206d 6f6e 6974 6f72  hould be monitor
+000013e0: 6564 2e20 4974 2065 7870 6563 7473 2061  ed. It expects a
+000013f0: 2070 7974 686f 6e20 6469 6374 2077 6974   python dict wit
+00001400: 6820 7468 6520 666f 6c6c 776f 696e 6720  h the follwoing 
+00001410: 706f 7373 6962 6c65 206b 6579 733a 0a2a  possible keys:.*
+00001420: 2073 616d 706c 696e 675f 7261 7469 6f20   sampling_ratio 
+00001430: 2831 293a 2041 206e 756d 6265 7220 6265  (1): A number be
+00001440: 7477 6565 6e20 3020 616e 6420 3120 666f  tween 0 and 1 fo
+00001450: 7220 686f 7720 6f66 7465 6e20 7368 6f75  r how often shou
+00001460: 6c64 2074 6865 2063 616c 6c20 6265 206c  ld the call be l
+00001470: 6f67 6765 642e 0a2a 2061 766f 6964 5f6d  ogged..* avoid_m
+00001480: 6f6e 6974 6f72 696e 675f 6578 6365 7074  onitoring_except
+00001490: 696f 6e73 2028 4661 6c73 6529 3a20 5768  ions (False): Wh
+000014a0: 6574 6865 7220 6f72 206e 6f74 2074 6f20  ether or not to 
+000014b0: 6c6f 6720 6f75 7420 746f 204d 6f6e 6120  log out to Mona 
+000014c0: 7768 656e 2074 6865 7265 2069 7320 616e  when there is an
+000014d0: 204f 7065 6e41 4920 6578 6365 7074 696f   OpenAI exceptio
+000014e0: 6e2e 2044 6566 6175 6c74 2069 7320 746f  n. Default is to
+000014f0: 2074 7261 636b 2065 7863 6570 7469 6f6e   track exception
+00001500: 7320 2d20 616e 6420 4d6f 6e61 2077 696c  s - and Mona wil
+00001510: 6c20 616c 6572 7420 796f 7520 6f6e 2074  l alert you on t
+00001520: 6869 6e67 7320 6c69 6b65 2061 206a 756d  hings like a jum
+00001530: 7020 696e 206e 756d 6265 7220 6f66 2065  p in number of e
+00001540: 7863 6570 7469 6f6e 730a 2a20 6578 706f  xceptions.* expo
+00001550: 7274 5f70 726f 6d70 7420 2846 616c 7365  rt_prompt (False
+00001560: 293a 2057 6865 7468 6572 204d 6f6e 6120  ): Whether Mona 
+00001570: 7368 6f75 6c64 2065 7870 6f72 7420 7468  should export th
+00001580: 6520 6163 7475 616c 2070 726f 6d70 7420  e actual prompt 
+00001590: 7465 7874 2e20 4265 2064 6566 6175 6c74  text. Be default
+000015a0: 2073 6574 2074 6f20 4661 6c73 6520 746f   set to False to
+000015b0: 2061 766f 6964 2070 7269 7661 6379 2063   avoid privacy c
+000015c0: 6f6e 6365 726e 732e 0a2a 2065 7870 6f72  oncerns..* expor
+000015d0: 745f 7265 7370 6f6e 7365 5f74 6578 7473  t_response_texts
+000015e0: 2028 4661 6c73 6529 3a20 5768 6574 6865   (False): Whethe
+000015f0: 7220 4d6f 6e61 2073 686f 756c 6420 6578  r Mona should ex
+00001600: 706f 7274 2074 6865 2061 6374 7561 6c20  port the actual 
+00001610: 7265 7370 6f6e 7365 2074 6578 7473 2e20  response texts. 
+00001620: 4265 2064 6566 6175 6c74 2073 6574 2074  Be default set t
+00001630: 6f20 4661 6c73 6520 746f 2061 766f 6964  o False to avoid
+00001640: 2070 7269 7661 6379 2063 6f6e 6365 726e   privacy concern
+00001650: 732e 0a2a 2061 6e61 6c79 7369 733a 2041  s..* analysis: A
+00001660: 2064 6963 7469 6f6e 6172 7920 6d61 7070   dictionary mapp
+00001670: 696e 6720 6561 6368 2061 6e61 6c79 7369  ing each analysi
+00001680: 7320 7479 7065 2074 6f20 6120 626f 6f6c  s type to a bool
+00001690: 6561 6e20 7661 6c75 6520 7465 6c6c 696e  ean value tellin
+000016a0: 6720 7468 6520 636c 6965 6e74 2077 6865  g the client whe
+000016b0: 7468 6572 206f 7220 6e6f 7420 746f 2072  ther or not to r
+000016c0: 756e 2073 6169 6420 616e 616c 7973 6973  un said analysis
+000016d0: 2061 6e64 206c 6f67 2069 7420 746f 204d   and log it to M
+000016e0: 6f6e 612e 2050 6f73 7369 626c 6520 6f70  ona. Possible op
+000016f0: 7469 6f6e 7320 6375 7272 656e 746c 7920  tions currently 
+00001700: 6172 6520 2270 7269 7661 6379 222c 2022  are "privacy", "
+00001710: 7072 6f66 616e 6974 7922 2c20 616e 6420  profanity", and 
+00001720: 2274 6578 7475 616c 222e 2042 7920 6465  "textual". By de
+00001730: 6661 756c 742c 2061 6c6c 2061 6e61 6c79  fault, all analy
+00001740: 7365 7320 7461 6b65 2070 6c61 6365 2061  ses take place a
+00001750: 6e64 2061 7265 206c 6f67 6765 6420 6f75  nd are logged ou
+00001760: 7420 746f 204d 6f6e 612e 0a0a 2323 2320  t to Mona...### 
+00001770: 5573 696e 6720 6375 7374 6f6d 206c 6f67  Using custom log
+00001780: 6765 7273 0a59 6f75 2064 6f6e 2774 2068  gers.You don't h
+00001790: 6176 6520 746f 2068 6176 6520 6120 4d6f  ave to have a Mo
+000017a0: 6e61 2061 6363 6f75 6e74 2074 6f20 7573  na account to us
+000017b0: 6520 7468 6973 2070 6163 6b61 6765 2e20  e this package. 
+000017c0: 596f 7520 6361 6e20 6465 6669 6e65 2073  You can define s
+000017d0: 7065 6369 6669 6320 6c6f 6767 6572 7320  pecific loggers 
+000017e0: 746f 206c 6f67 206f 7574 2074 6865 2064  to log out the d
+000017f0: 6174 6120 746f 2061 2066 696c 652c 206d  ata to a file, m
+00001800: 656d 6f72 792c 206f 7220 6a75 7374 2061  emory, or just a
+00001810: 2067 6976 656e 2070 7974 686f 6e20 6c6f   given python lo
+00001820: 6767 6572 2e20 466f 7220 6578 616d 706c  gger. For exampl
+00001830: 652c 2074 6f20 6c6f 6720 6f75 7420 7468  e, to log out th
+00001840: 6520 7265 6c65 7661 6e74 206d 6574 7269  e relevant metri
+00001850: 6373 2061 7320 5741 524e 494e 473a 0a0a  cs as WARNING:..
+00001860: 6060 6070 790a 6672 6f6d 206f 7320 696d  ```py.from os im
+00001870: 706f 7274 2065 6e76 6972 6f6e 0a69 6d70  port environ.imp
+00001880: 6f72 7420 6f70 656e 6169 0a66 726f 6d20  ort openai.from 
+00001890: 6d6f 6e61 5f6f 7065 6e61 692e 6c6f 6767  mona_openai.logg
+000018a0: 6572 7320 696d 706f 7274 2053 7461 6e64  ers import Stand
+000018b0: 6172 644c 6f67 6765 720a 6672 6f6d 206c  ardLogger.from l
+000018c0: 6f67 6769 6e67 2069 6d70 6f72 7420 5741  ogging import WA
+000018d0: 524e 494e 470a 0a66 726f 6d20 6d6f 6e61  RNING..from mona
+000018e0: 5f6f 7065 6e61 6920 696d 706f 7274 206d  _openai import m
+000018f0: 6f6e 6974 6f72 5f77 6974 685f 6c6f 6767  onitor_with_logg
+00001900: 6572 0a0a 6f70 656e 6169 2e61 7069 5f6b  er..openai.api_k
+00001910: 6579 203d 2065 6e76 6972 6f6e 2e67 6574  ey = environ.get
+00001920: 2822 4f50 454e 5f41 495f 4b45 5922 290a  ("OPEN_AI_KEY").
+00001930: 0a6d 6f6e 6974 6f72 6564 5f63 6f6d 706c  .monitored_compl
+00001940: 6574 696f 6e20 3d20 6d6f 6e69 746f 725f  etion = monitor_
+00001950: 7769 7468 5f6c 6f67 6765 7228 0a20 2020  with_logger(.   
+00001960: 206f 7065 6e61 692e 436f 6d70 6c65 7469   openai.Completi
+00001970: 6f6e 2c0a 2020 2020 5374 616e 6461 7264  on,.    Standard
+00001980: 4c6f 6767 6572 2857 4152 4e49 4e47 292c  Logger(WARNING),
+00001990: 0a29 0a0a 7265 7370 6f6e 7365 203d 206d  .)..response = m
+000019a0: 6f6e 6974 6f72 6564 5f63 6f6d 706c 6574  onitored_complet
+000019b0: 696f 6e2e 6372 6561 7465 280a 2020 2020  ion.create(.    
+000019c0: 6d6f 6465 6c3d 2274 6578 742d 6164 612d  model="text-ada-
+000019d0: 3030 3122 2c0a 2020 2020 7072 6f6d 7074  001",.    prompt
+000019e0: 3d22 4920 7761 6e74 2074 6f20 6765 6e65  ="I want to gene
+000019f0: 7261 7465 2073 6f6d 6520 7465 7874 2061  rate some text a
+00001a00: 626f 7574 2022 2c0a 2020 2020 6d61 785f  bout ",.    max_
+00001a10: 746f 6b65 6e73 3d32 302c 0a20 2020 206e  tokens=20,.    n
+00001a20: 3d31 2c0a 2020 2020 7465 6d70 6572 6174  =1,.    temperat
+00001a30: 7572 653d 302e 322c 0a20 2020 2023 2041  ure=0.2,.    # A
+00001a40: 6464 696e 6720 6164 6469 7469 6f6e 616c  dding additional
+00001a50: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f72   information for
+00001a60: 206d 6f6e 6974 6f72 696e 6720 7075 7270   monitoring purp
+00001a70: 6f73 6573 2c20 756e 7265 6c61 7465 6420  oses, unrelated 
+00001a80: 746f 0a20 2020 2023 2069 6e74 6572 6e61  to.    # interna
+00001a90: 6c20 4f70 656e 4149 2063 616c 6c2e 0a20  l OpenAI call.. 
+00001aa0: 2020 204d 4f4e 415f 6164 6469 7469 6f6e     MONA_addition
+00001ab0: 616c 5f64 6174 613d 7b22 6375 7374 6f6d  al_data={"custom
+00001ac0: 6572 5f69 6422 3a20 2241 3533 3132 3531  er_id": "A531251
+00001ad0: 227d 2c0a 290a 6060 600a 0a54 6869 7320  "},.).```..This 
+00001ae0: 5344 4b20 7072 6f76 6964 6573 2061 2073  SDK provides a s
+00001af0: 696d 706c 6520 696e 7465 7266 6163 6520  imple interface 
+00001b00: 746f 2069 6d70 6c65 6d65 6e74 2079 6f75  to implement you
+00001b10: 7220 6f77 6e20 6c6f 6767 6572 7320 6279  r own loggers by
+00001b20: 2069 6e68 6572 6974 696e 6720 6672 6f6d   inheriting from
+00001b30: 204c 6f67 6765 7220 756e 6465 7220 6c6f   Logger under lo
+00001b40: 6767 6572 732f 6c6f 6767 6572 2e70 792e  ggers/logger.py.
+00001b50: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
+00001b60: 6279 2075 7369 6e67 2074 6865 2073 7461  by using the sta
+00001b70: 6e64 6172 6420 7079 7468 6f6e 206c 6f67  ndard python log
+00001b80: 6769 6e67 206c 6962 7261 7279 2061 7320  ging library as 
+00001b90: 696e 2074 6865 2065 7861 6d70 6c65 2c20  in the example, 
+00001ba0: 796f 7520 6361 6e20 6372 6561 7465 206c  you can create l
+00001bb0: 6f67 6769 6e67 2068 616e 646c 6572 7320  ogging handlers 
+00001bc0: 746f 206c 6f67 2074 6865 2064 6174 6120  to log the data 
+00001bd0: 6f75 7420 746f 2061 6e79 206d 6563 6861  out to any mecha
+00001be0: 6e69 736d 2079 6f75 2063 686f 6f73 6520  nism you choose 
+00001bf0: 2865 2e67 2e2c 204b 6166 6b61 2c20 4c6f  (e.g., Kafka, Lo
+00001c00: 6773 7461 7368 2c20 6574 632e 2e2e 290a  gstash, etc...).
+00001c10: 0a23 2323 2043 6170 6162 696c 6974 6965  .### Capabilitie
+00001c20: 7320 6475 7269 6e67 2041 5049 2063 616c  s during API cal
+00001c30: 6c73 0a0a 4166 7465 7220 7772 6170 7069  ls..After wrappi
+00001c40: 6e67 2079 6f75 7220 656e 6470 6f69 6e74  ng your endpoint
+00001c50: 2077 6974 6820 606d 6f6e 6974 6f72 602c   with `monitor`,
+00001c60: 2079 6f75 2072 6561 6c6c 7920 646f 6e27   you really don'
+00001c70: 7420 6e65 6564 2074 6f20 646f 2061 6e79  t need to do any
+00001c80: 7468 696e 6720 656c 7365 2e20 5768 656e  thing else. When
+00001c90: 2075 7369 6e67 2060 6372 6561 7465 6020   using `create` 
+00001ca0: 6f72 2060 6163 7265 6174 6560 2064 6174  or `acreate` dat
+00001cb0: 6120 7769 6c6c 2062 6520 7472 6163 6b65  a will be tracke
+00001cc0: 6420 616e 6420 6d6f 6e69 746f 7269 6e67  d and monitoring
+00001cd0: 2077 696c 6c20 7461 6b65 2070 6c61 6365   will take place
+00001ce0: 2e0a 0a54 6865 7265 2061 7265 2c20 686f  ...There are, ho
+00001cf0: 7765 7665 722c 2073 6576 6572 616c 2063  wever, several c
+00001d00: 6170 6162 696c 6974 6965 7320 7468 6174  apabilities that
+00001d10: 2061 7265 2061 6464 6564 2074 6f20 7468   are added to th
+00001d20: 6573 6520 6675 6e63 7469 6f6e 732e 2053  ese functions. S
+00001d30: 7065 6369 6669 6361 6c6c 792c 2079 6f75  pecifically, you
+00001d40: 2063 616e 2061 6464 2074 6865 2066 6f6c   can add the fol
+00001d50: 6c6f 7769 6e67 2061 7267 756d 656e 7473  lowing arguments
+00001d60: 2074 6f20 616e 7920 6372 6561 7465 2063   to any create c
+00001d70: 616c 6c3a 0a2a 204d 4f4e 415f 636f 6e74  all:.* MONA_cont
+00001d80: 6578 745f 6964 3a20 5468 6520 756e 6971  ext_id: The uniq
+00001d90: 7565 2069 6420 6f66 2074 6865 2063 6f6e  ue id of the con
+00001da0: 7465 7874 2069 6e20 7768 6963 6820 7468  text in which th
+00001db0: 6520 6361 6c6c 2069 7320 6d61 6465 2e20  e call is made. 
+00001dc0: 4279 2075 7369 6e67 2074 6869 7320 4944  By using this ID
+00001dd0: 2079 6f75 2063 616e 2065 7870 6f72 7420   you can export 
+00001de0: 6d6f 7265 2064 6174 6120 746f 204d 6f6e  more data to Mon
+00001df0: 6120 746f 2074 6865 2073 616d 6520 636f  a to the same co
+00001e00: 6e74 6578 7420 6672 6f6d 206f 7468 6572  ntext from other
+00001e10: 2070 6c61 6365 732e 2049 6620 6e6f 7420   places. If not 
+00001e20: 7375 7070 6c69 6564 2c20 7468 6520 2269  supplied, the "i
+00001e30: 6422 2066 6965 6c64 206f 6620 7468 6520  d" field of the 
+00001e40: 4f70 656e 4149 2045 6e64 706f 696e 7427  OpenAI Endpoint'
+00001e50: 7320 7265 7370 6f6e 7365 2077 696c 6c20  s response will 
+00001e60: 6265 2075 7365 6420 6173 2074 6865 204d  be used as the M
+00001e70: 6f6e 6120 636f 6e74 6578 7420 4944 2061  ona context ID a
+00001e80: 7574 6f6d 6174 6963 616c 6c79 2e0a 2a20  utomatically..* 
+00001e90: 4d4f 4e41 5f65 7870 6f72 745f 7469 6d65  MONA_export_time
+00001ea0: 7374 616d 703a 2043 616e 2062 6520 7573  stamp: Can be us
+00001eb0: 6564 2074 6f20 7369 6d75 6c61 7465 2061  ed to simulate a
+00001ec0: 7320 6966 2074 6865 2063 7572 7265 6e74  s if the current
+00001ed0: 2063 616c 6c20 7761 7320 6d61 6465 2069   call was made i
+00001ee0: 6e20 6120 6469 6666 6572 656e 7420 7469  n a different ti
+00001ef0: 6d65 2c20 6173 2066 6172 2061 7320 4d6f  me, as far as Mo
+00001f00: 6e61 2069 7320 636f 6e63 6572 6e65 642e  na is concerned.
+00001f10: 0a2a 204d 4f4e 415f 6164 6469 7469 6f6e  .* MONA_addition
+00001f20: 616c 5f64 6174 613a 2041 204a 534f 4e2d  al_data: A JSON-
+00001f30: 7365 7269 616c 697a 6162 6c65 2064 6963  serializable dic
+00001f40: 7420 7769 7468 2061 6e79 206f 7468 6572  t with any other
+00001f50: 2064 6174 6120 796f 7520 7761 6e74 2074   data you want t
+00001f60: 6f20 6164 6420 746f 2074 6865 206d 6f6e  o add to the mon
+00001f70: 6974 6f72 696e 6720 636f 6e74 6578 742e  itoring context.
+00001f80: 2054 6869 7320 636f 6d65 7320 696e 2068   This comes in h
+00001f90: 616e 6479 2069 6620 796f 7520 7761 6e74  andy if you want
+00001fa0: 2074 6f20 6164 6420 6d6f 7265 2069 6e66   to add more inf
+00001fb0: 6f72 6d61 7469 6f6e 2074 6f20 7468 6520  ormation to the 
+00001fc0: 6d6f 6e69 746f 7269 6e67 2063 6f6e 7465  monitoring conte
+00001fd0: 7820 7468 6174 2069 736e 2774 2070 6172  x that isn't par
+00001fe0: 7420 6f66 2074 6865 2062 6173 6963 204f  t of the basic O
+00001ff0: 7065 6e41 4920 4150 4920 6361 6c6c 2069  penAI API call i
+00002000: 6e66 6f72 6d61 7469 6f6e 2e20 466f 7220  nformation. For 
+00002010: 6578 616d 706c 652c 2069 6620 796f 7520  example, if you 
+00002020: 6172 6520 7573 696e 6720 6120 7370 6563  are using a spec
+00002030: 6966 6963 2074 656d 706c 6174 6520 4944  ific template ID
+00002040: 206f 7220 6966 2074 6869 7320 6361 6c6c   or if this call
+00002050: 2069 7320 6265 696e 6720 6d61 6465 2066   is being made f
+00002060: 6f72 2061 2073 7065 6369 6669 6320 6375  or a specific cu
+00002070: 7374 6f6d 6572 2049 442c 2074 6865 7365  stomer ID, these
+00002080: 2061 7265 2066 6965 6c64 7320 796f 7520   are fields you 
+00002090: 6361 6e20 6164 6420 7468 6572 6520 746f  can add there to
+000020a0: 2068 656c 7020 6765 7420 6675 6c6c 2063   help get full c
+000020b0: 6f6e 7465 7874 2077 6865 6e20 6d6f 6e69  ontext when moni
+000020c0: 746f 7269 6e67 2077 6974 6820 4d6f 6e61  toring with Mona
+000020d0: 2e0a 0a45 7861 6d70 6c65 3a0a 6060 6070  ...Example:.```p
+000020e0: 790a 7265 7370 6f6e 7365 203d 2061 7379  y.response = asy
+000020f0: 6e63 696f 2e72 756e 286d 6f6e 6974 6f72  ncio.run(monitor
+00002100: 6564 5f63 6f6d 706c 6574 696f 6e2e 6163  ed_completion.ac
+00002110: 7265 6174 6528 0a20 2020 2065 6e67 696e  reate(.    engin
+00002120: 653d 6d6f 6465 6c2c 0a20 2020 2070 726f  e=model,.    pro
+00002130: 6d70 743d 7072 6f6d 7074 2c0a 2020 2020  mpt=prompt,.    
+00002140: 6d61 785f 746f 6b65 6e73 3d6d 6178 5f74  max_tokens=max_t
+00002150: 6f6b 656e 732c 0a20 2020 206e 3d6e 2c0a  okens,.    n=n,.
+00002160: 2020 2020 7465 6d70 6572 6174 7572 653d      temperature=
+00002170: 7465 6d70 6572 6174 7572 652c 0a20 2020  temperature,.   
+00002180: 204d 4f4e 415f 6164 6469 7469 6f6e 616c   MONA_additional
+00002190: 5f64 6174 613d 7b22 6375 7374 6f6d 6572  _data={"customer
+000021a0: 5f69 6422 3a20 2241 3533 3132 3531 227d  _id": "A531251"}
+000021b0: 2c0a 2929 0a70 7269 6e74 2872 6573 706f  ,.)).print(respo
+000021c0: 6e73 652e 6368 6f69 6365 735b 305d 2e74  nse.choices[0].t
+000021d0: 6578 7429 0a60 6060 0a0a 2323 2320 5573  ext).```..### Us
+000021e0: 696e 6720 4f70 656e 4149 2077 6974 6820  ing OpenAI with 
+000021f0: 5245 5354 2063 616c 6c73 2069 6e73 7465  REST calls inste
+00002200: 6164 206f 6620 4f70 656e 4149 2773 2050  ad of OpenAI's P
+00002210: 7974 686f 6e20 636c 6965 6e74 0a49 6e20  ython client.In 
+00002220: 736f 6d65 2063 6173 6573 2079 6f75 206d  some cases you m
+00002230: 6179 2063 686f 6f73 6520 746f 2075 7365  ay choose to use
+00002240: 204f 7065 6e41 4927 7320 4150 4920 6469   OpenAI's API di
+00002250: 7265 6374 6c79 2077 6974 6820 5245 5354  rectly with REST
+00002260: 2063 616c 6c73 2061 6e64 206e 6f74 2075   calls and not u
+00002270: 7369 6e67 204f 7065 6e41 4927 7320 5344  sing OpenAI's SD
+00002280: 4b2e 2046 6f72 2074 6865 7365 2063 6173  K. For these cas
+00002290: 6573 2077 6520 616c 6c6f 7720 6120 6d6f  es we allow a mo
+000022a0: 7265 2064 6972 6563 7420 6170 7072 6f61  re direct approa
+000022b0: 6368 2066 6f72 206c 6f67 6769 6e67 2074  ch for logging t
+000022c0: 6f20 4d6f 6e61 2061 7320 7765 6c6c 2c20  o Mona as well, 
+000022d0: 6279 2075 7369 6e67 2074 6865 2022 6765  by using the "ge
+000022e0: 745f 7265 7374 5f6d 6f6e 6974 6f72 2220  t_rest_monitor" 
+000022f0: 6675 6e63 7469 6f6e 2e20 5365 6520 6578  function. See ex
+00002300: 616d 706c 6520 6265 6c6f 772e 0a0a 6060  ample below...``
+00002310: 6070 790a 2320 4469 7265 6374 2052 4553  `py.# Direct RES
+00002320: 5420 7573 6167 652c 2077 6974 686f 7574  T usage, without
+00002330: 204f 7065 6e41 4920 636c 6965 6e74 0a69   OpenAI client.i
+00002340: 6d70 6f72 7420 7265 7175 6573 7473 0a66  mport requests.f
+00002350: 726f 6d20 6f73 2069 6d70 6f72 7420 656e  rom os import en
+00002360: 7669 726f 6e0a 6672 6f6d 206d 6f6e 615f  viron.from mona_
+00002370: 6f70 656e 6169 2069 6d70 6f72 7420 6765  openai import ge
+00002380: 745f 7265 7374 5f6d 6f6e 6974 6f72 0a0a  t_rest_monitor..
+00002390: 0a4d 4f4e 415f 4150 495f 4b45 5920 3d20  .MONA_API_KEY = 
+000023a0: 656e 7669 726f 6e2e 6765 7428 224d 4f4e  environ.get("MON
+000023b0: 415f 4150 495f 4b45 5922 290a 4d4f 4e41  A_API_KEY").MONA
+000023c0: 5f53 4543 5245 5420 3d20 656e 7669 726f  _SECRET = enviro
+000023d0: 6e2e 6765 7428 224d 4f4e 415f 5345 4352  n.get("MONA_SECR
+000023e0: 4554 2229 0a4d 4f4e 415f 4352 4544 5320  ET").MONA_CREDS 
+000023f0: 3d20 7b0a 2020 2020 226b 6579 223a 204d  = {.    "key": M
+00002400: 4f4e 415f 4150 495f 4b45 592c 0a20 2020  ONA_API_KEY,.   
+00002410: 2022 7365 6372 6574 223a 204d 4f4e 415f   "secret": MONA_
+00002420: 5345 4352 4554 2c0a 7d0a 434f 4e54 4558  SECRET,.}.CONTEX
+00002430: 545f 434c 4153 535f 4e41 4d45 203d 2022  T_CLASS_NAME = "
+00002440: 534f 4d45 5f4d 4f4e 4954 4f52 494e 475f  SOME_MONITORING_
+00002450: 434f 4e54 4558 545f 4e41 4d45 220a 0a23  CONTEXT_NAME"..#
+00002460: 2047 6574 204d 6f6e 6120 6c6f 6767 6572   Get Mona logger
+00002470: 0a6d 6f6e 615f 6c6f 6767 6572 203d 2067  .mona_logger = g
+00002480: 6574 5f72 6573 745f 6d6f 6e69 746f 7228  et_rest_monitor(
+00002490: 0a20 2020 2022 436f 6d70 6c65 7469 6f6e  .    "Completion
+000024a0: 222c 0a20 2020 204d 4f4e 415f 4352 4544  ",.    MONA_CRED
+000024b0: 532c 0a20 2020 2043 4f4e 5445 5854 5f43  S,.    CONTEXT_C
+000024c0: 4c41 5353 5f4e 414d 452c 0a29 0a0a 2320  LASS_NAME,.)..# 
+000024d0: 5365 7420 7570 2074 6865 2041 5049 2065  Set up the API e
+000024e0: 6e64 706f 696e 7420 5552 4c20 616e 6420  ndpoint URL and 
+000024f0: 6175 7468 656e 7469 6361 7469 6f6e 2068  authentication h
+00002500: 6561 6465 7273 0a75 726c 203d 2022 6874  eaders.url = "ht
+00002510: 7470 733a 2f2f 6170 692e 6f70 656e 6169  tps://api.openai
+00002520: 2e63 6f6d 2f76 312f 636f 6d70 6c65 7469  .com/v1/completi
+00002530: 6f6e 7322 0a68 6561 6465 7273 203d 207b  ons".headers = {
+00002540: 0a20 2020 2022 436f 6e74 656e 742d 5479  .    "Content-Ty
+00002550: 7065 223a 2022 6170 706c 6963 6174 696f  pe": "applicatio
+00002560: 6e2f 6a73 6f6e 222c 0a20 2020 2022 4175  n/json",.    "Au
+00002570: 7468 6f72 697a 6174 696f 6e22 3a20 6622  thorization": f"
+00002580: 4265 6172 6572 207b 656e 7669 726f 6e2e  Bearer {environ.
+00002590: 6765 7428 274f 5045 4e5f 4149 5f4b 4559  get('OPEN_AI_KEY
+000025a0: 2729 7d22 2c0a 7d0a 0a23 2053 6574 2075  ')}",.}..# Set u
+000025b0: 7020 7468 6520 7265 7175 6573 7420 6461  p the request da
+000025c0: 7461 0a64 6174 6120 3d20 7b0a 2020 2020  ta.data = {.    
+000025d0: 2270 726f 6d70 7422 3a20 7072 6f6d 7074  "prompt": prompt
+000025e0: 2c0a 2020 2020 226d 6178 5f74 6f6b 656e  ,.    "max_token
+000025f0: 7322 3a20 6d61 785f 746f 6b65 6e73 2c0a  s": max_tokens,.
+00002600: 2020 2020 2274 656d 7065 7261 7475 7265      "temperature
+00002610: 223a 2074 656d 7065 7261 7475 7265 2c0a  ": temperature,.
+00002620: 2020 2020 226d 6f64 656c 223a 206d 6f64      "model": mod
+00002630: 656c 2c0a 2020 2020 226e 223a 206e 2c0a  el,.    "n": n,.
+00002640: 7d0a 0a23 2054 6865 206c 6f67 5f72 6571  }..# The log_req
+00002650: 7565 7374 2066 756e 6374 696f 6e20 7265  uest function re
+00002660: 7475 726e 7320 7477 6f20 6f74 6865 7220  turns two other 
+00002670: 6675 6e63 7469 6f6e 2066 6f72 206c 6174  function for lat
+00002680: 6572 206c 6f67 6769 6e67 0a23 2074 6865  er logging.# the
+00002690: 2072 6573 706f 6e73 6520 6f72 2074 6865   response or the
+000026a0: 2065 7863 6570 7469 6f6e 2e20 5768 656e   exception. When
+000026b0: 2077 6520 6c61 7465 7220 646f 2074 6861   we later do tha
+000026c0: 742c 2074 6865 206c 6f67 6765 7220 7769  t, the logger wi
+000026d0: 6c6c 0a23 2061 6374 7561 6c6c 7920 6361  ll.# actually ca
+000026e0: 6c63 756c 6174 6520 616c 6c20 7468 6520  lculate all the 
+000026f0: 7265 6c65 7661 6e74 206d 6574 7269 6373  relevant metrics
+00002700: 2061 6e64 2077 696c 6c20 7365 6e64 2074   and will send t
+00002710: 6865 6d20 746f 0a23 204d 6f6e 612e 0a72  hem to.# Mona..r
+00002720: 6573 706f 6e73 655f 6c6f 6767 6572 2c20  esponse_logger, 
+00002730: 6578 6365 7074 696f 6e5f 6c6f 6767 6572  exception_logger
+00002740: 203d 206d 6f6e 615f 6c6f 6767 6572 2e6c   = mona_logger.l
+00002750: 6f67 5f72 6571 7565 7374 280a 2020 2020  og_request(.    
+00002760: 6461 7461 2c20 6164 6469 7469 6f6e 616c  data, additional
+00002770: 5f64 6174 613d 7b22 6375 7374 6f6d 6572  _data={"customer
+00002780: 5f69 6422 3a20 2241 3533 3132 3531 227d  _id": "A531251"}
+00002790: 0a29 0a0a 7472 793a 0a20 2020 2023 2053  .)..try:.    # S
+000027a0: 656e 6420 7468 6520 7265 7175 6573 7420  end the request 
+000027b0: 746f 2074 6865 2041 5049 0a20 2020 2072  to the API.    r
+000027c0: 6573 706f 6e73 6520 3d20 7265 7175 6573  esponse = reques
+000027d0: 7473 2e70 6f73 7428 7572 6c2c 2068 6561  ts.post(url, hea
+000027e0: 6465 7273 3d68 6561 6465 7273 2c20 6a73  ders=headers, js
+000027f0: 6f6e 3d64 6174 6129 0a0a 2020 2020 2320  on=data)..    # 
+00002800: 4368 6563 6b20 666f 7220 4854 5450 2065  Check for HTTP e
+00002810: 7272 6f72 730a 2020 2020 7265 7370 6f6e  rrors.    respon
+00002820: 7365 2e72 6169 7365 5f66 6f72 5f73 7461  se.raise_for_sta
+00002830: 7475 7328 290a 0a20 2020 2023 204c 6f67  tus()..    # Log
+00002840: 2072 6573 706f 6e73 6520 746f 204d 6f6e   response to Mon
+00002850: 610a 2020 2020 7265 7370 6f6e 7365 5f6c  a.    response_l
+00002860: 6f67 6765 7228 7265 7370 6f6e 7365 2e6a  ogger(response.j
+00002870: 736f 6e28 2929 0a20 2020 2070 7269 6e74  son()).    print
+00002880: 2872 6573 706f 6e73 652e 6a73 6f6e 2829  (response.json()
+00002890: 5b22 6368 6f69 6365 7322 5d5b 305d 5b22  ["choices"][0]["
+000028a0: 7465 7874 225d 290a 0a65 7863 6570 7420  text"])..except 
+000028b0: 4578 6365 7074 696f 6e20 6173 2065 7272  Exception as err
+000028c0: 3a0a 2020 2020 2320 4c6f 6720 6578 6365  :.    # Log exce
+000028d0: 7074 696f 6e20 746f 204d 6f6e 610a 2020  ption to Mona.  
+000028e0: 2020 6578 6365 7074 696f 6e5f 6c6f 6767    exception_logg
+000028f0: 6572 2829 0a60 6060 0a0a 2323 2320 5374  er().```..### St
+00002900: 7265 616d 2073 7570 706f 7274 0a0a 4f70  ream support..Op
+00002910: 656e 4149 2061 6c6c 6f77 7320 7265 6365  enAI allows rece
+00002920: 6976 696e 6720 7265 7370 6f6e 7365 7320  iving responses 
+00002930: 6173 2061 2073 7472 6561 6d20 6f66 2074  as a stream of t
+00002940: 6f6b 656e 7320 7573 696e 6720 7468 6520  okens using the 
+00002950: 2273 7472 6561 6d22 2070 6172 616d 6574  "stream" paramet
+00002960: 6572 2e20 5768 656e 2074 6869 7320 6973  er. When this is
+00002970: 2064 6f6e 652c 204d 6f6e 6120 7769 6c6c   done, Mona will
+00002980: 2063 6f6c 6c65 6374 2061 6c6c 2074 6865   collect all the
+00002990: 2074 6f6b 656e 7320 696e 206d 656d 6f72   tokens in memor
+000029a0: 7920 616e 6420 7769 6c6c 2063 7265 6174  y and will creat
+000029b0: 6520 7468 6520 616e 616c 7973 6973 2061  e the analysis a
+000029c0: 6e64 206c 6f67 206f 7574 2074 6865 2064  nd log out the d
+000029d0: 6174 6120 7468 6520 6d6f 6d65 6e74 2074  ata the moment t
+000029e0: 6865 2073 7472 6561 6d20 6973 206f 7665  he stream is ove
+000029f0: 722e 2059 6f75 2064 6f6e 2774 206e 6565  r. You don't nee
+00002a00: 6420 746f 2064 6f20 616e 7974 6869 6e67  d to do anything
+00002a10: 2074 6f20 6d61 6b65 2074 6869 7320 6861   to make this ha
+00002a20: 7070 656e 2e0a 0a53 696e 6365 2066 6f72  ppen...Since for
+00002a30: 2073 7472 6561 6d69 6e67 2072 6573 706f   streaming respo
+00002a40: 6e73 6573 204f 7065 6e41 4920 646f 6573  nses OpenAI does
+00002a50: 6e27 7420 7375 7070 6c79 2074 6865 2066  n't supply the f
+00002a60: 756c 6c20 7573 6167 6520 746f 6b65 6e73  ull usage tokens
+00002a70: 2073 756d 6d61 7279 2c20 4d6f 6e61 2075   summary, Mona u
+00002a80: 7365 7320 7468 6520 7469 6b74 6f6b 656e  ses the tiktoken
+00002a90: 2070 6163 6b61 6765 2074 6f20 6361 6c63   package to calc
+00002aa0: 756c 6174 6520 7468 6520 746f 6b65 6e73  ulate the tokens
+00002ab0: 206f 6620 7468 6520 7072 6f6d 7074 2061   of the prompt a
+00002ac0: 6e64 2063 6f6d 706c 6574 696f 6e20 616e  nd completion an
+00002ad0: 6420 6c6f 6720 7468 656d 2066 6f72 206d  d log them for m
+00002ae0: 6f6e 6974 6f72 696e 672e 0a0a 4e4f 5445  onitoring...NOTE
+00002af0: 3a20 5374 7265 616d 2069 7320 6375 7272  : Stream is curr
+00002b00: 656e 746c 7920 6f6e 6c79 2073 7570 706f  ently only suppo
+00002b10: 7274 6564 2077 6974 6820 5344 4b20 7573  rted with SDK us
+00002b20: 6167 652c 2061 6e64 206e 6f74 2077 6974  age, and not wit
+00002b30: 6820 7573 696e 6720 5245 5354 2064 6972  h using REST dir
+00002b40: 6563 746c 792e 0a0a 2323 204c 616e 6743  ectly...## LangC
+00002b50: 6861 696e 2073 7570 706f 7274 0a0a 596f  hain support..Yo
+00002b60: 7520 6361 6e20 7573 6520 7468 6520 6578  u can use the ex
+00002b70: 706f 7274 6564 2060 6d6f 6e69 746f 725f  ported `monitor_
+00002b80: 6c61 6e67 6368 6169 6e5f 6c6c 6d60 2074  langchain_llm` t
+00002b90: 6f20 7772 6170 2061 204c 616e 6743 6861  o wrap a LangCha
+00002ba0: 696e 204f 7065 6e41 4920 4c4c 4d20 2863  in OpenAI LLM (c
+00002bb0: 6861 7420 6f72 206e 6f72 6d61 6c29 2077  hat or normal) w
+00002bc0: 6974 6820 4d6f 6e61 2773 206d 6f6e 6974  ith Mona's monit
+00002bd0: 6f72 696e 6720 6361 7061 6269 6c69 7469  oring capabiliti
+00002be0: 6573 3a0a 0a60 6060 7079 0a66 726f 6d20  es:..```py.from 
+00002bf0: 6d6f 6e61 5f6f 7065 6e61 6920 696d 706f  mona_openai impo
+00002c00: 7274 206d 6f6e 6974 6f72 5f6c 616e 6763  rt monitor_langc
+00002c10: 6861 696e 5f6c 6c6d 0a0a 6672 6f6d 206c  hain_llm..from l
+00002c20: 616e 6763 6861 696e 2e6c 6c6d 7320 696d  angchain.llms im
+00002c30: 706f 7274 204f 7065 6e41 490a 0a23 2057  port OpenAI..# W
+00002c40: 7261 7020 7468 6520 4c4c 4d20 6f62 6a65  rap the LLM obje
+00002c50: 6374 2077 6974 6820 4d6f 6e61 206d 6f6e  ct with Mona mon
+00002c60: 6974 6f72 696e 672e 0a6c 6c6d 203d 206d  itoring..llm = m
+00002c70: 6f6e 6974 6f72 5f6c 616e 6763 6861 696e  onitor_langchain
+00002c80: 5f6c 6c6d 280a 2020 2020 4f70 656e 4149  _llm(.    OpenAI
+00002c90: 284f 5045 4e5f 4149 5f4b 4559 292c 0a20  (OPEN_AI_KEY),. 
+00002ca0: 2020 204d 4f4e 415f 4352 4544 532c 0a20     MONA_CREDS,. 
+00002cb0: 2020 2043 4f4e 5445 5854 5f43 4c41 5353     CONTEXT_CLASS
+00002cc0: 5f4e 414d 4529 0a60 6060 0a0a 5365 6520  _NAME).```..See 
+00002cd0: 6675 6c6c 2065 7861 6d70 6c65 2069 6e20  full example in 
+00002ce0: 636f 6d70 6c65 7469 6f6e 5f6c 616e 6763  completion_langc
+00002cf0: 6861 696e 2e70 7920 696e 2074 6865 2065  hain.py in the e
+00002d00: 7861 6d70 6c65 7320 666f 6c64 6572 2e0a  xamples folder..
+00002d10: 0a23 2320 4d6f 6e61 2053 444b 0a0a 5468  .## Mona SDK..Th
+00002d20: 6973 2070 6163 6b61 6765 2075 7365 7320  is package uses 
+00002d30: 7468 6520 6d6f 6e61 5f73 646b 2070 6163  the mona_sdk pac
+00002d40: 6b61 6765 2074 6f20 6578 706f 7274 2074  kage to export t
+00002d50: 6865 2072 656c 6576 616e 7420 6461 7461  he relevant data
+00002d60: 2074 6f20 4d6f 6e61 2e20 5468 6572 6520   to Mona. There 
+00002d70: 6172 6520 7365 7665 7261 6c20 656e 7669  are several envi
+00002d80: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00002d90: 7320 796f 7520 6361 6e20 7573 6520 746f  s you can use to
+00002da0: 2063 6f6e 6669 6775 7265 2074 6865 2053   configure the S
+00002db0: 444b 2773 2062 6568 6176 696f 722e 2046  DK's behavior. F
+00002dc0: 6f72 2065 7861 6d70 6c65 2c20 796f 7520  or example, you 
+00002dd0: 6361 6e20 7365 7420 6974 2075 7020 746f  can set it up to
+00002de0: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
+00002df0: 7320 7768 656e 2065 7870 6f72 7469 6e67  s when exporting
+00002e00: 2064 6174 6120 746f 204d 6f6e 6120 6661   data to Mona fa
+00002e10: 696c 7320 2869 7420 646f 6573 6e27 7420  ils (it doesn't 
+00002e20: 646f 2074 6861 7420 6279 2064 6566 6175  do that by defau
+00002e30: 6c74 292e 0a0a 2323 204d 6f6e 6974 6f72  lt)...## Monitor
+00002e40: 696e 6720 666f 7220 7072 6f66 616e 6974  ing for profanit
+00002e50: 790a 0a4d 6f6e 6120 7573 6573 2074 6865  y..Mona uses the
+00002e60: 2061 6c74 2d70 726f 6661 6e69 7479 2d63   alt-profanity-c
+00002e70: 6865 636b 2070 6163 616b 6765 2028 6874  heck pacakge (ht
+00002e80: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00002e90: 726f 6a65 6374 2f61 6c74 2d70 726f 6661  roject/alt-profa
+00002ea0: 6e69 7479 2d63 6865 636b 2f29 2074 6f20  nity-check/) to 
+00002eb0: 6372 6561 7465 2062 6f74 6820 626f 6f6c  create both bool
+00002ec0: 6561 6e20 7072 6564 6963 7469 6f6e 7320  ean predictions 
+00002ed0: 616e 6420 7072 6f62 6162 696c 7479 2073  and probabilty s
+00002ee0: 636f 7265 7320 666f 7220 7468 6520 6578  cores for the ex
+00002ef0: 6973 7465 6e63 6520 6f66 2070 726f 6661  istence of profa
+00002f00: 6e69 7479 2062 6f74 6820 696e 2074 6865  nity both in the
+00002f10: 2070 726f 6d70 7420 616e 6420 696e 2074   prompt and in t
+00002f20: 6865 2072 6573 706f 6e73 6573 2e20 5765  he responses. We
+00002f30: 2075 7365 2074 6865 2062 7569 6c74 2069   use the built i
+00002f40: 6e20 7061 636b 6167 6520 6d65 7468 6f64  n package method
+00002f50: 7320 666f 7220 7468 6174 2e20 4966 2079  s for that. If y
+00002f60: 6f75 2077 616e 742c 2066 6f72 2065 7861  ou want, for exa
+00002f70: 6d70 6c65 2c20 746f 2075 7365 2061 2064  mple, to use a d
+00002f80: 6966 6665 7265 6e74 2070 726f 6261 6269  ifferent probabi
+00002f90: 6c69 7479 2074 6872 6573 686f 6c64 2066  lity threshold f
+00002fa0: 6f72 2074 6865 2062 6f6f 6c65 616e 2070  or the boolean p
+00002fb0: 7265 6469 6374 696f 6e2c 2079 6f75 2063  rediction, you c
+00002fc0: 616e 2064 6f20 7468 6174 2062 7920 6368  an do that by ch
+00002fd0: 616e 6769 6e67 2079 6f75 7220 4d6f 6e61  anging your Mona
+00002fe0: 2063 6f6e 6669 6720 6f6e 2074 6865 204d   config on the M
+00002ff0: 6f6e 6120 6461 7368 626f 6172 642e 0a0a  ona dashboard...
+00003000: 2323 2055 7369 6e67 206e 6573 742d 6173  ## Using nest-as
+00003010: 796e 6369 6f0a 0a49 6e20 656e 7669 726f  yncio..In enviro
+00003020: 6e6d 656e 7473 2069 6e20 7768 6963 6820  nments in which 
+00003030: 7468 6572 6527 7320 6120 666f 7265 7665  there's a foreve
+00003040: 7220 7275 6e6e 696e 6720 6576 656e 7420  r running event 
+00003050: 6c6f 6f70 2028 652e 672e 2c20 4a75 7079  loop (e.g., Jupy
+00003060: 7465 7220 6e6f 7465 626f 6f6b 7329 2c20  ter notebooks), 
+00003070: 7468 6520 636c 6965 6e74 206d 6967 6874  the client might
+00003080: 2075 7365 205b 6e65 7374 5f61 7379 6e63   use [nest_async
+00003090: 696f 2e61 7070 6c79 2829 5d28 6874 7470  io.apply()](http
+000030a0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000030b0: 6a65 6374 2f6e 6573 742d 6173 796e 6369  ject/nest-asynci
+000030c0: 6f2f 2920 746f 2072 756e 206a 6f69 6e74  o/) to run joint
+000030d0: 2073 796e 6320 616e 6420 6173 796e 6320   sync and async 
+000030e0: 636f 6465 2e0a                           code..
```

### Comparing `mona-openai-0.1.0/mona_openai.egg-info/SOURCES.txt` & `mona-openai-0.1.1/mona_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/pyproject.toml` & `mona-openai-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mona-openai"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Itai Bar Sinai", email="itai@monalabs.io" },
 ]
 description = "Integration client for monitoring OpenAI usage with Mona"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mona-openai-0.1.0/tests/test_chat_completion.py` & `mona-openai-0.1.1/tests/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/tests/test_completion.py` & `mona-openai-0.1.1/tests/test_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,14 +227,30 @@
         _DEFAULT_CONTEXT_CLASS,
         mona_clients_getter=get_mock_mona_clients_getter(
             (_get_mona_message(),), ()
         ),
     ).log_request(_DEFAULT_INPUT)[0](_DEFAULT_RESPONSE)
 
 
+def test_rest_more_additional_data():
+    additional_data = {"foo": "bar"}
+    more_additional_data = {"foo2": "bar2"}
+    total_additional_data = {**additional_data, **more_additional_data}
+    get_rest_monitor(
+        Completion.__name__,
+        (),
+        _DEFAULT_CONTEXT_CLASS,
+        mona_clients_getter=get_mock_mona_clients_getter(
+            (_get_mona_message(additional_data=total_additional_data),), ()
+        ),
+    ).log_request(_DEFAULT_INPUT, additional_data=additional_data)[0](
+        _DEFAULT_RESPONSE, additional_data=more_additional_data
+    )
+
+
 def test_rest_async():
     asyncio.run(
         get_rest_monitor(
             Completion.__name__,
             (),
             _DEFAULT_CONTEXT_CLASS,
             mona_clients_getter=get_mock_mona_clients_getter(
```

### Comparing `mona-openai-0.1.0/tests/test_privacy_analyzer.py` & `mona-openai-0.1.1/tests/test_privacy_analyzer.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.1.0/tests/test_textual_analyzer.py` & `mona-openai-0.1.1/tests/test_textual_analyzer.py`

 * *Files identical despite different names*

