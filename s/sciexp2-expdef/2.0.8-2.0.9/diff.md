# Comparing `tmp/sciexp2-expdef-2.0.8.tar.gz` & `tmp/sciexp2-expdef-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sciexp2-expdef-2.0.8.tar", last modified: Wed Nov 20 11:52:14 2019, max compression
+gzip compressed data, was "dist/sciexp2-expdef-2.0.9.tar", last modified: Sun Jan 19 14:31:18 2020, max compression
```

## Comparing `sciexp2-expdef-2.0.8.tar` & `sciexp2-expdef-2.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/
--rw-r--r--   0 root         (0) root         (0)     1582 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       32 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/.requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2_expdef.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2_expdef.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1582 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2_expdef.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      899 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2_expdef.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       32 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2_expdef.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2_expdef.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1663 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/README.md
--rwxrwxrwx   0 root         (0) root         (0)    12313 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/launcher
--rw-r--r--   0 root         (0) root         (0)       38 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2/common/
--rw-rw-rw-   0 root         (0) root         (0)    13805 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/common/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4838 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/common/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    16836 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14811 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/common/text.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9928 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/common/parallel.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/common/pp.py
--rw-rw-rw-   0 root         (0) root         (0)    23775 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/common/instance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/
--rw-rw-rw-   0 root         (0) root         (0)     1211 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/env.py
--rw-rw-rw-   0 root         (0) root         (0)    12014 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/system/
--rw-rw-rw-   0 root         (0) root         (0)     2223 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/system/shell.py
--rw-rw-rw-   0 root         (0) root         (0)    10024 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4276 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/system/gridengine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-20 11:52:14.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/templates/
--rw-rw-rw-   0 root         (0) root         (0)      527 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/templates/gridengine.dsc
--rwxrwxrwx   0 root         (0) root         (0)     5070 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/templates/gridengine.tpl
--rwxrwxrwx   0 root         (0) root         (0)     2687 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/templates/shell.tpl
--rw-rw-rw-   0 root         (0) root         (0)      264 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/templates/shell.dsc
--rw-rw-rw-   0 root         (0) root         (0)      848 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/templates/dacupc-gridengine.dsc
--rw-rw-rw-   0 root         (0) root         (0)    11348 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/launcher.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    51241 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/expdef/experiments.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-11-20 11:51:52.000000 sciexp2-expdef-2.0.8/sciexp2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2/common/
+-rw-rw-rw-   0 root         (0) root         (0)    14811 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/common/text.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9928 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/common/parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)    23775 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/common/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4838 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/common/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      926 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/common/pp.py
+-rw-rw-rw-   0 root         (0) root         (0)    13805 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/common/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)    16836 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/templates/
+-rwxrwxrwx   0 root         (0) root         (0)     2687 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/templates/shell.tpl
+-rwxrwxrwx   0 root         (0) root         (0)     5070 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/templates/gridengine.tpl
+-rw-rw-rw-   0 root         (0) root         (0)      527 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/templates/gridengine.dsc
+-rw-rw-rw-   0 root         (0) root         (0)      264 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/templates/shell.dsc
+-rw-rw-rw-   0 root         (0) root         (0)      848 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/templates/dacupc-gridengine.dsc
+-rw-rw-rw-   0 root         (0) root         (0)      346 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/system/
+-rw-rw-rw-   0 root         (0) root         (0)    10024 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/system/gridengine.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/system/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)    51241 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/experiments.py
+-rw-rw-rw-   0 root         (0) root         (0)    12014 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/env.py
+-rw-rw-rw-   0 root         (0) root         (0)    11348 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/sciexp2/expdef/launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2_expdef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1582 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2_expdef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      899 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2_expdef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2_expdef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2_expdef.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/sciexp2_expdef.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)    12313 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/launcher
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     1582 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       61 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       38 2020-01-19 14:31:18.000000 sciexp2-expdef-2.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       32 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/.requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2020-01-19 14:30:51.000000 sciexp2-expdef-2.0.9/setup.py
```

### Comparing `sciexp2-expdef-2.0.8/PKG-INFO` & `sciexp2-expdef-2.0.9/sciexp2_expdef.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sciexp2-expdef
-Version: 2.0.8
+Version: 2.0.9
 Summary: Experiment definition framework for SciExp²
 Home-page: https://sciexp2-expdef.readthedocs.io/
 Author: Lluís Vilanova
 Author-email: llvilanovag@gmail.com
 License: GNU General Public License (GPL) version 3 or later
 Description: SciExp²-ExpDef (aka *Scientific Experiment Exploration - Experiment Definition*)
         provides a framework for defining experiments, creating all the files needed for
