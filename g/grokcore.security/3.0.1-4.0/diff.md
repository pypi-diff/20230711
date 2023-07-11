# Comparing `tmp/grokcore.security-3.0.1.tar.gz` & `tmp/grokcore.security-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grokcore.security-3.0.1.tar", last modified: Fri Jan 12 13:16:24 2018, max compression
+gzip compressed data, was "grokcore.security-4.0.tar", last modified: Tue Jul 11 06:24:43 2023, max compression
```

## Comparing `grokcore.security-3.0.1.tar` & `grokcore.security-4.0.tar`

### file list

```diff
@@ -1,67 +1,65 @@
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/
--rw-r--r--   0 jw         (501) staff       (20)      357 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/.travis.yml
--rw-r--r--   0 jw         (501) staff       (20)     6158 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/bootstrap.py
--rw-r--r--   0 jw         (501) staff       (20)      470 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/buildout.cfg
--rw-r--r--   0 jw         (501) staff       (20)     2660 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/CHANGES.txt
--rw-r--r--   0 jw         (501) staff       (20)       32 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/COPYRIGHT.txt
--rw-r--r--   0 jw         (501) staff       (20)      145 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/CREDITS.txt
--rw-r--r--   0 jw         (501) staff       (20)     2070 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/LICENSE.txt
--rw-r--r--   0 jw         (501) staff       (20)      124 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/MANIFEST.in
--rw-r--r--   0 jw         (501) staff       (20)    10236 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/PKG-INFO
--rw-r--r--   0 jw         (501) staff       (20)     4777 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/README.txt
--rw-r--r--   0 jw         (501) staff       (20)      124 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/requirements.txt
--rw-r--r--   0 jw         (501) staff       (20)       38 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/setup.cfg
--rw-r--r--   0 jw         (501) staff       (20)     2033 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/setup.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/
--rw-r--r--   0 jw         (501) staff       (20)      200 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/
--rw-r--r--   0 jw         (501) staff       (20)     1228 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     1418 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/components.py
--rw-r--r--   0 jw         (501) staff       (20)     3952 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/directive.py
--rw-r--r--   0 jw         (501) staff       (20)      467 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/ftesting.zcml
--rw-r--r--   0 jw         (501) staff       (20)     1649 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/interfaces.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/meta/
--rw-r--r--   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/meta/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     1972 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/meta/permission.py
--rw-r--r--   0 jw         (501) staff       (20)     3260 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/meta/role.py
--rw-r--r--   0 jw         (501) staff       (20)      210 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/meta.zcml
--rw-r--r--   0 jw         (501) staff       (20)     1716 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/testing.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/
--rw-r--r--   0 jw         (501) staff       (20)     1228 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/
--rw-r--r--   0 jw         (501) staff       (20)       32 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/permissions/
--rw-r--r--   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/permissions/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)      437 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/permissions/directive.py
--rw-r--r--   0 jw         (501) staff       (20)      220 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/permissions/directive_fixture.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/role/
--rw-r--r--   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/role/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)      376 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/role/missing_role_name.py
--rw-r--r--   0 jw         (501) staff       (20)      928 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/role/permissions.py
--rw-r--r--   0 jw         (501) staff       (20)     2097 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/role/role_i18n.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/security/
--rw-r--r--   0 jw         (501) staff       (20)       32 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/security/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)      477 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/security/fallback.py
--rw-r--r--   0 jw         (501) staff       (20)      554 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/security/missing_permission.py
--rw-r--r--   0 jw         (501) staff       (20)      385 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/security/missing_permission_name.py
--rw-r--r--   0 jw         (501) staff       (20)      573 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/security/multiple_require.py
--rw-r--r--   0 jw         (501) staff       (20)      607 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/security/not_a_permissionclass.py
--rw-r--r--   0 jw         (501) staff       (20)      949 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/security/permission.py
--rw-r--r--   0 jw         (501) staff       (20)      586 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/base/security/protect_getattr.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/functional/
--rw-r--r--   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/functional/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/functional/role/
--rw-r--r--   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/functional/role/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     3014 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/functional/role/roles.py
--rw-r--r--   0 jw         (501) staff       (20)     1627 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/test_base.py
--rw-r--r--   0 jw         (501) staff       (20)     1755 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/tests/test_functional.py
--rw-r--r--   0 jw         (501) staff       (20)     2198 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore/security/util.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore.security.egg-info/
--rw-r--r--   0 jw         (501) staff       (20)        1 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore.security.egg-info/dependency_links.txt
--rw-r--r--   0 jw         (501) staff       (20)        9 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore.security.egg-info/namespace_packages.txt
--rw-r--r--   0 jw         (501) staff       (20)        1 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore.security.egg-info/not-zip-safe
--rw-r--r--   0 jw         (501) staff       (20)    10236 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore.security.egg-info/PKG-INFO
--rw-r--r--   0 jw         (501) staff       (20)      240 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore.security.egg-info/requires.txt
--rw-r--r--   0 jw         (501) staff       (20)     2084 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore.security.egg-info/SOURCES.txt
--rw-r--r--   0 jw         (501) staff       (20)        9 2018-01-12 13:16:24.000000 grokcore.security-3.0.1/src/grokcore.security.egg-info/top_level.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.413803 grokcore.security-4.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2796 2023-07-11 06:24:43.000000 grokcore.security-4.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-11 06:24:43.000000 grokcore.security-4.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-11 06:24:43.000000 grokcore.security-4.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      145 2023-07-11 06:24:43.000000 grokcore.security-4.0/CREDITS.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-11 06:24:43.000000 grokcore.security-4.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2023-07-11 06:24:43.000000 grokcore.security-4.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8549 2023-07-11 06:24:43.413870 grokcore.security-4.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4777 2023-07-11 06:24:43.000000 grokcore.security-4.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      484 2023-07-11 06:24:43.414196 grokcore.security-4.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1956 2023-07-11 06:24:43.000000 grokcore.security-4.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.404689 grokcore.security-4.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.407769 grokcore.security-4.0/src/grokcore/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.410190 grokcore.security-4.0/src/grokcore/security/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1307 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1420 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/components.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4003 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/directive.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      467 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/ftesting.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1676 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/interfaces.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.410582 grokcore.security-4.0/src/grokcore/security/meta/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/meta/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1859 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/meta/permission.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3223 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/meta/role.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      210 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1715 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/testing.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.411018 grokcore.security-4.0/src/grokcore/security/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      641 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.411149 grokcore.security-4.0/src/grokcore/security/tests/base/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.411578 grokcore.security-4.0/src/grokcore/security/tests/base/permissions/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/permissions/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      437 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/permissions/directive.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      207 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/permissions/directive_fixture.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.412140 grokcore.security-4.0/src/grokcore/security/tests/base/role/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/role/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      355 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/role/missing_role_name.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      938 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/role/permissions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2112 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/role/role_i18n.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.413284 grokcore.security-4.0/src/grokcore/security/tests/base/security/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/security/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      478 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/security/fallback.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      567 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/security/missing_permission.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      386 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/security/missing_permission_name.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      604 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/security/multiple_require.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      607 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/security/not_a_permissionclass.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      950 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/security/permission.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      588 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/base/security/protect_getattr.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.413426 grokcore.security-4.0/src/grokcore/security/tests/functional/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/functional/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.413663 grokcore.security-4.0/src/grokcore/security/tests/functional/role/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/functional/role/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2993 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/functional/role/roles.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1080 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/test_base.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1394 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/tests/test_functional.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2205 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore/security/util.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-11 06:24:43.408993 grokcore.security-4.0/src/grokcore.security.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8549 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore.security.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2063 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore.security.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore.security.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore.security.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore.security.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      244 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore.security.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-11 06:24:43.000000 grokcore.security-4.0/src/grokcore.security.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1396 2023-07-11 06:24:43.000000 grokcore.security-4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grokcore.security-3.0.1/CHANGES.txt` & `grokcore.security-4.0/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 =======
 
