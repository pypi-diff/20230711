# Comparing `tmp/duckyshell-0.0.2.tar.gz` & `tmp/duckyshell-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckyshell-0.0.2.tar", last modified: Tue Jul 11 20:14:14 2023, max compression
+gzip compressed data, was "duckyshell-0.0.3.tar", last modified: Tue Jul 11 20:18:05 2023, max compression
```

## Comparing `duckyshell-0.0.2.tar` & `duckyshell-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:14:14.928613 duckyshell-0.0.2/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      211 2023-07-11 20:14:14.920834 duckyshell-0.0.2/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.2/README.md
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      356 2023-07-11 20:13:53.000000 duckyshell-0.0.2/__init__.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:14:14.513352 duckyshell-0.0.2/duckyshell/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     3593 2023-07-11 20:10:07.000000 duckyshell-0.0.2/duckyshell/main.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:14:14.847195 duckyshell-0.0.2/duckyshell.egg-info/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      211 2023-07-11 20:14:14.000000 duckyshell-0.0.2/duckyshell.egg-info/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      213 2023-07-11 20:14:14.000000 duckyshell-0.0.2/duckyshell.egg-info/SOURCES.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-11 20:14:14.000000 duckyshell-0.0.2/duckyshell.egg-info/dependency_links.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       54 2023-07-11 20:14:14.000000 duckyshell-0.0.2/duckyshell.egg-info/entry_points.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       11 2023-07-11 20:14:14.000000 duckyshell-0.0.2/duckyshell.egg-info/top_level.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-11 20:14:14.936649 duckyshell-0.0.2/setup.cfg
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:18:05.017789 duckyshell-0.0.3/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      211 2023-07-11 20:18:05.009420 duckyshell-0.0.3/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.3/README.md
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      347 2023-07-11 20:17:46.000000 duckyshell-0.0.3/__init__.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:18:04.632079 duckyshell-0.0.3/duckyshell/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     3593 2023-07-11 20:10:07.000000 duckyshell-0.0.3/duckyshell/main.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:18:04.938027 duckyshell-0.0.3/duckyshell.egg-info/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      211 2023-07-11 20:18:04.000000 duckyshell-0.0.3/duckyshell.egg-info/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      213 2023-07-11 20:18:04.000000 duckyshell-0.0.3/duckyshell.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-11 20:18:04.000000 duckyshell-0.0.3/duckyshell.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       45 2023-07-11 20:18:04.000000 duckyshell-0.0.3/duckyshell.egg-info/entry_points.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       11 2023-07-11 20:18:04.000000 duckyshell-0.0.3/duckyshell.egg-info/top_level.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-11 20:18:05.021582 duckyshell-0.0.3/setup.cfg
```

### Comparing `duckyshell-0.0.2/README.md` & `duckyshell-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `duckyshell-0.0.2/duckyshell/main.py` & `duckyshell-0.0.3/duckyshell/main.py`

 * *Files identical despite different names*

