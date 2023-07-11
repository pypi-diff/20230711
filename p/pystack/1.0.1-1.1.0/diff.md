# Comparing `tmp/pystack-1.0.1.tar.gz` & `tmp/pystack-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystack-1.0.1.tar", last modified: Tue Apr 11 09:48:40 2023, max compression
+gzip compressed data, was "pystack-1.1.0.tar", last modified: Tue Jul 11 16:38:52 2023, max compression
```

## Comparing `pystack-1.0.1.tar` & `pystack-1.1.0.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:48:40.853198 pystack-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-11 09:48:27.000000 pystack-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-11 09:48:27.000000 pystack-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-11 09:48:27.000000 pystack-1.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-04-11 09:48:40.853198 pystack-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-04-11 09:48:27.000000 pystack-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-11 09:48:27.000000 pystack-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 09:48:40.853198 pystack-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-11 09:48:27.000000 pystack-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:48:40.845198 pystack-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:48:40.845198 pystack-1.0.1/src/pystack/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:48:40.849198 pystack-1.0.1/src/pystack/_pystack/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/corefile.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/corefile.h
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/corefile.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:48:40.853198 pystack-1.0.1/src/pystack/_pystack/cpython/
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/code.h
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/dict.h
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/float.h
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/frame.h
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/gc.h
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/int.h
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/interpreter.h
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/list.h
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/object.h
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/pthread.h
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/runtime.h
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/string.h
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/thread.h
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/cpython/tuple.h
--rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/elf_common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/elf_common.h
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/elf_common.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/logging.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/mem.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/mem.h
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/mem.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/native_frame.h
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/native_frame.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/process.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/process.h
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/process.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pycode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pycode.h
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pycode.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pycompat.h
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pyframe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pyframe.h
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pyframe.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pythread.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pythread.h
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pythread.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    21248 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pytypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/pytypes.h
--rw-r--r--   0 runner    (1001) docker     (123)    18145 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/unwinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/unwinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/version.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28543 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_pystack.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/process.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/traceback_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-11 09:48:27.000000 pystack-1.0.1/src/pystack/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:48:40.845198 pystack-1.0.1/src/pystack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-04-11 09:48:40.000000 pystack-1.0.1/src/pystack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-11 09:48:40.000000 pystack-1.0.1/src/pystack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:48:40.000000 pystack-1.0.1/src/pystack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 09:48:40.000000 pystack-1.0.1/src/pystack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 09:48:40.000000 pystack-1.0.1/src/pystack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 09:48:40.000000 pystack-1.0.1/src/pystack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.356092 pystack-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 16:38:39.000000 pystack-1.1.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-11 16:38:39.000000 pystack-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-11 16:38:39.000000 pystack-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-11 16:38:39.000000 pystack-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-11 16:38:39.000000 pystack-1.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-11 16:38:39.000000 pystack-1.1.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-07-11 16:38:52.356092 pystack-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-07-11 16:38:39.000000 pystack-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-11 16:38:39.000000 pystack-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:38:52.356092 pystack-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-11 16:38:39.000000 pystack-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.344092 pystack-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.348092 pystack-1.1.0/src/pystack/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.352092 pystack-1.1.0/src/pystack/_pystack/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/corefile.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/corefile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/corefile.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.356092 pystack-1.1.0/src/pystack/_pystack/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/code.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/dict.h
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/float.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/frame.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/gc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/int.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/interpreter.h
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/list.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/object.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/pthread.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/runtime.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/string.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/thread.h
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/tuple.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/elf_common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/elf_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/elf_common.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/logging.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/mem.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/mem.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/native_frame.h
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/native_frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/process.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/process.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/process.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pycode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pycode.h
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pycode.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pycompat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pyframe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pyframe.h
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pyframe.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pythread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pythread.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pythread.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    21247 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pytypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pytypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/unwinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/unwinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/version.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26996 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/traceback_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.348092 pystack-1.1.0/src/pystack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-07-11 16:38:52.000000 pystack-1.1.0/src/pystack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 16:38:52.000000 pystack-1.1.0/src/pystack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:38:52.000000 pystack-1.1.0/src/pystack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 16:38:52.000000 pystack-1.1.0/src/pystack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 16:38:52.000000 pystack-1.1.0/src/pystack.egg-info/top_level.txt
```

### Comparing `pystack-1.0.1/LICENSE` & `pystack-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/PKG-INFO` & `pystack-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,97 +1,77 @@
-Metadata-Version: 2.1
-Name: pystack
-Version: 1.0.1
-Summary: Analysis of the stack of remote python processes
-Home-page: https://github.com/bloomberg/pystack
-Author: Pablo Galindo Salgado
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Debuggers
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-Provides-Extra: lint
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="center">
 <img src="https://user-images.githubusercontent.com/11718525/226942590-de015c9a-4d5b-4960-9c42-8c1eac0845c1.png" width="70%">
 </p>
 
