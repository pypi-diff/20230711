# Comparing `tmp/grokcore.site-3.1.tar.gz` & `tmp/grokcore.site-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grokcore.site-3.1.tar", last modified: Wed Sep  2 11:19:55 2020, max compression
+gzip compressed data, was "grokcore.site-4.0.tar", last modified: Tue Jul 11 06:34:46 2023, max compression
```

## Comparing `grokcore.site-3.1.tar` & `grokcore.site-4.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/
--rw-r--r--   0 janjaap    (501) staff       (20)     8059 2020-09-02 11:19:55.000000 grokcore.site-3.1/PKG-INFO
--rw-r--r--   0 janjaap    (501) staff       (20)       32 2020-09-02 11:19:54.000000 grokcore.site-3.1/COPYRIGHT.txt
--rw-r--r--   0 janjaap    (501) staff       (20)      124 2020-09-02 11:19:54.000000 grokcore.site-3.1/requirements.txt
--rw-r--r--   0 janjaap    (501) staff       (20)      399 2020-09-02 11:19:54.000000 grokcore.site-3.1/buildout.cfg
--rw-r--r--   0 janjaap    (501) staff       (20)     1993 2020-09-02 11:19:54.000000 grokcore.site-3.1/setup.py
--rw-r--r--   0 janjaap    (501) staff       (20)     1058 2020-09-02 11:19:54.000000 grokcore.site-3.1/tox.ini
--rw-r--r--   0 janjaap    (501) staff       (20)      157 2020-09-02 11:19:55.000000 grokcore.site-3.1/setup.cfg
--rw-r--r--   0 janjaap    (501) staff       (20)     2668 2020-09-02 11:19:54.000000 grokcore.site-3.1/README.rst
--rw-r--r--   0 janjaap    (501) staff       (20)     2070 2020-09-02 11:19:54.000000 grokcore.site-3.1/LICENSE.txt
--rw-r--r--   0 janjaap    (501) staff       (20)     2689 2020-09-02 11:19:54.000000 grokcore.site-3.1/CHANGES.rst
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore/
--rw-r--r--   0 janjaap    (501) staff       (20)      200 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/__init__.py
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore/site/
--rw-r--r--   0 janjaap    (501) staff       (20)     3546 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/interfaces.py
--rw-r--r--   0 janjaap    (501) staff       (20)      397 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/configure.zcml
--rw-r--r--   0 janjaap    (501) staff       (20)     2306 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/util.py
--rw-r--r--   0 janjaap    (501) staff       (20)     1689 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/subscriber.py
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore/site/tests/
--rw-r--r--   0 janjaap    (501) staff       (20)     1389 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/test_functional.py
--rw-r--r--   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/__init__.py
--rw-r--r--   0 janjaap    (501) staff       (20)     1607 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/test_base.py
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/
--rw-r--r--   0 janjaap    (501) staff       (20)       21 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/__init__.py
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/site/
--rw-r--r--   0 janjaap    (501) staff       (20)       21 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/site/__init__.py
--rw-r--r--   0 janjaap    (501) staff       (20)     1194 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/site/site.py
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/application/
--rw-r--r--   0 janjaap    (501) staff       (20)       21 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/application/__init__.py
--rw-r--r--   0 janjaap    (501) staff       (20)     1982 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/application/application.py
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/utility/
--rw-r--r--   0 janjaap    (501) staff       (20)     1377 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/utility/public.py
--rw-r--r--   0 janjaap    (501) staff       (20)     2876 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/utility/subclass.py
--rw-r--r--   0 janjaap    (501) staff       (20)     4386 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/utility/local.py
--rw-r--r--   0 janjaap    (501) staff       (20)       21 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/utility/__init__.py
--rw-r--r--   0 janjaap    (501) staff       (20)      959 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/utility/install_on.py
--rw-r--r--   0 janjaap    (501) staff       (20)      894 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/functional/utility/local_override.py
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore/site/tests/base/
--rw-r--r--   0 janjaap    (501) staff       (20)       21 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/base/__init__.py
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore/site/tests/base/application/
--rw-r--r--   0 janjaap    (501) staff       (20)       20 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/base/application/__init__.py
--rw-r--r--   0 janjaap    (501) staff       (20)     1003 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/base/application/application.py
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore/site/tests/base/utility/
--rw-r--r--   0 janjaap    (501) staff       (20)      134 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/tests/base/utility/local_implementsnone_fixture.py
--rw-r--r--   0 janjaap    (501) staff       (20)     1531 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/__init__.py
--rw-r--r--   0 janjaap    (501) staff       (20)     6493 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/directive.py
--rw-r--r--   0 janjaap    (501) staff       (20)      261 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/meta.zcml
--rw-r--r--   0 janjaap    (501) staff       (20)     3283 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/components.py
--rw-r--r--   0 janjaap    (501) staff       (20)      445 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/ftesting.zcml
--rw-r--r--   0 janjaap    (501) staff       (20)      988 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/testing.py
--rw-r--r--   0 janjaap    (501) staff       (20)     5017 2020-09-02 11:19:54.000000 grokcore.site-3.1/src/grokcore/site/meta.py
-drwxr-xr-x   0 janjaap    (501) staff       (20)        0 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore.site.egg-info/
--rw-r--r--   0 janjaap    (501) staff       (20)     8059 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore.site.egg-info/PKG-INFO
--rw-r--r--   0 janjaap    (501) staff       (20)        1 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore.site.egg-info/not-zip-safe
--rw-r--r--   0 janjaap    (501) staff       (20)        9 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore.site.egg-info/namespace_packages.txt
--rw-r--r--   0 janjaap    (501) staff       (20)     1691 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore.site.egg-info/SOURCES.txt
--rw-r--r--   0 janjaap    (501) staff       (20)      264 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore.site.egg-info/requires.txt
--rw-r--r--   0 janjaap    (501) staff       (20)        9 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore.site.egg-info/top_level.txt
--rw-r--r--   0 janjaap    (501) staff       (20)        1 2020-09-02 11:19:55.000000 grokcore.site-3.1/src/grokcore.site.egg-info/dependency_links.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.552715 grokcore.site-4.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2952 2023-07-11 06:34:46.000000 grokcore.site-4.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-11 06:34:46.000000 grokcore.site-4.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-11 06:34:46.000000 grokcore.site-4.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-11 06:34:46.000000 grokcore.site-4.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2023-07-11 06:34:46.000000 grokcore.site-4.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6601 2023-07-11 06:34:46.553065 grokcore.site-4.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2668 2023-07-11 06:34:46.000000 grokcore.site-4.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      418 2023-07-11 06:34:46.554478 grokcore.site-4.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2158 2023-07-11 06:34:46.000000 grokcore.site-4.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.483577 grokcore.site-4.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.499499 grokcore.site-4.0/src/grokcore/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      200 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.523042 grokcore.site-4.0/src/grokcore/site/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1531 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3276 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/components.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      397 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6481 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/directive.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      445 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/ftesting.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3589 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5054 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/meta.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      261 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1142 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/subscriber.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      989 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/testing.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.527718 grokcore.site-4.0/src/grokcore/site/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.529280 grokcore.site-4.0/src/grokcore/site/tests/base/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       21 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/base/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.532411 grokcore.site-4.0/src/grokcore/site/tests/base/application/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       20 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/base/application/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1003 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/base/application/application.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.533975 grokcore.site-4.0/src/grokcore/site/tests/base/utility/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      126 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/base/utility/local_implementsnone_fixture.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.535544 grokcore.site-4.0/src/grokcore/site/tests/functional/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       21 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.538710 grokcore.site-4.0/src/grokcore/site/tests/functional/application/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       21 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/application/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1982 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/application/application.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.541881 grokcore.site-4.0/src/grokcore/site/tests/functional/site/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       21 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/site/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1195 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/site/site.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.551433 grokcore.site-4.0/src/grokcore/site/tests/functional/utility/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       21 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/utility/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1023 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/utility/install_on.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4371 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/utility/local.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      912 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/utility/local_override.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1378 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/utility/public.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2877 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/functional/utility/subclass.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1128 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/test_base.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1133 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/tests/test_functional.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2375 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore/site/util.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:34:46.505872 grokcore.site-4.0/src/grokcore.site.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6601 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore.site.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1689 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore.site.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore.site.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore.site.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore.site.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      269 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore.site.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-11 06:34:46.000000 grokcore.site-4.0/src/grokcore.site.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1432 2023-07-11 06:34:46.000000 grokcore.site-4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grokcore.site-3.1/PKG-INFO` & `grokcore.site-4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,253 +1,265 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: grokcore.site
-Version: 3.1
+Version: 4.0
 Summary: Grok-like configuration for Zope local site and utilities
