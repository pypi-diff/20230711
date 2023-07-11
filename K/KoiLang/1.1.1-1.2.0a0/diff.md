# Comparing `tmp/KoiLang-1.1.1.tar.gz` & `tmp/KoiLang-1.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KoiLang-1.1.1.tar", last modified: Sun Jul  2 17:29:31 2023, max compression
+gzip compressed data, was "KoiLang-1.2.0a0.tar", last modified: Tue Jul 11 14:54:23 2023, max compression
```

## Comparing `KoiLang-1.1.1.tar` & `KoiLang-1.2.0a0.tar`

### file list

```diff
@@ -1,57 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.557168 KoiLang-1.1.1/
-drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.479516 KoiLang-1.1.1/KoiLang.egg-info/
--rw-rw-rw-   0        0        0    12456 2023-07-02 17:29:31.000000 KoiLang-1.1.1/KoiLang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1463 2023-07-02 17:29:31.000000 KoiLang-1.1.1/KoiLang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 17:29:31.000000 KoiLang-1.1.1/KoiLang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-02 17:29:31.000000 KoiLang-1.1.1/KoiLang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 17:29:31.000000 KoiLang-1.1.1/KoiLang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-08-17 13:41:36.000000 KoiLang-1.1.1/LICENSE
--rw-rw-rw-   0        0        0    12456 2023-07-02 17:29:31.556178 KoiLang-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    11401 2023-06-01 10:51:09.000000 KoiLang-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.511522 KoiLang-1.1.1/kola/
--rw-rw-rw-   0        0        0     1067 2023-05-18 14:12:37.000000 KoiLang-1.1.1/kola/__init__.py
--rw-rw-rw-   0        0        0     3172 2023-04-05 04:13:29.000000 KoiLang-1.1.1/kola/__main__.py
--rw-rw-rw-   0        0        0     7002 2023-04-07 10:48:13.000000 KoiLang-1.1.1/kola/_cutil.h
--rw-rw-rw-   0        0        0     3221 2023-04-06 11:35:14.000000 KoiLang-1.1.1/kola/_cutil.pxd
--rw-rw-rw-   0        0        0     1559 2023-03-28 16:42:40.000000 KoiLang-1.1.1/kola/_yylex.pxd
--rw-rw-rw-   0        0        0      375 2023-01-15 16:44:08.000000 KoiLang-1.1.1/kola/exception.py
-drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.528167 KoiLang-1.1.1/kola/klvm/
--rw-rw-rw-   0        0        0      561 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/klvm/__init__.py
--rw-rw-rw-   0        0        0     3057 2023-07-02 16:39:22.000000 KoiLang-1.1.1/kola/klvm/command.py
--rw-rw-rw-   0        0        0     5124 2023-07-02 16:53:02.000000 KoiLang-1.1.1/kola/klvm/commandset.py
--rw-rw-rw-   0        0        0     2419 2023-05-15 13:04:03.000000 KoiLang-1.1.1/kola/klvm/commandset.pyi
--rw-rw-rw-   0        0        0     2305 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/klvm/decorator.py
--rw-rw-rw-   0        0        0     2837 2023-04-20 10:43:55.000000 KoiLang-1.1.1/kola/klvm/decorator.pyi
--rw-rw-rw-   0        0        0     8316 2023-07-02 15:45:52.000000 KoiLang-1.1.1/kola/klvm/environment.py
--rw-rw-rw-   0        0        0     5894 2023-07-02 15:06:42.000000 KoiLang-1.1.1/kola/klvm/handler.py
--rw-rw-rw-   0        0        0    11575 2023-05-16 10:25:45.000000 KoiLang-1.1.1/kola/klvm/koilang.py
--rw-rw-rw-   0        0        0     2428 2023-07-02 14:57:58.000000 KoiLang-1.1.1/kola/klvm/mask.py
--rw-rw-rw-   0        0        0     3337 2023-05-15 09:19:47.000000 KoiLang-1.1.1/kola/klvm/writer.py
--rw-rw-rw-   0        0        0   680498 2023-04-06 12:20:02.000000 KoiLang-1.1.1/kola/lexer.c
--rw-rw-rw-   0        0        0     1087 2023-04-06 11:32:42.000000 KoiLang-1.1.1/kola/lexer.pxd
--rw-rw-rw-   0        0        0     3049 2023-04-06 12:02:51.000000 KoiLang-1.1.1/kola/lexer.pyi
-drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.534168 KoiLang-1.1.1/kola/lib/
--rw-rw-rw-   0        0        0     3697 2023-04-21 10:29:04.000000 KoiLang-1.1.1/kola/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.540167 KoiLang-1.1.1/kola/lib/debugger/
--rw-rw-rw-   0        0        0      327 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/lib/debugger/__init__.py
--rw-rw-rw-   0        0        0      900 2023-05-16 11:17:29.000000 KoiLang-1.1.1/kola/lib/debugger/base.py
--rw-rw-rw-   0        0        0      465 2023-04-13 10:44:00.000000 KoiLang-1.1.1/kola/lib/debugger/command_debugger.py
--rw-rw-rw-   0        0        0     6372 2023-05-16 11:39:57.000000 KoiLang-1.1.1/kola/lib/debugger/default_runner.py
--rw-rw-rw-   0        0        0    11900 2023-04-23 08:21:48.000000 KoiLang-1.1.1/kola/lib/disabled.jklvm.py
--rw-rw-rw-   0        0        0     3349 2023-07-02 16:37:30.000000 KoiLang-1.1.1/kola/lib/fastfiles.py
--rw-rw-rw-   0        0        0     1253 2023-05-05 14:41:55.000000 KoiLang-1.1.1/kola/lib/recorder.py
--rw-rw-rw-   0        0        0   577664 2023-04-06 11:40:03.000000 KoiLang-1.1.1/kola/parser.c
--rw-rw-rw-   0        0        0      586 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/parser.pxd
--rw-rw-rw-   0        0        0      845 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/parser.pyi
--rw-rw-rw-   0        0        0     3769 2023-03-28 17:09:26.000000 KoiLang-1.1.1/kola/unicode_handler.c
--rw-rw-rw-   0        0        0       46 2023-07-02 17:29:16.000000 KoiLang-1.1.1/kola/version.py
--rw-rw-rw-   0        0        0  1137811 2023-04-06 11:40:04.000000 KoiLang-1.1.1/kola/writer.c
--rw-rw-rw-   0        0        0     2374 2023-02-24 14:55:22.000000 KoiLang-1.1.1/kola/writer.pxd
--rw-rw-rw-   0        0        0     2185 2023-03-26 03:31:45.000000 KoiLang-1.1.1/kola/writer.pyi
--rw-rw-rw-   0        0        0       42 2023-07-02 17:29:31.557168 KoiLang-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3131 2023-07-02 14:56:00.000000 KoiLang-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 17:29:31.554169 KoiLang-1.1.1/tests/
--rw-rw-rw-   0        0        0     5834 2023-05-15 17:49:36.000000 KoiLang-1.1.1/tests/test_kola.py
--rw-rw-rw-   0        0        0     3685 2023-04-12 07:40:39.000000 KoiLang-1.1.1/tests/test_lexer.py
--rw-rw-rw-   0        0        0     2709 2023-04-20 12:41:53.000000 KoiLang-1.1.1/tests/test_parser.py
--rw-rw-rw-   0        0        0     3668 2023-04-20 09:10:18.000000 KoiLang-1.1.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:54:23.046117 KoiLang-1.2.0a0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:54:23.034117 KoiLang-1.2.0a0/KoiLang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-11 14:54:22.000000 KoiLang-1.2.0a0/KoiLang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-11 14:54:22.000000 KoiLang-1.2.0a0/KoiLang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:54:22.000000 KoiLang-1.2.0a0/KoiLang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 14:54:22.000000 KoiLang-1.2.0a0/KoiLang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 14:54:22.000000 KoiLang-1.2.0a0/KoiLang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-11 14:54:23.046117 KoiLang-1.2.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:54:23.042117 KoiLang-1.2.0a0/kola/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/_cutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/_cutil.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/_yylex.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:54:23.042117 KoiLang-1.2.0a0/kola/klvm/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/commandset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/commandset.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/koilang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/klvm/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   680498 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lexer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lexer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lexer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:54:23.042117 KoiLang-1.2.0a0/kola/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:54:23.046117 KoiLang-1.2.0a0/kola/lib/debugger/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lib/debugger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lib/debugger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lib/debugger/command_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lib/debugger/default_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lib/envutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lib/fastfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/lib/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)   577664 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/parser.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/unicode_handler.c
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1137811 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/writer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/writer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/kola/writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:54:23.046117 KoiLang-1.2.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-11 14:54:10.000000 KoiLang-1.2.0a0/setup.py
```

### Comparing `KoiLang-1.1.1/KoiLang.egg-info/PKG-INFO` & `KoiLang-1.2.0a0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,342 +1,315 @@
-Metadata-Version: 2.1
-Name: KoiLang
-Version: 1.1.1
-Summary: simple python module for KoiLang parsing
-Home-page: https://github.com/Ovizro/Kola
-Author: Visecy
-Author-email: Visecy@visecy.top
-Maintainer: Ovizro
-Maintainer-email: Ovizro@visecy.top
-License: Apache 2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: Markup
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Kola
-Simple python module for KoiLang parsing.
-
-[![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
-![PyPI - Downloads](https://img.shields.io/pypi/dw/KoiLang)
-![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
-
-## Installation
-From pip:
-
-    pip install KoiLang
-
-From source code:
-    
-    python setup.py build_ext --inplace
-    python setup.py install
-
-## What is KoiLang
-
-KoiLang is a markup language while is easy to read for people.
-There is an simple example.
-```
-#background Street
-    #camera on(Orga)
-    #character Orga
-        Huh... I'm a pretty good shot, huh?
-    #camera on(Ride, Ched)
-    #character Ride
-        B- boss...
-    #character Orga
-        #action bleed
-    #camera on(object: blood, source: Orga)
-
-    #camera on(Ched, Orga, Ride)
-    #character Orga
-        How come you're stammering like that... Ride!
-
-    #playsound freesia
-
-    #character Orga
-        #action stand_up speed(slowly)
-
-    #character Ride
-        But... but!
-    #character Orga
-        I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
-    #character Ride
-        #action shed_tear
-        No... not for me...
-
-    #camera on(Orga)
-    #character Orga
-        Protecting my members is my job!
-    #character Ched
-        #action shed_tear
-
-    #character Ride
-        But...!
-    #character Orga
-        Shut up and let's go!
-
-        #camera on(Orga)
-        #action walk direction(front) speed(slowly)
-        Everyone's waiting, besides...
-
-        I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
-        As long as we don't stop, the road will continue!
-```
-
-### Grammar
-
-In KoiLang, the code contains 'command' section and 'text' section.
-The format of the command section is similar to a C prepared statement,
-using '#' as the prefix. And other lines that do not start with '#' are the text section.
-
-    #command "This is a command"
-    This is the text.
-
-The format of a single command like:
-
-    #command_name [param 1] [param 2] ...
-
-There are several parameters behind the command whose name should be a valid variable name.
-
-> An unsigned decimal integer like is also a legal command name, like `#114`.
-
-Each command can have several parameters behind the command name.
-Valid argument type include integer, float, literal and string.
-    
-    #arg_int    1 0b101 0x6CF
-    #arg_float  1. 2e-2 .114514
-    #arg_literal string __name__
-    #arg_string "A string"
-
-> Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
- 
-The above parameter types are often referred to base parameters.
-Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
-The format is as follows:
-
-    #kwargs key(value)
-    
-    And another format:
-    #keyargs_list key(item0, item1)
-    
-    And the third:
-    #kwargs_dict key(x: 11, y: 45, z: 14)
-
-All the parameters above can be put together:
-    
-    #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
-        thickness(2) color(255, 255, 255)
-
-## What can Kola module do
-
-Kola module provides a fast way to translate KoiLang command into a python function call.
-
-Above command `#draw` will convert to function call below:
-
-```py
-draw(
-    "Line", 2,
-    pos0={"x": 0, "y": 0},
-    pos1={"x": 16, "y": 16},
-    thickness=2,
-    color=[255, 255, 255]
-)
-```
-
-Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
-
-### Example
-
-Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
-
-Let us start with a kola file:
-
-```
-## This is the file `makefiles.kola`
-
-#file "hello.txt" encoding("utf-8")
-Hello world!
-And there are all my friends.
-
-#space hello
-
-    #file "Bob.txt"
-    Hello Bob.
-
-    #file "Alice.txt"
-    Hello Alice.
-
-#endspace
-```
-
-Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
-
-```py
-import os
-from kola import KoiLang, kola_command, kola_text
-
-
-class FastFile(KoiLang):
-    @kola_command
-    def file(self, path: str, encoding: str = "utf-8") -> None:
-        if self._file:
-            self._file.close()
-        path_dir = os.path.dirname(path)
-        if path_dir:
-            os.makedirs(path_dir, exist_ok=True)
-        self._file = open(path, "w", encoding=encoding)
-    
-    @kola_command
-    def space(self, name: str) -> None:
-        path = name.replace('.', '/')
-        if not os.path.isdir(path):
-            os.makedirs(path)
-        os.chdir(path)
-    
-    @kola_command
-    def endspace(self) -> None:
-        os.chdir("..")
-        self.end()
-
-    @kola_command
-    def end(self) -> None:
-        if self._file:
-            self._file.close()
-            self._file = None
-    
-    @kola_text
-    def text(self, text: str) -> None:
-        if not self._file:
-            raise OSError("write texts before the file open")
-        self._file.write(text)
-    
-    def at_start(self) -> None:
-        self._file = None
-    
-    def at_end(self) -> None:
-        self.end()
-```
-
-You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
-
-```sh
-python -m kola makefiles.kola -s script.py
-```
-
-Or add these directly at the end of the script:
-```py
-if __name__ = "__main__":
-    FastFile().parse_file("makefiles.kola")
-```
-
-You will see new files in your work dir.
-
-    <workdir>
-    │      
-    │  hello.txt
-    │      
-    └─hello
-        Alice.txt
-        Bob.txt
-
-### What happened
-
-It seems amusing? Well, if you make a python script as this:
-
-```py
-vmobj = FastFile()
-
-with vmobj.exec_block():
-    vmobj.file("hello.txt", encoding="utf-8")
-    vmobj.text("Hello world!")
-    vmobj.text("And there are all my friends.")
-
-    vmobj.space("hello")
-
-    vmobj.file("Bob.txt")
-    vmobj.text("Hello Bob.")
-
-    vmobj.file("Alice.txt")
-    vmobj.text("Hello Alice.")
-
-    vmobj.endspace()
-```
-the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
-
-So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
-```py
-class FastFile(KoiLang):
-    ...
-```
-The next step is making the kola command we need. So a function is defined here:
-```py
-def file(self, path: str, encoding: str = "utf-8") -> None:
-    if self._file:
-        self._file.close()
-    path_dir = os.path.dirname(path)
-    if path_dir:
-        os.makedirs(path_dir, exist_ok=True)
-    self._file = open(path, "w", encoding=encoding)
-```
-But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
-```py
-@kola_command("open")
-def file(self, path: str, encoding: str = "utf-8") -> None:
-    if self._file:
-        self._file.close()
-    path_dir = os.path.dirname(path)
-    if path_dir:
-        os.makedirs(path_dir, exist_ok=True)
-    self._file = open(path, "w", encoding=encoding)
-```
-Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
-
-You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
-
-### File parse
-`KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
-
-### Advanced techniques
-In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
-
-```py
-class FastFile(KoiLang):
-    ...
-
-    class space(Environment):
-        @kola_env_enter("space")
-        def enter(self, name: str) -> None:
-            self.pwd = os.getcwd()
-            path = name.replace('.', '/')
-            if not os.path.isdir(path):
-                os.makedirs(path)
-            os.chdir(path)
-        
-        @kola_env_exit("endspace")
-        def exit(self) -> None:
-            os.chdir(self.pwd)
-```
-
-> There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
-
-## What is more
-
-The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
-
-On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
-
-## Bugs/Requests
-
-Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
+# Kola
+Simple python module for KoiLang parsing.
+
+[![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/KoiLang)
+![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
+
+## Installation
+From pip:
+
+    pip install KoiLang
+
+From source code:
+    
+    python setup.py build_ext --inplace
+    python setup.py install
+
+## What is KoiLang
+
+KoiLang is a markup language while is easy to read for people.
+There is an simple example.
+```
+#background Street
+    #camera on(Orga)
+    #character Orga
+        Huh... I'm a pretty good shot, huh?
+    #camera on(Ride, Ched)
+    #character Ride
+        B- boss...
+    #character Orga
+        #action bleed
+    #camera on(object: blood, source: Orga)
+
+    #camera on(Ched, Orga, Ride)
+    #character Orga
+        How come you're stammering like that... Ride!
+
+    #playsound freesia
+
+    #character Orga
+        #action stand_up speed(slowly)
+
+    #character Ride
+        But... but!
+    #character Orga
+        I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
+    #character Ride
+        #action shed_tear
+        No... not for me...
+
+    #camera on(Orga)
+    #character Orga
+        Protecting my members is my job!
+    #character Ched
+        #action shed_tear
+
+    #character Ride
+        But...!
+    #character Orga
+        Shut up and let's go!
+
+        #camera on(Orga)
+        #action walk direction(front) speed(slowly)
+        Everyone's waiting, besides...
+
+        I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
+        As long as we don't stop, the road will continue!
+```
+
+### Grammar
+
+In KoiLang, the code contains 'command' section and 'text' section.
+The format of the command section is similar to a C prepared statement,
+using '#' as the prefix. And other lines that do not start with '#' are the text section.
+
+    #command "This is a command"
+    This is the text.
+
+The format of a single command like:
+
+    #command_name [param 1] [param 2] ...
+
+There are several parameters behind the command whose name should be a valid variable name.
+
+> An unsigned decimal integer like is also a legal command name, like `#114`.
+
+Each command can have several parameters behind the command name.
+Valid argument type include integer, float, literal and string.
+    
+    #arg_int    1 0b101 0x6CF
+    #arg_float  1. 2e-2 .114514
+    #arg_literal string __name__
+    #arg_string "A string"
+
+> Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
+ 
+The above parameter types are often referred to base parameters.
+Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
+The format is as follows:
+
+    #kwargs key(value)
+    
+    And another format:
+    #keyargs_list key(item0, item1)
+    
+    And the third:
+    #kwargs_dict key(x: 11, y: 45, z: 14)
+
+All the parameters above can be put together:
+    
+    #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
+        thickness(2) color(255, 255, 255)
+
+## What can Kola module do
+
+Kola module provides a fast way to translate KoiLang command into a python function call.
+
+Above command `#draw` will convert to function call below:
+
+```py
+draw(
+    "Line", 2,
+    pos0={"x": 0, "y": 0},
+    pos1={"x": 16, "y": 16},
+    thickness=2,
+    color=[255, 255, 255]
+)
+```
+
+Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
+
+### Example
+
+Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
+
+Let us start with a kola file:
+
+```
+## This is the file `makefiles.kola`
+
+#file "hello.txt" encoding("utf-8")
+Hello world!
+And there are all my friends.
+
+#space hello
+
+    #file "Bob.txt"
+    Hello Bob.
+
+    #file "Alice.txt"
+    Hello Alice.
+
+#endspace
+```
+
+Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
+
+```py
+import os
+from kola import KoiLang, kola_command, kola_text
+
+
+class FastFile(KoiLang):
+    @kola_command
+    def file(self, path: str, encoding: str = "utf-8") -> None:
+        if self._file:
+            self._file.close()
+        path_dir = os.path.dirname(path)
+        if path_dir:
+            os.makedirs(path_dir, exist_ok=True)
+        self._file = open(path, "w", encoding=encoding)
+    
+    @kola_command
+    def space(self, name: str) -> None:
+        path = name.replace('.', '/')
+        if not os.path.isdir(path):
+            os.makedirs(path)
+        os.chdir(path)
+    
+    @kola_command
+    def endspace(self) -> None:
+        os.chdir("..")
+        self.end()
+
+    @kola_command
+    def end(self) -> None:
+        if self._file:
+            self._file.close()
+            self._file = None
+    
+    @kola_text
+    def text(self, text: str) -> None:
+        if not self._file:
+            raise OSError("write texts before the file open")
+        self._file.write(text)
+    
+    def at_start(self) -> None:
+        self._file = None
+    
+    def at_end(self) -> None:
+        self.end()
+```
+
+You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
+
+```sh
+python -m kola makefiles.kola -s script.py
+```
+
+Or add these directly at the end of the script:
+```py
+if __name__ = "__main__":
+    FastFile().parse_file("makefiles.kola")
+```
+
+You will see new files in your work dir.
+
+    <workdir>
+    │      
+    │  hello.txt
+    │      
+    └─hello
+        Alice.txt
+        Bob.txt
+
+### What happened
+
+It seems amusing? Well, if you make a python script as this:
+
+```py
+vmobj = FastFile()
+
+with vmobj.exec_block():
+    vmobj.file("hello.txt", encoding="utf-8")
+    vmobj.text("Hello world!")
+    vmobj.text("And there are all my friends.")
+
+    vmobj.space("hello")
+
+    vmobj.file("Bob.txt")
+    vmobj.text("Hello Bob.")
+
+    vmobj.file("Alice.txt")
+    vmobj.text("Hello Alice.")
+
+    vmobj.endspace()
+```
+the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
+
+So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
+```py
+class FastFile(KoiLang):
+    ...
+```
+The next step is making the kola command we need. So a function is defined here:
+```py
+def file(self, path: str, encoding: str = "utf-8") -> None:
+    if self._file:
+        self._file.close()
+    path_dir = os.path.dirname(path)
+    if path_dir:
+        os.makedirs(path_dir, exist_ok=True)
+    self._file = open(path, "w", encoding=encoding)
+```
+But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
+```py
+@kola_command("open")
+def file(self, path: str, encoding: str = "utf-8") -> None:
+    if self._file:
+        self._file.close()
+    path_dir = os.path.dirname(path)
+    if path_dir:
+        os.makedirs(path_dir, exist_ok=True)
+    self._file = open(path, "w", encoding=encoding)
+```
+Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
+
+You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
+
+### File parse
+`KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
+
+### Advanced techniques
+In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
+
+```py
+class FastFile(KoiLang):
+    ...
+
+    class space(Environment):
+        @kola_env_enter("space")
+        def enter(self, name: str) -> None:
+            self.pwd = os.getcwd()
+            path = name.replace('.', '/')
+            if not os.path.isdir(path):
+                os.makedirs(path)
+            os.chdir(path)
+        
+        @kola_env_exit("endspace")
+        def exit(self) -> None:
+            os.chdir(self.pwd)
+```
+
+> There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
+
+## What is more
+
+The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
+
+On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
+
+## Bugs/Requests
+
+Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
```

### Comparing `KoiLang-1.1.1/KoiLang.egg-info/SOURCES.txt` & `KoiLang-1.2.0a0/KoiLang.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -31,37 +31,14 @@
 kola/klvm/decorator.pyi
 kola/klvm/environment.py
 kola/klvm/handler.py
 kola/klvm/koilang.py
 kola/klvm/mask.py
 kola/klvm/writer.py
 kola/lib/__init__.py
-kola/lib/disabled.jklvm.py
+kola/lib/envutils.py
 kola/lib/fastfiles.py
 kola/lib/recorder.py
 kola/lib/debugger/__init__.py
 kola/lib/debugger/base.py
 kola/lib/debugger/command_debugger.py
-kola/lib/debugger/default_runner.py
-kola/klvm/__init__.py
-kola/klvm/command.py
-kola/klvm/commandset.py
-kola/klvm/commandset.pyi
-kola/klvm/decorator.py
-kola/klvm/decorator.pyi
-kola/klvm/environment.py
-kola/klvm/handler.py
-kola/klvm/koilang.py
-kola/klvm/mask.py
-kola/klvm/writer.py
-kola/lib/__init__.py
-kola/lib/disabled.jklvm.py
-kola/lib/fastfiles.py
-kola/lib/recorder.py
-kola/lib/debugger/__init__.py
-kola/lib/debugger/base.py
-kola/lib/debugger/command_debugger.py
-kola/lib/debugger/default_runner.py
-tests/test_kola.py
-tests/test_lexer.py
-tests/test_parser.py
-tests/test_writer.py
+kola/lib/debugger/default_runner.py
```

### Comparing `KoiLang-1.1.1/LICENSE` & `KoiLang-1.2.0a0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `KoiLang-1.1.1/PKG-INFO` & `KoiLang-1.2.0a0/KoiLang.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,342 +1,341 @@
-Metadata-Version: 2.1
-Name: KoiLang
-Version: 1.1.1
-Summary: simple python module for KoiLang parsing
-Home-page: https://github.com/Ovizro/Kola
-Author: Visecy
-Author-email: Visecy@visecy.top
-Maintainer: Ovizro
-Maintainer-email: Ovizro@visecy.top
-License: Apache 2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: Markup
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Kola
-Simple python module for KoiLang parsing.
-
-[![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
-![PyPI - Downloads](https://img.shields.io/pypi/dw/KoiLang)
-![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
-
-## Installation
-From pip:
-
-    pip install KoiLang
-
-From source code:
-    
-    python setup.py build_ext --inplace
-    python setup.py install
-
-## What is KoiLang
-
-KoiLang is a markup language while is easy to read for people.
-There is an simple example.
-```
-#background Street
-    #camera on(Orga)
-    #character Orga
-        Huh... I'm a pretty good shot, huh?
-    #camera on(Ride, Ched)
-    #character Ride
-        B- boss...
-    #character Orga
-        #action bleed
-    #camera on(object: blood, source: Orga)
-
-    #camera on(Ched, Orga, Ride)
-    #character Orga
-        How come you're stammering like that... Ride!
-
-    #playsound freesia
-
-    #character Orga
-        #action stand_up speed(slowly)
-
-    #character Ride
-        But... but!
-    #character Orga
-        I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
-    #character Ride
-        #action shed_tear
-        No... not for me...
-
-    #camera on(Orga)
-    #character Orga
-        Protecting my members is my job!
-    #character Ched
-        #action shed_tear
-
-    #character Ride
-        But...!
-    #character Orga
-        Shut up and let's go!
-
-        #camera on(Orga)
-        #action walk direction(front) speed(slowly)
-        Everyone's waiting, besides...
-
-        I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
-        As long as we don't stop, the road will continue!
-```
-
-### Grammar
-
-In KoiLang, the code contains 'command' section and 'text' section.
-The format of the command section is similar to a C prepared statement,
-using '#' as the prefix. And other lines that do not start with '#' are the text section.
-
-    #command "This is a command"
-    This is the text.
-
-The format of a single command like:
-
-    #command_name [param 1] [param 2] ...
-
-There are several parameters behind the command whose name should be a valid variable name.
-
-> An unsigned decimal integer like is also a legal command name, like `#114`.
-
-Each command can have several parameters behind the command name.
-Valid argument type include integer, float, literal and string.
-    
-    #arg_int    1 0b101 0x6CF
-    #arg_float  1. 2e-2 .114514
-    #arg_literal string __name__
-    #arg_string "A string"
-
-> Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
- 
-The above parameter types are often referred to base parameters.
-Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
-The format is as follows:
-
-    #kwargs key(value)
-    
-    And another format:
-    #keyargs_list key(item0, item1)
-    
-    And the third:
-    #kwargs_dict key(x: 11, y: 45, z: 14)
-
-All the parameters above can be put together:
-    
-    #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
-        thickness(2) color(255, 255, 255)
-
-## What can Kola module do
-
-Kola module provides a fast way to translate KoiLang command into a python function call.
-
-Above command `#draw` will convert to function call below:
-
-```py
-draw(
-    "Line", 2,
-    pos0={"x": 0, "y": 0},
-    pos1={"x": 16, "y": 16},
-    thickness=2,
-    color=[255, 255, 255]
-)
-```
-
-Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
-
-### Example
-
-Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
-
-Let us start with a kola file:
-
-```
-## This is the file `makefiles.kola`
-
-#file "hello.txt" encoding("utf-8")
-Hello world!
-And there are all my friends.
-
-#space hello
-
-    #file "Bob.txt"
-    Hello Bob.
-
-    #file "Alice.txt"
-    Hello Alice.
-
-#endspace
-```
-
-Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
-
-```py
-import os
-from kola import KoiLang, kola_command, kola_text
-
-
-class FastFile(KoiLang):
-    @kola_command
-    def file(self, path: str, encoding: str = "utf-8") -> None:
-        if self._file:
-            self._file.close()
-        path_dir = os.path.dirname(path)
-        if path_dir:
-            os.makedirs(path_dir, exist_ok=True)
-        self._file = open(path, "w", encoding=encoding)
-    
-    @kola_command
-    def space(self, name: str) -> None:
-        path = name.replace('.', '/')
-        if not os.path.isdir(path):
-            os.makedirs(path)
-        os.chdir(path)
-    
-    @kola_command
-    def endspace(self) -> None:
-        os.chdir("..")
-        self.end()
-
-    @kola_command
-    def end(self) -> None:
-        if self._file:
-            self._file.close()
-            self._file = None
-    
-    @kola_text
-    def text(self, text: str) -> None:
-        if not self._file:
-            raise OSError("write texts before the file open")
-        self._file.write(text)
-    
-    def at_start(self) -> None:
-        self._file = None
-    
-    def at_end(self) -> None:
-        self.end()
-```
-
-You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
-
-```sh
-python -m kola makefiles.kola -s script.py
-```
-
-Or add these directly at the end of the script:
-```py
-if __name__ = "__main__":
-    FastFile().parse_file("makefiles.kola")
-```
-
-You will see new files in your work dir.
-
-    <workdir>
-    │      
-    │  hello.txt
-    │      
-    └─hello
-        Alice.txt
-        Bob.txt
-
-### What happened
-
-It seems amusing? Well, if you make a python script as this:
-
-```py
-vmobj = FastFile()
-
-with vmobj.exec_block():
-    vmobj.file("hello.txt", encoding="utf-8")
-    vmobj.text("Hello world!")
-    vmobj.text("And there are all my friends.")
-
-    vmobj.space("hello")
-
-    vmobj.file("Bob.txt")
-    vmobj.text("Hello Bob.")
-
-    vmobj.file("Alice.txt")
-    vmobj.text("Hello Alice.")
-
-    vmobj.endspace()
-```
-the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
-
-So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
-```py
-class FastFile(KoiLang):
-    ...
-```
-The next step is making the kola command we need. So a function is defined here:
-```py
-def file(self, path: str, encoding: str = "utf-8") -> None:
-    if self._file:
-        self._file.close()
-    path_dir = os.path.dirname(path)
-    if path_dir:
-        os.makedirs(path_dir, exist_ok=True)
-    self._file = open(path, "w", encoding=encoding)
-```
-But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
-```py
-@kola_command("open")
-def file(self, path: str, encoding: str = "utf-8") -> None:
-    if self._file:
-        self._file.close()
-    path_dir = os.path.dirname(path)
-    if path_dir:
-        os.makedirs(path_dir, exist_ok=True)
-    self._file = open(path, "w", encoding=encoding)
-```
-Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
-
-You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
-
-### File parse
-`KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
-
-### Advanced techniques
-In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
-
-```py
-class FastFile(KoiLang):
-    ...
-
-    class space(Environment):
-        @kola_env_enter("space")
-        def enter(self, name: str) -> None:
-            self.pwd = os.getcwd()
-            path = name.replace('.', '/')
-            if not os.path.isdir(path):
-                os.makedirs(path)
-            os.chdir(path)
-        
-        @kola_env_exit("endspace")
-        def exit(self) -> None:
-            os.chdir(self.pwd)
-```
-
-> There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
-
-## What is more
-
-The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
-
-On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
-
-## Bugs/Requests
-
-Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
+Metadata-Version: 2.1
+Name: KoiLang
+Version: 1.2.0a0
+Summary: simple python module for KoiLang parsing
+Home-page: https://github.com/Ovizro/Kola
+Author: Visecy
+Author-email: Visecy@visecy.top
+Maintainer: Ovizro
+Maintainer-email: Ovizro@visecy.top
+License: Apache 2.0
+Description: # Kola
+        Simple python module for KoiLang parsing.
+        
+        [![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
+        [![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
+        ![PyPI - Downloads](https://img.shields.io/pypi/dw/KoiLang)
+        ![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
+        
+        ## Installation
+        From pip:
+        
+            pip install KoiLang
+        
+        From source code:
+            
+            python setup.py build_ext --inplace
+            python setup.py install
+        
+        ## What is KoiLang
+        
+        KoiLang is a markup language while is easy to read for people.
+        There is an simple example.
+        ```
+        #background Street
+            #camera on(Orga)
+            #character Orga
+                Huh... I'm a pretty good shot, huh?
+            #camera on(Ride, Ched)
+            #character Ride
+                B- boss...
+            #character Orga
+                #action bleed
+            #camera on(object: blood, source: Orga)
+        
+            #camera on(Ched, Orga, Ride)
+            #character Orga
+                How come you're stammering like that... Ride!
+        
+            #playsound freesia
+        
+            #character Orga
+                #action stand_up speed(slowly)
+        
+            #character Ride
+                But... but!
+            #character Orga
+                I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
+            #character Ride
+                #action shed_tear
+                No... not for me...
+        
+            #camera on(Orga)
+            #character Orga
+                Protecting my members is my job!
+            #character Ched
+                #action shed_tear
+        
+            #character Ride
+                But...!
+            #character Orga
+                Shut up and let's go!
+        
+                #camera on(Orga)
+                #action walk direction(front) speed(slowly)
+                Everyone's waiting, besides...
+        
+                I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
+                As long as we don't stop, the road will continue!
+        ```
+        
+        ### Grammar
+        
+        In KoiLang, the code contains 'command' section and 'text' section.
+        The format of the command section is similar to a C prepared statement,
+        using '#' as the prefix. And other lines that do not start with '#' are the text section.
+        
+            #command "This is a command"
+            This is the text.
+        
+        The format of a single command like:
+        
+            #command_name [param 1] [param 2] ...
+        
+        There are several parameters behind the command whose name should be a valid variable name.
+        
+        > An unsigned decimal integer like is also a legal command name, like `#114`.
+        
+        Each command can have several parameters behind the command name.
+        Valid argument type include integer, float, literal and string.
+            
+            #arg_int    1 0b101 0x6CF
+            #arg_float  1. 2e-2 .114514
+            #arg_literal string __name__
+            #arg_string "A string"
+        
+        > Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
+         
+        The above parameter types are often referred to base parameters.
+        Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
+        The format is as follows:
+        
+            #kwargs key(value)
+            
+            And another format:
+            #keyargs_list key(item0, item1)
+            
+            And the third:
+            #kwargs_dict key(x: 11, y: 45, z: 14)
+        
+        All the parameters above can be put together:
+            
+            #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
+                thickness(2) color(255, 255, 255)
+        
+        ## What can Kola module do
+        
+        Kola module provides a fast way to translate KoiLang command into a python function call.
+        
+        Above command `#draw` will convert to function call below:
+        
+        ```py
+        draw(
+            "Line", 2,
+            pos0={"x": 0, "y": 0},
+            pos1={"x": 16, "y": 16},
+            thickness=2,
+            color=[255, 255, 255]
+        )
+        ```
+        
+        Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
+        
+        ### Example
+        
+        Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
+        
+        Let us start with a kola file:
+        
+        ```
+        ## This is the file `makefiles.kola`
+        
+        #file "hello.txt" encoding("utf-8")
+        Hello world!
+        And there are all my friends.
+        
+        #space hello
+        
+            #file "Bob.txt"
+            Hello Bob.
+        
+            #file "Alice.txt"
+            Hello Alice.
+        
+        #endspace
+        ```
+        
+        Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
+        
+        ```py
+        import os
+        from kola import KoiLang, kola_command, kola_text
+        
+        
+        class FastFile(KoiLang):
+            @kola_command
+            def file(self, path: str, encoding: str = "utf-8") -> None:
+                if self._file:
+                    self._file.close()
+                path_dir = os.path.dirname(path)
+                if path_dir:
+                    os.makedirs(path_dir, exist_ok=True)
+                self._file = open(path, "w", encoding=encoding)
+            
+            @kola_command
+            def space(self, name: str) -> None:
+                path = name.replace('.', '/')
+                if not os.path.isdir(path):
+                    os.makedirs(path)
+                os.chdir(path)
+            
+            @kola_command
+            def endspace(self) -> None:
+                os.chdir("..")
+                self.end()
+        
+            @kola_command
+            def end(self) -> None:
+                if self._file:
+                    self._file.close()
+                    self._file = None
+            
+            @kola_text
+            def text(self, text: str) -> None:
+                if not self._file:
+                    raise OSError("write texts before the file open")
+                self._file.write(text)
+            
+            def at_start(self) -> None:
+                self._file = None
+            
+            def at_end(self) -> None:
+                self.end()
+        ```
+        
+        You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
+        
+        ```sh
+        python -m kola makefiles.kola -s script.py
+        ```
+        
+        Or add these directly at the end of the script:
+        ```py
+        if __name__ = "__main__":
+            FastFile().parse_file("makefiles.kola")
+        ```
+        
+        You will see new files in your work dir.
+        
+            <workdir>
+            │      
+            │  hello.txt
+            │      
+            └─hello
+                Alice.txt
+                Bob.txt
+        
+        ### What happened
+        
+        It seems amusing? Well, if you make a python script as this:
+        
+        ```py
+        vmobj = FastFile()
+        
+        with vmobj.exec_block():
+            vmobj.file("hello.txt", encoding="utf-8")
+            vmobj.text("Hello world!")
+            vmobj.text("And there are all my friends.")
+        
+            vmobj.space("hello")
+        
+            vmobj.file("Bob.txt")
+            vmobj.text("Hello Bob.")
+        
+            vmobj.file("Alice.txt")
+            vmobj.text("Hello Alice.")
+        
+            vmobj.endspace()
+        ```
+        the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
+        
+        So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
+        ```py
+        class FastFile(KoiLang):
+            ...
+        ```
+        The next step is making the kola command we need. So a function is defined here:
+        ```py
+        def file(self, path: str, encoding: str = "utf-8") -> None:
+            if self._file:
+                self._file.close()
+            path_dir = os.path.dirname(path)
+            if path_dir:
+                os.makedirs(path_dir, exist_ok=True)
+            self._file = open(path, "w", encoding=encoding)
+        ```
+        But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
+        ```py
+        @kola_command("open")
+        def file(self, path: str, encoding: str = "utf-8") -> None:
+            if self._file:
+                self._file.close()
+            path_dir = os.path.dirname(path)
+            if path_dir:
+                os.makedirs(path_dir, exist_ok=True)
+            self._file = open(path, "w", encoding=encoding)
+        ```
+        Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
+        
+        You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
+        
+        ### File parse
+        `KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
+        
+        ### Advanced techniques
+        In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
+        
+        ```py
+        class FastFile(KoiLang):
+            ...
+        
+            class space(Environment):
+                @kola_env_enter("space")
+                def enter(self, name: str) -> None:
+                    self.pwd = os.getcwd()
+                    path = name.replace('.', '/')
+                    if not os.path.isdir(path):
+                        os.makedirs(path)
+                    os.chdir(path)
+                
+                @kola_env_exit("endspace")
+                def exit(self) -> None:
+                    os.chdir(self.pwd)
+        ```
+        
+        > There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
+        
+        ## What is more
+        
+        The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
+        
+        On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
+        
+        ## Bugs/Requests
+        
+        Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Markup
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `KoiLang-1.1.1/README.md` & `KoiLang-1.2.0a0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,315 +1,341 @@
-# Kola
-Simple python module for KoiLang parsing.
-
-[![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
-![PyPI - Downloads](https://img.shields.io/pypi/dw/KoiLang)
-![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
-
-## Installation
-From pip:
-
-    pip install KoiLang
-
-From source code:
-    
-    python setup.py build_ext --inplace
-    python setup.py install
-
-## What is KoiLang
-
-KoiLang is a markup language while is easy to read for people.
-There is an simple example.
-```
-#background Street
-    #camera on(Orga)
-    #character Orga
-        Huh... I'm a pretty good shot, huh?
-    #camera on(Ride, Ched)
-    #character Ride
-        B- boss...
-    #character Orga
-        #action bleed
-    #camera on(object: blood, source: Orga)
-
-    #camera on(Ched, Orga, Ride)
-    #character Orga
-        How come you're stammering like that... Ride!
-
-    #playsound freesia
-
-    #character Orga
-        #action stand_up speed(slowly)
-
-    #character Ride
-        But... but!
-    #character Orga
-        I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
-    #character Ride
-        #action shed_tear
-        No... not for me...
-
-    #camera on(Orga)
-    #character Orga
-        Protecting my members is my job!
-    #character Ched
-        #action shed_tear
-
-    #character Ride
-        But...!
-    #character Orga
-        Shut up and let's go!
-
-        #camera on(Orga)
-        #action walk direction(front) speed(slowly)
-        Everyone's waiting, besides...
-
-        I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
-        As long as we don't stop, the road will continue!
-```
-
-### Grammar
-
-In KoiLang, the code contains 'command' section and 'text' section.
-The format of the command section is similar to a C prepared statement,
-using '#' as the prefix. And other lines that do not start with '#' are the text section.
-
-    #command "This is a command"
-    This is the text.
-
-The format of a single command like:
-
-    #command_name [param 1] [param 2] ...
-
-There are several parameters behind the command whose name should be a valid variable name.
-
-> An unsigned decimal integer like is also a legal command name, like `#114`.
-
-Each command can have several parameters behind the command name.
-Valid argument type include integer, float, literal and string.
-    
-    #arg_int    1 0b101 0x6CF
-    #arg_float  1. 2e-2 .114514
-    #arg_literal string __name__
-    #arg_string "A string"
-
-> Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
- 
-The above parameter types are often referred to base parameters.
-Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
-The format is as follows:
-
-    #kwargs key(value)
-    
-    And another format:
-    #keyargs_list key(item0, item1)
-    
-    And the third:
-    #kwargs_dict key(x: 11, y: 45, z: 14)
-
-All the parameters above can be put together:
-    
-    #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
-        thickness(2) color(255, 255, 255)
-
-## What can Kola module do
-
-Kola module provides a fast way to translate KoiLang command into a python function call.
-
-Above command `#draw` will convert to function call below:
-
-```py
-draw(
-    "Line", 2,
-    pos0={"x": 0, "y": 0},
-    pos1={"x": 16, "y": 16},
-    thickness=2,
-    color=[255, 255, 255]
-)
-```
-
-Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
-
-### Example
-
-Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
-
-Let us start with a kola file:
-
-```
-## This is the file `makefiles.kola`
-
-#file "hello.txt" encoding("utf-8")
-Hello world!
-And there are all my friends.
-
-#space hello
-
-    #file "Bob.txt"
-    Hello Bob.
-
-    #file "Alice.txt"
-    Hello Alice.
-
-#endspace
-```
-
-Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
-
-```py
-import os
-from kola import KoiLang, kola_command, kola_text
-
-
-class FastFile(KoiLang):
-    @kola_command
-    def file(self, path: str, encoding: str = "utf-8") -> None:
-        if self._file:
-            self._file.close()
-        path_dir = os.path.dirname(path)
-        if path_dir:
-            os.makedirs(path_dir, exist_ok=True)
-        self._file = open(path, "w", encoding=encoding)
-    
-    @kola_command
-    def space(self, name: str) -> None:
-        path = name.replace('.', '/')
-        if not os.path.isdir(path):
-            os.makedirs(path)
-        os.chdir(path)
-    
-    @kola_command
-    def endspace(self) -> None:
-        os.chdir("..")
-        self.end()
-
-    @kola_command
-    def end(self) -> None:
-        if self._file:
-            self._file.close()
-            self._file = None
-    
-    @kola_text
-    def text(self, text: str) -> None:
-        if not self._file:
-            raise OSError("write texts before the file open")
-        self._file.write(text)
-    
-    def at_start(self) -> None:
-        self._file = None
-    
-    def at_end(self) -> None:
-        self.end()
-```
-
-You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
-
-```sh
-python -m kola makefiles.kola -s script.py
-```
-
-Or add these directly at the end of the script:
-```py
-if __name__ = "__main__":
-    FastFile().parse_file("makefiles.kola")
-```
-
-You will see new files in your work dir.
-
-    <workdir>
-    │      
-    │  hello.txt
-    │      
-    └─hello
-        Alice.txt
-        Bob.txt
-
-### What happened
-
-It seems amusing? Well, if you make a python script as this:
-
-```py
-vmobj = FastFile()
-
-with vmobj.exec_block():
-    vmobj.file("hello.txt", encoding="utf-8")
-    vmobj.text("Hello world!")
-    vmobj.text("And there are all my friends.")
-
-    vmobj.space("hello")
-
-    vmobj.file("Bob.txt")
-    vmobj.text("Hello Bob.")
-
-    vmobj.file("Alice.txt")
-    vmobj.text("Hello Alice.")
-
-    vmobj.endspace()
-```
-the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
-
-So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
-```py
-class FastFile(KoiLang):
-    ...
-```
-The next step is making the kola command we need. So a function is defined here:
-```py
-def file(self, path: str, encoding: str = "utf-8") -> None:
-    if self._file:
-        self._file.close()
-    path_dir = os.path.dirname(path)
-    if path_dir:
-        os.makedirs(path_dir, exist_ok=True)
-    self._file = open(path, "w", encoding=encoding)
-```
-But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
-```py
-@kola_command("open")
-def file(self, path: str, encoding: str = "utf-8") -> None:
-    if self._file:
-        self._file.close()
-    path_dir = os.path.dirname(path)
-    if path_dir:
-        os.makedirs(path_dir, exist_ok=True)
-    self._file = open(path, "w", encoding=encoding)
-```
-Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
-
-You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
-
-### File parse
-`KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
-
-### Advanced techniques
-In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
-
-```py
-class FastFile(KoiLang):
-    ...
-
-    class space(Environment):
-        @kola_env_enter("space")
-        def enter(self, name: str) -> None:
-            self.pwd = os.getcwd()
-            path = name.replace('.', '/')
-            if not os.path.isdir(path):
-                os.makedirs(path)
-            os.chdir(path)
-        
-        @kola_env_exit("endspace")
-        def exit(self) -> None:
-            os.chdir(self.pwd)
-```
-
-> There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
-
-## What is more
-
-The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
-
-On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
-
-## Bugs/Requests
-
-Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
+Metadata-Version: 2.1
+Name: KoiLang
+Version: 1.2.0a0
+Summary: simple python module for KoiLang parsing
+Home-page: https://github.com/Ovizro/Kola
+Author: Visecy
+Author-email: Visecy@visecy.top
+Maintainer: Ovizro
+Maintainer-email: Ovizro@visecy.top
+License: Apache 2.0
+Description: # Kola
+        Simple python module for KoiLang parsing.
+        
+        [![License](https://img.shields.io/github/license/Ovizro/Kola.svg)](LICENSE)
+        [![PyPI](https://img.shields.io/pypi/v/KoiLang.svg)](https://pypi.python.org/pypi/KoiLang)
+        ![PyPI - Downloads](https://img.shields.io/pypi/dw/KoiLang)
+        ![Python Version](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10-blue.svg)
+        
+        ## Installation
+        From pip:
+        
+            pip install KoiLang
+        
+        From source code:
+            
+            python setup.py build_ext --inplace
+            python setup.py install
+        
+        ## What is KoiLang
+        
+        KoiLang is a markup language while is easy to read for people.
+        There is an simple example.
+        ```
+        #background Street
+            #camera on(Orga)
+            #character Orga
+                Huh... I'm a pretty good shot, huh?
+            #camera on(Ride, Ched)
+            #character Ride
+                B- boss...
+            #character Orga
+                #action bleed
+            #camera on(object: blood, source: Orga)
+        
+            #camera on(Ched, Orga, Ride)
+            #character Orga
+                How come you're stammering like that... Ride!
+        
+            #playsound freesia
+        
+            #character Orga
+                #action stand_up speed(slowly)
+        
+            #character Ride
+                But... but!
+            #character Orga
+                I'm the Boss of Tekkadan, Orga Itsuka, this is nothing to me.
+            #character Ride
+                #action shed_tear
+                No... not for me...
+        
+            #camera on(Orga)
+            #character Orga
+                Protecting my members is my job!
+            #character Ched
+                #action shed_tear
+        
+            #character Ride
+                But...!
+            #character Orga
+                Shut up and let's go!
+        
+                #camera on(Orga)
+                #action walk direction(front) speed(slowly)
+                Everyone's waiting, besides...
+        
+                I finally understand now, Mika, we don't need any destinations, we just need to keep moving forward.
+                As long as we don't stop, the road will continue!
+        ```
+        
+        ### Grammar
+        
+        In KoiLang, the code contains 'command' section and 'text' section.
+        The format of the command section is similar to a C prepared statement,
+        using '#' as the prefix. And other lines that do not start with '#' are the text section.
+        
+            #command "This is a command"
+            This is the text.
+        
+        The format of a single command like:
+        
+            #command_name [param 1] [param 2] ...
+        
+        There are several parameters behind the command whose name should be a valid variable name.
+        
+        > An unsigned decimal integer like is also a legal command name, like `#114`.
+        
+        Each command can have several parameters behind the command name.
+        Valid argument type include integer, float, literal and string.
+            
+            #arg_int    1 0b101 0x6CF
+            #arg_float  1. 2e-2 .114514
+            #arg_literal string __name__
+            #arg_string "A string"
+        
+        > Here literal argument is a valid python variety name containing letter, digit, underline and not starting with digit. Usually it is the same as a string.
+         
+        The above parameter types are often referred to base parameters.
+        Combination parameter which is composed of multiple basic parameters is another argument type. It is a key-to-value mode which is starting with a literal as key and followed by several basic parameters.
+        The format is as follows:
+        
+            #kwargs key(value)
+            
+            And another format:
+            #keyargs_list key(item0, item1)
+            
+            And the third:
+            #kwargs_dict key(x: 11, y: 45, z: 14)
+        
+        All the parameters above can be put together:
+            
+            #draw Line 2 pos0(x: 0, y: 0) pos1(x: 16, y: 16) \
+                thickness(2) color(255, 255, 255)
+        
+        ## What can Kola module do
+        
+        Kola module provides a fast way to translate KoiLang command into a python function call.
+        
+        Above command `#draw` will convert to function call below:
+        
+        ```py
+        draw(
+            "Line", 2,
+            pos0={"x": 0, "y": 0},
+            pos1={"x": 16, "y": 16},
+            thickness=2,
+            color=[255, 255, 255]
+        )
+        ```
+        
+        Kola mudule just create a bridge from kola file to Python script. The bridge, the main class of Kola module, is `KoiLang` class. There is a simple example.
+        
+        ### Example
+        
+        Let's image a simple situation, where you want to create some small files. Manual creating is complex and time-consuming. Here is a way to solve that. We can use a single kola file to write all my text. Then use commands to devide these text in to different files.
+        
+        Let us start with a kola file:
+        
+        ```
+        ## This is the file `makefiles.kola`
+        
+        #file "hello.txt" encoding("utf-8")
+        Hello world!
+        And there are all my friends.
+        
+        #space hello
+        
+            #file "Bob.txt"
+            Hello Bob.
+        
+            #file "Alice.txt"
+            Hello Alice.
+        
+        #endspace
+        ```
+        
+        Just name it as `makefiles.kola`. Then, we make a script to explain how to do with these commands:
+        
+        ```py
+        import os
+        from kola import KoiLang, kola_command, kola_text
+        
+        
+        class FastFile(KoiLang):
+            @kola_command
+            def file(self, path: str, encoding: str = "utf-8") -> None:
+                if self._file:
+                    self._file.close()
+                path_dir = os.path.dirname(path)
+                if path_dir:
+                    os.makedirs(path_dir, exist_ok=True)
+                self._file = open(path, "w", encoding=encoding)
+            
+            @kola_command
+            def space(self, name: str) -> None:
+                path = name.replace('.', '/')
+                if not os.path.isdir(path):
+                    os.makedirs(path)
+                os.chdir(path)
+            
+            @kola_command
+            def endspace(self) -> None:
+                os.chdir("..")
+                self.end()
+        
+            @kola_command
+            def end(self) -> None:
+                if self._file:
+                    self._file.close()
+                    self._file = None
+            
+            @kola_text
+            def text(self, text: str) -> None:
+                if not self._file:
+                    raise OSError("write texts before the file open")
+                self._file.write(text)
+            
+            def at_start(self) -> None:
+                self._file = None
+            
+            def at_end(self) -> None:
+                self.end()
+        ```
+        
+        You can save the script in file `script.py`. After that, let us try to mix them together by entering the following in terminal:
+        
+        ```sh
+        python -m kola makefiles.kola -s script.py
+        ```
+        
+        Or add these directly at the end of the script:
+        ```py
+        if __name__ = "__main__":
+            FastFile().parse_file("makefiles.kola")
+        ```
+        
+        You will see new files in your work dir.
+        
+            <workdir>
+            │      
+            │  hello.txt
+            │      
+            └─hello
+                Alice.txt
+                Bob.txt
+        
+        ### What happened
+        
+        It seems amusing? Well, if you make a python script as this:
+        
+        ```py
+        vmobj = FastFile()
+        
+        with vmobj.exec_block():
+            vmobj.file("hello.txt", encoding="utf-8")
+            vmobj.text("Hello world!")
+            vmobj.text("And there are all my friends.")
+        
+            vmobj.space("hello")
+        
+            vmobj.file("Bob.txt")
+            vmobj.text("Hello Bob.")
+        
+            vmobj.file("Alice.txt")
+            vmobj.text("Hello Alice.")
+        
+            vmobj.endspace()
+        ```
+        the same result will be get. This is the python script corresponding to the previous kola file. What we have done is to make KoiLang interpreter know the correspondence between kola commands and python functions.
+        
+        So let's go back to the script. Here the first we need is a kola command set that is the top interface for parsing. All commands we want to use will be included in the set. The best way is create a subclass of `KoiLang` with all commands as methods. That is:
+        ```py
+        class FastFile(KoiLang):
+            ...
+        ```
+        The next step is making the kola command we need. So a function is defined here:
+        ```py
+        def file(self, path: str, encoding: str = "utf-8") -> None:
+            if self._file:
+                self._file.close()
+            path_dir = os.path.dirname(path)
+            if path_dir:
+                os.makedirs(path_dir, exist_ok=True)
+            self._file = open(path, "w", encoding=encoding)
+        ```
+        But it is not enough. Use the decorator `@kola_command` to annotate the function can be used in the kola text. In default case, the name of kola command will be the same to that of the function's. If another name is expected to use in kola files instead of the raw function name, you can use `@kola_command("new_name")` as the decorator. It wiil look like:
+        ```py
+        @kola_command("open")
+        def file(self, path: str, encoding: str = "utf-8") -> None:
+            if self._file:
+                self._file.close()
+            path_dir = os.path.dirname(path)
+            if path_dir:
+                os.makedirs(path_dir, exist_ok=True)
+            self._file = open(path, "w", encoding=encoding)
+        ```
+        Than `#open "hello.txt"` will be a valid command, while using `#space hello` would get a `KoiLangCommandError`.
+        
+        You may have notice that there is a special decorator `@kola_text`. As we know, the text section in kola files is a command, too. This decorator is to annotate the function to use to handle texts. Using `@kola_command("@text")` has the same effect. And another special decorator which is not shown here is `@kola_number`. It can handle commands like `#114` or `#1919`. The first argument wiil be the number in the command.
+        
+        ### File parse
+        `KoiLang` class provides several method. Use `parse` method to parse a string and `parse_file` to parse a file. It is suggested to use the second way so that KoiLang interpreter can give a traceback to the file when an error occure.
+        
+        ### Advanced techniques
+        In above example, we define two commands to create and leave the space. While, if users use `#endspace` before creating space, this can cause some problems. To correct user behavior, we can use the environment to restrict the use of some commands. `Environment` class should be used here to define a sub class that is the new environment:
+        
+        ```py
+        class FastFile(KoiLang):
+            ...
+        
+            class space(Environment):
+                @kola_env_enter("space")
+                def enter(self, name: str) -> None:
+                    self.pwd = os.getcwd()
+                    path = name.replace('.', '/')
+                    if not os.path.isdir(path):
+                        os.makedirs(path)
+                    os.chdir(path)
+                
+                @kola_env_exit("endspace")
+                def exit(self) -> None:
+                    os.chdir(self.pwd)
+        ```
+        
+        > There is a parameter named `envs` in `@kola_command`, which is also used to limit the environment where commands use. It means the top stack of environment must have the same name, while commands defined in the environment class mean the they can be used until the environment is pop from the environment stack, even though the stack top is other environment.
+        
+        ## What is more
+        
+        The most difference between KoiLang and other markup language like YAML which is data-centric is that KoiLang more pay attention to the command. Yeah, text in Kola file is a special command named `@text` too. In fact, the core idea of Kola is to separate data and instructions. The kola file is the data to execute commands, and the python script is the instructions. Then Kola module just mix they together. It can be considered as a simple virtual machine engine. if you want, you can even build a Python virtual machine (of course, I guess no one like to do that).
+        
+        On the other hand, text is also an important feature of Kola, which is a separate part, independent of context during parsing. The text is the soul of a Kola file. Any commands just are used to tell the computer what to do with the text. Though you can make a Kola file with only commands, it is not recommended. Instead, you ought to consider switching to another language.
+        
+        ## Bugs/Requests
+        
+        Please send bug reports and feature requests through [github issue tracker](https://github.com/Ovizro/Kola/issues). Kola is open to any constructive suggestions.
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Markup
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `KoiLang-1.1.1/kola/__init__.py` & `KoiLang-1.2.0a0/kola/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""
-simple python module for KoiLang parsing
-"""
-
-from .lexer import BaseLexer, FileLexer, StringLexer
-from .parser import Parser
-from .writer import BaseWriter, FileWriter, StringWriter, BaseWriterItem, FormatItem, ComplexArg, WriterItemLike
-from .klvm import KoiLang, Environment, kola_command, kola_text, kola_number, kola_annotation, kola_env_enter, kola_env_exit, kola_env_class
-from .version import __version__, __version_num__
-from .exception import KoiLangError, KoiLangSyntaxError, KoiLangCommandError
-
-
-__author__ = "Ovizro"
-__author_email__ = "Ovizro@visecy.top"
-
-__all__ = [
-    "KoiLang",
-    "Environment",
-    "kola_command",
-    "kola_text",
-    "kola_number",
-    "kola_annotation",
-    "kola_env_enter",
-    "kola_env_exit",
-    
-    "BaseLexer",
-    "FileLexer",
-    "StringLexer",
-    "Parser",
-    "BaseWriter",
-    "FileWriter",
-    "StringWriter",
-    "BaseWriterItem",
-    "FormatItem",
-    "ComplexArg",
-    "WriterItemLike",
-
-    "KoiLangError",
-    "KoiLangSyntaxError",
-    "KoiLangCommandError"
-]
+"""
+simple python module for KoiLang parsing
+"""
+
+from .lexer import BaseLexer, FileLexer, StringLexer
+from .parser import Parser
+from .writer import BaseWriter, FileWriter, StringWriter, BaseWriterItem, FormatItem, ComplexArg, WriterItemLike
+from .klvm import KoiLang, Environment, kola_command, kola_text, kola_number, kola_annotation, kola_env_enter, kola_env_exit, kola_env_class
+from .version import __version__, __version_num__
+from .exception import KoiLangError, KoiLangSyntaxError, KoiLangCommandError
+
+
+__author__ = "Ovizro"
+__author_email__ = "Ovizro@visecy.top"
+
+__all__ = [
+    "KoiLang",
+    "Environment",
+    "kola_command",
+    "kola_text",
+    "kola_number",
+    "kola_annotation",
+    "kola_env_enter",
+    "kola_env_exit",
+    
+    "BaseLexer",
+    "FileLexer",
+    "StringLexer",
+    "Parser",
+    "BaseWriter",
+    "FileWriter",
+    "StringWriter",
+    "BaseWriterItem",
+    "FormatItem",
+    "ComplexArg",
+    "WriterItemLike",
+
+    "KoiLangError",
+    "KoiLangSyntaxError",
+    "KoiLangCommandError"
+]
```

### Comparing `KoiLang-1.1.1/kola/_cutil.h` & `KoiLang-1.2.0a0/kola/_cutil.h`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-#ifndef _INCLUDE_HELPER_
-#define _INCLUDE_HELPER_ 
-
-#include <stdint.h>
-#include <stdio.h>
-#include <stdlib.h>
-#include <Python.h>
-
-#ifdef MS_WINDOWS
-#include <Windows.h>
-#endif
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-/* An opaque pointer. */
-#ifndef YY_TYPEDEF_YY_SCANNER_T
-#define YY_TYPEDEF_YY_SCANNER_T
-typedef void* yyscan_t;
-#endif
-
-#define LFLAG_DISABLED      (1 << 0)
-#define LFLAG_ISANNOTATION  (1 << 1)
-#define LFLAG_NOLSTRIP        (1 << 2)
-
-typedef struct lexer_extra {
-    const char* filename;
-    uint8_t command_threshold;
-    uint8_t flag;
-} LexerData;
-
-#define YY_EXTRA_TYPE LexerData*
-
-enum TokenSyn {
-    CMD=1, CMD_N, TEXT, LITERAL, STRING, NUM, NUM_H,
-    NUM_B, NUM_F, CLN, CMA, SLP, SRP, ANNOTATION
-};
-
-static const uint8_t yy_goto[7][8] = {
-    {15,    63,     0,      0,      0,      0,      0,  0},     // CMD | CMD_N | TEXT
-    {34,    162,    35,     117,    0,      151,    0,  40},    // LITERAL   
-    {17,    49,     35,     117,    0,      151,    0,  40},    // NUM | STRING
-    {0,     0,      134,    0,      0,      0,      0,  6},     // CLN
-    {0,     0,      100,    0,      4,      0,      8,  0},     // CMA
-    {0,     3,      0,      0,      0,      0,      0,  0},     // SLP
-    {0,     0,      65,     0,      81,     0,      81, 0}     // SRP
-};
-
-#ifdef Py_PYTHON_H
-
-#define get_type_qualname(obj) (Py_TYPE(obj)->tp_name)
-
-static __inline const char* get_type_name(PyObject* obj) {
-    const char* qualname = get_type_qualname(obj);
-    const char* name = strrchr(qualname, '.');
-    if (name == NULL) {
-        name = qualname;
-    } else {
-        name += 1;
-    }
-    return name;
-}
-
-#define ERR_CASE(syn, act) case (act << 4) + syn
-#define ERR_MSG(msg) return "[%d] " # msg
-
-static const char* get_format(int code) {
-    switch (code)
-    {
-    case 1:
-        ERR_MSG(unknown symbol '%s');
-    case 2:
-        ERR_MSG(command '%s' not found);
-    case 3:
-        ERR_MSG(an error occured during handling command '%s');
-    case 4:
-        ERR_MSG(an error occured during handling text '%s');
-    case 5:
-        ERR_MSG(cannot decode string '%s');
-    case 10:
-        ERR_MSG(end of line in incurrect place);
-    case 16:
-        ERR_MSG(unclosed parentheses);
-    case 28:
-        ERR_MSG(keyword must be a literal);
-    case 201:
-    case 202:
-    case 210:
-        ERR_MSG(bad argument count);
-    }
-    
-    switch (code & 0x0F)
-    {
-    case CMD:
-    case CMD_N:
-    case TEXT:
-    case ANNOTATION:
-        ERR_MSG(end of line in incurrect place);
-    }
-    ERR_MSG(unknown syntax);
-}
-
-#include "frameobject.h"
-// For Cython limiting, error setting function has to define here 
-static void __inline kola_set_error(PyObject* exc_type, int errorno,
-                            const char* filename, int lineno, const char* text) 
-{
-    PyErr_Format(exc_type, get_format(errorno), errorno, text);
-
-    // add traceback in .kola file
-    #if PY_VERSION_HEX >= 0x03080000
-        _PyTraceback_Add("<kola>", filename, lineno);
-    #else
-        PyCodeObject* code = NULL;
-        PyFrameObject* frame = NULL;
-        PyObject* globals = NULL;
-        PyObject *exc, *val, *tb;
-
-        PyErr_Fetch(&exc, &val, &tb);
-
-        globals = PyDict_New();
-        if (!globals) goto end;
-        code = PyCode_NewEmpty(filename, "<kola>", lineno);
-        if (!code) goto end;
-        frame = PyFrame_New(
-            PyThreadState_Get(),
-            code,
-            globals,
-            NULL
-        );
-        if (!frame) goto end;
-
-        frame->f_lineno = lineno;
-        PyErr_Restore(exc, val, tb);
-        PyTraceBack_Here(frame);
-
-    end:
-        Py_XDECREF(code);
-        Py_XDECREF(frame);
-        Py_XDECREF(globals);
-    #endif
-}
-
-static void __inline kola_set_errcause(PyObject* exc_type, int errorno,
-                            const char* filename, int lineno, const char* text, PyObject* cause) 
-{
-    PyErr_Format(exc_type, get_format(errorno), errorno, text);
-    
-    PyObject *exc, *val, *tb;
-    PyErr_Fetch(&exc, &val, &tb);
-    if (cause == Py_None) {
-        PyException_SetContext(val, NULL);
-    } else {
-        Py_INCREF(cause);
-        PyException_SetCause(val, cause);
-    }
-    #if PY_VERSION_HEX >= 0x03080000
-        PyErr_Restore(exc, val, tb);
-        _PyTraceback_Add("<kola>", filename, lineno);
-    #else
-        PyCodeObject* code = NULL;
-        PyFrameObject* frame = NULL;
-        PyObject* globals = NULL;
-        globals = PyDict_New();
-        if (!globals) goto end;
-        code = PyCode_NewEmpty(filename, "<kola>", lineno);
-        if (!code) goto end;
-        frame = PyFrame_New(
-            PyThreadState_Get(),
-            code,
-            globals,
-            NULL
-        );
-        if (!frame) goto end;
-
-        frame->f_lineno = lineno;
-        PyErr_Restore(exc, val, tb);
-        PyTraceBack_Here(frame);
-
-    end:
-        Py_XDECREF(code);
-        Py_XDECREF(frame);
-        Py_XDECREF(globals);
-    #endif
-}
-
-static __inline FILE* kola_open(PyObject* raw_path, PyObject** out, const char* mode) {
-    PyObject* stringobj = NULL;
-    FILE* fp;
-#ifdef MS_WINDOWS
-    wchar_t wmode[5];
-    DWORD dwNum = MultiByteToWideChar(CP_ACP, 0, mode, -1, NULL, 0); 
-    if (dwNum > 4) {
-        PyErr_Format(PyExc_ValueError, "invalid mode: %.200s", mode);
-        return NULL;
-    }
-    MultiByteToWideChar(CP_ACP, 0, mode, -1, wmode, dwNum);
-    Py_UNICODE *widename = NULL;
-    if (!PyUnicode_FSDecoder(raw_path, &stringobj)) {
-        return NULL;
-    }
-    widename = PyUnicode_AsWideCharString(stringobj, NULL);
-    if (widename == NULL) {
-        return NULL;
-    }
-
-    Py_BEGIN_ALLOW_THREADS
-    fp = _wfopen(widename, wmode);
-    Py_END_ALLOW_THREADS
-#else
-    const char *name = NULL;
-    if (!PyUnicode_FSConverter(raw_path, &stringobj)) {
-        return NULL;
-    }
-    name = PyBytes_AS_STRING(stringobj);
-
-    Py_BEGIN_ALLOW_THREADS
-    fp = fopen(name, mode);
-    Py_END_ALLOW_THREADS
-#endif
-    if (fp == NULL) {
-        PyErr_SetFromErrno(PyExc_OSError);
-        // PyErr_Format(PyExc_OSError, "fail to open '%S'", raw_path);
-    }
-    if (out)
-        *out = stringobj;
-    else
-        Py_DECREF(stringobj);
-    return fp;
-}
-
-static __inline const char* unicode2string(PyObject* __s, Py_ssize_t* s_len) {
-    Py_ssize_t _s_len;
-    const char* s = PyUnicode_AsUTF8AndSize(__s, &_s_len);
-    if (s == NULL)
-        return NULL;
-    else if (strlen(s) != (size_t)_s_len) {
-        PyErr_SetString(PyExc_ValueError, "embedded null character");
-        return NULL;
-    }
-    if (s_len)
-        *s_len = _s_len;
-    return s;
-}
-
-// from cpython:string_parser.decode_unicode_with_escapes
-PyObject* decode_escapes(const char* s, Py_ssize_t len);
-PyObject* filter_text(PyObject* string);
-#endif
-
-#ifdef __cplusplus
-}
-#endif
+#ifndef _INCLUDE_HELPER_
+#define _INCLUDE_HELPER_ 
+
+#include <stdint.h>
+#include <stdio.h>
+#include <stdlib.h>
+#include <Python.h>
+
+#ifdef MS_WINDOWS
+#include <Windows.h>
+#endif
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+/* An opaque pointer. */
+#ifndef YY_TYPEDEF_YY_SCANNER_T
+#define YY_TYPEDEF_YY_SCANNER_T
+typedef void* yyscan_t;
+#endif
+
+#define LFLAG_DISABLED      (1 << 0)
+#define LFLAG_ISANNOTATION  (1 << 1)
+#define LFLAG_NOLSTRIP        (1 << 2)
+
+typedef struct lexer_extra {
+    const char* filename;
+    uint8_t command_threshold;
+    uint8_t flag;
+} LexerData;
+
+#define YY_EXTRA_TYPE LexerData*
+
+enum TokenSyn {
+    CMD=1, CMD_N, TEXT, LITERAL, STRING, NUM, NUM_H,
+    NUM_B, NUM_F, CLN, CMA, SLP, SRP, ANNOTATION
+};
+
+static const uint8_t yy_goto[7][8] = {
+    {15,    63,     0,      0,      0,      0,      0,  0},     // CMD | CMD_N | TEXT
+    {34,    162,    35,     117,    0,      151,    0,  40},    // LITERAL   
+    {17,    49,     35,     117,    0,      151,    0,  40},    // NUM | STRING
+    {0,     0,      134,    0,      0,      0,      0,  6},     // CLN
+    {0,     0,      100,    0,      4,      0,      8,  0},     // CMA
+    {0,     3,      0,      0,      0,      0,      0,  0},     // SLP
+    {0,     0,      65,     0,      81,     0,      81, 0}     // SRP
+};
+
+#ifdef Py_PYTHON_H
+
+#define get_type_qualname(obj) (Py_TYPE(obj)->tp_name)
+
+static __inline const char* get_type_name(PyObject* obj) {
+    const char* qualname = get_type_qualname(obj);
+    const char* name = strrchr(qualname, '.');
+    if (name == NULL) {
+        name = qualname;
+    } else {
+        name += 1;
+    }
+    return name;
+}
+
+#define ERR_CASE(syn, act) case (act << 4) + syn
+#define ERR_MSG(msg) return "[%d] " # msg
+
+static const char* get_format(int code) {
+    switch (code)
+    {
+    case 1:
+        ERR_MSG(unknown symbol '%s');
+    case 2:
+        ERR_MSG(command '%s' not found);
+    case 3:
+        ERR_MSG(an error occured during handling command '%s');
+    case 4:
+        ERR_MSG(an error occured during handling text '%s');
+    case 5:
+        ERR_MSG(cannot decode string '%s');
+    case 10:
+        ERR_MSG(end of line in incurrect place);
+    case 16:
+        ERR_MSG(unclosed parentheses);
+    case 28:
+        ERR_MSG(keyword must be a literal);
+    case 201:
+    case 202:
+    case 210:
+        ERR_MSG(bad argument count);
+    }
+    
+    switch (code & 0x0F)
+    {
+    case CMD:
+    case CMD_N:
+    case TEXT:
+    case ANNOTATION:
+        ERR_MSG(end of line in incurrect place);
+    }
+    ERR_MSG(unknown syntax);
+}
+
+#include "frameobject.h"
+// For Cython limiting, error setting function has to define here 
+static void __inline kola_set_error(PyObject* exc_type, int errorno,
+                            const char* filename, int lineno, const char* text) 
+{
+    PyErr_Format(exc_type, get_format(errorno), errorno, text);
+
+    // add traceback in .kola file
+    #if PY_VERSION_HEX >= 0x03080000
+        _PyTraceback_Add("<kola>", filename, lineno);
+    #else
+        PyCodeObject* code = NULL;
+        PyFrameObject* frame = NULL;
+        PyObject* globals = NULL;
+        PyObject *exc, *val, *tb;
+
+        PyErr_Fetch(&exc, &val, &tb);
+
+        globals = PyDict_New();
+        if (!globals) goto end;
+        code = PyCode_NewEmpty(filename, "<kola>", lineno);
+        if (!code) goto end;
+        frame = PyFrame_New(
+            PyThreadState_Get(),
+            code,
+            globals,
+            NULL
+        );
+        if (!frame) goto end;
+
+        frame->f_lineno = lineno;
+        PyErr_Restore(exc, val, tb);
+        PyTraceBack_Here(frame);
+
+    end:
+        Py_XDECREF(code);
+        Py_XDECREF(frame);
+        Py_XDECREF(globals);
+    #endif
+}
+
+static void __inline kola_set_errcause(PyObject* exc_type, int errorno,
+                            const char* filename, int lineno, const char* text, PyObject* cause) 
+{
+    PyErr_Format(exc_type, get_format(errorno), errorno, text);
+    
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    if (cause == Py_None) {
+        PyException_SetContext(val, NULL);
+    } else {
+        Py_INCREF(cause);
+        PyException_SetCause(val, cause);
+    }
+    #if PY_VERSION_HEX >= 0x03080000
+        PyErr_Restore(exc, val, tb);
+        _PyTraceback_Add("<kola>", filename, lineno);
+    #else
+        PyCodeObject* code = NULL;
+        PyFrameObject* frame = NULL;
+        PyObject* globals = NULL;
+        globals = PyDict_New();
+        if (!globals) goto end;
+        code = PyCode_NewEmpty(filename, "<kola>", lineno);
+        if (!code) goto end;
+        frame = PyFrame_New(
+            PyThreadState_Get(),
+            code,
+            globals,
+            NULL
+        );
+        if (!frame) goto end;
+
+        frame->f_lineno = lineno;
+        PyErr_Restore(exc, val, tb);
+        PyTraceBack_Here(frame);
+
+    end:
+        Py_XDECREF(code);
+        Py_XDECREF(frame);
+        Py_XDECREF(globals);
+    #endif
+}
+
+static __inline FILE* kola_open(PyObject* raw_path, PyObject** out, const char* mode) {
+    PyObject* stringobj = NULL;
+    FILE* fp;
+#ifdef MS_WINDOWS
+    wchar_t wmode[5];
+    DWORD dwNum = MultiByteToWideChar(CP_ACP, 0, mode, -1, NULL, 0); 
+    if (dwNum > 4) {
+        PyErr_Format(PyExc_ValueError, "invalid mode: %.200s", mode);
+        return NULL;
+    }
+    MultiByteToWideChar(CP_ACP, 0, mode, -1, wmode, dwNum);
+    Py_UNICODE *widename = NULL;
+    if (!PyUnicode_FSDecoder(raw_path, &stringobj)) {
+        return NULL;
+    }
+    widename = PyUnicode_AsWideCharString(stringobj, NULL);
+    if (widename == NULL) {
+        return NULL;
+    }
+
+    Py_BEGIN_ALLOW_THREADS
+    fp = _wfopen(widename, wmode);
+    Py_END_ALLOW_THREADS
+#else
+    const char *name = NULL;
+    if (!PyUnicode_FSConverter(raw_path, &stringobj)) {
+        return NULL;
+    }
+    name = PyBytes_AS_STRING(stringobj);
+
+    Py_BEGIN_ALLOW_THREADS
+    fp = fopen(name, mode);
+    Py_END_ALLOW_THREADS
+#endif
+    if (fp == NULL) {
+        PyErr_SetFromErrno(PyExc_OSError);
+        // PyErr_Format(PyExc_OSError, "fail to open '%S'", raw_path);
+    }
+    if (out)
+        *out = stringobj;
+    else
+        Py_DECREF(stringobj);
+    return fp;
+}
+
+static __inline const char* unicode2string(PyObject* __s, Py_ssize_t* s_len) {
+    Py_ssize_t _s_len;
+    const char* s = PyUnicode_AsUTF8AndSize(__s, &_s_len);
+    if (s == NULL)
+        return NULL;
+    else if (strlen(s) != (size_t)_s_len) {
+        PyErr_SetString(PyExc_ValueError, "embedded null character");
+        return NULL;
+    }
+    if (s_len)
+        *s_len = _s_len;
+    return s;
+}
+
+// from cpython:string_parser.decode_unicode_with_escapes
+PyObject* decode_escapes(const char* s, Py_ssize_t len);
+PyObject* filter_text(PyObject* string);
+#endif
+
+#ifdef __cplusplus
+}
+#endif
 #endif
```

### Comparing `KoiLang-1.1.1/kola/_cutil.pxd` & `KoiLang-1.2.0a0/kola/_cutil.pxd`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-from libc.stdio cimport FILE
-from libc.stdint cimport uint8_t, uint64_t
-from cpython cimport PyObject
-
-
-cdef extern from "<stdarg.h>":
-    ctypedef struct va_list
-    void va_start(va_list ap, const char* last_arg) nogil
-    void va_end(va_list ap) nogil
-
-cdef extern from "Python.h":
-    PyObject* _PyType_Lookup(type t, str name)
-    
-    ctypedef uint64_t Py_UCS4
-    
-    str PyUnicode_FromFormat(const char* format, ...)
-    Py_UCS4 PyUnicode_READ_CHAR(str unicode, Py_ssize_t index)
-    int PyUnicode_WriteChar(
-        str unicode, Py_ssize_t index, Py_UCS4 character) except -1
-
-    enum PyUnicode_Kind:
-        PyUnicode_WCHAR_KIND = 0
-        PyUnicode_1BYTE_KIND = 1
-        PyUnicode_2BYTE_KIND = 2
-        PyUnicode_4BYTE_KIND = 4
-
-    ctypedef struct _PyUnicodeWriter:
-        PyObject* buffer
-        void* data
-        PyUnicode_Kind kind
-        Py_UCS4 maxchar
-        Py_ssize_t size
-        Py_ssize_t pos
-
-        # minimum number of allocated characters (default: 0)
-        Py_ssize_t min_length
-
-        # minimum character (default: 127, ASCII)
-        Py_UCS4 min_char
-
-        # If non-zero, overallocate the buffer (default: 0).
-        unsigned char overallocate
-
-        # If readonly is 1, buffer is a shared string (cannot be modified)
-        # and size is set to 0.
-        unsigned char readonly_ "readonly"
-    
-    void _PyUnicodeWriter_Init(_PyUnicodeWriter *writer)
-    int _PyUnicodeWriter_Prepare(_PyUnicodeWriter *writer, Py_ssize_t length, Py_UCS4 maxchar) except -1
-    int _PyUnicodeWriter_PrepareKind(_PyUnicodeWriter *writer, PyUnicode_Kind kind) except -1
-    int _PyUnicodeWriter_WriteChar(_PyUnicodeWriter *writer, Py_UCS4 ch) except -1
-    int _PyUnicodeWriter_WriteStr(_PyUnicodeWriter *writer, str string) except -1
-    int _PyUnicodeWriter_WriteASCIIString(_PyUnicodeWriter *writer, const char* string, Py_ssize_t len) except -1
-    str _PyUnicodeWriter_Finish(_PyUnicodeWriter *writer)
-    void _PyUnicodeWriter_Dealloc(_PyUnicodeWriter *writer)
-
-
-cdef extern from "_cutil.h":
-    enum TokenSyn:
-        CMD
-        CMD_N
-        TEXT
-        LITERAL
-        STRING
-        NUM
-        NUM_H
-        NUM_B
-        NUM_F
-        CLN
-        CMA
-        SLP
-        SRP
-        ANNOTATION
-    const uint8_t yy_goto[7][8]
-
-    const int LFLAG_DISABLED
-    const int LFLAG_ISANNOTATION
-    const int LFLAG_NOLSTRIP
-    
-    ctypedef struct LexerData:
-        const char* filename
-        uint8_t command_threshold
-        uint8_t flag
-    ctypedef void* yyscan_t
-
-    void kola_set_error(object exc_type, int errorno, const char* filename, int lineno, const char* text) except *
-    void kola_set_errcause(object exc_type, int errorno, const char* filename, int lineno, const char* text, object cause) except *
-
-    FILE* kola_open(object raw_path, PyObject** out, const char* mod) except NULL
-
-    const char* get_type_name(object obj) nogil
-    const char* get_type_qualname(object obj) nogil
-    const char* unicode2string(str __s, Py_ssize_t* s_len) except NULL
-    str decode_escapes(const char* string, Py_ssize_t len)
-    PyObject* filter_text(str string) except NULL
+from libc.stdio cimport FILE
+from libc.stdint cimport uint8_t, uint64_t
+from cpython cimport PyObject
+
+
+cdef extern from "<stdarg.h>":
+    ctypedef struct va_list
+    void va_start(va_list ap, const char* last_arg) nogil
+    void va_end(va_list ap) nogil
+
+cdef extern from "Python.h":
+    PyObject* _PyType_Lookup(type t, str name)
+    
+    ctypedef uint64_t Py_UCS4
+    
+    str PyUnicode_FromFormat(const char* format, ...)
+    Py_UCS4 PyUnicode_READ_CHAR(str unicode, Py_ssize_t index)
+    int PyUnicode_WriteChar(
+        str unicode, Py_ssize_t index, Py_UCS4 character) except -1
+
+    enum PyUnicode_Kind:
+        PyUnicode_WCHAR_KIND = 0
+        PyUnicode_1BYTE_KIND = 1
+        PyUnicode_2BYTE_KIND = 2
+        PyUnicode_4BYTE_KIND = 4
+
+    ctypedef struct _PyUnicodeWriter:
+        PyObject* buffer
+        void* data
+        PyUnicode_Kind kind
+        Py_UCS4 maxchar
+        Py_ssize_t size
+        Py_ssize_t pos
+
+        # minimum number of allocated characters (default: 0)
+        Py_ssize_t min_length
+
+        # minimum character (default: 127, ASCII)
+        Py_UCS4 min_char
+
+        # If non-zero, overallocate the buffer (default: 0).
+        unsigned char overallocate
+
+        # If readonly is 1, buffer is a shared string (cannot be modified)
+        # and size is set to 0.
+        unsigned char readonly_ "readonly"
+    
+    void _PyUnicodeWriter_Init(_PyUnicodeWriter *writer)
+    int _PyUnicodeWriter_Prepare(_PyUnicodeWriter *writer, Py_ssize_t length, Py_UCS4 maxchar) except -1
+    int _PyUnicodeWriter_PrepareKind(_PyUnicodeWriter *writer, PyUnicode_Kind kind) except -1
+    int _PyUnicodeWriter_WriteChar(_PyUnicodeWriter *writer, Py_UCS4 ch) except -1
+    int _PyUnicodeWriter_WriteStr(_PyUnicodeWriter *writer, str string) except -1
+    int _PyUnicodeWriter_WriteASCIIString(_PyUnicodeWriter *writer, const char* string, Py_ssize_t len) except -1
+    str _PyUnicodeWriter_Finish(_PyUnicodeWriter *writer)
+    void _PyUnicodeWriter_Dealloc(_PyUnicodeWriter *writer)
+
+
+cdef extern from "_cutil.h":
+    enum TokenSyn:
+        CMD
+        CMD_N
+        TEXT
+        LITERAL
+        STRING
+        NUM
+        NUM_H
+        NUM_B
+        NUM_F
+        CLN
+        CMA
+        SLP
+        SRP
+        ANNOTATION
+    const uint8_t yy_goto[7][8]
+
+    const int LFLAG_DISABLED
+    const int LFLAG_ISANNOTATION
+    const int LFLAG_NOLSTRIP
+    
+    ctypedef struct LexerData:
+        const char* filename
+        uint8_t command_threshold
+        uint8_t flag
+    ctypedef void* yyscan_t
+
+    void kola_set_error(object exc_type, int errorno, const char* filename, int lineno, const char* text) except *
+    void kola_set_errcause(object exc_type, int errorno, const char* filename, int lineno, const char* text, object cause) except *
+
+    FILE* kola_open(object raw_path, PyObject** out, const char* mod) except NULL
+
+    const char* get_type_name(object obj) nogil
+    const char* get_type_qualname(object obj) nogil
+    const char* unicode2string(str __s, Py_ssize_t* s_len) except NULL
+    str decode_escapes(const char* string, Py_ssize_t len)
+    PyObject* filter_text(str string) except NULL
```

### Comparing `KoiLang-1.1.1/kola/_yylex.pxd` & `KoiLang-1.2.0a0/kola/_yylex.pxd`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from libc.stdio cimport FILE
-from ._cutil cimport yyscan_t, LexerData
-
-cdef extern from "lex.yy.c":
-    ctypedef LexerData* YY_EXTRA_TYPE
-    ctypedef void* YY_BUFFER_STATE
-
-    # main parser
-    int yylex(yyscan_t yyscanner) nogil
-    
-    int yylex_init(yyscan_t* ptr_yy_globals) nogil
-    int yylex_init_extra(YY_EXTRA_TYPE yy_user_defined, yyscan_t* ptr_yy_globals) nogil
-    int yylex_destroy(yyscan_t yyscanner) nogil
-    void yyrestart(FILE* input_file, yyscan_t yyscanner) nogil
-    bint yylex_check(yyscan_t yyscanner) nogil
-
-    # Accessor  methods (get/set functions) to struct members.
-    int yyget_lineno(yyscan_t yyscanner) nogil
-    int yyget_column(yyscan_t yyscanner) nogil
-    FILE *yyget_in(yyscan_t yyscanner) nogil
-    FILE *yyget_out(yyscan_t yyscanner) nogil
-    int yyget_leng(yyscan_t yyscanner) nogil
-    char* yyget_text(yyscan_t yyscanner) nogil
-    void yyset_lineno(int _line_number, yyscan_t yyscanner) nogil
-    void yyset_column(int _column_no , yyscan_t yyscanner) nogil
-    void yyset_in(FILE* _in_str , yyscan_t yyscanner) nogil
-    void yyset_out(FILE* _out_str , yyscan_t yyscanner) nogil
-
-    void yypush_buffer_state(YY_BUFFER_STATE new_buffer, yyscan_t yyscanner) nogil
-    void yypop_buffer_state(yyscan_t yyscanner) nogil
-    YY_BUFFER_STATE yy_create_buffer(FILE* file, int size, yyscan_t yyscanner) nogil
-    YY_BUFFER_STATE yy_scan_buffer(char* base, Py_ssize_t size, yyscan_t yyscanner) nogil
+from libc.stdio cimport FILE
+from ._cutil cimport yyscan_t, LexerData
+
+cdef extern from "lex.yy.c":
+    ctypedef LexerData* YY_EXTRA_TYPE
+    ctypedef void* YY_BUFFER_STATE
+
+    # main parser
+    int yylex(yyscan_t yyscanner) nogil
+    
+    int yylex_init(yyscan_t* ptr_yy_globals) nogil
+    int yylex_init_extra(YY_EXTRA_TYPE yy_user_defined, yyscan_t* ptr_yy_globals) nogil
+    int yylex_destroy(yyscan_t yyscanner) nogil
+    void yyrestart(FILE* input_file, yyscan_t yyscanner) nogil
+    bint yylex_check(yyscan_t yyscanner) nogil
+
+    # Accessor  methods (get/set functions) to struct members.
+    int yyget_lineno(yyscan_t yyscanner) nogil
+    int yyget_column(yyscan_t yyscanner) nogil
+    FILE *yyget_in(yyscan_t yyscanner) nogil
+    FILE *yyget_out(yyscan_t yyscanner) nogil
+    int yyget_leng(yyscan_t yyscanner) nogil
+    char* yyget_text(yyscan_t yyscanner) nogil
+    void yyset_lineno(int _line_number, yyscan_t yyscanner) nogil
+    void yyset_column(int _column_no , yyscan_t yyscanner) nogil
+    void yyset_in(FILE* _in_str , yyscan_t yyscanner) nogil
+    void yyset_out(FILE* _out_str , yyscan_t yyscanner) nogil
+
+    void yypush_buffer_state(YY_BUFFER_STATE new_buffer, yyscan_t yyscanner) nogil
+    void yypop_buffer_state(yyscan_t yyscanner) nogil
+    YY_BUFFER_STATE yy_create_buffer(FILE* file, int size, yyscan_t yyscanner) nogil
+    YY_BUFFER_STATE yy_scan_buffer(char* base, Py_ssize_t size, yyscan_t yyscanner) nogil
     YY_BUFFER_STATE yy_scan_bytes(const char* text, int len, yyscan_t yyscanner) nogil
```

### Comparing `KoiLang-1.1.1/kola/klvm/command.py` & `KoiLang-1.2.0a0/kola/klvm/command.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from functools import partialmethod
-from types import MethodType
-from typing import Any, Callable, Dict, Generator, Iterable, Tuple, Union, overload
-from typing_extensions import Self, Protocol, runtime_checkable
-
-
-class CommandCaller(Protocol):
-    def __call__(self, __command: Any, __args: tuple, __kwargs: Dict[str, Any], **kwds: Any) -> Any: ...
-
-
-@runtime_checkable
-class CommandLike(Protocol):
-    def __kola_command__(self) -> Generator[Tuple[str, Callable], None, None]: ...
-
-
-class Command(object):
-    __slots__ = ["__name__", "__func__", "suppression", "virtual", "alias", "extra_data"]
-
-    def __init__(
-        self,
-        __name: str,
-        func: Callable,
-        *,
-        alias: Union[Iterable[str], str] = (),
-        suppression: bool = False,
-        virtual: bool = False,
-        **kwds: Any
-    ) -> None:
-        self.__name__ = __name
-        self.__func__ = func
-        self.alias = (alias,) if isinstance(alias, str) else tuple(alias)
-        self.suppression = suppression
-        self.virtual = virtual
-        self.extra_data = kwds
-    
-    @overload
-    def set_data(self, __name: str, value: Any) -> Self: ...
-    @overload
-    def set_data(self, __name: str) -> Callable[[Any], Self]: ...
-
-    def set_data(self, __name: str, value: Any = None) -> Union[Self, Callable[[Any], Self]]:
-        if value is not None:
-            self.extra_data[__name] = value
-            return self
-        
-        def wrapper(val: Any) -> Self:
-            self.extra_data[__name] = val
-            return self
-        return wrapper
-
-    writer = partialmethod(set_data, "writer_func")
-    
-    @classmethod
-    def from_command(cls, command: "Command", **kwds: Any) -> Self:
-        data = command.extra_data.copy()
-        data.update(kwds)
-        return cls(
-            command.__name__,
-            command.__func__,
-            alias=command.alias,
-            **data
-        )
-    
-    @property
-    def __wrapped__(self) -> Callable:  # pragma: no cover
-        return self.__func__
-    
-    def __kola_command__(self, force: bool = False) -> Generator[Tuple[str, Self], None, None]:
-        if not self.suppression or force:
-            bound_func = self
-            yield self.__name__, bound_func
-            for i in self.alias:
-                yield i, bound_func
-
-    def __get__(self, ins: Any, owner: type) -> Any:
-        if ins is None:
-            return self
-        elif self.virtual and (not hasattr(owner, "check_virtual") or ins.check_virtual(self)):
-            return ins[self.__name__]
-        return MethodType(self, ins)
-
-    def __call__(self, vmobj: Any, *args: Any, **kwds: Any) -> Any:
-        caller = getattr(vmobj, "__kola_caller__", None)
-        if caller is None:  # pragma: no cover
-            return self.__func__(vmobj, *args, **kwds)
-        return caller(self, args, kwds, **self.extra_data)
-
-    def __repr__(self) -> str:
-        return f"<kola command {self.__name__} with {self.__func__}>"
+from functools import partialmethod
+from types import MethodType
+from typing import Any, Callable, Dict, Generator, Iterable, Tuple, Union, overload
+from typing_extensions import Self, Protocol, runtime_checkable
+
+
+class CommandCaller(Protocol):
+    def __call__(self, __command: Any, __args: tuple, __kwargs: Dict[str, Any], **kwds: Any) -> Any: ...
+
+
+@runtime_checkable
+class CommandLike(Protocol):
+    def __kola_command__(self) -> Generator[Tuple[str, Callable], None, None]: ...
+
+
+class Command(object):
+    __slots__ = ["__name__", "__func__", "suppression", "virtual", "alias", "extra_data"]
+
+    def __init__(
+        self,
+        __name: str,
+        func: Callable,
+        *,
+        alias: Union[Iterable[str], str] = (),
+        suppression: bool = False,
+        virtual: bool = False,
+        **kwds: Any
+    ) -> None:
+        self.__name__ = __name
+        self.__func__ = func
+        self.alias = (alias,) if isinstance(alias, str) else tuple(alias)
+        self.suppression = suppression
+        self.virtual = virtual
+        self.extra_data = kwds
+    
+    @overload
+    def set_data(self, __name: str, value: Any) -> Self: ...
+    @overload
+    def set_data(self, __name: str) -> Callable[[Any], Self]: ...
+
+    def set_data(self, __name: str, value: Any = None) -> Union[Self, Callable[[Any], Self]]:
+        if value is not None:
+            self.extra_data[__name] = value
+            return self
+        
+        def wrapper(val: Any) -> Self:
+            self.extra_data[__name] = val
+            return self
+        return wrapper
+
+    writer = partialmethod(set_data, "writer_func")
+    
+    @classmethod
+    def from_command(cls, command: "Command", **kwds: Any) -> Self:
+        data = command.extra_data.copy()
+        data.update(kwds)
+        return cls(
+            command.__name__,
+            command.__func__,
+            alias=command.alias,
+            **data
+        )
+    
+    @property
+    def __wrapped__(self) -> Callable:  # pragma: no cover
+        return self.__func__
+    
+    def __kola_command__(self, force: bool = False) -> Generator[Tuple[str, Self], None, None]:
+        if not self.suppression or force:
+            bound_func = self
+            yield self.__name__, bound_func
+            for i in self.alias:
+                yield i, bound_func
+
+    def __get__(self, ins: Any, owner: type) -> Any:
+        if ins is None:
+            return self
+        elif self.virtual and (not hasattr(owner, "check_virtual") or ins.check_virtual(self)):
+            return ins[self.__name__]
+        return MethodType(self, ins)
+
+    def __call__(self, vmobj: Any, *args: Any, **kwds: Any) -> Any:
+        caller = getattr(vmobj, "__kola_caller__", None)
+        if caller is None:  # pragma: no cover
+            return self.__func__(vmobj, *args, **kwds)
+        return caller(self, args, kwds, **self.extra_data)
+
+    def __repr__(self) -> str:
+        return f"<kola command {self.__name__} with {self.__func__}>"
```

### Comparing `KoiLang-1.1.1/kola/klvm/commandset.py` & `KoiLang-1.2.0a0/kola/klvm/commandset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,137 +1,139 @@
-from abc import ABCMeta
-from types import MethodType
-from typing import Any, Callable, Dict, Optional, Set, Tuple, Type, Union
-from typing_extensions import Self
-
-from .command import CommandLike, Command
-
-
-class CommandSetMeta(ABCMeta):
-    """
-    metaclass for all command sets
-    """
-    __command_field__: Set[CommandLike]
-    __virtual_table__: Dict[str, str]
-
-    def __new__(cls, name: str, bases: Tuple[Type, ...], attr: Dict[str, Any], **kwds: Any) -> Self:
-        command_field = set()
-        virtual_table = attr.get("__virtual_table__", {})
-        for i in bases:
-            if isinstance(i, CommandSetMeta):
-                virtual_table.update(i.__virtual_table__)
-        for k, v in attr.items():
-            if isinstance(v, Command):
-                if v.virtual:
-                    virtual_table[k] = v.__name__
-            elif k in virtual_table:
-                attr[k] = v = Command(virtual_table[k], v, virtual=True)
-            elif not isinstance(v, CommandLike):
-                continue
-            command_field.add(v)
-        attr["__command_field__"] = command_field
-        attr["__virtual_table__"] = virtual_table
-        return super().__new__(cls, name, bases, attr, **kwds)
-
-    def generate_raw_commands(self) -> Dict[str, Any]:
-        cmd_set = {}
-        for cls in reversed(self.__mro__):
-            cls: Type
-            if not isinstance(cls, CommandSetMeta):
-                continue
-            for c in cls.__command_field__:
-                cmd_set.update(c.__kola_command__())
-        return cmd_set
-
-    def _command_register_factory(cmd_name: Optional[str] = None):  # type: ignore
-        def inner(
-            self,
-            __func_or_name: Union[Callable, str, None] = None,
-            **kwds
-        ) -> Union[Callable[[Callable], Command], Command]:
-            def wrapper(wrapped_func: Callable[..., Any]) -> Command:
-                if cmd_name is not None:
-                    assert not isinstance(__func_or_name, str)
-                    name = cmd_name
-                elif isinstance(__func_or_name, str):
-                    name = __func_or_name
-                else:
-                    name = wrapped_func.__name__
-                cmd = Command(name, wrapped_func, **kwds)
-                self.__command_field__.add(cmd)
-                return cmd
-            if callable(__func_or_name):
-                return wrapper(__func_or_name)
-            else:
-                return wrapper
-        return inner
-
-    register_command = _command_register_factory()
-    register_text = _command_register_factory("@text")
-    register_number = _command_register_factory("@number")
-    register_annotation = _command_register_factory("@annotation")
-
-    del _command_register_factory
-    
-    def __repr__(self) -> str:
-        return f"<kola command set '{self.__qualname__}'>"
-
-
-class CommandSet(object, metaclass=CommandSetMeta):
-    __slots__ = ["raw_command_set", "_bound_command_cache"]
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.raw_command_set = self.__class__.generate_raw_commands()
-        self._bound_command_cache = {}
-
-    def get(self, __key: str, default: Optional[Callable] = None) -> Optional[Callable]:
-        """
-        get command in the command set
-
-        NOTE: This method will only try to get its own commands.
-        If you want to get a command as a normal case, use `__getitem__` instead.
-        """
-        cache = self._bound_command_cache.get(__key, None)
-        if cache is not None:
-            return cache
-        raw_cmd = self.raw_command_set.get(__key, default)
-        if raw_cmd is default:
-            return raw_cmd
-        
-        assert raw_cmd
-        bound_cmd = MethodType(raw_cmd, self)
-        self._bound_command_cache[__key] = bound_cmd
-        return bound_cmd
-
-    def check_virtual(self, command: Command) -> bool:
-        return command is self.raw_command_set[command.__name__]
-
-    @classmethod
-    def mask(cls, type: Union["Mask.MType", str] = "") -> "Mask":
-        return ClassTypeMask(cls, type)  # type: ignore
-
-    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds: Any) -> Any:
-        """hook function used to change the calling behavior of the `Command` class
-
-        :param command: the `Command` object being invoked
-        :type command: Command
-        :param args: call positional arguments
-        :type args: Tuple[Any]
-        :param kwargs: call keyword arguments
-        :type kwargs: Dict[str, Any]
-        :return: command return value
-        :rtype: Any
-        """
-        return command.__func__(self, *args, **kwargs)
-
-    def __getitem__(self, __key: str) -> Callable:
-        cmd = self.get(__key)
-        if cmd is None:
-            raise KeyError(f"unknown command '{__key}'")
-        return cmd
-    
-    def __repr__(self) -> str:
-        return f"<kola {self.__class__.__name__} object at 0x{id(self):08X}>"
-
-
-from .mask import Mask, ClassTypeMask
+from abc import ABCMeta
+from types import MethodType
+from typing import Any, Callable, Dict, Optional, Set, Tuple, Type, Union
+from typing_extensions import Self
+
+from .command import CommandLike, Command
+
+
+class CommandSetMeta(ABCMeta):
+    """
+    metaclass for all command sets
+    """
+    __command_field__: Set[CommandLike]
+    __virtual_table__: Dict[str, str]
+
+    def __new__(cls, name: str, bases: Tuple[Type, ...], attr: Dict[str, Any], **kwds: Any) -> Self:
+        command_field = set()
+        virtual_table = attr.get("__virtual_table__", {})
+        for i in bases:
+            if isinstance(i, CommandSetMeta):
+                virtual_table.update(i.__virtual_table__)
+        for k, v in attr.items():
+            if isinstance(v, Command):
+                if v.virtual:
+                    virtual_table[k] = v.__name__
+                elif k in virtual_table:
+                    v.virtual = True
+            elif k in virtual_table:
+                attr[k] = v = Command(virtual_table[k], v, virtual=True)
+            elif not isinstance(v, CommandLike):
+                continue
+            command_field.add(v)
+        attr["__command_field__"] = command_field
+        attr["__virtual_table__"] = virtual_table
+        return super().__new__(cls, name, bases, attr, **kwds)
+
+    def generate_raw_commands(self) -> Dict[str, Any]:
+        cmd_set = {}
+        for cls in reversed(self.__mro__):
+            cls: Type
+            if not isinstance(cls, CommandSetMeta):
+                continue
+            for c in cls.__command_field__:
+                cmd_set.update(c.__kola_command__())
+        return cmd_set
+
+    def _command_register_factory(cmd_name: Optional[str] = None):  # type: ignore
+        def inner(
+            self,
+            __func_or_name: Union[Callable, str, None] = None,
+            **kwds
+        ) -> Union[Callable[[Callable], Command], Command]:
+            def wrapper(wrapped_func: Callable[..., Any]) -> Command:
+                if cmd_name is not None:
+                    assert not isinstance(__func_or_name, str)
+                    name = cmd_name
+                elif isinstance(__func_or_name, str):
+                    name = __func_or_name
+                else:
+                    name = wrapped_func.__name__
+                cmd = Command(name, wrapped_func, **kwds)
+                self.__command_field__.add(cmd)
+                return cmd
+            if callable(__func_or_name):
+                return wrapper(__func_or_name)
+            else:
+                return wrapper
+        return inner
+
+    register_command = _command_register_factory()
+    register_text = _command_register_factory("@text")
+    register_number = _command_register_factory("@number")
+    register_annotation = _command_register_factory("@annotation")
+
+    del _command_register_factory
+    
+    def __repr__(self) -> str:
+        return f"<kola command set '{self.__qualname__}'>"
+
+
+class CommandSet(object, metaclass=CommandSetMeta):
+    __slots__ = ["raw_command_set", "_bound_command_cache"]
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.raw_command_set = self.__class__.generate_raw_commands()
+        self._bound_command_cache = {}
+
+    def get(self, __key: str, default: Optional[Callable] = None) -> Optional[Callable]:
+        """
+        get command in the command set
+
+        NOTE: This method will only try to get its own commands.
+        If you want to get a command as a normal case, use `__getitem__` instead.
+        """
+        cache = self._bound_command_cache.get(__key, None)
+        if cache is not None:
+            return cache
+        raw_cmd = self.raw_command_set.get(__key, default)
+        if raw_cmd is default:
+            return raw_cmd
+        
+        assert raw_cmd
+        bound_cmd = MethodType(raw_cmd, self)
+        self._bound_command_cache[__key] = bound_cmd
+        return bound_cmd
+
+    def check_virtual(self, command: Command) -> bool:
+        return command is self.raw_command_set[command.__name__]
+
+    @classmethod
+    def mask(cls, type: Union["Mask.MType", str] = "") -> "Mask":
+        return ClassTypeMask(cls, type)  # type: ignore
+
+    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds: Any) -> Any:
+        """hook function used to change the calling behavior of the `Command` class
+
+        :param command: the `Command` object being invoked
+        :type command: Command
+        :param args: call positional arguments
+        :type args: Tuple[Any]
+        :param kwargs: call keyword arguments
+        :type kwargs: Dict[str, Any]
+        :return: command return value
+        :rtype: Any
+        """
+        return command.__func__(self, *args, **kwargs)
+
+    def __getitem__(self, __key: str) -> Callable:
+        cmd = self.get(__key)
+        if cmd is None:
+            raise KeyError(f"unknown command '{__key}'")
+        return cmd
+    
+    def __repr__(self) -> str:
+        return f"<kola {self.__class__.__name__} object at 0x{id(self):08X}>"
+
+
+from .mask import Mask, ClassTypeMask
```

### Comparing `KoiLang-1.1.1/kola/klvm/commandset.pyi` & `KoiLang-1.2.0a0/kola/klvm/commandset.pyi`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from abc import ABCMeta
-from typing import (Any, Callable, Dict, Iterable, Optional, Set, Tuple, Union,
-                    overload)
-
-from typing_extensions import Self
-
-from .command import Command, CommandLike
-from .mask import Mask, ClassTypeMask
-
-
-class CommandSetMeta(ABCMeta):
-    __command_field__: Set[CommandLike]
-    __virtual_table__: Dict[str, str]
-
-    def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any], **kwds: Any) -> Self: ...
-    def generate_raw_commands(self) -> Dict[str, Any]: ...
-    @overload
-    def register_command(
-        self, __func: Callable[..., Any], **kwds) -> Command: ...
-    @overload
-    def register_command(
-        self, __name: Optional[str] = ..., *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
-    ) -> Callable[[Callable[..., Any]], Command]: ...
-    @overload
-    def register_text(
-        self, __func: Callable[..., Any], **kwds) -> Command: ...
-    @overload
-    def register_text(
-        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
-    ) -> Callable[[Callable[..., Any]], Command]: ...
-    @overload
-    def register_number(
-        self, __func: Callable[..., Any], **kwds) -> Command: ...
-    @overload
-    def register_number(
-        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
-    ) -> Callable[[Callable[..., Any]], Command]: ...
-    @overload
-    def register_annotation(
-        self, __func: Callable[..., Any], **kwds) -> Command: ...
-    @overload
-    def register_annotation(
-        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
-    ) -> Callable[[Callable[..., Any]], Command]: ...
-    
-
-class CommandSet(metaclass=CommandSetMeta):
-    __slots__ = ["raw_command_set", "_bound_command_cache"]
-
-    raw_command_set: Dict[str, Callable]
-    _bound_command_set: Dict[str, Callable]
-
-    def __init__(self) -> None: ...
-    def check_virtual(self, command: Command) -> bool: ...
-    def get(self, __key: str, default: Optional[Callable] = ...) -> Optional[Callable]: ...
-    @classmethod
-    def mask(cls, type: Union["Mask.MType", str] = "") -> ClassTypeMask: ...
-    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds) -> Any: ...
-    def __getitem__(self, __key: str) -> Callable: ...
+from abc import ABCMeta
+from typing import (Any, Callable, Dict, Iterable, Optional, Set, Tuple, Union,
+                    overload)
+
+from typing_extensions import Self
+
+from .command import Command, CommandLike
+from .mask import Mask, ClassTypeMask
+
+
+class CommandSetMeta(ABCMeta):
+    __command_field__: Set[CommandLike]
+    __virtual_table__: Dict[str, str]
+
+    def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any], **kwds: Any) -> Self: ...
+    def generate_raw_commands(self) -> Dict[str, Any]: ...
+    @overload
+    def register_command(
+        self, __func: Callable[..., Any], **kwds) -> Command: ...
+    @overload
+    def register_command(
+        self, __name: Optional[str] = ..., *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+    ) -> Callable[[Callable[..., Any]], Command]: ...
+    @overload
+    def register_text(
+        self, __func: Callable[..., Any], **kwds) -> Command: ...
+    @overload
+    def register_text(
+        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+    ) -> Callable[[Callable[..., Any]], Command]: ...
+    @overload
+    def register_number(
+        self, __func: Callable[..., Any], **kwds) -> Command: ...
+    @overload
+    def register_number(
+        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+    ) -> Callable[[Callable[..., Any]], Command]: ...
+    @overload
+    def register_annotation(
+        self, __func: Callable[..., Any], **kwds) -> Command: ...
+    @overload
+    def register_annotation(
+        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+    ) -> Callable[[Callable[..., Any]], Command]: ...
+    
+
+class CommandSet(metaclass=CommandSetMeta):
+    __slots__ = ["raw_command_set", "_bound_command_cache"]
+
+    raw_command_set: Dict[str, Callable]
+    _bound_command_set: Dict[str, Callable]
+
+    def __init__(self) -> None: ...
+    def check_virtual(self, command: Command) -> bool: ...
+    def get(self, __key: str, default: Optional[Callable] = ...) -> Optional[Callable]: ...
+    @classmethod
+    def mask(cls, type: Union["Mask.MType", str] = "") -> ClassTypeMask: ...
+    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds) -> Any: ...
+    def __getitem__(self, __key: str) -> Callable: ...
```

### Comparing `KoiLang-1.1.1/kola/klvm/decorator.py` & `KoiLang-1.2.0a0/kola/klvm/decorator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from types import new_class
-from typing import Any, Callable, Optional, Type, Union
-
-from .command import Command
-from .commandset import CommandSet
-from .environment import Environment, EnvironmentEntry, EnvironmentExit
-from .koilang import KoiLang
-
-
-def _kola_decorator_factory(cmd_name: Optional[str] = None, cmd_type: Type[Command] = Command):
-    def kola_decorator(
-        func: Union[Callable[..., Any], str, None] = None,
-        **kwds
-    ) -> Union[Command, Callable[[Callable], Command]]:
-        def wrapper(wrapped_func: Callable[..., Any]) -> Command:
-            nonlocal cmd_type
-            if cmd_name is not None:
-                assert not isinstance(func, str)
-                name = cmd_name
-            elif isinstance(func, str):
-                name = func
-            else:
-                name = wrapped_func.__name__
-            return cmd_type(name, wrapped_func, **kwds)
-        if callable(func):
-            return wrapper(func)
-        else:
-            return wrapper
-    return kola_decorator
-
-
-kola_command = _kola_decorator_factory()
-kola_text = _kola_decorator_factory("@text")
-kola_number = _kola_decorator_factory("@number")
-kola_annotation = _kola_decorator_factory("@annotation")
-kola_env_enter = _kola_decorator_factory(cmd_type=EnvironmentEntry)
-kola_env_exit = _kola_decorator_factory(cmd_type=EnvironmentExit)
-
-
-def _kola_class_decorator_factory(base: Type[CommandSet] = CommandSet):
-    def kola_class_decoractor(kola_cls: Union[Type[KoiLang], str, None] = None, **kwds):
-        def wrapper(wrapped_class: Type) -> Type[CommandSet]:
-            if isinstance(kola_cls, str):
-                env_name = kola_cls
-            else:
-                env_name = wrapped_class.__name__
-            
-            return new_class(
-                env_name,
-                (base,),
-                kwds,
-                lambda attrs: attrs.update(wrapped_class.__dict__)
-            )
-        if isinstance(kola_cls, type):
-            return wrapper(kola_cls)
-        else:
-            return wrapper
-    return kola_class_decoractor
-
-
-kola_command_set = _kola_class_decorator_factory()
-kola_environment = _kola_class_decorator_factory(Environment)
-kola_main = _kola_class_decorator_factory(KoiLang)
+from types import new_class
+from typing import Any, Callable, Optional, Type, Union
+
+from .command import Command
+from .commandset import CommandSet
+from .environment import Environment, EnvironmentEntry, EnvironmentExit
+from .koilang import KoiLang
+
+
+def _kola_decorator_factory(cmd_name: Optional[str] = None, cmd_type: Type[Command] = Command):
+    def kola_decorator(
+        func: Union[Callable[..., Any], str, None] = None,
+        **kwds
+    ) -> Union[Command, Callable[[Callable], Command]]:
+        def wrapper(wrapped_func: Callable[..., Any]) -> Command:
+            nonlocal cmd_type
+            if cmd_name is not None:
+                assert not isinstance(func, str)
+                name = cmd_name
+            elif isinstance(func, str):
+                name = func
+            else:
+                name = wrapped_func.__name__
+            return cmd_type(name, wrapped_func, **kwds)
+        if callable(func):
+            return wrapper(func)
+        else:
+            return wrapper
+    return kola_decorator
+
+
+kola_command = _kola_decorator_factory()
+kola_text = _kola_decorator_factory("@text")
+kola_number = _kola_decorator_factory("@number")
+kola_annotation = _kola_decorator_factory("@annotation")
+kola_env_enter = _kola_decorator_factory(cmd_type=EnvironmentEntry)
+kola_env_exit = _kola_decorator_factory(cmd_type=EnvironmentExit)
+
+
+def _kola_class_decorator_factory(base: Type[CommandSet] = CommandSet):
+    def kola_class_decoractor(kola_cls: Union[Type[KoiLang], str, None] = None, **kwds):
+        def wrapper(wrapped_class: Type) -> Type[CommandSet]:
+            if isinstance(kola_cls, str):
+                env_name = kola_cls
+            else:
+                env_name = wrapped_class.__name__
+            
+            return new_class(
+                env_name,
+                (base,),
+                kwds,
+                lambda attrs: attrs.update(wrapped_class.__dict__)
+            )
+        if isinstance(kola_cls, type):
+            return wrapper(kola_cls)
+        else:
+            return wrapper
+    return kola_class_decoractor
+
+
+kola_command_set = _kola_class_decorator_factory()
+kola_environment = _kola_class_decorator_factory(Environment)
+kola_main = _kola_class_decorator_factory(KoiLang)
```

### Comparing `KoiLang-1.1.1/kola/klvm/decorator.pyi` & `KoiLang-1.2.0a0/kola/klvm/decorator.pyi`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from typing import Any, Callable, Iterable, Optional, Type, overload, Union
-
-from .command import Command
-from .commandset import CommandSet
-from .environment import Environment, EnvironmentEntry, EnvironmentExit
-from .koilang import KoiLang
-
-
-@overload
-def kola_command(func: Callable[..., Any], **kwds: Any) -> Command: ...
-@overload
-def kola_command(
-    func: Optional[str] = None,
-    *,
-    envs: Union[Iterable[str], str] = ...,
-    alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
-    **kwds: Any
-) -> Callable[[Callable[..., Any]], Command]: ...
-@overload
-def kola_text(func: Callable[..., Any], **kwds: Any) -> Command: ...
-@overload
-def kola_text(
-    *,
-    envs: Union[Iterable[str], str] = ...,
-    alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
-    **kwds: Any
-) -> Callable[[Callable[..., Any]], Command]: ...
-@overload
-def kola_number(func: Callable[..., Any], **kwds: Any) -> Command: ...
-@overload
-def kola_number(
-    *,
-    envs: Union[Iterable[str], str] = ...,
-    alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
-    **kwds: Any
-) -> Callable[[Callable[..., Any]], Command]: ...
-@overload
-def kola_annotation(func: Callable[..., Any], **kwds: Any) -> Command: ...
-@overload
-def kola_annotation(
-    *,
-    envs: Union[Iterable[str], str] = ...,
-    alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
-    **kwds: Any
-) -> Callable[[Callable[..., Any]], Command]: ...
-@overload
-def kola_env_enter(func: Callable[..., Any], **kwds: Any) -> EnvironmentEntry: ...
-@overload
-def kola_env_enter(
-    func: Optional[str] = None,
-    *,
-    envs: Union[Iterable[str], str] = ...,
-    alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
-    **kwds: Any
-) -> Callable[[Callable[..., Any]], EnvironmentEntry]: ...
-@overload
-def kola_env_exit(func: Callable[..., Any], **kwds: Any) -> EnvironmentExit: ...
-@overload
-def kola_env_exit(
-    func: Optional[str] = None,
-    *,
-    envs: Union[Iterable[str], str] = ...,
-    alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
-    **kwds: Any
-) -> Callable[[Callable[..., Any]], EnvironmentExit]: ...
-@overload
-def kola_command_set(kola_cls: Type, **kwds: Any) -> Type[CommandSet]: ...
-@overload
-def kola_command_set(kola_cls: Optional[str] = None, **kwds: Any) -> Callable[[Type], Type[CommandSet]]: ...
-@overload
-def kola_environment(kola_cls: Type, **kwds: Any) -> Type[Environment]: ...
-@overload
-def kola_environment(kola_cls: Optional[str] = None, **kwds: Any) -> Callable[[Type], Type[Environment]]: ...
-@overload
-def kola_main(kola_cls: Type, **kwds: Any) -> Type[KoiLang]: ...
-@overload
-def kola_main(kola_cls: Optional[str] = None, **kwds: Any) -> Callable[[Type], Type[KoiLang]]: ...
+from typing import Any, Callable, Iterable, Optional, Type, overload, Union
+
+from .command import Command
+from .commandset import CommandSet
+from .environment import Environment, EnvironmentEntry, EnvironmentExit
+from .koilang import KoiLang
+
+
+@overload
+def kola_command(func: Callable[..., Any], **kwds: Any) -> Command: ...
+@overload
+def kola_command(
+    func: Optional[str] = None,
+    *,
+    envs: Union[Iterable[str], str] = ...,
+    alias: Union[Iterable[str], str] = ...,
+    virtual: bool = False,
+    **kwds: Any
+) -> Callable[[Callable[..., Any]], Command]: ...
+@overload
+def kola_text(func: Callable[..., Any], **kwds: Any) -> Command: ...
+@overload
+def kola_text(
+    *,
+    envs: Union[Iterable[str], str] = ...,
+    alias: Union[Iterable[str], str] = ...,
+    virtual: bool = False,
+    **kwds: Any
+) -> Callable[[Callable[..., Any]], Command]: ...
+@overload
+def kola_number(func: Callable[..., Any], **kwds: Any) -> Command: ...
+@overload
+def kola_number(
+    *,
+    envs: Union[Iterable[str], str] = ...,
+    alias: Union[Iterable[str], str] = ...,
+    virtual: bool = False,
+    **kwds: Any
+) -> Callable[[Callable[..., Any]], Command]: ...
+@overload
+def kola_annotation(func: Callable[..., Any], **kwds: Any) -> Command: ...
+@overload
+def kola_annotation(
+    *,
+    envs: Union[Iterable[str], str] = ...,
+    alias: Union[Iterable[str], str] = ...,
+    virtual: bool = False,
+    **kwds: Any
+) -> Callable[[Callable[..., Any]], Command]: ...
+@overload
+def kola_env_enter(func: Callable[..., Any], **kwds: Any) -> EnvironmentEntry: ...
+@overload
+def kola_env_enter(
+    func: Optional[str] = None,
+    *,
+    envs: Union[Iterable[str], str] = ...,
+    alias: Union[Iterable[str], str] = ...,
+    virtual: bool = False,
+    **kwds: Any
+) -> Callable[[Callable[..., Any]], EnvironmentEntry]: ...
+@overload
+def kola_env_exit(func: Callable[..., Any], **kwds: Any) -> EnvironmentExit: ...
+@overload
+def kola_env_exit(
+    func: Optional[str] = None,
+    *,
+    envs: Union[Iterable[str], str] = ...,
+    alias: Union[Iterable[str], str] = ...,
+    virtual: bool = False,
+    **kwds: Any
+) -> Callable[[Callable[..., Any]], EnvironmentExit]: ...
+@overload
+def kola_command_set(kola_cls: Type, **kwds: Any) -> Type[CommandSet]: ...
+@overload
+def kola_command_set(kola_cls: Optional[str] = None, **kwds: Any) -> Callable[[Type], Type[CommandSet]]: ...
+@overload
+def kola_environment(kola_cls: Type, **kwds: Any) -> Type[Environment]: ...
+@overload
+def kola_environment(kola_cls: Optional[str] = None, **kwds: Any) -> Callable[[Type], Type[Environment]]: ...
+@overload
+def kola_main(kola_cls: Type, **kwds: Any) -> Type[KoiLang]: ...
+@overload
+def kola_main(kola_cls: Optional[str] = None, **kwds: Any) -> Callable[[Type], Type[KoiLang]]: ...
```

### Comparing `KoiLang-1.1.1/kola/klvm/environment.py` & `KoiLang-1.2.0a0/kola/klvm/environment.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-from functools import partial
-from types import TracebackType
-from typing import Any, Callable, Dict, Generator, Iterable, Optional, Set, Tuple, Type, TypeVar, Union, overload
-from typing_extensions import Self
-
-from ..exception import KoiLangError
-
-from .command import Command
-from .commandset import CommandSet, CommandSetMeta
-
-
-T = TypeVar("T")
-
-
-class EnvironmentCommand(Command):
-    __slots__ = ["env_class"]
-
-    def __init__(
-        self,
-        __name: str,
-        func: Callable,
-        env_class: Optional[Type["Environment"]] = None,
-        envs: Union[Iterable[str], str, None] = None,
-        **kwds
-    ) -> None:
-        super().__init__(__name, func, **kwds)
-        if envs:
-            self.extra_data["envs"] = (envs,) if isinstance(envs, str) else tuple(envs)
-        self.env_class = env_class
-    
-    @classmethod
-    def from_command(cls, command: "Command", **kwds: Any) -> Self:
-        if isinstance(command, EnvironmentCommand):
-            kwds["env_class"] = command.env_class
-        return super().from_command(command, **kwds)
-
-
-class EnvironmentEntry(EnvironmentCommand):
-    __slots__ = []
-    
-    def __init__(self, *args, **kwds) -> None:
-        super().__init__(*args, suppression=True, **kwds)
-    
-    def __get__(self, ins: Any, owner: type) -> Any:
-        assert self.env_class
-        if isinstance(ins, self.env_class) and self.env_class.__env_autopop__:
-            return EnvironmentAutopop.from_command(self).__get__(ins, owner)
-        return super().__get__(ins, owner)
-
-    def __call__(self, vmobj: Union["Environment", "KoiLang"], *args: Any, **kwds: Any) -> Any:
-        assert self.env_class
-        home = vmobj.home
-        env = home.push_prepare(self.env_class)
-        ret = super().__call__(env, *args, **kwds)
-        home.push_apply(env)
-        return ret
-
-
-class EnvironmentExit(EnvironmentCommand):
-    __slots__ = []
-
-    def __call__(self, vmobj: "Environment", *args: Any, **kwds: Any) -> Any:
-        home = vmobj.home
-        pop_env = home.pop_prepare(self.env_class)
-        ret = super().__call__(vmobj, *args, **kwds)
-        home.pop_apply(pop_env)
-        return ret
-
-
-class EnvironmentAutopop(EnvironmentCommand):
-    __slots__ = []
-
-    def __call__(self, vmobj: "Environment", *args: Any, **kwds: Any) -> Any:
-        assert self.env_class
-        home = vmobj.home
-
-        cache = home.pop_prepare(self.env_class)
-        home.pop_apply(cache)
-        cache = home.push_prepare(self.env_class)
-        ret = super().__call__(cache, *args, **kwds)
-        home.push_apply(cache)
-        return ret
-
-
-class EnvironmentMeta(CommandSetMeta):
-    __env_entry__: Set[EnvironmentCommand]
-    __env_exit__: Set[EnvironmentCommand]
-
-    def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any], **kwds: Any) -> Self:
-        entry = set()
-        exit = set()
-        
-        # Usually, there are not many entry points and exit points.
-        # Therefore, unlike the attribute `__command_fields__`, they are computed here
-        for i in bases:
-            if not isinstance(i, EnvironmentMeta):
-                continue
-            entry.update(i.__env_entry__)
-            exit.update(i.__env_exit__)
-
-        attr["__env_entry__"] = entry
-        attr["__env_exit__"] = exit
-        new_cls = super().__new__(cls, name, bases, attr, **kwds)
-        
-        for v in attr.values():
-            if not isinstance(v, EnvironmentCommand):
-                continue
-            v.env_class = new_cls  # type: ignore
-            if isinstance(v, EnvironmentEntry):
-                entry.add(v)
-            elif isinstance(v, EnvironmentExit):
-                exit.add(v)
-        return new_cls
-    
-    @property
-    def __env_autopop__(self) -> bool:
-        return not self.__env_exit__
-    
-    def __kola_command__(self) -> Generator[Tuple[str, EnvironmentCommand], None, None]:
-        for i in self.__env_entry__:
-            yield from i.__kola_command__(force=True)
-
-    @overload
-    def __get__(self, ins: Any, owner: type) -> Self: ...
-    @overload  # noqa: E301
-    def __get__(
-        self: Type[T],
-        ins: Union["KoiLang", "Environment"],
-        owner: Union[Type["KoiLang"], Type["Environment"]]
-    ) -> T: ...
-    def __get__(self, ins: Any, owner: type) -> Any:  # noqa: E301
-        if ins is not None and issubclass(owner, CommandSet):
-            home: KoiLang = ins.home
-            cur = home.top
-            while isinstance(cur, Environment):
-                if cur.back is ins and isinstance(cur, self):
-                    return cur
-                cur = cur.back
-            else:
-                if ins is home.top:
-                    return self.EntryPointInterface(self, ins)
-                raise ValueError(f"cannot find env '{self.__name__}' in the {home}")
-        return self
-    
-    class EntryPointInterface:
-        """
-        interface for entry points in Python level
-        """
-        __slots__ = ["__env_class", "__bound_ins"]
-
-        def __init__(self, env_class: "EnvironmentMeta", bound_ins: CommandSet) -> None:
-            self.__env_class = env_class
-            self.__bound_ins = bound_ins
-        
-        def __getattr__(self, __name: str) -> Any:
-            attr = getattr(self.__env_class, __name)
-            if isinstance(attr, EnvironmentEntry):
-                return attr.__get__(self.__bound_ins, self.__bound_ins.__class__)
-            elif isinstance(attr, Command):
-                raise AttributeError(f"cannot fetch command '{__name}' before the environment initialization")
-            raise AttributeError("only entry commands can be accessed through the interface")
-        
-        def __repr__(self) -> str:  # pragma: no cover
-            return f"<kola environment '{self.__env_class.__name__}' entry point command interface>"
-
-
-class Environment(CommandSet, metaclass=EnvironmentMeta):
-    __slots__ = ["back"]
-
-    def __init__(self, back: CommandSet) -> None:
-        if not self.__class__.__env_entry__:
-            raise TypeError(
-                "cannot instantiate an environment that has no entry points"
-            )
-        super().__init__()
-        self.back = back
-
-        if self.__class__.__env_autopop__:
-            # for these have no exit point, use the same name as entry points
-            for c in self.__class__.__env_entry__:
-                self.raw_command_set.update(
-                    EnvironmentAutopop.from_command(c).__kola_command__()
-                )
-
-    def __getitem__(self, __key: str) -> Callable:
-        cmd_set = self
-        cmd = cmd_set.get(__key)
-        while cmd is None:
-            if not isinstance(cmd_set, Environment):
-                raise KeyError(f"unknown command '{__key}'")
-            cmd_set = cmd_set.back
-            cmd = cmd_set.get(__key)
-        return cmd
-    
-    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds: Any) -> Any:
-        return self.home.__kola_caller__(command, args, kwargs, bound_instance=self, **kwds)
-
-    @property
-    def home(self) -> "KoiLang":
-        cmd_set = self
-        while isinstance(cmd_set, Environment):
-            cmd_set = cmd_set.back
-        assert isinstance(cmd_set, KoiLang)
-        return cmd_set
-    
-    def set_up(self, top: CommandSet) -> None:
-        """called before the environment added to the env stack top"""
-
-    def tear_down(self, top: CommandSet) -> None:
-        """called after the environment removed from the env stack top"""
-
-    @partial(Command, "@end")
-    def at_end(self) -> None:
-        """
-        ensure autopop environments properly popped at the end of parsing
-        """
-        if not self.__class__.__env_autopop__:
-            return
-        home = self.home
-        home.pop_apply(home.pop_prepare(self.__class__))
-        home.at_end()
-    
-    @partial(Command, "@exception", virtual=True, suppression=True)
-    def on_exception(self, exc_type: Type[KoiLangError], exc_ins: Optional[KoiLangError], traceback: TracebackType) -> Any:
-        return self.back["@exception"]
-
-
-from .koilang import KoiLang
+from functools import partial
+from types import TracebackType
+from typing import Any, Callable, Dict, Generator, Iterable, Optional, Set, Tuple, Type, TypeVar, Union, overload
+from typing_extensions import Self
+
+from ..exception import KoiLangError
+
+from .command import Command
+from .commandset import CommandSet, CommandSetMeta
+
+
+T = TypeVar("T")
+
+
+class EnvironmentCommand(Command):
+    __slots__ = ["env_class"]
+
+    def __init__(
+        self,
+        __name: str,
+        func: Callable,
+        env_class: Optional[Type["Environment"]] = None,
+        envs: Union[Iterable[str], str, None] = None,
+        **kwds
+    ) -> None:
+        super().__init__(__name, func, **kwds)
+        if envs:
+            self.extra_data["envs"] = (envs,) if isinstance(envs, str) else tuple(envs)
+        self.env_class = env_class
+    
+    @classmethod
+    def from_command(cls, command: "Command", **kwds: Any) -> Self:
+        if isinstance(command, EnvironmentCommand):
+            kwds["env_class"] = command.env_class
+        return super().from_command(command, **kwds)
+
+
+class EnvironmentEntry(EnvironmentCommand):
+    __slots__ = []
+    
+    def __init__(self, *args, **kwds) -> None:
+        super().__init__(*args, suppression=True, **kwds)
+    
+    def __get__(self, ins: Any, owner: type) -> Any:
+        assert self.env_class
+        if isinstance(ins, self.env_class) and self.env_class.__env_autopop__:
+            return EnvironmentAutopop.from_command(self).__get__(ins, owner)
+        return super().__get__(ins, owner)
+
+    def __call__(self, vmobj: Union["Environment", "KoiLang"], *args: Any, **kwds: Any) -> Any:
+        assert self.env_class
+        home = vmobj.home
+        env = home.push_prepare(self.env_class)
+        ret = super().__call__(env, *args, **kwds)
+        home.push_apply(env)
+        return ret
+
+
+class EnvironmentExit(EnvironmentCommand):
+    __slots__ = []
+
+    def __call__(self, vmobj: "Environment", *args: Any, **kwds: Any) -> Any:
+        home = vmobj.home
+        pop_env = home.pop_prepare(self.env_class)
+        ret = super().__call__(vmobj, *args, **kwds)
+        home.pop_apply(pop_env)
+        return ret
+
+
+class EnvironmentAutopop(EnvironmentCommand):
+    __slots__ = []
+
+    def __call__(self, vmobj: "Environment", *args: Any, **kwds: Any) -> Any:
+        assert self.env_class
+        home = vmobj.home
+
+        cache = home.pop_prepare(self.env_class)
+        home.pop_apply(cache)
+        cache = home.push_prepare(self.env_class)
+        ret = super().__call__(cache, *args, **kwds)
+        home.push_apply(cache)
+        return ret
+
+
+class EnvironmentMeta(CommandSetMeta):
+    __env_entry__: Set[EnvironmentCommand]
+    __env_exit__: Set[EnvironmentCommand]
+
+    def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any], **kwds: Any) -> Self:
+        entry = set()
+        exit = set()
+        
+        # Usually, there are not many entry points and exit points.
+        # Therefore, unlike the attribute `__command_fields__`, they are computed here
+        for i in bases:
+            if not isinstance(i, EnvironmentMeta):
+                continue
+            entry.update(i.__env_entry__)
+            exit.update(i.__env_exit__)
+
+        attr["__env_entry__"] = entry
+        attr["__env_exit__"] = exit
+        new_cls = super().__new__(cls, name, bases, attr, **kwds)
+        
+        for v in attr.values():
+            if not isinstance(v, EnvironmentCommand):
+                continue
+            v.env_class = new_cls  # type: ignore
+            if isinstance(v, EnvironmentEntry):
+                entry.add(v)
+            elif isinstance(v, EnvironmentExit):
+                exit.add(v)
+        return new_cls
+    
+    @property
+    def __env_autopop__(self) -> bool:
+        return not self.__env_exit__
+    
+    def __kola_command__(self) -> Generator[Tuple[str, EnvironmentCommand], None, None]:
+        for i in self.__env_entry__:
+            yield from i.__kola_command__(force=True)
+
+    @overload
+    def __get__(self, ins: Any, owner: type) -> Self: ...
+    @overload  # noqa: E301
+    def __get__(
+        self: Type[T],
+        ins: Union["KoiLang", "Environment"],
+        owner: Union[Type["KoiLang"], Type["Environment"]]
+    ) -> T: ...
+    def __get__(self, ins: Any, owner: type) -> Any:  # noqa: E301
+        if ins is not None and issubclass(owner, CommandSet):
+            home: KoiLang = ins.home
+            cur = home.top
+            while isinstance(cur, Environment):
+                if cur.back is ins and isinstance(cur, self):
+                    return cur
+                cur = cur.back
+            else:
+                if ins is home.top:
+                    return self.EntryPointInterface(self, ins)
+                raise ValueError(f"cannot find env '{self.__name__}' in the {home}")
+        return self
+    
+    class EntryPointInterface:
+        """
+        interface for entry points in Python level
+        """
+        __slots__ = ["__env_class", "__bound_ins"]
+
+        def __init__(self, env_class: "EnvironmentMeta", bound_ins: CommandSet) -> None:
+            self.__env_class = env_class
+            self.__bound_ins = bound_ins
+        
+        def __getattr__(self, __name: str) -> Any:
+            attr = getattr(self.__env_class, __name)
+            if isinstance(attr, EnvironmentEntry):
+                return attr.__get__(self.__bound_ins, self.__bound_ins.__class__)
+            elif isinstance(attr, Command):
+                raise AttributeError(f"cannot fetch command '{__name}' before the environment initialization")
+            raise AttributeError("only entry commands can be accessed through the interface")
+        
+        def __repr__(self) -> str:  # pragma: no cover
+            return f"<kola environment '{self.__env_class.__name__}' entry point command interface>"
+
+
+class Environment(CommandSet, metaclass=EnvironmentMeta):
+    __slots__ = ["back"]
+
+    def __init__(self, back: CommandSet) -> None:
+        if not self.__class__.__env_entry__:
+            raise TypeError(
+                "cannot instantiate an environment that has no entry points"
+            )
+        super().__init__()
+        self.back = back
+
+        if self.__class__.__env_autopop__:
+            # for these have no exit point, use the same name as entry points
+            for c in self.__class__.__env_entry__:
+                self.raw_command_set.update(
+                    EnvironmentAutopop.from_command(c).__kola_command__()
+                )
+
+    def __getitem__(self, __key: str) -> Callable:
+        cmd_set = self
+        cmd = cmd_set.get(__key)
+        while cmd is None:
+            if not isinstance(cmd_set, Environment):
+                raise KeyError(f"unknown command '{__key}'")
+            cmd_set = cmd_set.back
+            cmd = cmd_set.get(__key)
+        return cmd
+    
+    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds: Any) -> Any:
+        return self.home.__kola_caller__(command, args, kwargs, bound_instance=self, **kwds)
+
+    @property
+    def home(self) -> "KoiLang":
+        cmd_set = self
+        while isinstance(cmd_set, Environment):
+            cmd_set = cmd_set.back
+        assert isinstance(cmd_set, KoiLang)
+        return cmd_set
+    
+    def set_up(self, top: CommandSet) -> None:
+        """called before the environment added to the env stack top"""
+
+    def tear_down(self, top: CommandSet) -> None:
+        """called after the environment removed from the env stack top"""
+
+    @partial(Command, "@end")
+    def at_end(self) -> None:
+        """
+        ensure autopop environments properly popped at the end of parsing
+        """
+        if not self.__class__.__env_autopop__:
+            return
+        home = self.home
+        home.pop_apply(home.pop_prepare(self.__class__))
+        home.at_end()
+    
+    @partial(Command, "@exception", virtual=True, suppression=True)
+    def on_exception(self, exc_type: Type[KoiLangError], exc_ins: Optional[KoiLangError], traceback: TracebackType) -> Any:
+        return self.back["@exception"]
+
+
+from .koilang import KoiLang
```

### Comparing `KoiLang-1.1.1/kola/klvm/koilang.py` & `KoiLang-1.2.0a0/kola/klvm/koilang.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,314 +1,319 @@
-import os
-import sys
-from contextlib import contextmanager, suppress
-from functools import partial
-from threading import Lock
-from types import TracebackType, new_class
-from typing import (Any, Callable, Dict, Generator, List, Optional, Tuple,
-                    Type, TypeVar, Union, overload)
-from typing_extensions import Literal, Self
-
-from ..exception import KoiLangError
-from ..lexer import BaseLexer, FileLexer, StringLexer
-from ..parser import Parser
-from .command import Command
-from .commandset import CommandSet, CommandSetMeta
-from .environment import Environment
-
-
-_T_EnvCls = TypeVar("_T_EnvCls", bound=Type[Environment])
-_T_Handler = TypeVar("_T_Handler", bound=Type["AbstractHandler"])
-
-
-class KoiLangMeta(CommandSetMeta):
-    """
-    metaclass for KoiLang class
-
-    Provide encoding and command threshold support.
-    """
-    __text_encoding__: str
-    __text_lstrip__: bool
-    __command_threshold__: int
-    __command_handlers__: List[Type["AbstractHandler"]]
-
-    def __new__(
-        cls,
-        name: str,
-        bases: Tuple[type, ...],
-        attr: Dict[str, Any],
-        command_threshold: int = 0,
-        encoding: Optional[str] = None,
-        lstrip_text: Optional[bool] = None,
-        **kwds: Any
-    ) -> Self:
-        """
-        create a top-level language class
-
-        :param name: class name
-        :type name: str
-        :param bases: class bases
-        :type bases: Tuple[type, ...]
-        :param attr: class namespace
-        :type attr: Dict[str, Any]
-        :param command_threshold: the `#` prefix length of commands, defaults to 0
-        :type command_threshold: int, optional
-        :param encoding: encoding for file parsing, defaults to None
-        :type encoding: Optional[str], optional
-        :param lstrip_text: whether to remove text indentation, defaults to True
-        :type lstrip_text: bool, optional
-        :return: new class
-        :rtype: KoiLangMeta
-        """
-        # if not base KoiLang class, set a default value
-        if not any(isinstance(i, cls) for i in bases):
-            command_threshold = command_threshold or 1
-            encoding = encoding or "utf-8"
-            lstrip_text = lstrip_text if lstrip_text is not None else True
-            if "__command_handlers__" not in attr:
-                attr["__command_handlers__"] = []
-        
-        if command_threshold:
-            assert command_threshold >= 0
-            attr["__command_threshold__"] = command_threshold
-        if lstrip_text is not None:
-            attr["__text_lstrip__"] = lstrip_text
-        if encoding:
-            attr["__text_encoding__"] = encoding
-        return super().__new__(cls, name, bases, attr, **kwds)
-
-    def register_environment(self, env_class: _T_EnvCls) -> _T_EnvCls:
-        self.__command_field__.add(env_class)
-        return env_class
-    
-    def register_handler(self, handler: _T_Handler) -> _T_Handler:
-        if "__command_handlers__" not in self.__dict__:
-            # copy the handler list to avoid changing the base classes
-            self.__command_handlers__ = self.__command_handlers__.copy()
-        self.__command_handlers__.append(handler)
-        return handler
-    
-    @property
-    def writer(self) -> Type:
-        """writer class for KoiLang file building
-
-        :return: the writer class, which is a subclass of KoiLangWriter and current KoiLang class
-        :rtype: Type[KoiLang, Self]
-        """
-        cache = None
-        with suppress(AttributeError):
-            cache = self.__writer_class
-        if cache is not None:
-            return cache
-        cache = new_class(f"{self.__qualname__}.writer", (KoiLangWriter, self))
-        self.__writer_class = cache
-        return cache
-
-
-class KoiLang(CommandSet, metaclass=KoiLangMeta):
-    """
-    main class for KoiLang virtual machine
-
-    `KoiLang` class is the top-level interface of 'kola' package.
-    Just create a subclass to define your own markup language based on KoiLang.
-    """
-    __slots__ = ["_handler", "_lock", "__top", "__exec_level"]
-
-    def __init__(self) -> None:
-        super().__init__()
-        self._lock = Lock()
-        self.__top = self
-        self.__exec_level = 0
-        self._handler = build_handlers(self.__class__.__command_handlers__, self)
-    
-    def push_prepare(self, __env_type: Type[Environment]) -> Environment:
-        env = __env_type(self.__top)
-        env.set_up(self.__top)
-        return env
-
-    def push_apply(self, __env_cache: Environment) -> None:
-        assert __env_cache.back is self.__top
-        with self._lock:
-            self.__top = __env_cache
-    
-    def pop_prepare(self, __env_type: Optional[Type[Environment]] = None) -> Environment:
-        top = self.__top
-        if top is self:  # pragma: no cover
-            raise ValueError('cannot pop the inital environment')
-        if __env_type is None:
-            assert isinstance(top, Environment)
-        else:
-            while isinstance(top, Environment) and top.__class__.__env_autopop__:
-                if isinstance(top, __env_type):
-                    break
-                top = top.back
-            else:
-                if not isinstance(top, __env_type):  # pragma: no cover
-                    raise ValueError("unmatched environment")
-        return top
-
-    def pop_apply(self, __env_cache: Environment) -> None:
-        with self._lock:
-            top = self.__top
-            self.__top = __env_cache.back
-        while isinstance(top, Environment):
-            top.tear_down(self.__top)
-            if top is __env_cache:
-                break
-            top = top.back
-        else:
-            raise ValueError('cannot pop the inital environment')
-    
-    def add_handler(self, handler: Union[Type["AbstractHandler"], "AbstractHandler"]) -> "AbstractHandler":
-        if isinstance(handler, type):
-            handler = handler(self)
-        self._handler = self._handler.insert(handler)
-        return handler
-    
-    def remove_handler(self, handler: "AbstractHandler") -> None:
-        hdl = self._handler.remove(handler)
-        if hdl is None:  # pragma: no cover
-            raise ValueError("cannot remove all handlers")
-        self._handler = hdl
-
-    def __parse(self, __lexer: BaseLexer, *, close_lexer: bool = True) -> None:
-        parser = Parser(__lexer, self)
-        try:
-            with self.exec_block():
-                while True:
-                    try:
-                        # Parser.exec() is a fast C level loop
-                        parser.exec()
-                    except KoiLangError:
-                        if not self.on_exception(*sys.exc_info()):
-                            raise
-                    else:
-                        break
-        finally:
-            if close_lexer:
-                __lexer.close()
-    
-    def __parse_and_ret(self, __lexer: BaseLexer, *, close_lexer: bool = True) -> Generator[Any, None, None]:
-        parser = Parser(__lexer, self)
-        try:
-            with self.exec_block():
-                while True:
-                    try:
-                        yield from parser
-                    except KoiLangError:
-                        if not self.on_exception(*sys.exc_info()):
-                            raise
-                    else:
-                        break
-        finally:
-            if close_lexer:
-                __lexer.close()
-
-    @overload
-    def parse(self, lexer: Union[BaseLexer, str], *, with_ret: Literal[False] = False, close_lexer: bool = True) -> None: ...
-    @overload  # noqa: E301
-    def parse(
-        self,
-        lexer: Union[BaseLexer, str],
-        *,
-        with_ret: Literal[True],
-        close_lexer: bool = True
-    ) -> Generator[Any, None, None]: ...
-    
-    def parse(self, lexer: Union[BaseLexer, str], *, with_ret: bool = False, close_lexer: bool = True) -> Any:
-        """parse kola text
-
-        :param lexer: Lexer object or legal KoiLang string
-        :type lexer: Union[BaseLexer, str]
-        :param with_ret: if true, return a gererater where command returns would be yielded, defaults to False
-        :type with_ret: bool, optional
-        :param close_lexer: whether or not to close the lexer, defaults to True
-        :type close_lexer: bool, optional
-        :raises ValueError: when a KoiLang string given without trying to close it
-        :return: return a generator if `with_ret` set
-        :rtype: Generator[Any, None, None] or None
-        """
-        if isinstance(lexer, str):
-            if not close_lexer:  # pragma: no cover
-                raise ValueError("inner string lexer must be closed at the end of parsing")
-            lexer = StringLexer(
-                lexer,
-                encoding=self.__class__.__text_encoding__,
-                command_threshold=self.__class__.__command_threshold__,
-                no_lstrip=not self.__class__.__text_lstrip__
-            )
-        if with_ret:
-            return self.__parse_and_ret(lexer, close_lexer=close_lexer)
-        else:
-            self.__parse(lexer, close_lexer=close_lexer)
-        
-    def parse_file(self, path: Union[str, bytes, os.PathLike], *, encoding: Optional[str] = None, **kwds: Any) -> Any:
-        """
-        parse a kola file.
-        """
-        return self.parse(
-            FileLexer(
-                path, encoding=encoding or self.__class__.__text_encoding__,
-                command_threshold=self.__class__.__command_threshold__,
-                no_lstrip=not self.__class__.__text_lstrip__
-            ), **kwds
-        )
-    
-    @contextmanager
-    def exec_block(self) -> Generator[Self, None, None]:
-        if not self.__exec_level:
-            self.at_start()
-        with self._lock:
-            self.__exec_level += 1
-        try:
-            yield self
-        finally:
-            with self._lock:
-                self.__exec_level -= 1
-            if not self.__exec_level:
-                self.at_end()
-
-    def __getitem__(self, __key: str) -> Callable:
-        if self.__top is self:
-            return super().__getitem__(__key)
-        return self.__top[__key]
-
-    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds: Any) -> Any:
-        return self._handler(command, args, kwargs, **kwds)
-
-    @property
-    def top(self) -> CommandSet:
-        return self.__top
-    
-    @property
-    def home(self) -> Self:
-        return self
-
-    @partial(Command, "@start", virtual=True)
-    def at_start(self) -> None:
-        """
-        parser initalize command
-        
-        It is called before parsing start.
-        """
-
-    @partial(Command, "@end", virtual=True)
-    def at_end(self) -> None:
-        """
-        parser finalize command
-        
-        It is called after parsing end. And the return value
-        will be that of 'parse' method.
-        """
-    
-    @partial(Command, "@exception", virtual=True)
-    def on_exception(self, exc_type: Type[KoiLangError], exc_ins: Optional[KoiLangError], traceback: TracebackType) -> None:
-        """
-        exception handling command
-
-        It is called when a KoiLang error occurs.
-        If the command wishes to suppress the exception, it should a true value.
-        """
-
-
-from .handler import AbstractHandler, build_handlers
-from .writer import KoiLangWriter
+import os
+import sys
+from contextlib import contextmanager, suppress
+from functools import partial
+from threading import Lock
+from types import TracebackType, new_class
+from typing import (Any, Callable, Dict, Generator, List, Optional, Tuple,
+                    Type, TypeVar, Union, overload)
+from typing_extensions import Literal, Self
+
+from ..exception import KoiLangError
+from ..lexer import BaseLexer, FileLexer, StringLexer
+from ..parser import Parser
+from .command import Command
+from .commandset import CommandSet, CommandSetMeta
+from .environment import Environment
+
+
+_T_EnvCls = TypeVar("_T_EnvCls", bound=Type[Environment])
+_T_Handler = TypeVar("_T_Handler", bound=Type["AbstractHandler"])
+
+
+class KoiLangMeta(CommandSetMeta):
+    """
+    metaclass for KoiLang class
+
+    Provide encoding and command threshold support.
+    """
+    __text_encoding__: str
+    __text_lstrip__: bool
+    __command_threshold__: int
+    __command_handlers__: List[Type["AbstractHandler"]]
+
+    def __new__(
+        cls,
+        name: str,
+        bases: Tuple[type, ...],
+        attr: Dict[str, Any],
+        command_threshold: int = 0,
+        encoding: Optional[str] = None,
+        lstrip_text: Optional[bool] = None,
+        **kwds: Any
+    ) -> Self:
+        """
+        create a top-level language class
+
+        :param name: class name
+        :type name: str
+        :param bases: class bases
+        :type bases: Tuple[type, ...]
+        :param attr: class namespace
+        :type attr: Dict[str, Any]
+        :param command_threshold: the `#` prefix length of commands, defaults to 0
+        :type command_threshold: int, optional
+        :param encoding: encoding for file parsing, defaults to None
+        :type encoding: Optional[str], optional
+        :param lstrip_text: whether to remove text indentation, defaults to True
+        :type lstrip_text: bool, optional
+        :return: new class
+        :rtype: KoiLangMeta
+        """
+        # if not base KoiLang class, set a default value
+        if not any(isinstance(i, cls) for i in bases):
+            command_threshold = command_threshold or 1
+            encoding = encoding or "utf-8"
+            lstrip_text = lstrip_text if lstrip_text is not None else True
+            if "__command_handlers__" not in attr:
+                attr["__command_handlers__"] = []
+        
+        if command_threshold:
+            assert command_threshold >= 0
+            attr["__command_threshold__"] = command_threshold
+        if lstrip_text is not None:
+            attr["__text_lstrip__"] = lstrip_text
+        if encoding:
+            attr["__text_encoding__"] = encoding
+        return super().__new__(cls, name, bases, attr, **kwds)
+
+    def register_environment(self, env_class: _T_EnvCls) -> _T_EnvCls:
+        self.__command_field__.add(env_class)
+        return env_class
+    
+    def register_handler(self, handler: _T_Handler) -> _T_Handler:
+        if "__command_handlers__" not in self.__dict__:
+            # copy the handler list to avoid changing the base classes
+            self.__command_handlers__ = self.__command_handlers__.copy()
+        self.__command_handlers__.append(handler)
+        return handler
+    
+    @property
+    def writer(self) -> Type:
+        """writer class for KoiLang file building
+
+        :return: the writer class, which is a subclass of KoiLangWriter and current KoiLang class
+        :rtype: Type[KoiLang, Self]
+        """
+        # sourcery skip: inline-immediately-returned-variable
+        cache = None
+        with suppress(AttributeError):
+            cache = self.__writer_class
+            return cache
+        cache = new_class(f"{self.__qualname__}.writer", (KoiLangWriter, self))
+        self.__writer_class = cache
+        return cache
+
+
+class KoiLang(CommandSet, metaclass=KoiLangMeta):
+    """
+    main class for KoiLang virtual machine
+
+    `KoiLang` class is the top-level interface of 'kola' package.
+    Just create a subclass to define your own markup language based on KoiLang.
+    """
+    __slots__ = ["_handler", "_lock", "__top", "__exec_level"]
+
+    def __init__(self) -> None:
+        super().__init__()
+        self._lock = Lock()
+        self.__top = self
+        self.__exec_level = 0
+        self._handler = build_handlers(self.__class__.__command_handlers__, self)
+    
+    def push_prepare(self, __env_type: Union[Type[Environment], Environment]) -> Environment:
+        if not isinstance(__env_type, Environment):
+            __env_type = __env_type(self.__top)
+        __env_type.set_up(self.__top)
+        return __env_type
+
+    def push_apply(self, __env_cache: Environment) -> None:
+        assert __env_cache.back is self.__top
+        with self._lock:
+            self.__top = __env_cache
+    
+    def pop_prepare(self, __env_type: Optional[Type[Environment]] = None) -> Environment:
+        top = self.__top
+        if top is self:  # pragma: no cover
+            raise ValueError('cannot pop the inital environment')
+        if __env_type is None:
+            assert isinstance(top, Environment)
+        else:
+            while isinstance(top, Environment) and top.__class__.__env_autopop__:
+                if isinstance(top, __env_type):
+                    break
+                top = top.back
+            else:
+                if not isinstance(top, __env_type):  # pragma: no cover
+                    raise ValueError("unmatched environment")
+        return top
+
+    def pop_apply(self, __env_cache: Environment) -> None:
+        with self._lock:
+            top = self.__top
+            self.__top = __env_cache.back
+        while isinstance(top, Environment):
+            top.tear_down(self.__top)
+            if top is __env_cache:
+                break
+            top = top.back
+        else:
+            raise ValueError('cannot pop the inital environment')
+    
+    def add_handler(self, handler: Union[Type["AbstractHandler"], "AbstractHandler"]) -> "AbstractHandler":
+        if isinstance(handler, type):
+            handler = handler(self)
+        self._handler = self._handler.insert(handler)
+        return handler
+    
+    def remove_handler(self, handler: "AbstractHandler") -> None:
+        hdl = self._handler.remove(handler)
+        if hdl is None:  # pragma: no cover
+            raise ValueError("cannot remove all handlers")
+        self._handler = hdl
+
+    def __parse(self, __lexer: BaseLexer, *, close_lexer: bool = True) -> None:
+        parser = Parser(__lexer, self)
+        try:
+            with self.exec_block():
+                while True:
+                    try:
+                        # Parser.exec() is a fast C level loop
+                        parser.exec()
+                    except KoiLangError:
+                        if not self.on_exception(*sys.exc_info()):
+                            raise
+                    else:
+                        break
+        finally:
+            if close_lexer:
+                __lexer.close()
+    
+    def __parse_and_ret(self, __lexer: BaseLexer, *, close_lexer: bool = True) -> Generator[Any, None, None]:
+        parser = Parser(__lexer, self)
+        try:
+            with self.exec_block():
+                while True:
+                    try:
+                        yield from parser
+                    except KoiLangError:
+                        if not self.on_exception(*sys.exc_info()):
+                            raise
+                    else:
+                        break
+        finally:
+            if close_lexer:
+                __lexer.close()
+
+    @overload
+    def parse(self, lexer: Union[BaseLexer, str], *, with_ret: Literal[False] = False, close_lexer: bool = True) -> None: ...
+    @overload  # noqa: E301
+    def parse(
+        self,
+        lexer: Union[BaseLexer, str],
+        *,
+        with_ret: Literal[True],
+        close_lexer: bool = True
+    ) -> Generator[Any, None, None]: ...
+    
+    def parse(self, lexer: Union[BaseLexer, str], *, with_ret: bool = False, close_lexer: bool = True) -> Any:
+        """parse kola text
+
+        :param lexer: Lexer object or legal KoiLang string
+        :type lexer: Union[BaseLexer, str]
+        :param with_ret: if true, return a gererater where command returns would be yielded, defaults to False
+        :type with_ret: bool, optional
+        :param close_lexer: whether or not to close the lexer, defaults to True
+        :type close_lexer: bool, optional
+        :raises ValueError: when a KoiLang string given without trying to close it
+        :return: return a generator if `with_ret` set
+        :rtype: Generator[Any, None, None] or None
+        """
+        if isinstance(lexer, str):
+            if not close_lexer:  # pragma: no cover
+                raise ValueError("inner string lexer must be closed at the end of parsing")
+            lexer = StringLexer(
+                lexer,
+                encoding=self.__class__.__text_encoding__,
+                command_threshold=self.__class__.__command_threshold__,
+                no_lstrip=not self.__class__.__text_lstrip__
+            )
+        if with_ret:
+            return self.__parse_and_ret(lexer, close_lexer=close_lexer)
+        else:
+            self.__parse(lexer, close_lexer=close_lexer)
+        
+    def parse_file(self, path: Union[str, bytes, os.PathLike], *, encoding: Optional[str] = None, **kwds: Any) -> Any:
+        """
+        parse a kola file.
+        """
+        return self.parse(
+            FileLexer(
+                path, encoding=encoding or self.__class__.__text_encoding__,
+                command_threshold=self.__class__.__command_threshold__,
+                no_lstrip=not self.__class__.__text_lstrip__
+            ), **kwds
+        )
+    
+    @contextmanager
+    def exec_block(self) -> Generator[Self, None, None]:
+        if not self.__exec_level:
+            self.at_start()
+        with self._lock:
+            self.__exec_level += 1
+        try:
+            yield self
+        finally:
+            with self._lock:
+                self.__exec_level -= 1
+            if not self.__exec_level:
+                self.at_end()
+
+    def __getitem__(self, __key: str) -> Callable:
+        if self.__top is self:
+            return super().__getitem__(__key)
+        return self.__top[__key]
+
+    def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds: Any) -> Any:
+        return self._handler(command, args, kwargs, **kwds)
+
+    @property
+    def top(self) -> CommandSet:
+        return self.__top
+    
+    @property
+    def home(self) -> Self:
+        return self
+    
+    @property
+    def handlers(self) -> "HandlerSequence":
+        return HandlerSequence(self._handler)
+
+    @partial(Command, "@start", virtual=True)
+    def at_start(self) -> None:
+        """
+        parser initalize command
+        
+        It is called before parsing start.
+        """
+
+    @partial(Command, "@end", virtual=True)
+    def at_end(self) -> None:
+        """
+        parser finalize command
+        
+        It is called after parsing end. And the return value
+        will be that of 'parse' method.
+        """
+    
+    @partial(Command, "@exception", virtual=True)
+    def on_exception(self, exc_type: Type[KoiLangError], exc_ins: Optional[KoiLangError], traceback: TracebackType) -> None:
+        """
+        exception handling command
+
+        It is called when a KoiLang error occurs.
+        If the command wishes to suppress the exception, it should a true value.
+        """
+
+
+from .handler import AbstractHandler, HandlerSequence, build_handlers
+from .writer import KoiLangWriter
```

### Comparing `KoiLang-1.1.1/kola/klvm/mask.py` & `KoiLang-1.2.0a0/kola/klvm/mask.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from abc import ABC, abstractmethod
-from enum import Enum
-from typing import Any, Type, Union
-
-
-from .commandset import CommandSet
-
-
-class Mask(ABC):
-    __slots__ = ["type", "not_"]
-
-    class MType(Enum):
-        default = ""    # test all reachable env
-        exact = "+"     # test top env
-        all = "*"      # test all env
-
-    def __init__(self, type: Union[MType, str] = MType.default, not_: bool = False) -> None:
-        if isinstance(type, str):
-            type = self.MType(type)
-        self.type = type
-        self.not_ = not_
-
-    @abstractmethod
-    def __contains__(self, other: Any) -> bool:
-        raise NotImplementedError
-
-
-class ClassTypeMask(Mask):
-    __slots__ = ["env_type"]
-
-    def __init__(
-        self,
-        env_type: Type[CommandSet],
-        type: Union[Mask.MType, str] = Mask.MType.default,
-        not_: bool = False
-    ) -> None:
-        self.env_type = env_type
-        super().__init__(type=type, not_=not_)
-    
-    def __contains__(self, other: Any) -> bool:
-        return isinstance(other, self.env_type)
-
-
-class ClassNameMask(Mask):
-    __slots__ = ["env_name"]
-
-    def __init__(
-        self,
-        env_name: str,
-        type: Union[Mask.MType, str, None] = None,
-        not_: bool = False,
-        **kwds: CommandSet
-    ) -> None:
-        if env_name.startswith('!'):
-            env_name = env_name[1:]
-            not_ = True
-        if type is None:
-            if env_name.startswith('+'):
-                env_name = env_name[1:]
-                type = Mask.MType.exact
-            elif env_name.startswith('*'):
-                env_name = env_name[1:]
-                type = Mask.MType.all
-            else:
-                type = Mask.MType.default
-        elif env_name[0] in ('+', '*'):
-            raise ValueError(
-                "the name prefix should not be used to specify the type when the Mask type is specified"
-            )
-        if env_name.startswith('$'):
-            name = env_name[1:]
-            if name in kwds:
-                env_name = kwds[name].__class__.__name__
-        elif env_name == "__init__":
-            env_name = kwds["__init__"].__class__.__name__
-        self.env_name = env_name
-        super().__init__(type=type, not_=not_)
-    
-    def __contains__(self, other: Any) -> bool:
-        return self.env_name == other.__class__.__name__
+from abc import ABC, abstractmethod
+from enum import Enum
+from typing import Any, Type, Union
+
+
+from .commandset import CommandSet
+
+
+class Mask(ABC):
+    __slots__ = ["type", "not_"]
+
+    class MType(Enum):
+        default = ""    # test all reachable env
+        exact = "+"     # test top env
+        all = "*"      # test all env
+
+    def __init__(self, type: Union[MType, str] = MType.default, not_: bool = False) -> None:
+        if isinstance(type, str):
+            type = self.MType(type)
+        self.type = type
+        self.not_ = not_
+
+    @abstractmethod
+    def __contains__(self, other: Any) -> bool:
+        raise NotImplementedError
+
+
+class ClassTypeMask(Mask):
+    __slots__ = ["env_type"]
+
+    def __init__(
+        self,
+        env_type: Type[CommandSet],
+        type: Union[Mask.MType, str] = Mask.MType.default,
+        not_: bool = False
+    ) -> None:
+        self.env_type = env_type
+        super().__init__(type=type, not_=not_)
+    
+    def __contains__(self, other: Any) -> bool:
+        return isinstance(other, self.env_type)
+
+
+class ClassNameMask(Mask):
+    __slots__ = ["env_name"]
+
+    def __init__(
+        self,
+        env_name: str,
+        type: Union[Mask.MType, str, None] = None,
+        not_: bool = False,
+        **kwds: CommandSet
+    ) -> None:
+        if env_name.startswith('!'):
+            env_name = env_name[1:]
+            not_ = True
+        if type is None:
+            if env_name.startswith('+'):
+                env_name = env_name[1:]
+                type = Mask.MType.exact
+            elif env_name.startswith('*'):
+                env_name = env_name[1:]
+                type = Mask.MType.all
+            else:
+                type = Mask.MType.default
+        elif env_name[0] in ('+', '*'):
+            raise ValueError(
+                "the name prefix should not be used to specify the type when the Mask type is specified"
+            )
+        if env_name.startswith('$'):
+            name = env_name[1:]
+            if name in kwds:
+                env_name = kwds[name].__class__.__name__
+        elif env_name == "__init__":
+            env_name = kwds["__init__"].__class__.__name__
+        self.env_name = env_name
+        super().__init__(type=type, not_=not_)
+    
+    def __contains__(self, other: Any) -> bool:
+        return self.env_name == other.__class__.__name__
```

### Comparing `KoiLang-1.1.1/kola/lexer.c` & `KoiLang-1.2.0a0/kola/lexer.c`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.1/kola/lexer.pxd` & `KoiLang-1.2.0a0/kola/lexer.pxd`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-cimport cython
-from libc.stdio cimport stdin, FILE, fopen, fclose, EOF
-from cpython cimport PyObject
-
-from ._cutil cimport *
-
-
-cdef extern from *:
-    bint PyDescr_IsData(object desc)
-
-
-cdef class Token:
-    cdef:
-        Token next     # used in grammar parser
-    cdef readonly:
-        TokenSyn syn
-        object val
-        bytes raw_val
-        int lineno
-    
-    cpdef int get_flag(self)
-
-
-cdef class LexerConfig:
-    cdef LexerData* lexer_data
-    cdef readonly BaseLexer lexer
-
-
-@cython.no_gc
-cdef class BaseLexer:
-    cdef:
-        yyscan_t scanner
-        LexerData lexer_data
-    cdef readonly:
-        str encoding
-
-    cpdef void close(self)
-    cdef void set_error(self, const char* text) except *
-    cdef (int, const char*, Py_ssize_t) next_syn(self) nogil
-    cdef Token next_token(self)
-
-
-cdef class FileLexer(BaseLexer):
-    cdef:
-        object _filenameo
-        bytes _filenameb
-        FILE* fp
-    
-    cpdef void close(self)
-
-
-@cython.no_gc
-cdef class StringLexer(BaseLexer):
+cimport cython
+from libc.stdio cimport stdin, FILE, fopen, fclose, EOF
+from cpython cimport PyObject
+
+from ._cutil cimport *
+
+
+cdef extern from *:
+    bint PyDescr_IsData(object desc)
+
+
+cdef class Token:
+    cdef:
+        Token next     # used in grammar parser
+    cdef readonly:
+        TokenSyn syn
+        object val
+        bytes raw_val
+        int lineno
+    
+    cpdef int get_flag(self)
+
+
+cdef class LexerConfig:
+    cdef LexerData* lexer_data
+    cdef readonly BaseLexer lexer
+
+
+@cython.no_gc
+cdef class BaseLexer:
+    cdef:
+        yyscan_t scanner
+        LexerData lexer_data
+    cdef readonly:
+        str encoding
+
+    cpdef void close(self)
+    cdef void set_error(self, const char* text) except *
+    cdef (int, const char*, Py_ssize_t) next_syn(self) nogil
+    cdef Token next_token(self)
+
+
+cdef class FileLexer(BaseLexer):
+    cdef:
+        object _filenameo
+        bytes _filenameb
+        FILE* fp
+    
+    cpdef void close(self)
+
+
+@cython.no_gc
+cdef class StringLexer(BaseLexer):
     cdef readonly bytes content