```

### Comparing `sciexp2-expdef-2.0.8/sciexp2_expdef.egg-info/PKG-INFO` & `sciexp2-expdef-2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sciexp2-expdef
-Version: 2.0.8
+Version: 2.0.9
 Summary: Experiment definition framework for SciExp²
 Home-page: https://sciexp2-expdef.readthedocs.io/
 Author: Lluís Vilanova
 Author-email: llvilanovag@gmail.com
 License: GNU General Public License (GPL) version 3 or later
 Description: SciExp²-ExpDef (aka *Scientific Experiment Exploration - Experiment Definition*)
         provides a framework for defining experiments, creating all the files needed for
```

### Comparing `sciexp2-expdef-2.0.8/sciexp2_expdef.egg-info/SOURCES.txt` & `sciexp2-expdef-2.0.9/sciexp2_expdef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/setup.py` & `sciexp2-expdef-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/README.md` & `sciexp2-expdef-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/launcher` & `sciexp2-expdef-2.0.9/launcher`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/common/progress.py` & `sciexp2-expdef-2.0.9/sciexp2/common/progress.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/common/filter.py` & `sciexp2-expdef-2.0.9/sciexp2/common/filter.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/common/utils.py` & `sciexp2-expdef-2.0.9/sciexp2/common/utils.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/common/text.py` & `sciexp2-expdef-2.0.9/sciexp2/common/text.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/common/parallel.py` & `sciexp2-expdef-2.0.9/sciexp2/common/parallel.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/common/pp.py` & `sciexp2-expdef-2.0.9/sciexp2/common/pp.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/common/instance.py` & `sciexp2-expdef-2.0.9/sciexp2/common/instance.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/env.py` & `sciexp2-expdef-2.0.9/sciexp2/expdef/env.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/templates.py` & `sciexp2-expdef-2.0.9/sciexp2/expdef/templates.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/system/shell.py` & `sciexp2-expdef-2.0.9/sciexp2/expdef/system/shell.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/system/__init__.py` & `sciexp2-expdef-2.0.9/sciexp2/expdef/system/__init__.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/system/gridengine.py` & `sciexp2-expdef-2.0.9/sciexp2/expdef/system/gridengine.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/templates/gridengine.dsc` & `sciexp2-expdef-2.0.9/sciexp2/expdef/templates/gridengine.dsc`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/templates/gridengine.tpl` & `sciexp2-expdef-2.0.9/sciexp2/expdef/templates/gridengine.tpl`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/templates/shell.tpl` & `sciexp2-expdef-2.0.9/sciexp2/expdef/templates/shell.tpl`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/templates/dacupc-gridengine.dsc` & `sciexp2-expdef-2.0.9/sciexp2/expdef/templates/dacupc-gridengine.dsc`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/launcher.py` & `sciexp2-expdef-2.0.9/sciexp2/expdef/launcher.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.0.8/sciexp2/expdef/experiments.py` & `sciexp2-expdef-2.0.9/sciexp2/expdef/experiments.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -220,16 +220,16 @@
         else:
             key = variables_missing[0]
             variables_missing = variables_missing[1:]
 
             for val in variables[key]:
                 for exp in cartesian_product(base, variables_missing):
                     new_exp = Instance(base)
-                    new_exp[key] = val
                     new_exp.update(exp)
+                    new_exp[key] = val
                     yield new_exp
 
     def cartesian_product_ff(base, ff_info, ffs_missing=None):
         """Yield cartesian product of `ff_info` and overlay each on `base`"""
         if ffs_missing is None:
             ffs_missing = sorted(ff_info.keys())
 
@@ -239,17 +239,17 @@
         else:
             ff = ffs_missing[0]
             ffs_missing = ffs_missing[1:]
 
             for val in ff_info[ff][0]:
                 for exp in cartesian_product_ff(base, ff_info, ffs_missing):
                     new_exp = Instance(base)
+                    new_exp.update(exp)
                     for var in ff_info[ff][1]:
                         new_exp[var[0]] = val[var[1]]
-                    new_exp.update(exp)
                     yield new_exp
 
     def merge_old_experiment(exp, force=False):
         exp_dups = tuple(exp.items())
         if exp_dups not in new_dups:
             new_experiments.add(exp)
             new_dups.add(exp_dups)
```