----
+______________________________________________________________________
 
 ![OS Linux](https://img.shields.io/badge/OS-Linux-blue)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pystack)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/pystack)
 ![PyPI](https://img.shields.io/pypi/v/pystack)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pystack)
 [![Tests](https://github.com/bloomberg/pystack/actions/workflows/build_wheels.yml/badge.svg)](https://github.com/bloomberg/pystack/actions/workflows/build_wheels.yml)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # PyStack
 
 > Print the stack trace of a running Python process, or of a Python core dump.
 
 PyStack is a tool that uses forbidden magic to let you inspect the stack frames of a running Python
-process or a Python core dump, helping you quickly and easily learn what it's doing (or what it was doing
-when it crashed) without having to interpret nasty CPython internals.
+process or a Python core dump, helping you quickly and easily learn what it's doing (or what it was
+doing when it crashed) without having to interpret nasty CPython internals.
 
 # What PyStack can do
 
 PyStack has the following amazing features:
 
 - 💻 Works with both running processes and core dump files.
-- 🧵 Shows if each thread currently holds the Python GIL, is waiting to acquire it, or is
-  currently dropping it.
+- 🧵 Shows if each thread currently holds the Python GIL, is waiting to acquire it, or is currently
+  dropping it.
 - 🗑️ Shows if a thread is running a garbage collection cycle.
 - 🐍 Optionally shows native function calls, as well as Python ones. In this mode, PyStack prints
   the native stack trace (C/C++/Rust function calls), except that the calls to Python callables are
   replaced with frames showing the Python code being executed, instead of showing the internal C
   code the interpreter used to make the call.
 - 🔍 Automatically demangles symbols shown in the native stack.
 - 📈 Includes calls to inlined functions in the native stack whenever enough debug information is
   available.
 - 🔍 Optionally shows the values of local variables and function arguments in Python stack frames.
-- 🔒 Safe to use on running processes. PyStack does not modify any memory or execute any code in
-  a process that is running. It simply attaches just long enough to read some of the process's memory.
+- 🔒 Safe to use on running processes. PyStack does not modify any memory or execute any code in a
+  process that is running. It simply attaches just long enough to read some of the process's
+  memory.
 - ⚡ Optionally, it can perform a Python stack analysis without pausing the process at all. This
   minimizes impact to the debugged process, at the cost of potentially failing due to data races.
 - 🚀 Super fast! It can analyze core files 10x faster than general-purpose tools like GDB.
 - 🎯 Even works with aggressively optimized Python interpreter binaries.
 - 🔍 Even works with Python interpreters' binaries that do not have symbols or debug information
   (Python stack only).
-- 💥 Tolerates memory corruption well. Even if the process crashed due to memory corruption, PyStack
-  can usually reconstruct the stack.
+- 💥 Tolerates memory corruption well. Even if the process crashed due to memory corruption,
+  PyStack can usually reconstruct the stack.
 - 💼 Self-contained: it does not depend on external tools or programs other than the Python
   interpreter used to run PyStack itself.
 
 ## Building from source
 
-If you wish to build PyStack from source, you need the following binary dependencies in your system:
+If you wish to build PyStack from source, you need the following binary dependencies in your
+system:
 
 - libdw
 - libelf
 
 Note that sometimes both libraries are provided together as part of a distribution's `elfutils`
 package.
 
 Check your package manager on how to install these dependencies (e.g.,
 `apt-get install libdw-dev libelf-dev` in Debian-based systems). Note that you may need to tell the
-compiler where to find the header and library files of the dependencies for the build to
-succeed. Check your distribution's documentation to determine the location of the header and
-library files or for more detailed information.
+compiler where to find the header and library files of the dependencies for the build to succeed.
+Check your distribution's documentation to determine the location of the header and library files
+or for more detailed information. When building on Alpine Linux (or any other distribution that
+doesn't use glibc) you'll need elfutils 0.188 or newer. You may need to build this from source if
+your distribution's package manager doesn't have it.
 
 Once you have these binary dependencies installed, you can clone the repository and follow the
 typical build process for Python libraries:
 
 ```shell
 git clone git@github.com:bloomberg/pystack.git pystack
 cd pystack
@@ -102,14 +82,22 @@
 python3 -m pip install -r requirements-test.txt -r requirements-extra.txt
 ```
 
 This will install PyStack in the virtual environment in development mode (the `-e` of the last
 `pip install` command), and then install the Python libraries needed to test it, lint it, and
 generate its documentation.
 
+If you plan to contribute back, you should install the pre-commit hooks:
+
+```shell
+pre-commit install
+```
+
+This will ensure that your contribution passes our linting checks.
+
 # Documentation
 
 You can find the full documentation [here](https://bloomberg.github.io/pystack/).
 
 # Usage
 
 PyStack uses distinct subcommands for analyzing running processes and core dump files.
@@ -129,19 +117,19 @@
     remote       Analyze a remote process given its PID
     core         Analyze a core dump file given its location and the executable
 ```
 
 ## Analyzing running processes
 
 The `remote` command is used to analyze the status of a running (remote) process. The analysis is
-always done in a safe and non-intrusive way, as no code is loaded in the memory space of the process
-under analysis and no memory is modified in the remote process. This makes analysis using PyStack a
-great option even for those services and applications that are running in environments where the running process
-must not be impacted in any way (other than being temporarily paused, though `--no-block` can avoid
-even that). There are several options available:
+always done in a safe and non-intrusive way, as no code is loaded in the memory space of the
+process under analysis and no memory is modified in the remote process. This makes analysis using
+PyStack a great option even for those services and applications that are running in environments
+where the running process must not be impacted in any way (other than being temporarily paused,
+though `--no-block` can avoid even that). There are several options available:
 
 ```shell
 usage: pystack remote [-h] [-v] [--no-color] [--no-block] [--native] [--native-all] [--locals] [--exhaustive] [--self] pid
 
 positional arguments:
   pid            The PID of the remote process
 
@@ -172,17 +160,17 @@
 ```
 
 ## Analyzing core dumps
 
 The `core` subcommand is used to analyze the status of a core dump file. Analyzing core files is
 very similar to analyzing processes but there are some differences, as the core file does not
 contain the totality of the memory that was valid when the program was live. In most cases, this
-makes no difference, as PyStack will try to adapt automatically. However, in some cases, you will need to
-specify extra command line options to help PyStack locate the information it needs. When analyzing
-cores, there are several options available:
+makes no difference, as PyStack will try to adapt automatically. However, in some cases, you will
+need to specify extra command line options to help PyStack locate the information it needs. When
+analyzing cores, there are several options available:
 
 ```shell
 usage: pystack core [-h] [-v] [--no-color] [--native] [--native-all] [--locals] [--exhaustive] [--lib-search-path LIB_SEARCH_PATH | --lib-search-root LIB_SEARCH_ROOT] core [executable]
 
 positional arguments:
   core                  The path to the core file
   executable            (Optional) The path to the executable of the core file
@@ -197,15 +185,16 @@
   --exhaustive          Use all possible methods to obtain the Python stack info (may be slow)
   --lib-search-path LIB_SEARCH_PATH
                         List of paths to search for shared libraries loaded in the core. Paths must be separated by the ':' character
   --lib-search-root LIB_SEARCH_ROOT
                         Root directory to search recursively for shared libraries loaded into the core.
 ```
 
-In most cases, you just need to provide the location of the core to use PyStack with core dump files:
+In most cases, you just need to provide the location of the core to use PyStack with core dump
+files:
 
 ```shell
 $ pystack core ./the_core_file
 Using executable found in the core file: /usr/bin/python3.8
 
 Core file information:
 state: t zombie: True niceness: 0
@@ -255,25 +244,26 @@
 any questions about this process or any other aspect of contributing to a Bloomberg open source
 project, feel free to send an email to opensource@bloomberg.net and we'll get your questions
 answered as quickly as we can.
 
 ## Contribution Licensing
 
 Since this project is distributed under the terms of an [open source license](LICENSE),
-contributions that you make are licensed under the same terms. For us to be able to accept
-your contributions, we will need explicit confirmation from you that you are able and willing to
-provide them under these terms, and the mechanism we use to do this is called a Developer's
-Certificate of Origin [(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is
-similar to the process used by the Linux(R) kernel, Samba, and many other major open source
-projects.
+contributions that you make are licensed under the same terms. For us to be able to accept your
+contributions, we will need explicit confirmation from you that you are able and willing to provide
+them under these terms, and the mechanism we use to do this is called a Developer's Certificate of
+Origin [(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is similar to the
+process used by the Linux kernel, Samba, and many other major open source projects.
 
 To participate under these terms, all that you must do is include a line like the following as the
 last line of the commit message for each commit in your contribution:
 
-    Signed-Off-By: Random J. Developer <random@developer.example.org>
+```
+Signed-Off-By: Random J. Developer <random@developer.example.org>
+```
 
 The simplest way to accomplish this is to add `-s` or `--signoff` to your `git commit` command.
 
 You must use your real name (sorry, no pseudonyms, and no anonymous contributions).
 
 ## Steps
```

### Comparing `pystack-1.0.1/README.md` & `pystack-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,97 @@
+Metadata-Version: 2.1
+Name: pystack
+Version: 1.1.0
+Summary: Analysis of the stack of remote python processes
+Home-page: https://github.com/bloomberg/pystack
+Author: Pablo Galindo Salgado
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Debuggers
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
 <img src="https://user-images.githubusercontent.com/11718525/226942590-de015c9a-4d5b-4960-9c42-8c1eac0845c1.png" width="70%">
 </p>
 
----
+______________________________________________________________________
 
 ![OS Linux](https://img.shields.io/badge/OS-Linux-blue)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pystack)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/pystack)
 ![PyPI](https://img.shields.io/pypi/v/pystack)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pystack)
 [![Tests](https://github.com/bloomberg/pystack/actions/workflows/build_wheels.yml/badge.svg)](https://github.com/bloomberg/pystack/actions/workflows/build_wheels.yml)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # PyStack
 
 > Print the stack trace of a running Python process, or of a Python core dump.
 
 PyStack is a tool that uses forbidden magic to let you inspect the stack frames of a running Python
-process or a Python core dump, helping you quickly and easily learn what it's doing (or what it was doing
-when it crashed) without having to interpret nasty CPython internals.
+process or a Python core dump, helping you quickly and easily learn what it's doing (or what it was
+doing when it crashed) without having to interpret nasty CPython internals.
 
 # What PyStack can do
 
 PyStack has the following amazing features:
 
 - 💻 Works with both running processes and core dump files.
-- 🧵 Shows if each thread currently holds the Python GIL, is waiting to acquire it, or is
-  currently dropping it.
+- 🧵 Shows if each thread currently holds the Python GIL, is waiting to acquire it, or is currently
+  dropping it.
 - 🗑️ Shows if a thread is running a garbage collection cycle.
 - 🐍 Optionally shows native function calls, as well as Python ones. In this mode, PyStack prints
   the native stack trace (C/C++/Rust function calls), except that the calls to Python callables are
   replaced with frames showing the Python code being executed, instead of showing the internal C
   code the interpreter used to make the call.
 - 🔍 Automatically demangles symbols shown in the native stack.
 - 📈 Includes calls to inlined functions in the native stack whenever enough debug information is
   available.
 - 🔍 Optionally shows the values of local variables and function arguments in Python stack frames.
-- 🔒 Safe to use on running processes. PyStack does not modify any memory or execute any code in
-  a process that is running. It simply attaches just long enough to read some of the process's memory.
+- 🔒 Safe to use on running processes. PyStack does not modify any memory or execute any code in a
+  process that is running. It simply attaches just long enough to read some of the process's
+  memory.
 - ⚡ Optionally, it can perform a Python stack analysis without pausing the process at all. This
   minimizes impact to the debugged process, at the cost of potentially failing due to data races.
 - 🚀 Super fast! It can analyze core files 10x faster than general-purpose tools like GDB.
 - 🎯 Even works with aggressively optimized Python interpreter binaries.
 - 🔍 Even works with Python interpreters' binaries that do not have symbols or debug information
   (Python stack only).
-- 💥 Tolerates memory corruption well. Even if the process crashed due to memory corruption, PyStack
-  can usually reconstruct the stack.
+- 💥 Tolerates memory corruption well. Even if the process crashed due to memory corruption,
+  PyStack can usually reconstruct the stack.
 - 💼 Self-contained: it does not depend on external tools or programs other than the Python
   interpreter used to run PyStack itself.
 
 ## Building from source
 
-If you wish to build PyStack from source, you need the following binary dependencies in your system:
+If you wish to build PyStack from source, you need the following binary dependencies in your
+system:
 
 - libdw
 - libelf
 
 Note that sometimes both libraries are provided together as part of a distribution's `elfutils`
 package.
 
 Check your package manager on how to install these dependencies (e.g.,
 `apt-get install libdw-dev libelf-dev` in Debian-based systems). Note that you may need to tell the
-compiler where to find the header and library files of the dependencies for the build to
-succeed. Check your distribution's documentation to determine the location of the header and
-library files or for more detailed information.
+compiler where to find the header and library files of the dependencies for the build to succeed.
+Check your distribution's documentation to determine the location of the header and library files
+or for more detailed information. When building on Alpine Linux (or any other distribution that
+doesn't use glibc) you'll need elfutils 0.188 or newer. You may need to build this from source if
+your distribution's package manager doesn't have it.
 
 Once you have these binary dependencies installed, you can clone the repository and follow the
 typical build process for Python libraries:
 
 ```shell
 git clone git@github.com:bloomberg/pystack.git pystack
 cd pystack
@@ -78,14 +102,22 @@
 python3 -m pip install -r requirements-test.txt -r requirements-extra.txt
 ```
 
 This will install PyStack in the virtual environment in development mode (the `-e` of the last
 `pip install` command), and then install the Python libraries needed to test it, lint it, and
 generate its documentation.
 
+If you plan to contribute back, you should install the pre-commit hooks:
+
+```shell
+pre-commit install
+```
+
+This will ensure that your contribution passes our linting checks.
+
 # Documentation
 
 You can find the full documentation [here](https://bloomberg.github.io/pystack/).
 
 # Usage
 
 PyStack uses distinct subcommands for analyzing running processes and core dump files.
@@ -105,19 +137,19 @@
     remote       Analyze a remote process given its PID
     core         Analyze a core dump file given its location and the executable
 ```
 
 ## Analyzing running processes
 
 The `remote` command is used to analyze the status of a running (remote) process. The analysis is
-always done in a safe and non-intrusive way, as no code is loaded in the memory space of the process
-under analysis and no memory is modified in the remote process. This makes analysis using PyStack a
-great option even for those services and applications that are running in environments where the running process
-must not be impacted in any way (other than being temporarily paused, though `--no-block` can avoid
-even that). There are several options available:
+always done in a safe and non-intrusive way, as no code is loaded in the memory space of the
+process under analysis and no memory is modified in the remote process. This makes analysis using
+PyStack a great option even for those services and applications that are running in environments
+where the running process must not be impacted in any way (other than being temporarily paused,
+though `--no-block` can avoid even that). There are several options available:
 
 ```shell
 usage: pystack remote [-h] [-v] [--no-color] [--no-block] [--native] [--native-all] [--locals] [--exhaustive] [--self] pid
 
 positional arguments:
   pid            The PID of the remote process
 
@@ -148,17 +180,17 @@
 ```
 
 ## Analyzing core dumps
 
 The `core` subcommand is used to analyze the status of a core dump file. Analyzing core files is
 very similar to analyzing processes but there are some differences, as the core file does not
 contain the totality of the memory that was valid when the program was live. In most cases, this
-makes no difference, as PyStack will try to adapt automatically. However, in some cases, you will need to
-specify extra command line options to help PyStack locate the information it needs. When analyzing
-cores, there are several options available:
+makes no difference, as PyStack will try to adapt automatically. However, in some cases, you will
+need to specify extra command line options to help PyStack locate the information it needs. When
+analyzing cores, there are several options available:
 
 ```shell
 usage: pystack core [-h] [-v] [--no-color] [--native] [--native-all] [--locals] [--exhaustive] [--lib-search-path LIB_SEARCH_PATH | --lib-search-root LIB_SEARCH_ROOT] core [executable]
 
 positional arguments:
   core                  The path to the core file
   executable            (Optional) The path to the executable of the core file
@@ -173,15 +205,16 @@
   --exhaustive          Use all possible methods to obtain the Python stack info (may be slow)
   --lib-search-path LIB_SEARCH_PATH
                         List of paths to search for shared libraries loaded in the core. Paths must be separated by the ':' character
   --lib-search-root LIB_SEARCH_ROOT
                         Root directory to search recursively for shared libraries loaded into the core.
 ```
 
-In most cases, you just need to provide the location of the core to use PyStack with core dump files:
+In most cases, you just need to provide the location of the core to use PyStack with core dump
+files:
 
 ```shell
 $ pystack core ./the_core_file
 Using executable found in the core file: /usr/bin/python3.8
 
 Core file information:
 state: t zombie: True niceness: 0
@@ -231,25 +264,26 @@
 any questions about this process or any other aspect of contributing to a Bloomberg open source
 project, feel free to send an email to opensource@bloomberg.net and we'll get your questions
 answered as quickly as we can.
 
 ## Contribution Licensing
 
 Since this project is distributed under the terms of an [open source license](LICENSE),
-contributions that you make are licensed under the same terms. For us to be able to accept
-your contributions, we will need explicit confirmation from you that you are able and willing to
-provide them under these terms, and the mechanism we use to do this is called a Developer's
-Certificate of Origin [(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is
-similar to the process used by the Linux(R) kernel, Samba, and many other major open source
-projects.
+contributions that you make are licensed under the same terms. For us to be able to accept your
+contributions, we will need explicit confirmation from you that you are able and willing to provide
+them under these terms, and the mechanism we use to do this is called a Developer's Certificate of
+Origin [(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is similar to the
+process used by the Linux kernel, Samba, and many other major open source projects.
 
 To participate under these terms, all that you must do is include a line like the following as the
 last line of the commit message for each commit in your contribution:
 
-    Signed-Off-By: Random J. Developer <random@developer.example.org>
+```
+Signed-Off-By: Random J. Developer <random@developer.example.org>
+```
 
 The simplest way to accomplish this is to add `-s` or `--signoff` to your `git commit` command.
 
 You must use your real name (sorry, no pseudonyms, and no anonymous contributions).
 
 ## Steps
```

### Comparing `pystack-1.0.1/setup.py` & `pystack-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,16 @@
-from distutils.core import setup
 import os
-import sys
 import pathlib
+import sys
+from distutils.core import setup
 
-from setuptools import Extension
 from Cython.Build import cythonize
+from setuptools import Extension
 
 install_requires = []
-docs_requires = [
-    "bump2version",
-    "recommonmark",
-    "sphinx",
-    "furo",
-    "sphinx-autobuild",
-    "sphinx-argparse",
-    "towncrier",
-]
-
-lint_requires = [
-    "black",
-    "flake8",
-    "isort",
-    "mypy",
-]
-
-test_requires = [
-    "Cython",
-    "pytest",
-    "pytest-xdist",
-    "pytest-cov",
-]
 
 
 TEST_BUILD = False
 if "--test-build" in sys.argv:
     TEST_BUILD = True
     sys.argv.remove("--test-build")
 
@@ -132,17 +109,11 @@
     ext_modules=cythonize(
         [PYSTACK_EXTENSION],
         include_path=["src/pystack"],
         compiler_directives=COMPILER_DIRECTIVES,
     ),
     install_requires=install_requires,
     include_package_data=True,
-    extras_require={
-        "test": test_requires,
-        "docs": docs_requires,
-        "lint": lint_requires,
-        "dev": test_requires + lint_requires + docs_requires,
-    },
     entry_points={
         "console_scripts": ["pystack=pystack.__main__:main"],
     },
 )
```

### Comparing `pystack-1.0.1/src/pystack/__main__.py` & `pystack-1.1.0/src/pystack/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sys
 from contextlib import suppress
 from textwrap import dedent
 from typing import Any
 from typing import Dict
 from typing import NoReturn
 from typing import Optional
+from typing import Set
 
 from pystack.errors import InvalidPythonProcess
 from pystack.process import is_elf
 
 from . import errors
 from . import print_thread
 from .colors import colored
@@ -338,15 +339,15 @@
     if not executable.exists():
         parser.error(f"Executable {executable} does not exist")
 
     lib_search_path = ""
     if args.lib_search_path:
         lib_search_path = args.lib_search_path
     if args.lib_search_root:
-        library_dirs = set()
+        library_dirs: Set[str] = set()
         for pattern in {"**/*.so", "**/*.so.*"}:
             library_dirs.update(
                 str(file.parent)
                 for file in pathlib.Path(args.lib_search_root).glob(pattern)
             )
         lib_search_path = ":".join(sorted(library_dirs))
     LOGGER.info("Using library search path: %s", lib_search_path)
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/CMakeLists.txt` & `pystack-1.1.0/src/pystack/_pystack/CMakeLists.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 cmake_minimum_required(VERSION 2.8)
 project(_pystack)
 set(CMAKE_CXX_STANDARD 17)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
-include_directories(/opt/bb/include/)
-
 find_package(PythonInterp 3.7 REQUIRED)
 find_package(PythonLibs 3.7 REQUIRED)
 IF(NOT PYTHONLIBS_FOUND OR NOT PYTHON_EXECUTABLE)
     MESSAGE(SEND_ERROR "You need Python to build Python binding")
 ENDIF(NOT PYTHONLIBS_FOUND OR NOT PYTHON_EXECUTABLE)
 
 add_library(_pystack STATIC
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/compat.h` & `pystack-1.1.0/src/pystack/_pystack/compat.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/corefile.cpp` & `pystack-1.1.0/src/pystack/_pystack/corefile.cpp`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/corefile.h` & `pystack-1.1.0/src/pystack/_pystack/corefile.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/corefile.pxd` & `pystack-1.1.0/src/pystack/_pystack/corefile.pxd`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/cpython/code.h` & `pystack-1.1.0/src/pystack/_pystack/cpython/code.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/cpython/dict.h` & `pystack-1.1.0/src/pystack/_pystack/cpython/dict.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/cpython/frame.h` & `pystack-1.1.0/src/pystack/_pystack/cpython/frame.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/cpython/gc.h` & `pystack-1.1.0/src/pystack/_pystack/cpython/gc.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/cpython/interpreter.h` & `pystack-1.1.0/src/pystack/_pystack/cpython/interpreter.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/cpython/object.h` & `pystack-1.1.0/src/pystack/_pystack/cpython/object.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/cpython/pthread.h` & `pystack-1.1.0/src/pystack/_pystack/cpython/pthread.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/cpython/runtime.h` & `pystack-1.1.0/src/pystack/_pystack/cpython/runtime.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/cpython/string.h` & `pystack-1.1.0/src/pystack/_pystack/cpython/string.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/cpython/thread.h` & `pystack-1.1.0/src/pystack/_pystack/cpython/thread.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/elf_common.cpp` & `pystack-1.1.0/src/pystack/_pystack/elf_common.cpp`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/elf_common.h` & `pystack-1.1.0/src/pystack/_pystack/elf_common.h`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     std::optional<std::string> d_executable;
     std::optional<std::string> d_lib_search_path;
     int d_fd;
     int d_pid;
     elf_unique_ptr d_elf;
     std::vector<std::string> d_missing_modules{};
 
-private:
+  private:
     void removeModuleIf(std::function<bool(Dwfl_Module*)> predicate) const;
     void resolveLibraries();
 };
 
 class ProcessAnalyzer : public Analyzer
 {
   public:
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/elf_common.pxd` & `pystack-1.1.0/src/pystack/_pystack/elf_common.pxd`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/logging.cpp` & `pystack-1.1.0/src/pystack/_pystack/logging.cpp`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/logging.h` & `pystack-1.1.0/src/pystack/_pystack/logging.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/mem.cpp` & `pystack-1.1.0/src/pystack/_pystack/mem.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -198,19 +198,20 @@
 : ProcessMemoryManager(pid)
 , d_tids(tids)
 {
     for (auto& tid : tids) {
         LOG(INFO) << "Trying to stop thread " << tid;
         long ret = ptrace(PTRACE_ATTACH, tid, nullptr, nullptr);
         if (ret < 0) {
+            int error = errno;
             detachFromProcess();
-            if (errno == EPERM) {
+            if (error == EPERM) {
                 throw std::runtime_error(PERM_MESSAGE);
             }
-            throw std::system_error(errno, std::generic_category());
+            throw std::system_error(error, std::generic_category());
         }
         LOG(INFO) << "Waiting for thread " << tid << " to be stopped";
         ret = waitpid(tid, nullptr, WUNTRACED);
         if (ret < 0) {
             // In some old kernels is not possible to use WUNTRACED with
             // threads (only the main thread will return a non zero value).
             if (tid == pid || errno != ECHILD) {
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/mem.h` & `pystack-1.1.0/src/pystack/_pystack/mem.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/mem.pxd` & `pystack-1.1.0/src/pystack/_pystack/mem.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,13 @@
         cppstring buildid
 
     cdef cppclass VirtualMap:
         VirtualMap()
         VirtualMap(uintptr_t start, uintptr_t end, unsigned long filesize,
                    cppstring flags, unsigned long offset, cppstring permissions,
                    unsigned long inode, cppstring pathname)
-    
+
     cdef cppclass MemoryMapInformation:
         MemoryMapInformation()
         void setMainMap(const VirtualMap& bss)
         void setBss(const VirtualMap& bss)
         void setHeap(const VirtualMap& heap)
-
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/process.cpp` & `pystack-1.1.0/src/pystack/_pystack/process.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -510,15 +510,16 @@
 
 int
 AbstractProcessManager::minorVersion() const
 {
     return d_minor;
 }
 
-const python_v& AbstractProcessManager::offsets() const
+const python_v&
+AbstractProcessManager::offsets() const
 {
     return *d_py_v;
 }
 
 remote_addr_t
 AbstractProcessManager::findInterpreterStateFromElfData() const
 {
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/process.h` & `pystack-1.1.0/src/pystack/_pystack/process.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/process.pxd` & `pystack-1.1.0/src/pystack/_pystack/process.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from libcpp.string cimport string as cppstring
 from libcpp.utility cimport pair
 from libcpp.vector cimport vector
 
 
 cdef extern from "process.h" namespace "pystack::AbstractProcessManager":
     cdef enum InterpreterStatus:
-        RUNNING = 1
-        FINALIZED = 0
-        UNKNOWN = -1
+        RUNNING
+        FINALIZED
+        UNKNOWN
 
 cdef extern from "process.h" namespace "pystack":
     cdef cppclass AbstractProcessManager:
         remote_addr_t scanBSS() except+
         remote_addr_t scanHeap() except+
         remote_addr_t scanAllAnonymousMaps() except+
         remote_addr_t findInterpreterStateFromSymbols() except+
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/pycode.cpp` & `pystack-1.1.0/src/pystack/_pystack/pycode.cpp`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/pycode.h` & `pystack-1.1.0/src/pystack/_pystack/pycode.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/pyframe.cpp` & `pystack-1.1.0/src/pystack/_pystack/pyframe.cpp`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/pyframe.h` & `pystack-1.1.0/src/pystack/_pystack/pyframe.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/pyframe.pxd` & `pystack-1.1.0/src/pystack/_pystack/pyframe.pxd`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/pythread.cpp` & `pystack-1.1.0/src/pystack/_pystack/pythread.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,16 @@
     if (frame_addr != (remote_addr_t) nullptr) {
         LOG(DEBUG) << std::hex << std::showbase << "Attempting to construct frame from address "
                    << frame_addr;
         d_first_frame = std::make_unique<FrameObject>(manager, frame_addr, 0);
     }
 
     d_addr = addr;
-    remote_addr_t candidate_next_addr = manager->versionedThreadField<remote_addr_t, &py_thread_v::o_next>(ts);
+    remote_addr_t candidate_next_addr =
+            manager->versionedThreadField<remote_addr_t, &py_thread_v::o_next>(ts);
     d_next_addr = candidate_next_addr == addr ? (remote_addr_t) nullptr : candidate_next_addr;
 
     d_pthread_id = manager->versionedThreadField<unsigned long, &py_thread_v::o_thread_id>(ts);
     d_tid = getThreadTid(manager, addr, d_pthread_id);
     d_next = nullptr;
 
     if (d_next_addr != (remote_addr_t)NULL) {
@@ -213,15 +214,16 @@
 remote_addr_t
 PyThread::getFrameAddr(
         const std::shared_ptr<const AbstractProcessManager>& manager,
         const PyThreadState& ts)
 {
     if (manager->majorVersion() > 3 || (manager->majorVersion() == 3 && manager->minorVersion() >= 11)) {
         Python3_11::CFrame cframe;
-        remote_addr_t cframe_addr = manager->versionedThreadField<remote_addr_t, &py_thread_v::o_frame>(ts);
+        remote_addr_t cframe_addr =
+                manager->versionedThreadField<remote_addr_t, &py_thread_v::o_frame>(ts);
         if (!manager->isAddressValid(cframe_addr)) {
             return reinterpret_cast<remote_addr_t>(nullptr);
         }
         manager->copyObjectFromProcess(cframe_addr, &cframe);
         return reinterpret_cast<remote_addr_t>(cframe.current_frame);
     } else {
         return manager->versionedThreadField<remote_addr_t, &py_thread_v::o_frame>(ts);
@@ -372,12 +374,13 @@
         tid_offset_in_pthread_struct = findPthreadTidOffset(manager, addr);
     }
 
     LOG(DEBUG) << std::hex << std::showbase << "Copying PyInterpreterState struct from address " << addr;
     PyInterpreterState is;
     manager->copyObjectFromProcess(addr, &is);
 
-    auto thread_addr = manager->versionedInterpreterStateField<remote_addr_t, &py_is_v::o_tstate_head>(is);
+    auto thread_addr =
+            manager->versionedInterpreterStateField<remote_addr_t, &py_is_v::o_tstate_head>(is);
     return std::make_shared<PyThread>(manager, thread_addr);
 }
 
 }  // namespace pystack
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/pythread.h` & `pystack-1.1.0/src/pystack/_pystack/pythread.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/pythread.pxd` & `pystack-1.1.0/src/pystack/_pystack/pythread.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,7 @@
         shared_ptr[FrameObject] FirstFrame()
         shared_ptr[Thread] NextThread()
         vector[NativeFrame]& NativeFrames()
         GilStatus isGilHolder()
         GCStatus isGCCollecting()
         void populateNativeStackTrace(shared_ptr[AbstractProcessManager] manager) except+
     shared_ptr[Thread] getThreadFromInterpreterState(shared_ptr[AbstractProcessManager] manager, remote_addr_t addr) except+
-
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/pytypes.cpp` & `pystack-1.1.0/src/pystack/_pystack/pytypes.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -613,15 +613,14 @@
              | Pystack_TPFLAGS_DICT_SUBCLASS
              | Pystack_TPFLAGS_BASE_EXC_SUBCLASS
              | Pystack_TPFLAGS_TYPE_SUBCLASS);
     // clang-format on
 
     const long subclass_flags = d_flags & subclass_mask;
 
-
     if (subclass_flags == Pystack_TPFLAGS_BYTES_SUBCLASS) {
         return d_manager->majorVersion() > 2 ? ObjectType::BYTES : ObjectType::STRING;
     } else if (subclass_flags == Pystack_TPFLAGS_UNICODE_SUBCLASS) {
         return ObjectType::STRING;
     } else if (subclass_flags == Pystack_TPFLAGS_INT_SUBCLASS) {
         if (d_classname == "bool") {
             return ObjectType::INT_BOOL;
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/pytypes.h` & `pystack-1.1.0/src/pystack/_pystack/pytypes.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/unwinder.cpp` & `pystack-1.1.0/src/pystack/_pystack/unwinder.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -81,42 +81,62 @@
     Dwarf_Addr pc;
     bool isActivation;
     if (!dwfl_frame_pc(state, &pc, &isActivation)) {
         LOG(DEBUG) << "dwfl_frame_pc failed";
         return -1;
     }
 
+    std::optional<Dwarf_Word> stackPointer;
+    // Unwinding through musl libc with elfutils can get stuck returning the
+    // same PC in a loop forever.
+    //
+    //   https://sourceware.org/bugzilla/show_bug.cgi?id=30272
+    //   https://marc.info/?l=musl&m=168053842303968&w=2
+    //
+    // We can work around this by asking elfutils what the stack pointer is for
+    // each frame and breaking out on our own if two different frames report
+    // the same stack pointer. When PyStack is built with glibc and not built
+    // with a recent enough version of elfutils for us to do this check, we
+    // skip it. This isn't entirely correct, as it means that a PyStack built
+    // with glibc and an old elfutils can fail to collect stacks for Python
+    // interpreters built against musl libc, but it avoids a hard dependency on
+    // a newer version of elfutils than most distros have available. It's
+    // unlikely that users will encounter problems, but if they do, the simple
+    // work around is to install PyStack using the same interpreter they want
+    // to get stacks for, or to build with a more recent version of elfutils.
+
+#if _ELFUTILS_VERSION >= 188 or (defined(__linux__) && !defined(__GLIBC__))
+
     // These platform specific magic numbers are part of the platform ABI.
     // For any platform not handled below we never look up the value of the
     // stack pointer register, and so never return DWARF_CB_ABORT.
-    std::optional<Dwarf_Word> stackPointer;
     std::optional<unsigned int> stackPointerRegNo;
-
-#if defined(__linux__) && defined(__x86_64__)
+#    if defined(__x86_64__)
     // https://refspecs.linuxbase.org/elf/x86_64-abi-0.99.pdf
     // Figure 3.36: DWARF Register Number Mapping
     stackPointerRegNo = 7;
-#elif defined(__linux__) && defined(__aarch64__)
+#    elif defined(__aarch64__)
     // https://refspecs.linuxfoundation.org/ELF/ppc64/PPC-elf64abi.html#DW-REG
     stackPointerRegNo = 31;
-#endif
+#    endif
 
     if (stackPointerRegNo) {
         stackPointer.emplace(0);
         if (0 != dwfl_frame_reg(state, stackPointerRegNo.value(), &stackPointer.value())) {
             throw UnwinderError("Invalid register number!");
         }
     }
 
     if (!frames->empty() && pc == frames->back().pc && isActivation == frames->back().isActivation
         && stackPointer && stackPointer == frames->back().stackPointer)
     {
         LOG(DEBUG) << std::hex << std::showbase << "Breaking out of (infinite?) unwind loop @ " << pc;
         return DWARF_CB_ABORT;
     }
+#endif
 
     frames->emplace_back(pc, isActivation, stackPointer);
     return DWARF_CB_OK;
 }
 
 static void
 gatherInformationFromDIE(Dwarf_Die* cudie, Dwarf_Die* die, int* line, int* col, const char** sname)
@@ -421,15 +441,16 @@
         case DWARF_CB_ABORT:
             break;
         case -1:
             // This may or may not be an error, as it can signal the end of the stack
             // unwinding.
             if (frames.empty()) {
                 int dwfl_err = dwfl_errno();
-                std::string error(dwfl_errmsg(dwfl_err));
+                std::string error(
+                        dwfl_err ? dwfl_errmsg(dwfl_err) : "unwinding failed with no error reported");
                 throw UnwinderError("Unknown error happened when gathering thread frames: " + error);
             }
             break;
         default:
             throw UnwinderError("Unknown error happened when gathering thread frames");
     }
     return gatherFrames(frames);
@@ -468,15 +489,16 @@
         case DWARF_CB_ABORT:
             break;
         case -1:
             // This may or may not be an error, as it can signal the end of the stack
             // unwinding.
             if (thread_arg->frames.empty()) {
                 int dwfl_err = dwfl_errno();
-                std::string error(dwfl_errmsg(dwfl_err));
+                std::string error(
+                        dwfl_err ? dwfl_errmsg(dwfl_err) : "unwinding failed with no error reported");
                 throw UnwinderError("Unknown error happened when gathering thread frames: " + error);
             }
             break;
         default:
             throw UnwinderError("Unknown error happened when gathering thread frames");
     }
     return DWARF_CB_OK;
@@ -501,15 +523,16 @@
         case DWARF_CB_ABORT:
             break;
         case -1:
             // This may or may not be an error, as it can signal the end of the stack
             // unwinding.
             if (frames.empty()) {
                 int dwfl_err = dwfl_errno();
-                std::string error(dwfl_errmsg(dwfl_err));
+                std::string error(
+                        dwfl_err ? dwfl_errmsg(dwfl_err) : "unwinding failed with no error reported");
                 throw UnwinderError("Unknown error happened when gathering thread frames: " + error);
             }
             break;
         default:
             throw UnwinderError("Unknown error happened when gathering thread frames");
     }
     return gatherFrames(frames);
```

### Comparing `pystack-1.0.1/src/pystack/_pystack/unwinder.h` & `pystack-1.1.0/src/pystack/_pystack/unwinder.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/version.cpp` & `pystack-1.1.0/src/pystack/_pystack/version.cpp`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack/version.h` & `pystack-1.1.0/src/pystack/_pystack/version.h`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/_pystack.pyi` & `pystack-1.1.0/src/pystack/_pystack.pyi`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import enum
 import pathlib
 from typing import Any
 from typing import Dict
 from typing import Iterable
 from typing import List
+from typing import Optional
 from typing import Tuple
 from typing import Union
-from typing import Optional
 
 from .types import PyThread
 
 class CoreFileAnalyzer:
     @classmethod
     def __init__(cls, *args: Any, **kwargs: Any) -> None: ...
     def extract_module_load_points(self) -> Dict[str, int]: ...
```

### Comparing `pystack-1.0.1/src/pystack/_pystack.pyx` & `pystack-1.1.0/src/pystack/_pystack.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from _pystack.process cimport ProcessManager as NativeProcessManager
 from _pystack.process cimport remote_addr_t
 from _pystack.pycode cimport CodeObject
 from _pystack.pyframe cimport FrameObject
 from _pystack.pythread cimport NativeThread
 from _pystack.pythread cimport Thread
 from _pystack.pythread cimport getThreadFromInterpreterState
+from cpython.unicode cimport PyUnicode_Decode
 from libcpp.memory cimport make_shared
 from libcpp.memory cimport make_unique
 from libcpp.memory cimport shared_ptr
 from libcpp.memory cimport unique_ptr
 from libcpp.string cimport string as cppstring
 from libcpp.unordered_map cimport unordered_map
 from libcpp.vector cimport vector
@@ -66,33 +67,30 @@
 
 LOGGER = logging.getLogger(__file__)
 
 initializePythonLoggerInterface()
 
 
 class StackMethod(enum.Enum):
-    AUTO = 0
-    ELF_DATA = 1
-    SYMBOLS = 2
-    BSS = 3
-    ANONYMOUS_MAPS = 4
-    HEAP = 5
-    ALL = 1000
+    ELF_DATA = 1 << 0
+    SYMBOLS = 1 << 1
+    BSS = 1 << 2
+    ANONYMOUS_MAPS = 1 << 3
+    HEAP = 1 << 4
+    AUTO = ELF_DATA | SYMBOLS | BSS
+    ALL = AUTO | ANONYMOUS_MAPS | HEAP
 
 
 class NativeReportingMode(enum.Enum):
     OFF = 0
     PYTHON = 1
     ALL = 1000
 
 
 cdef api void log_with_python(const char* message, int level):
-    # Early return to avoid paying from the string conversion
-    if level < LOGGER.level:
-        return
     with contextlib.suppress(UnicodeDecodeError):
         LOGGER.log(level, message)
 
 T = TypeVar("T", bound=Callable[..., Any])
 
 
 class intercept_runtime_errors:
@@ -107,26 +105,21 @@
             except RuntimeError as e:
                 raise self.exception(*e.args) from e
 
         return wrapper
 
 
 @intercept_runtime_errors(EngineError)
-def copy_memory_from_address(pid, address, size, blocking=False):
+def copy_memory_from_address(pid, address, size):
     cdef shared_ptr[AbstractRemoteMemoryManager] manager
     cdef int the_pid = pid
     cdef vector[int] tids
-    if blocking:
-        manager = <shared_ptr[AbstractRemoteMemoryManager]> (
-            make_shared[BlockingProcessMemoryManager](the_pid, tids)
-        )
-    else:
-        manager = <shared_ptr[AbstractRemoteMemoryManager]> (
-            make_shared[ProcessMemoryManager](the_pid)
-        )
+    manager = <shared_ptr[AbstractRemoteMemoryManager]> (
+        make_shared[ProcessMemoryManager](the_pid)
+    )
 
     cdef AbstractRemoteMemoryManager *manager_handle = manager.get()
 
     memory = bytearray(size)
     cdef char *buffer = memory
     cdef remote_addr_t _address = address
     manager_handle.copyMemoryFromProcess(_address, size, <void *> buffer)
@@ -149,22 +142,22 @@
     )
 
 
 cdef CppMemoryMapInformation _pymapinfo_to_mapinfo(map_info: MemoryMapInformation):
     interpreter_map = (
         map_info.libpython if map_info.libpython is not None else map_info.python
     )
-    cdef CppMemoryMapInformation cppmap_info 
+    cdef CppMemoryMapInformation cppmap_info
     assert(interpreter_map is not None)
     cppmap_info.setMainMap(_pymap_to_map(interpreter_map))
     if map_info.bss:
         cppmap_info.setBss(_pymap_to_map(map_info.bss))
     if map_info.heap:
         cppmap_info.setHeap(_pymap_to_map(map_info.heap))
-    
+
     return cppmap_info
 
 
 cdef vector[CppVirtualMap] _pymaps_to_maps(pymaps: Iterable[VirtualMap]) except *:
     cdef vector[CppVirtualMap] native_maps
     for pymap in pymaps:
         native_maps.push_back(_pymap_to_map(pymap))
@@ -200,15 +193,15 @@
     else:
         analyzer = make_shared[NativeCoreFileAnalyzer](the_core_file)
     return analyzer
 
 
 cdef class CoreFileAnalyzer:
     cdef shared_ptr[CoreFileExtractor] _core_analyzer
-    cdef object ignored_libs 
+    cdef object ignored_libs
 
     def __cinit__(self, core_file, executable=None, lib_search_path=None):
         self.ignored_libs = frozenset(("ld-linux", "linux-vdso"))
         self._initialize_core_analyzer(core_file, executable, lib_search_path)
 
     @intercept_runtime_errors(EngineError)
     def _initialize_core_analyzer(self, core_file, executable, lib_search_path) -> None:
@@ -234,15 +227,15 @@
     @intercept_runtime_errors(EngineError)
     def extract_failure_info(self) -> Dict[str, Any]:
         return self._core_analyzer.get().extractFailureInfo()
 
     @intercept_runtime_errors(EngineError)
     def extract_ps_info(self) -> Dict[str, Any]:
         return self._core_analyzer.get().extractPSInfo()
-    
+
     cdef _is_ignored_lib(self, object path):
         return any(prefix in str(path) for prefix in self.ignored_libs)
 
     @intercept_runtime_errors(EngineError)
     def missing_modules(self) -> List[str]:
         cdef set result = set()
         cdef set missing_mod_names = set()
@@ -343,19 +336,14 @@
 
         virtual_maps = list(
             generate_maps_from_core_data(mapped_files, memory_maps)
         )
         pid = core_extractor.get().Pid()
         map_info = parse_maps_file_for_binary(executable, virtual_maps, load_point_by_module)
 
-        if map_info.python is None:
-            raise InvalidPythonProcess(
-                f"The core file {core_file} does not look generated by a Python process"
-            )
-
         the_core_file = str(core_file)
         the_executable = str(executable)
         maps = _pymaps_to_maps(virtual_maps)
         native_map_info =  _pymapinfo_to_mapinfo(map_info)
         cdef shared_ptr[AbstractProcessManager] native_manager = <shared_ptr[AbstractProcessManager]> (
             make_shared[CoreFileProcessManager](pid, analyzer, maps, native_map_info)
         )
@@ -389,18 +377,15 @@
 
 
 ######################################
 # COMMON STACK-RETRIEVING FUNCTIONS  #
 ######################################
 
 cdef object _try_to_decode_string(const cppstring *the_string):
-    try:
-        return dereference(the_string)
-    except UnicodeDecodeError:
-        return "???"
+    return PyUnicode_Decode(the_string.c_str(), the_string.size(), NULL, "replace")
 
 cdef object _safe_cppmap_to_py(unordered_map[cppstring, cppstring] themap):
     cdef unordered_map[cppstring, cppstring] . iterator it = themap.begin()
     cdef dict result = {}
     while it != themap.end():
         key = _try_to_decode_string(&(dereference(it).first))
         val = _try_to_decode_string(&(dereference(it).second))
@@ -458,19 +443,14 @@
     bint add_native_traces,
     bint resolve_locals,
 ):
     LOGGER.info("Fetching Python threads")
     threads = []
 
     cdef shared_ptr[Thread] thread = getThreadFromInterpreterState(manager, head)
-
-    if not thread:
-        LOGGER.info("No active Python thread was found")
-        return None
-
     cdef Thread *current_thread = thread.get()
     while current_thread != NULL:
         LOGGER.info("Constructing new Python thread with tid %s", current_thread.Tid())
         if add_native_traces:
             current_thread.populateNativeStackTrace(manager)
         frame = _construct_frame_stack_from_thread_object(
             pid, resolve_locals, current_thread.FirstFrame().get()
@@ -528,87 +508,54 @@
 
     return threads
 
 cdef remote_addr_t _get_interpreter_state_addr(
     AbstractProcessManager *manager, object method, int core=False
 ) except*:
     cdef remote_addr_t head = 0
+    possible_methods = [
+        StackMethod.ELF_DATA,
+        StackMethod.SYMBOLS,
+        StackMethod.BSS,
+        StackMethod.ANONYMOUS_MAPS,
+        StackMethod.HEAP,
+    ]
 
-    if method in {StackMethod.AUTO, StackMethod.ALL, StackMethod.ELF_DATA}:
-        try:
-            head = manager.findInterpreterStateFromElfData()
-        except Exception as exc:
-            LOGGER.warning(
-                "Unexpected error using ELF data to find PyInterpreterState: %s",
-                exc,
-            )
-        if head:
-            LOGGER.info(
-                "Address of PyInterpreterState found using ELF data at 0x%0.2X", head
-            )
-            return head
-
-    if method in {StackMethod.AUTO, StackMethod.ALL, StackMethod.SYMBOLS}:
-        try:
-            head = manager.findInterpreterStateFromSymbols()
-        except Exception as exc:
-            LOGGER.warning(
-                "Unexpected error using symbols to find PyInterpreterState: %s",
-                exc,
-            )
-        if head:
-            LOGGER.info(
-                "Address of PyInterpreterState found using symbols at 0x%0.2X", head
-            )
-            return head
-
-    if method in {StackMethod.AUTO, StackMethod.ALL, StackMethod.BSS}:
-        try:
-            head = manager.scanBSS()
-        except Exception as exc:
-            LOGGER.warning(
-                "Unexpected error scanning BSS to find PyInterpreterState: %s",
-                exc,
-            )
-        if head:
-            LOGGER.info(
-                "Address of PyInterpreterState found scanning the .bss section at 0x%0.2X",
-                head,
-            )
-            return head
+    for possible_method in possible_methods:
+        if method.value & possible_method.value == 0:
+            continue
 
-    if core and method in {StackMethod.ALL, StackMethod.ANONYMOUS_MAPS}:
         try:
-            head = manager.scanAllAnonymousMaps()
+            if possible_method == StackMethod.ELF_DATA:
+                how = "using ELF data"
+                head = manager.findInterpreterStateFromElfData()
+            elif possible_method == StackMethod.SYMBOLS:
+                how = "using symbols"
+                head = manager.findInterpreterStateFromSymbols()
+            elif possible_method == StackMethod.BSS:
+                how = "scanning the BSS"
+                head = manager.scanBSS()
+            elif possible_method == StackMethod.ANONYMOUS_MAPS:
+                how = "scanning all anonymous maps"
+                head = manager.scanAllAnonymousMaps()
+            elif possible_method == StackMethod.HEAP:
+                how = "scanning the heap"
+                head = manager.scanHeap()
         except Exception as exc:
             LOGGER.warning(
-                "Unexpected error scanning anonymous maps to find PyInterpreterState: %s",
-                exc,
+                "Unexpected error finding PyInterpreterState by %s: %s", how, exc
             )
-        if head:
-            LOGGER.info(
-                "Address of PyInterpreterState found scanning anonymous maps at 0x%0.2X",
-                head,
-            )
-            return head
 
-    if not core and method in {StackMethod.ALL, StackMethod.HEAP}:
-        try:
-            head = manager.scanHeap()
-        except Exception as exc:
-            LOGGER.warning(
-                "Unexpected error scanning heap to find PyInterpreterState: %s",
-                exc,
-            )
         if head:
-            LOGGER.info(
-                "Address of PyInterpreterState found scanning the heap at 0x%0.2X", head
-            )
+            LOGGER.info("PyInterpreterState found by %s at address 0x%0.2X", how, head)
             return head
+        else:
+            LOGGER.info("Address of PyInterpreterState not found by %s", how)
 
+    LOGGER.info("Address of PyInterpreterState could not be found")
     return 0
 
 
 def _check_interpreter_shutdown(manager):
     status = manager.interpreter_status()
     if status == InterpreterStatus.UNKNOWN:
         return
@@ -704,16 +651,14 @@
         "Analyzing process with pid %s using stack method %s with native mode %s",
         pid,
         method,
         native_mode,
     )
     virtual_maps = list(generate_maps_for_process(pid))
     map_info = parse_maps_file(pid, virtual_maps)
-    if map_info.python is None:
-        raise InvalidPythonProcess(f"Process {pid} does not look like a Python process")
 
     try:
         with ProcessManager.create_from_pid(pid, stop_process) as manager:
             yield from _get_process_threads(manager, pid, native_mode, locals, method)
     except RuntimeError as e:
         raise EngineError(*e.args, pid=pid) from e
```

### Comparing `pystack-1.0.1/src/pystack/colors.py` & `pystack-1.1.0/src/pystack/colors.py`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/errors.py` & `pystack-1.1.0/src/pystack/errors.py`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/maps.py` & `pystack-1.1.0/src/pystack/maps.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,21 +65,22 @@
     def is_private(self) -> bool:
         return "p" in self.flags
 
     @property
     def size(self) -> int:
         return self.end - self.start
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         start = f"0x{self.start:016x}"
         end = f"0x{self.end:016x}"
         filesize = f"0x{self.filesize:x}"
         offset = f"0x{self.offset:x}"
         return (
-            f"VirtualMap({start=!s}, {end=!s}, {filesize=!s}, {offset=!s},"
+            f"VirtualMap(start={start!s}, end={end!s},"
+            f" filesize={filesize!s}, offset={offset!s},"
             f" device={self.device!r}, flags={self.flags!r}, inode={self.inode!r},"
             f" path={str(self.path)!r})"
         )
 
 
 @dataclasses.dataclass
 class MemoryRange:
@@ -133,15 +134,15 @@
     missing_mapped_files = [
         map
         for map in mapped_files
         if (map["start"], map["end"]) not in memory_map_ranges
     ]
 
     all_maps: RawCoreMapList = sorted(
-        memory_maps + missing_mapped_files, key=lambda map: map["start"]  # type: ignore
+        memory_maps + missing_mapped_files, key=lambda map: map["start"]
     )
 
     # Some paths in the mapped files can be absolute, but we need to work with the canonical
     # paths that the linker reported, so we need to "unresolve" those path back to whatever
     # the memory math paths are so we can properly group then together. For example, the map
     # for the interpreter may be "/usr/bin/python" in the mapped files and "/venv/bin/python"
     # in the memory maps.
@@ -192,15 +193,15 @@
 
 def _get_bss(elf_maps: List[VirtualMap], load_point: int) -> Optional[VirtualMap]:
     binary_map = _get_base_map(elf_maps)
     if not binary_map or not binary_map.path:
         return None
     try:
         from ._pystack import get_bss_info
-    except ImportError:
+    except ImportError:  # pragma: no cover
         return None
     bss_info = get_bss_info(binary_map.path)
     if not bss_info:
         return None
     start = load_point + bss_info["corrected_addr"]
     LOGGER.info(
         "Determined exact addr of .bss section: %s (%s + %s)",
```

### Comparing `pystack-1.0.1/src/pystack/process.py` & `pystack-1.1.0/src/pystack/process.py`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack/traceback_formatter.py` & `pystack-1.1.0/src/pystack/traceback_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
         yield from _format_merged_stacks(thread, current_frame)
     yield ""
 
 
 def _format_merged_stacks(
     thread: PyThread, current_frame: Optional[PyFrame]
 ) -> Iterable[str]:
-
     for frame in thread.native_frames:
         if frame_type(frame, thread.python_version) == NativeFrame.FrameType.EVAL:
             assert current_frame is not None
             yield from format_frame(current_frame)
             current_frame = current_frame.next
             while current_frame and not current_frame.is_entry:
                 yield from format_frame(current_frame)
```

### Comparing `pystack-1.0.1/src/pystack/types.py` & `pystack-1.1.0/src/pystack/types.py`

 * *Files identical despite different names*

### Comparing `pystack-1.0.1/src/pystack.egg-info/PKG-INFO` & `pystack-1.1.0/src/pystack.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystack
-Version: 1.0.1
+Version: 1.1.0
 Summary: Analysis of the stack of remote python processes
 Home-page: https://github.com/bloomberg/pystack
 Author: Pablo Galindo Salgado
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
@@ -12,86 +12,86 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Debuggers
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-Provides-Extra: lint
-Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/11718525/226942590-de015c9a-4d5b-4960-9c42-8c1eac0845c1.png" width="70%">
 </p>
 
----
+______________________________________________________________________
 
 ![OS Linux](https://img.shields.io/badge/OS-Linux-blue)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pystack)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/pystack)
 ![PyPI](https://img.shields.io/pypi/v/pystack)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pystack)
 [![Tests](https://github.com/bloomberg/pystack/actions/workflows/build_wheels.yml/badge.svg)](https://github.com/bloomberg/pystack/actions/workflows/build_wheels.yml)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # PyStack
 
 > Print the stack trace of a running Python process, or of a Python core dump.
 
 PyStack is a tool that uses forbidden magic to let you inspect the stack frames of a running Python
-process or a Python core dump, helping you quickly and easily learn what it's doing (or what it was doing
-when it crashed) without having to interpret nasty CPython internals.
+process or a Python core dump, helping you quickly and easily learn what it's doing (or what it was
+doing when it crashed) without having to interpret nasty CPython internals.
 
 # What PyStack can do
 
 PyStack has the following amazing features:
 
 - 💻 Works with both running processes and core dump files.
-- 🧵 Shows if each thread currently holds the Python GIL, is waiting to acquire it, or is
-  currently dropping it.
+- 🧵 Shows if each thread currently holds the Python GIL, is waiting to acquire it, or is currently
+  dropping it.
 - 🗑️ Shows if a thread is running a garbage collection cycle.
 - 🐍 Optionally shows native function calls, as well as Python ones. In this mode, PyStack prints
   the native stack trace (C/C++/Rust function calls), except that the calls to Python callables are
   replaced with frames showing the Python code being executed, instead of showing the internal C
   code the interpreter used to make the call.
 - 🔍 Automatically demangles symbols shown in the native stack.
 - 📈 Includes calls to inlined functions in the native stack whenever enough debug information is
   available.
 - 🔍 Optionally shows the values of local variables and function arguments in Python stack frames.
-- 🔒 Safe to use on running processes. PyStack does not modify any memory or execute any code in
-  a process that is running. It simply attaches just long enough to read some of the process's memory.
+- 🔒 Safe to use on running processes. PyStack does not modify any memory or execute any code in a
+  process that is running. It simply attaches just long enough to read some of the process's
+  memory.
 - ⚡ Optionally, it can perform a Python stack analysis without pausing the process at all. This
   minimizes impact to the debugged process, at the cost of potentially failing due to data races.
 - 🚀 Super fast! It can analyze core files 10x faster than general-purpose tools like GDB.
 - 🎯 Even works with aggressively optimized Python interpreter binaries.
 - 🔍 Even works with Python interpreters' binaries that do not have symbols or debug information
   (Python stack only).
-- 💥 Tolerates memory corruption well. Even if the process crashed due to memory corruption, PyStack
-  can usually reconstruct the stack.
+- 💥 Tolerates memory corruption well. Even if the process crashed due to memory corruption,
+  PyStack can usually reconstruct the stack.
 - 💼 Self-contained: it does not depend on external tools or programs other than the Python
   interpreter used to run PyStack itself.
 
 ## Building from source
 
-If you wish to build PyStack from source, you need the following binary dependencies in your system:
+If you wish to build PyStack from source, you need the following binary dependencies in your
+system:
 
 - libdw
 - libelf
 
 Note that sometimes both libraries are provided together as part of a distribution's `elfutils`
 package.
 
 Check your package manager on how to install these dependencies (e.g.,
 `apt-get install libdw-dev libelf-dev` in Debian-based systems). Note that you may need to tell the
-compiler where to find the header and library files of the dependencies for the build to
-succeed. Check your distribution's documentation to determine the location of the header and
-library files or for more detailed information.
+compiler where to find the header and library files of the dependencies for the build to succeed.
+Check your distribution's documentation to determine the location of the header and library files
+or for more detailed information. When building on Alpine Linux (or any other distribution that
+doesn't use glibc) you'll need elfutils 0.188 or newer. You may need to build this from source if
+your distribution's package manager doesn't have it.
 
 Once you have these binary dependencies installed, you can clone the repository and follow the
 typical build process for Python libraries:
 
 ```shell
 git clone git@github.com:bloomberg/pystack.git pystack
 cd pystack
@@ -102,14 +102,22 @@
 python3 -m pip install -r requirements-test.txt -r requirements-extra.txt
 ```
 
 This will install PyStack in the virtual environment in development mode (the `-e` of the last
 `pip install` command), and then install the Python libraries needed to test it, lint it, and
 generate its documentation.
 
+If you plan to contribute back, you should install the pre-commit hooks:
+
+```shell
+pre-commit install
+```
+
+This will ensure that your contribution passes our linting checks.
+
 # Documentation
 
 You can find the full documentation [here](https://bloomberg.github.io/pystack/).
 
 # Usage
 
 PyStack uses distinct subcommands for analyzing running processes and core dump files.
@@ -129,19 +137,19 @@
     remote       Analyze a remote process given its PID
     core         Analyze a core dump file given its location and the executable
 ```
 
 ## Analyzing running processes
 
 The `remote` command is used to analyze the status of a running (remote) process. The analysis is
-always done in a safe and non-intrusive way, as no code is loaded in the memory space of the process
-under analysis and no memory is modified in the remote process. This makes analysis using PyStack a
-great option even for those services and applications that are running in environments where the running process
-must not be impacted in any way (other than being temporarily paused, though `--no-block` can avoid
-even that). There are several options available:
+always done in a safe and non-intrusive way, as no code is loaded in the memory space of the
+process under analysis and no memory is modified in the remote process. This makes analysis using
+PyStack a great option even for those services and applications that are running in environments
+where the running process must not be impacted in any way (other than being temporarily paused,
+though `--no-block` can avoid even that). There are several options available:
 
 ```shell
 usage: pystack remote [-h] [-v] [--no-color] [--no-block] [--native] [--native-all] [--locals] [--exhaustive] [--self] pid
 
 positional arguments:
   pid            The PID of the remote process
 
@@ -172,17 +180,17 @@
 ```
 
 ## Analyzing core dumps
 
 The `core` subcommand is used to analyze the status of a core dump file. Analyzing core files is
 very similar to analyzing processes but there are some differences, as the core file does not
 contain the totality of the memory that was valid when the program was live. In most cases, this
-makes no difference, as PyStack will try to adapt automatically. However, in some cases, you will need to
-specify extra command line options to help PyStack locate the information it needs. When analyzing
-cores, there are several options available:
+makes no difference, as PyStack will try to adapt automatically. However, in some cases, you will
+need to specify extra command line options to help PyStack locate the information it needs. When
+analyzing cores, there are several options available:
 
 ```shell
 usage: pystack core [-h] [-v] [--no-color] [--native] [--native-all] [--locals] [--exhaustive] [--lib-search-path LIB_SEARCH_PATH | --lib-search-root LIB_SEARCH_ROOT] core [executable]
 
 positional arguments:
   core                  The path to the core file
   executable            (Optional) The path to the executable of the core file
@@ -197,15 +205,16 @@
   --exhaustive          Use all possible methods to obtain the Python stack info (may be slow)
   --lib-search-path LIB_SEARCH_PATH
                         List of paths to search for shared libraries loaded in the core. Paths must be separated by the ':' character
   --lib-search-root LIB_SEARCH_ROOT
                         Root directory to search recursively for shared libraries loaded into the core.
 ```
 
-In most cases, you just need to provide the location of the core to use PyStack with core dump files:
+In most cases, you just need to provide the location of the core to use PyStack with core dump
+files:
 
 ```shell
 $ pystack core ./the_core_file
 Using executable found in the core file: /usr/bin/python3.8
 
 Core file information:
 state: t zombie: True niceness: 0
@@ -255,25 +264,26 @@
 any questions about this process or any other aspect of contributing to a Bloomberg open source
 project, feel free to send an email to opensource@bloomberg.net and we'll get your questions
 answered as quickly as we can.
 
 ## Contribution Licensing
 
 Since this project is distributed under the terms of an [open source license](LICENSE),
-contributions that you make are licensed under the same terms. For us to be able to accept
-your contributions, we will need explicit confirmation from you that you are able and willing to
-provide them under these terms, and the mechanism we use to do this is called a Developer's
-Certificate of Origin [(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is
-similar to the process used by the Linux(R) kernel, Samba, and many other major open source
-projects.
+contributions that you make are licensed under the same terms. For us to be able to accept your
+contributions, we will need explicit confirmation from you that you are able and willing to provide
+them under these terms, and the mechanism we use to do this is called a Developer's Certificate of
+Origin [(DCO)](https://github.com/bloomberg/.github/blob/main/DCO.md). This is similar to the
+process used by the Linux kernel, Samba, and many other major open source projects.
 
 To participate under these terms, all that you must do is include a line like the following as the
 last line of the commit message for each commit in your contribution:
 
-    Signed-Off-By: Random J. Developer <random@developer.example.org>
+```
+Signed-Off-By: Random J. Developer <random@developer.example.org>
+```
 
 The simplest way to accomplish this is to add `-s` or `--signoff` to your `git commit` command.
 
 You must use your real name (sorry, no pseudonyms, and no anonymous contributions).
 
 ## Steps
```

### Comparing `pystack-1.0.1/src/pystack.egg-info/SOURCES.txt` & `pystack-1.1.0/src/pystack.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+.bumpversion.cfg
+.pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 Makefile
+NEWS.rst
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 src/pystack/__init__.py
 src/pystack/__main__.py
 src/pystack/_pystack.pyi
 src/pystack/_pystack.pyx
 src/pystack/_version.py
 src/pystack/colors.py
@@ -18,15 +20,14 @@
 src/pystack/py.typed
 src/pystack/traceback_formatter.py
 src/pystack/types.py
 src/pystack.egg-info/PKG-INFO
 src/pystack.egg-info/SOURCES.txt
 src/pystack.egg-info/dependency_links.txt
 src/pystack.egg-info/entry_points.txt
-src/pystack.egg-info/requires.txt
 src/pystack.egg-info/top_level.txt
 src/pystack/_pystack/CMakeLists.txt
 src/pystack/_pystack/__init__.pxd
 src/pystack/_pystack/compat.h
 src/pystack/_pystack/corefile.cpp
 src/pystack/_pystack/corefile.h
 src/pystack/_pystack/corefile.pxd
```