```

### Comparing `KoiLang-1.1.1/kola/lib/__init__.py` & `KoiLang-1.2.0a0/kola/lib/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-"""
-Kola sub libraries support modules
-
-Include some useful builtin kola sub module.
-And modules imported from `load_library()` will be mounted as a sub module.
-"""
-
-import inspect
-import os
-import re
-import sys
-from glob import glob
-from importlib.util import spec_from_file_location
-from importlib._bootstrap import _load
-from types import ModuleType
-from typing import List, NamedTuple, Optional, Type
-
-from ..klvm import CommandSetMeta, KoiLang
-
-
-if "KOLA_LIB_PATH" in os.environ:  # pragma: no cover
-    KOLA_LIB_PATH = os.environ["KOLA_LIB_PATH"].split(os.pathsep)
-else:
-    KOLA_LIB_PATH = ['.', './kola_lib', os.path.dirname(__file__)]
-
-
-_module_pattern = re.compile(r"^[A-Za-z_]\w*(?:\.[A-Za-z_]\w*)*$", re.A)
-
-
-class KolaSpec(NamedTuple):
-    """
-    Kola module spec
-    
-    Usage:
-        __kola_spec__ = KolaSpec(
-            __name__,
-            collect_all()
-        )
-    """
-    name: str
-    command_set_classes: List[CommandSetMeta]
-    
-    doc: Optional[str] = None
-    main_class: Optional[Type[KoiLang]] = None
-
-
-def collect_all() -> List[CommandSetMeta]:
-    """get all CommandSet class defined in the module
-
-    :return: a list of CommandSet class found
-    :rtype: List[CommandSetMeta]
-    """
-    frame = inspect.currentframe()
-    if not frame or not frame.f_back:  # pragma: no cover
-        raise ValueError("cannot read variables from the frame")
-    return [
-        i for i in frame.f_back.f_locals.values()
-        if isinstance(i, CommandSetMeta)
-    ]
-
-
-def load_library(name: str, paths: List[str] = KOLA_LIB_PATH) -> ModuleType:
-    """load a Phython script or package as a Kola module
-
-    :param name: module name like 'mymodule.sub'
-    :type name: str
-    :param paths: base path to load the module, defaults to KOLA_LIB_PATH
-    :type paths: List[str], optional
-    :raises ValueError: illegal module name
-    :raises ImportError: fail to load the module
-    :return: the Kola module
-    :rtype: ModuleType
-    """
-    if not _module_pattern.match(name):  # pragma: no cover
-        raise ValueError(f"illegal module name '{name}'")
-    module_name = "kola.lib." + name
-    if module_name in sys.modules:
-        return sys.modules[module_name]
-
-    for b in paths:
-        spec = None
-        b = os.path.abspath(b)
-        full_path = os.path.join(b, name)
-        if os.path.isdir(full_path):
-            spec = spec_from_file_location(
-                module_name, os.path.join(full_path, "__init__.py"),
-                submodule_search_locations=[full_path]
-            )
-        else:
-            for i in glob(full_path + '.*'):
-                spec = spec_from_file_location(module_name, i)
-                if spec:
-                    full_path = i
-                    break
-        if spec:
-            spec.name = module_name
-            return _load(spec)
-    raise ImportError(f"cannot load script {name}", name=name)  # pragma: no cover
-
-
-def main_class_from_module(module: ModuleType) -> Type[KoiLang]:
-    spec = getattr(module, "__kola_spec__", None)
-    if spec:
-        if not isinstance(spec, KolaSpec):
-            spec = KolaSpec(*spec)
-        if spec.main_class:
-            return spec.main_class
-        for i in spec.command_set_classes:
-            if issubclass(i, KoiLang):
-                return i
-    else:
-        for i in module.__dict__.values():
-            if isinstance(i, type) and issubclass(i, KoiLang) and i is not KoiLang:
-                return i
-    raise ValueError(  # pragma: no cover
-        f"no available main class for kola module '{spec.name if spec else module.__name__}'"
-    )
+"""
+Kola sub libraries support modules
+
+Include some useful builtin kola sub module.
+And modules imported from `load_library()` will be mounted as a sub module.
+"""
+
+import inspect
+import os
+import re
+import sys
+from glob import glob
+from importlib.util import spec_from_file_location
+from importlib._bootstrap import _load
+from types import ModuleType
+from typing import List, NamedTuple, Optional, Type
+
+from ..klvm import CommandSetMeta, KoiLang
+
+
+if "KOLA_LIB_PATH" in os.environ:  # pragma: no cover
+    KOLA_LIB_PATH = os.environ["KOLA_LIB_PATH"].split(os.pathsep)
+else:
+    KOLA_LIB_PATH = ['.', './kola_lib', os.path.dirname(__file__)]
+
+
+_module_pattern = re.compile(r"^[A-Za-z_]\w*(?:\.[A-Za-z_]\w*)*$", re.A)
+
+
+class KolaSpec(NamedTuple):
+    """
+    Kola module spec
+    
+    Usage:
+        __kola_spec__ = KolaSpec(
+            __name__,
+            collect_all()
+        )
+    """
+    name: str
+    command_set_classes: List[CommandSetMeta]
+    
+    doc: Optional[str] = None
+    main_class: Optional[Type[KoiLang]] = None
+
+
+def collect_all() -> List[CommandSetMeta]:
+    """get all CommandSet class defined in the module
+
+    :return: a list of CommandSet class found
+    :rtype: List[CommandSetMeta]
+    """
+    frame = inspect.currentframe()
+    if not frame or not frame.f_back:  # pragma: no cover
+        raise ValueError("cannot read variables from the frame")
+    return [
+        i for i in frame.f_back.f_locals.values()
+        if isinstance(i, CommandSetMeta)
+    ]
+
+
+def load_library(name: str, paths: List[str] = KOLA_LIB_PATH) -> ModuleType:
+    """load a Phython script or package as a Kola module
+
+    :param name: module name like 'mymodule.sub'
+    :type name: str
+    :param paths: base path to load the module, defaults to KOLA_LIB_PATH
+    :type paths: List[str], optional
+    :raises ValueError: illegal module name
+    :raises ImportError: fail to load the module
+    :return: the Kola module
+    :rtype: ModuleType
+    """
+    if not _module_pattern.match(name):  # pragma: no cover
+        raise ValueError(f"illegal module name '{name}'")
+    module_name = "kola.lib." + name
+    if module_name in sys.modules:
+        return sys.modules[module_name]
+
+    for b in paths:
+        spec = None
+        b = os.path.abspath(b)
+        full_path = os.path.join(b, name)
+        if os.path.isdir(full_path):
+            spec = spec_from_file_location(
+                module_name, os.path.join(full_path, "__init__.py"),
+                submodule_search_locations=[full_path]
+            )
+        else:
+            for i in glob(full_path + '.*'):
+                spec = spec_from_file_location(module_name, i)
+                if spec:
+                    full_path = i
+                    break
+        if spec:
+            spec.name = module_name
+            return _load(spec)
+    raise ImportError(f"cannot load script {name}", name=name)  # pragma: no cover
+
+
+def main_class_from_module(module: ModuleType) -> Type[KoiLang]:
+    spec = getattr(module, "__kola_spec__", None)
+    if spec:
+        if not isinstance(spec, KolaSpec):
+            spec = KolaSpec(*spec)
+        if spec.main_class:
+            return spec.main_class
+        for i in spec.command_set_classes:
+            if issubclass(i, KoiLang):
+                return i
+    else:
+        for i in module.__dict__.values():
+            if isinstance(i, type) and issubclass(i, KoiLang) and i is not KoiLang:
+                return i
+    raise ValueError(  # pragma: no cover
+        f"no available main class for kola module '{spec.name if spec else module.__name__}'"
+    )
```

### Comparing `KoiLang-1.1.1/kola/lib/debugger/base.py` & `KoiLang-1.2.0a0/kola/lib/debugger/base.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import sys
-from types import TracebackType
-from typing import Optional, Type
-from traceback import print_exception
-
-from kola import __version__
-from kola.klvm import KoiLang, kola_command
-
-
-class BaseDebugger(KoiLang):
-    """
-    provide unified version checking and error suppression functions
-    """
-    __slots__ = []
-
-    @kola_command
-    def version(self, __chk_ver: Optional[int] = None) -> None:
-        if __chk_ver is None:
-            print(__version__)
-        elif __chk_ver < 100 or __chk_ver > 120:
-            print(f"version {__chk_ver} is not support by runner {__version__}")
-            sys.exit(2)
-
-    def on_exception(self, exc_type: Type[BaseException], exc_ins: BaseException, traceback: TracebackType) -> bool:
-        super().on_exception(exc_type, exc_ins, traceback)
-        print_exception(exc_type, exc_ins, traceback)
-        return True
+import sys
+from types import TracebackType
+from typing import Optional, Type
+from traceback import print_exception
+
+from kola import __version__
+from kola.klvm import KoiLang, kola_command
+
+
+class BaseDebugger(KoiLang):
+    """
+    provide unified version checking and error suppression functions
+    """
+    __slots__ = []
+
+    @kola_command
+    def version(self, __chk_ver: Optional[int] = None) -> None:
+        if __chk_ver is None:
+            print(__version__)
+        elif __chk_ver < 100 or __chk_ver > 120:
+            print(f"version {__chk_ver} is not support by runner {__version__}")
+            sys.exit(2)
+
+    def on_exception(self, exc_type: Type[BaseException], exc_ins: BaseException, traceback: TracebackType) -> bool:
+        super().on_exception(exc_type, exc_ins, traceback)
+        print_exception(exc_type, exc_ins, traceback)
+        return True
```

### Comparing `KoiLang-1.1.1/kola/lib/debugger/default_runner.py` & `KoiLang-1.2.0a0/kola/lib/debugger/default_runner.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-"""
-Copyright 2023 Ovizro
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-import os
-import re
-import sys
-from types import ModuleType
-from typing import Any, Dict, List, Optional, TypeVar, Union
-from typing_extensions import Literal
-
-from kola.exception import KoiLangCommandError
-from kola.klvm import Environment, kola_command, kola_text
-from kola.lib import KOLA_LIB_PATH, KolaSpec, collect_all, load_library, main_class_from_module
-from kola.lib.debugger.base import BaseDebugger
-
-
-T = TypeVar("T")
-
-
-FLAG_DEBUG = 1
-
-
-class KoiLangRunner(BaseDebugger):
-    """
-    default class for KoiLang module runner
-    """
-
-    var_pattern = re.compile(r"\$(\{)?(?P<name>[a-zA-Z_]\w*)(?(1)\}|)", re.ASCII)
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.flag = 0
-
-    @kola_command
-    def license(self) -> None:
-        print(__doc__)
-    
-    @kola_command(alias="raise")
-    def raises(self, *msg: str) -> None:
-        raise KoiLangCommandError(*msg)
-    
-    @kola_command
-    def pragma(self, *, debug: Optional[Literal["on", "off"]] = None) -> None:
-        if debug:
-            if debug == "on":
-                self.flag |= FLAG_DEBUG
-            elif debug == "off":
-                self.flag &= ~FLAG_DEBUG
-            else:
-                raise ValueError(f"illegal value '{debug}'")
-    
-    @kola_command
-    def echo(self, *text: str) -> None:
-        print(' '.join(text))
-    
-    @kola_command
-    def execute(self, source: str) -> None:
-        code = compile(source, "<kola_runner>", "single")
-        exec(code, {"kola_runner": self, "__vars__": self.vars})
-    
-    @kola_command(alias="export")
-    def set(self, **kwds) -> None:
-        self.vars.update(kwds)
-    
-    @kola_command
-    def exit(self, code: int = 0) -> None:
-        sys.exit(code)
-        
-    @kola_text
-    def text(self, text: str) -> None:
-        print(f"## [TEXT] {text}")
-    
-    @kola_command
-    def load(self, path: Union[str, bytes, os.PathLike], type: Optional[str] = None, **kwds: Any) -> None:
-        path = os.fsdecode(path)
-        if type is None:
-            if path.endswith(".kola"):
-                type = "kola"
-            else:
-                type = "script"
-        else:
-            type = type.lower()
-        if type == "kola":
-            self.load_kola(path, **kwds)
-        elif type in ["script", "lib"]:
-            self.load_script(path, **kwds)
-        else:
-            raise ValueError(f"invalid type name '{type}'")
-    
-    @kola_command
-    def load_kola(self, path: Union[str, bytes, os.PathLike], *, encoding: str = "utf-8", **kwds) -> None:
-        self.parse_file(path, encoding=encoding, **kwds)
-    
-    @kola_command(alias=["load_lib", "load_library"])
-    def load_script(self, name: str, lib_path: Optional[List[str]] = None) -> None:
-        kola_module = load_library(name, lib_path or KOLA_LIB_PATH)
-        self.load_command_set(kola_module)
-    
-    def at_start(self) -> None:
-        self.vars = {}
-        self.flag = 0
-        self.loaded_class = set()
-    
-    def at_end(self) -> None:
-        super().at_end()
-        for i in self.loaded_class:
-            i.at_end(self)
-    
-    def get_var(self, key: str) -> Any:
-        if key == '__top__':
-            return self.top.__class__.__name__
-        elif key == "__dir__":
-            return ', '.join(self.raw_command_set)
-        elif key == "__name__":
-            return self.__class__.__name__
-        elif key == "__stack_info__":
-            env_names = []
-            top = self.top
-            while top is not self:
-                env_names.append(top.__class__.__name__)
-                top = top.back  # type: ignore
-            env_names.append("__init__")
-            return " -> ".join(env_names)
-        else:
-            return self.vars.get(key, None)
-    
-    def load_command_set(self, module: ModuleType) -> None:
-        cls = main_class_from_module(module)
-        if self.flag & FLAG_DEBUG:
-            print(f"## [DEBUG] Load class: {cls}")
-        self.loaded_class.add(cls)
-        cls.at_start(self)
-        self.raw_command_set.update(
-            cls.generate_raw_commands()
-        )
-    
-    def format_text(self, argument: T) -> T:
-        if isinstance(argument, list):
-            return [self.format_text(i) for i in argument]  # type: ignore
-        elif isinstance(argument, dict):
-            return {k: self.format_text(v) for k, v in argument.items()}  # type: ignore
-        elif isinstance(argument, str):
-            return self.var_pattern.sub(
-                lambda match: str(self.get_var(match.group("name")) or ''),
-                argument
-            )
-        return argument
-    
-    def __kola_caller__(
-            self, command: Any, args: tuple, kwargs: Dict[str, Any],
-            *, bound_instance: Any = None, **kwds: Any) -> Any:
-        if self.flag & FLAG_DEBUG:
-            print(f"## [DEBUG] Run command: {command.__name__} ({(bound_instance or self).__class__.__name__})")
-        return super().__kola_caller__(
-            command,
-            tuple(self.format_text(i) for i in args),
-            self.format_text(kwargs),
-            bound_instance=bound_instance,
-            **kwds
-        )
-    
-    def push_apply(self, __push_cache: Environment) -> None:
-        if self.flag & FLAG_DEBUG:
-            print(f"## [DEBUG] Push env: {__push_cache}")
-        return super().push_apply(__push_cache)
-    
-    def pop_apply(self, __env_cache: Environment) -> None:
-        if self.flag & FLAG_DEBUG:
-            print(f"## [DEBUG] Pop env: {__env_cache}")
-        return super().pop_apply(__env_cache)
-
-
-__kola_spec__ = KolaSpec(
-    "Kola Runner",
-    collect_all(),
-    main_class=KoiLangRunner
-)
+"""
+Copyright 2023 Ovizro
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+import os
+import re
+import sys
+from types import ModuleType
+from typing import Any, Dict, List, Optional, TypeVar, Union
+from typing_extensions import Literal
+
+from kola.exception import KoiLangCommandError
+from kola.klvm import Environment, kola_command, kola_text
+from kola.lib import KOLA_LIB_PATH, KolaSpec, collect_all, load_library, main_class_from_module
+from kola.lib.debugger.base import BaseDebugger
+
+
+T = TypeVar("T")
+
+
+FLAG_DEBUG = 1
+
+
+class KoiLangRunner(BaseDebugger):
+    """
+    default class for KoiLang module runner
+    """
+
+    var_pattern = re.compile(r"\$(\{)?(?P<name>[a-zA-Z_]\w*)(?(1)\}|)", re.ASCII)
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.flag = 0
+
+    @kola_command
+    def license(self) -> None:
+        print(__doc__)
+    
+    @kola_command(alias="raise")
+    def raises(self, *msg: str) -> None:
+        raise KoiLangCommandError(*msg)
+    
+    @kola_command
+    def pragma(self, *, debug: Optional[Literal["on", "off"]] = None) -> None:
+        if debug:
+            if debug == "on":
+                self.flag |= FLAG_DEBUG
+            elif debug == "off":
+                self.flag &= ~FLAG_DEBUG
+            else:
+                raise ValueError(f"illegal value '{debug}'")
+    
+    @kola_command
+    def echo(self, *text: str) -> None:
+        print(' '.join(text))
+    
+    @kola_command
+    def execute(self, source: str) -> None:
+        code = compile(source, "<kola_runner>", "single")
+        exec(code, {"kola_runner": self, "__vars__": self.vars})
+    
+    @kola_command(alias="export")
+    def set(self, **kwds) -> None:
+        self.vars.update(kwds)
+    
+    @kola_command
+    def exit(self, code: int = 0) -> None:
+        sys.exit(code)
+        
+    @kola_text
+    def text(self, text: str) -> None:
+        print(f"## [TEXT] {text}")
+    
+    @kola_command
+    def load(self, path: Union[str, bytes, os.PathLike], type: Optional[str] = None, **kwds: Any) -> None:
+        path = os.fsdecode(path)
+        if type is None:
+            if path.endswith(".kola"):
+                type = "kola"
+            else:
+                type = "script"
+        else:
+            type = type.lower()
+        if type == "kola":
+            self.load_kola(path, **kwds)
+        elif type in ["script", "lib"]:
+            self.load_script(path, **kwds)
+        else:
+            raise ValueError(f"invalid type name '{type}'")
+    
+    @kola_command
+    def load_kola(self, path: Union[str, bytes, os.PathLike], *, encoding: str = "utf-8", **kwds) -> None:
+        self.parse_file(path, encoding=encoding, **kwds)
+    
+    @kola_command(alias=["load_lib", "load_library"])
+    def load_script(self, name: str, lib_path: Optional[List[str]] = None) -> None:
+        kola_module = load_library(name, lib_path or KOLA_LIB_PATH)
+        self.load_command_set(kola_module)
+    
+    def at_start(self) -> None:
+        self.vars = {}
+        self.flag = 0
+        self.loaded_class = set()
+    
+    def at_end(self) -> None:
+        super().at_end()
+        for i in self.loaded_class:
+            i.at_end(self)
+    
+    def get_var(self, key: str) -> Any:
+        if key == '__top__':
+            return self.top.__class__.__name__
+        elif key == "__dir__":
+            return ', '.join(self.raw_command_set)
+        elif key == "__name__":
+            return self.__class__.__name__
+        elif key == "__stack_info__":
+            env_names = []
+            top = self.top
+            while top is not self:
+                env_names.append(top.__class__.__name__)
+                top = top.back  # type: ignore
+            env_names.append("__init__")
+            return " -> ".join(env_names)
+        else:
+            return self.vars.get(key, None)
+    
+    def load_command_set(self, module: ModuleType) -> None:
+        cls = main_class_from_module(module)
+        if self.flag & FLAG_DEBUG:
+            print(f"## [DEBUG] Load class: {cls}")
+        self.loaded_class.add(cls)
+        cls.at_start(self)
+        self.raw_command_set.update(
+            cls.generate_raw_commands()
+        )
+    
+    def format_text(self, argument: T) -> T:
+        if isinstance(argument, list):
+            return [self.format_text(i) for i in argument]  # type: ignore
+        elif isinstance(argument, dict):
+            return {k: self.format_text(v) for k, v in argument.items()}  # type: ignore
+        elif isinstance(argument, str):
+            return self.var_pattern.sub(
+                lambda match: str(self.get_var(match.group("name")) or ''),
+                argument
+            )
+        return argument
+    
+    def __kola_caller__(
+            self, command: Any, args: tuple, kwargs: Dict[str, Any],
+            *, bound_instance: Any = None, **kwds: Any) -> Any:
+        if self.flag & FLAG_DEBUG:
+            print(f"## [DEBUG] Run command: {command.__name__} ({(bound_instance or self).__class__.__name__})")
+        return super().__kola_caller__(
+            command,
+            tuple(self.format_text(i) for i in args),
+            self.format_text(kwargs),
+            bound_instance=bound_instance,
+            **kwds
+        )
+    
+    def push_apply(self, __push_cache: Environment) -> None:
+        if self.flag & FLAG_DEBUG:
+            print(f"## [DEBUG] Push env: {__push_cache}")
+        return super().push_apply(__push_cache)
+    
+    def pop_apply(self, __env_cache: Environment) -> None:
+        if self.flag & FLAG_DEBUG:
+            print(f"## [DEBUG] Pop env: {__env_cache}")
+        return super().pop_apply(__env_cache)
+
+
+__kola_spec__ = KolaSpec(
+    "Kola Runner",
+    collect_all(),
+    main_class=KoiLangRunner
+)
```

### Comparing `KoiLang-1.1.1/kola/lib/fastfiles.py` & `KoiLang-1.2.0a0/kola/lib/fastfiles.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import os
-from pathlib import Path
-from typing import ClassVar, Optional, Type, Union
-from typing_extensions import Literal
-
-from kola.klvm import CommandSet, Environment, KoiLang, kola_command, kola_text, kola_env_enter, kola_env_exit
-from kola.lib import _module_pattern
-
-
-class FastFiles(KoiLang):
-    __slots__ = ["base_path", "__base_path"]
-
-    def __init__(self, base: Union[str, os.PathLike, None] = None) -> None:
-        super().__init__()
-        if base is None:
-            self.__base_path = Path.cwd()
-        else:
-            self.__base_path = Path(base)
-
-    class FileContains(Environment):
-        __slots__ = ["fp"]
-
-        home: "FastFiles"
-        Space: ClassVar[Type["FastFiles.Space"]]
-
-        @kola_env_enter("file", envs="!$?")
-        def open(self, path: Union[str, os.PathLike], *, encoding: str = "utf-8") -> None:
-            base = self.home.base_path
-            self.fp = (base / path).open("w", encoding=encoding)
-        
-        @kola_command
-        def seek(self, __cookie: int, __whence: Union[Literal["SET", "CUR", "END"], int]) -> None:
-            if __whence == "SET":
-                __whence = os.SEEK_SET
-            elif __whence == "CUR":
-                __whence = os.SEEK_CUR
-            elif __whence == "END":
-                __whence = os.SEEK_END
-            elif not isinstance(__whence, int):
-                raise ValueError(f"invalid seek whence {__whence}")
-            self.fp.seek(__cookie, __whence)
-        
-        @kola_text
-        def text(self, text: str) -> None:
-            self.fp.write(text)
-        
-        @property
-        def path(self) -> str:
-            return self.fp.name
-
-        def tear_down(self, top: CommandSet) -> None:
-            self.fp.close()
-            return super().tear_down(top)
-    
-    class Space(Environment):
-        __slots__ = ["parent_path", "path"]
-
-        home: "FastFiles"
-        FileContains: ClassVar[Type["FastFiles.FileContains"]]
-
-        @kola_env_enter("space")
-        def enter(self, name: Optional[str] = None, path: Optional[Union[str, os.PathLike]] = None) -> None:
-            base_path = self.home.base_path
-            self.parent_path = base_path
-            if not path:
-                assert name
-                if not _module_pattern.match(name):
-                    raise ValueError(f"invalid space name {name}")
-                path = os.path.join(*name.split('.'))
-            self.path = base_path / path
-            self.path.mkdir(755, exist_ok=True)
-            self.home.base_path = self.path
-        
-        @kola_env_exit("endspace")
-        def exit(self) -> None:
-            self.home.base_path = self.parent_path
-        
-        def set_up(self, top: CommandSet) -> None:
-            if isinstance(top, FastFiles.FileContains):
-                home = self.home
-                cache = home.pop_prepare()
-                home.pop_apply(cache)
-                # update self.back
-                self.back = home.top
-            return super().set_up(top)
-    
-    def at_start(self) -> None:
-        self.base_path = self.__base_path
-    
-    def at_end(self) -> None:
-        del self.base_path
-
-
-FastFiles.FileContains.Space = FastFiles.Space
-FastFiles.Space.FileContains = FastFiles.FileContains
+import os
+from pathlib import Path
+from typing import ClassVar, Optional, Type, Union
+from typing_extensions import Literal
+
+from kola.klvm import CommandSet, Environment, KoiLang, kola_command, kola_text, kola_env_enter, kola_env_exit
+from kola.lib import _module_pattern
+
+
+class FastFiles(KoiLang):
+    __slots__ = ["base_path", "__base_path"]
+
+    def __init__(self, base: Union[str, os.PathLike, None] = None) -> None:
+        super().__init__()
+        if base is None:
+            self.__base_path = Path.cwd()
+        else:
+            self.__base_path = Path(base)
+
+    class FileContains(Environment):
+        __slots__ = ["fp"]
+
+        home: "FastFiles"
+        Space: ClassVar[Type["FastFiles.Space"]]
+
+        @kola_env_enter("file", envs="!$?")
+        def open(self, path: Union[str, os.PathLike], *, encoding: str = "utf-8") -> None:
+            base = self.home.base_path
+            self.fp = (base / path).open("w", encoding=encoding)
+        
+        @kola_command
+        def seek(self, __cookie: int, __whence: Union[Literal["SET", "CUR", "END"], int]) -> None:
+            if __whence == "SET":
+                __whence = os.SEEK_SET
+            elif __whence == "CUR":
+                __whence = os.SEEK_CUR
+            elif __whence == "END":
+                __whence = os.SEEK_END
+            elif not isinstance(__whence, int):
+                raise ValueError(f"invalid seek whence {__whence}")
+            self.fp.seek(__cookie, __whence)
+        
+        @kola_text
+        def text(self, text: str) -> None:
+            self.fp.write(text)
+        
+        @property
+        def path(self) -> str:
+            return self.fp.name
+
+        def tear_down(self, top: CommandSet) -> None:
+            self.fp.close()
+            return super().tear_down(top)
+    
+    class Space(Environment):
+        __slots__ = ["parent_path", "path"]
+
+        home: "FastFiles"
+        FileContains: ClassVar[Type["FastFiles.FileContains"]]
+
+        @kola_env_enter("space")
+        def enter(self, name: Optional[str] = None, path: Optional[Union[str, os.PathLike]] = None) -> None:
+            base_path = self.home.base_path
+            self.parent_path = base_path
+            if not path:
+                assert name
+                if not _module_pattern.match(name):
+                    raise ValueError(f"invalid space name {name}")
+                path = os.path.join(*name.split('.'))
+            self.path = base_path / path
+            self.path.mkdir(755, exist_ok=True)
+            self.home.base_path = self.path
+        
+        @kola_env_exit("endspace")
+        def exit(self) -> None:
+            self.home.base_path = self.parent_path
+        
+        def set_up(self, top: CommandSet) -> None:
+            if isinstance(top, FastFiles.FileContains):
+                home = self.home
+                cache = home.pop_prepare()
+                home.pop_apply(cache)
+                # update self.back
+                self.back = home.top
+            return super().set_up(top)
+    
+    def at_start(self) -> None:
+        self.base_path = self.__base_path
+    
+    def at_end(self) -> None:
+        del self.base_path
+
+
+FastFiles.FileContains.Space = FastFiles.Space
+FastFiles.Space.FileContains = FastFiles.FileContains
```

### Comparing `KoiLang-1.1.1/kola/lib/recorder.py` & `KoiLang-1.2.0a0/kola/lib/recorder.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import os
-from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Union, overload
-
-from kola.lexer import BaseLexer, FileLexer, StringLexer
-from kola.parser import Parser
-from kola.klvm import CommandSet
-
-
-class Instruction(NamedTuple):
-    name: str
-    args: Tuple[Any, ...]
-    kwargs: Dict[Any, Any]
-
-
-class _Recorder(CommandSet):
-    __slots__ = []
-
-    def __getitem__(self, __key: str) -> Callable[..., Instruction]:
-        return lambda *args, **kwds: Instruction(__key, args, kwds)
-
-
-recorder = _Recorder()
-
-
-@overload
-def parse(__lexer: BaseLexer) -> List[Instruction]: ...
-@overload
-def parse(__str: str, *, command_threshold: int = 1, no_lstrip: bool = ...) -> List[Instruction]: ...
-def parse(__lexer_or_str: Union[str, BaseLexer], **kwds: Any) -> List[Instruction]:  # noqa: E302
-    if isinstance(__lexer_or_str, str):
-        __lexer_or_str = StringLexer(__lexer_or_str, **kwds)
-    else:
-        assert not kwds
-    return list(Parser(__lexer_or_str, recorder))
-
-
-def parse_file(path: Union[str, bytes, os.PathLike], *, encoding: Optional[str] = None, **kwds: Any) -> List[Instruction]:
-    lexer = FileLexer(path, encoding=encoding or "utf-8", **kwds)
-    return parse(lexer)
+import os
+from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Union, overload
+
+from kola.lexer import BaseLexer, FileLexer, StringLexer
+from kola.parser import Parser
+from kola.klvm import CommandSet
+
+
+class Instruction(NamedTuple):
+    name: str
+    args: Tuple[Any, ...]
+    kwargs: Dict[Any, Any]
+
+
+class _Recorder(CommandSet):
+    __slots__ = []
+
+    def __getitem__(self, __key: str) -> Callable[..., Instruction]:
+        return lambda *args, **kwds: Instruction(__key, args, kwds)
+
+
+recorder = _Recorder()
+
+
+@overload
+def parse(__lexer: BaseLexer) -> List[Instruction]: ...
+@overload
+def parse(__str: str, *, command_threshold: int = 1, no_lstrip: bool = ...) -> List[Instruction]: ...
+def parse(__lexer_or_str: Union[str, BaseLexer], **kwds: Any) -> List[Instruction]:  # noqa: E302
+    if isinstance(__lexer_or_str, str):
+        __lexer_or_str = StringLexer(__lexer_or_str, **kwds)
+    else:
+        assert not kwds
+    return list(Parser(__lexer_or_str, recorder))
+
+
+def parse_file(path: Union[str, bytes, os.PathLike], *, encoding: Optional[str] = None, **kwds: Any) -> List[Instruction]:
+    lexer = FileLexer(path, encoding=encoding or "utf-8", **kwds)
+    return parse(lexer)
```

### Comparing `KoiLang-1.1.1/kola/parser.c` & `KoiLang-1.2.0a0/kola/parser.c`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.1/kola/parser.pyi` & `KoiLang-1.2.0a0/kola/parser.pyi`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Any, Callable, Final, Generic, Tuple, TypeVar
-from typing_extensions import Protocol, Self
-from .lexer import BaseLexer, Token
-
-
-class SupportGetCommand(Protocol):
-    def __getitem__(self, __key: str) -> Callable: ...
-
-
-T_CmdSet = TypeVar("T_CmdSet", bound=SupportGetCommand)
-T_Lexer = TypeVar("T_Lexer", bound=BaseLexer)
-
-
-class Parser(Generic[T_Lexer, T_CmdSet]):
-    lexer: Final[T_Lexer]
-    command_set: Final[T_CmdSet]
-
-    def __init__(self, lexer: T_Lexer, command_set: T_CmdSet) -> None: ...
-    def push(self, token: Token) -> None: ...
-    def pop(self) -> Token: ...
-    def parse_args(self) -> Tuple[tuple, dict]: ...
-    def exec_once(self) -> Any: ...
-    def exec(self) -> None: ...
-    def eof(self) -> bool: ...
-    def __iter__(self) -> Self: ...
+from typing import Any, Callable, Final, Generic, Tuple, TypeVar
+from typing_extensions import Protocol, Self
+from .lexer import BaseLexer, Token
+
+
+class SupportGetCommand(Protocol):
+    def __getitem__(self, __key: str) -> Callable: ...
+
+
+T_CmdSet = TypeVar("T_CmdSet", bound=SupportGetCommand)
+T_Lexer = TypeVar("T_Lexer", bound=BaseLexer)
+
+
+class Parser(Generic[T_Lexer, T_CmdSet]):
+    lexer: Final[T_Lexer]
+    command_set: Final[T_CmdSet]
+
+    def __init__(self, lexer: T_Lexer, command_set: T_CmdSet) -> None: ...
+    def push(self, token: Token) -> None: ...
+    def pop(self) -> Token: ...
+    def parse_args(self) -> Tuple[tuple, dict]: ...
+    def exec_once(self) -> Any: ...
+    def exec(self) -> None: ...
+    def eof(self) -> bool: ...
+    def __iter__(self) -> Self: ...
     def __next__(self) -> Any: ...