+4.0 (2023-07-11)
+----------------
+
+- Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
+
+- Drop support for Python 2.7, 3.4, 3.5, 3.6.
+
+
 3.0.1 (2018-01-12)
 ------------------
 
 - Rearrange tests such that Travis CI can pick up all functional tests too.
 
 3.0.0 (2018-01-05)
 ------------------
```

### Comparing `grokcore.security-3.0.1/LICENSE.txt` & `grokcore.security-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grokcore.security-3.0.1/PKG-INFO` & `grokcore.security-4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,255 +1,265 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: grokcore.security
-Version: 3.0.1
+Version: 4.0
 Summary: Grok-like configuration for Zope security components
-Home-page: http://grok.zope.org
+Home-page: https://github.com/zopefoundation/grokcore.security
 Author: Grok Team
-Author-email: grok-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL
-Download-URL: http://pypi.python.org/pypi/grokcore.security
-Description: This package provides basic elements for defining Zope permissions and
-        security checkers without ZCML.
-        
-        .. contents::
-        
-        Setting up ``grokcore.security``
-        ================================
-        
-        This package is essentially set up like the `grokcore.component`_
-        package, please refer to its documentation for details.  The
-        additional ZCML lines you will need are::
-        
-          <include package="grokcore.security" file="meta.zcml" />
-          <include package="grokcore.security" />
-        
-        Put this somewhere near the top of your root ZCML file but below the
-        line where you include ``grokcore.component``'s configuration.
-        
-        
-        Defining permissions
-        ====================
-        
-        In `grokcore.component`_, various components are defined (and
-        automatically registered) by subclassing from certain baseclasses.
-        The same applies to defining permissions with ``grokcore.security`` as
-        well::
-        
-          import grokcore.security
-        
-          class EditContent(grokcore.security.Permission):
-              grokcore.security.name('mypkg.EditContent')
-        
-        This defines a permission with the ID ``mypkg.EditContent``.  You must
-        always specify this ID explicitly.  In addition, you can also give the
-        permission a human-readable title and description.  This is useful
-        when your application provides lists of permissions somewhere and you
-        don't want to bother users with deciphering the dotted IDs::
-        
-          import grokcore.security
-        
-          class EditContent(grokcore.security.Permission):
-              grokcore.security.name('mypkg.EditContent')
-              grokcore.security.title('Edit content')
-              grokcore.security.description('Anyone who has this permission may '
-                                            'modify content in the application.')
-        
-        
-        Defining checkers for components
-        ================================
-        
-        ``grokcore.security`` provides some means for defining checkers for
-        components:
-        
-        * ``grokcore.security.require(permission)`` which can be used either
-          as a class-level directive to set a permission for a whole
-          component, or as a decorator to set a permission for a function or
-          method.
-        
-        * ``protect_getattr`` and ``protect_setattr``, available from
-          ``grokcore.security.util``, which take a class, an attribute name
-          and a permission as arguments and define Zope security checkers for
-          getting or setting a particular attribute on instance of said class.
-        
-        With these, you can build grokkers for components that need security
-        declarations.  For instance, the `grokcore.view`_ package uses them to
-        define a grokker that makes security declarations for views::
-        
-          class ViewSecurityGrokker(martian.ClassGrokker):
-              martian.component(grokcore.view.View)
-              martian.directive(grokcore.security.require, name='permission')
-        
-              def execute(self, factory, config, permission, **kw):
-                  for method_name in zope.publisher.interfaces.browser.IBrowserPage:
-                      config.action(
-                          discriminator=('protectName', factory, method_name),
-                          callable=grokcore.security.util.protect_getattr,
-                          args=(factory, method_name, permission),
-                          )
-                  return True
-        
-        With such a grokker, it is possible to protect views like so::
-        
-          class Edit(grokcore.view.View):
-              grokcore.security.require(EditContent)
-        
-        Note how we can simply pass a permission class to the ``require``
-        directive.  Alternatively, you can pass the permission ID::
-        
-          class Edit(grokcore.view.View):
-              grokcore.security.require('mypkg.EditContent')
-        
-        If you wanted to be able to define permissions for individual class
-        methods rather than the whole class, you would simply base your
-        grokker on ``martian.MethodGrokker`` rather than ``ClassGrokker``.
-        The actual mechanics of defining a checker are the same.
-        
-        Please note that ``grokcore.security`` does not yet provide directives
-        that allow you to specify permissions for simple attribute access
-        (read and write).
-        
-        
-        API overview
-        ============
-        
-        ``Permission``
-            Base class for defining permissions.  Use the ``name`` directive
-            to define the mandatory permission ID.  Optionally use the
-            ``title`` and ``description`` directives to give the permission
-            human-readable information.
-        
-        ``Public``
-            Special permission that can be referred to whenever a component
-            should not be protected by a permission at all (public access).
-        
-        ``require(permission_class_or_id)``
-            declares that the use of a particular component (when used as a
-            class-level directive) or a method (when used as a method
-            decorator) requires a certain permission.  The argument can either
-            be a permission class (subclass of ``Permission``) or a permission
-            ID.
-        
-        In addition, the ``grokcore.security`` package exposes the
-        `grokcore.component`_ API.
-        
-        
-        .. _grokcore.component: http://pypi.python.org/pypi/grokcore.component
-        .. _grokcore.view: http://pypi.python.org/pypi/grokcore.view
-        
-        Changes
-        =======
-        
-        3.0.1 (2018-01-12)
-        ------------------
-        
-        - Rearrange tests such that Travis CI can pick up all functional tests too.
-        
-        3.0.0 (2018-01-05)
-        ------------------
-        
-        - Fix several test error that came to light.
-        
-        1.7 (2018-01-03)
-        ----------------
-        
-        - Python 3 compatibility.
-        
-        1.6.3 (2016-01-29)
-        ------------------
-        
-        - Update tests.
-        
-        1.6.2 (2012-05-07)
-        ------------------
-        
-        - Properly declare zope.dottedname as a dependency.
-        
-        1.6.1 (2012-05-02)
-        ------------------
-        
-        - Fix the package to properly work if the extra ``role`` is not
-          specified.
-        
-        1.6 (2012-05-01)
-        ----------------
-        
-        - The Permission and Role components moved from the grok package to the
-          grokcore.security package where it belongs.
-        
-        - The permissions() directive moved from the grok package to
-          grokcore.security where it belongs.
-        
-        1.5 (2010-11-01)
-        ----------------
-        
-        - Upped the requirements for martian and grokcore.component.
-        
-        - Made package comply to zope.org repository policy.
-        
-        1.4 (2009-12-13)
-        ----------------
-        
-        * **note** Backed out the version requirements for
-          grokcore.component-2.0 and martian-0.12. These requirements
-          stood in the way of further development especially towards
-          grok-1.1 based on the ZTK. The 1.3 version should probably
-          have been called 2.0 like with grokcore.component.
-        
-        * Ported setup.py dependency fixes from trunk.
-        
-        * Use zope.security instead of zope.app.security.
-        
-        1.3 (2009-09-16)
-        ----------------
-        
-        * Use the grok.zope.org/releaseinfo information instead of our own
-          copy of ``versions.cfg``, for easier maintenance.
-        
-        * Depend on grokcore.component 2.0 and the 0.12 Martian - this changes
-          inheritance issues but doesn't appear to affect grokcore.security
-          itself.
-        
-        1.2 (2009-09-14)
-        ----------------
-        
-        * Changed the default permissions from grok.View to zope.View. There seems no
-          particular reason not to use the standard zope.View permission defined
-          in zope.app.security.
-        
-          NOTE: YOU MUST STILL ASSIGN THIS PERMISSION TO USERS IN YOUR
-          site.zcml FILE. OTHERWISE YOU DO NOT HAVE ACCESS TO ANY VIEWS.
-        
-        * Made sure to include zope.app.security configuration as well, as that
-          package defines the zope.View permission. Note that in the future this will
-          change to zope.security.
-        
-        * Bring versions.cfg in line with grok 1.0 release candidate
-          versions.cfg.
-        
-        
-        1.1 (2009-07-03)
-        ----------------
-        
-        * Changed the default permissions from zope.Public to grok.View.
-        
-          NOTE: YOU MUST ASSIGN THIS PERMISSION TO USERS IN YOUR
-          site.zcml FILE. OTHERWISE YOU DO NOT HAVE ACCESS TO ANY VIEWS.
-        
-        1.0 (2008-08-03)
-        ----------------
-        
-        * Created ``grokcore.security`` in July 2008 by factoring
-          security-related components, grokkers and directives out of Grok.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Provides-Extra: role
+Provides-Extra: test
+License-File: LICENSE.txt
+
+This package provides basic elements for defining Zope permissions and
+security checkers without ZCML.
+
+.. contents::
+
+Setting up ``grokcore.security``
+================================
+
+This package is essentially set up like the `grokcore.component`_
+package, please refer to its documentation for details.  The
+additional ZCML lines you will need are::
+
+  <include package="grokcore.security" file="meta.zcml" />
+  <include package="grokcore.security" />
+
+Put this somewhere near the top of your root ZCML file but below the
+line where you include ``grokcore.component``'s configuration.
+
+
+Defining permissions
+====================
+
+In `grokcore.component`_, various components are defined (and
+automatically registered) by subclassing from certain baseclasses.
+The same applies to defining permissions with ``grokcore.security`` as
+well::
+
+  import grokcore.security
+
+  class EditContent(grokcore.security.Permission):
+      grokcore.security.name('mypkg.EditContent')
+
+This defines a permission with the ID ``mypkg.EditContent``.  You must
+always specify this ID explicitly.  In addition, you can also give the
+permission a human-readable title and description.  This is useful
+when your application provides lists of permissions somewhere and you
+don't want to bother users with deciphering the dotted IDs::
+
+  import grokcore.security
+
+  class EditContent(grokcore.security.Permission):
+      grokcore.security.name('mypkg.EditContent')
+      grokcore.security.title('Edit content')
+      grokcore.security.description('Anyone who has this permission may '
+                                    'modify content in the application.')
+
+
+Defining checkers for components
+================================
+
+``grokcore.security`` provides some means for defining checkers for
+components:
+
+* ``grokcore.security.require(permission)`` which can be used either
+  as a class-level directive to set a permission for a whole
+  component, or as a decorator to set a permission for a function or
+  method.
+
+* ``protect_getattr`` and ``protect_setattr``, available from
+  ``grokcore.security.util``, which take a class, an attribute name
+  and a permission as arguments and define Zope security checkers for
+  getting or setting a particular attribute on instance of said class.
+
+With these, you can build grokkers for components that need security
+declarations.  For instance, the `grokcore.view`_ package uses them to
+define a grokker that makes security declarations for views::
+
+  class ViewSecurityGrokker(martian.ClassGrokker):
+      martian.component(grokcore.view.View)
+      martian.directive(grokcore.security.require, name='permission')
+
+      def execute(self, factory, config, permission, **kw):
+          for method_name in zope.publisher.interfaces.browser.IBrowserPage:
+              config.action(
+                  discriminator=('protectName', factory, method_name),
+                  callable=grokcore.security.util.protect_getattr,
+                  args=(factory, method_name, permission),
+                  )
+          return True
+
+With such a grokker, it is possible to protect views like so::
+
+  class Edit(grokcore.view.View):
+      grokcore.security.require(EditContent)
+
+Note how we can simply pass a permission class to the ``require``
+directive.  Alternatively, you can pass the permission ID::
+
+  class Edit(grokcore.view.View):
+      grokcore.security.require('mypkg.EditContent')
+
+If you wanted to be able to define permissions for individual class
+methods rather than the whole class, you would simply base your
+grokker on ``martian.MethodGrokker`` rather than ``ClassGrokker``.
+The actual mechanics of defining a checker are the same.
+
+Please note that ``grokcore.security`` does not yet provide directives
+that allow you to specify permissions for simple attribute access
+(read and write).
+
+
+API overview
+============
+
+``Permission``
+    Base class for defining permissions.  Use the ``name`` directive
+    to define the mandatory permission ID.  Optionally use the
+    ``title`` and ``description`` directives to give the permission
+    human-readable information.
+
+``Public``
+    Special permission that can be referred to whenever a component
+    should not be protected by a permission at all (public access).
+
+``require(permission_class_or_id)``
+    declares that the use of a particular component (when used as a
+    class-level directive) or a method (when used as a method
+    decorator) requires a certain permission.  The argument can either
+    be a permission class (subclass of ``Permission``) or a permission
+    ID.
+
+In addition, the ``grokcore.security`` package exposes the
+`grokcore.component`_ API.
+
+
+.. _grokcore.component: http://pypi.python.org/pypi/grokcore.component
+.. _grokcore.view: http://pypi.python.org/pypi/grokcore.view
+
+Changes
+=======
+
+4.0 (2023-07-11)
+----------------
+
+- Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
+
+- Drop support for Python 2.7, 3.4, 3.5, 3.6.
+
+
+3.0.1 (2018-01-12)
+------------------
+
+- Rearrange tests such that Travis CI can pick up all functional tests too.
+
+3.0.0 (2018-01-05)
+------------------
+
+- Fix several test error that came to light.
+
+1.7 (2018-01-03)
+----------------
+
+- Python 3 compatibility.
+
+1.6.3 (2016-01-29)
+------------------
+
+- Update tests.
+
+1.6.2 (2012-05-07)
+------------------
+
+- Properly declare zope.dottedname as a dependency.
+
+1.6.1 (2012-05-02)
+------------------
+
+- Fix the package to properly work if the extra ``role`` is not
+  specified.
+
+1.6 (2012-05-01)
+----------------
+
+- The Permission and Role components moved from the grok package to the
+  grokcore.security package where it belongs.
+
+- The permissions() directive moved from the grok package to
+  grokcore.security where it belongs.
+
+1.5 (2010-11-01)
+----------------
+
+- Upped the requirements for martian and grokcore.component.
+
+- Made package comply to zope.org repository policy.
+
+1.4 (2009-12-13)
+----------------
+
+* **note** Backed out the version requirements for
+  grokcore.component-2.0 and martian-0.12. These requirements
+  stood in the way of further development especially towards
+  grok-1.1 based on the ZTK. The 1.3 version should probably
+  have been called 2.0 like with grokcore.component.
+
+* Ported setup.py dependency fixes from trunk.
+
+* Use zope.security instead of zope.app.security.
+
+1.3 (2009-09-16)
+----------------
+
+* Use the grok.zope.org/releaseinfo information instead of our own
+  copy of ``versions.cfg``, for easier maintenance.
+
+* Depend on grokcore.component 2.0 and the 0.12 Martian - this changes
+  inheritance issues but doesn't appear to affect grokcore.security
+  itself.
+
+1.2 (2009-09-14)
+----------------
+
+* Changed the default permissions from grok.View to zope.View. There seems no
+  particular reason not to use the standard zope.View permission defined
+  in zope.app.security.
+
+  NOTE: YOU MUST STILL ASSIGN THIS PERMISSION TO USERS IN YOUR
+  site.zcml FILE. OTHERWISE YOU DO NOT HAVE ACCESS TO ANY VIEWS.
+
+* Made sure to include zope.app.security configuration as well, as that
+  package defines the zope.View permission. Note that in the future this will
+  change to zope.security.
+
+* Bring versions.cfg in line with grok 1.0 release candidate
+  versions.cfg.
+
+
+1.1 (2009-07-03)
+----------------
+
+* Changed the default permissions from zope.Public to grok.View.
+
+  NOTE: YOU MUST ASSIGN THIS PERMISSION TO USERS IN YOUR
+  site.zcml FILE. OTHERWISE YOU DO NOT HAVE ACCESS TO ANY VIEWS.
+
+1.0 (2008-08-03)
+----------------
+
+* Created ``grokcore.security`` in July 2008 by factoring
+  security-related components, grokkers and directives out of Grok.
```

### Comparing `grokcore.security-3.0.1/README.txt` & `grokcore.security-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `grokcore.security-3.0.1/setup.py` & `grokcore.security-4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,71 @@
-from setuptools import setup, find_packages
 import os
 
+from setuptools import find_packages
+from setuptools import setup
+
+
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
+
 long_description = (
-    read('README.txt')
+    read('README.rst')
     + '\n' +
-    read('CHANGES.txt')
-    )
+    read('CHANGES.rst')
+)
 
 tests_require = [
-    'grok',
     'grokcore.view[test]',
     'zope.app.wsgi',
     'zope.configuration',
     'zope.securitypolicy',
     'zope.testing',
-    ]
+]
 
 setup(
     name='grokcore.security',
-    version='3.0.1',
+    version='4.0',
     author='Grok Team',
-    author_email='grok-dev@zope.org',
-    url='http://grok.zope.org',
-    download_url='http://pypi.python.org/pypi/grokcore.security',
+    author_email='zope-dev@zope.dev',
+    url='https://github.com/zopefoundation/grokcore.security',
     description='Grok-like configuration for Zope security components',
     long_description=long_description,
     license='ZPL',
-    classifiers=['Intended Audience :: Developers',
-                 'Development Status :: 6 - Mature',
-                 'License :: OSI Approved :: Zope Public License',
-                 'Operating System :: OS Independent',
-                 'Programming Language :: Python :: 2',
-                 'Programming Language :: Python :: 2.7',
-                 'Programming Language :: Python :: 3',
-                 'Programming Language :: Python :: 3.4',
-                 'Programming Language :: Python :: 3.5',
-                 'Programming Language :: Python :: 3.6',
-                 'Programming Language :: Python :: Implementation :: CPython',
-                 'Programming Language :: Python :: Implementation :: PyPy',
+    classifiers=[
+        'Intended Audience :: Developers',
+        'Development Status :: 6 - Mature',
+        'License :: OSI Approved :: Zope Public License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy',
                  ],
     packages=find_packages('src'),
-    package_dir = {'': 'src'},
+    package_dir={'': 'src'},
     namespace_packages=['grokcore'],
     include_package_data=True,
     zip_safe=False,
+    python_requires='>=3.7',
     install_requires=[
+        'Chameleon >= 2',
         'grokcore.component >= 2.1',
         'martian >= 0.13',
         'setuptools',
         'zope.component',
         'zope.dottedname',
         'zope.interface',
         'zope.security',
-        ],
+    ],
     tests_require=tests_require,
     extras_require={
         'role': [
             'zope.securitypolicy',
-            ],
+        ],
         'test': tests_require
-        },
+    },
 )
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/__init__.py` & `grokcore.security-4.0/src/grokcore/security/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grok
 """
 from grokcore.component import *
 
-from grokcore.security.components import Permission
-from grokcore.security.components import Public
-from grokcore.security.directive import require, permissions
-
 # Import this module so that it's available as soon as you import the
 # 'grokcore.security' package.  Useful for tests and interpreter examples.
 import grokcore.security.testing
-
+from grokcore.security.components import Permission
+from grokcore.security.components import Public
+from grokcore.security.directive import permissions
+from grokcore.security.directive import require
 # Only export public API
-from grokcore.security.interfaces import IGrokcoreSecurityAPI, HAVE_ROLE
+from grokcore.security.interfaces import HAVE_ROLE
+from grokcore.security.interfaces import IGrokcoreSecurityAPI
+
+
 if HAVE_ROLE:
     from grokcore.security.components import Role
 
 __all__ = list(IGrokcoreSecurityAPI)
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/components.py` & `grokcore.security-4.0/src/grokcore/security/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grok components"""
 
 from zope.security.permission import Permission
+
 from grokcore.security.interfaces import HAVE_ROLE
 
 
 class Permission(Permission):
     pass
 
+
 Public = 'zope.Public'
 
 
 if HAVE_ROLE:
     from zope.securitypolicy.role import Role as securitypolicy_Role
 
     class Role(securitypolicy_Role):
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/directive.py` & `grokcore.security-4.0/src/grokcore/security/directive.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,25 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grok directives.
 """
 import sys
-import martian
+
 import grokcore.component
+import martian
 from martian import util
-from martian.error import GrokImportError, GrokError
 from martian.directive import StoreMultipleTimes
+from martian.error import GrokError
+from martian.error import GrokImportError
+
 from grokcore.security import components
 
+
 class RequireDirectiveStore(StoreMultipleTimes):
 
     def get(self, directive, component, default):
         permissions = getattr(component, directive.dotted_name(), default)
         if (permissions is default) or not permissions:
             return default
         if len(permissions) > 1:
@@ -33,14 +37,15 @@
                 '%r. It may only be set once for a class.'
                 % component, component)
         return permissions[0]
 
     def pop(self, locals_, directive):
         return locals_[directive.dotted_name()].pop()
 
+
 class require(martian.Directive):
     scope = martian.CLASS
     store = RequireDirectiveStore()
 
     def validate(self, value):
         if util.check_subclass(value, components.Permission):
             return
@@ -60,14 +65,15 @@
         # here, which may be used for methods, or simply ignored when
         # used as a directive.
         frame = sys._getframe(1)
         permission = self.store.pop(frame.f_locals, self)
         self.set(func, [permission])
         return func
 
+
 class permissions(martian.Directive):
     """The `grokcore.security.permissions()` directive.
 
     This directive is used inside of a `grok.Role` subclass to list the
     permissions which each member of the role should always possess.
     Note that permissions should be passed as strings, and that several
     permissions they can simply be supplied as multiple arguments; there
@@ -92,11 +98,12 @@
                     "subclasses of grok.Permission to the '%s' directive."
                     % self.name)
 
     def factory(self, *values):
         permission_ids = []
         for value in values:
             if martian.util.check_subclass(value, components.Permission):
-                permission_ids.append(grokcore.component.name.bind().get(value))
+                permission_ids.append(
+                    grokcore.component.name.bind().get(value))
             else:
                 permission_ids.append(value)
         return permission_ids
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/interfaces.py` & `grokcore.security-4.0/src/grokcore/security/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grok interfaces
 """
-from zope.interface import Interface, Attribute
 from zope.dottedname.resolve import resolve
+from zope.interface import Attribute
+from zope.interface import Interface
+
 
 def api(name):
     try:
         return True, resolve(name)
     except ImportError:
         return False, Interface
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/meta/permission.py` & `grokcore.security-4.0/src/grokcore/security/meta/permission.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,20 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grokkers for security-related components."""
 
-import sys
-import martian
 import grokcore.component
-import grokcore.security
-
-from zope.security.interfaces import IPermission
+import martian
 from martian.error import GrokError
+from zope.security.interfaces import IPermission
 
-
-PY2 = sys.version_info[0] == 2
-
-
-if not PY2:
-    unicode = lambda s: s
+import grokcore.security
 
 
 def default_fallback_to_name(factory, module, name, **data):
     return name
 
 
 class PermissionGrokker(martian.ClassGrokker):
@@ -42,17 +34,16 @@
     martian.directive(grokcore.component.description)
 
     def execute(self, factory, config, name, title, description, **kw):
         if not name:
             raise GrokError(
                 "A permission needs to have a dotted name for its id. Use "
                 "grok.name to specify one.", factory)
-        permission = factory(
-            unicode(name), unicode(title), unicode(description))
+        permission = factory(str(name), str(title), str(description))
 
         config.action(
             discriminator=('utility', IPermission, name),
             callable=grokcore.component.provideUtility,
             args=(permission, IPermission, name),
             order=-1  # need to do this early in the process
-            )
+        )
         return True
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/meta/role.py` & `grokcore.security-4.0/src/grokcore/security/meta/role.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,31 +12,29 @@
 #
 ##############################################################################
 """Grokkers for security-related components."""
 
 
 from grokcore.security.interfaces import HAVE_ROLE
 
-if HAVE_ROLE:
-    import martian
 
+if HAVE_ROLE:
     import grokcore.component
-    import grokcore.security
-
+    import martian
     from martian.error import GrokError
     from zope.i18nmessageid import Message
-    from zope.securitypolicy.rolepermission import rolePermissionManager
     from zope.securitypolicy.interfaces import IRole
+    from zope.securitypolicy.rolepermission import rolePermissionManager
 
+    import grokcore.security
     from grokcore.security.components import Role
     from grokcore.security.directive import permissions
     from grokcore.security.meta.permission import PermissionGrokker
     from grokcore.security.meta.permission import default_fallback_to_name
 
-
     class RoleGrokker(martian.ClassGrokker):
         """Grokker for components subclassed from `grok.Role`.
 
         Each role is registered as a global utility providing the service
         `IRole` under its own particular name, and then granted every
         permission named in its `grok.permission()` directive.
 
@@ -54,25 +52,25 @@
             if not name:
                 raise GrokError(
                     "A role needs to have a dotted name for its id. Use "
                     "grok.name to specify one.", factory)
             # We can safely convert to unicode, since the directives makes sure
             # it is either unicode already or ASCII.
             if not isinstance(title, Message):
-                title = u'{}'.format(str(title))  # python2 and 3
+                title = f'{str(title)}'  # python2 and 3
             if not isinstance(description, Message):
-                description = u'{}'.format(str(description))  # python2 and 3
-            role = factory(u'{}'.format(str(name)), title, description)
+                description = f'{str(description)}'  # python2 and 3
+            role = factory(f'{str(name)}', title, description)
 
             config.action(
                 discriminator=('utility', IRole, name),
                 callable=grokcore.component.provideUtility,
                 args=(role, IRole, name),
-                )
+            )
 
             for permission in permissions:
                 config.action(
                     discriminator=('grantPermissionToRole', permission, name),
                     callable=rolePermissionManager.grantPermissionToRole,
                     args=(permission, name),
-                    )
+                )
             return True
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/testing.py` & `grokcore.security-4.0/src/grokcore/security/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,35 +9,38 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grok test helpers
 """
-import martian
 import grokcore.component
-from zope.configuration.config import ConfigurationMachine
+import martian
 from grokcore.component import zcml
+from zope.configuration.config import ConfigurationMachine
+
 from grokcore.security import directive
 from grokcore.security import util
 
+
 class ClasslevelGrokker(martian.ClassGrokker):
     """Simple grokker that looks for grokk.require() directives on a
     class and checks whether the permissione exists."""
     martian.component(grokcore.component.Context)
     martian.directive(directive.require, name='permission')
 
     def execute(self, factory, config, permission, **kw):
         config.action(
             discriminator=('protectName', factory, 'protected'),
             callable=util.protect_getattr,
             args=(factory, 'protected', permission),
-            )
+        )
         return True
 
+
 def grok(module_name):
     config = ConfigurationMachine()
     zcml.do_grok('grokcore.component.meta', config)
     zcml.do_grok('grokcore.security.meta', config)
     zcml.do_grok('grokcore.security.testing', config)
     zcml.do_grok(module_name, config)
     config.execute_actions()
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/tests/base/role/permissions.py` & `grokcore.security-4.0/src/grokcore/security/tests/base/role/permissions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 """
 A Role component optionally defines what permission it comprises.
 
 The grok.permissions() directive is used to specify the set of permissions
 that are aggregated in the particular Role. The permissions can be referenced
 by "name" or by class.
 
+  >>> import grokcore.security.testing
   >>> grokcore.security.testing.grok(__name__)
 """
 
 import grokcore.component as grok
-import grokcore.security.testing
+
+from grokcore.security import Permission
 from grokcore.security import Role
-from grokcore.security import Permission, permissions
-import zope.interface
+from grokcore.security import permissions
+
 
 class FirstPermission(Permission):
     grok.name('first permission')
 
+
 class SecondPermission(Permission):
     grok.name('second permission')
 
+
 class RoleComprisingTwoPermissionsByName(Role):
     grok.name('ByName')
     permissions(
         'first permission',
         'second permission'
-        )
+    )
+
 
 class RoleComprisingTwoPermissionsByClass(Role):
     grok.name('ByClass')
     permissions(
         FirstPermission,
         SecondPermission
-        )
+    )
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/tests/base/role/role_i18n.py` & `grokcore.security-4.0/src/grokcore/security/tests/base/role/role_i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 A Role component have a title and description, that can be internationalized.
 
 Let's grok this package and check we still have a Message object for the
 internationalized title and description of the defined roles.
 
+  >>> import grokcore.security.testing
   >>> grokcore.security.testing.grok(__name__)
   >>> from zope.securitypolicy.interfaces import IRole
   >>> from zope.component import getUtility
   >>> from zope.i18nmessageid import Message
 
 A grok.Role without any internationalization. The id, title and description
 should be unicode::
@@ -50,18 +51,18 @@
   >>> isinstance(role.title, Message)
   True
   >>> isinstance(role.description, Message)
   True
 """
 
 import grokcore.component as grok
-import grokcore.security
+from zope.i18nmessageid import MessageFactory
 
 from grokcore.security import Role
-from zope.i18nmessageid import MessageFactory
+
 
 _ = MessageFactory("testi18n")
 
 
 class RoleWithoutI18n(Role):
     grok.name('RoleWithoutI18n')
     grok.description('My role without i18n')
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/tests/base/security/missing_permission.py` & `grokcore.security-4.0/src/grokcore/security/tests/base/security/missing_permission.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 A permission has to be defined first (using grok.Permission for example)
 before it can be used in grok.require().
 
-  >>> grok.testing.grok(__name__)
-  Traceback (most recent call last):
-  ...
-  zope.configuration.config.ConfigurationExecutionError: \
-  martian.error.GrokError: Undefined permission 'doesnt.exist' in <class \
-  'grokcore.security.tests.base.security.missing_permission.MissingPermission'>. \
-  Use grok.Permission first...
-"""
+>>> grok.testing.grok(__name__)
+Traceback (most recent call last):
+...
+zope.configuration.config.ConfigurationExecutionError: \
+martian.error.GrokError: Undefined permission 'doesnt.exist' in <class \
+'grokcore.security.tests.base.security.missing_permission.MissingPermission'>. \
+Use grok.Permission first.
+"""  # noqa: E501 line too long
 import grokcore.security as grok
 
+
 class MissingPermission(grok.Context):
     grok.require('doesnt.exist')
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/tests/base/security/multiple_require.py` & `grokcore.security-4.0/src/grokcore/security/tests/base/security/multiple_require.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,22 @@
   >>> grok.testing.grok(__name__)
   Traceback (most recent call last):
     ...
   martian.error.GrokError: grok.require was called multiple times in \
   <class 'grokcore.security.tests.base.security.multiple_require.MultipleView'>. \
   It may only be set once for a class.
 
-"""
+"""  # noqa: E501 line too long
 import grokcore.security as grok
 
+
 class One(grok.Permission):
     grok.name('permission.1')
 
+
 class Two(grok.Permission):
     grok.name('permission.2')
 
+
 class MultipleView(grok.Context):
     grok.require(One)
     grok.require(Two)
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/tests/base/security/not_a_permissionclass.py` & `grokcore.security-4.0/src/grokcore/security/tests/base/security/not_a_permissionclass.py`

 * *Files identical despite different names*

