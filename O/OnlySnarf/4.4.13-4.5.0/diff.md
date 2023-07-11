# Comparing `tmp/OnlySnarf-4.4.13.tar.gz` & `tmp/OnlySnarf-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnlySnarf-4.4.13.tar", last modified: Mon Apr 17 17:48:33 2023, max compression
+gzip compressed data, was "OnlySnarf-4.5.0.tar", last modified: Tue Jul 11 19:45:09 2023, max compression
```

## Comparing `OnlySnarf-4.4.13.tar` & `OnlySnarf-4.5.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    30127 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/CHANGELOG.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/LICENSE.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/MANIFEST.in
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.716371 OnlySnarf-4.4.13/OnlySnarf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/__main__.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/OnlySnarf/classes/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/discount.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/element.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15697 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/file.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12176 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/message.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1974 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/poll.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    13655 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/promotion.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4922 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/schedule.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    18008 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/user.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/OnlySnarf/conf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2240 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/conf/config.conf
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2262 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/conf/test-config.conf
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/OnlySnarf/elements/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/elements/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/elements/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/elements/login.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/elements/profile.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/OnlySnarf/lib/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/lib/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   163434 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/lib/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/lib/ffmpeg.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5069 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/snarf.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/OnlySnarf/util/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/util/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1321 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/util/args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/util/colorize.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1482 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/util/config.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3114 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/util/defaults.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/util/logger.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12152 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/util/optional_args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    19125 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/util/settings.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3725 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/util/validators.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.716371 OnlySnarf-4.4.13/OnlySnarf.egg-info/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3266 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1153 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/SOURCES.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/dependency_links.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       47 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/entry_points.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       53 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/requires.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/top_level.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3266 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2636 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/README.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/setup.cfg
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1285 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/setup.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/tests/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/tests/test_profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/tests/test_promotion.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.054544 OnlySnarf-4.5.0/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    31118 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/CHANGELOG.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/LICENSE.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/MANIFEST.in
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/__main__.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf/classes/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/discount.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/element.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/OnlySnarf/classes/file.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12176 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/message.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1974 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/poll.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.0/OnlySnarf/classes/profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/promotion.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4922 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/classes/schedule.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    18096 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/OnlySnarf/classes/user.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf/conf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2240 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/conf/config.conf
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2263 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/OnlySnarf/conf/test-config.conf
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf/elements/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/elements/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/elements/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/elements/login.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/elements/profile.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf/lib/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/lib/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   163518 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/OnlySnarf/lib/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/lib/ffmpeg.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5130 2023-07-06 00:06:23.000000 OnlySnarf-4.5.0/OnlySnarf/menu.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5069 2023-05-29 23:03:04.000000 OnlySnarf-4.5.0/OnlySnarf/snarf.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.054544 OnlySnarf-4.5.0/OnlySnarf/util/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/util/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1372 2023-07-06 00:40:42.000000 OnlySnarf-4.5.0/OnlySnarf/util/args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/util/colorize.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1482 2023-05-29 23:59:50.000000 OnlySnarf-4.5.0/OnlySnarf/util/config.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3183 2023-05-29 23:06:57.000000 OnlySnarf-4.5.0/OnlySnarf/util/defaults.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/OnlySnarf/util/logger.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12269 2023-05-29 23:06:57.000000 OnlySnarf-4.5.0/OnlySnarf/util/optional_args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    19436 2023-07-06 00:06:23.000000 OnlySnarf-4.5.0/OnlySnarf/util/settings.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/OnlySnarf/util/validators.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.050544 OnlySnarf-4.5.0/OnlySnarf.egg-info/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1171 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/SOURCES.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/dependency_links.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/entry_points.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       62 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/requires.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-07-11 19:45:09.000000 OnlySnarf-4.5.0/OnlySnarf.egg-info/top_level.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-11 19:45:09.054544 OnlySnarf-4.5.0/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.0/README.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-11 19:45:09.054544 OnlySnarf-4.5.0/setup.cfg
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1351 2023-07-11 19:44:50.000000 OnlySnarf-4.5.0/setup.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-11 19:45:09.054544 OnlySnarf-4.5.0/tests/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/tests/test_profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.0/tests/test_promotion.py
```

### Comparing `OnlySnarf-4.4.13/CHANGELOG.md` & `OnlySnarf-4.5.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -668,30 +668,53 @@
   - full test coverage
   - merged w/ main
   - published changes to pypi
   **4.4.11**
   - fixed 'onlysnarf' cmd references
   - removed nonworking browser references in optional args
   - fixed discount bug
-**4.4.12: 3/24/2023**
+  **4.4.12: 3/24/2023**
   - RPi4 debugging
   - fixed element bug when posting
   - fixed users
   - fixed error message on close
   **4/15/2023**
   - cleaned up git repo size / long clone time
 **4.4.13: 4/17/2023**
   - Windows compatability testing
   - updated pathings for Windows
   - retested google login (remains disabled)
