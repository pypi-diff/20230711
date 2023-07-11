# Comparing `tmp/fast-checkers-0.3.0.tar.gz` & `tmp/fast-checkers-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-checkers-0.3.0.tar", last modified: Tue Jul 11 09:05:46 2023, max compression
+gzip compressed data, was "fast-checkers-0.3.1.tar", last modified: Tue Jul 11 09:43:43 2023, max compression
```

## Comparing `fast-checkers-0.3.0.tar` & `fast-checkers-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 09:05:46.965417 fast-checkers-0.3.0/
--rw-rw-rw-   0        0        0    35823 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       44 2023-07-11 08:55:47.000000 fast-checkers-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5712 2023-07-11 09:05:46.962423 fast-checkers-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4257 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-11 09:05:46.911268 fast-checkers-0.3.0/checkers/
--rw-rw-rw-   0        0        0      947 2023-07-11 09:05:03.000000 fast-checkers-0.3.0/checkers/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-10 08:43:08.000000 fast-checkers-0.3.0/checkers/american.py
--rw-rw-rw-   0        0        0     7204 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/checkers/base.py
--rw-rw-rw-   0        0        0     1627 2023-07-10 08:43:08.000000 fast-checkers-0.3.0/checkers/main.py
--rw-rw-rw-   0        0        0      674 2023-07-07 08:25:35.000000 fast-checkers-0.3.0/checkers/models.py
--rw-rw-rw-   0        0        0     4120 2023-07-07 08:25:35.000000 fast-checkers-0.3.0/checkers/move.py
--rw-rw-rw-   0        0        0     4363 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/checkers/server.py
--rw-rw-rw-   0        0        0     2340 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/checkers/standard.py
--rw-rw-rw-   0        0        0     1968 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/checkers/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:05:46.939178 fast-checkers-0.3.0/fast_checkers.egg-info/
--rw-rw-rw-   0        0        0     5712 2023-07-11 09:05:42.000000 fast-checkers-0.3.0/fast_checkers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-07-11 09:05:45.000000 fast-checkers-0.3.0/fast_checkers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 09:05:42.000000 fast-checkers-0.3.0/fast_checkers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 09:05:42.000000 fast-checkers-0.3.0/fast_checkers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       27 2023-07-05 07:24:19.000000 fast-checkers-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 09:05:46.966437 fast-checkers-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2005 2023-07-11 08:55:38.000000 fast-checkers-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:05:46.955657 fast-checkers-0.3.0/test/
--rw-rw-rw-   0        0        0     1123 2023-07-07 08:25:35.000000 fast-checkers-0.3.0/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:43:43.569990 fast-checkers-0.3.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       44 2023-07-11 08:55:47.000000 fast-checkers-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5712 2023-07-11 09:43:43.567991 fast-checkers-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4257 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-11 09:43:43.446993 fast-checkers-0.3.1/checkers/
+-rw-rw-rw-   0        0        0      947 2023-07-11 09:42:38.000000 fast-checkers-0.3.1/checkers/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-10 08:43:08.000000 fast-checkers-0.3.1/checkers/american.py
+-rw-rw-rw-   0        0        0     7204 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/checkers/base.py
+-rw-rw-rw-   0        0        0     1627 2023-07-10 08:43:08.000000 fast-checkers-0.3.1/checkers/main.py
+-rw-rw-rw-   0        0        0      674 2023-07-07 08:25:35.000000 fast-checkers-0.3.1/checkers/models.py
+-rw-rw-rw-   0        0        0     4120 2023-07-07 08:25:35.000000 fast-checkers-0.3.1/checkers/move.py
+-rw-rw-rw-   0        0        0     4363 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/checkers/server.py
+-rw-rw-rw-   0        0        0     2340 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/checkers/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:43:43.309001 fast-checkers-0.3.1/checkers/static/
+drwxrwxrwx   0        0        0        0 2023-07-11 09:43:43.491993 fast-checkers-0.3.1/checkers/static/css/
+-rw-rw-rw-   0        0        0     2803 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/checkers/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-11 09:43:43.500994 fast-checkers-0.3.1/checkers/static/js/
+-rw-rw-rw-   0        0        0     5385 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/checkers/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-11 09:43:43.516993 fast-checkers-0.3.1/checkers/templates/
+-rw-rw-rw-   0        0        0     1857 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/checkers/templates/base.html
+-rw-rw-rw-   0        0        0     2445 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/checkers/templates/index.html
+-rw-rw-rw-   0        0        0     1968 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/checkers/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:43:43.546995 fast-checkers-0.3.1/fast_checkers.egg-info/
+-rw-rw-rw-   0        0        0     5712 2023-07-11 09:43:38.000000 fast-checkers-0.3.1/fast_checkers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-07-11 09:43:41.000000 fast-checkers-0.3.1/fast_checkers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 09:43:38.000000 fast-checkers-0.3.1/fast_checkers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 09:43:38.000000 fast-checkers-0.3.1/fast_checkers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       27 2023-07-05 07:24:19.000000 fast-checkers-0.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 09:43:43.571999 fast-checkers-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1942 2023-07-11 09:34:34.000000 fast-checkers-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:43:43.561992 fast-checkers-0.3.1/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-07 08:25:35.000000 fast-checkers-0.3.1/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-11 08:33:07.000000 fast-checkers-0.3.1/test/test_board.py
```

### Comparing `fast-checkers-0.3.0/LICENSE` & `fast-checkers-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/PKG-INFO` & `fast-checkers-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-checkers
-Version: 0.3.0
+Version: 0.3.1
 Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/checkers
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/checkers/index.html
 Keywords: checkers AI mini-max droughts,game,board
