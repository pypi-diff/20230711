# Comparing `tmp/oceanum-0.7.8.tar.gz` & `tmp/oceanum-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanum-0.7.8.tar", last modified: Wed Jun 14 05:24:13 2023, max compression
+gzip compressed data, was "oceanum-0.7.9.tar", last modified: Tue Jul 11 07:09:15 2023, max compression
```

## Comparing `oceanum-0.7.8.tar` & `oceanum-0.7.9.tar`

### file list

```diff
@@ -1,70 +1,187 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.396674 oceanum-0.7.8/
--rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.7.8/AUTHORS.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.7.8/CONTRIBUTING.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       89 2023-05-14 22:31:40.000000 oceanum-0.7.8/HISTORY.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.7.8/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.7.8/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-06-14 05:24:13.396674 oceanum-0.7.8/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.7.8/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.380674 oceanum-0.7.8/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/Makefile
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.376674 oceanum-0.7.8/docs/_build/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.376674 oceanum-0.7.8/docs/_build/html/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.384674 oceanum-0.7.8/docs/_build/html/_static/
--rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/_build/html/_static/file.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/_build/html/_static/minus.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.376674 oceanum-0.7.8/docs/_templates/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.384674 oceanum-0.7.8/docs/_templates/autosummary/
--rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/about.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/api.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.376674 oceanum-0.7.8/docs/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.384674 oceanum-0.7.8/docs/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/classes/datamesh/oceanum.datamesh.Connector.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/classes/datamesh/oceanum.datamesh.Query.rst
--rwxrwxr-x   0 dave      (1000) dave      (1000)     5220 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/conf.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      160 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/index.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/installation.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/make.bat
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/modules.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/oceanum.datamesh.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/oceanum.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/usage.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.384674 oceanum-0.7.8/oceanum/
--rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-06-14 05:17:45.000000 oceanum-0.7.8/oceanum/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.7.8/oceanum/cli.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.388674 oceanum-0.7.8/oceanum/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.7.8/oceanum/datamesh/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.7.8/oceanum/datamesh/catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    20720 2023-06-08 20:52:11.000000 oceanum-0.7.8/oceanum/datamesh/connection.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    10443 2023-05-14 22:31:40.000000 oceanum-0.7.8/oceanum/datamesh/datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-05-14 22:31:40.000000 oceanum-0.7.8/oceanum/datamesh/exceptions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7537 2023-05-14 22:35:23.000000 oceanum-0.7.8/oceanum/datamesh/query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.7.8/oceanum/datamesh/zarr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.388674 oceanum-0.7.8/oceanum.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-06-14 05:24:13.396674 oceanum-0.7.8/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2023-05-14 22:31:40.000000 oceanum-0.7.8/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.388674 oceanum-0.7.8/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.396674 oceanum-0.7.8/tests/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/data/grid_data_1.nc
--rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/data/ocean_test_1.mp4
--rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/data/point_data_1.csv
--rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_datamesh_connect.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_datamesh_load.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_datamesh_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_datamesh_write.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2936 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_video_compat.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.991456 oceanum-0.7.9/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1834 2023-05-14 22:31:40.000000 oceanum-0.7.9/.gitignore
+-rw-rw-r--   0 dave      (1000) dave      (1000)      167 2023-05-14 22:31:40.000000 oceanum-0.7.9/.gitlab-ci.yml
+-rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.7.9/AUTHORS.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.7.9/CONTRIBUTING.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       89 2023-05-14 22:31:40.000000 oceanum-0.7.9/HISTORY.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.7.9/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.7.9/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2245 2023-05-14 22:31:40.000000 oceanum-0.7.9/Makefile
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1200 2023-07-11 07:09:15.991456 oceanum-0.7.9/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      364 2023-05-14 22:31:40.000000 oceanum-0.7.9/README.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.7.9/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.839452 oceanum-0.7.9/docs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/Makefile
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.851452 oceanum-0.7.9/docs/_build/doctrees/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7953 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/about.doctree
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9406 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/api.doctree
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/doctrees/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.871453 oceanum-0.7.9/docs/_build/doctrees/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    29966 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/classes/datamesh/oceanum.datamesh.Catalog.doctree
+-rw-rw-r--   0 dave      (1000) dave      (1000)   110431 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/classes/datamesh/oceanum.datamesh.Connector.doctree
+-rw-rw-r--   0 dave      (1000) dave      (1000)    69623 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/classes/datamesh/oceanum.datamesh.Datasource.doctree
+-rw-rw-r--   0 dave      (1000) dave      (1000)    33031 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/classes/datamesh/oceanum.datamesh.Query.doctree
+-rw-rw-r--   0 dave      (1000) dave      (1000)   188704 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/environment.pickle
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2827 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/index.doctree
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7395 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/installation.doctree
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2701 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/modules.doctree
+-rw-rw-r--   0 dave      (1000) dave      (1000)   366728 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/oceanum.datamesh.doctree
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4792 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/oceanum.doctree
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7535 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/doctrees/usage.doctree
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.891453 oceanum-0.7.9/docs/_build/html/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      230 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/.buildinfo
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.891453 oceanum-0.7.9/docs/_build/html/_modules/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6581 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_modules/index.html
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/html/_modules/oceanum/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.895454 oceanum-0.7.9/docs/_build/html/_modules/oceanum/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    20408 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_modules/oceanum/datamesh/catalog.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)    85038 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_modules/oceanum/datamesh/connection.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)    52867 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_modules/oceanum/datamesh/datasource.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)    35899 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_modules/oceanum/datamesh/query.html
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.907454 oceanum-0.7.9/docs/_build/html/_sources/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/about.rst.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/api.rst.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/html/_sources/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.911454 oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/oceanum.datamesh.Catalog.rst.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/oceanum.datamesh.Connector.rst.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/oceanum.datamesh.Datasource.rst.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/oceanum.datamesh.Query.rst.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      160 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/installation.rst.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/oceanum.datamesh.rst.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/oceanum.rst.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_sources/usage.rst.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.939455 oceanum-0.7.9/docs/_build/html/_static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4418 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)      121 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/autodoc_pydantic.css
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11521 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/banner_dark.svg
+-rw-rw-r--   0 dave      (1000) dave      (1000)    14621 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4472 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/doctools.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/file.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)   288580 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/jquery-3.6.0.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)    89501 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/jquery.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4758 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/language_data.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)    15069 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/pygments.css
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.943455 oceanum-0.7.9/docs/_build/html/_static/scripts/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    88212 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)    18215 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/searchtools.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4712 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/sphinx_highlight.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.943455 oceanum-0.7.9/docs/_build/html/_static/styles/
+-rw-rw-r--   0 dave      (1000) dave      (1000)   171194 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/styles/pydata-sphinx-theme.css
+-rw-rw-r--   0 dave      (1000) dave      (1000)      106 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/styles/theme.css
+-rw-rw-r--   0 dave      (1000) dave      (1000)    68420 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/underscore-1.13.1.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)    19530 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/underscore.js
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/html/_static/vendor/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.943455 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1548 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.943455 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/css/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    58578 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/css/all.min.css
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.967455 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/
+-rw-rw-r--   0 dave      (1000) dave      (1000)   133034 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.eot
+-rw-rw-r--   0 dave      (1000) dave      (1000)   715890 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.svg
+-rw-rw-r--   0 dave      (1000) dave      (1000)   132728 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.ttf
+-rw-rw-r--   0 dave      (1000) dave      (1000)    89824 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff
+-rw-rw-r--   0 dave      (1000) dave      (1000)    76612 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2
+-rw-rw-r--   0 dave      (1000) dave      (1000)    34390 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.eot
+-rw-rw-r--   0 dave      (1000) dave      (1000)   144322 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.svg
+-rw-rw-r--   0 dave      (1000) dave      (1000)    34092 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.ttf
+-rw-rw-r--   0 dave      (1000) dave      (1000)    16800 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff
+-rw-rw-r--   0 dave      (1000) dave      (1000)    13584 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-regular-400.woff2
+-rw-rw-r--   0 dave      (1000) dave      (1000)   202902 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.eot
+-rw-rw-r--   0 dave      (1000) dave      (1000)   897426 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.svg
+-rw-rw-r--   0 dave      (1000) dave      (1000)   202616 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.ttf
+-rw-rw-r--   0 dave      (1000) dave      (1000)   103300 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff
+-rw-rw-r--   0 dave      (1000) dave      (1000)    79444 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1361 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/_static/webpack-macros.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10044 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/about.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9934 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/api.html
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.827452 oceanum-0.7.9/docs/_build/html/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.971455 oceanum-0.7.9/docs/_build/html/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    18843 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/classes/datamesh/oceanum.datamesh.Catalog.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)    44376 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/classes/datamesh/oceanum.datamesh.Connector.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)    37152 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/classes/datamesh/oceanum.datamesh.Datasource.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21536 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/classes/datamesh/oceanum.datamesh.Query.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)    35493 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/genindex.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8374 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/index.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9389 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/installation.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8086 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/modules.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1427 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/objects.inv
+-rw-rw-r--   0 dave      (1000) dave      (1000)   182788 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/oceanum.datamesh.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)    32052 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/oceanum.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7827 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/py-modindex.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6915 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/search.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)    33738 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/searchindex.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)    13261 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_build/html/usage.html
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.831452 oceanum-0.7.9/docs/_templates/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.971455 oceanum-0.7.9/docs/_templates/autosummary/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/about.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/api.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11521 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/banner_dark.svg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.831452 oceanum-0.7.9/docs/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.975456 oceanum-0.7.9/docs/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/classes/datamesh/oceanum.datamesh.Connector.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/classes/datamesh/oceanum.datamesh.Query.rst
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     5654 2023-07-11 03:17:01.000000 oceanum-0.7.9/docs/conf.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      522 2023-07-11 03:17:01.000000 oceanum-0.7.9/docs/index.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/installation.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/make.bat
+-rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/modules.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)    15086 2023-07-11 03:17:01.000000 oceanum-0.7.9/docs/oceanum-favicon.ico
+-rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/oceanum.datamesh.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/oceanum.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/requirements.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.7.9/docs/usage.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-07-11 03:28:18.000000 oceanum-0.7.9/log.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.979456 oceanum-0.7.9/oceanum/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      292 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/.editorconfig
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.983456 oceanum-0.7.9/oceanum/.github/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      318 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1172 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/.gitignore
+-rw-rw-r--   0 dave      (1000) dave      (1000)      290 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/.travis.yml
+-rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-07-11 03:18:32.000000 oceanum-0.7.9/oceanum/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/cli.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.983456 oceanum-0.7.9/oceanum/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/datamesh/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/datamesh/catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    20940 2023-07-11 03:58:41.000000 oceanum-0.7.9/oceanum/datamesh/connection.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10443 2023-07-11 03:34:29.000000 oceanum-0.7.9/oceanum/datamesh/datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-05-14 22:31:40.000000 oceanum-0.7.9/oceanum/datamesh/exceptions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7537 2023-07-11 03:34:33.000000 oceanum-0.7.9/oceanum/datamesh/query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.7.9/oceanum/datamesh/zarr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.983456 oceanum-0.7.9/oceanum.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1200 2023-07-11 07:09:14.000000 oceanum-0.7.9/oceanum.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5979 2023-07-11 07:09:15.000000 oceanum-0.7.9/oceanum.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-11 07:09:14.000000 oceanum-0.7.9/oceanum.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-07-11 07:09:15.000000 oceanum-0.7.9/oceanum.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-11 07:09:14.000000 oceanum-0.7.9/oceanum.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-07-11 07:09:15.000000 oceanum-0.7.9/oceanum.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-07-11 07:09:15.000000 oceanum-0.7.9/oceanum.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      126 2023-07-11 07:03:39.000000 oceanum-0.7.9/requirements.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      124 2023-05-14 22:31:40.000000 oceanum-0.7.9/requirements_dev.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-07-11 07:09:15.991456 oceanum-0.7.9/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2023-05-14 22:31:40.000000 oceanum-0.7.9/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.987456 oceanum-0.7.9/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-11 07:09:15.991456 oceanum-0.7.9/tests/data/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/data/grid_data_1.nc
+-rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/data/ocean_test_1.mp4
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/data/point_data_1.csv
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_datamesh_connect.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_datamesh_load.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_datamesh_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_datamesh_write.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2936 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.7.9/tests/test_video_compat.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      618 2023-05-14 22:31:40.000000 oceanum-0.7.9/tox.ini
```

### Comparing `oceanum-0.7.8/CONTRIBUTING.rst` & `oceanum-0.7.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/LICENSE` & `oceanum-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/PKG-INFO` & `oceanum-0.7.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.7.8
+Version: 0.7.9
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
+Platform: UNKNOWN
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ==============
 oceanum-python
 ==============
 
