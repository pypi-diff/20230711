# Comparing `tmp/duckyshell-0.0.1.tar.gz` & `tmp/duckyshell-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckyshell-0.0.1.tar", last modified: Tue Jul 11 20:04:31 2023, max compression
+gzip compressed data, was "duckyshell-0.0.2.tar", last modified: Tue Jul 11 20:14:14 2023, max compression
```

## Comparing `duckyshell-0.0.1.tar` & `duckyshell-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:31.871890 duckyshell-0.0.1/
--rw-rw-rw-   0        0        0      153 2023-07-11 20:04:31.869871 duckyshell-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      604 2023-07-11 19:48:42.000000 duckyshell-0.0.1/README.md
--rw-rw-rw-   0        0        0      356 2023-07-11 19:58:36.000000 duckyshell-0.0.1/__init__.py
--rw-rw-rw-   0        0        0     1715 2023-07-11 19:48:42.000000 duckyshell-0.0.1/click.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:31.837639 duckyshell-0.0.1/duckyshell/
--rw-rw-rw-   0        0        0     3593 2023-07-11 19:48:42.000000 duckyshell-0.0.1/duckyshell/ducky.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:04:31.866475 duckyshell-0.0.1/duckyshell.egg-info/
--rw-rw-rw-   0        0        0      153 2023-07-11 20:04:31.000000 duckyshell-0.0.1/duckyshell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-11 20:04:31.000000 duckyshell-0.0.1/duckyshell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 20:04:31.000000 duckyshell-0.0.1/duckyshell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-11 20:04:31.000000 duckyshell-0.0.1/duckyshell.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-07-11 20:04:31.000000 duckyshell-0.0.1/duckyshell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 20:04:31.871890 duckyshell-0.0.1/setup.cfg
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:14:14.928613 duckyshell-0.0.2/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      211 2023-07-11 20:14:14.920834 duckyshell-0.0.2/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.2/README.md
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      356 2023-07-11 20:13:53.000000 duckyshell-0.0.2/__init__.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:14:14.513352 duckyshell-0.0.2/duckyshell/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     3593 2023-07-11 20:10:07.000000 duckyshell-0.0.2/duckyshell/main.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:14:14.847195 duckyshell-0.0.2/duckyshell.egg-info/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      211 2023-07-11 20:14:14.000000 duckyshell-0.0.2/duckyshell.egg-info/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      213 2023-07-11 20:14:14.000000 duckyshell-0.0.2/duckyshell.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-11 20:14:14.000000 duckyshell-0.0.2/duckyshell.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       54 2023-07-11 20:14:14.000000 duckyshell-0.0.2/duckyshell.egg-info/entry_points.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       11 2023-07-11 20:14:14.000000 duckyshell-0.0.2/duckyshell.egg-info/top_level.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-11 20:14:14.936649 duckyshell-0.0.2/setup.cfg
```

### Comparing `duckyshell-0.0.1/README.md` & `duckyshell-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `duckyshell-0.0.1/duckyshell/ducky.py` & `duckyshell-0.0.2/duckyshell/main.py`

 * *Files identical despite different names*