-
+**4.4.14 : 5/29/2023**
+  - beginning readd of cli menu
+  - switch from pyinquirer to inquirer
+**4.4.15 : 6/2/2023**
+  - fixed cookies bug
+**4.4.16 : 7/5/2023**
+  - update readme and help&menu docs / added personal touchups
+  - fixed get random user for discount test 
+**4.5.0 : 7/11/2023**
+  - added wget functionality to input for when a url is provided
+  - cleaned up bin/test scripts
+  
 ------------------------------------------------------------------------------------
 
 ## TODO
 
+- fix how tabs open and scroll and then the process opens another tab to find the same elements and scroll again ala: find users then discount user
+
+- add smart idea for getting statement information
+- add better version notes to readme's list of "works on"
+- re-add stuff for testing on multiple platforms ala mac ;) 
+
+- double check how tags & performers are implemented in config and text config and then re-add to docs
+
+- finish updating image/video downloading
+- finish updating cli menu functionality
+- finish updating profile class & menu
+
 - add bypass for 2fa
 https://www.geeksforgeeks.org/two-factor-authentication-using-google-authenticator-in-python/
 https://stackoverflow.com/questions/55870489/how-to-handle-google-authenticator-with-selenium
 https://stackoverflow.com/questions/8529265/google-authenticator-implementation-in-python
 
 (review usability and code first)
 -> OnlyFans: Promos
@@ -727,15 +750,15 @@
 
 -> Tests
 - separate driver functions into individual components ala schedule --> individual steps; for easier testing (and to clean up the giant ass driver file)
 - add tests for newly separated driver files / functions
 - add tests for additional config variables such as browser and image/video options, limits
 - finish adding tests for individual messaging circumstances: all, recent, favorite, renew on
 - finish adding tests for individual message entry parts, individual post entry parts
-- add and finish tests for remote browser testing; requires remote server setup for testing? or test on same device or the rpi
+- add and finish tests for remote browser testing; requires remote server setup for testing? or test on same device or the rpi; readd references to remote in config files and such
 
 (webdriver)
 - (if necessary) finish integrating edge, ie, and opera
 - figure out how to request specific webdriver versions installs to test v102 for edge
 
 -> CLI Menu
 (probably never)
```

### Comparing `OnlySnarf-4.4.13/LICENSE.txt` & `OnlySnarf-4.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/classes/discount.py` & `OnlySnarf-4.5.0/OnlySnarf/classes/discount.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/classes/element.py` & `OnlySnarf-4.5.0/OnlySnarf/classes/element.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/classes/file.py` & `OnlySnarf-4.5.0/OnlySnarf/classes/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os, shutil, random, sys
 from os import walk
 ##
 from ..lib.ffmpeg import ffmpeg
 from ..util.settings import Settings
+import wget
 
 ###############################################################
 
 class File():
     """File class for manipulating files."""
 
     ONE_GIGABYTE = 1000000000
@@ -67,14 +68,23 @@
             Settings.err_print("empty file size")
             return False
         self.size = size
         return True
 
     ##############################
 
+    def download(self):
+        """Download a url. An input can only be a valid path or a valid url."""
+
+        Settings.maybe_print("downloading file...")
+        filename = wget.download(self.path, out=self.get_tmp())
+        Settings.print("") # resume same line after wget download
+        Settings.maybe_print("downloaded: "+filename)
+        self.path = filename
+
     def get_ext(self):
         """Get the file's extension"""
 
         if self.ext != "": return self.ext
         self.get_title()
         return self.ext
 
@@ -154,14 +164,16 @@
         bool
             Whether or not the file is prepared
 
         """
 
         Settings.maybe_print("preparing file: {}".format(self.get_title()))
         # self.get_type().prepare()
+        if not self.check_size():
+            self.download()
         return self.check_size()
 
     @staticmethod
     def get_files_by_folder(path):
         """
         Get local files from the local folder path.
```

### Comparing `OnlySnarf-4.4.13/OnlySnarf/classes/message.py` & `OnlySnarf-4.5.0/OnlySnarf/classes/message.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/classes/poll.py` & `OnlySnarf-4.5.0/OnlySnarf/classes/poll.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/classes/profile.py` & `OnlySnarf-4.5.0/OnlySnarf/classes/profile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python3
 # Profile Settings
 import json
+import inquirer
 ##
 from ..lib.driver import Driver
 from ..util.settings import Settings
 from .user import User
 
 class Profile:
     TABS = ["profile", "advanced", "messaging", "notifications", "security", "story", "other"]
@@ -13,33 +14,64 @@
     #   enabled or disabled
     #   display text, variable type, variable name in settings
     def __init__(self):
         profile = Profile.fill_data()
         for key, value in profile.items():
             setattr(self, str(key), value)
 
+    @staticmethod
+    def ask_action():
+        questions = [
+            inquirer.List('action',
+                message= "Please select an action:",
+                choices= ['Back', 'Backup', 'Check', 'Posts', 'Setup', 'Sync']
+            )
+        ]
+        answers = inquirer.prompt(questions)
+        return answers["action"]
+
     # Backup
 
     @staticmethod