@@ -48,7 +49,9 @@
 History
 =======
 
 0.4.2 (2022-05-20)
 ------------------
 
 * First release on PyPI.
+
+
```

### Comparing `oceanum-0.7.8/README.rst` & `oceanum-0.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/docs/Makefile` & `oceanum-0.7.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/docs/api.rst` & `oceanum-0.7.9/docs/_build/html/_sources/api.rst.txt`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/docs/classes/datamesh/oceanum.datamesh.Connector.rst` & `oceanum-0.7.9/docs/_build/html/_sources/classes/datamesh/oceanum.datamesh.Connector.rst.txt`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/docs/conf.py` & `oceanum-0.7.9/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,20 +89,37 @@
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "pydata_sphinx_theme"
 html_logo = "banner_dark.svg"
+html_favicon = "oceanum-favicon.ico"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
-# html_theme_options = {}
+html_theme_options = {
+    "collapse_navigation": True,
+    "show_nav_level": 2,
+    "secondary_sidebar_items": ["page-toc", "edit-this-page", "sourcelink"],
+    "icon_links": [
+        {
+            "name": "GitHub",
+            "url": "https://github.com/oceanum-io/oceanum-python",
+            "icon": "fab fa-github",
+            "type": "fontawesome",
+        }
+   ]
+}
+
+html_sidebars = {
+  "**": ["globaltoc.html"],
+}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
```

### Comparing `oceanum-0.7.8/docs/installation.rst` & `oceanum-0.7.9/docs/_build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/docs/make.bat` & `oceanum-0.7.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/docs/oceanum.datamesh.rst` & `oceanum-0.7.9/docs/_build/html/_sources/oceanum.datamesh.rst.txt`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/docs/usage.rst` & `oceanum-0.7.9/docs/_build/html/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/oceanum/datamesh/catalog.py` & `oceanum-0.7.9/oceanum/datamesh/catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/oceanum/datamesh/connection.py` & `oceanum-0.7.9/oceanum/datamesh/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import io
+import re
 import json
 import datetime
 import tempfile
 import hashlib
 import requests
 import fsspec
 import xarray
@@ -436,14 +437,18 @@
             append (string, optional): Coordinate to append on. default=None
             overwrite (bool, optional): Overwrite existing datasource. default=False
             **properties: Additional properties for the datasource - see :obj:`oceanum.datamesh.Datasource`
 
         Returns:
             :obj:`oceanum.datamesh.Datasource`: The datasource instance that was written to
         """
+        if not re.match("^[a-z0-9_-]*$", datasource_id):
+            raise DatameshWriteError(
+                "Datasource ID must only contain lowercase letters, numbers, dashes and underscores"
+            )
         try:
             ds = self.get_datasource(datasource_id)
         except DatameshConnectError as e:
             overwrite = True
         if data is not None:
             with tempfile.NamedTemporaryFile("w+b", delete=False) as f:
                 try:
```