### Comparing `grokcore.security-3.0.1/src/grokcore/security/tests/base/security/permission.py` & `grokcore.security-4.0/src/grokcore/security/tests/base/security/permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,11 +25,12 @@
 
   >>> print(permission.description)
   This is *the* permission.
 """
 
 import grokcore.security as grok
 
+
 class ThePermission(grok.Permission):
     grok.name('the.permission')
     grok.title('The permission!')
     grok.description('This is *the* permission.')
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/tests/base/security/protect_getattr.py` & `grokcore.security-4.0/src/grokcore/security/tests/base/security/protect_getattr.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
   >>> obj = ProxyFactory(obj)
   >>> checker = getChecker(obj)
   >>> checker.permission_id('protected')
   'the.permission'
 """
 import grokcore.security as grok
 
+
 class ThePermission(grok.Permission):
     grok.name('the.permission')
 
+
 class ProtectedObject(grok.Context):
     grok.require(ThePermission)
 
     protected = 'this is protected'
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/tests/functional/role/roles.py` & `grokcore.security-4.0/src/grokcore/security/tests/functional/role/roles.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 Viewing a protected view with insufficient privileges will yield
 Unauthorized:
 
   >>> from zope.testbrowser.wsgi import Browser
   >>> browser = Browser()
+  >>> # Work around https://github.com/python/cpython/issues/90113
+  >>> browser.raiseHttpErrors = False
 
   >>> browser.open("http://localhost/@@cavepainting")
