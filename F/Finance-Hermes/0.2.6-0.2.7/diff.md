# Comparing `tmp/Finance-Hermes-0.2.6.tar.gz` & `tmp/Finance-Hermes-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Hermes-0.2.6.tar", last modified: Tue Jul 11 12:18:16 2023, max compression
+gzip compressed data, was "dist/Finance-Hermes-0.2.7.tar", last modified: Tue Jul 11 12:27:24 2023, max compression
```

## Comparing `Finance-Hermes-0.2.6.tar` & `Finance-Hermes-0.2.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/Finance_Hermes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-11 12:18:15.000000 Finance-Hermes-0.2.6/Finance_Hermes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      759 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/Finance_Hermes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:18:15.000000 Finance-Hermes-0.2.6/Finance_Hermes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-11 12:18:15.000000 Finance-Hermes-0.2.6/Finance_Hermes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 12:18:15.000000 Finance-Hermes-0.2.6/Finance_Hermes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-24 10:42:40.000000 Finance-Hermes-0.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/hermes/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-11 12:18:09.000000 Finance-Hermes-0.2.6/hermes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/hermes/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.6/hermes/factors/__init__.py
--rw-r--r--   0 root         (0) root         (0)   327314 2023-07-11 12:10:03.000000 Finance-Hermes-0.2.6/hermes/factors/base.c
--rw-r--r--   0 root         (0) root         (0)     4012 2023-07-11 12:07:24.000000 Finance-Hermes-0.2.6/hermes/factors/base.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/hermes/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.6/hermes/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)   271147 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.6/hermes/kdutils/base.c
--rw-r--r--   0 root         (0) root         (0)     2338 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.6/hermes/kdutils/base.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/hermes/kdutils/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.6/hermes/kdutils/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)   678491 2023-06-24 10:39:53.000000 Finance-Hermes-0.2.6/hermes/kdutils/core/fixes.c
--rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.6/hermes/kdutils/core/fixes.pyx
--rw-r--r--   0 root         (0) root         (0)   392670 2023-06-24 10:39:53.000000 Finance-Hermes-0.2.6/hermes/kdutils/core/helper.c
--rw-r--r--   0 root         (0) root         (0)     7825 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.6/hermes/kdutils/core/helper.pyx
--rw-r--r--   0 root         (0) root         (0)   190192 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.6/hermes/kdutils/create_id.c
--rw-r--r--   0 root         (0) root         (0)      870 2023-06-21 21:57:15.000000 Finance-Hermes-0.2.6/hermes/kdutils/create_id.pyx
--rw-r--r--   0 root         (0) root         (0)   235985 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.6/hermes/kdutils/lazy.c
--rw-r--r--   0 root         (0) root         (0)     1578 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.6/hermes/kdutils/lazy.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/hermes/lzador/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.6/hermes/lzador/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161732 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.6/hermes/lzador/calculater.c
--rw-r--r--   0 root         (0) root         (0)      657 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.6/hermes/lzador/calculater.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/requirements/
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-24 12:13:59.000000 Finance-Hermes-0.2.6/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 12:18:16.000000 Finance-Hermes-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3292 2023-07-11 12:09:04.000000 Finance-Hermes-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/Finance_Hermes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/Finance_Hermes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      759 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/Finance_Hermes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/Finance_Hermes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/Finance_Hermes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/Finance_Hermes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-24 10:42:40.000000 Finance-Hermes-0.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/hermes/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-11 12:27:04.000000 Finance-Hermes-0.2.7/hermes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/hermes/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.7/hermes/factors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   329316 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/hermes/factors/base.c
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-07-11 12:26:32.000000 Finance-Hermes-0.2.7/hermes/factors/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/hermes/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.7/hermes/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   271147 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.7/hermes/kdutils/base.c
+-rw-r--r--   0 root         (0) root         (0)     2338 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.7/hermes/kdutils/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/hermes/kdutils/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.7/hermes/kdutils/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   678491 2023-06-24 10:39:53.000000 Finance-Hermes-0.2.7/hermes/kdutils/core/fixes.c
+-rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.7/hermes/kdutils/core/fixes.pyx
+-rw-r--r--   0 root         (0) root         (0)   392670 2023-06-24 10:39:53.000000 Finance-Hermes-0.2.7/hermes/kdutils/core/helper.c
+-rw-r--r--   0 root         (0) root         (0)     7825 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.7/hermes/kdutils/core/helper.pyx
+-rw-r--r--   0 root         (0) root         (0)   190192 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.7/hermes/kdutils/create_id.c
+-rw-r--r--   0 root         (0) root         (0)      870 2023-06-21 21:57:15.000000 Finance-Hermes-0.2.7/hermes/kdutils/create_id.pyx
+-rw-r--r--   0 root         (0) root         (0)   235985 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.7/hermes/kdutils/lazy.c
+-rw-r--r--   0 root         (0) root         (0)     1578 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.7/hermes/kdutils/lazy.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/hermes/lzador/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.7/hermes/lzador/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161732 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.7/hermes/lzador/calculater.c
+-rw-r--r--   0 root         (0) root         (0)      657 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.7/hermes/lzador/calculater.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/requirements/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-24 12:13:59.000000 Finance-Hermes-0.2.7/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 12:27:24.000000 Finance-Hermes-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-07-11 12:09:04.000000 Finance-Hermes-0.2.7/setup.py
```

### Comparing `Finance-Hermes-0.2.6/Finance_Hermes.egg-info/SOURCES.txt` & `Finance-Hermes-0.2.7/Finance_Hermes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/LICENSE` & `Finance-Hermes-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/factors/base.c` & `Finance-Hermes-0.2.7/hermes/factors/base.c`

 * *Files 1% similar despite different names*

```diff
@@ -827,15 +827,15 @@
 static const char *__pyx_f[] = {
   "hermes/factors/base.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list;
 
-/* "hermes/factors/base.pyx":130
+/* "hermes/factors/base.pyx":132
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list {
@@ -978,14 +978,31 @@
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
 #endif
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
+/* PyDictContains.proto */
+static CYTHON_INLINE int __Pyx_PyDict_ContainsTF(PyObject* item, PyObject* dict, int eq) {
+    int result = PyDict_Contains(dict, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
+/* DictGetItem.proto */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
+#define __Pyx_PyObject_Dict_GetItem(obj, name)\
+    (likely(PyDict_CheckExact(obj)) ?\
+     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
+#else
+#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
+#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
+#endif
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1025,25 +1042,14 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
 /* GetAttr.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* PySequenceContains.proto */
@@ -1321,14 +1327,15 @@
 /* Implementation of 'hermes.factors.base' */
 static PyObject *__pyx_builtin_filter;
 static const char __pyx_k_[] = "_";
 static const char __pyx_k_0[] = "{0}";
 static const char __pyx_k_s[] = "s";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_abc[] = "abc";
+static const char __pyx_k_ddb[] = "ddb";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_md5[] = "md5";
 static const char __pyx_k_pdb[] = "pdb";
 static const char __pyx_k_six[] = "six";
 static const char __pyx_k_copy[] = "copy";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_func[] = "func";
@@ -1346,14 +1353,15 @@
 static const char __pyx_k_stack[] = "stack";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_filter[] = "filter";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_kwargs[] = "kwargs";
+static const char __pyx_k_method[] = "method";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_ABCMeta[] = "ABCMeta";
 static const char __pyx_k_buy_put[] = "\n        \346\267\267\345\205\245\347\261\273\357\274\214\346\267\267\345\205\245\344\273\243\350\241\250\347\251\272\345\244\264\357\274\214\345\272\224\347\224\250\345\234\272\346\231\257\345\234\250\344\272\216\346\234\237\346\235\203\357\274\214\346\234\237\350\264\247\347\255\226\347\225\245\344\270\255\357\274\214\n        \344\270\215\345\256\214\345\205\250\346\230\257\346\234\237\346\235\203\344\270\255buy put\347\232\204\346\246\202\345\277\265\357\274\214\345\217\252\344\273\243\347\234\213\350\267\214\345\217\215\345\220\221\346\223\215\344\275\234\357\274\214\n        \345\215\263\346\234\237\346\234\233\344\271\260\345\205\245\345\220\216\344\272\244\346\230\223\347\233\256\346\240\207\344\273\267\346\240\274\344\270\213\350\267\214\357\274\214\344\270\213\350\267\214\345\270\246\346\235\245\346\224\266\347\233\212\n    ";
 static const char __pyx_k_columns[] = "columns";
 static const char __pyx_k_default[] = "default";
 static const char __pyx_k_feature[] = "feature";
@@ -1451,14 +1459,15 @@
 static PyObject *__pyx_n_s_category;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_columns;
 static PyObject *__pyx_n_s_copy;
 static PyObject *__pyx_n_s_create_id;
 static PyObject *__pyx_n_s_create_id_2;
 static PyObject *__pyx_n_s_data;
+static PyObject *__pyx_n_s_ddb;
 static PyObject *__pyx_n_s_deepcopy;
 static PyObject *__pyx_n_s_default;
 static PyObject *__pyx_n_s_dependencies;
 static PyObject *__pyx_n_s_dependencies_list;
 static PyObject *__pyx_n_s_digit;
 static PyObject *__pyx_n_s_doc;
 static PyObject *__pyx_n_s_dumps;
@@ -1495,14 +1504,15 @@
 static PyObject *__pyx_n_s_kwargs;
 static PyObject *__pyx_n_s_long;
 static PyObject *__pyx_n_s_long_type_str;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_md5;
 static PyObject *__pyx_n_s_member_func;
 static PyObject *__pyx_n_s_metaclass;
+static PyObject *__pyx_n_s_method;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_original;
 static PyObject *__pyx_n_s_parameters;
 static PyObject *__pyx_n_s_pdb;
 static PyObject *__pyx_n_s_prepare;
@@ -2205,15 +2215,15 @@
 }
 
 /* "hermes/factors/base.pyx":93
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
- *         data = get_data_by_map(columns=dependencies_list,
+ *         method = 'ddb' if 'method' in kwargs else kwargs['method']
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6hermes_7factors_4base_10FactorBase_5init_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6hermes_7factors_4base_10FactorBase_4init_data[] = "FactorBase.init_data(self, **kwargs)";
 static PyMethodDef __pyx_mdef_6hermes_7factors_4base_10FactorBase_5init_data = {"init_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6hermes_7factors_4base_10FactorBase_5init_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6hermes_7factors_4base_10FactorBase_4init_data};
 static PyObject *__pyx_pw_6hermes_7factors_4base_10FactorBase_5init_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -2270,31 +2280,33 @@
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_6hermes_7factors_4base_10FactorBase_4init_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_kwargs) {
   PyObject *__pyx_v_dependencies_list = NULL;
+  PyObject *__pyx_v_method = NULL;
   PyObject *__pyx_v_data = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("init_data", 0);
 
   /* "hermes/factors/base.pyx":94
  * 
  *     def init_data(self, **kwargs):
  *         dependencies_list = self.get_dependencies()             # <<<<<<<<<<<<<<
+ *         method = 'ddb' if 'method' in kwargs else kwargs['method']
  *         data = get_data_by_map(columns=dependencies_list,
- *                       begin_date=kwargs['begin_date'],
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -2311,98 +2323,128 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_dependencies_list = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "hermes/factors/base.pyx":95
  *     def init_data(self, **kwargs):
  *         dependencies_list = self.get_dependencies()
+ *         method = 'ddb' if 'method' in kwargs else kwargs['method']             # <<<<<<<<<<<<<<
+ *         data = get_data_by_map(columns=dependencies_list,
+ *                       begin_date=kwargs['begin_date'],
+ */
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_method, __pyx_v_kwargs, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
+  if ((__pyx_t_4 != 0)) {
+    __Pyx_INCREF(__pyx_n_s_ddb);
+    __pyx_t_1 = __pyx_n_s_ddb;
+  } else {
+    __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_method); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __pyx_t_2;
+    __pyx_t_2 = 0;
+  }
+  __pyx_v_method = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "hermes/factors/base.pyx":96
+ *         dependencies_list = self.get_dependencies()
+ *         method = 'ddb' if 'method' in kwargs else kwargs['method']
  *         data = get_data_by_map(columns=dependencies_list,             # <<<<<<<<<<<<<<
  *                       begin_date=kwargs['begin_date'],
- *                       end_date=kwargs['end_date'])
+ *                       end_date=kwargs['end_date'],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_data_by_map); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_data_by_map); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_columns, __pyx_v_dependencies_list) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_columns, __pyx_v_dependencies_list) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":96
- *         dependencies_list = self.get_dependencies()
+  /* "hermes/factors/base.pyx":97
+ *         method = 'ddb' if 'method' in kwargs else kwargs['method']
  *         data = get_data_by_map(columns=dependencies_list,
  *                       begin_date=kwargs['begin_date'],             # <<<<<<<<<<<<<<
- *                       end_date=kwargs['end_date'])
- *         return data
+ *                       end_date=kwargs['end_date'],
+ *                       method=method)
  */
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_begin_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_begin_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_begin_date, __pyx_t_3) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_begin_date, __pyx_t_3) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/base.pyx":97
+  /* "hermes/factors/base.pyx":98
  *         data = get_data_by_map(columns=dependencies_list,
  *                       begin_date=kwargs['begin_date'],
- *                       end_date=kwargs['end_date'])             # <<<<<<<<<<<<<<
+ *                       end_date=kwargs['end_date'],             # <<<<<<<<<<<<<<
+ *                       method=method)
  *         return data
- * 
  */
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_end_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_end_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_end_date, __pyx_t_3) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_end_date, __pyx_t_3) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/base.pyx":95
- *     def init_data(self, **kwargs):
+  /* "hermes/factors/base.pyx":99
+ *                       begin_date=kwargs['begin_date'],
+ *                       end_date=kwargs['end_date'],
+ *                       method=method)             # <<<<<<<<<<<<<<
+ *         return data
+ * 
+ */
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_method, __pyx_v_method) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+
+  /* "hermes/factors/base.pyx":96
  *         dependencies_list = self.get_dependencies()
+ *         method = 'ddb' if 'method' in kwargs else kwargs['method']
  *         data = get_data_by_map(columns=dependencies_list,             # <<<<<<<<<<<<<<
  *                       begin_date=kwargs['begin_date'],
- *                       end_date=kwargs['end_date'])
+ *                       end_date=kwargs['end_date'],
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "hermes/factors/base.pyx":98
- *                       begin_date=kwargs['begin_date'],
- *                       end_date=kwargs['end_date'])
+  /* "hermes/factors/base.pyx":100
+ *                       end_date=kwargs['end_date'],
+ *                       method=method)
  *         return data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
   /* "hermes/factors/base.pyx":93
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
- *         data = get_data_by_map(columns=dependencies_list,
+ *         method = 'ddb' if 'method' in kwargs else kwargs['method']
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("hermes.factors.base.FactorBase.init_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_dependencies_list);
+  __Pyx_XDECREF(__pyx_v_method);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":102
+/* "hermes/factors/base.pyx":104
  * 
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
 
@@ -2439,222 +2481,222 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_dependencies", 0);
 
-  /* "hermes/factors/base.pyx":103
+  /* "hermes/factors/base.pyx":105
  * 
  *     def get_dependencies(self):
  *         dependencies_list = []             # <<<<<<<<<<<<<<
  *         member_func = self.factors_list()
  *         for func in member_func:
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_dependencies_list = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":104
+  /* "hermes/factors/base.pyx":106
  *     def get_dependencies(self):
  *         dependencies_list = []
  *         member_func = self.factors_list()             # <<<<<<<<<<<<<<
  *         for func in member_func:
  *             func_module = getattr(self, func)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_factors_list); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_factors_list); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_member_func = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":105
+  /* "hermes/factors/base.pyx":107
  *         dependencies_list = []
  *         member_func = self.factors_list()
  *         for func in member_func:             # <<<<<<<<<<<<<<
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  */
   if (likely(PyList_CheckExact(__pyx_v_member_func)) || PyTuple_CheckExact(__pyx_v_member_func)) {
     __pyx_t_1 = __pyx_v_member_func; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_member_func); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_member_func); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 105, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 107, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 105, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 107, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_5(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 105, __pyx_L1_error)