+    def ask_backup():
+        questions = [
+            inquirer.List('backup',
+                message= "Please select a backup action:",
+                choices= ['Back', 'Content', 'Messages']
+            )
+        ]
+        answers = inquirer.prompt(questions)
+        return answers["backup"]
+
+    @staticmethod
+    def backup_menu():
+        action = Profile.ask_backup()
+        if (action == 'Back'): return
+        elif (action == 'Content'): Profile.backup_content()
+        elif (action == 'Messages'): Profile.backup_messages()
+
+    @staticmethod
     def backup_content():
         print("Backing Up: Content")
-        Driver.download_content()
+        driver = Driver.get_driver()
+        driver.download_content()
         ## TODO
-        # files = Driver.download_content()
-        # Files.backup(files)
+        # Files.backup()
         print("Backed Up: Content")
         return True
 
     @staticmethod
     def backup_messages():
         print("Backing Up: Messages")
+        # TODO: add user select
         # select user
         user = "all"
         # user = User.select_user()
-        Driver.download_messages(user)
+        driver = Driver.get_driver()
+        driver.download_messages(user)
         print("Backed Up: Messages")
 
     # new - advertise - tweet to advertise new account, tweet to ask about what you should post
     def advertise():
         pass
 
     def advertise_menu():
@@ -143,22 +175,20 @@
         # elif (action == 'new')
 
         Profile.menu()
 
     @staticmethod
     def menu():
         action = Profile.ask_action()
-        if (action == 'Back'): 
-            from OnlySnarf.bin.menu import Menu
-            return Menu.main_menu()
-        elif (action == 'backup'): Profile.backup_menu()
-        elif (action == 'check'): Profile.check()
-        elif (action == 'posts'): Profile.posts_menu()
-        elif (action == 'setup'): Profile.setup()
-        elif (action == 'sync'): Profile.sync_from_profile()
+        if (action == 'Back'): return
+        elif (action == 'Backup'): Profile.backup_menu()
+        elif (action == 'Check'): Profile.check()
+        elif (action == 'Posts'): Profile.posts_menu()
+        elif (action == 'Setup'): Profile.setup()
+        elif (action == 'Sync'): Profile.sync_from_profile()
         # elif (action == 'sync to'): Profile.sync_to_profile()
         
     @staticmethod
     def get_profile():
         print("Getting Profile")
         profile = Profile()
         for tab in Profile.TABS:
```

### Comparing `OnlySnarf-4.4.13/OnlySnarf/classes/promotion.py` & `OnlySnarf-4.5.0/OnlySnarf/classes/promotion.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/classes/schedule.py` & `OnlySnarf-4.5.0/OnlySnarf/classes/schedule.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/classes/user.py` & `OnlySnarf-4.5.0/OnlySnarf/classes/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,21 +209,21 @@
         -------
         list
             The users
 
         """
 
         Settings.dev_print("getting all users...")
+        users = []
         if Settings.is_prefer_local():
             users = User.read_users_local()
-            if len(users) > 0: return users
-        users = []
-        for user in Driver.users_get():
-            if user is None: continue
-            users.append(User(user))
+        else:
+            for user in Driver.users_get():
+                if user is None: continue
+                users.append(User(user))
         Settings.maybe_print("users: {}".format(len(users)))
         User.write_users_local(users=users)
         Settings.set_prefer_local(True)
         return users
 
     ## TODO
     # make this actually do something
@@ -326,15 +326,17 @@
         classes.User
             A random user
 
         """
 
         Settings.dev_print("getting random user...")
         import random
-        return random.choice(User.get_all_users())
+        randomUser = random.choice(User.get_all_users())
+        Settings.dev_print("random user: {}".format(randomUser.username))
+        return randomUser
 
     @staticmethod
     def get_recent_messagers():
         """
         Get users that have recently sent messages.
 
         Returns
```

### Comparing `OnlySnarf-4.4.13/OnlySnarf/conf/config.conf` & `OnlySnarf-4.5.0/OnlySnarf/conf/config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/conf/test-config.conf` & `OnlySnarf-4.5.0/OnlySnarf/conf/test-config.conf`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # auto, brave, chrome, chromium, firefox, ie, edge, opera; reconnect[-firefox, chrome, etc], remote[-firefox, chrome, etc]
 #browser = auto
 #cookies = True
 #keep = False
 #session_id = 
 #session_url = 
 ## show browser window
-show = True
+show = False
 
 ## Debugging ##
 debug = True
 #debug_cookies = False
 debug_delay = True
 #debug_firefox = False
 #debug_google = False
```

### Comparing `OnlySnarf-4.4.13/OnlySnarf/elements/driver.py` & `OnlySnarf-4.5.0/OnlySnarf/elements/driver.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/elements/login.py` & `OnlySnarf-4.5.0/OnlySnarf/elements/login.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/elements/profile.py` & `OnlySnarf-4.5.0/OnlySnarf/elements/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/lib/driver.py` & `OnlySnarf-4.5.0/OnlySnarf/lib/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,18 +105,19 @@
         Initiliaze the web driver aspect.
 
 
         """
 
         if self._initialized_: return
         self.browser = self.spawn_browser(Settings.get_browser_type())
-        self.browsers.append(self.browser)
-        # ## Cookies
-        # if str(Settings.is_cookies()) == "True": self.cookies_load()
         if self.browser:
+            self.browsers.append(self.browser)
+            ## Cookies
+            if str(Settings.is_cookies()) == "True":
+                self.cookies_load()
             self.tabs.append([self.browser.current_url, self.browser.current_window_handle, 0])
         self._initialized_ = True
         Driver.DRIVERS.append(self)
 
     def auth(self):
         """
         Authorization check
@@ -150,14 +151,15 @@
                 # must be at onlyfans.com to load cookies of onlyfans.com
                 self.go_to_home()
                 file = open(Settings.get_cookies_path(), "rb")
                 cookies = pickle.load(file)
                 file.close()
                 Settings.dev_print("cookies: ")
                 for cookie in cookies:
+                    Settings.dev_print(cookie)
                     self.browser.add_cookie(cookie)
                 Settings.maybe_print("successfully loaded cookies")
                 self.refresh()
             else: 
                 Settings.maybe_print("failed to load cookies, do not exist")
         except Exception as e:
             Settings.print("error loading cookies!")
@@ -166,14 +168,15 @@
     def cookies_save(self):
         """Saves existing web browser cookies to local source"""
 
         Settings.maybe_print("saving cookies...")
         try:
             # must be at onlyfans.com to save cookies of onlyfans.com
             self.go_to_home()
+            Settings.dev_print(self.browser.get_cookies())
             file = open(Settings.get_cookies_path(), "wb")
             pickle.dump(self.browser.get_cookies(), file) # "cookies.pkl"
             file.close()
             Settings.maybe_print("successfully saved cookies")
         except Exception as e:
             Settings.print("failed to save cookies!")
             Settings.dev_print(e)
@@ -401,44 +404,76 @@
                 Settings.err_print("failed to find content to scroll")
         scroll_to_bottom()
         imagesDownloaded = self.download_images()
         videosDownloaded = self.download_videos()
         Settings.print("downloaded content")
         Settings.print("count: {}".format(len(imagesDownloaded)+len(videosDownloaded)))
 
-    def download_images(self):
+    def download_images(self, destination=None):
         """Downloads all images on the page"""
 
-        imagesDownloaded = []
+        downloaded = []
+        downloadMe = []
         try:
             images = self.browser.find_elements(By.TAG_NAME, "img")
-            downloadPath = os.path.join(Settings.get_download_path(), "images")
-            Path(downloadPath).mkdir(parents=True, exist_ok=True)
-            i=1
-            for image in images:
-                if Driver.DOWNLOADING_MAX and i > Driver.DOWNLOAD_MAX_IMAGES: break
+            end = len(images)
+            if len(images) == 0:
+                Settings.warn_print("no images found!")
+                return downloaded
+            if not destination: destination = os.path.join(Settings.get_download_path(), "images")
+            Path(destination).mkdir(parents=True, exist_ok=True)
+            i=0
+            for j in range(end):
+                try:
+                    images = self.browser.find_elements(By.TAG_NAME, "img")
+                    # click on each image
+                    # download each image via class "pswp__img"
+                    self.move_to_then_click_element(images[i])
+                    time.sleep(1)
+                    hdImages = self.browser.find_elements(By.CLASS_NAME, "pswp__img")
+                    downloadMe.extend(hdImages)
+                except Exception as err:
+                    Settings.print("")            
+                    Settings.warn_print(err)
+                finally:
+                    ActionChains(self.browser).send_keys(Keys.ESCAPE).perform()
+                    i+=1
+            Settings.print("")
+        except Exception as err:
+            Settings.err_print(err)
+
+        downloadMe = list(set(downloadMe)) # remove duplicates
+
+        i=1
+        for image in downloadMe:
+            src = ""
+            try:
+                # if Driver.DOWNLOADING_MAX and i > Driver.DOWNLOAD_MAX_IMAGES: break
                 src = str(image.get_attribute("src"))
                 if not src or src == "" or src == "None" or "/thumbs/" in src or "_frame_" in src or "http" not in src: continue
                 Settings.print_same_line("downloading image: {}/{}".format(i, len(images)))
                 # Settings.print("Image: {}".format(src[:src.find(".jpg")+4]))
-                # Settings.print("Image: {}".format(src))
-                if Driver.DOWNLOADING:
-                    try:
-                        while os.path.isfile("{}/{}.jpg".format(downloadPath, i)):
-                            i+=1
-                        wget.download(src, "{}/{}.jpg".format(downloadPath, i), False)
-                        imagesDownloaded.append(i)
-                    except Exception as e: Settings.print(e)
+                # Settings.dev_print("image src: {}".format(src))
+                    # while os.path.isfile("{}/{}.jpg".format(destination, i)):
+                        # i+=1
+
+                # TODO: maybe open image in new tab then download it
+
+                wget.download(src, "{}/{}.jpg".format(destination, i), False)
+                downloaded.append(i)
+            except Exception as err:
+                Settings.print("")            
+                Settings.err_print(err)
+                Settings.warn_print("skipped image: "+src)
+            finally:
                 i+=1
-            Settings.print("")
-        except Exception as e:
-            Settings.print(e)
-        return imagesDownloaded
 
-    def download_messages(self, user="all"):
+        return downloaded
+
+    def download_messages(self, user="all", destination=None):
         """
         Downloads all content in messages with the user
 
         Parameters
         ----------
         user : str or classes.User
             The user to download message content from