```

### Comparing `KoiLang-1.1.1/kola/unicode_handler.c` & `KoiLang-1.2.0a0/kola/unicode_handler.c`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-#include "Python.h"
-#include "_cutil.h"
-
-#ifdef HAVE_WCHAR_H
-    #include <wchar.h>
-#endif
-
-PyObject* _decode_utf8(const char **sPtr, const char *end)
-{
-    const char *s;
-    const char *t;
-    t = s = *sPtr;
-    while (s < end && (*s & 0x80)) {
-        s++;
-    }
-    *sPtr = s;
-    return PyUnicode_DecodeUTF8(t, s - t, NULL);
-}
-
-// from cpython:string_parser.decode_unicode_with_escapes
-PyObject* decode_escapes(const char* s, Py_ssize_t len) {
-    PyObject *v = NULL;
-
-    /* check for integer overflow */
-    if ((uint64_t)len > SIZE_MAX / 6) {
-        return NULL;
-    }
-    /* "ä" (2 bytes) may become "\U000000E4" (10 bytes), or 1:5
-       "\ä" (3 bytes) may become "\u005c\U000000E4" (16 bytes), or ~1:6 */
-    PyObject *u = PyBytes_FromStringAndSize((char *)NULL, len * 6);
-    if (u == NULL) {
-        return NULL;
-    }
-
-    char *buf;
-    char *p;
-    p = buf = PyBytes_AsString(u);
-    if (p == NULL) {
-        return NULL;
-    }
-    const char *end = s + len;
-    while (s < end) {
-        if (*s == '\\') {
-            *p++ = *s++;
-            if (s >= end || *s & 0x80) {
-                strcpy(p, "u005c");
-                p += 5;
-                if (s >= end) {
-                    break;
-                }
-            } else if (s + 1 < end && *s == '\r' && s[1] == '\n') {
-                p--;
-                s += 2;
-                if (s >= end) {
-                    break;
-                }
-            } else if (*s == '\n') {
-                p--;
-                s++;
-                if (s >= end) {
-                    break;
-                }
-            }
-        }
-        if (*s & 0x80) {
-            PyObject *w;
-            int kind;
-            const void *data;
-            Py_ssize_t w_len;
-            Py_ssize_t i;
-            w = _decode_utf8(&s, end);
-            if (w == NULL) {
-                Py_DECREF(u);
-                return NULL;
-            }
-            kind = PyUnicode_KIND(w);
-            data = PyUnicode_DATA(w);
-            w_len = PyUnicode_GET_LENGTH(w);
-            for (i = 0; i < w_len; i++) {
-                Py_UCS4 chr = PyUnicode_READ(kind, data, i);
-                sprintf(p, "\\U%08x", chr);
-                p += 10;
-            }
-            /* Should be impossible to overflow */
-            assert(p - buf <= PyBytes_GET_SIZE(u));
-            Py_DECREF(w);
-        }
-        else {
-            *p++ = *s++;
-        }
-    }
-    len = p - buf;
-    s = buf;
-    v = PyUnicode_DecodeUnicodeEscape(s, len, NULL);
-    return v;
-}
-
-PyObject* filter_text(PyObject* string) {
-    Py_ssize_t len = PyUnicode_GET_LENGTH(string);
-    Py_ssize_t offset = 0;
-    for (Py_ssize_t i = 0; i < len; ++i) {
-        Py_UCS4 chr = PyUnicode_READ_CHAR(string, i);
-        if (chr == '\\') {
-            offset++;
-            Py_UCS4 tc = PyUnicode_READ_CHAR(string, ++i);
-            switch (tc) {
-            case '\n':
-                offset++;
-                break;
-            case '\r':
-                if (PyUnicode_READ_CHAR(string, i + 1) == '\n') {
-                    i++;
-                    offset += 2;
-                    break;
-                }
-            default:
-                if (PyUnicode_WriteChar(string, i - offset, '\\') == -1)
-                    goto bad;
-                --offset;
-                if (PyUnicode_WriteChar(string, i - offset, tc) == -1)
-                    goto bad;
-                break;
-            }
-        } else if (offset) {
-            if (PyUnicode_WriteChar(string, i - offset, chr) == -1) goto bad;
-        }
-    }
-    if (offset)
-        PyUnicode_Resize(&string, len - offset);
-    return string;
-bad:
-    return NULL;
-}
+#include "Python.h"
+#include "_cutil.h"
+
+#ifdef HAVE_WCHAR_H
+    #include <wchar.h>
+#endif
+
+PyObject* _decode_utf8(const char **sPtr, const char *end)
+{
+    const char *s;
+    const char *t;
+    t = s = *sPtr;
+    while (s < end && (*s & 0x80)) {
+        s++;
+    }
+    *sPtr = s;
+    return PyUnicode_DecodeUTF8(t, s - t, NULL);
+}
+
+// from cpython:string_parser.decode_unicode_with_escapes
+PyObject* decode_escapes(const char* s, Py_ssize_t len) {
+    PyObject *v = NULL;
+
+    /* check for integer overflow */
+    if ((uint64_t)len > SIZE_MAX / 6) {
+        return NULL;
+    }
+    /* "ä" (2 bytes) may become "\U000000E4" (10 bytes), or 1:5
+       "\ä" (3 bytes) may become "\u005c\U000000E4" (16 bytes), or ~1:6 */
+    PyObject *u = PyBytes_FromStringAndSize((char *)NULL, len * 6);
+    if (u == NULL) {
+        return NULL;
+    }
+
+    char *buf;
+    char *p;
+    p = buf = PyBytes_AsString(u);
+    if (p == NULL) {
+        return NULL;
+    }
+    const char *end = s + len;
+    while (s < end) {
+        if (*s == '\\') {
+            *p++ = *s++;
+            if (s >= end || *s & 0x80) {
+                strcpy(p, "u005c");
+                p += 5;
+                if (s >= end) {
+                    break;
+                }
+            } else if (s + 1 < end && *s == '\r' && s[1] == '\n') {
+                p--;
+                s += 2;
+                if (s >= end) {
+                    break;
+                }
+            } else if (*s == '\n') {
+                p--;
+                s++;
+                if (s >= end) {
+                    break;
+                }
+            }
+        }
+        if (*s & 0x80) {
+            PyObject *w;
+            int kind;
+            const void *data;
+            Py_ssize_t w_len;
+            Py_ssize_t i;
+            w = _decode_utf8(&s, end);
+            if (w == NULL) {
+                Py_DECREF(u);
+                return NULL;
+            }
+            kind = PyUnicode_KIND(w);
+            data = PyUnicode_DATA(w);
+            w_len = PyUnicode_GET_LENGTH(w);
+            for (i = 0; i < w_len; i++) {
+                Py_UCS4 chr = PyUnicode_READ(kind, data, i);
+                sprintf(p, "\\U%08x", chr);
+                p += 10;
+            }
+            /* Should be impossible to overflow */
+            assert(p - buf <= PyBytes_GET_SIZE(u));
+            Py_DECREF(w);
+        }
+        else {
+            *p++ = *s++;
+        }
+    }
+    len = p - buf;
+    s = buf;
+    v = PyUnicode_DecodeUnicodeEscape(s, len, NULL);
+    return v;
+}
+
+PyObject* filter_text(PyObject* string) {
+    Py_ssize_t len = PyUnicode_GET_LENGTH(string);
+    Py_ssize_t offset = 0;
+    for (Py_ssize_t i = 0; i < len; ++i) {
+        Py_UCS4 chr = PyUnicode_READ_CHAR(string, i);
+        if (chr == '\\') {
+            offset++;
+            Py_UCS4 tc = PyUnicode_READ_CHAR(string, ++i);
+            switch (tc) {
+            case '\n':
+                offset++;
+                break;
+            case '\r':
+                if (PyUnicode_READ_CHAR(string, i + 1) == '\n') {
+                    i++;
+                    offset += 2;
+                    break;
+                }
+            default:
+                if (PyUnicode_WriteChar(string, i - offset, '\\') == -1)
+                    goto bad;
+                --offset;
+                if (PyUnicode_WriteChar(string, i - offset, tc) == -1)
+                    goto bad;
+                break;
+            }
+        } else if (offset) {
+            if (PyUnicode_WriteChar(string, i - offset, chr) == -1) goto bad;
+        }
+    }
+    if (offset)
+        PyUnicode_Resize(&string, len - offset);
+    return string;
+bad:
+    return NULL;
+}
```