+          else __PYX_ERR(0, 107, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XDECREF_SET(__pyx_v_func, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "hermes/factors/base.pyx":106
+    /* "hermes/factors/base.pyx":108
  *         member_func = self.factors_list()
  *         for func in member_func:
  *             func_module = getattr(self, func)             # <<<<<<<<<<<<<<
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:
  */
-    __pyx_t_2 = __Pyx_GetAttr(__pyx_v_self, __pyx_v_func); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetAttr(__pyx_v_self, __pyx_v_func); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_func_module, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "hermes/factors/base.pyx":107
+    /* "hermes/factors/base.pyx":109
  *         for func in member_func:
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters             # <<<<<<<<<<<<<<
  *             if 'dependencies' in fun_param:
  *                 dependencies = fun_param['dependencies'].default
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_inspect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_inspect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_signature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_signature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_v_func_module) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_func_module);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_parameters); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_parameters); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF_SET(__pyx_v_fun_param, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "hermes/factors/base.pyx":108
+    /* "hermes/factors/base.pyx":110
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:             # <<<<<<<<<<<<<<
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies
  */
-    __pyx_t_7 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_dependencies, __pyx_v_fun_param, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_7 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_dependencies, __pyx_v_fun_param, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 110, __pyx_L1_error)
     __pyx_t_8 = (__pyx_t_7 != 0);
     if (__pyx_t_8) {
 
-      /* "hermes/factors/base.pyx":109
+      /* "hermes/factors/base.pyx":111
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:
  *                 dependencies = fun_param['dependencies'].default             # <<<<<<<<<<<<<<
  *                 dependencies_list += dependencies
  *         return list(set(dependencies_list))
  */
-      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 111, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_default); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_default); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_v_dependencies, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "hermes/factors/base.pyx":110
+      /* "hermes/factors/base.pyx":112
  *             if 'dependencies' in fun_param:
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies             # <<<<<<<<<<<<<<
  *         return list(set(dependencies_list))
  * 
  */