@@ -448,65 +483,100 @@
         Settings.print("downloading messages: {}".format(user))
         try:
             if str(user) == "all":
                 # from OnlySnarf.classes.user import User
                 from ..classes.user import User
                 user = random.choice(User.get_all_users())
             self.message_user(user.username)
+            time.sleep(1)
             contentCount = 0
             while True:
                 self.browser.execute_script("document.querySelector('div[id=chatslist]').scrollTop=1e100")
                 time.sleep(1)
                 self.browser.execute_script("document.querySelector('div[id=chatslist]').scrollTop=1e100")
                 time.sleep(1)
                 self.browser.execute_script("document.querySelector('div[id=chatslist]').scrollTop=1e100")
                 time.sleep(1)
                 images = self.browser.find_elements(By.TAG_NAME, "img")
                 videos = self.browser.find_elements(By.TAG_NAME, "video")
                 # Settings.print((len(images)+len(videos)))
                 if contentCount == len(images)+len(videos): break
                 contentCount = len(images)+len(videos)
             # download all images and videos
+
+            # TODO: download into correct user folders by username
             imagesDownloaded = self.download_images()
             videosDownloaded = self.download_videos()
+
             Settings.print("downloaded messages")
             Settings.print("count: {}".format(len(imagesDownloaded)+len(videosDownloaded)))
         except Exception as e:
-            Settings.maybe_print(e)
+            Settings.err_print(e)
 
-    def download_videos(self):
+    def download_videos(self, destination=None):
         """Downloads all videos on the page"""
 
-        videosDownloaded = []
+        downloaded = []
+        downloadMe = []
         try:
             # find all video elements on page
-            videos = self.browser.find_elements(By.TAG_NAME, "video")
-            downloadPath = os.path.join(Settings.get_download_path(), "videos")
-            Path(downloadPath).mkdir(parents=True, exist_ok=True)
+            # videos = self.browser.find_elements(By.TAG_NAME, "video")
+            # videos = self.browser.find_elements(By.CLASS_NAME, "m-video-item")
+            playButtons = self.browser.find_elements(By.CLASS_NAME, "b-photos__item__play-btn")
+            end = len(playButtons)
+
+            if len(playButtons) == 0:
+                Settings.warn_print("no videos found!")
+                return downloaded
+            if not destination: destination = os.path.join(Settings.get_download_path(), "videos")
+            Path(destination).mkdir(parents=True, exist_ok=True)
+            i=0
+            for j in range(end):
+                src = ""
+                playButtons = self.browser.find_elements(By.CLASS_NAME, "b-photos__item__play-btn")
+
+                try:
+                    # click on play button
+                    # find new and only video ele on page
+                    self.move_to_then_click_element(playButtons[i])
+                    time.sleep(3)
+                    video = self.browser.find_element(By.TAG_NAME, "video")
+                    # if Driver.DOWNLOADING_MAX and i > Driver.DOWNLOAD_MAX_VIDEOS: break
+                    src = str(video.get_attribute("src"))
+                    if not src or src == "" or src == "None" or "http" not in src: continue
+                    downloadMe.append(src)
+                except Exception as e:
+                    Settings.warn_print(e)
+                finally:
+                    ActionChains(self.browser).send_keys(Keys.ESCAPE).perform()
+                    i+=1
+
+            downloadMe = list(set(downloadMe)) # remove duplicates
+
             i=1
-            # download all video.src -> /arrrg/$username/videos            
-            for video in videos:
-                if Driver.DOWNLOADING_MAX and i > Driver.DOWNLOAD_MAX_VIDEOS: break
-                src = str(video.get_attribute("src"))
-                if not src or src == "" or src == "None" or "http" not in src: continue
-                Settings.print_same_line("downloading video: {}/{}".format(i, len(videos)))
-                # Settings.print("Video: {}".format(src[:src.find(".mp4")+4]))
-                # Settings.print("Video: {}".format(src))
-                if Driver.DOWNLOADING:
-                    try:
-                        while os.path.isfile("{}/{}.mp4".format(downloadPath, i)):
-                            i+=1
-                        wget.download(src, "{}/{}.mp4".format(downloadPath, i), False)
-                        videosDownloaded.append(i)
-                    except Exception as e: Settings.print(e)
-                i+=1
+            for src in downloadMe:
+                try:
+                    Settings.print_same_line("downloading video: {}/{}".format(i, end))
+                    # Settings.print("Video: {}".format(src[:src.find(".mp4")+4]))
+                    Settings.dev_print("video src: {}".format(src))
+                    # while os.path.isfile("{}/{}.mp4".format(destination, i)):
+                        # i+=1
+                    wget.download(src, "{}/{}.mp4".format(destination, i), False)
+                    downloaded.append(i)
+                except Exception as e:
+                    Settings.print("")            
+                    Settings.err_print(e)
+                    Settings.warn_print("skipped video: "+src)
+                finally:
+                    ActionChains(self.browser).send_keys(Keys.ESCAPE).perform()
+                    i+=1
             Settings.print("")
         except Exception as e:
-            Settings.print(e)
-        return videosDownloaded
+            Settings.err_print(e)
+        return downloaded
 
     @staticmethod
     def drag_and_drop_file(drop_target, path):
         """
         Drag and drop the provided file path onto the provided element target.
 
 
@@ -1317,26 +1387,26 @@
             if loggedin_check():
                 self.logged_in = True
                 return True
         except Exception as e:
             Settings.err_print(e)
             return False
 
-        if str(Settings.is_cookies()) == "True":
-            self.cookies_load()
-            if loggedin_check():
-                self.logged_in = True
-                return True
-            elif str(Settings.is_cookies()) == "True" and str(Settings.is_debug("cookies")) == "True":
-                Settings.err_print("failed to login from cookies!")
-                Settings.set_cookies(False)
-                return False
-            elif str(Settings.is_cookies()) == "True":
-                Settings.set_cookies(False)
-                Settings.maybe_print("failed to login from cookies!")
+        # if str(Settings.is_cookies()) == "True":
+        #     self.cookies_load()
+        #     if loggedin_check():
+        #         self.logged_in = True
+        #         return True
+        #     elif str(Settings.is_cookies()) == "True" and str(Settings.is_debug("cookies")) == "True":
+        #         Settings.err_print("failed to login from cookies!")
+        #         Settings.set_cookies(False)
+        #         return False
+        #     elif str(Settings.is_cookies()) == "True":
+        #         Settings.set_cookies(False)
+        #         Settings.maybe_print("failed to login from cookies!")
 
         Settings.dev_print("attempting login...")
         successful = False
         try:
             if Settings.get_login_method() == "auto":
                 successful = via_form()
                 if not successful: successful = via_twitter()
@@ -2828,16 +2898,16 @@
             options.add_argument("--disable-gpu")
             options.add_argument("--disable-extensions")
             options.add_argument("--disable-dev-shm-usage")
 
             # if os.name == 'nt':
                 # options.add_argument(r"--user-data-dir=C:\Users\brain\AppData\Local\Google\Chrome\User Data")
             # else:
-                # options.add_argument("--user-data-dir="+os.path.join(Settings.get_base_directory(),"tmp","selenium")) # do not disable, required for cookies to work 
-            options.add_argument(r'--profile-directory=Alex D') #e.g. Profile 3
+            options.add_argument("--user-data-dir="+os.path.join(Settings.get_base_directory(),"tmp","selenium")) # do not disable, required for cookies to work 
+            # options.add_argument(r'--profile-directory=Alex D') #e.g. Profile 3
             
             # options.add_argument("--allow-insecure-localhost")            
             # possibly linux only
             # options.add_argument('disable-notifications')
             # https://stackoverflow.com/questions/50642308/webdriverexception-unknown-error-devtoolsactiveport-file-doesnt-exist-while-t
             # options.add_arguments("start-maximized"); // open Browser in maximized mode
             # options.add_argument("--window-size=1920,1080")
@@ -3295,84 +3365,36 @@
 
         """
 
         users = []
         try:
             driver = Driver.get_driver()
             driver.go_to_page(page)
-            user_count = driver.browser.find_elements(By.TAG_NAME, "a")
-            # for debugging new regexes:
-            for ele in user_count:
-                Settings.dev_print("{}  -  {}".format(ele.get_attribute("href"), ele.get_attribute("innerHTML")))
-            user_count = [ele.get_attribute("innerHTML").strip() for ele in user_count
-                            if "/my/subscribers/active" in str(ele.get_attribute("href"))]
-            user_count = user_count[2] # get 3rd occurrence
-            # should be:
-            # '<span data-v-601d81dd="" class="l-sidebar__user-data__item__count"> 190 </span><span data-v-601d81dd="" class="l-sidebar__user-data__item__text m-break-word"> Fans </span>', 
-            user_count = re.search(r'>\s*[0-9]+\s*<', str(user_count))
-            Settings.dev_print(user_count)
-            user_count = user_count.group()
-            user_count = user_count.replace("<","").replace(">","").strip()
-            Settings.dev_print(user_count)
-            if not user_count or not user_count.isnumeric():
-                raise Exception("unable to find fan count!")
-            Settings.maybe_print("num fans found: "+user_count)
+            # scroll until elements stop spawning
             thirdTime = 0
             count = 0
             while True:
                 elements = driver.browser.find_elements(By.CLASS_NAME, "m-fans")
-                if len(elements) == int(user_count): break
                 if len(elements) == int(count) and thirdTime >= 3: break
-                Settings.print_same_line("({}/{}) scrolling...".format(count, user_count))
+                Settings.print_same_line("({}) scrolling...".format(count))
                 count = len(elements)
                 driver.browser.execute_script("window.scrollTo(0, document.body.scrollHeight);")
                 time.sleep(2)
                 if thirdTime >= 3 and len(elements) == 0: break
                 thirdTime += 1
             Settings.print("")
             elements = driver.browser.find_elements(By.CLASS_NAME, "m-fans")
             Settings.dev_print("searching fan elements...")
             for ele in elements:
-
-                # TODO ?
-                # add checks for lists here
-
-                # /my/favorites
-                # /my/lists/34324234
-
-                # eles_ = ele.find_elements(By.TAG_NAME, "a")
-                # isFavorite = False
-                # eles = [ele for ele in eles_
-                #     if "/my/favorites" in str(ele.get_attribute("href"))]
-                # if len(eles) > 0: isFavorite = True
-
-                # lists = []
-                # eles = [ele.get_attribute("href") for ele in eles_
-                #     if "/my/lists" in str(ele.get_attribute("href"))]
-                # for list_ in eles:
-                #     listNum = str(list_).replace("https://onlyfans.com/my/lists/", "")
-                #     Settings.maybe_print("list #: {}".format(listNum))
-                #     lists.append(listNum)
-
-                    ##
-                    # need to open tab and find name of list if not already known
-                    ##
-                    # check if list name is already known
-                    # open tab to list page
-                    # find html on page with list name
-                    # save list
-                # Settings.dev_print("successfully found lists")
                 username = ele.find_element(By.CLASS_NAME, "g-user-username").get_attribute("innerHTML").strip()
                 name = ele.find_element(By.CLASS_NAME, "g-user-name").get_attribute("innerHTML")
                 name = re.sub("<!-*>", "", name)
                 name = re.sub("<.*\">", "", name)
                 name = re.sub("</.*>", "", name).strip()
-                # start = datetime.strptime(str(datetime.now()), "%m-%d-%Y:%H:%M")
-                # users.append({"name":name, "username":username.replace("@",""), "isFavorite":isFavorite, "lists":lists}) # ,"id":user_id, "started":start})
-                users.append({"name":name, "username":username.replace("@","")}) # ,"id":user_id, "started":start})
+                users.append({"name":name, "username":username.replace("@","")})
                 Settings.dev_print(users[-1])
             Settings.maybe_print("found {} fans".format(len(users)))
             Settings.dev_print("successfully found fans")
         except Exception as e:
             Settings.print(e)
             Driver.error_checker(e)
             Settings.err_print("failed to find fans")
```

### Comparing `OnlySnarf-4.4.13/OnlySnarf/lib/ffmpeg.py` & `OnlySnarf-4.5.0/OnlySnarf/lib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/snarf.py` & `OnlySnarf-4.5.0/OnlySnarf/snarf.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/util/args.py` & `OnlySnarf-4.5.0/OnlySnarf/util/args.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 apply_args(parser)
 
 ##
 import pkg_resources
 parser.version = str(pkg_resources.get_distribution("onlysnarf").version)
 parser.add_argument('-version', action='version')
 
+parser.add_argument('-version', action='version')
+
 ############################################################################################
 
 try:
   parsedargs, unknownargs = parser.parse_known_args()
   # print("unknown args: {}".format(unknownargs))
   args.update(vars(parsedargs))
 except Exception as e:
```

### Comparing `OnlySnarf-4.4.13/OnlySnarf/util/colorize.py` & `OnlySnarf-4.5.0/OnlySnarf/util/colorize.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/util/config.py` & `OnlySnarf-4.5.0/OnlySnarf/util/config.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/util/defaults.py` & `OnlySnarf-4.5.0/OnlySnarf/util/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from datetime import datetime
 from pathlib import Path
 
 ##
 # Defaults 
 ##
 
+ACTIONS = [ "Discount", "Message", "Post", "Profile", "Promotion" ]
+
 AMOUNT_NONE = 0
 
 DATE_FORMAT = "%m/%d/%Y"
 TIME_FORMAT = "%H:%M:%S"
 SCHEDULE_FORMAT = "{} {}".format(DATE_FORMAT, TIME_FORMAT)
 
 date_ = datetime.strptime(str(datetime.now().strftime(SCHEDULE_FORMAT)), SCHEDULE_FORMAT)
```

### Comparing `OnlySnarf-4.4.13/OnlySnarf/util/logger.py` & `OnlySnarf-4.5.0/OnlySnarf/util/logger.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/OnlySnarf/util/optional_args.py` & `OnlySnarf-4.5.0/OnlySnarf/util/optional_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,20 @@
   # the user to discount
   userAndUsers.add_argument('-user', type=str,  default=None, dest='user', help='user to discount')
   ##
   # -users
   # the users to discount
   userAndUsers.add_argument('-users', dest='users', action='append', default=[], help='users to discount')
 
+  ##########
+  ## Menu ##
+  ##########
+
+  parser_menu = subparsers.add_parser('menu', help='> access the cli menu')
+
   #############
   ## Message ##
   #############
 
   parser_message = subparsers.add_parser('message', help='> send a message to one or more users')
   dateAndSchedule = parser_message.add_mutually_exclusive_group()
   userAndUsers = parser_message.add_mutually_exclusive_group()
```

### Comparing `OnlySnarf-4.4.13/OnlySnarf/util/settings.py` & `OnlySnarf-4.5.0/OnlySnarf/util/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     def print_same_line(text):
         sys.stdout.write('\r')
         sys.stdout.flush()
         sys.stdout.write(text)
         sys.stdout.flush()
 
     def maybe_print(text):
-        if int(config["verbose"]) >= 1:
+        if int(config["verbose"]) >= 1 or str(os.environ.get("ENV")) == "test":
             log.debug(text)
 
     def dev_print(text):