-Home-page: http://grok.zope.org
+Home-page: https://github.com/zopefoundation/grokcore.site
 Author: Grok Team
-Author-email: grok-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL
-Download-URL: http://pypi.python.org/pypi/grokcore.site
-Description-Content-Type: UNKNOWN
-Description: 
-        This package provides support to write local site and utilities for
-        Zope directly in Python (without ZCML).
-        
-        .. contents::
-        
-        
-        Setting up ``grokcore.site``
-        ============================
-        
-        This package is essentially set up like the `grokcore.component`_
-        package, please refer to its documentation for details.  The only
-        additional ZCML line you will need is::
-        
-          <include package="grokcore.site" />
-        
-        Put this somewhere near the top of your root ZCML file but below the
-        line where you include ``grokcore.component``'s configuration.
-        
-        
-        Examples
-        ========
-        
-        Global utilities are already managed by `grokcore.component`_.
-        
-        Here a simple example of a local utility::
-        
-          from zope.interface import implements, Interface
-          import grokcore.site
-        
-          class IKangaroo(Interface):
-        
-              def jump():
-                 """Make all kangaroos jump somewhere.
-                 """
-        
-          class KangarooUtility(grokcore.site.LocalUtility):
-              implements(IKangaroo)
-        
-              def jump(self):
-                  pass
-        
-        
-        Now, we can register our utility to a local site. That will create
-        automatically, and register that utility when we create that site::
-        
-        
-           class Jungle(grokcore.site.Site):
-        
-               grokcore.site.local_utility(KangarooUtility, IKangaroo)
-        
-        
-        If you don't add the last line, you will still have your site, but
-        nothing to make jump your kangaroo. Then, you will be able to add
-        manually by hand after (if you want).
-        
-        
-        API Overview
-        ============
-        
-        Base classes
-        ------------
-        
-        ``Site``
-           Base class for your site.
-        
-        ``LocalUtility``
-           Base class for a ZODB-persitent local utility.
-        
-        
-        Directives
-        ----------
-        
-        ``local_utility(factory, provides=None, name=u'', setup=None, public=False, name_in_container=None``)
-           Directive used on a site to register a local utility at the
-           creation time:
-        
-           ``factory``
-              Would be the component to register (required parameter),
-        
-           ``provides``
-              Would be the interface used to query the local utility (required
-              parameter),
-        
-           ``name``
-              Would be the name used to query the local utility,
-        
-           ``setup``
-              Would be a function taking parameter. If defined it will be
-              called after the utility is created with it as first and unique
-              parameter.
-        
-           ``public``
-              If true, the utility will be created in the site container
-              itself, not in the site manager, and public will be able to
-              access it directly.
-        
-           ``name_in_container``
-              Would be used as id for the utility in container itwill be
-              created. If not defined it will ask NameChooser to pick a name
-              for it.
-        
-        In addition, the ``grokcore.site`` package exposes the
-        `grokcore.component`_ API.
-        
-        .. _grokcore.component: http://pypi.python.org/pypi/grokcore.component
-        
-        Changes
-        =======
-        
-        3.1 (2020-09-02)
-        ----------------
-        
-        - Fix DeprecationWarnings.
-        
-        - Drop support for Python 3.4 and add support for 3.7 and 3.8.
-        
-        3.0.3 (2018-01-12)
-        ------------------
-        
-        - Rearrange tests such that Travis CI can pick up all functional tests too.
-        
-        3.0.2 (2018-01-11)
-        ------------------
-        
-        - Do not import `getSite` from `zope.site.hooks` anymore but from
-          `zope.component.hooks`.
-        
-        3.0.1 (2018-01-10)
-        ------------------
-        
-        - Fix dependencies by removing ZODB3.
-        
-        3.0.0 (2018-01-05)
-        ------------------
-        
-        - Python 3 compatibility.
-        
-        1.8 (2016-09-21)
-        ----------------
-        
-        - When removing a site make sure reference are removed from the parent
-          site.
-        
-        1.7.1 (2016-01-29)
-        ------------------
-        
-        - Update tests.
-        
-        1.7 (2015-06-11)
-        ----------------
-        
-        - Add a new directive ``install_on`` that is usable on a site. This
-          directive let you customize when (namely the event) to install the
-          configured local sites.
-        
-        - Rename ``ApplicationInitializedEvent`` to ``ApplicationAddedEvent``.
-        
-        - When the ``IApplicationAddedEvent`` is triggered the new application
-          will be current Zope local site. The site is restored after the
-          event.
-        
-        1.6.1 (2012-05-02)
-        ------------------
-        
-        - Exposed ApplicationInitializedEvent and IApplicationInitializedEvent.
-        
-        - Added the missing import for the exposed IApplication interface.
-        
-        1.6 (2012-05-01)
-        ----------------
-        
-        - Moved the directive `site` from Grok to this package.
-        
-        - Moved the component `Application` and all the related utilities from Grok
-          to this package.
-        
-        1.5 (2011-01-03)
-        ----------------
-        
-        - Moved IApplication and getApplication from the Grok package into
-          this one.
-        
-        1.4 (2010-11-01)
-        ----------------
-        
-        - Upped versions requirements for martian and grokcore.component.
-        
-        1.3 (2010-10-18)
-        ----------------
-        
-        - Made package comply to repository policy.
-        
-        - Update functional tests to only use zope.app.appsetup instead
-          of zope.app.testing.
-        
-        - Update functional tests not to require zope.app.zcmlfiles
-          anymore.
-        
-        1.2 (2009-12-20)
-        ----------------
-        
-        * Migrated imports from zope.app.component to zope.site.
-        
-        1.1 (2009-09-18)
-        ----------------
-        
-        * Updated dependencies (added missing ones and added separate test
-          dependencies).
-        
-        * A local utility now implements IAttributeAnnotatable.
-        
-        * Update code documentation from Grok itself.
-        
-        * Use 1.0b2 versions.cfg in Grok's release info instead of a local
-          copy; a local copy for all grokcore packages is just too hard to
-          maintain.
-        
-        
-        1.0.1 (2009-06-30)
-        ------------------
-        
-        * Reupload to pypi with a correct version of Python which doesn't have
-          a distutils bug.
-        
-        1.0 (2009-06-29)
-        ----------------
-        
-        * Created ``grokcore.site`` by factoring local site based components,
-          grokkers and directives out of Grok.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Zope :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Zope :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Provides-Extra: test
+License-File: LICENSE.txt
+
+
+This package provides support to write local site and utilities for
+Zope directly in Python (without ZCML).
+
+.. contents::
+
+
+Setting up ``grokcore.site``
+============================
+
+This package is essentially set up like the `grokcore.component`_
+package, please refer to its documentation for details.  The only
+additional ZCML line you will need is::
+
+  <include package="grokcore.site" />
+
+Put this somewhere near the top of your root ZCML file but below the
+line where you include ``grokcore.component``'s configuration.
+
+
+Examples
+========
+
+Global utilities are already managed by `grokcore.component`_.
+
+Here a simple example of a local utility::
+
+  from zope.interface import implements, Interface
+  import grokcore.site
+
+  class IKangaroo(Interface):
+
+      def jump():
+         """Make all kangaroos jump somewhere.
+         """
+
+  class KangarooUtility(grokcore.site.LocalUtility):
+      implements(IKangaroo)
+
+      def jump(self):
+          pass
+
+
+Now, we can register our utility to a local site. That will create
+automatically, and register that utility when we create that site::
+
+
+   class Jungle(grokcore.site.Site):
+
+       grokcore.site.local_utility(KangarooUtility, IKangaroo)
+
+
+If you don't add the last line, you will still have your site, but
+nothing to make jump your kangaroo. Then, you will be able to add
+manually by hand after (if you want).
+
+
+API Overview
+============
+
+Base classes
+------------
+
+``Site``
+   Base class for your site.
+
+``LocalUtility``
+   Base class for a ZODB-persitent local utility.
+
+
+Directives
+----------
+
+``local_utility(factory, provides=None, name=u'', setup=None, public=False, name_in_container=None``)
+   Directive used on a site to register a local utility at the
+   creation time:
+
+   ``factory``
+      Would be the component to register (required parameter),
+
+   ``provides``
+      Would be the interface used to query the local utility (required
+      parameter),
+
+   ``name``
+      Would be the name used to query the local utility,
+
+   ``setup``
+      Would be a function taking parameter. If defined it will be
+      called after the utility is created with it as first and unique
+      parameter.
+
+   ``public``
+      If true, the utility will be created in the site container
+      itself, not in the site manager, and public will be able to
+      access it directly.
+
+   ``name_in_container``
+      Would be used as id for the utility in container itwill be
+      created. If not defined it will ask NameChooser to pick a name
+      for it.
+
+In addition, the ``grokcore.site`` package exposes the
+`grokcore.component`_ API.
+
+.. _grokcore.component: http://pypi.python.org/pypi/grokcore.component
+
+Changes
+=======
+
+4.0 (2023-07-11)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+- Adapt code to ``zope.site >= 4.4`` thus requiring at least that version.
+  (`#7 <https://github.com/zopefoundation/grokcore.site/pull/7>`_)
+
+3.1 (2020-09-02)
+----------------
+
+- Fix DeprecationWarnings.
+
+- Drop support for Python 3.4 and add support for 3.7 and 3.8.
+
+3.0.3 (2018-01-12)
+------------------
+
+- Rearrange tests such that Travis CI can pick up all functional tests too.
+
+3.0.2 (2018-01-11)
+------------------
+
+- Do not import `getSite` from `zope.site.hooks` anymore but from
+  `zope.component.hooks`.
+
+3.0.1 (2018-01-10)
+------------------
+
+- Fix dependencies by removing ZODB3.
+
+3.0.0 (2018-01-05)
+------------------
+
+- Python 3 compatibility.
+
+1.8 (2016-09-21)
+----------------
+
+- When removing a site make sure reference are removed from the parent
+  site.
+
+1.7.1 (2016-01-29)
+------------------
+
+- Update tests.
+
+1.7 (2015-06-11)
+----------------
+
+- Add a new directive ``install_on`` that is usable on a site. This
+  directive let you customize when (namely the event) to install the
+  configured local sites.
+
+- Rename ``ApplicationInitializedEvent`` to ``ApplicationAddedEvent``.
+
+- When the ``IApplicationAddedEvent`` is triggered the new application
+  will be current Zope local site. The site is restored after the
+  event.
+
+1.6.1 (2012-05-02)
+------------------
+
+- Exposed ApplicationInitializedEvent and IApplicationInitializedEvent.
+
+- Added the missing import for the exposed IApplication interface.
+
+1.6 (2012-05-01)
+----------------
+
+- Moved the directive `site` from Grok to this package.
+
+- Moved the component `Application` and all the related utilities from Grok
+  to this package.
+
+1.5 (2011-01-03)
+----------------
+
+- Moved IApplication and getApplication from the Grok package into
+  this one.
+
+1.4 (2010-11-01)
+----------------
+
+- Upped versions requirements for martian and grokcore.component.
+
+1.3 (2010-10-18)
+----------------
+
+- Made package comply to repository policy.
+
+- Update functional tests to only use zope.app.appsetup instead
+  of zope.app.testing.
+
+- Update functional tests not to require zope.app.zcmlfiles
+  anymore.
+
+1.2 (2009-12-20)
+----------------
+
+* Migrated imports from zope.app.component to zope.site.
+
+1.1 (2009-09-18)
+----------------
+
+* Updated dependencies (added missing ones and added separate test
+  dependencies).
+
+* A local utility now implements IAttributeAnnotatable.
+
+* Update code documentation from Grok itself.
+
+* Use 1.0b2 versions.cfg in Grok's release info instead of a local
+  copy; a local copy for all grokcore packages is just too hard to
+  maintain.
+
+
+1.0.1 (2009-06-30)
+------------------
+
+* Reupload to pypi with a correct version of Python which doesn't have
+  a distutils bug.
+
+1.0 (2009-06-29)
+----------------
+
+* Created ``grokcore.site`` by factoring local site based components,
+  grokkers and directives out of Grok.
```

### Comparing `grokcore.site-3.1/setup.py` & `grokcore.site-4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from setuptools import setup, find_packages
 import os
 
