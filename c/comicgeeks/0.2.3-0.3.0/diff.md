# Comparing `tmp/comicgeeks-0.2.3.tar.gz` & `tmp/comicgeeks-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicgeeks-0.2.3.tar", last modified: Sat Apr  8 11:29:36 2023, max compression
+gzip compressed data, was "comicgeeks-0.3.0.tar", last modified: Tue Jul 11 19:21:04 2023, max compression
```

## Comparing `comicgeeks-0.2.3.tar` & `comicgeeks-0.3.0.tar`

### file list

```diff
@@ -1,63 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 11:29:36.830943 comicgeeks-0.2.3/
--rw-rw-rw-   0        0        0      788 2022-08-08 18:46:53.000000 comicgeeks-0.2.3/.coveragerc
--rw-rw-rw-   0        0        0      195 2022-08-01 18:04:01.000000 comicgeeks-0.2.3/.flake8
--rw-rw-rw-   0        0        0     3274 2022-08-08 19:46:07.000000 comicgeeks-0.2.3/.gitignore
--rw-rw-rw-   0        0        0       61 2022-07-31 17:40:01.000000 comicgeeks-0.2.3/.isort.cfg
--rw-rw-rw-   0        0        0     1431 2022-08-05 14:31:59.000000 comicgeeks-0.2.3/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      560 2022-08-05 13:26:52.000000 comicgeeks-0.2.3/.readthedocs.yml
--rw-rw-rw-   0        0        0     2309 2023-04-08 11:24:17.000000 comicgeeks-0.2.3/CHANGELOG.md
--rw-rw-rw-   0        0        0    10776 2022-08-05 14:32:20.000000 comicgeeks-0.2.3/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    33094 2022-07-31 17:40:01.000000 comicgeeks-0.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2463 2023-04-08 11:29:36.831950 comicgeeks-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1592 2022-08-08 20:11:44.000000 comicgeeks-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 11:29:36.754767 comicgeeks-0.2.3/docs/
--rw-rw-rw-   0        0        0     1183 2022-07-31 17:40:01.000000 comicgeeks-0.2.3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-08 11:29:36.759767 comicgeeks-0.2.3/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-04-08 11:29:36.760768 comicgeeks-0.2.3/docs/_static/css/
--rw-rw-rw-   0        0        0      999 2022-07-31 19:02:28.000000 comicgeeks-0.2.3/docs/_static/css/custom.css
--rw-rw-rw-   0        0        0      299 2022-06-28 16:31:38.000000 comicgeeks-0.2.3/docs/_static/custom.js
--rw-rw-rw-   0        0        0      191 2022-06-22 09:23:44.000000 comicgeeks-0.2.3/docs/_static/debug.js
--rw-rw-rw-   0        0        0    30394 2022-06-28 15:59:36.000000 comicgeeks-0.2.3/docs/_static/icon.png
--rw-rw-rw-   0        0        0    37456 2022-06-28 16:08:46.000000 comicgeeks-0.2.3/docs/_static/icon.svg
--rw-rw-rw-   0        0        0      685 2022-06-22 09:23:44.000000 comicgeeks-0.2.3/docs/_static/revitron-ui-mobile.svg
-drwxrwxrwx   0        0        0        0 2023-04-08 11:29:36.761767 comicgeeks-0.2.3/docs/_templates/
--rw-rw-rw-   0        0        0     1526 2022-07-15 11:19:23.000000 comicgeeks-0.2.3/docs/_templates/layout.html
--rw-rw-rw-   0        0        0       77 2022-07-31 17:40:01.000000 comicgeeks-0.2.3/docs/changelog.md
--rw-rw-rw-   0        0        0    10946 2023-04-08 11:22:39.000000 comicgeeks-0.2.3/docs/conf.py
--rw-rw-rw-   0        0        0       80 2022-07-31 17:40:01.000000 comicgeeks-0.2.3/docs/contributing.md
--rw-rw-rw-   0        0        0    11645 2022-08-05 14:32:20.000000 comicgeeks-0.2.3/docs/examples.md
--rw-rw-rw-   0        0        0        9 2022-08-01 17:10:47.000000 comicgeeks-0.2.3/docs/genindex.md
--rw-rw-rw-   0        0        0      883 2022-08-08 18:47:29.000000 comicgeeks-0.2.3/docs/get-started.md
--rw-rw-rw-   0        0        0      527 2022-08-05 14:32:20.000000 comicgeeks-0.2.3/docs/index.rst
--rw-rw-rw-   0        0        0       71 2022-07-31 17:40:01.000000 comicgeeks-0.2.3/docs/license.md
--rw-rw-rw-   0        0        0      660 2022-08-01 17:56:27.000000 comicgeeks-0.2.3/docs/modules.rst
--rw-rw-rw-   0        0        0      177 2022-08-01 18:13:05.000000 comicgeeks-0.2.3/docs/requirements.txt
--rw-rw-rw-   0        0        0      355 2022-07-31 17:40:01.000000 comicgeeks-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       55 2022-08-01 18:04:04.000000 comicgeeks-0.2.3/requirements.txt
--rw-rw-rw-   0        0        0     1852 2023-04-08 11:29:36.837963 comicgeeks-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      726 2022-07-31 17:40:01.000000 comicgeeks-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 11:29:36.727779 comicgeeks-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 11:29:36.768770 comicgeeks-0.2.3/src/comicgeeks/
--rw-rw-rw-   0        0        0     7359 2023-04-08 11:17:27.000000 comicgeeks-0.2.3/src/comicgeeks/Comic_Geeks.py
--rw-rw-rw-   0        0        0       38 2022-08-01 17:01:21.000000 comicgeeks-0.2.3/src/comicgeeks/__init__.py
--rw-rw-rw-   0        0        0       66 2023-01-16 18:12:33.000000 comicgeeks-0.2.3/src/comicgeeks/__version__.py
--rw-rw-rw-   0        0        0    49778 2023-04-08 11:17:24.000000 comicgeeks-0.2.3/src/comicgeeks/classes.py
--rw-rw-rw-   0        0        0     9540 2022-07-15 11:19:27.000000 comicgeeks-0.2.3/src/comicgeeks/extract.py
--rw-rw-rw-   0        0        0      120 2023-04-08 11:16:45.000000 comicgeeks-0.2.3/src/comicgeeks/test.py
--rw-rw-rw-   0        0        0     1468 2022-08-04 20:35:50.000000 comicgeeks-0.2.3/src/comicgeeks/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-08 11:29:36.821955 comicgeeks-0.2.3/src/comicgeeks.egg-info/
--rw-rw-rw-   0        0        0     2463 2023-04-08 11:29:36.000000 comicgeeks-0.2.3/src/comicgeeks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1129 2023-04-08 11:29:36.000000 comicgeeks-0.2.3/src/comicgeeks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 11:29:36.000000 comicgeeks-0.2.3/src/comicgeeks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-08 11:29:35.000000 comicgeeks-0.2.3/src/comicgeeks.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      250 2023-04-08 11:29:36.000000 comicgeeks-0.2.3/src/comicgeeks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-08 11:29:36.000000 comicgeeks-0.2.3/src/comicgeeks.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 11:29:36.829946 comicgeeks-0.2.3/tests/
--rw-rw-rw-   0        0        0      297 2022-08-04 13:38:03.000000 comicgeeks-0.2.3/tests/conftest.py
--rw-rw-rw-   0        0        0     1897 2022-08-08 18:37:11.000000 comicgeeks-0.2.3/tests/test_Character.py
--rw-rw-rw-   0        0        0     1118 2022-08-04 20:52:35.000000 comicgeeks-0.2.3/tests/test_Creator.py
--rw-rw-rw-   0        0        0     6489 2022-08-08 18:12:12.000000 comicgeeks-0.2.3/tests/test_Issue.py
--rw-rw-rw-   0        0        0     6037 2022-08-07 20:18:53.000000 comicgeeks-0.2.3/tests/test_Series.py
--rw-rw-rw-   0        0        0      498 2022-08-05 11:19:37.000000 comicgeeks-0.2.3/tests/test_new_releases.py
--rw-rw-rw-   0        0        0      780 2022-08-08 18:27:11.000000 comicgeeks-0.2.3/tests/test_session.py
--rw-rw-rw-   0        0        0     2711 2022-09-12 09:30:44.000000 comicgeeks-0.2.3/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.707633 comicgeeks-0.3.0/
+-rw-rw-rw-   0        0        0      788 2022-08-08 18:46:53.000000 comicgeeks-0.3.0/.coveragerc
+-rw-rw-rw-   0        0        0      195 2022-08-01 18:04:01.000000 comicgeeks-0.3.0/.flake8
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.632633 comicgeeks-0.3.0/.github/
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.647631 comicgeeks-0.3.0/.github/workflows/
+-rw-rw-rw-   0        0        0     4016 2023-07-11 17:05:34.000000 comicgeeks-0.3.0/.github/workflows/ci.yml
+-rw-rw-rw-   0        0        0     3274 2022-08-08 19:46:07.000000 comicgeeks-0.3.0/.gitignore
+-rw-rw-rw-   0        0        0       61 2022-07-31 17:40:01.000000 comicgeeks-0.3.0/.isort.cfg
+-rw-rw-rw-   0        0        0     1431 2022-08-05 14:31:59.000000 comicgeeks-0.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      560 2022-08-05 13:26:52.000000 comicgeeks-0.3.0/.readthedocs.yml
+-rw-rw-rw-   0        0        0     3737 2023-07-11 18:15:11.000000 comicgeeks-0.3.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    10776 2022-08-05 14:32:20.000000 comicgeeks-0.3.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    33094 2022-07-31 17:40:01.000000 comicgeeks-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2463 2023-07-11 19:21:04.707633 comicgeeks-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1592 2022-08-08 20:11:44.000000 comicgeeks-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.658632 comicgeeks-0.3.0/docs/
+-rw-rw-rw-   0        0        0     1183 2023-07-11 16:25:48.000000 comicgeeks-0.3.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.663637 comicgeeks-0.3.0/docs/_static/
+-rw-rw-rw-   0        0        0       19 2023-07-11 16:25:48.000000 comicgeeks-0.3.0/docs/_static/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.664631 comicgeeks-0.3.0/docs/_static/css/
+-rw-rw-rw-   0        0        0      999 2022-07-31 19:02:28.000000 comicgeeks-0.3.0/docs/_static/css/custom.css
+-rw-rw-rw-   0        0        0      299 2022-06-28 16:31:38.000000 comicgeeks-0.3.0/docs/_static/custom.js
+-rw-rw-rw-   0        0        0      191 2022-06-22 09:23:44.000000 comicgeeks-0.3.0/docs/_static/debug.js
+-rw-rw-rw-   0        0        0    30394 2022-06-28 15:59:36.000000 comicgeeks-0.3.0/docs/_static/icon.png
+-rw-rw-rw-   0        0        0    37456 2022-06-28 16:08:46.000000 comicgeeks-0.3.0/docs/_static/icon.svg
+-rw-rw-rw-   0        0        0      685 2022-06-22 09:23:44.000000 comicgeeks-0.3.0/docs/_static/revitron-ui-mobile.svg
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.665631 comicgeeks-0.3.0/docs/_templates/
+-rw-rw-rw-   0        0        0     1526 2022-07-15 11:19:23.000000 comicgeeks-0.3.0/docs/_templates/layout.html
+-rw-rw-rw-   0        0        0       77 2022-07-31 17:40:01.000000 comicgeeks-0.3.0/docs/changelog.md
+-rw-rw-rw-   0        0        0    10872 2023-07-11 16:38:28.000000 comicgeeks-0.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0       80 2022-07-31 17:40:01.000000 comicgeeks-0.3.0/docs/contributing.md
+-rw-rw-rw-   0        0        0    11791 2023-07-11 16:10:22.000000 comicgeeks-0.3.0/docs/examples.md
+-rw-rw-rw-   0        0        0        9 2022-08-01 17:10:47.000000 comicgeeks-0.3.0/docs/genindex.md
+-rw-rw-rw-   0        0        0     1247 2023-07-11 16:17:38.000000 comicgeeks-0.3.0/docs/get-started.md
+-rw-rw-rw-   0        0        0      527 2023-07-11 16:40:09.000000 comicgeeks-0.3.0/docs/index.rst
+-rw-rw-rw-   0        0        0       71 2022-07-31 17:40:01.000000 comicgeeks-0.3.0/docs/license.md
+-rw-rw-rw-   0        0        0      810 2023-07-11 16:11:17.000000 comicgeeks-0.3.0/docs/modules.rst
+-rw-rw-rw-   0        0        0       74 2023-07-11 16:25:48.000000 comicgeeks-0.3.0/docs/readme.md
+-rw-rw-rw-   0        0        0      177 2022-08-01 18:13:05.000000 comicgeeks-0.3.0/docs/requirements.txt
+-rw-rw-rw-   0        0        0      355 2022-07-31 17:40:01.000000 comicgeeks-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       55 2022-08-01 18:04:04.000000 comicgeeks-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0     1869 2023-07-11 19:21:04.716634 comicgeeks-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      726 2023-07-11 16:25:48.000000 comicgeeks-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.634631 comicgeeks-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.671631 comicgeeks-0.3.0/src/comicgeeks/
+-rw-rw-rw-   0        0        0     8534 2023-07-11 16:42:17.000000 comicgeeks-0.3.0/src/comicgeeks/Comic_Geeks.py
+-rw-rw-rw-   0        0        0      631 2023-07-11 16:51:21.000000 comicgeeks-0.3.0/src/comicgeeks/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-07-11 18:16:22.000000 comicgeeks-0.3.0/src/comicgeeks/__version__.py
+-rw-rw-rw-   0        0        0    53331 2023-07-11 16:42:14.000000 comicgeeks-0.3.0/src/comicgeeks/classes.py
+-rw-rw-rw-   0        0        0     9540 2022-07-15 11:19:27.000000 comicgeeks-0.3.0/src/comicgeeks/extract.py
+-rw-rw-rw-   0        0        0      222 2023-07-11 16:59:07.000000 comicgeeks-0.3.0/src/comicgeeks/test.py
+-rw-rw-rw-   0        0        0     1682 2023-07-08 19:10:32.000000 comicgeeks-0.3.0/src/comicgeeks/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.698630 comicgeeks-0.3.0/src/comicgeeks.egg-info/
+-rw-rw-rw-   0        0        0     2463 2023-07-11 19:21:04.000000 comicgeeks-0.3.0/src/comicgeeks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1222 2023-07-11 19:21:04.000000 comicgeeks-0.3.0/src/comicgeeks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 19:21:04.000000 comicgeeks-0.3.0/src/comicgeeks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 19:21:03.000000 comicgeeks-0.3.0/src/comicgeeks.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      250 2023-07-11 19:21:04.000000 comicgeeks-0.3.0/src/comicgeeks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-11 19:21:04.000000 comicgeeks-0.3.0/src/comicgeeks.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 19:21:04.706634 comicgeeks-0.3.0/tests/
+-rw-rw-rw-   0        0        0      297 2022-08-04 13:38:03.000000 comicgeeks-0.3.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     2146 2023-07-11 17:09:26.000000 comicgeeks-0.3.0/tests/test_Character.py
+-rw-rw-rw-   0        0        0     1118 2023-07-08 11:11:46.000000 comicgeeks-0.3.0/tests/test_Creator.py
+-rw-rw-rw-   0        0        0     6815 2023-07-11 19:19:56.000000 comicgeeks-0.3.0/tests/test_Issue.py
+-rw-rw-rw-   0        0        0     6428 2023-07-11 17:09:41.000000 comicgeeks-0.3.0/tests/test_Series.py
+-rw-rw-rw-   0        0        0     2947 2023-07-11 19:20:12.000000 comicgeeks-0.3.0/tests/test_TradePaperback.py
+-rw-rw-rw-   0        0        0      498 2022-08-05 11:19:37.000000 comicgeeks-0.3.0/tests/test_new_releases.py
+-rw-rw-rw-   0        0        0     1367 2023-07-11 17:09:46.000000 comicgeeks-0.3.0/tests/test_session.py
+-rw-rw-rw-   0        0        0     2767 2023-07-11 18:02:50.000000 comicgeeks-0.3.0/tox.ini
```

### Comparing `comicgeeks-0.2.3/.coveragerc` & `comicgeeks-0.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/.gitignore` & `comicgeeks-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/.pre-commit-config.yaml` & `comicgeeks-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/.readthedocs.yml` & `comicgeeks-0.3.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/CHANGELOG.md` & `comicgeeks-0.3.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,35 @@
 # Changelog
 