### Comparing `KoiLang-1.1.1/kola/writer.c` & `KoiLang-1.2.0a0/kola/writer.c`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.1/kola/writer.pxd` & `KoiLang-1.2.0a0/kola/writer.pxd`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from libc.stdio cimport FILE
-from libc.stdint cimport uint8_t
-from ._cutil cimport *
-
-
-cdef enum ItemLevel:
-    BASE_ITEM
-    COMPLEX_ITEM
-    ARG_ITEM
-    FULL_CMD
-
-
-cdef class BaseWriterItem(object):
-    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
-
-
-cdef class FormatItem(BaseWriterItem):
-    cdef readonly:
-        object value
-        str spec
-    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
-
-
-cdef class ComplexArg(BaseWriterItem):
-    cdef readonly:
-        str name
-        object value
-        bint split_line
-    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
-
-
-cdef class NewlineItem(BaseWriterItem):
-    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
-
-
-cdef NewlineItem i_newline
-
-
-cdef class BaseWriter:
-    cdef Py_ssize_t cur_indent
-    cdef readonly:
-        uint8_t indent
-        int command_threshold
-    cdef public bint line_beginning
-
-    cpdef void raw_write(self, str text) except *
-    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
-    cdef void raw_write_char(self, char ch) except *
-    cpdef void close(self)
-    cpdef void inc_indent(self)
-    cpdef void dec_indent(self) except *
-    cdef void _write_indent(self) except *
-    cdef void _write_prefix(self, Py_ssize_t length) except *
-    cpdef void newline(self, bint concat_prev = *) except *
-    cpdef void prepare(self) except *
-    cdef void _write_text(self, str text) except *
-
-
-cdef class FileWriter(BaseWriter):
-    cdef FILE* fp
-    cdef readonly:
-        object path
-        str encoding
-    cpdef void close(self)
-    cpdef void prepare(self) except *
-    cpdef void raw_write(self, str text) except *
-    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
-    cdef void raw_write_char(self, char ch) except *
-
-
-cdef class StringWriter(BaseWriter):
-    cdef:
-        bint _closed
-        _PyUnicodeWriter writer
-    
-    cpdef void close(self)
-    cpdef void prepare(self) except *
-    cpdef void raw_write(self, str text) except *
-    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
-    cdef void raw_write_char(self, char ch) except *
-    cpdef str getvalue(self)
+from libc.stdio cimport FILE
+from libc.stdint cimport uint8_t
+from ._cutil cimport *
+
+
+cdef enum ItemLevel:
+    BASE_ITEM
+    COMPLEX_ITEM
+    ARG_ITEM
+    FULL_CMD
+
+
+cdef class BaseWriterItem(object):
+    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
+
+
+cdef class FormatItem(BaseWriterItem):
+    cdef readonly:
+        object value
+        str spec
+    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
+
+
+cdef class ComplexArg(BaseWriterItem):
+    cdef readonly:
+        str name
+        object value
+        bint split_line
+    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
+
+
+cdef class NewlineItem(BaseWriterItem):
+    cpdef void __kola_write__(self, BaseWriter writer, ItemLevel level) except *
+
+
+cdef NewlineItem i_newline
+
+
+cdef class BaseWriter:
+    cdef Py_ssize_t cur_indent
+    cdef readonly:
+        uint8_t indent
+        int command_threshold
+    cdef public bint line_beginning
+
+    cpdef void raw_write(self, str text) except *
+    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
+    cdef void raw_write_char(self, char ch) except *
+    cpdef void close(self)
+    cpdef void inc_indent(self)
+    cpdef void dec_indent(self) except *
+    cdef void _write_indent(self) except *
+    cdef void _write_prefix(self, Py_ssize_t length) except *
+    cpdef void newline(self, bint concat_prev = *) except *
+    cpdef void prepare(self) except *
+    cdef void _write_text(self, str text) except *
+
+
+cdef class FileWriter(BaseWriter):
+    cdef FILE* fp
+    cdef readonly:
+        object path
+        str encoding
+    cpdef void close(self)
+    cpdef void prepare(self) except *
+    cpdef void raw_write(self, str text) except *
+    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
+    cdef void raw_write_char(self, char ch) except *
+
+
+cdef class StringWriter(BaseWriter):
+    cdef:
+        bint _closed
+        _PyUnicodeWriter writer
+    
+    cpdef void close(self)
+    cpdef void prepare(self) except *
+    cpdef void raw_write(self, str text) except *
+    cdef void raw_write_string(self, const char* string, Py_ssize_t length = *) except *
+    cdef void raw_write_char(self, char ch) except *
+    cpdef str getvalue(self)
```

### Comparing `KoiLang-1.1.1/kola/writer.pyi` & `KoiLang-1.2.0a0/kola/writer.pyi`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import os
-from types import TracebackType
-from typing import Any, Dict, Final, List, Type, Union
-from typing_extensions import Protocol, runtime_checkable, Self
-
-
-WF_BASE_ITEM: int
-WF_COMPLEX_ITEM: int
-WF_ARG_ITEM: int
-WF_FULL_CMD: int
-
-
-@runtime_checkable
-class WriterItemLike(Protocol):
-    def __kola_write__(self, __writer: BaseWriter, __level: int) -> None: ...
-
-
-class BaseWriterItem(object):
-    def __kola_write__(self, writer: BaseWriter, level: int) -> None: ...
-
-
-class FormatItem(BaseWriterItem):
-    value: Final[Any]
-    spec: Final[str]
-
-    def __init__(self, value: Any, spec: str) -> None: ...
-
-
-class ComplexArg(BaseWriterItem):
-    name: Final[str]
-    value: Final[Any]
-
-    def __init__(self, name: str, value: Any, *, split_line: bool = ...) -> None: ...
-
-
-WI_NEWLINE: BaseWriterItem
-
-
-_BaseItem = Union[str, bytes, int, float, WriterItemLike]
-_ComplexItem = Union[_BaseItem, List[_BaseItem], Dict[str, _BaseItem]]
-
-
-class BaseWriter(object):
-    indent: Final[int]
-
-    def __init__(self, indent: int = 4, command_threshold: int = 1) -> None: ...
-    def raw_write(self, text: str) -> None: ...
-    def close(self) -> None: ...
-    def inc_indent(self) -> None: ...
-    def dec_indent(self) -> None: ...
-    def newline(self, concat_prev: bool = ...) -> None: ...
-    def write_text(self, text: str) -> None: ...
-    def write_annotation(self, annotation: str) -> None: ...
-    def write_command(self, __name: Union[str, int], *args: _BaseItem, **kwds: _ComplexItem) -> None: ...
-    def write(self, command: Union[str, WriterItemLike]) -> None: ...
-    @property
-    def closed(self) -> bool: ...
-    def __enter__(self) -> Self: ...
-    def __exit__(self, exc_type: Type[BaseException], exc_ins: Exception, traceback: TracebackType) -> None: ...
-
-
-class FileWriter(BaseWriter):
-    path: Final[Union[str, bytes, os.PathLike]]
-    encoding: Final[str]
-
-    def __init__(self, __path: Union[str, bytes, os.PathLike], encoding: str = "utf-8",
-                 indent: int = ..., command_threshold: int = ...) -> None: ...
-
-
-class StringWriter(BaseWriter):
-    def getvalue(self) -> str: ...
+import os
+from types import TracebackType
+from typing import Any, Dict, Final, List, Type, Union
+from typing_extensions import Protocol, runtime_checkable, Self
+
+
+WF_BASE_ITEM: int
+WF_COMPLEX_ITEM: int
+WF_ARG_ITEM: int
+WF_FULL_CMD: int
+
+
+@runtime_checkable
+class WriterItemLike(Protocol):
+    def __kola_write__(self, __writer: BaseWriter, __level: int) -> None: ...
+
+
+class BaseWriterItem(object):
+    def __kola_write__(self, writer: BaseWriter, level: int) -> None: ...
+
+
+class FormatItem(BaseWriterItem):
+    value: Final[Any]
+    spec: Final[str]
+
+    def __init__(self, value: Any, spec: str) -> None: ...
+
+
+class ComplexArg(BaseWriterItem):
+    name: Final[str]
+    value: Final[Any]
+
+    def __init__(self, name: str, value: Any, *, split_line: bool = ...) -> None: ...
+
+
+WI_NEWLINE: BaseWriterItem
+
+
+_BaseItem = Union[str, bytes, int, float, WriterItemLike]
+_ComplexItem = Union[_BaseItem, List[_BaseItem], Dict[str, _BaseItem]]
+
+
+class BaseWriter(object):
+    indent: Final[int]
+
+    def __init__(self, indent: int = 4, command_threshold: int = 1) -> None: ...
+    def raw_write(self, text: str) -> None: ...
+    def close(self) -> None: ...
+    def inc_indent(self) -> None: ...
+    def dec_indent(self) -> None: ...
+    def newline(self, concat_prev: bool = ...) -> None: ...
+    def write_text(self, text: str) -> None: ...
+    def write_annotation(self, annotation: str) -> None: ...
+    def write_command(self, __name: Union[str, int], *args: _BaseItem, **kwds: _ComplexItem) -> None: ...
+    def write(self, command: Union[str, WriterItemLike]) -> None: ...
+    @property
+    def closed(self) -> bool: ...
+    def __enter__(self) -> Self: ...
+    def __exit__(self, exc_type: Type[BaseException], exc_ins: Exception, traceback: TracebackType) -> None: ...
+
+
+class FileWriter(BaseWriter):
+    path: Final[Union[str, bytes, os.PathLike]]
+    encoding: Final[str]
+
+    def __init__(self, __path: Union[str, bytes, os.PathLike], encoding: str = "utf-8",
+                 indent: int = ..., command_threshold: int = ...) -> None: ...
+
+
+class StringWriter(BaseWriter):
+    def getvalue(self) -> str: ...
```