+from setuptools import find_packages
+from setuptools import setup
+
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 long_description = (
     read('README.rst')
@@ -18,49 +20,51 @@
     'zope.configuration',
     'zope.testing',
     'grokcore.content',
     ]
 
 setup(
     name='grokcore.site',
-    version='3.1',
+    version='4.0',
     author='Grok Team',
-    author_email='grok-dev@zope.org',
-    url='http://grok.zope.org',
-    download_url='http://pypi.python.org/pypi/grokcore.site',
+    author_email='zope-dev@zope.dev',
+    url='https://github.com/zopefoundation/grokcore.site',
     description='Grok-like configuration for Zope local site and utilities',
     long_description=long_description,
     license='ZPL',
     classifiers=[
         'Environment :: Web Environment',
+        'Framework :: Zope :: 3',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Framework :: Zope :: 3',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy',
+        'Programming Language :: Python',
     ],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['grokcore'],
     include_package_data=True,
     zip_safe=False,
+    python_requires='>=3.7',
     install_requires=['setuptools',
                       'grokcore.component >= 2.1',
                       'martian >= 0.13',
                       'persistent',
                       'zope.annotation',
                       'zope.component',
                       'zope.container',
                       'zope.event',
                       'zope.interface',
                       'zope.lifecycleevent',
                       'zope.schema',
-                      'zope.site',
+                      'zope.site >= 4.4',
                       ],
     tests_require=tests_require,
     extras_require={'test': tests_require},
 )