-        if int(config["verbose"]) >= 2:
+        if int(config["verbose"]) >= 2 or str(os.environ.get("ENV")) == "test":
             log.debug(text)
 
     def err_print(error):
         log.error(error)
 
     def warn_print(error):
         log.warning(error)
@@ -63,14 +63,26 @@
 
     def format_time(time):
         if isinstance(time, str):
             return datetime.strptime(time, DEFAULT.TIME_FORMAT).strftime(DEFAULT.TIME_FORMAT)
         else:
             return time.strftime(DEFAULT.TIME_FORMAT)
 
+    def header():
+        Settings.print("### SETTINGS ###")
+        Settings.print("...")
+        Settings.print("...")
+        Settings.print("...")
+
+    def menu():
+        Settings.print("### SETTINGS MENU ###")
+        Settings.print("...")
+        Settings.print("...")
+        Settings.print("...")
+
     ##
     # Getters
     ##
 
     def get_action():
         return config["action"]
 
@@ -220,15 +232,15 @@
             return os.path.join(path_, "chromedriver.log")
         return ""
 
     def get_message_choices():
         return DEFAULT.MESSAGE_CHOICES
 
     def get_root_path():
-        return config["root_path"] or DEFAULT.ROOT_PATH
+        return DEFAULT.ROOT_PATH
 
     def get_sort_method():
         return config["sort"] or "random"
 
     def get_performers():
         try:
             performers = config["performers"] or []
@@ -386,17 +398,14 @@
             elif isinstance(user, int): user = User({"id":user})
             users.append(user)
         return users
 
     def get_user():
         return Settings.get_users()[0]
 
-    def get_email():
-        return config["email"]
-
     def get_user_configs():
         # load configs from .onlysnarf or baseDir
         pass
 
     def get_user_config(username="default"):
         import configparser
         config_file = configparser.ConfigParser()
```

### Comparing `OnlySnarf-4.4.13/OnlySnarf/util/validators.py` & `OnlySnarf-4.5.0/OnlySnarf/util/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse, os
+import validators
 from datetime import datetime
 from . import defaults as DEFAULT
 
 # Validators
 
 #
 # Args
@@ -87,15 +88,23 @@
 
 def valid_path(s):
 	try:
 		if isinstance(s, list):
 			for f in s: os.stat(s)
 		else: os.stat(s)
 	except FileNotFoundError:
-		msg = "Not a valid path: '{0}'.".format(s)
+		# check as url
+		return valid_url(s)
+		# msg = "Not a valid path: '{0}'.".format(s)
+		# raise argparse.ArgumentTypeError(msg)
+	return s
+
+def valid_url(s):
+	if not validators.url(s):
+		msg = "Not a valid path or url: '{0}'.".format(s)
 		raise argparse.ArgumentTypeError(msg)
 	return s
 
 def valid_price(s):
 	if str(s) == "max": return DEFAULT.PRICE_MAXIMUM
 	elif str(s) == "min": return DEFAULT.PRICE_MINIMUM
 	try: return "{:.2f}".format(float(s))
```

### Comparing `OnlySnarf-4.4.13/OnlySnarf.egg-info/SOURCES.txt` & `OnlySnarf-4.5.0/OnlySnarf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 OnlySnarf/__init__.py
 OnlySnarf/__main__.py
+OnlySnarf/menu.py
 OnlySnarf/snarf.py
 OnlySnarf.egg-info/PKG-INFO
 OnlySnarf.egg-info/SOURCES.txt
 OnlySnarf.egg-info/dependency_links.txt
 OnlySnarf.egg-info/entry_points.txt
 OnlySnarf.egg-info/requires.txt
 OnlySnarf.egg-info/top_level.txt
```

### Comparing `OnlySnarf-4.4.13/setup.py` & `OnlySnarf-4.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OnlySnarf",
-    version="4.4.13",
+    version="4.5.0",
     author="Skeetzo",
     author_email="WebmasterSkeetzo@gmail.com",
     url = 'https://github.com/skeetzo/onlysnarf',
     keywords = ['OnlyFans', 'OnlySnarf', 'selenium', 'snarf'],
     description="OnlyFans Content Distribution Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # packages=setuptools.find_packages(),
     packages=["OnlySnarf", "OnlySnarf/classes","OnlySnarf/conf","OnlySnarf/elements","OnlySnarf/lib","OnlySnarf/util"],
     include_package_data=True,
     install_requires=[
         'ffmpeg',
+        'inquirer',
         'wget',
         'selenium',
         'webdriver_manager'
         ],
     extras_require={
         'dev': [
             'pytest'
         ]
     },
     entry_points={
         'console_scripts' : [
+            'onlysnarf = OnlySnarf.menu:main',
             'snarf = OnlySnarf.snarf:main'
         ]
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: End Users/Desktop',
         'Topic :: System :: Emulators',
```

### Comparing `OnlySnarf-4.4.13/tests/test_profile.py` & `OnlySnarf-4.5.0/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.13/tests/test_promotion.py` & `OnlySnarf-4.5.0/tests/test_promotion.py`

 * *Files identical despite different names*