### Comparing `KoiLang-1.1.1/setup.py` & `KoiLang-1.2.0a0/setup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-"""
-Copyright 2023 Ovizro
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-import os
-import re
-import sys
-import warnings
-from setuptools import setup, Extension
-
-try:
-    with open("README.md", encoding='utf-8') as f:
-        description = f.read()
-except OSError:
-    warnings.warn("Miss file 'README.md', using default description.", ResourceWarning)
-    description = "simple python module for KoiLang parsing"
-
-try:
-    with open("kola/version.py") as f:
-        version = re.search(r"__version__\s*=\s*\"(.*)\"\n", f.read()).group(1) # type: ignore
-except Exception as e:
-    raise ValueError("fail to read kola version") from e
-
-
-USE_CYTHON = "USE_CYTHON" in os.environ
-FILE_SUFFIX = ".pyx" if USE_CYTHON else ".c"
-
-extensions = [
-    Extension("kola.lexer", ["kola/lexer" + FILE_SUFFIX, "kola/unicode_handler.c"]),
-    Extension("kola.parser", ["kola/parser" + FILE_SUFFIX]),
-    Extension("kola.writer", ["kola/writer" + FILE_SUFFIX])
-]
-if USE_CYTHON:
-    from Cython.Build import cythonize
-    from Cython.Compiler import Options
-
-    Options.fast_fail = True
-    extensions = cythonize(extensions, annotate=True, compiler_directives={"language_level": "3"})
-
-
-setup(
-    name="KoiLang",
-    version=version,
-    description="simple python module for KoiLang parsing",
-    long_description=description,
-    long_description_content_type='text/markdown',
-
-    author="Visecy",
-    author_email="Visecy@visecy.top",
-    maintainer="Ovizro",
-    maintainer_email="Ovizro@visecy.top",
-    license="Apache 2.0",
-
-    url="https://github.com/Ovizro/Kola",
-    packages=["kola", "kola/klvm", "kola/lib", "kola/lib/debugger"],
-    python_requires=">=3.6",
-    package_data={'':["*.pyi", "*.pxd", "*.h"]},
-    install_requires=[
-        "typing_extensions>=4.0" if sys.version_info >= (3, 7)
-            else "typing_extensions>=4.0,<4.2"
-    ],
-    ext_modules=extensions,
-
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: C",
-        "Programming Language :: Cython",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Text Processing :: Markup"
-    ]
+"""
+Copyright 2023 Ovizro
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+import os
+import re
+import sys
+import warnings
+from setuptools import setup, Extension
+
+try:
+    with open("README.md", encoding='utf-8') as f:
+        description = f.read()
+except OSError:
+    warnings.warn("Miss file 'README.md', using default description.", ResourceWarning)
+    description = "simple python module for KoiLang parsing"
+
+try:
+    with open("kola/version.py") as f:
+        version = re.search(r"__version__\s*=\s*\"(.*)\"\n", f.read()).group(1) # type: ignore
+except Exception as e:
+    raise ValueError("fail to read kola version") from e
+
+
+USE_CYTHON = "USE_CYTHON" in os.environ
+FILE_SUFFIX = ".pyx" if USE_CYTHON else ".c"
+
+extensions = [
+    Extension("kola.lexer", ["kola/lexer" + FILE_SUFFIX, "kola/unicode_handler.c"]),
+    Extension("kola.parser", ["kola/parser" + FILE_SUFFIX]),
+    Extension("kola.writer", ["kola/writer" + FILE_SUFFIX])
+]
+if USE_CYTHON:
+    from Cython.Build import cythonize
+    from Cython.Compiler import Options
+
+    Options.fast_fail = True
+    extensions = cythonize(extensions, annotate=True, compiler_directives={"language_level": "3"})
+
+
+setup(
+    name="KoiLang",
+    version=version,
+    description="simple python module for KoiLang parsing",
+    long_description=description,
+    long_description_content_type='text/markdown',
+
+    author="Visecy",
+    author_email="Visecy@visecy.top",
+    maintainer="Ovizro",
+    maintainer_email="Ovizro@visecy.top",
+    license="Apache 2.0",
+
+    url="https://github.com/Ovizro/Kola",
+    packages=["kola", "kola/klvm", "kola/lib", "kola/lib/debugger"],
+    python_requires=">=3.6",
+    package_data={'':["*.pyi", "*.pxd", "*.h"]},
+    install_requires=[
+        "typing_extensions>=4.0" if sys.version_info >= (3, 7)
+            else "typing_extensions>=4.0,<4.2"
+    ],
+    ext_modules=extensions,
+
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: C",
+        "Programming Language :: Cython",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Text Processing :: Markup"
+    ]
 )
```