```

### Comparing `grokcore.site-3.1/README.rst` & `grokcore.site-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `grokcore.site-3.1/LICENSE.txt` & `grokcore.site-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grokcore.site-3.1/CHANGES.rst` & `grokcore.site-4.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes
 =======
 
+4.0 (2023-07-11)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+- Adapt code to ``zope.site >= 4.4`` thus requiring at least that version.
+  (`#7 <https://github.com/zopefoundation/grokcore.site/pull/7>`_)
+
 3.1 (2020-09-02)
 ----------------
 
 - Fix DeprecationWarnings.
 
 - Drop support for Python 3.4 and add support for 3.7 and 3.8.
```

### Comparing `grokcore.site-3.1/src/grokcore/site/interfaces.py` & `grokcore.site-4.0/src/grokcore/site/interfaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
-from zope.interface import Interface, Attribute, implementer
+from zope.interface import Attribute
+from zope.interface import Interface
+from zope.interface import implementer
 from zope.interface.interfaces import IObjectEvent
+
 from grokcore.component.interfaces import IGrokcoreComponentAPI
 
 
 class IApplication(Interface):
     """Interface to mark the local site used as application root.
     """
 
@@ -27,44 +30,44 @@
 
     This event can be used to trigger the creation of contents or other tasks
     that require the application to be fully there : utilities installed
     and indexes created in the catalog."""
 
 
 @implementer(IApplicationAddedEvent)
-class ApplicationAddedEvent(object):
+class ApplicationAddedEvent:
     """A Grok Application has been added.
     """
 
     def __init__(self, app):
         assert IApplication.providedBy(app)
         self.object = app
 
 
 class IUtilityInstaller(Interface):
     """This install an utility in a site. Let you have different
     'installation' method if you want (one for Zope2 / Zope3).
     """
 
-    def __call__(site, utility, provides, name=u'',
+    def __call__(site, utility, provides, name='',
                  name_in_container=None, public=False, setup=None):
         """Setup an utility.
         """
 
 
 class IBaseClasses(Interface):
     Site = Attribute("Mixin class for sites.")
 
     LocalUtility = Attribute("Base class for local utilities.")
 
     Application = Attribute("Base class for applications.")
 
 
 class IDirectives(Interface):
-    def local_utility(factory, provides=None, name=u'',
+    def local_utility(factory, provides=None, name='',
                       setup=None, public=False, name_in_container=None):
         """Register a local utility.
 
         factory - the factory that creates the local utility
         provides - the interface the utility should be looked up with
         name - the name of the utility
         setup - a callable that receives the utility as its single argument,
```

### Comparing `grokcore.site-3.1/src/grokcore/site/util.py` & `grokcore.site-4.0/src/grokcore/site/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
-from grokcore.site.interfaces import IApplication, ApplicationAddedEvent
-from zope.component.hooks import getSite, setSite
+from zope.component.hooks import getSite
+from zope.component.hooks import setSite
 from zope.event import notify
 from zope.lifecycleevent import ObjectCreatedEvent
 from zope.schema.interfaces import WrongType
 
+from grokcore.site.interfaces import ApplicationAddedEvent
+from grokcore.site.interfaces import IApplication
+
 
 def getApplication():
     """Return the nearest enclosing :class:`grokcore.site.Application`.
 
     Raises :exc:`ValueError` if no application can be found.
     """
     site = getSite()
```

### Comparing `grokcore.site-3.1/src/grokcore/site/subscriber.py` & `grokcore.site-4.0/src/grokcore/site/subscriber.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,38 +9,22 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 from zope.lifecycleevent.interfaces import IObjectAddedEvent
-from zope.lifecycleevent.interfaces import IObjectRemovedEvent
 from zope.site import LocalSiteManager