+## 0.3.0 (2023-07-11)
+
+### Features
+
+- login with user and password ([422d044](https://github.com/pruizlezcano/comicgeeks/commit/422d04426e198f9c691c0443cb0f1d48f7a54602))
+- added TradePaperback class ([3620470](https://github.com/pruizlezcano/comicgeeks/commit/3620470d4e3f1a0bd12193f3bdb038e37261f02c))
+- added github actions ([46f4639](https://github.com/pruizlezcano/comicgeeks/commit/46f46396df44ad949f51bab1731bea67bba01705))
+
+### Fixes
+
+- new issue name location ([f837c74](https://github.com/pruizlezcano/comicgeeks/commit/f837c74eb03096d1e3ddc4adf92571543f685862))
+- module export ([9981d02](https://github.com/pruizlezcano/comicgeeks/commit/9981d02557704b124c3e9e580e97a22a46691139))
+
+### Tests
+
+- update for the new session system ([17bacc7](https://github.com/pruizlezcano/comicgeeks/commit/17bacc74000bb1e1a095138f773202b4af4bcd1c))
+- fixed github actions secrets ([2f8ce3c](https://github.com/pruizlezcano/comicgeeks/commit/2f8ce3c54926bb78ccde8eef4bd23693098d9e6c), [8b95823](https://github.com/pruizlezcano/comicgeeks/commit/8b95823705eb42db82268f6c6d48d53318fe4bf6), [8db643d](https://github.com/pruizlezcano/comicgeeks/commit/8db643d334237aab4d1a58e49713a2b6e2aa73e5))
+
+### Refactors
+
+- share client session for all classes ([c6c174b](https://github.com/pruizlezcano/comicgeeks/commit/c6c174bf8a9ca32b82d45e9057a279aa85b9b650))
+
+### Documentation
+
+- added login method and Trade_Paperback class ([40c4094]())
+
 ## 0.2.3 (2023-04-08)
 
 ### Fixes
 
 - **issue:** error getting rating of new issues that haven't had any ratings [#2](https://github.com/pruizlezcano/comicgeeks/issues/2) ([b402714](https://github.com/pruizlezcano/comicgeeks/commit/b40271400e877e792b1be9a2a458e6f5a9eb2eba))
 
 ## 0.2.2 (2023-01-16)
```

### Comparing `comicgeeks-0.2.3/CONTRIBUTING.md` & `comicgeeks-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/LICENSE.txt` & `comicgeeks-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/PKG-INFO` & `comicgeeks-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comicgeeks
-Version: 0.2.3
+Version: 0.3.0
 Summary: A python client for League of Comics Geeks.
 Home-page: https://github.com/pruizlezcano/comicgeeks
 Author: Pablo Ruiz
 Author-email: pruizlezcano@gmail.com
 License: GPL-3.0-only
 Project-URL: Documentation, https://comicgeeks.readthedocs.io
 Project-URL: Source, https://github.com/pruizlezcano/comicgeeks
```

### Comparing `comicgeeks-0.2.3/README.md` & `comicgeeks-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/docs/Makefile` & `comicgeeks-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/docs/_static/css/custom.css` & `comicgeeks-0.3.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/docs/_static/icon.png` & `comicgeeks-0.3.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/docs/_static/icon.svg` & `comicgeeks-0.3.0/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/docs/_static/revitron-ui-mobile.svg` & `comicgeeks-0.3.0/docs/_static/revitron-ui-mobile.svg`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/docs/_templates/layout.html` & `comicgeeks-0.3.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/docs/conf.py` & `comicgeeks-0.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import os
-import shutil
 import sys
+import shutil
 
 # -- Path setup --------------------------------------------------------------
 
 __location__ = os.path.dirname(__file__)
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
@@ -48,15 +48,15 @@
     args = cmd_line.split(" ")
     if tuple(sphinx.__version__.split(".")) >= ("1", "7"):
         # This is a rudimentary parse_version to avoid external dependencies
         args = args[1:]
 
     apidoc.main(args)
 except Exception as e:
-    print(f"Running `sphinx-apidoc` failed!\n{e}")
+    print("Running `sphinx-apidoc` failed!\n{}".format(e))
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
@@ -68,15 +68,14 @@
     "sphinx.ext.autosummary",
     "sphinx.ext.viewcode",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.ifconfig",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
-    "revitron_sphinx_theme",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 
 # Enable markdown
@@ -103,37 +102,30 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "comicgeeks"
-version = "0.2.3"
-release = "0.2.3"
 author = "Pablo Ruiz"
 copyright = '2022 <a href="https://github.com/pruizlezcano">Pablo Ruiz</a>'
-language = "en"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # version: The short X.Y version.
 # release: The full version, including alpha/beta/rc tags.
 # If you don’t need the separation provided between version and release,
 # just set them both to the same value.
-
 try:
     from comicgeeks import __version__ as version
-
-    version = version.__version__
 except ImportError:
     version = ""
 
-
 if not version or version.lower() == "unknown":
     version = os.getenv("READTHEDOCS_VERSION", "unknown")  # automatically set by RTD
 
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
@@ -207,15 +199,16 @@
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
 
-# The name of an image file (relative to this directory)
+# The name of an image file (relative to this directory) to place at the top
+# of the sidebar.
 html_logo = "_static/icon.svg"
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 # html_favicon = None
 
@@ -284,15 +277,15 @@
     # Additional stuff for the LaTeX preamble.
     # "preamble": "",
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ("index", "user_guide.tex", "comicgeeks Documentation", "Pablo", "manual")
+    ("index", "user_guide.tex", "comicgeeks Documentation", "Pablo Ruiz", "manual")
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = ""
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # This file is execfile()d with the current directory set to its containing
 dir. # # This file only contains a selection of the most common options. For a
 full # list see the documentation: # https://www.sphinx-doc.org/en/master/
 usage/configuration.html # # All configuration values have a default; values
-that are commented out # serve to show the default. import os import shutil
-import sys # -- Path setup ----------------------------------------------------
----------- __location__ = os.path.dirname(__file__) # If extensions (or modules
-to document with autodoc) are in another directory, # add these directories to
+that are commented out # serve to show the default. import os import sys import
+shutil # -- Path setup --------------------------------------------------------
+------ __location__ = os.path.dirname(__file__) # If extensions (or modules to
+document with autodoc) are in another directory, # add these directories to
 sys.path here. If the directory is relative to the # documentation root, use
 os.path.abspath to make it absolute, like shown here. sys.path.insert(0,
 os.path.join(__location__, "../src")) # -- Run sphinx-apidoc ------------------
 ------------------------------------- # This hack is necessary since RTD does
 not issue `sphinx-apidoc` before running # `sphinx-build -b html . _build/
 html`. See Issue: # https://github.com/readthedocs/readthedocs.org/issues/1139
 # DON'T FORGET: Check the box "Install your project inside a virtualenv using #
@@ -18,75 +18,73 @@
 apidoc except ImportError: from sphinx import apidoc output_dir = os.path.join
 (__location__, "api") module_dir = os.path.join(__location__, "../src/
 comicgeeks") try: shutil.rmtree(output_dir) except FileNotFoundError: pass try:
 import sphinx cmd_line = f"sphinx-apidoc --implicit-namespaces -f -o
 {output_dir} {module_dir}" args = cmd_line.split(" ") if tuple
 (sphinx.__version__.split(".")) >= ("1", "7"): # This is a rudimentary
 parse_version to avoid external dependencies args = args[1:] apidoc.main(args)
-except Exception as e: print(f"Running `sphinx-apidoc` failed!\n{e}") # -
-- General configuration --------------------------------------------------- #
+except Exception as e: print("Running `sphinx-apidoc` failed!\n{}".format(e)) #
+-- General configuration --------------------------------------------------- #
 If your documentation needs a minimal Sphinx version, state it here. #
 needs_sphinx = '1.0' # Add any Sphinx extension module names here, as strings.
 They can be extensions # coming with Sphinx (named 'sphinx.ext.*') or your
 custom ones. extensions = [ "sphinx.ext.autodoc", "sphinx.ext.intersphinx",
 "sphinx.ext.todo", "sphinx.ext.autosummary", "sphinx.ext.viewcode",
 "sphinx.ext.coverage", "sphinx.ext.doctest", "sphinx.ext.ifconfig",
-"sphinx.ext.mathjax", "sphinx.ext.napoleon", "revitron_sphinx_theme", ] # Add
-any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"] # Enable markdown extensions.append
-("myst_parser") # Configure MyST-Parser myst_enable_extensions = [ "amsmath",
-"colon_fence", "deflist", "dollarmath", "html_image", "linkify",
-"replacements", "smartquotes", "substitution", "tasklist", ] # The suffix of
-source filenames. source_suffix = [".rst", ".md"] # The encoding of source
-files. # source_encoding = 'utf-8-sig' # The master toctree document.
-master_doc = "index" # General information about the project. project =
-"comicgeeks" version = "0.2.3" release = "0.2.3" author = "Pablo Ruiz"
-copyright = '2022 Pablo_Ruiz' language = "en" # The version info for the
-project you're documenting, acts as replacement for # |version| and |release|,
-also used in various other places throughout the # built documents. # #
-version: The short X.Y version. # release: The full version, including alpha/
-beta/rc tags. # If you donât need the separation provided between version and
-release, # just set them both to the same value. try: from comicgeeks import
-__version__ as version version = version.__version__ except ImportError:
-version = "" if not version or version.lower() == "unknown": version =
-os.getenv("READTHEDOCS_VERSION", "unknown") # automatically set by RTD release
-= version # The language for content autogenerated by Sphinx. Refer to
-documentation # for a list of supported languages. # language = None # There
-are two options for replacing |today|: either, you set today to some # non-
-false value, then it is used: # today = '' # Else, today_fmt is used as the
-format for a strftime call. # today_fmt = '%B %d, %Y' # List of patterns,
-relative to source directory, that match files and # directories to ignore when
-looking for source files. exclude_patterns = ["_build", "Thumbs.db",
-".DS_Store", ".venv"] # The reST default role (used for this markup: `text`) to
-use for all documents. # default_role = None # If true, '()' will be appended
-to :func: etc. cross-reference text. # add_function_parentheses = True # If
-true, the current module name will be prepended to all description # unit
-titles (such as .. function::). # add_module_names = True # If true,
-sectionauthor and moduleauthor directives will be shown in the # output. They
-are ignored by default. # show_authors = False # The name of the Pygments
-(syntax highlighting) style to use. pygments_style = "sphinx" # A list of
-ignored prefixes for module index sorting. # modindex_common_prefix = [] # If
-true, keep warnings as "system message" paragraphs in the built documents. #
-keep_warnings = False # If this is True, todo emits a warning for each TODO
-entries. The default is False. todo_emit_warnings = True # -- Options for HTML
-output ------------------------------------------------- # The theme to use for
-HTML and HTML Help pages. See the documentation for # a list of builtin themes.
-html_theme = "revitron_sphinx_theme" # Theme options are theme-specific and
-customize the look and feel of a theme # further. For a list of options
-available for each theme, see the # documentation. html_theme_options =
-{ "navigation_depth": 2, "github_url": "https://github.com/pruizlezcano/
-comicgeeks", "color_scheme": "blue", } html_context = { "landing_page":
-{ "menu": [ {"title": "Docs", "url": "get-started.html"}, {"title": "GitHub",
-"url": "https://github.com/pruizlezcano/comicgeeks"}, {"title": "â¡ Sponsor",
-"url": "#"}, ] } } # Add any paths that contain custom themes here, relative to
-this directory. # html_theme_path = [] # The name for this set of Sphinx
-documents. If None, it defaults to # " v documentation". # html_title = None #
-A shorter title for the navigation bar. Default is the same as html_title. #
-html_short_title = None # The name of an image file (relative to this
-directory) html_logo = "_static/icon.svg" # The name of an image file (within
+"sphinx.ext.mathjax", "sphinx.ext.napoleon", ] # Add any paths that contain
+templates here, relative to this directory. templates_path = ["_templates"] #
+Enable markdown extensions.append("myst_parser") # Configure MyST-Parser
+myst_enable_extensions = [ "amsmath", "colon_fence", "deflist", "dollarmath",
+"html_image", "linkify", "replacements", "smartquotes", "substitution",
+"tasklist", ] # The suffix of source filenames. source_suffix = [".rst", ".md"]
+# The encoding of source files. # source_encoding = 'utf-8-sig' # The master
+toctree document. master_doc = "index" # General information about the project.
+project = "comicgeeks" author = "Pablo Ruiz" copyright = '2022 Pablo_Ruiz' #
+The version info for the project you're documenting, acts as replacement for #
+|version| and |release|, also used in various other places throughout the #
+built documents. # # version: The short X.Y version. # release: The full
+version, including alpha/beta/rc tags. # If you donât need the separation
+provided between version and release, # just set them both to the same value.
+try: from comicgeeks import __version__ as version except ImportError: version
+= "" if not version or version.lower() == "unknown": version = os.getenv
+("READTHEDOCS_VERSION", "unknown") # automatically set by RTD release = version
+# The language for content autogenerated by Sphinx. Refer to documentation #
+for a list of supported languages. # language = None # There are two options
+for replacing |today|: either, you set today to some # non-false value, then it
+is used: # today = '' # Else, today_fmt is used as the format for a strftime
+call. # today_fmt = '%B %d, %Y' # List of patterns, relative to source
+directory, that match files and # directories to ignore when looking for source
+files. exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".venv"] # The
+reST default role (used for this markup: `text`) to use for all documents. #
+default_role = None # If true, '()' will be appended to :func: etc. cross-
+reference text. # add_function_parentheses = True # If true, the current module
+name will be prepended to all description # unit titles (such as .. function::
+). # add_module_names = True # If true, sectionauthor and moduleauthor
+directives will be shown in the # output. They are ignored by default. #
+show_authors = False # The name of the Pygments (syntax highlighting) style to
+use. pygments_style = "sphinx" # A list of ignored prefixes for module index
+sorting. # modindex_common_prefix = [] # If true, keep warnings as "system
+message" paragraphs in the built documents. # keep_warnings = False # If this
+is True, todo emits a warning for each TODO entries. The default is False.
+todo_emit_warnings = True # -- Options for HTML output ------------------------
+------------------------- # The theme to use for HTML and HTML Help pages. See
+the documentation for # a list of builtin themes. html_theme =
+"revitron_sphinx_theme" # Theme options are theme-specific and customize the
+look and feel of a theme # further. For a list of options available for each
+theme, see the # documentation. html_theme_options = { "navigation_depth": 2,
+"github_url": "https://github.com/pruizlezcano/comicgeeks", "color_scheme":
+"blue", } html_context = { "landing_page": { "menu": [ {"title": "Docs", "url":
+"get-started.html"}, {"title": "GitHub", "url": "https://github.com/
+pruizlezcano/comicgeeks"}, {"title": "â¡ Sponsor", "url": "#"}, ] } } # Add
+any paths that contain custom themes here, relative to this directory. #
+html_theme_path = [] # The name for this set of Sphinx documents. If None, it
+defaults to # " v documentation". # html_title = None # A shorter title for the
+navigation bar. Default is the same as html_title. # html_short_title = None #
+The name of an image file (relative to this directory) to place at the top # of
+the sidebar. html_logo = "_static/icon.svg" # The name of an image file (within
 the static path) to use as favicon of the # docs. This file should be a Windows
 icon file (.ico) being 16x16 or 32x32 # pixels large. # html_favicon = None #
 Add any paths that contain custom static files (such as style sheets) here, #
 relative to this directory. They are copied after the builtin static files, #
 so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"] # If not '', a 'Last updated on:' timestamp is
 inserted at every page bottom, # using the given strftime format. #
@@ -111,25 +109,25 @@
 ("custom.js") # -- Options for LaTeX output -----------------------------------
 ------------- latex_elements = { # The paper size ("letterpaper" or "a4paper").
 # "papersize": "letterpaper", # The font size ("10pt", "11pt" or "12pt"). #
 "pointsize": "10pt", # Additional stuff for the LaTeX preamble. # "preamble":
 "", } # Grouping the document tree into LaTeX files. List of tuples # (source
 start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [ ("index", "user_guide.tex", "comicgeeks Documentation",
-"Pablo", "manual") ] # The name of an image file (relative to this directory)
-to place at the top of # the title page. # latex_logo = "" # For "manual"
-documents, if this is true, then toplevel headings are parts, # not chapters. #
-latex_use_parts = False # If true, show page references after internal links. #
-latex_show_pagerefs = False # If true, show URL addresses after external links.
-# latex_show_urls = False # Documents to append as an appendix to all manuals.
-# latex_appendices = [] # If false, no module index is generated. #
-latex_domain_indices = True # -- External mapping -----------------------------
---------------------------- python_version = ".".join(map(str, sys.version_info
-[0:2])) intersphinx_mapping = { "sphinx": ("https://www.sphinx-doc.org/en/
-master", None), "python": ("https://docs.python.org/" + python_version, None),
-"matplotlib": ("https://matplotlib.org", None), "numpy": ("https://numpy.org/
-doc/stable", None), "sklearn": ("https://scikit-learn.org/stable", None),
-"pandas": ("https://pandas.pydata.org/pandas-docs/stable", None), "scipy":
-("https://docs.scipy.org/doc/scipy/reference", None), "setuptools": ("https://
-setuptools.pypa.io/en/stable/", None), "pyscaffold": ("https://pyscaffold.org/
-en/stable", None), } print(f"loading configurations for {project} {version}
-...", file=sys.stderr)
+"Pablo Ruiz", "manual") ] # The name of an image file (relative to this
+directory) to place at the top of # the title page. # latex_logo = "" # For
+"manual" documents, if this is true, then toplevel headings are parts, # not
+chapters. # latex_use_parts = False # If true, show page references after
+internal links. # latex_show_pagerefs = False # If true, show URL addresses
+after external links. # latex_show_urls = False # Documents to append as an
+appendix to all manuals. # latex_appendices = [] # If false, no module index is
+generated. # latex_domain_indices = True # -- External mapping ----------------
+---------------------------------------- python_version = ".".join(map(str,
+sys.version_info[0:2])) intersphinx_mapping = { "sphinx": ("https://www.sphinx-
+doc.org/en/master", None), "python": ("https://docs.python.org/" +
+python_version, None), "matplotlib": ("https://matplotlib.org", None), "numpy":
+("https://numpy.org/doc/stable", None), "sklearn": ("https://scikit-learn.org/
+stable", None), "pandas": ("https://pandas.pydata.org/pandas-docs/stable",
+None), "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
+"setuptools": ("https://setuptools.pypa.io/en/stable/", None), "pyscaffold":
+("https://pyscaffold.org/en/stable", None), } print(f"loading configurations
+for {project} {version} ...", file=sys.stderr)
```

### Comparing `comicgeeks-0.2.3/docs/examples.md` & `comicgeeks-0.3.0/docs/examples.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```python
 from comicgeeks import Comic_Geeks
 
 comic_geeks = Comic_Geeks()
 series = comic_geeks.search_series("Daredevil")
 ```
 
-```{admonition} Return
+````{admonition} Return
 ```{eval-rst}
   .. code-block:: none
 
     [
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
@@ -25,26 +25,26 @@
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
       94 more...
     ]
 
-```
+````
 
 ### Search creator
 
 ```python
 from comicgeeks import Comic_Geeks
 
 client = Comic_Geeks()
 creators = client.search_creator("Chip")
 ```
 
-```{admonition} Return
+````{admonition} Return
 ```{eval-rst}
    .. code-block:: none
 
     [
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
@@ -53,25 +53,26 @@
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
       <Series object at 0x00000...>,
       94 more...
     ]
-```
+````
 
 ### Search character
+
 ```python
 from comicgeeks import Comic_Geeks
 
 client = Comic_Geeks()
 characters = client.search_character("Spider-man")
 ```
 
-```{admonition} Return
+````{admonition} Return
 ```{eval-rst}
    .. code-block:: none
 
     [
       <Character object at 0x00000...>,
       <Character object at 0x00000...>,
       <Character object at 0x00000...>,
@@ -80,26 +81,26 @@
       <Character object at 0x00000...>,
       <Character object at 0x00000...>,
       <Character object at 0x00000...>,
       <Character object at 0x00000...>,
       <Character object at 0x00000...>,
       40 more...
     ]
-```
+````
 
 ### Get new releases
 
 ```python
 from comicgeeks import Comic_Geeks
 
 client = Comic_Geeks()
 issues = client.new_releases()
 ```
 
-```{admonition} Return
+````{admonition} Return
 ```{eval-rst}
    .. code-block:: none
 
     [
       <Issue object at 0x00000...>,
       <Issue object at 0x00000...>,
       <Issue object at 0x00000...>,
@@ -108,28 +109,28 @@
       <Issue object at 0x00000...>,
       <Issue object at 0x00000...>,
       <Issue object at 0x00000...>,
       <Issue object at 0x00000...>,
       <Issue object at 0x00000...>,
       73 more...
     ]
-```
+````
 
 ## Get by id
 
 ### Get series
 
 ```python
 from comicgeeks import Comic_Geeks
 
 client = Comic_Geeks()
 series = client.series_info(150065)
 ```
 
-```{admonition} Return
+````{admonition} Return
 ```{eval-rst}
    .. code-block:: json
 
     {
       "series_id": 150065,
       "name": "Beta Ray Bill",
       "publisher": "Marvel Comics",
@@ -140,34 +141,38 @@
           "<Issue object at 0x00000..>",
           "<Issue object at 0x00000..>",
           "<Issue object at 0x00000..>",
           "<Issue object at 0x00000..>",
           "<Issue object at 0x00000..>"
       ],
       "issue_count": 5,
+      "trade_paperbacks": [
+          "<Trade_Paperback object at 0x00000..>",
+      ],
+      "trade_paperback_count": 1,
       "url": "/comics/series/150065/beta-ray-bill",
       "cover": "https://s3.amazonaws.com/comicgeeks/series/150065.jpg?1619183332",
       "user": { // Only valid if ci_session is provided
         "pull": "None",
         "owned": "None",
         "read": "None"
       }
     }
-```
+````
 
 ### Get issue
 
 ```python
 from comicgeeks import Comic_Geeks
 
 client = Comic_Geeks()
 issue = client.issue_info(3616996)
 ```
 
-```{admonition} Return
+````{admonition} Return
 ```{eval-rst}
    .. code-block:: json
 
     {
       "issue_id": 3616996,
       "character_credits": [
         "<classes.Character object at 0x00000...>",
@@ -278,26 +283,26 @@
         "pull": "None",
         "collect": "None",
         "readlist": "None",
         "wishlist": "None",
         "rating": "None"
       }
     }
-```
+````
 
 ### Get creator
 
 ```python
 from comicgeeks import Comic_Geeks
 
 client = Comic_Geeks()
 creator = client.creator_info(6209)
 ```
 
-```{admonition} Return
+````{admonition} Return
 ```{eval-rst}
    .. code-block:: json
 
     {
       "characters": [
         "<classes.Character object at 0x00000...>",
         "<classes.Character object at 0x00000...>",
@@ -318,25 +323,26 @@
       "description": "Steve Murray (better known under the pen name of Chip Zdarsky) is a Canadian comic book creator most known for his work with Matt Fraction in Sex Criminals\xa0as the artist and his books at Marvel such as Daredevil, The Spectacular Spider-Man and Howard the Duck.",
       "image": "https://s3.amazonaws.com/comicgeeks/people/avatars/6209.jpg?t=1604083961", "name": "Chip Zdarsky",
       "url": "/people/6209/chip-zdarsky",
       "read": "None", // Only valid if ci_session is provided
       "owned": "None", // Only valid if ci_session is provided
       "issue_count": 378
     }
-```
+````
 
 ### Get character
+
 ```python
 from comicgeeks import Comic_Geeks
 
 client = Comic_Geeks()
 character = client.creator_info(6209)
 ```
 
-```{admonition} Return
+````{admonition} Return
 ```{eval-rst}
   .. code-block:: json
 
     {
       "character_id": 11699,
       "image": "https://s3.amazonaws.com/comicgeeks/characters/avatars/11699.jpg?t=1608688306",
       "creators": [
@@ -371,8 +377,8 @@
       "name": "Daredevil",
       "real_name": "Elektra Natchios",
       "url": "/character/11699/daredevil",
       "read": "None", // Only valid if ci_session is provided
       "owned": "None", // Only valid if ci_session is provided
       "issue_count": 37
     }
-```
+````
```

### Comparing `comicgeeks-0.2.3/docs/get-started.md` & `comicgeeks-0.3.0/docs/get-started.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 # Getting started
 
 ## Installation
 
-Install the package (or add it to your ``requirements.txt`` file):
+Install the package (or add it to your `requirements.txt` file):
 
 ```console
 $ pip install comicgeeks
 ```
 
-## Getting cookie session
+## Login
 
-In order to use some of the package functions, you will need to provide a valid cookie session.
+In order to use some of the package functions, you will need to provide a valid cookie session or login with your user and password.
 To do that, follow this steps:
 
+### Using cookie session
+
 1. Login into [League of Comics Geeks ](https://leagueofcomicgeeks.com/)
 2. Open you browser's dev tools and search for the `ci_session` cookie
 3. Use the cookie value to create a session when calling the package class `Comic_Geeks(ci_session)`
 
+### Using user and password
+
+Use the `login` method to login into your account and get a valid cookie session.
+
+```python
+from Comic_Geeks import Comic_Geeks
+client = Comic_Geeks()
+client.login("user", "password")
+```
+
 ## Usage
 
 ```python
 from comicgeeks import Comic_Geeks
 
+# login to your account
 client = Comic_Geeks("mycisession")
+# or
+client = Comic_Geeks()
+client.login("user", "password")
 
 # search series
 client.search_series("daredevil")
 
 # get new releases
 client.new_releases()
```

### Comparing `comicgeeks-0.2.3/docs/index.rst` & `comicgeeks-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/docs/modules.rst` & `comicgeeks-0.3.0/docs/modules.rst`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,22 @@
 ======
 
 .. autoclass:: comicgeeks.classes.Issue
    :members:
    :no-undoc-members:
    :show-inheritance:
 
+Trade Paperback
+================
+
+.. autoclass:: comicgeeks.classes.Trade_Paperback
+   :members:
+   :no-undoc-members:
+   :show-inheritance:
+
 Series
 =======
 
 .. autoclass:: comicgeeks.classes.Series
    :members:
    :no-undoc-members:
    :show-inheritance:
```

### Comparing `comicgeeks-0.2.3/setup.cfg` & `comicgeeks-0.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -105,12 +105,13 @@
 00000680: 6465 203d 200d 0a09 2e74 6f78 0d0a 0962  de = ....tox...b
 00000690: 7569 6c64 0d0a 0964 6973 740d 0a09 2e65  uild...dist....e
 000006a0: 6767 730d 0a09 646f 6373 2f63 6f6e 662e  ggs...docs/conf.
 000006b0: 7079 0d0a 0d0a 5b70 7973 6361 6666 6f6c  py....[pyscaffol
 000006c0: 645d 0d0a 7665 7273 696f 6e20 3d20 342e  d]..version = 4.
 000006d0: 330d 0a70 6163 6b61 6765 203d 2063 6f6d  3..package = com
 000006e0: 6963 6765 656b 730d 0a65 7874 656e 7369  icgeeks..extensi
-000006f0: 6f6e 7320 3d20 0d0a 096d 6172 6b64 6f77  ons = ...markdow
-00000700: 6e0d 0a09 7072 655f 636f 6d6d 6974 0d0a  n...pre_commit..
-00000710: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000720: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000730: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+000006f0: 6f6e 7320 3d20 0d0a 0967 6974 6875 625f  ons = ...github_
+00000700: 6163 7469 6f6e 730d 0a09 6d61 726b 646f  actions...markdo
+00000710: 776e 0d0a 0970 7265 5f63 6f6d 6d69 740d  wn...pre_commit.
+00000720: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000730: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000740: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `comicgeeks-0.2.3/setup.py` & `comicgeeks-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/src/comicgeeks/Comic_Geeks.py` & `comicgeeks-0.3.0/src/comicgeeks/Comic_Geeks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,136 @@
 from datetime import datetime
+from typing import Union
 
 import requests
 from bs4 import BeautifulSoup
 
-from .classes import Character, Creator, Issue, Series
-from .utils import get_series
-
-_headers = {
-    "User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:20.0) Gecko/20100101 Firefox/20.0"
-}
+from comicgeeks.classes import Character, Creator, Issue, Series, Trade_Paperback
+from comicgeeks.utils import get_series, is_trade_paperback
 
 
 class Comic_Geeks:
     """League of Comic Geeks client
 
     Attributes:
         ci_session (str): Cookie ci_session of League of Comic Geeks
     """
 
     def __init__(self, ci_session: str = None) -> None:
-        self._ci_session: str = self._check_session(ci_session)
+        self._session = requests.Session()
+        self._session.headers.update(
+            {
+                "User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:20.0) Gecko/20100101 Firefox/20.0"
+            }
+        )
+        self._session.authenticated = False
+        self._session.authenticated = False
+        if self._validate_session(ci_session):
+            self._session.authenticated = True
+
+    def login(self, username: str, password: str) -> bool:
+        """Login to League of Comic Geeks
 
-    def _check_session(self, ci_session: str = None) -> bool:
+        Args:
+            username (str): Username
+            password (str): Password
+
+        Returns:
+            str: ci_session cookie
+        """
+        url = "https://leagueofcomicgeeks.com/login"
+        r = self._session.post(url, data={"username": username, "password": password})
+        r.raise_for_status()
+        ci_session = self._validate_session(r.cookies.get("ci_session"))
+        if ci_session:
+            self._session.authenticated = True
+            return True
+        else:
+            self._session.authenticated = False
+            return False
+
+    def _validate_session(self, ci_session: str = None) -> bool:
         """Check if session is valid.
         Make a request to the main page and if is redirected to the dashboard, the session is valid.
         """
-        if ci_session is None:
-            return ""
-        s = requests.Session()
-        s.cookies.update({"ci_session": ci_session})
-        r = s.get("https://leagueofcomicgeeks.com/", headers=_headers)
+        if ci_session is None or ci_session == "":
+            return False
+        r = self._session.get(
+            "https://leagueofcomicgeeks.com/", cookies={"ci_session": ci_session}
+        )
+        r.raise_for_status()
         if "dashboard" in r.url:
-            return ci_session
-        return ""
+            return True
+        self._session.cookies.clear()  # Clear invalid ci_session
+        return False
 
     def search_series(self, query: str) -> list[Series]:
         """Search series by name
 
         Args:
             query (str): Series name
 
         Returns:
             list (Series): List of series
         """
         query = query.strip().lower().replace(" ", "+")
         url = f"https://leagueofcomicgeeks.com/comic/get_comics?&list=search&list_option=series&view=thumbs&title={query}&order=alpha-asc&format[]=1&format[]=6"
-        r = requests.get(url, headers=_headers)
+        r = self._session.get(url)
         r.raise_for_status()
         r = r.json()
         if r["count"] == 0:
             return []
 
         soup = BeautifulSoup(r["list"], features="lxml")
         content = soup.find(id="comic-list-block")
         comics = content.find_all("li")
-        data = get_series(comics, Series, self._ci_session)
+        data = get_series(comics, Series, self._session)
         return data
 
     def search_creator(self, query: str) -> list[Creator]:
         """Search series by name
 
         Args:
             query (str): Series name
 
         Returns:
             list (Series): List of series
         """
         query = query.strip().lower().replace(" ", "+")
         url = f"https://leagueofcomicgeeks.com/search/creators?keyword={query}"
-        r = requests.get(url, headers=_headers)
+        r = self._session.get(url)
         r.raise_for_status()
         soup = BeautifulSoup(r.content, features="lxml")
         content = soup.find(class_="comic-series-thumb-list")
         if content is None:
             return []
         data = []
         for item in content.findAll("li"):
             creator_id = int(item.find("a")["href"].split("/")[2])
-            creator = Creator(creator_id, self._ci_session)
+            creator = Creator(creator_id, self._session)
             creator.name = item.find(class_="title").text.strip()
             creator.url = item.find("a")["href"]
             if item.find("img"):
                 creator.image = item.find("img")["src"]
             data.append(creator)
         return data
 
     def search_character(self, query: str) -> list[Character]:
         query = query.strip().lower().replace(" ", "+")
         url = f"https://leagueofcomicgeeks.com/search/characters?keyword={query}"
-        r = requests.get(url, headers=_headers)
+        r = self._session.get(url)
         r.raise_for_status()
         soup = BeautifulSoup(r.content, features="lxml")
         content = soup.find(class_="character-thumb-list")
         if content is None:
             return []
         data = []
         for item in content.findAll("li"):
             character_id = int(item.find("a")["href"].split("/")[2])
-            character = Character(character_id, self._ci_session)
+            character = Character(character_id, self._session)
             character.name = item.find(class_="title").text.strip()
             character.url = item.find("a")["href"]
             character.real_name = (
                 item.find(class_="publisher").text.strip()
                 if item.find(class_="publisher")
                 else ""
             )
@@ -124,15 +153,15 @@
             list (Issue): List of issues
         """
         if date == "now":
             date = datetime.now()
         date = f"{date.month}/{date.day}/{date.year}"
 
         url = f"https://leagueofcomicgeeks.com/comic/get_comics?list=releases&view=thumbs&format[]=1%2C6&date_type=week&date={date}&order=pulls"
-        r = requests.get(url, headers=_headers).json()
+        r = self._session.get(url).json()
         if r["count"] == 0:
             return []
 
         soup = BeautifulSoup(r["list"], features="lxml")
         content = soup.find(id="comic-list-block")
         comics = content.find_all("li")
         data = []
@@ -151,15 +180,15 @@
             store_date = comic.find(class_="date")["data-date"]
             publisher = comic.find(class_="publisher").text.strip()
             cover = comic.find("img")["data-src"]
             community = {"rating": rating, "pull": pulls}
 
             issue = Issue(
                 issue_id=issue_id,
-                ci_session=self._ci_session,
+                session=self._session,
             )
 
             issue.name = name
             issue.url = url
             issue.store_date = store_date
             issue.price = price
             issue.publisher = publisher
@@ -173,41 +202,43 @@
 
         Args:
             series_id (int): series id
 
         Returns:
             Series: Series class
         """
-        return Series(series_id, self._ci_session)
+        return Series(series_id, self._session)
 
-    def issue_info(self, issue_id: int) -> Issue:
+    def issue_info(self, issue_id: int) -> Union[Issue, Trade_Paperback]:
         """Get issue info by id
 
         Args:
             issue_id (int): issue id
 
         Returns:
-            Issue: Issue object
+            Issue | Trade_Paperback: Issue object
         """
-        return Issue(issue_id, self._ci_session)
+        if is_trade_paperback(issue_id):
+            return Trade_Paperback(issue_id, self._session)
+        return Issue(issue_id, self._session)
 
     def creator_info(self, creator_id: int) -> Creator:
         """Get creator info by id
 
         Args:
             creator_id (int): creator id
 
         Returns:
             Creator: Creator object
         """
-        return Creator(creator_id, self._ci_session)
+        return Creator(creator_id, self._session)
 
     def character_info(self, character_id: int) -> Character:
         """Get character info by id
 
         Args:
             character_id (int): character id
 
         Returns:
             Character: Character object
         """
-        return Character(character_id, self._ci_session)
+        return Character(character_id, self._session)
```

### Comparing `comicgeeks-0.2.3/src/comicgeeks/classes.py` & `comicgeeks-0.3.0/src/comicgeeks/classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,85 @@
 # Sorry, but due to circular imports, all of this must be in the same file
 # Please, make a pull request if you know how to fix it
 
 import datetime
-
+import re
 import requests
 from bs4 import BeautifulSoup
 
-from .extract import extract
-from .utils import get_characters, get_series
+from comicgeeks.extract import extract
+from comicgeeks.utils import get_characters, get_series
+
+
+class Issue:
+    None
+
 
-_headers = {
-    "User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:20.0) Gecko/20100101 Firefox/20.0"
-}
+class Trade_Paperback:
+    None
 
 
 class Series:
     """ComicGeeks Series class"""
 
-    def __init__(self, series_id: int, ci_session: str = None):
-        self._ci_session = ci_session
+    def __init__(self, series_id: int, session: requests.Session):
+        self._session = session
         self._series_id = series_id
         self._name = None
         self._publisher = None
         self._description = None
         self._start_year = None
         self._end_year = None
         self._issues = None
         self._issue_count = None
+        self._trade_paperbacks = None
+        self._trade_paperback_count = None
         self._url = None
         self._cover = None
         self._user = {"pull": None, "owned": None, "read": None}
-        self._session = requests.Session()
-        self._session.cookies.update({"ci_session": ci_session})
 
     @property
     def user(self) -> dict:
         """Dictionary with user data
 
         Parameters:
             pull (bool) : Is the series in the pull list?,
             owned (str) : Is the issue in the collection?,
             read (str) : Is the issue in the read list?
         """
         if (
             self._user["pull"] is None
             or self._user["owned"] is None
             or self._user["read"] is None
-        ) and self._ci_session:
+        ) and self._session.authenticated:
             self._get_data()
         return self._user
 
     @property
     def series_id(self) -> int:
         """Series id"""
         if self._series_id is None:
             self._get_data()
         return self._series_id
 
     @property
-    def issues(self) -> list:
+    def issues(self) -> list[Issue]:
         """List of issues of the series"""
         if self._issues is None:
             self._get_data()
         return self._issues
 
     @property
+    def trade_paperbacks(self) -> list[Trade_Paperback]:
+        """List of trade paperbacks of the series"""
+        if self._trade_paperbacks is None:
+            self._get_data()
+        return self._trade_paperbacks
+
+    @property
     def description(self) -> str:
         """Series description"""
         if self._description is None:
             self._get_data()
         return self._description
 
     @property
@@ -144,18 +155,29 @@
             self._get_data()
         return self._issue_count
 
     @issue_count.setter
     def issue_count(self, value):
         self._issue_count = value
 
+    @property
+    def trade_paperback_count(self) -> int:
+        """Number of trade paperbacks"""
+        if self._trade_paperback_count is None:
+            self._get_data()
+        return self._trade_paperback_count
+
+    @trade_paperback_count.setter
+    def trade_paperback_count(self, value):
+        self._trade_paperback_count = value
+
     def _get_data(self):
         """Get series info"""
         url = f"https://leagueofcomicgeeks.com/comic/get_comics?&list=search&view=thumbs&format[]=1&series_id={self._series_id}&character=0&order=date-desc"
-        r = self._session.get(url, headers=_headers)
+        r = self._session.get(url)
         r.raise_for_status()
         r = r.json()
         if r["count"] == 0:
             raise Exception("No series found")
         soup = BeautifulSoup(r["list"], features="lxml")
         header = BeautifulSoup(r["header"], features="lxml")
         statbar = BeautifulSoup(r["statbar"], features="lxml")
@@ -167,15 +189,15 @@
         issues = []
         for issue in content.find_all("li"):
             title = issue.find(class_="title").text.strip()
             name, number, volume = extract(title)
             issue_id = int(issue.find("a")["href"].split("/")[2])
             i = Issue(
                 issue_id=issue_id,
-                ci_session=self._ci_session,
+                session=self._session,
             )
 
             i.name = title
             i.url = url
             i.store_date = issue.find(class_="date")["data-date"]
             i.price = (
                 float(issue.find(class_="price").text.split("·")[1].strip()[1::])
@@ -202,32 +224,86 @@
                 else False,
                 "rating": int(issue["data-rating"])
                 if "data-rating" in issue
                 else "Unknown",
             }
             issues.append(i)
 
+        url = f"https://leagueofcomicgeeks.com/comic/get_comics?&list=search&view=thumbs&format[]=3&series_id={self._series_id}&character=0&order=date-desc"
+        r = self._session.get(url)
+        r.raise_for_status()
+        r = r.json()
+        if r["count"] == 0:
+            raise Exception("No series found")
+        soup = BeautifulSoup(r["list"], features="lxml")
+        content = soup.find(id="comic-list-issues")
+
+        trade_paperbacks = []
+        for issue in content.find_all("li"):
+            title = issue.find(class_="title").text.strip()
+            number = re.findall(r"\d+", title)
+            number = number[-1] if number else 1
+            issue_id = int(issue.find("a")["href"].split("/")[2])
+            i = Trade_Paperback(
+                issue_id=issue_id,
+                session=self._session,
+            )
+
+            i.name = title
+            i.url = url
+            i.store_date = issue.find(class_="date")["data-date"]
+            i.price = (
+                float(issue.find(class_="price").text.split("·")[1].strip()[1::])
+                if issue.find(class_="price")
+                else "Unknown"
+            )
+            i.publisher = r["series"]["publisher_name"]
+            i.cover = issue.find("img")["data-src"]
+            i.number = str(number) if number else ""
+            comic_controller = issue.findAll(class_="comic-controller")
+            i.user = {
+                "pull": True if "active" in comic_controller[0]["class"] else False,
+                "collect": True
+                if len(comic_controller) >= 2
+                and "active" in comic_controller[1]["class"]
+                else False,
+                "readlist": True
+                if len(comic_controller) >= 3
+                and "active" in comic_controller[2]["class"]
+                else False,
+                "wishlist": True
+                if len(comic_controller) >= 4
+                and "active" in comic_controller[3]["class"]
+                else False,
+                "rating": int(issue["data-rating"])
+                if "data-rating" in issue
+                else "Unknown",
+            }
+            trade_paperbacks.append(i)
+
         self._name = r["series"]["title"]
         self._publisher = r["series"]["publisher_name"]
         self._description = BeautifulSoup(
             r["series"]["description"], features="lxml"
         ).text
         self._start_year = int(begin.strip()) if begin else 0
         self._end_year = int(end.strip()) if end and end.strip() != "Present" else 0
-        self._issues = sorted(issues, key=lambda x: int(x.number))
+        self._issues = sorted(issues, key=lambda x: float(x.number))
         self._issue_count = len(issues)
+        self._trade_paperbacks = sorted(trade_paperbacks, key=lambda x: float(x.number))
+        self._trade_paperback_count = len(trade_paperbacks)
         self._url = header.find(class_="dropdown-item")["href"].split(
             "/submit-new-issue"
         )[0]
         self._cover = (
             header.find(class_="cover")["style"].split("'")[1]
             if header.find(class_="cover")
             else "#"
         )
-        if self._ci_session:
+        if self._session.authenticated:
             self._user["pull"] = True if statbar.find(class_="btn-remove") else False
             stats = statbar.findAll(class_="comic-score")
             if stats:
                 self._user["owned"] = int(
                     stats[0]
                     .find(class_="text")
                     .text.strip()
@@ -251,265 +327,262 @@
 
     def pull(self) -> dict:
         """Pull series
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 1,
             "action": "subscribe",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def unsubscribe(self) -> dict:
         """Unsubscribe series
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 1,
             "action": "unsubscribe",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def pull_tp(self) -> dict:
         """Pull only trade paperback issues
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 1,
             "action": "subscribetp",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def pull_hc(self) -> dict:
         """Pull only hard cover issues
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 1,
             "action": "subscribehc",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def add_to_collection(self) -> dict:
         """Add series to collection
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 2,
             "action": "add",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def add_to_wishlist(self) -> dict:
         """Add series to wishlist
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 3,
             "action": "add",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def add_missing_to_wishlist(self) -> dict:
         """Add missing issues to wishlist
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
 
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 3,
             "action": "addnotowned",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def mark_read(self) -> dict:
         """Mark series as read
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 5,
             "action": "addall",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def mark_owned_read(self) -> dict:
         """Mark owned issues as read
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 5,
             "action": "addowned",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def remove_from_collection(self) -> dict:
         """Remove series from collection
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 2,
             "action": "remove",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def remove_from_wishlist(self) -> dict:
         """Remove series from wishlist
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 3,
             "action": "remove",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def remove_from_readlist(self) -> dict:
         """Mark series as unread
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_bulk"
         data = {
             "series_id": self._series_id,
             "list_id": 5,
             "action": "remove",
             "date": "",
             "date_type": "",
         }
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def json(self) -> dict:
         """Return data in json format"""
         return {
             "series_id": self._series_id,
             "name": self.name,
             "publisher": self.publisher,
             "description": self.description,
             "start_year": self.start_year,
             "end_year": self.end_year,
             "issues": self.issues,
             "issue_count": self.issue_count,
+            "trade_paperbacks": self.trade_paperbacks,
+            "trade_paperback_count": self.trade_paperback_count,
             "url": self.url,
             "cover": self.cover,
             "user": self.user,
         }
 
 
 class Issue:
     """ComicGeeks Issue class"""
 
-    def __init__(
-        self,
-        issue_id: int,
-        ci_session: str = None,
-    ):
-        self._ci_session = ci_session
+    def __init__(self, issue_id: int, session: requests.Session):
         self._issue_id = issue_id
-
+        self._session = session
         self._characters = None
         self._cover = None
         self._community = {
             "pull": None,
             "collect": None,
             "readlist": None,
             "wishlist": None,
@@ -529,16 +602,14 @@
         self._person_credits = None
         self._price = None
         self._publisher = None
         self._series_pagination = None
         self._store_date = None
         self._url = None
         self._variant_covers = None
-        self._session = requests.Session()
-        self._session.cookies.update({"ci_session": ci_session})
 
     @property
     def characters(self) -> list:
         """List of characters that appear in this issue"""
         if self._characters is None:
             self._get_data()
         return self._characters
@@ -568,15 +639,15 @@
         """
         if (
             self._user["pull"] is None
             or self._user["collect"] is None
             or self._user["readlist"] is None
             or self._user["wishlist"] is None
             or self._user["rating"] is None
-        ) and self._ci_session:
+        ) and self._session.authenticated:
             self._get_data()
         return self._user
 
     @user.setter
     def user(self, value):
         self._user = value
 
@@ -734,17 +805,16 @@
         """List of variant covers"""
         if self._variant_covers is None:
             self._get_data()
         return self._variant_covers
 
     def _get_data(self):
         """Get series info"""
-
         url = f"https://leagueofcomicgeeks.com/comic/{self.issue_id}/foo"
-        r = self._session.get(url, headers=_headers)
+        r = self._session.get(url)
         r.raise_for_status()
         soup = BeautifulSoup(r.content, features="lxml")
         year, month, day = list(
             map(
                 int,
                 soup.find(class_="header-intro")
                 .find_all("a")[1]["href"]
@@ -764,26 +834,26 @@
         creators = comic.find(id="creators")
         person_credits = []
         if creators:
             creators = creators.find_all(class_="row")[1].find_all(class_="row")
             for creator in creators:
                 creator_url = creator.find("a")["href"]
                 creator_id = creator_url.split("/")[2]
-                c = Creator(creator_id, self._ci_session)
+                c = Creator(creator_id, self._session)
                 c.url = creator_url
                 c.name = creator.find(class_="name").text.strip()
                 person_credits.append(
                     {
                         "role": creator.find(class_="role").text.strip().lower(),
                         "Creator": c,
                     }
                 )
 
         characters = comic.find(id="characters")
-        characters_credits = get_characters(characters, Character, self._ci_session)
+        characters_credits = get_characters(characters, Character, self._session)
 
         covers = []
         cover = comic.find(class_="cover-art")
         covers.append(
             {
                 "name": cover.find("img")["alt"],
                 "image": cover.find("img")["src"],
@@ -799,25 +869,28 @@
                         "url": variant.find("a")["href"],
                         "image": img["data-src"] if "data-src" in img else "#",
                     }
                 )
         pagination = comic.find(class_="series-pagination")
         series_pagination = {
             "prev": Issue(
-                pagination.find(class_="prev")["href"].split("/")[2], self._ci_session
+                pagination.find(class_="prev")["href"].split("/")[2],
+                self._session,
             )
             if pagination.find(class_="prev")["href"] != "#"
             else None,
             "series": Series(
-                pagination.find(class_="series")["href"].split("/")[3], self._ci_session
+                pagination.find(class_="series")["href"].split("/")[3],
+                self._session,
             )
             if pagination.find(class_="series")["href"] != "#"
             else None,
             "next": Issue(
-                pagination.find(class_="next")["href"].split("/")[2], self._ci_session
+                pagination.find(class_="next")["href"].split("/")[2],
+                self._session,
             )
             if pagination.find(class_="next")["href"] != "#"
             else None,
         }
         counters = comic.findAll("span", class_="ml-1")
         counters_data = {}
         for counter in counters:
@@ -828,20 +901,20 @@
 
         counters_data["rating"] = soup.find(class_="percentage")
         if counters_data["rating"] is not None:
             counters_data["rating"] = counters_data["rating"].text.strip()
 
         title = soup.find("h1").text.strip()
         name, number, volume = extract(title)
+        if type(self).__name__ == "Trade_Paperback":
+            number = re.findall(r"\d+", title)[0]
 
         description: BeautifulSoup = comic.find(class_="listing-description")
-        if description.find("h3"):
-            name: str = description.find("h3").text.strip()
-        elif description.find("h4"):
-            name: str = description.find("h4").text.strip()
+        if comic.find(class_="story-title"):
+            name: str = comic.find(class_="story-title").text.strip()
         else:
             name: str = title
         self._name = name.title()
         self._number = str(number) if number else ""
         self._publisher = soup.find(class_="header-intro").find("a").text.strip()
         self._store_date = int(datetime.datetime(year, month, day).timestamp())
         self._description = description.text.strip()
@@ -877,15 +950,15 @@
             and counters_data["rating"] is not None
             and counters_data["rating"] != "TBD"
             else "Unknown"
         )
         self._price = price
         self._url = "/" + "/".join(r.url.split("/")[3:])
 
-        if self._ci_session:
+        if self._session.authenticated:
             counters = soup.findAll(class_="comic-controller")[1:]
             self._user["pull"] = True if "active" in counters[0]["class"] else False
             self._user["collect"] = (
                 True
                 if len(counters) >= 2 and "active" in counters[1]["class"]
                 else False
             )
@@ -901,140 +974,150 @@
             )
             rate = soup.find(class_="rateit")
             self._user["rating"] = (
                 int(rate["data-rateit-value"])
                 if rate and "data-rateit-value" in rate
                 else "Unknown"
             )
+        if type(self).__name__ == "Trade_Paperback":
+            collects = soup.find("section", id="collected-issues-list")
+            if collects:
+                collects = collects.find_all("li")
+                self._collects = [
+                    Issue(i.find("a")["href"].split("/")[2], self._session)
+                    for i in collects
+                ]
+            else:
+                self._collects = []
 
     def pull(self) -> dict:
         """Pull issue
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_move"
         data = {"comic_id": self.issue_id, "list_id": 1, "action_id": 1}
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def unsubscribe(self) -> dict:
         """Unsubscribe issue
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_move"
         data = {"comic_id": self.issue_id, "list_id": 1, "action_id": 0}
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def add_to_collection(self) -> dict:
         """Add issue to collection
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_move"
         data = {"comic_id": self.issue_id, "list_id": 2, "action_id": 1}
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def remove_from_collection(self) -> dict:
         """Remove series from collection
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_move"
         data = {"comic_id": self.issue_id, "list_id": 2, "action_id": 0}
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def mark_read(self) -> dict:
         """Mark issue as read
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_move"
         data = {"comic_id": self.issue_id, "list_id": 5, "action_id": 1}
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def remove_from_readlist(self) -> dict:
         """Mark issue as unread
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_move"
         data = {"comic_id": self.issue_id, "list_id": 5, "action_id": 0}
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def add_to_wishlist(self) -> dict:
         """Add series to wishlist
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_move"
         data = {"comic_id": self.issue_id, "list_id": 3, "action_id": 1}
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def remove_from_wishlist(self) -> dict:
         """Remove series from wishlist
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/my_list_move"
         data = {"comic_id": self.issue_id, "list_id": 3, "action_id": 0}
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def rate(self, score: int) -> dict:
         """Rate issue
 
         Args:
             score (int): number from 0 to 5
 
         Returns:
             dict: {"text": "", "type": "error|success"}
         """
-        if not self._ci_session:
+        if not self._session.authenticated:
             return {"text": "No ci_session is given", "type": "error"}
         if score < 0 or score > 5:
             return {"text": "Score must be between 1 and 5", "type": "error"}
         url = "https://leagueofcomicgeeks.com/comic/post_rating"
         data = {"comic_id": self.issue_id, "score": score}
-        r = self._session.post(url, headers=_headers, data=data).json()
+        r = self._session.post(url, data=data).json()
         return {"text": r["text"], "type": r["type"]}
 
     def json(self) -> dict:
         """Return data in json format"""
-        return {
+        r = {
             "issue_id": self.issue_id,
             "characters": self.characters,
             "cover": self.cover,
             "community": self.community,
             "description": self.description,
             "details": self.details,
             "name": self.name,
@@ -1044,52 +1127,66 @@
             "publisher": self.publisher,
             "series_pagination": self.series_pagination,
             "store_date": self.store_date,
             "url": self.url,
             "variant_covers": self.variant_covers,
             "user": self.user,
         }
+        if type(self).__name__ == "Trade_Paperback":
+            r["collects"] = self.collects
+        return r
+
+
+class Trade_Paperback(Issue):
+    def __init__(self, issue_id: int, session: requests.Session):
+        super().__init__(issue_id, session)
+        self._collects = None
+
+    @property
+    def collects(self) -> list[Issue]:
+        """List of issues collected in this trade paperback"""
+        if self._collects is None:
+            self._get_data()
+        return self._collects
 
 
 class Creator:
     """Creator class"""
 
-    def __init__(self, creator_id: int, ci_session: str = None):
+    def __init__(self, creator_id: int, session: requests.Session):
         self._characters = None
-        self._ci_session = ci_session
+        self._session = session
         self._series = None
         self._creator_id = creator_id
         self._description = None
         self._image = None
         self._name = None
         self._url = None
         self._read = None
         self._owned = None
         self._issue_count = None
-        self._session = requests.Session()
-        self._session.cookies.update({"ci_session": ci_session})
 
     @property
     def issue_count(self) -> int:
         """Number of issues made by this creator"""
-        if self._issue_count is None and self._ci_session:
+        if self._issue_count is None and self._session.authenticated:
             self._get_data()
         return self._issue_count
 
     @property
     def read(self) -> int:
         """Issues by this creator read"""
-        if self._read is None and self._ci_session:
+        if self._read is None and self._session.authenticated:
             self._get_data()
         return self._read
 
     @property
     def owned(self) -> int:
         """Issues by this creator owned"""
-        if self._owned is None and self._ci_session:
+        if self._owned is None and self._session.authenticated:
             self._get_data()
         return self._owned
 
     @property
     def description(self) -> list:
         """Creator description"""
         if self._description is None:
@@ -1148,18 +1245,18 @@
 
     @url.setter
     def url(self, value):
         self._url = value
 
     def _get_data(self):
         url = f"https://leagueofcomicgeeks.com/people/{self.creator_id}/foo"
-        r = self._session.get(url, headers=_headers)
+        r = self._session.get(url)
         r.raise_for_status()
         comics_url = f"{r.url}/comics"
-        comics_r = self._session.get(comics_url, headers=_headers)
+        comics_r = self._session.get(comics_url)
         comics_r.raise_for_status()
         comics_soup = BeautifulSoup(comics_r.content, features="lxml")
         soup = BeautifulSoup(r.content, features="lxml")
 
         self._name = soup.find(class_="page-details").find("h1").text.strip()
         self._description = (
             soup.find(class_="series-summary").find("p").text
@@ -1168,25 +1265,25 @@
         )
 
         avatar = soup.find(class_="avatar")
         self._image = avatar.find("img")["src"] if avatar is not None else "#"
         self._url = r.url.split(".com")[1]
 
         characters = soup.find(id="characters")
-        self._characters = get_characters(characters, Character, self._ci_session)
+        self._characters = get_characters(characters, Character, self._session)
         comics = comics_soup.find(id="comic-list-block").find_all("li")
-        self._series = get_series(comics, Series, self._ci_session)
+        self._series = get_series(comics, Series, self._session)
         stats = comics_soup.findAll(class_="comic-score")
         if stats:
             self._issue_count = int(
                 stats[0].find(class_="text").text.strip().split("\n")[0].split(" ")[2]
             )
         else:
             self._issue_count = "Unknown"
-        if self._ci_session:
+        if self._session.authenticated:
             if stats:
                 self._owned = int(
                     stats[0]
                     .find(class_="text")
                     .text.strip()
                     .split("\n")[0]
                     .split(" ")[0]
@@ -1217,52 +1314,50 @@
             "issue_count": self.issue_count,
         }
 
 
 class Character:
     """Character class"""
 
-    def __init__(self, character_id: int, ci_session: str = None):
+    def __init__(self, character_id: int, session: requests.Session):
         self._character_id = character_id
-        self._ci_session = ci_session
+        self._session = session
         self._image = None
         self._creators = None
         self._description = None
         self._information = None
         self._also_known_as = None
         self._series = None
         self._universe = None
         self._publisher = None
         self._name = None
         self._real_name = None
         self._url = None
         self._read = None
         self._owned = None
         self._issue_count = None
-        self._session = requests.Session()
-        self._session.cookies.update({"ci_session": ci_session})
 
     @property
     def read(self) -> int:
         """Issues with this character read"""
-        if self._read is None and self._ci_session:
+        if self._read is None and self._session.authenticated:
             self._get_data()
         return self._read
 
     @property
     def issue_count(self) -> int:
         """Issues with this character"""
-        if self._issue_count is None and self._ci_session:
+        if self._issue_count is None and self._session.authenticated:
             self._get_data()
         return self._issue_count
 
     @property
     def owned(self) -> int:
         """Issues with this character owned"""
-        if self._owned is None and self._ci_session:
+        if self._owned is None and self._session.authenticated:
             self._get_data()
         return self._owned
 
     @property
     def image(self) -> str:
         """Character image"""
         if self._image is None:
@@ -1368,18 +1463,18 @@
         """Character id"""
         if self._character_id is None:
             self._get_data()
         return self._character_id
 
     def _get_data(self):
         url = f"https://leagueofcomicgeeks.com/character/{self.character_id}/foo"
-        r = self._session.get(url, headers=_headers)
+        r = self._session.get(url)
         r.raise_for_status()
         comics_url = f"{r.url}/comics"
-        comics_r = self._session.get(comics_url, headers=_headers)
+        comics_r = self._session.get(comics_url)
         comics_r.raise_for_status()
         comics_soup = BeautifulSoup(comics_r.content, features="lxml")
         soup = BeautifulSoup(r.content, features="lxml")
 
         name = soup.find("h1").text.strip()
         self._name = name
         details = soup.find(class_="header-intro").text.strip().split("·")
@@ -1400,15 +1495,15 @@
         lists = soup.find(class_="content-sidebar-wrapper").findAll("ul")
         creators = []
         if lists:
             for creator in lists[0].findAll("li"):
                 a = creator.find("a")
                 if "people" in a["href"]:
                     creator_id = a["href"].split("/")[2]
-                    c = Creator(creator_id, self._ci_session)
+                    c = Creator(creator_id, self._session)
                     c.name = creator.find(class_="title").text.strip()
                     c.url = a["href"]
                     creators.append(c)
         self._creators = creators
 
         info = []
         if len(lists) > 1:
@@ -1432,21 +1527,21 @@
         if soup.find(id="personas"):
             for persona in soup.find(id="personas").findAll(class_="name"):
                 href = persona.find("a")["href"]
                 if "character" in href:
                     aka.append({"name": persona.text.strip(), "url": href})
         self._also_known_as = aka
         comics = comics_soup.find(id="comic-list-block").find_all("li")
-        self._series = get_series(comics, Series, self._ci_session)
+        self._series = get_series(comics, Series, self._session)
         stats = comics_soup.findAll(class_="comic-score")
         if stats:
             self._issue_count = int(
                 stats[0].find(class_="text").text.strip().split("\n")[0].split(" ")[2]
             )
-        if self._ci_session:
+        if self._session.authenticated:
             if stats:
                 self._owned = int(
                     stats[0]
                     .find(class_="text")
                     .text.strip()
                     .split("\n")[0]
                     .split(" ")[0]
```

### Comparing `comicgeeks-0.2.3/src/comicgeeks/extract.py` & `comicgeeks-0.3.0/src/comicgeeks/extract.py`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/src/comicgeeks.egg-info/PKG-INFO` & `comicgeeks-0.3.0/src/comicgeeks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comicgeeks
-Version: 0.2.3
+Version: 0.3.0
 Summary: A python client for League of Comics Geeks.
 Home-page: https://github.com/pruizlezcano/comicgeeks
 Author: Pablo Ruiz
 Author-email: pruizlezcano@gmail.com
 License: GPL-3.0-only
 Project-URL: Documentation, https://comicgeeks.readthedocs.io
 Project-URL: Source, https://github.com/pruizlezcano/comicgeeks
```

### Comparing `comicgeeks-0.2.3/src/comicgeeks.egg-info/SOURCES.txt` & `comicgeeks-0.3.0/src/comicgeeks.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 LICENSE.txt
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/ci.yml
 docs/Makefile
 docs/changelog.md
 docs/conf.py
 docs/contributing.md
 docs/examples.md
 docs/genindex.md
 docs/get-started.md
 docs/index.rst
 docs/license.md
 docs/modules.rst
+docs/readme.md
 docs/requirements.txt
+docs/_static/.gitignore
 docs/_static/custom.js
 docs/_static/debug.js
 docs/_static/icon.png
 docs/_static/icon.svg
 docs/_static/revitron-ui-mobile.svg
 docs/_static/css/custom.css
 docs/_templates/layout.html
@@ -45,9 +48,10 @@
 src/comicgeeks.egg-info/requires.txt
 src/comicgeeks.egg-info/top_level.txt
 tests/conftest.py
 tests/test_Character.py
 tests/test_Creator.py
 tests/test_Issue.py
 tests/test_Series.py
+tests/test_TradePaperback.py
 tests/test_new_releases.py
 tests/test_session.py
```

### Comparing `comicgeeks-0.2.3/tests/test_Creator.py` & `comicgeeks-0.3.0/tests/test_Creator.py`

 * *Files identical despite different names*

### Comparing `comicgeeks-0.2.3/tests/test_Issue.py` & `comicgeeks-0.3.0/tests/test_Issue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import pytest
 from comicgeeks import Comic_Geeks
 from dotenv import dotenv_values
 from pathlib import Path
 
 dotenv_path = Path(".devdata.env")
 env = dotenv_values(dotenv_path=dotenv_path)
+if "LCG_CI_SESSION" not in env:
+    import os
+
+    env = {
+        "LCG_CI_SESSION": os.environ.get("LCG_CI_SESSION"),
+        "LCG_USERNAME": os.environ.get("LCG_USERNAME"),
+        "LCG_PASSWORD": os.environ.get("LCG_PASSWORD"),
+    }
 
 __author__ = "Pablo Ruiz"
 __copyright__ = "Pablo Ruiz"
 __license__ = "GPL-3.0-only"
 
 
 def test_get_issue_by_id():
@@ -48,14 +56,15 @@
             else community["rating"] == "Unknown"
         )
     )
     assert data["description"] != ""
     assert data["details"] == {
         "format": "comic",
         "page_count": "28 pages",
+        "cover_date": "sep 2019",
         "upc": "75960609142300811",
         "distributor_sku": "may190864",
     }
     assert data["name"] == "No Devils, Only God, Part 3"
     assert data["number"] == "8"
     assert len(data["person_credits"]) > 0
     assert data["price"] == 3.99
@@ -63,24 +72,24 @@
     pagination = data["series_pagination"]
     assert all(
         map(
             lambda x: pagination[x] is not None,
             pagination.keys(),
         )
     )
-    assert data["store_date"] == 1563314400
+    assert data["store_date"] == 1563321600
     assert data["url"] == "/comic/3616996/daredevil-8"
     assert len(data["variant_covers"]) >= 2
     user = data["user"]
     assert all(map(lambda x: user[x] is None, user.keys()))
 
 
 def test_get_issue_by_id_session():
     """Get issue by id test"""
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     data = client.issue_info(3616996)
     assert any(map(lambda x: data.user[x] is not None, data.user.keys()))
 
 
 def test_get_issue_without_characters():
     """Get issue without characters credits test"""
     client = Comic_Geeks()
@@ -93,14 +102,15 @@
     client = Comic_Geeks()
     data = client.issue_info(7757146)
     assert len(data.variant_covers) == 0
 
 
 ## TODO: issue without creator credits
 
+
 def test_add_to_collection_error():
     client = Comic_Geeks()
     issue = client.issue_info(7757146)
     data = issue.add_to_collection()
     assert data["type"] == "error"
 
 
@@ -157,74 +167,74 @@
     client = Comic_Geeks()
     issue = client.issue_info(7757146)
     data = issue.unsubscribe()
     assert data["type"] == "error"
 
 
 def test_add_to_collection():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     issue = client.issue_info(7757146)
     data = issue.add_to_collection()
     assert data["type"] == "success"
 
 
 def test_add_to_wishlist():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     issue = client.issue_info(7757146)
     data = issue.add_to_wishlist()
     assert data["type"] == "success"
 
 
 def test_mark_read():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     issue = client.issue_info(7757146)
     data = issue.mark_read()
     assert data["type"] == "success"
 
 
 def test_pull():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     issue = client.issue_info(7757146)
     data = issue.pull()
     assert data["type"] == "success"
 
 
 def test_rate():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     issue = client.issue_info(7757146)
     data = issue.rate(0)
     assert data["type"] == "success"
 
 
 def test_rate_invalid_error():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     issue = client.issue_info(7757146)
     data = issue.rate(20)
     assert data["type"] == "error"
 
 
 def test_remove_collection():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     issue = client.issue_info(7757146)
     data = issue.remove_from_collection()
     assert data["type"] == "success"
 
 
 def test_remove_readlist():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     issue = client.issue_info(7757146)
     data = issue.remove_from_readlist()
     assert data["type"] == "success"
 
 
 def test_remove_wishlist():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     issue = client.issue_info(7757146)
     data = issue.remove_from_wishlist()
     assert data["type"] == "success"
 
 
 def test_unsubscribe():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     issue = client.issue_info(7757146)
     data = issue.unsubscribe()
     assert data["type"] == "success"
```

### Comparing `comicgeeks-0.2.3/tests/test_Series.py` & `comicgeeks-0.3.0/tests/test_Series.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import pytest
 from comicgeeks import Comic_Geeks
 from dotenv import dotenv_values
 from pathlib import Path
 
 dotenv_path = Path(".devdata.env")
 env = dotenv_values(dotenv_path=dotenv_path)
+if "LCG_CI_SESSION" not in env:
+    import os
+
+    env = {
+        "LCG_CI_SESSION": os.environ.get("LCG_CI_SESSION"),
+        "LCG_USERNAME": os.environ.get("LCG_USERNAME"),
+        "LCG_PASSWORD": os.environ.get("LCG_PASSWORD"),
+    }
 
 __author__ = "Pablo Ruiz"
 __copyright__ = "Pablo Ruiz"
 __license__ = "GPL-3.0-only"
 
 
 def test_search_series():
@@ -36,105 +44,107 @@
     assert data["name"] == "Beta Ray Bill"
     assert data["publisher"] == "Marvel Comics"
     assert data["description"] != ""
     assert data["start_year"] == 2021
     assert data["end_year"] == 2021
     assert len(data["issues"]) == 5
     assert data["issue_count"] == 5
+    assert len(data["trade_paperbacks"]) == 1
+    assert data["trade_paperback_count"] == 1
     assert data["url"] == "/comics/series/150065/beta-ray-bill"
     assert data["cover"] != "#"
     user = data["user"]
     assert all(map(lambda x: user[x] is None, user.keys()))
 
 
 def test_get_series_by_id_session():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     data = client.series_info(150065)
     assert any(map(lambda x: data.user[x] is not None, data.user.keys()))
 
 
 def test_add_missing():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.add_missing_to_wishlist()
     assert data["type"] == "success"
 
 
 def test_add_collection():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.add_to_collection()
     assert data["type"] == "success"
 
 
 def test_add_wishlist():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.add_to_wishlist()
     assert data["type"] == "success"
 
 
 def test_mark_owned():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.mark_owned_read()
     assert data["type"] == "success"
 
 
 def test_mark_read():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.mark_read()
     assert data["type"] == "success"
 
 
 def test_pull():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.pull()
     assert data["type"] == "success"
 
 
 def test_pull_hc():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.pull_hc()
     assert data["type"] == "success"
 
 
 def test_pull_tp():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.pull_tp()
     assert data["type"] == "success"
 
 
 def test_remove_collection():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.remove_from_collection()
     assert data["type"] == "success"
 
 
 def test_remove_readlist():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.remove_from_readlist()
     assert data["type"] == "success"
 
 
 def test_remove_wishlist():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.remove_from_wishlist()
     assert data["type"] == "success"
 
 
 def test_unsubscribe():
-    client = Comic_Geeks(env["CI_SESSION"])
+    client = Comic_Geeks(env["LCG_CI_SESSION"])
     series = client.series_info(148315)
     data = series.unsubscribe()
     assert data["type"] == "success"
 
 
 def test_add_missing_error():
     client = Comic_Geeks()
```

### Comparing `comicgeeks-0.2.3/tox.ini` & `comicgeeks-0.3.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 [testenv:{docs,doctests,linkcheck}]
 description =
     docs: Invoke sphinx-build to build the docs
     doctests: Invoke sphinx-build to run doctests
     linkcheck: Check for broken links in the documentation
 passenv =
     SETUPTOOLS_*
+    LCG_CI_SESSION
+    LCG_USERNAME
+    LCG_PASSWORD
 setenv =
     DOCSDIR = {toxinidir}/docs
     BUILDDIR = {toxinidir}/docs/_build
     docs: BUILD = html
     doctests: BUILD = doctest
     linkcheck: BUILD = linkcheck
 deps =
```