```

### Comparing `fast-checkers-0.3.0/README.rst` & `fast-checkers-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/checkers/__init__.py` & `fast-checkers-0.3.1/checkers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A checkers library for Python, with move generation and validation,
 PDN parsing and writing. Supprots multiple variants of game.
 """
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __author__ = "Michał Skibiński"
```

### Comparing `fast-checkers-0.3.0/checkers/american.py` & `fast-checkers-0.3.1/checkers/american.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/checkers/base.py` & `fast-checkers-0.3.1/checkers/base.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/checkers/main.py` & `fast-checkers-0.3.1/checkers/main.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/checkers/models.py` & `fast-checkers-0.3.1/checkers/models.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/checkers/move.py` & `fast-checkers-0.3.1/checkers/move.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/checkers/server.py` & `fast-checkers-0.3.1/checkers/server.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/checkers/standard.py` & `fast-checkers-0.3.1/checkers/standard.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/checkers/utils.py` & `fast-checkers-0.3.1/checkers/utils.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/fast_checkers.egg-info/PKG-INFO` & `fast-checkers-0.3.1/fast_checkers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-checkers
-Version: 0.3.0
+Version: 0.3.1
 Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/checkers
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/checkers/index.html
 Keywords: checkers AI mini-max droughts,game,board
```

### Comparing `fast-checkers-0.3.0/setup.py` & `fast-checkers-0.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,25 +11,24 @@
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="fast-checkers",
     version=__version__,
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
-    files_to_include=["checkers"],
     description=__doc__.replace("\n", " ").strip(),
     long_description=long_description,
     # rst
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(),
     package_data={
         'checkers': [
-        "checkers/static/js/*",
-        "checkers/static/css/*",
-        "checkers/templates/*"
+        "static/js/*",
+        "static/css/*",
+        "templates/*"
     ]
     },
     requires=requirements,
     license="GPL-3.0+",
     keywords="checkers AI mini-max droughts, game, board",
     url="https://github.com/michalskibinski109/checkers",
     classifiers=[
```

### Comparing `fast-checkers-0.3.0/test/test_american_board.py` & `fast-checkers-0.3.1/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.3.0/test/test_board.py` & `fast-checkers-0.3.1/test/test_board.py`

 * *Files identical despite different names*