-from zope.site.site import _findNextSiteManager
 
 import grokcore.component
 from grokcore.site.components import Site
 
 
 @grokcore.component.subscribe(Site, IObjectAddedEvent)
 def addSiteHandler(site, event):
     """Add a local site manager to a Grok site object upon its creation.
     """
     if event.oldParent is not None:
         return
     sitemanager = LocalSiteManager(site)
     del sitemanager['default']
     site.setSiteManager(sitemanager)
-
-
-@grokcore.component.subscribe(Site, IObjectRemovedEvent)
-def removeSiteHandler(site, event):
-    """Cleanup a after a site was removed.
-    """
-    if event.newParent is not None:
-        # Please note that the code for moving a site is properly implemented
-        # inside zope.site.
-        return
-    local = site.getSiteManager()
-    parent = _findNextSiteManager(site)
-    if parent is not None:
-        parent.removeSub(local)
```

### Comparing `grokcore.site-3.1/src/grokcore/site/tests/functional/site/site.py` & `grokcore.site-4.0/src/grokcore/site/tests/functional/site/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,19 @@
   >>> nonsitecontainer['manfred'] = manfred
   >>> ISite.providedBy(manfred)
   True
   >>> nonsitecontainer['herd'] = herd
   >>> ISite.providedBy(herd)
   True
 """
-import grokcore.site
 from persistent import Persistent
 from zope.container.btree import BTreeContainer
 
+import grokcore.site
+
 
 class Mammoth(grokcore.site.Site):
     pass
 
 
 class Herd(grokcore.site.Site):
     pass
```

### Comparing `grokcore.site-3.1/src/grokcore/site/tests/functional/application/application.py` & `grokcore.site-4.0/src/grokcore/site/tests/functional/application/application.py`

 * *Files identical despite different names*

### Comparing `grokcore.site-3.1/src/grokcore/site/tests/functional/utility/public.py` & `grokcore.site-4.0/src/grokcore/site/tests/functional/utility/public.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,19 @@
    >>> setSite(cave2)
    >>> (cave2.getSiteManager()['fireplace'] is
    ...  component.getUtility(IFireplace))
    True
 
 """
 
-import grokcore.site
 from zope import interface
 from zope.container.btree import BTreeContainer
 
+import grokcore.site
+
 
 class IFireplace(interface.Interface):
     pass
 
 
 @interface.implementer(IFireplace)
 class Fireplace(grokcore.site.LocalUtility):
```

### Comparing `grokcore.site-3.1/src/grokcore/site/tests/functional/utility/subclass.py` & `grokcore.site-4.0/src/grokcore/site/tests/functional/utility/subclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,18 @@
 
   >>> setSite(scary)
   >>> fireplace = component.getUtility(IFireplace)
   >>> painting = component.getUtility(IPainting)
   >>> great_painting = component.getUtility(IPainting, 'great')
   >>> bad_painting = component.getUtility(IPainting, 'bad')
 """  # noqa: E501
-import grokcore.site
 from zope import interface
 
+import grokcore.site
+
 
 class IFireplace(interface.Interface):
     pass
 
 
 class IPainting(interface.Interface):
     pass
```

### Comparing `grokcore.site-3.1/src/grokcore/site/tests/functional/utility/local.py` & `grokcore.site-4.0/src/grokcore/site/tests/functional/utility/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,18 @@
   zope.interface.interfaces.ComponentLookupError: (<InterfaceClass grokcore.site.tests.functional.utility.local.IPainting>, 'blackandwhite')
 
   >>> component.getUtility(IPainting, name='color')
   Traceback (most recent call last):
     ...
   zope.interface.interfaces.ComponentLookupError: (<InterfaceClass grokcore.site.tests.functional.utility.local.IPainting>, 'color')
 """  # noqa: E501
-import grokcore.site
-from zope import interface
 import persistent
+from zope import interface
+
+import grokcore.site
 
 
 class IFireplace(interface.Interface):
     pass
 
 
 class IClub(interface.Interface):
@@ -112,20 +113,20 @@
 
 @interface.implementer(IFireplace)
 class Fireplace(grokcore.site.LocalUtility):
     pass
 
 
 @interface.implementer(IClub)
-class Club(object):
+class Club:
     pass
 
 
 @interface.implementer(IClub, ISpiky)
-class SpikyClub(object):
+class SpikyClub:
     pass
 
 
 @interface.implementer(IMammoth, IClub)
 class Mammoth(grokcore.site.LocalUtility):
     pass
```

### Comparing `grokcore.site-3.1/src/grokcore/site/tests/functional/utility/install_on.py` & `grokcore.site-4.0/src/grokcore/site/tests/functional/utility/install_on.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,20 @@
   True
 
   >>> notify(PartyEvent(cave))
   >>> club = queryUtility(IClub)
   >>> IClub.providedBy(club)
   True
 """
+from zope.interface import Interface
+from zope.interface import implementer
+from zope.interface.interfaces import IObjectEvent
+from zope.interface.interfaces import ObjectEvent
+
 import grokcore.site
-from zope.interface import Interface, implementer
-from zope.interface.interfaces import ObjectEvent, IObjectEvent
 
 
 class IPartyEvent(IObjectEvent):
     pass
 
 
 @implementer(IPartyEvent)
```

### Comparing `grokcore.site-3.1/src/grokcore/site/tests/functional/utility/local_override.py` & `grokcore.site-4.0/src/grokcore/site/tests/functional/utility/local_override.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,21 @@
   >>> names = list(cave.getSiteManager().keys())
   >>> len(names)
   1
 
   >>> print(names[0])
   SpikyClub
 
+  >>> setSite()
+
 """
-import grokcore.site
 from zope import interface
 
+import grokcore.site
+
 
 class IClub(interface.Interface):
     pass
 
 
 @interface.implementer(IClub)
 class Club(grokcore.site.LocalUtility):
```

### Comparing `grokcore.site-3.1/src/grokcore/site/tests/base/application/application.py` & `grokcore.site-4.0/src/grokcore/site/tests/base/application/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     <class 'grokcore.site.tests.base.application.application.Calendar'>
 
 Applications are both containers and sites::
 
     >>> issubclass(calendar_app, grokcore.site.Site)
     True
 