-      __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_dependencies_list, __pyx_v_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+      __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_dependencies_list, __pyx_v_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF_SET(__pyx_v_dependencies_list, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "hermes/factors/base.pyx":108
+      /* "hermes/factors/base.pyx":110
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:             # <<<<<<<<<<<<<<
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies
  */
     }
 
-    /* "hermes/factors/base.pyx":105
+    /* "hermes/factors/base.pyx":107
  *         dependencies_list = []
  *         member_func = self.factors_list()
  *         for func in member_func:             # <<<<<<<<<<<<<<
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":111
+  /* "hermes/factors/base.pyx":113
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies
  *         return list(set(dependencies_list))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PySet_New(__pyx_v_dependencies_list); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(__pyx_v_dependencies_list); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":102
+  /* "hermes/factors/base.pyx":104
  * 
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
 
@@ -2674,15 +2716,15 @@
   __Pyx_XDECREF(__pyx_v_fun_param);
   __Pyx_XDECREF(__pyx_v_dependencies);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":116
+/* "hermes/factors/base.pyx":118
  * 
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
 
@@ -2716,26 +2758,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_create_id") < 0)) __PYX_ERR(0, 116, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_create_id") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_create_id", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 116, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_create_id", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.base.FactorBase._create_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_8_create_id(__pyx_self, __pyx_v_self, __pyx_v_kwargs);
@@ -2758,103 +2800,103 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_create_id", 0);
 
-  /* "hermes/factors/base.pyx":117
+  /* "hermes/factors/base.pyx":119
  * 
  *     def _create_id(self, **kwargs):
  *         feature = copy.deepcopy(kwargs)             # <<<<<<<<<<<<<<
  *         feature['category'] = self.category
  *         s = hashlib.md5(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_copy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_deepcopy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_deepcopy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_kwargs) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_kwargs);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_feature = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":118
+  /* "hermes/factors/base.pyx":120
  *     def _create_id(self, **kwargs):
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category             # <<<<<<<<<<<<<<
  *         s = hashlib.md5(
  *             json.dumps(feature).encode(encoding="utf-8")).hexdigest()
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyObject_SetItem(__pyx_v_feature, __pyx_n_s_category, __pyx_t_1) < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_feature, __pyx_n_s_category, __pyx_t_1) < 0)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":119
+  /* "hermes/factors/base.pyx":121
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  *         s = hashlib.md5(             # <<<<<<<<<<<<<<
  *             json.dumps(feature).encode(encoding="utf-8")).hexdigest()
  *         return "{0}".format(create_id(original=s, digit=10))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_hashlib); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_hashlib); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_md5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_md5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":120
+  /* "hermes/factors/base.pyx":122
  *         feature['category'] = self.category
  *         s = hashlib.md5(
  *             json.dumps(feature).encode(encoding="utf-8")).hexdigest()             # <<<<<<<<<<<<<<
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_feature) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_feature);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_encoding, __pyx_kp_s_utf_8) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_encoding, __pyx_kp_s_utf_8) < 0) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
@@ -2863,55 +2905,55 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_hexdigest); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_hexdigest); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_s = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":121
+  /* "hermes/factors/base.pyx":123
  *         s = hashlib.md5(
  *             json.dumps(feature).encode(encoding="utf-8")).hexdigest()
  *         return "{0}".format(create_id(original=s, digit=10))             # <<<<<<<<<<<<<<
  * 
  *     def _format(self, data, name, **kwargs):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_0, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_0, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_create_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_create_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_original, __pyx_v_s) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_digit, __pyx_int_10) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_original, __pyx_v_s) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_digit, __pyx_int_10) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
@@ -2920,22 +2962,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":116
+  /* "hermes/factors/base.pyx":118
  * 
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
 
@@ -2953,15 +2995,15 @@
   __Pyx_XDECREF(__pyx_v_feature);
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":123
+/* "hermes/factors/base.pyx":125
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
  *         data = data.stack()
  *         data.name = name
  */
 
