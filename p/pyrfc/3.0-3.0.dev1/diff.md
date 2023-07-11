# Comparing `tmp/pyrfc-3.0.tar.gz` & `tmp/pyrfc-3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfc-3.0.tar", last modified: Tue Jul 11 12:51:09 2023, max compression
+gzip compressed data, was "pyrfc-3.0.dev1.tar", last modified: Mon May 15 10:06:29 2023, max compression
```

## Comparing `pyrfc-3.0.tar` & `pyrfc-3.0.dev1.tar`

### file list

```diff
@@ -1,35 +1,22 @@
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-07-11 12:51:09.948619 pyrfc-3.0/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-07-11 12:51:08.313176 pyrfc-3.0/.github/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-07-11 12:51:08.857888 pyrfc-3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      500 2022-11-14 10:18:39.000000 pyrfc-3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      595 2022-11-14 10:18:39.000000 pyrfc-3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      403 2023-07-07 15:17:11.000000 pyrfc-3.0/.gitignore
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-07-11 12:51:08.902293 pyrfc-3.0/.reuse/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     2233 2023-07-07 15:17:11.000000 pyrfc-3.0/.reuse/dep5
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     4622 2022-11-14 10:18:39.000000 pyrfc-3.0/CONTRIBUTING.md
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-07-07 15:17:11.000000 pyrfc-3.0/LICENSE
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-07-11 12:51:08.938957 pyrfc-3.0/LICENSES/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-03-29 13:04:51.000000 pyrfc-3.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       58 2023-07-07 15:17:11.000000 pyrfc-3.0/MANIFEST.in
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23946 2023-07-11 12:51:09.941481 pyrfc-3.0/PKG-INFO
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10683 2023-07-07 15:17:11.000000 pyrfc-3.0/README.md
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-07-11 12:51:08.373027 pyrfc-3.0/ci/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-07-11 12:51:09.018835 pyrfc-3.0/ci/utils/
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1393 2023-03-29 13:04:51.000000 pyrfc-3.0/ci/utils/paths_fix.sh
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)      228 2022-11-14 10:18:39.000000 pyrfc-3.0/ci/utils/paths_show.sh
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     2555 2023-07-11 12:33:17.000000 pyrfc-3.0/pyproject.toml
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       38 2023-07-11 12:51:09.952101 pyrfc-3.0/setup.cfg
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     5404 2023-07-07 15:17:11.000000 pyrfc-3.0/setup.py
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-07-11 12:51:08.428434 pyrfc-3.0/src/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-07-11 12:51:09.672530 pyrfc-3.0/src/pyrfc/
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1452 2023-07-11 12:33:17.000000 pyrfc-3.0/src/pyrfc/__init__.py
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)  2313314 2023-07-11 12:51:05.000000 pyrfc-3.0/src/pyrfc/_cyrfc.cpp
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)   129764 2023-07-10 17:44:54.000000 pyrfc-3.0/src/pyrfc/_cyrfc.pyx
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     5677 2023-07-07 15:17:11.000000 pyrfc-3.0/src/pyrfc/_exception.py
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      317 2023-07-07 15:17:11.000000 pyrfc-3.0/src/pyrfc/_utils.py
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)    23820 2023-07-07 15:17:11.000000 pyrfc-3.0/src/pyrfc/csapnwrfc.pxd
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-07-11 12:51:09.884807 pyrfc-3.0/src/pyrfc.egg-info/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23946 2023-07-11 12:51:08.000000 pyrfc-3.0/src/pyrfc.egg-info/PKG-INFO
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      504 2023-07-11 12:51:08.000000 pyrfc-3.0/src/pyrfc.egg-info/SOURCES.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-07-11 12:51:08.000000 pyrfc-3.0/src/pyrfc.egg-info/dependency_links.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        6 2023-07-11 12:51:08.000000 pyrfc-3.0/src/pyrfc.egg-info/top_level.txt
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-15 10:06:29.802777 pyrfc-3.0.dev1/
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-15 10:06:29.605086 pyrfc-3.0.dev1/LICENSES/
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-05-15 09:42:00.000000 pyrfc-3.0.dev1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)       58 2023-05-15 09:42:00.000000 pyrfc-3.0.dev1/MANIFEST.in
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23951 2023-05-15 10:06:29.799392 pyrfc-3.0.dev1/PKG-INFO
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10683 2023-05-15 09:42:00.000000 pyrfc-3.0.dev1/README.md
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)     1749 2023-05-15 09:42:00.000000 pyrfc-3.0.dev1/pyproject.toml
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)       38 2023-05-15 10:06:29.804140 pyrfc-3.0.dev1/setup.cfg
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)     5404 2023-05-15 09:42:00.000000 pyrfc-3.0.dev1/setup.py
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-15 10:06:29.577157 pyrfc-3.0.dev1/src/
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-15 10:06:29.737112 pyrfc-3.0.dev1/src/pyrfc/
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1522 2023-05-15 09:42:00.000000 pyrfc-3.0.dev1/src/pyrfc/__init__.py
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)  2312352 2023-05-15 10:06:25.000000 pyrfc-3.0.dev1/src/pyrfc/_cyrfc.cpp
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)   129764 2023-05-15 09:42:00.000000 pyrfc-3.0.dev1/src/pyrfc/_cyrfc.pyx
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     5677 2023-05-15 09:42:00.000000 pyrfc-3.0.dev1/src/pyrfc/_exception.py
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)      317 2023-05-15 09:42:00.000000 pyrfc-3.0.dev1/src/pyrfc/_utils.py
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)    23820 2023-05-15 09:42:00.000000 pyrfc-3.0.dev1/src/pyrfc/csapnwrfc.pxd
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-15 10:06:29.791464 pyrfc-3.0.dev1/src/pyrfc.egg-info/
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23951 2023-05-15 10:06:29.000000 pyrfc-3.0.dev1/src/pyrfc.egg-info/PKG-INFO
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)      333 2023-05-15 10:06:29.000000 pyrfc-3.0.dev1/src/pyrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-05-15 10:06:29.000000 pyrfc-3.0.dev1/src/pyrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)        6 2023-05-15 10:06:29.000000 pyrfc-3.0.dev1/src/pyrfc.egg-info/top_level.txt
```

### Comparing `pyrfc-3.0/LICENSE` & `pyrfc-3.0.dev1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0/PKG-INFO` & `pyrfc-3.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfc
-Version: 3.0
+Version: 3.0.dev1
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Author-email: srdjan.boskovic@sap.com
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
```

### Comparing `pyrfc-3.0/README.md` & `pyrfc-3.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0/pyproject.toml` & `pyrfc-3.0.dev1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["Cython >= 0.29, < 1", "setuptools >= 67", "wheel >= 0.40"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrfc"
-version = "3.0"
+version = "3.0.dev1"
 readme = "README.md"
 license = { file = "LICENSES/Apache-2.0.txt" }
 description = "Python bindings for SAP NetWeaver RFC SDK"
 authors = [ { name = "SAP SE"}, { email = "srdjan.boskovic@sap.com" } ]
 maintainers = [ { name = "Srdjan Boskovic", email = "srdjan.boskovic@sap.com" } ]
 requires-python = ">=3.8"
 keywords = ["pyrfc", "sap", "nwrfc", "sapnwrfc", "abap"]
@@ -32,58 +32,25 @@
 
 [project.urls]
 bug-tracker = "https://github.com/wntrblm/nox/issues"
 documentation = "http://sap.github.io/PyRFC"
 homepage = "https://github.com/SAP/PyRFC"
 repository = "https://github.com/SAP/PyRFC.git"
 
+[tool.black]
+line-length = 120
+
 [tool.cython-lint]
-max-line-length = 172
+max-line-length = 180
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 include-package-data = false
 license-files=["LICENSES/*.txt"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["pyrfc"]
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 testpaths =["tests"]
-
-[tool.ruff]
-select = [
-  "C90",    # McCabe cyclomatic complexity
-  "E",      # pycodestyle
-  "F",      # Pyflakes
-  "ICN",    # flake8-import-conventions
-  "INT",    # flake8-gettext
-  "PLC",    # Pylint conventions
-  "PLE",    # Pylint errors
-  "PLR09",  # Pylint refactoring: max-args, max-branches, max returns, max-statements
-  "PYI",    # flake8-pyi
-  "RSE",    # flake8-raise
-  "RUF",    # Ruff-specific rules
-  "T10",    # flake8-debugger
-  "TCH",    # flake8-type-checking
-  "TID",    # flake8-tidy-imports
-  "W",      # pycodestyle
-  "YTT",    # flake8-2020
-]
-
-line-length = 172
-target-version = "py38"
-
-[tool.ruff.mccabe]
-max-complexity = 100
-
-[tool.ruff.per-file-ignores]
-"src/pyrfc/__init__.py" = ["F401"]
-"tests/test_server.py" = ["E402"]
-
-[tool.ruff.pylint]
-max-args = 11
-max-branches = 110
-max-returns = 8
-max-statements = 289
```

### Comparing `pyrfc-3.0/setup.py` & `pyrfc-3.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0/src/pyrfc/__init__.py` & `pyrfc-3.0.dev1/src/pyrfc/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 __version_info__ = tuple(__version__.split("."))
 
 if os.name == "nt":
     # add SAP NWRFC SDK to DLL pth
     with suppress(Exception):
         os.add_dll_directory(os.path.join(os.environ["SAPNWRFC_HOME"], "lib"))
 
+from pyrfc._exception import CommunicationError  # noqa F401
 from pyrfc._exception import (
     ABAPApplicationError,
     ABAPRuntimeError,
-    CommunicationError,
     ExternalApplicationError,
     ExternalAuthorizationError,
     ExternalRuntimeError,
     LogonError,
     RFCError,
     RFCLibError,
 )
 
 try:
+    from pyrfc._cyrfc import RCStatus  # noqa F401
     from pyrfc._cyrfc import (
-        RCStatus,
         Connection,
         ConnectionParameters,
         Decimal,
         FunctionDescription,
         RfcFieldType,
         RfcParameterDirection,
         Server,
```

### Comparing `pyrfc-3.0/src/pyrfc/_cyrfc.cpp` & `pyrfc-3.0.dev1/src/pyrfc/_cyrfc.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.36 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NDEBUG",
@@ -76,16 +76,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_36"
-#define CYTHON_HEX_VERSION 0x001D24F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -145,22 +145,18 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
+  #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -450,14 +446,17 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define Py_OptimizeFlag 0
+#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -527,19 +526,14 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
-#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
-  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
-#else
-  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
-#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -41125,15 +41119,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_5pyrfc_6_cyrfc_ConnectionParameters(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_5pyrfc_6_cyrfc_ConnectionParameters[] = {
@@ -41207,15 +41201,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5pyrfc_6_cyrfc_Connection __pyx_vtable_5pyrfc_6_cyrfc_Connection;
 
 static PyObject *__pyx_tp_new_5pyrfc_6_cyrfc_Connection(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_5pyrfc_6_cyrfc_Connection *p;
@@ -41232,15 +41226,15 @@
   p->_connection = ((struct __pyx_obj_5pyrfc_6_cyrfc_ConnectionParameters *)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_5pyrfc_6_cyrfc_Connection(PyObject *o) {
   struct __pyx_obj_5pyrfc_6_cyrfc_Connection *p = (struct __pyx_obj_5pyrfc_6_cyrfc_Connection *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__config);
   Py_CLEAR(p->_connection);
   (*Py_TYPE(o)->tp_free)(o);
@@ -41471,15 +41465,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5pyrfc_6_cyrfc_ServerConnection __pyx_vtable_5pyrfc_6_cyrfc_ServerConnection;
 
 static PyObject *__pyx_tp_new_5pyrfc_6_cyrfc_ServerConnection(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_5pyrfc_6_cyrfc_ServerConnection *p;
@@ -41495,15 +41489,15 @@
   p->_connection = ((struct __pyx_obj_5pyrfc_6_cyrfc_ConnectionParameters *)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_5pyrfc_6_cyrfc_ServerConnection(PyObject *o) {
   struct __pyx_obj_5pyrfc_6_cyrfc_ServerConnection *p = (struct __pyx_obj_5pyrfc_6_cyrfc_ServerConnection *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_connection);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -41704,15 +41698,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5pyrfc_6_cyrfc_Server __pyx_vtable_5pyrfc_6_cyrfc_Server;
 
 static PyObject *__pyx_tp_new_5pyrfc_6_cyrfc_Server(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_5pyrfc_6_cyrfc_Server *p;
@@ -41734,15 +41728,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_5pyrfc_6_cyrfc_Server(PyObject *o) {
   struct __pyx_obj_5pyrfc_6_cyrfc_Server *p = (struct __pyx_obj_5pyrfc_6_cyrfc_Server *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_client_connection);
   Py_CLEAR(p->_server_connection);
   Py_CLEAR(p->_server_thread);
@@ -41890,15 +41884,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5pyrfc_6_cyrfc_Throughput __pyx_vtable_5pyrfc_6_cyrfc_Throughput;
 
 static PyObject *__pyx_tp_new_5pyrfc_6_cyrfc_Throughput(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_5pyrfc_6_cyrfc_Throughput *p;
@@ -41914,15 +41908,15 @@
   p->_connections = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_5pyrfc_6_cyrfc_Throughput(PyObject *o) {
   struct __pyx_obj_5pyrfc_6_cyrfc_Throughput *p = (struct __pyx_obj_5pyrfc_6_cyrfc_Throughput *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_connections);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -42040,15 +42034,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_object____object___to_py *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_object____object___to_py[8];
 static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_object____object___to_py = 0;
 
@@ -42136,15 +42130,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -49030,18 +49024,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -50021,15 +50012,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -50217,15 +50208,15 @@
                         } else if (8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT) {
                             return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -50413,15 +50404,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -50647,15 +50638,15 @@
                         } else if (8 * sizeof(short) >= 4 * PyLong_SHIFT) {
                             return (short) (((((((((short)digits[3]) << PyLong_SHIFT) | (short)digits[2]) << PyLong_SHIFT) | (short)digits[1]) << PyLong_SHIFT) | (short)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -50881,15 +50872,15 @@
                         } else if (8 * sizeof(RFC_RC) >= 4 * PyLong_SHIFT) {
                             return (RFC_RC) (((((((((RFC_RC)digits[3]) << PyLong_SHIFT) | (RFC_RC)digits[2]) << PyLong_SHIFT) | (RFC_RC)digits[1]) << PyLong_SHIFT) | (RFC_RC)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -51077,15 +51068,15 @@
                         } else if (8 * sizeof(RFCTYPE) >= 4 * PyLong_SHIFT) {
                             return (RFCTYPE) (((((((((RFCTYPE)digits[3]) << PyLong_SHIFT) | (RFCTYPE)digits[2]) << PyLong_SHIFT) | (RFCTYPE)digits[1]) << PyLong_SHIFT) | (RFCTYPE)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -51273,15 +51264,15 @@
                         } else if (8 * sizeof(RFC_DIRECTION) >= 4 * PyLong_SHIFT) {
                             return (RFC_DIRECTION) (((((((((RFC_DIRECTION)digits[3]) << PyLong_SHIFT) | (RFC_DIRECTION)digits[2]) << PyLong_SHIFT) | (RFC_DIRECTION)digits[1]) << PyLong_SHIFT) | (RFC_DIRECTION)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -51507,15 +51498,15 @@
                         } else if (8 * sizeof(RFC_INT) >= 4 * PyLong_SHIFT) {
                             return (RFC_INT) (((((((((RFC_INT)digits[3]) << PyLong_SHIFT) | (RFC_INT)digits[2]) << PyLong_SHIFT) | (RFC_INT)digits[1]) << PyLong_SHIFT) | (RFC_INT)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -51703,15 +51694,15 @@
                         } else if (8 * sizeof(RFC_INT8) >= 4 * PyLong_SHIFT) {
                             return (RFC_INT8) (((((((((RFC_INT8)digits[3]) << PyLong_SHIFT) | (RFC_INT8)digits[2]) << PyLong_SHIFT) | (RFC_INT8)digits[1]) << PyLong_SHIFT) | (RFC_INT8)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -51937,15 +51928,15 @@
                         } else if (8 * sizeof(RFC_ERROR_GROUP) >= 4 * PyLong_SHIFT) {
                             return (RFC_ERROR_GROUP) (((((((((RFC_ERROR_GROUP)digits[3]) << PyLong_SHIFT) | (RFC_ERROR_GROUP)digits[2]) << PyLong_SHIFT) | (RFC_ERROR_GROUP)digits[1]) << PyLong_SHIFT) | (RFC_ERROR_GROUP)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -52285,15 +52276,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pyrfc-3.0/src/pyrfc/_cyrfc.pyx` & `pyrfc-3.0.dev1/src/pyrfc/_cyrfc.pyx`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0/src/pyrfc/_exception.py` & `pyrfc-3.0.dev1/src/pyrfc/_exception.py`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0/src/pyrfc/csapnwrfc.pxd` & `pyrfc-3.0.dev1/src/pyrfc/csapnwrfc.pxd`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0/src/pyrfc.egg-info/PKG-INFO` & `pyrfc-3.0.dev1/src/pyrfc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfc
-Version: 3.0
+Version: 3.0.dev1
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Author-email: srdjan.boskovic@sap.com
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
```