-Applications can be instanciated without any arguments::
+Applications can be instantiated without any arguments::
 
     >>> calendar = calendar_app()
     >>> calendar
     <grokcore.site.tests.base.application.application.Calendar object at 0x...>
 
 """
```

### Comparing `grokcore.site-3.1/src/grokcore/site/__init__.py` & `grokcore.site-4.0/src/grokcore/site/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 from zope.component.hooks import getSite  # noqa: F401
-from grokcore.component import *  # noqa: F401, F403
-from grokcore.site.directive import site  # noqa: F401
-from grokcore.site.directive import local_utility  # noqa: F401
-from grokcore.site.directive import install_on  # noqa: F401
-from grokcore.site.components import Site  # noqa: F401
-from grokcore.site.components import LocalUtility  # noqa: F401
-from grokcore.site.components import Application  # noqa: F401
-from grokcore.site.util import getApplication  # noqa: F401
 
 import grokcore.site.testing  # noqa: F401
-
+from grokcore.component import *  # noqa: F401, F403
+from grokcore.site.components import Application  # noqa: F401
+from grokcore.site.components import LocalUtility  # noqa: F401
+from grokcore.site.components import Site  # noqa: F401
+from grokcore.site.directive import install_on  # noqa: F401
+from grokcore.site.directive import local_utility  # noqa: F401
+from grokcore.site.directive import site  # noqa: F401
+from grokcore.site.interfaces import ApplicationAddedEvent  # noqa: F401
 from grokcore.site.interfaces import IApplication  # noqa: F401
 from grokcore.site.interfaces import IApplicationAddedEvent  # noqa: F401
-from grokcore.site.interfaces import ApplicationAddedEvent  # noqa: F401
-
 from grokcore.site.interfaces import IGrokcoreSiteAPI  # noqa: F401
+from grokcore.site.util import getApplication  # noqa: F401
+
+
 __all__ = list(IGrokcoreSiteAPI)
```

### Comparing `grokcore.site-3.1/src/grokcore/site/directive.py` & `grokcore.site-4.0/src/grokcore/site/directive.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grok directives.
 """
 
-import grokcore.component
-
-from grokcore.site.components import LocalUtility
-
-from zope import interface
-from zope.interface.interfaces import IInterface
-
 import martian
 from martian import util
 from martian.error import GrokImportError
+from zope import interface
+from zope.interface.interfaces import IInterface
+
+import grokcore.component
+from grokcore.site.components import LocalUtility
 
 
 class site(martian.Directive):
     """This directive is used to indicate the Grok site
     object for which the component should be used/registered.
     """
     scope = martian.CLASS
@@ -78,15 +76,15 @@
     interface.
 
     """
 
     scope = martian.CLASS
     store = martian.DICT
 
-    def factory(self, factory, provides=None, name=u'',
+    def factory(self, factory, provides=None, name='',
                 setup=None, public=False, name_in_container=None):
         if provides is not None and not IInterface.providedBy(provides):
             raise GrokImportError("You can only pass an interface to the "
                                   "provides argument of %s." % self.name)
 
         if provides is None:
             # We cannot bind the provides directive and get information
@@ -124,30 +122,30 @@
                 (factory, provides, name), factory)
 
         info = LocalUtilityInfo(factory, provides, name, setup, public,
                                 name_in_container)
         return (provides, name), info
 
 
-class LocalUtilityInfo(object):
+class LocalUtilityInfo:
     """The information about how to register a local utility.
 
     An instance of this class is created for each
     `grokcore.site.local_utility()` in a Grok application's code, to
     remember how the user wants their local utility registered.
     Later, whenever the application creates new instances of the site
     or application for which the local utility directive was supplied,
     this block of information is used as the parameters to the
     creation of the local utility which is created along with the new
     site in the Zope database.
 
     """
     _order = 0
 
-    def __init__(self, factory, provides, name=u'',
+    def __init__(self, factory, provides, name='',
                  setup=None, public=False, name_in_container=None):
         self.factory = factory
         self.provides = provides
         self.name = name
         self.setup = setup
         self.public = public
         self.name_in_container = name_in_container
```

### Comparing `grokcore.site-3.1/src/grokcore/site/components.py` & `grokcore.site-4.0/src/grokcore/site/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 from persistent import Persistent
-from grokcore.component.interfaces import IContext
-from grokcore.site.interfaces import IApplication
 from zope.annotation.interfaces import IAttributeAnnotatable
 from zope.container.contained import Contained
 from zope.interface import implementer
 from zope.site.site import SiteManagerContainer
 
+from grokcore.component.interfaces import IContext
+from grokcore.site.interfaces import IApplication
+
 
-class BaseSite(object):
+class BaseSite:
     """Mixin to grok sites in Grok applications.
 
     It's used to let different implementation of sites to exists, and
     still being grokked correctly.
     """
```

### Comparing `grokcore.site-3.1/src/grokcore/site/testing.py` & `grokcore.site-4.0/src/grokcore/site/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grok test helpers
 """
 from zope.configuration.config import ConfigurationMachine
+
 from grokcore.component import zcml
 
 
 def grok(module_name):
     config = ConfigurationMachine()
     zcml.do_grok('grokcore.component.meta', config)
     zcml.do_grok('grokcore.site.meta', config)
```

### Comparing `grokcore.site-3.1/src/grokcore/site/meta.py` & `grokcore.site-4.0/src/grokcore/site/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
-from zope import component
-
-from zope.lifecycleevent.interfaces import IObjectAddedEvent
-from zope.container.interfaces import IContainer,  INameChooser
-
 import martian
 from martian.error import GrokError
+from zope import component
+from zope.container.interfaces import IContainer
+from zope.container.interfaces import INameChooser
+from zope.lifecycleevent.interfaces import IObjectAddedEvent
 
 import grokcore.component
 import grokcore.site
 import grokcore.site.components
 import grokcore.site.interfaces
 
 
@@ -75,15 +74,15 @@
 
     # we are done. If this subscriber gets fired again, we therefore
     # do not register utilities anymore
     site.__grok_utilities_installed__ = True
 
 
 @grokcore.component.provider(grokcore.site.interfaces.IUtilityInstaller)