-  Traceback (most recent call last):
-  urllib.error.HTTPError: HTTP Error 401: Unauthorized
+  >>> print(browser.headers['status'])
+  401 Unauthorized
 
   >>> browser.open("http://localhost/@@editcavepainting")
-  Traceback (most recent call last):
-  urllib.error.HTTPError: HTTP Error 401: Unauthorized
+  >>> print(browser.headers['status'])
+  401 Unauthorized
 
   >>> browser.open("http://localhost/@@erasecavepainting")
-  Traceback (most recent call last):
-  urllib.error.HTTPError: HTTP Error 401: Unauthorized
+  >>> print(browser.headers['status'])
+  401 Unauthorized
 
 Let's now grant anonymous the PaintingOwner role locally (so that we
 don't have to modify the global setup).  Then we can access the views
 just fine:
 
   >>> from zope.securitypolicy.interfaces import IPrincipalRoleManager
   >>> root = getRootFolder()
@@ -35,65 +37,75 @@
   Let's make it even prettier.
 
   >>> browser.open("http://localhost/@@erasecavepainting")
   >>> print(browser.contents)
   Oops, mistake, let's erase it.
 
   >>> browser.open("http://localhost/@@approvecavepainting")
-  Traceback (most recent call last):
-  urllib.error.HTTPError: HTTP Error 401: Unauthorized
+  >>> print(browser.headers['status'])
+  401 Unauthorized
 """
 
-import grokcore.security
-import grokcore.view
 import grokcore.component as grok
+import grokcore.view
 import zope.interface
 
+import grokcore.security
+
+
 class ViewPermission(grokcore.security.Permission):
     grok.name('paint.ViewPainting')
 
+
 class EditPermission(grokcore.security.Permission):
     grok.name('paint.EditPainting')
 
+
 class ErasePermission(grokcore.security.Permission):
     grok.name('paint.ErasePainting')
 
+
 class ApprovePermission(grokcore.security.Permission):
     grok.name('paint.ApprovePainting')
 
+
 class PaintingOwner(grokcore.security.Role):
     grok.name('paint.PaintingOwner')
     grok.title('Painting Owner')
     grokcore.security.permissions(
         'paint.ViewPainting', 'paint.EditPainting', 'paint.ErasePainting')
 
+
 class CavePainting(grokcore.view.View):
 
     grok.context(zope.interface.Interface)
     grokcore.security.require(ViewPermission)
 
     def render(self):
         return 'What a beautiful painting.'
 
+
 class EditCavePainting(grokcore.view.View):
 
     grok.context(zope.interface.Interface)
     grokcore.security.require(EditPermission)
 
     def render(self):
         return 'Let\'s make it even prettier.'
 
+
 class EraseCavePainting(grokcore.view.View):
 
     grok.context(zope.interface.Interface)
     grokcore.security.require(ErasePermission)
 
     def render(self):
         return 'Oops, mistake, let\'s erase it.'
 
+
 class ApproveCavePainting(grokcore.view.View):
 
     grok.context(zope.interface.Interface)
     grokcore.security.require(ApprovePermission)
 
     def render(self):
         return 'Painting owners cannot approve their paintings.'
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/tests/test_functional.py` & `grokcore.security-4.0/src/grokcore/security/tests/test_functional.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,54 @@
 import doctest
-import grokcore.security
-import re
 import unittest
-import zope.app.wsgi.testlayer
-import zope.testbrowser.wsgi
 
 from pkg_resources import resource_listdir
-from zope.testing import renormalizing
+
+import zope.app.wsgi.testlayer
+import zope.testbrowser.wsgi
 from zope.app.wsgi.testlayer import http
 
+import grokcore.security
+
 
 class Layer(
         zope.testbrowser.wsgi.TestBrowserLayer,
         zope.app.wsgi.testlayer.BrowserLayer):
     pass
 
 
 layer = Layer(grokcore.security, allowTearDown=True)
 
 
-checker = renormalizing.RENormalizing([
-    # Accommodate to exception wrapping in newer versions of mechanize
-    (re.compile(r'httperror_seek_wrapper:', re.M), 'HTTPError:'),
-    ])
-
-
 def suiteFromPackage(name):
     layer_dir = 'functional'
-    files = resource_listdir(__name__, '{}/{}'.format(layer_dir, name))
+    files = resource_listdir(__name__, f'{layer_dir}/{name}')
     suite = unittest.TestSuite()
     for filename in files:
         if not filename.endswith('.py'):
             continue
         if filename == '__init__.py':
             continue
-        dottedname = 'grokcore.security.tests.%s.%s.%s' % (
+        dottedname = 'grokcore.security.tests.{}.{}.{}'.format(
             layer_dir, name, filename[:-3])
         test = doctest.DocTestSuite(
             dottedname,
-            checker=checker,
             extraglobs=dict(
                 getRootFolder=layer.getRootFolder,
                 http=http,
-                ),
+            ),
             optionflags=(
                 doctest.ELLIPSIS +
                 doctest.NORMALIZE_WHITESPACE +
                 doctest.REPORT_NDIFF +
-                renormalizing.IGNORE_EXCEPTION_MODULE_IN_PYTHON2))
+                doctest.IGNORE_EXCEPTION_DETAIL))
         test.layer = layer
         suite.addTest(test)
     return suite
 
 
 def test_suite():
     suite = unittest.TestSuite()
     for name in [
             'role']:
         suite.addTest(suiteFromPackage(name))
     return suite
-
-if __name__ == '__main__':
-    unittest.main(defaultTest='test_suite')
```

### Comparing `grokcore.security-3.0.1/src/grokcore/security/util.py` & `grokcore.security-4.0/src/grokcore/security/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,42 +15,46 @@
 """
 from martian.error import GrokError
 from zope.component import queryUtility
 from zope.security.interfaces import IPermission
 from zope.security.protectclass import protectName
 from zope.security.protectclass import protectSetAttribute
 