@@ -3003,40 +3045,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, 1); __PYX_ERR(0, 123, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, 1); __PYX_ERR(0, 125, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, 2); __PYX_ERR(0, 123, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, 2); __PYX_ERR(0, 125, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_format") < 0)) __PYX_ERR(0, 123, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_format") < 0)) __PYX_ERR(0, 125, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_data = values[1];
     __pyx_v_name = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 123, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_format", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 125, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.base.FactorBase._format", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_10_format(__pyx_self, __pyx_v_self, __pyx_v_data, __pyx_v_name, __pyx_v_kwargs);
@@ -3055,97 +3097,97 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_format", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "hermes/factors/base.pyx":124
+  /* "hermes/factors/base.pyx":126
  * 
  *     def _format(self, data, name, **kwargs):
  *         data = data.stack()             # <<<<<<<<<<<<<<
  *         data.name = name
  *         data.category = self.category
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_stack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_stack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":125
+  /* "hermes/factors/base.pyx":127
  *     def _format(self, data, name, **kwargs):
  *         data = data.stack()
  *         data.name = name             # <<<<<<<<<<<<<<
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":126
+  /* "hermes/factors/base.pyx":128
  *         data = data.stack()
  *         data.name = name
  *         data.category = self.category             # <<<<<<<<<<<<<<
  *         data.id = self._create_id(name=name, **kwargs)
  *         return data
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_category, __pyx_t_1) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_category, __pyx_t_1) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":127
+  /* "hermes/factors/base.pyx":129
  *         data.name = name
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_id_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_id_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
   __pyx_t_2 = __pyx_t_3;
   __pyx_t_3 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_id, __pyx_t_3) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_id, __pyx_t_3) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/base.pyx":128
+  /* "hermes/factors/base.pyx":130
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def factors_list(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":123
+  /* "hermes/factors/base.pyx":125
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
  *         data = data.stack()
  *         data.name = name
  */
 
@@ -3159,15 +3201,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":130
+/* "hermes/factors/base.pyx":132
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3182,15 +3224,15 @@
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_12factors_list(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":133
+/* "hermes/factors/base.pyx":135
  *         return list(
  *             filter(
  *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
  *                 callable(getattr(self, x)), dir(self)))
  */
 
 /* Python wrapper */
@@ -3221,66 +3263,66 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 0);
   __pyx_outer_scope = (struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_n_s_) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_6 = (!__pyx_t_5);
   if (__pyx_t_6) {
   } else {
-    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L3_bool_binop_done;
   }
 