### Comparing `oceanum-0.7.8/oceanum/datamesh/datasource.py` & `oceanum-0.7.9/oceanum/datamesh/datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/oceanum/datamesh/query.py` & `oceanum-0.7.9/oceanum/datamesh/query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/oceanum/datamesh/zarr.py` & `oceanum-0.7.9/oceanum/datamesh/zarr.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/oceanum.egg-info/PKG-INFO` & `oceanum-0.7.9/oceanum.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.7.8
+Version: 0.7.9
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
+Platform: UNKNOWN
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ==============
 oceanum-python
 ==============
 
@@ -48,7 +49,9 @@
 History
 =======
 
 0.4.2 (2022-05-20)
 ------------------
 
 * First release on PyPI.
+
+
```

### Comparing `oceanum-0.7.8/setup.py` & `oceanum-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/data/grid_data_1.nc` & `oceanum-0.7.9/tests/data/grid_data_1.nc`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/data/ocean_test_1.mp4` & `oceanum-0.7.9/tests/data/ocean_test_1.mp4`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/data/point_data_1.csv` & `oceanum-0.7.9/tests/data/point_data_1.csv`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/test_catalog.py` & `oceanum-0.7.9/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/test_datamesh_connect.py` & `oceanum-0.7.9/tests/test_datamesh_connect.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/test_datamesh_load.py` & `oceanum-0.7.9/tests/test_datamesh_load.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/test_datamesh_query.py` & `oceanum-0.7.9/tests/test_datamesh_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/test_datamesh_write.py` & `oceanum-0.7.9/tests/test_datamesh_write.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/test_datasource.py` & `oceanum-0.7.9/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/test_query.py` & `oceanum-0.7.9/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.8/tests/test_video_compat.py` & `oceanum-0.7.9/tests/test_video_compat.py`

 * *Files identical despite different names*