+
 def protect_getattr(class_, name, permission=None):
     """Install a getattr permission check for the attribute ``name``.
 
     If ``permission`` is not supplied, access will be public.
     """
     permission = check_or_default_permission(class_, permission)
     protectName(class_, name, permission)
 
+
 def protect_setattr(class_, name, permission=None):
     """Install a setattr permission check for the attribute ``name``.
 
     If ``permission`` is not supplied, access will be public.
     """
     permission = check_or_default_permission(class_, permission)
     protectSetAttribute(class_, name, permission)
 
+
 def check_or_default_permission(class_, permission):
     """Return default permission (zope.View) if permission is None,
     otherwise make sure permission has been defined.
     """
     if permission is None:
         permission = 'zope.View'
     else:
         check_permission(class_, permission)
     return permission
 
+
 def check_permission(factory, permission):
     """Check whether a permission is defined.
 
     If not, raise error for factory.
     """
     if queryUtility(IPermission, name=permission) is None:
-       raise GrokError('Undefined permission %r in %r. Use '
-                       'grok.Permission first.'
-                       % (permission, factory), factory)
+        raise GrokError('Undefined permission %r in %r. Use '
+                        'grok.Permission first.'
+                        % (permission, factory), factory)
```

### Comparing `grokcore.security-3.0.1/src/grokcore.security.egg-info/PKG-INFO` & `grokcore.security-4.0/src/grokcore.security.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,255 +1,265 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: grokcore.security
-Version: 3.0.1
+Version: 4.0
 Summary: Grok-like configuration for Zope security components