-  /* "hermes/factors/base.pyx":134
+  /* "hermes/factors/base.pyx":136
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  *                 callable(getattr(self, x)), dir(self)))             # <<<<<<<<<<<<<<
  */
-  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 134, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 136, __pyx_L1_error) }
   __pyx_t_2 = __pyx_cur_scope->__pyx_v_self;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetAttr(__pyx_t_2, __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetAttr(__pyx_t_2, __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyCallable_Check(__pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyCallable_Check(__pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":133
+  /* "hermes/factors/base.pyx":135
  *         return list(
  *             filter(
  *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
  *                 callable(getattr(self, x)), dir(self)))
  */
 
   /* function exit code */
@@ -3293,15 +3335,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":130
+/* "hermes/factors/base.pyx":132
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3316,85 +3358,85 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("factors_list", 0);
   __pyx_cur_scope = (struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *)__pyx_tp_new_6hermes_7factors_4base___pyx_scope_struct__factors_list(__pyx_ptype_6hermes_7factors_4base___pyx_scope_struct__factors_list, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 130, __pyx_L1_error)
+    __PYX_ERR(0, 132, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
 
-  /* "hermes/factors/base.pyx":131
+  /* "hermes/factors/base.pyx":133
  * 
  *     def factors_list(self):
  *         return list(             # <<<<<<<<<<<<<<
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "hermes/factors/base.pyx":133
+  /* "hermes/factors/base.pyx":135
  *         return list(
  *             filter(
  *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
  *                 callable(getattr(self, x)), dir(self)))
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_12factors_list_lambda, 0, __pyx_n_s_FactorBase_factors_list_locals_l, ((PyObject*)__pyx_cur_scope), __pyx_n_s_hermes_factors_base, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_12factors_list_lambda, 0, __pyx_n_s_FactorBase_factors_list_locals_l, ((PyObject*)__pyx_cur_scope), __pyx_n_s_hermes_factors_base, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "hermes/factors/base.pyx":134
+  /* "hermes/factors/base.pyx":136
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  *                 callable(getattr(self, x)), dir(self)))             # <<<<<<<<<<<<<<
  */
   __pyx_t_2 = __pyx_cur_scope->__pyx_v_self;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_Dir(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Dir(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":132
+  /* "hermes/factors/base.pyx":134
  *     def factors_list(self):
  *         return list(
  *             filter(             # <<<<<<<<<<<<<<
  *                 lambda x: not x.startswith('_')  and
  *                 callable(getattr(self, x)), dir(self)))
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":131
+  /* "hermes/factors/base.pyx":133
  * 
  *     def factors_list(self):
  *         return list(             # <<<<<<<<<<<<<<
  *             filter(
  *                 lambda x: not x.startswith('_')  and
  */
-  __pyx_t_2 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":130
+  /* "hermes/factors/base.pyx":132
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3605,14 +3647,15 @@
   {&__pyx_n_s_category, __pyx_k_category, sizeof(__pyx_k_category), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_columns, __pyx_k_columns, sizeof(__pyx_k_columns), 0, 0, 1, 1},
   {&__pyx_n_s_copy, __pyx_k_copy, sizeof(__pyx_k_copy), 0, 0, 1, 1},
   {&__pyx_n_s_create_id, __pyx_k_create_id, sizeof(__pyx_k_create_id), 0, 0, 1, 1},
   {&__pyx_n_s_create_id_2, __pyx_k_create_id_2, sizeof(__pyx_k_create_id_2), 0, 0, 1, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
+  {&__pyx_n_s_ddb, __pyx_k_ddb, sizeof(__pyx_k_ddb), 0, 0, 1, 1},
   {&__pyx_n_s_deepcopy, __pyx_k_deepcopy, sizeof(__pyx_k_deepcopy), 0, 0, 1, 1},
   {&__pyx_n_s_default, __pyx_k_default, sizeof(__pyx_k_default), 0, 0, 1, 1},
   {&__pyx_n_s_dependencies, __pyx_k_dependencies, sizeof(__pyx_k_dependencies), 0, 0, 1, 1},
   {&__pyx_n_s_dependencies_list, __pyx_k_dependencies_list, sizeof(__pyx_k_dependencies_list), 0, 0, 1, 1},
   {&__pyx_n_s_digit, __pyx_k_digit, sizeof(__pyx_k_digit), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
   {&__pyx_n_s_dumps, __pyx_k_dumps, sizeof(__pyx_k_dumps), 0, 0, 1, 1},
@@ -3649,14 +3692,15 @@
   {&__pyx_n_s_kwargs, __pyx_k_kwargs, sizeof(__pyx_k_kwargs), 0, 0, 1, 1},
   {&__pyx_n_s_long, __pyx_k_long, sizeof(__pyx_k_long), 0, 0, 1, 1},
   {&__pyx_n_s_long_type_str, __pyx_k_long_type_str, sizeof(__pyx_k_long_type_str), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_md5, __pyx_k_md5, sizeof(__pyx_k_md5), 0, 0, 1, 1},
   {&__pyx_n_s_member_func, __pyx_k_member_func, sizeof(__pyx_k_member_func), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
+  {&__pyx_n_s_method, __pyx_k_method, sizeof(__pyx_k_method), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_original, __pyx_k_original, sizeof(__pyx_k_original), 0, 0, 1, 1},
   {&__pyx_n_s_parameters, __pyx_k_parameters, sizeof(__pyx_k_parameters), 0, 0, 1, 1},
   {&__pyx_n_s_pdb, __pyx_k_pdb, sizeof(__pyx_k_pdb), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
@@ -3671,15 +3715,15 @@
   {&__pyx_n_s_startswith, __pyx_k_startswith, sizeof(__pyx_k_startswith), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
   {&__pyx_n_s_with_metaclass, __pyx_k_with_metaclass, sizeof(__pyx_k_with_metaclass), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 134, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -3806,68 +3850,68 @@
   __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_self, 89, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 89, __pyx_L1_error)
 
   /* "hermes/factors/base.pyx":93
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
- *         data = get_data_by_map(columns=dependencies_list,
+ *         method = 'ddb' if 'method' in kwargs else kwargs['method']
  */
-  __pyx_tuple__22 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_dependencies_list, __pyx_n_s_data); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_dependencies_list, __pyx_n_s_method, __pyx_n_s_data); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_data, 93, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_data, 93, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 93, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":102
+  /* "hermes/factors/base.pyx":104
  * 
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
-  __pyx_tuple__24 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_dependencies_list, __pyx_n_s_member_func, __pyx_n_s_func, __pyx_n_s_func_module, __pyx_n_s_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_dependencies_list, __pyx_n_s_member_func, __pyx_n_s_func, __pyx_n_s_func_module, __pyx_n_s_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_get_dependencies, 102, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_get_dependencies, 104, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 104, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":116
+  /* "hermes/factors/base.pyx":118
  * 
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
-  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_feature, __pyx_n_s_s); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_feature, __pyx_n_s_s); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_create_id_2, 116, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_create_id_2, 118, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 118, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":123
+  /* "hermes/factors/base.pyx":125
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
  *         data = data.stack()
  *         data.name = name
  */
-  __pyx_tuple__28 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_name, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_name, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_format_2, 123, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_format_2, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 125, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":130
+  /* "hermes/factors/base.pyx":132
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_factors_list, 130, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_factors_list, 132, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3916,15 +3960,15 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_dictoffset && __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6hermes_7factors_4base___pyx_scope_struct__factors_list = &__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list;
@@ -4892,67 +4936,67 @@
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "hermes/factors/base.pyx":93
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
- *         data = get_data_by_map(columns=dependencies_list,
+ *         method = 'ddb' if 'method' in kwargs else kwargs['method']
  */
   __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_5init_data, 0, __pyx_n_s_FactorBase_init_data, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init_data, __pyx_t_4) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":102
+  /* "hermes/factors/base.pyx":104
  * 
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_7get_dependencies, 0, __pyx_n_s_FactorBase_get_dependencies, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_7get_dependencies, 0, __pyx_n_s_FactorBase_get_dependencies, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_get_dependencies, __pyx_t_4) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_get_dependencies, __pyx_t_4) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":116
+  /* "hermes/factors/base.pyx":118
  * 
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_9_create_id, 0, __pyx_n_s_FactorBase__create_id, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_9_create_id, 0, __pyx_n_s_FactorBase__create_id, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_create_id_2, __pyx_t_4) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_create_id_2, __pyx_t_4) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":123
+  /* "hermes/factors/base.pyx":125
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
  *         data = data.stack()
  *         data.name = name
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_11_format, 0, __pyx_n_s_FactorBase__format, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_11_format, 0, __pyx_n_s_FactorBase__format, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_format_2, __pyx_t_4) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_format_2, __pyx_t_4) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":130
+  /* "hermes/factors/base.pyx":132
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_13factors_list, 0, __pyx_n_s_FactorBase_factors_list, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_13factors_list, 0, __pyx_n_s_FactorBase_factors_list, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_factors_list, __pyx_t_4) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_factors_list, __pyx_t_4) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "hermes/factors/base.pyx":82
  * 
  * 
  * class FactorBase(six.with_metaclass(ABCMeta, ParamBase)):             # <<<<<<<<<<<<<<
  * 
@@ -5434,14 +5478,38 @@
     if (unlikely(!args)) return NULL;
     result = __Pyx_PyObject_Call(func, args, NULL);
     Py_DECREF(args);
     return result;
 }
 #endif
 
+/* DictGetItem */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
+    PyObject *value;
+    value = PyDict_GetItemWithError(d, key);
+    if (unlikely(!value)) {
+        if (!PyErr_Occurred()) {
+            if (unlikely(PyTuple_Check(key))) {
+                PyObject* args = PyTuple_Pack(1, key);
+                if (likely(args)) {
+                    PyErr_SetObject(PyExc_KeyError, args);
+                    Py_DECREF(args);
+                }
+            } else {
+                PyErr_SetObject(PyExc_KeyError, key);
+            }
+        }
+        return NULL;
+    }
+    Py_INCREF(value);
+    return value;
+}
+#endif
+
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -5495,38 +5563,14 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* DictGetItem */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
 /* GetAttr */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
 #if CYTHON_USE_TYPE_SLOTS
 #if PY_MAJOR_VERSION >= 3
     if (likely(PyUnicode_Check(n)))
 #else
     if (likely(PyString_Check(n)))
```

### Comparing `Finance-Hermes-0.2.6/hermes/factors/base.pyx` & `Finance-Hermes-0.2.7/hermes/factors/base.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -88,17 +88,19 @@
     @abstractmethod
     def _init_self(self, **kwargs):
         """子类因子针对可扩展参数的初始化"""
         pass
 
     def init_data(self, **kwargs):
         dependencies_list = self.get_dependencies()
+        method = 'ddb' if 'method' in kwargs else kwargs['method']
         data = get_data_by_map(columns=dependencies_list,
                       begin_date=kwargs['begin_date'],
-                      end_date=kwargs['end_date'])
+                      end_date=kwargs['end_date'],
+                      method=method)
         return data
 
 
     
     def get_dependencies(self):
         dependencies_list = []
         member_func = self.factors_list()
```

### Comparing `Finance-Hermes-0.2.6/hermes/kdutils/base.c` & `Finance-Hermes-0.2.7/hermes/kdutils/base.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/kdutils/base.pyx` & `Finance-Hermes-0.2.7/hermes/kdutils/base.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/kdutils/core/fixes.c` & `Finance-Hermes-0.2.7/hermes/kdutils/core/fixes.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/kdutils/core/fixes.pyx` & `Finance-Hermes-0.2.7/hermes/kdutils/core/fixes.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/kdutils/core/helper.c` & `Finance-Hermes-0.2.7/hermes/kdutils/core/helper.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/kdutils/core/helper.pyx` & `Finance-Hermes-0.2.7/hermes/kdutils/core/helper.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/kdutils/create_id.c` & `Finance-Hermes-0.2.7/hermes/kdutils/create_id.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/kdutils/create_id.pyx` & `Finance-Hermes-0.2.7/hermes/kdutils/create_id.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/kdutils/lazy.c` & `Finance-Hermes-0.2.7/hermes/kdutils/lazy.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/kdutils/lazy.pyx` & `Finance-Hermes-0.2.7/hermes/kdutils/lazy.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/lzador/calculater.c` & `Finance-Hermes-0.2.7/hermes/lzador/calculater.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/hermes/lzador/calculater.pyx` & `Finance-Hermes-0.2.7/hermes/lzador/calculater.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.6/setup.py` & `Finance-Hermes-0.2.7/setup.py`

 * *Files identical despite different names*