-def setupUtility(site, utility, provides, name=u'',
+def setupUtility(site, utility, provides, name='',
                  name_in_container=None, public=False, setup=None):
     """Set up a utility in a site.
 
     site - the site to set up the utility in
     utility - the utility to set up
     provides - the interface the utility should be registered with
     name - the name the utility should be registered under, default
@@ -119,14 +118,14 @@
     """Grokker for Grok application classes."""
     martian.component(grokcore.site.components.Application)
     martian.priority(500)
 
     def grok(self, name, factory, module_info, config, **kw):
         # XXX fail loudly if the same application name is used twice.
         provides = grokcore.site.interfaces.IApplication
-        name = '%s.%s' % (module_info.dotted_name, name)
+        name = '{}.{}'.format(module_info.dotted_name, name)
         config.action(
             discriminator=('utility', provides, name),
             callable=grokcore.component.provideUtility,
             args=(factory, provides, name),
             )
         return True
```

### Comparing `grokcore.site-3.1/src/grokcore.site.egg-info/PKG-INFO` & `grokcore.site-4.0/src/grokcore.site.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,253 +1,265 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: grokcore.site
-Version: 3.1
+Version: 4.0
 Summary: Grok-like configuration for Zope local site and utilities
-Home-page: http://grok.zope.org
+Home-page: https://github.com/zopefoundation/grokcore.site
 Author: Grok Team
-Author-email: grok-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL
-Download-URL: http://pypi.python.org/pypi/grokcore.site
-Description-Content-Type: UNKNOWN
-Description: 
-        This package provides support to write local site and utilities for
-        Zope directly in Python (without ZCML).
-        
-        .. contents::
-        
-        
-        Setting up ``grokcore.site``
-        ============================
-        
-        This package is essentially set up like the `grokcore.component`_
-        package, please refer to its documentation for details.  The only
-        additional ZCML line you will need is::
-        
-          <include package="grokcore.site" />
-        
-        Put this somewhere near the top of your root ZCML file but below the
-        line where you include ``grokcore.component``'s configuration.
-        
-        
-        Examples
-        ========
-        
-        Global utilities are already managed by `grokcore.component`_.
-        
-        Here a simple example of a local utility::
-        
-          from zope.interface import implements, Interface
-          import grokcore.site
-        
-          class IKangaroo(Interface):
-        
-              def jump():
-                 """Make all kangaroos jump somewhere.
-                 """
-        
-          class KangarooUtility(grokcore.site.LocalUtility):
-              implements(IKangaroo)
-        
-              def jump(self):
-                  pass
-        
-        
-        Now, we can register our utility to a local site. That will create
-        automatically, and register that utility when we create that site::
-        
-        
-           class Jungle(grokcore.site.Site):
-        
-               grokcore.site.local_utility(KangarooUtility, IKangaroo)
-        
-        
-        If you don't add the last line, you will still have your site, but
-        nothing to make jump your kangaroo. Then, you will be able to add
-        manually by hand after (if you want).
-        
-        
-        API Overview
-        ============
-        
-        Base classes
-        ------------
-        
-        ``Site``
-           Base class for your site.
-        
-        ``LocalUtility``
-           Base class for a ZODB-persitent local utility.
-        
-        
-        Directives
-        ----------
-        
-        ``local_utility(factory, provides=None, name=u'', setup=None, public=False, name_in_container=None``)
-           Directive used on a site to register a local utility at the
-           creation time:
-        
-           ``factory``
-              Would be the component to register (required parameter),
-        
-           ``provides``
-              Would be the interface used to query the local utility (required
-              parameter),
-        
-           ``name``
-              Would be the name used to query the local utility,
-        
-           ``setup``
-              Would be a function taking parameter. If defined it will be
-              called after the utility is created with it as first and unique
-              parameter.
-        
-           ``public``
-              If true, the utility will be created in the site container
-              itself, not in the site manager, and public will be able to
-              access it directly.
-        
-           ``name_in_container``
-              Would be used as id for the utility in container itwill be
-              created. If not defined it will ask NameChooser to pick a name
-              for it.
-        
-        In addition, the ``grokcore.site`` package exposes the
-        `grokcore.component`_ API.
-        
-        .. _grokcore.component: http://pypi.python.org/pypi/grokcore.component
-        
-        Changes
-        =======
-        
-        3.1 (2020-09-02)
-        ----------------
-        
-        - Fix DeprecationWarnings.
-        
-        - Drop support for Python 3.4 and add support for 3.7 and 3.8.
-        
-        3.0.3 (2018-01-12)
-        ------------------
-        
-        - Rearrange tests such that Travis CI can pick up all functional tests too.
-        
-        3.0.2 (2018-01-11)
-        ------------------
-        
-        - Do not import `getSite` from `zope.site.hooks` anymore but from
-          `zope.component.hooks`.
-        
-        3.0.1 (2018-01-10)
-        ------------------
-        
-        - Fix dependencies by removing ZODB3.
-        
-        3.0.0 (2018-01-05)
-        ------------------
-        
-        - Python 3 compatibility.
-        
-        1.8 (2016-09-21)
-        ----------------
-        
-        - When removing a site make sure reference are removed from the parent
-          site.
-        
-        1.7.1 (2016-01-29)
-        ------------------
-        
-        - Update tests.
-        
-        1.7 (2015-06-11)
-        ----------------
-        
-        - Add a new directive ``install_on`` that is usable on a site. This
-          directive let you customize when (namely the event) to install the
-          configured local sites.
-        
-        - Rename ``ApplicationInitializedEvent`` to ``ApplicationAddedEvent``.
-        
-        - When the ``IApplicationAddedEvent`` is triggered the new application
-          will be current Zope local site. The site is restored after the
-          event.
-        
-        1.6.1 (2012-05-02)
-        ------------------
-        
-        - Exposed ApplicationInitializedEvent and IApplicationInitializedEvent.
-        
-        - Added the missing import for the exposed IApplication interface.
-        
-        1.6 (2012-05-01)
-        ----------------
-        
-        - Moved the directive `site` from Grok to this package.
-        
-        - Moved the component `Application` and all the related utilities from Grok
-          to this package.
-        
-        1.5 (2011-01-03)
-        ----------------
-        
-        - Moved IApplication and getApplication from the Grok package into
-          this one.
-        
-        1.4 (2010-11-01)
-        ----------------
-        
-        - Upped versions requirements for martian and grokcore.component.
-        
-        1.3 (2010-10-18)
-        ----------------
-        
-        - Made package comply to repository policy.
-        
-        - Update functional tests to only use zope.app.appsetup instead
-          of zope.app.testing.
-        
-        - Update functional tests not to require zope.app.zcmlfiles
-          anymore.
-        
-        1.2 (2009-12-20)
-        ----------------
-        
-        * Migrated imports from zope.app.component to zope.site.
-        
-        1.1 (2009-09-18)
-        ----------------
-        
-        * Updated dependencies (added missing ones and added separate test
-          dependencies).
-        
-        * A local utility now implements IAttributeAnnotatable.
-        
-        * Update code documentation from Grok itself.
-        
-        * Use 1.0b2 versions.cfg in Grok's release info instead of a local
-          copy; a local copy for all grokcore packages is just too hard to
-          maintain.
-        
-        
-        1.0.1 (2009-06-30)
-        ------------------
-        
-        * Reupload to pypi with a correct version of Python which doesn't have
-          a distutils bug.
-        
-        1.0 (2009-06-29)
-        ----------------
-        
-        * Created ``grokcore.site`` by factoring local site based components,
-          grokkers and directives out of Grok.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Zope :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Zope :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Provides-Extra: test
+License-File: LICENSE.txt
+
+
+This package provides support to write local site and utilities for
+Zope directly in Python (without ZCML).
+
+.. contents::
+
+
+Setting up ``grokcore.site``
+============================
+
+This package is essentially set up like the `grokcore.component`_
+package, please refer to its documentation for details.  The only
+additional ZCML line you will need is::
+
+  <include package="grokcore.site" />
+
+Put this somewhere near the top of your root ZCML file but below the
+line where you include ``grokcore.component``'s configuration.
+
+
+Examples
+========
+
+Global utilities are already managed by `grokcore.component`_.
+
+Here a simple example of a local utility::
+
+  from zope.interface import implements, Interface
+  import grokcore.site
+
+  class IKangaroo(Interface):
+
+      def jump():
+         """Make all kangaroos jump somewhere.
+         """
+
+  class KangarooUtility(grokcore.site.LocalUtility):
+      implements(IKangaroo)
+
+      def jump(self):
+          pass
+
+
+Now, we can register our utility to a local site. That will create
+automatically, and register that utility when we create that site::
+
+
+   class Jungle(grokcore.site.Site):
+
+       grokcore.site.local_utility(KangarooUtility, IKangaroo)
+
+
+If you don't add the last line, you will still have your site, but
+nothing to make jump your kangaroo. Then, you will be able to add
+manually by hand after (if you want).
+
+
+API Overview
+============
+
+Base classes
+------------
+
+``Site``
+   Base class for your site.
+
+``LocalUtility``
+   Base class for a ZODB-persitent local utility.
+
+
+Directives
+----------
+
+``local_utility(factory, provides=None, name=u'', setup=None, public=False, name_in_container=None``)
+   Directive used on a site to register a local utility at the
+   creation time:
+
+   ``factory``
+      Would be the component to register (required parameter),
+
+   ``provides``
+      Would be the interface used to query the local utility (required
+      parameter),
+
+   ``name``
+      Would be the name used to query the local utility,
+
+   ``setup``
+      Would be a function taking parameter. If defined it will be
+      called after the utility is created with it as first and unique
+      parameter.
+
+   ``public``
+      If true, the utility will be created in the site container
+      itself, not in the site manager, and public will be able to
+      access it directly.
+
+   ``name_in_container``
+      Would be used as id for the utility in container itwill be
+      created. If not defined it will ask NameChooser to pick a name
+      for it.
+
+In addition, the ``grokcore.site`` package exposes the
+`grokcore.component`_ API.
+
+.. _grokcore.component: http://pypi.python.org/pypi/grokcore.component
+
+Changes
+=======
+
+4.0 (2023-07-11)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+- Adapt code to ``zope.site >= 4.4`` thus requiring at least that version.
+  (`#7 <https://github.com/zopefoundation/grokcore.site/pull/7>`_)
+
+3.1 (2020-09-02)
+----------------
+
+- Fix DeprecationWarnings.
+
+- Drop support for Python 3.4 and add support for 3.7 and 3.8.
+
+3.0.3 (2018-01-12)
+------------------
+
+- Rearrange tests such that Travis CI can pick up all functional tests too.
+
+3.0.2 (2018-01-11)
+------------------
+
+- Do not import `getSite` from `zope.site.hooks` anymore but from
+  `zope.component.hooks`.
+
+3.0.1 (2018-01-10)
+------------------
+
+- Fix dependencies by removing ZODB3.
+
+3.0.0 (2018-01-05)
+------------------
+
+- Python 3 compatibility.
+
+1.8 (2016-09-21)
+----------------
+
+- When removing a site make sure reference are removed from the parent
+  site.
+
+1.7.1 (2016-01-29)
+------------------
+
+- Update tests.
+
+1.7 (2015-06-11)
+----------------
+
+- Add a new directive ``install_on`` that is usable on a site. This
+  directive let you customize when (namely the event) to install the
+  configured local sites.
+
+- Rename ``ApplicationInitializedEvent`` to ``ApplicationAddedEvent``.
+
+- When the ``IApplicationAddedEvent`` is triggered the new application
+  will be current Zope local site. The site is restored after the
+  event.
+
+1.6.1 (2012-05-02)
+------------------
+
+- Exposed ApplicationInitializedEvent and IApplicationInitializedEvent.
+
+- Added the missing import for the exposed IApplication interface.
+
+1.6 (2012-05-01)
+----------------
+
+- Moved the directive `site` from Grok to this package.
+
+- Moved the component `Application` and all the related utilities from Grok
+  to this package.
+
+1.5 (2011-01-03)
+----------------
+
+- Moved IApplication and getApplication from the Grok package into
+  this one.
+
+1.4 (2010-11-01)
+----------------
+
+- Upped versions requirements for martian and grokcore.component.
+
+1.3 (2010-10-18)
+----------------
+
+- Made package comply to repository policy.
+
+- Update functional tests to only use zope.app.appsetup instead
+  of zope.app.testing.
+
+- Update functional tests not to require zope.app.zcmlfiles
+  anymore.
+
+1.2 (2009-12-20)
+----------------
+
+* Migrated imports from zope.app.component to zope.site.
+
+1.1 (2009-09-18)
+----------------
+
+* Updated dependencies (added missing ones and added separate test
+  dependencies).
+
+* A local utility now implements IAttributeAnnotatable.
+
+* Update code documentation from Grok itself.
+
+* Use 1.0b2 versions.cfg in Grok's release info instead of a local
+  copy; a local copy for all grokcore packages is just too hard to
+  maintain.
+
+
+1.0.1 (2009-06-30)
+------------------
+
+* Reupload to pypi with a correct version of Python which doesn't have
+  a distutils bug.
+
+1.0 (2009-06-29)
+----------------
+
+* Created ``grokcore.site`` by factoring local site based components,
+  grokkers and directives out of Grok.
```

### Comparing `grokcore.site-3.1/src/grokcore.site.egg-info/SOURCES.txt` & `grokcore.site-4.0/src/grokcore.site.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
+MANIFEST.in
 README.rst
-buildout.cfg
-requirements.txt
 setup.cfg
 setup.py
 tox.ini
 src/grokcore/__init__.py
 src/grokcore.site.egg-info/PKG-INFO
 src/grokcore.site.egg-info/SOURCES.txt
 src/grokcore.site.egg-info/dependency_links.txt
```