-Home-page: http://grok.zope.org
+Home-page: https://github.com/zopefoundation/grokcore.security
 Author: Grok Team
-Author-email: grok-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL
-Download-URL: http://pypi.python.org/pypi/grokcore.security
-Description: This package provides basic elements for defining Zope permissions and
-        security checkers without ZCML.
-        
-        .. contents::
-        
-        Setting up ``grokcore.security``
-        ================================
-        
-        This package is essentially set up like the `grokcore.component`_
-        package, please refer to its documentation for details.  The
-        additional ZCML lines you will need are::
-        
-          <include package="grokcore.security" file="meta.zcml" />
-          <include package="grokcore.security" />
-        
-        Put this somewhere near the top of your root ZCML file but below the
-        line where you include ``grokcore.component``'s configuration.
-        
-        
-        Defining permissions
-        ====================
-        
-        In `grokcore.component`_, various components are defined (and
-        automatically registered) by subclassing from certain baseclasses.
-        The same applies to defining permissions with ``grokcore.security`` as
-        well::
-        
-          import grokcore.security
-        
-          class EditContent(grokcore.security.Permission):
-              grokcore.security.name('mypkg.EditContent')
-        
-        This defines a permission with the ID ``mypkg.EditContent``.  You must
-        always specify this ID explicitly.  In addition, you can also give the
-        permission a human-readable title and description.  This is useful
-        when your application provides lists of permissions somewhere and you
-        don't want to bother users with deciphering the dotted IDs::
-        
-          import grokcore.security
-        
-          class EditContent(grokcore.security.Permission):
-              grokcore.security.name('mypkg.EditContent')
-              grokcore.security.title('Edit content')
-              grokcore.security.description('Anyone who has this permission may '
-                                            'modify content in the application.')
-        
-        
-        Defining checkers for components
-        ================================
-        
-        ``grokcore.security`` provides some means for defining checkers for
-        components:
-        
-        * ``grokcore.security.require(permission)`` which can be used either
-          as a class-level directive to set a permission for a whole
-          component, or as a decorator to set a permission for a function or
-          method.
-        
-        * ``protect_getattr`` and ``protect_setattr``, available from
-          ``grokcore.security.util``, which take a class, an attribute name
-          and a permission as arguments and define Zope security checkers for
-          getting or setting a particular attribute on instance of said class.
-        
-        With these, you can build grokkers for components that need security
-        declarations.  For instance, the `grokcore.view`_ package uses them to
-        define a grokker that makes security declarations for views::
-        
-          class ViewSecurityGrokker(martian.ClassGrokker):
-              martian.component(grokcore.view.View)
-              martian.directive(grokcore.security.require, name='permission')
-        
-              def execute(self, factory, config, permission, **kw):
-                  for method_name in zope.publisher.interfaces.browser.IBrowserPage:
-                      config.action(
-                          discriminator=('protectName', factory, method_name),
-                          callable=grokcore.security.util.protect_getattr,
-                          args=(factory, method_name, permission),
-                          )
-                  return True
-        
-        With such a grokker, it is possible to protect views like so::
-        
-          class Edit(grokcore.view.View):
-              grokcore.security.require(EditContent)
-        
-        Note how we can simply pass a permission class to the ``require``
-        directive.  Alternatively, you can pass the permission ID::
-        
-          class Edit(grokcore.view.View):
-              grokcore.security.require('mypkg.EditContent')
-        
-        If you wanted to be able to define permissions for individual class
-        methods rather than the whole class, you would simply base your
-        grokker on ``martian.MethodGrokker`` rather than ``ClassGrokker``.
-        The actual mechanics of defining a checker are the same.
-        
-        Please note that ``grokcore.security`` does not yet provide directives
-        that allow you to specify permissions for simple attribute access
-        (read and write).
-        
-        
-        API overview
-        ============
-        
-        ``Permission``
-            Base class for defining permissions.  Use the ``name`` directive
-            to define the mandatory permission ID.  Optionally use the
-            ``title`` and ``description`` directives to give the permission
-            human-readable information.
-        
-        ``Public``
-            Special permission that can be referred to whenever a component
-            should not be protected by a permission at all (public access).
-        
-        ``require(permission_class_or_id)``
-            declares that the use of a particular component (when used as a
-            class-level directive) or a method (when used as a method
-            decorator) requires a certain permission.  The argument can either
-            be a permission class (subclass of ``Permission``) or a permission
-            ID.
-        
-        In addition, the ``grokcore.security`` package exposes the
-        `grokcore.component`_ API.
-        
-        
-        .. _grokcore.component: http://pypi.python.org/pypi/grokcore.component
-        .. _grokcore.view: http://pypi.python.org/pypi/grokcore.view
-        
-        Changes
-        =======
-        
-        3.0.1 (2018-01-12)
-        ------------------
-        
-        - Rearrange tests such that Travis CI can pick up all functional tests too.
-        
-        3.0.0 (2018-01-05)
-        ------------------
-        
-        - Fix several test error that came to light.
-        
-        1.7 (2018-01-03)
-        ----------------
-        
-        - Python 3 compatibility.
-        
-        1.6.3 (2016-01-29)
-        ------------------
-        
-        - Update tests.
-        
-        1.6.2 (2012-05-07)
-        ------------------
-        
-        - Properly declare zope.dottedname as a dependency.
-        
-        1.6.1 (2012-05-02)
-        ------------------
-        
-        - Fix the package to properly work if the extra ``role`` is not
-          specified.
-        
-        1.6 (2012-05-01)
-        ----------------
-        
-        - The Permission and Role components moved from the grok package to the
-          grokcore.security package where it belongs.
-        
-        - The permissions() directive moved from the grok package to
-          grokcore.security where it belongs.
-        
-        1.5 (2010-11-01)
-        ----------------
-        
-        - Upped the requirements for martian and grokcore.component.
-        
-        - Made package comply to zope.org repository policy.
-        
-        1.4 (2009-12-13)
-        ----------------
-        
-        * **note** Backed out the version requirements for
-          grokcore.component-2.0 and martian-0.12. These requirements
-          stood in the way of further development especially towards
-          grok-1.1 based on the ZTK. The 1.3 version should probably
-          have been called 2.0 like with grokcore.component.
-        
-        * Ported setup.py dependency fixes from trunk.
-        
-        * Use zope.security instead of zope.app.security.
-        
-        1.3 (2009-09-16)
-        ----------------
-        
-        * Use the grok.zope.org/releaseinfo information instead of our own
-          copy of ``versions.cfg``, for easier maintenance.
-        
-        * Depend on grokcore.component 2.0 and the 0.12 Martian - this changes
-          inheritance issues but doesn't appear to affect grokcore.security
-          itself.
-        
-        1.2 (2009-09-14)
-        ----------------
-        
-        * Changed the default permissions from grok.View to zope.View. There seems no
-          particular reason not to use the standard zope.View permission defined
-          in zope.app.security.
-        
-          NOTE: YOU MUST STILL ASSIGN THIS PERMISSION TO USERS IN YOUR
-          site.zcml FILE. OTHERWISE YOU DO NOT HAVE ACCESS TO ANY VIEWS.
-        
-        * Made sure to include zope.app.security configuration as well, as that
-          package defines the zope.View permission. Note that in the future this will
-          change to zope.security.
-        
-        * Bring versions.cfg in line with grok 1.0 release candidate
-          versions.cfg.
-        
-        
-        1.1 (2009-07-03)
-        ----------------
-        
-        * Changed the default permissions from zope.Public to grok.View.
-        
-          NOTE: YOU MUST ASSIGN THIS PERMISSION TO USERS IN YOUR
-          site.zcml FILE. OTHERWISE YOU DO NOT HAVE ACCESS TO ANY VIEWS.
-        
-        1.0 (2008-08-03)
-        ----------------
-        
-        * Created ``grokcore.security`` in July 2008 by factoring
-          security-related components, grokkers and directives out of Grok.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Provides-Extra: role
+Provides-Extra: test
+License-File: LICENSE.txt
+
+This package provides basic elements for defining Zope permissions and
+security checkers without ZCML.
+
+.. contents::
+
+Setting up ``grokcore.security``
+================================
+
+This package is essentially set up like the `grokcore.component`_
+package, please refer to its documentation for details.  The
+additional ZCML lines you will need are::
+
+  <include package="grokcore.security" file="meta.zcml" />
+  <include package="grokcore.security" />
+
+Put this somewhere near the top of your root ZCML file but below the
+line where you include ``grokcore.component``'s configuration.
+
+
+Defining permissions
+====================
+
+In `grokcore.component`_, various components are defined (and
+automatically registered) by subclassing from certain baseclasses.
+The same applies to defining permissions with ``grokcore.security`` as
+well::
+
+  import grokcore.security
+
+  class EditContent(grokcore.security.Permission):
+      grokcore.security.name('mypkg.EditContent')
+
+This defines a permission with the ID ``mypkg.EditContent``.  You must
+always specify this ID explicitly.  In addition, you can also give the
+permission a human-readable title and description.  This is useful
+when your application provides lists of permissions somewhere and you
+don't want to bother users with deciphering the dotted IDs::
+
+  import grokcore.security
+
+  class EditContent(grokcore.security.Permission):
+      grokcore.security.name('mypkg.EditContent')
+      grokcore.security.title('Edit content')
+      grokcore.security.description('Anyone who has this permission may '
+                                    'modify content in the application.')
+
+
+Defining checkers for components
+================================
+
+``grokcore.security`` provides some means for defining checkers for
+components:
+
+* ``grokcore.security.require(permission)`` which can be used either
+  as a class-level directive to set a permission for a whole
+  component, or as a decorator to set a permission for a function or
+  method.
+
+* ``protect_getattr`` and ``protect_setattr``, available from
+  ``grokcore.security.util``, which take a class, an attribute name
+  and a permission as arguments and define Zope security checkers for
+  getting or setting a particular attribute on instance of said class.
+
+With these, you can build grokkers for components that need security
+declarations.  For instance, the `grokcore.view`_ package uses them to
+define a grokker that makes security declarations for views::
+
+  class ViewSecurityGrokker(martian.ClassGrokker):
+      martian.component(grokcore.view.View)
+      martian.directive(grokcore.security.require, name='permission')
+
+      def execute(self, factory, config, permission, **kw):
+          for method_name in zope.publisher.interfaces.browser.IBrowserPage:
+              config.action(
+                  discriminator=('protectName', factory, method_name),
+                  callable=grokcore.security.util.protect_getattr,
+                  args=(factory, method_name, permission),
+                  )
+          return True
+
+With such a grokker, it is possible to protect views like so::
+
+  class Edit(grokcore.view.View):
+      grokcore.security.require(EditContent)
+
+Note how we can simply pass a permission class to the ``require``
+directive.  Alternatively, you can pass the permission ID::
+
+  class Edit(grokcore.view.View):
+      grokcore.security.require('mypkg.EditContent')
+
+If you wanted to be able to define permissions for individual class
+methods rather than the whole class, you would simply base your
+grokker on ``martian.MethodGrokker`` rather than ``ClassGrokker``.
+The actual mechanics of defining a checker are the same.
+
+Please note that ``grokcore.security`` does not yet provide directives
+that allow you to specify permissions for simple attribute access
+(read and write).
+
+
+API overview
+============
+
+``Permission``
+    Base class for defining permissions.  Use the ``name`` directive
+    to define the mandatory permission ID.  Optionally use the
+    ``title`` and ``description`` directives to give the permission
+    human-readable information.
+
+``Public``
+    Special permission that can be referred to whenever a component
+    should not be protected by a permission at all (public access).
+
+``require(permission_class_or_id)``
+    declares that the use of a particular component (when used as a
+    class-level directive) or a method (when used as a method
+    decorator) requires a certain permission.  The argument can either
+    be a permission class (subclass of ``Permission``) or a permission
+    ID.
+
+In addition, the ``grokcore.security`` package exposes the
+`grokcore.component`_ API.
+
+
+.. _grokcore.component: http://pypi.python.org/pypi/grokcore.component
+.. _grokcore.view: http://pypi.python.org/pypi/grokcore.view
+
+Changes
+=======
+
+4.0 (2023-07-11)
+----------------
+
+- Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
+
+- Drop support for Python 2.7, 3.4, 3.5, 3.6.
+
+
+3.0.1 (2018-01-12)
+------------------
+
+- Rearrange tests such that Travis CI can pick up all functional tests too.
+
+3.0.0 (2018-01-05)
+------------------
+
+- Fix several test error that came to light.
+
+1.7 (2018-01-03)
+----------------
+
+- Python 3 compatibility.
+
+1.6.3 (2016-01-29)
+------------------
+
+- Update tests.
+
+1.6.2 (2012-05-07)
+------------------
+
+- Properly declare zope.dottedname as a dependency.
+
+1.6.1 (2012-05-02)
+------------------
+
+- Fix the package to properly work if the extra ``role`` is not
+  specified.
+
+1.6 (2012-05-01)
+----------------
+
+- The Permission and Role components moved from the grok package to the
+  grokcore.security package where it belongs.
+
+- The permissions() directive moved from the grok package to
+  grokcore.security where it belongs.
+
+1.5 (2010-11-01)
+----------------
+
+- Upped the requirements for martian and grokcore.component.
+
+- Made package comply to zope.org repository policy.
+
+1.4 (2009-12-13)
+----------------
+
+* **note** Backed out the version requirements for
+  grokcore.component-2.0 and martian-0.12. These requirements
+  stood in the way of further development especially towards
+  grok-1.1 based on the ZTK. The 1.3 version should probably
+  have been called 2.0 like with grokcore.component.
+
+* Ported setup.py dependency fixes from trunk.
+
+* Use zope.security instead of zope.app.security.
+
+1.3 (2009-09-16)
+----------------
+
+* Use the grok.zope.org/releaseinfo information instead of our own
+  copy of ``versions.cfg``, for easier maintenance.
+
+* Depend on grokcore.component 2.0 and the 0.12 Martian - this changes
+  inheritance issues but doesn't appear to affect grokcore.security
+  itself.
+
+1.2 (2009-09-14)
+----------------
+
+* Changed the default permissions from grok.View to zope.View. There seems no
+  particular reason not to use the standard zope.View permission defined
+  in zope.app.security.
+
+  NOTE: YOU MUST STILL ASSIGN THIS PERMISSION TO USERS IN YOUR
+  site.zcml FILE. OTHERWISE YOU DO NOT HAVE ACCESS TO ANY VIEWS.
+
+* Made sure to include zope.app.security configuration as well, as that
+  package defines the zope.View permission. Note that in the future this will
+  change to zope.security.
+
+* Bring versions.cfg in line with grok 1.0 release candidate
+  versions.cfg.
+
+
+1.1 (2009-07-03)
+----------------
+
+* Changed the default permissions from zope.Public to grok.View.
+
+  NOTE: YOU MUST ASSIGN THIS PERMISSION TO USERS IN YOUR
+  site.zcml FILE. OTHERWISE YOU DO NOT HAVE ACCESS TO ANY VIEWS.
+
+1.0 (2008-08-03)
+----------------
+
+* Created ``grokcore.security`` in July 2008 by factoring
+  security-related components, grokkers and directives out of Grok.
```

### Comparing `grokcore.security-3.0.1/src/grokcore.security.egg-info/SOURCES.txt` & `grokcore.security-4.0/src/grokcore.security.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-.travis.yml
-CHANGES.txt
+CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 CREDITS.txt
 LICENSE.txt
 MANIFEST.in
-README.txt
-bootstrap.py
-buildout.cfg
-requirements.txt
+README.rst
+setup.cfg
 setup.py
+tox.ini
 src/grokcore/__init__.py
 src/grokcore.security.egg-info/PKG-INFO
 src/grokcore.security.egg-info/SOURCES.txt
 src/grokcore.security.egg-info/dependency_links.txt
 src/grokcore.security.egg-info/namespace_packages.txt
 src/grokcore.security.egg-info/not-zip-safe
 src/grokcore.security.egg-info/requires.txt
```

