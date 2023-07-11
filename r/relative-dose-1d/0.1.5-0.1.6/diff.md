# Comparing `tmp/relative_dose_1d-0.1.5.tar.gz` & `tmp/relative_dose_1d-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative_dose_1d-0.1.5.tar", last modified: Tue Jul 11 03:32:38 2023, max compression
+gzip compressed data, was "relative_dose_1d-0.1.6.tar", last modified: Tue Jul 11 15:23:52 2023, max compression
```

## Comparing `relative_dose_1d-0.1.5.tar` & `relative_dose_1d-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 03:32:38.848834 relative_dose_1d-0.1.5/
--rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     4831 2023-07-11 03:32:38.842850 relative_dose_1d-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3743 2023-07-11 02:17:16.000000 relative_dose_1d-0.1.5/README.md
--rw-rw-rw-   0        0        0     1404 2023-07-10 23:57:40.000000 relative_dose_1d-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 03:32:38.849833 relative_dose_1d-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 03:32:38.699762 relative_dose_1d-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 03:32:38.770866 relative_dose_1d-0.1.5/src/relative_dose_1d/
--rw-rw-rw-   0        0        0     1410 2023-07-08 19:50:00.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/GUI.py
--rw-rw-rw-   0        0        0    13205 2023-07-11 00:52:51.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/GUI_tool.py
--rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/__init__.py
--rw-rw-rw-   0        0        0      482 2023-07-11 02:57:11.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/forTest.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:32:38.827210 relative_dose_1d-0.1.5/src/relative_dose_1d/test_data/
--rw-rw-rw-   0        0        0      341 2023-07-10 23:57:40.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/test_data/clean.py
--rw-rw-rw-   0        0        0    10639 2023-07-10 03:51:03.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:32:38.823219 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/
--rw-rw-rw-   0        0        0     4831 2023-07-11 03:32:38.000000 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-07-11 03:32:38.000000 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 03:32:38.000000 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-11 03:32:38.000000 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-11 03:32:38.000000 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 15:23:52.744233 relative_dose_1d-0.1.6/
+-rw-rw-rw-   0        0        0     1108 2023-04-04 17:36:43.000000 relative_dose_1d-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     4831 2023-07-11 15:23:52.744233 relative_dose_1d-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3743 2023-07-11 15:21:04.000000 relative_dose_1d-0.1.6/README.md
+-rw-rw-rw-   0        0        0     1404 2023-07-11 15:20:51.000000 relative_dose_1d-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 15:23:52.759832 relative_dose_1d-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 15:23:52.666086 relative_dose_1d-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 15:23:52.712986 relative_dose_1d-0.1.6/src/relative_dose_1d/
+-rw-rw-rw-   0        0        0     1410 2023-07-10 15:29:21.000000 relative_dose_1d-0.1.6/src/relative_dose_1d/GUI.py
+-rw-rw-rw-   0        0        0    13205 2023-07-11 15:18:58.000000 relative_dose_1d-0.1.6/src/relative_dose_1d/GUI_tool.py
+-rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 relative_dose_1d-0.1.6/src/relative_dose_1d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:23:52.744233 relative_dose_1d-0.1.6/src/relative_dose_1d/test_data/
+-rw-rw-rw-   0        0        0      341 2023-07-10 18:36:09.000000 relative_dose_1d-0.1.6/src/relative_dose_1d/test_data/clean.py
+-rw-rw-rw-   0        0        0    10639 2023-07-10 15:29:21.000000 relative_dose_1d-0.1.6/src/relative_dose_1d/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:23:52.744233 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/
+-rw-rw-rw-   0        0        0     4831 2023-07-11 15:23:52.000000 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-07-11 15:23:52.000000 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 15:23:52.000000 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-11 15:23:52.000000 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-11 15:23:52.000000 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/top_level.txt
```

### Comparing `relative_dose_1d-0.1.5/LICENSE` & `relative_dose_1d-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.5/PKG-INFO` & `relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: relative_dose_1d
-Version: 0.1.5
+Name: relative-dose-1d
+Version: 0.1.6
 Summary: Python package to read 1-dimensional dose profile from a text file to perform subtraction and gamma analysis.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://relative-dose-1d.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d/issues
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
@@ -101,13 +101,13 @@
 
 May-2023 Version 0.1.2
   * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
 May-2023 Version 0.1.3
   * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
 
-Jul-2023 Version 0.1.4 - 0.1.5
+Jul-2023 Version 0.1.4 - 0.1.6
 * Two new functions, [build_from_array_and_step](Tools_module_label) to add physical positions, and [plot](GUI_tool_module_label) to show a GUI. 
 * [New GUI_tool module](GUI_tool_module_label).
 * Now it is possible to change tolerance parameter for gamma evaluation.
 * Pass rate, total and evaluated points are now displayed on the GUI.
 * gamma_1d function returns the number of evaluated points.
```

### Comparing `relative_dose_1d-0.1.5/README.md` & `relative_dose_1d-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -80,13 +80,13 @@
 
 May-2023 Version 0.1.2
   * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
 May-2023 Version 0.1.3
   * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
 
-Jul-2023 Version 0.1.4 - 0.1.5
+Jul-2023 Version 0.1.4 - 0.1.6
 * Two new functions, [build_from_array_and_step](Tools_module_label) to add physical positions, and [plot](GUI_tool_module_label) to show a GUI. 
 * [New GUI_tool module](GUI_tool_module_label).
 * Now it is possible to change tolerance parameter for gamma evaluation.
 * Pass rate, total and evaluated points are now displayed on the GUI.
 * gamma_1d function returns the number of evaluated points.
```

### Comparing `relative_dose_1d-0.1.5/pyproject.toml` & `relative_dose_1d-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative_dose_1d"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
 description = "Python package to read 1-dimensional dose profile from a text file to perform subtraction and gamma analysis."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
```

### Comparing `relative_dose_1d-0.1.5/src/relative_dose_1d/GUI.py` & `relative_dose_1d-0.1.6/src/relative_dose_1d/GUI.py`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.5/src/relative_dose_1d/GUI_tool.py` & `relative_dose_1d-0.1.6/src/relative_dose_1d/GUI_tool.py`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.5/src/relative_dose_1d/tools.py` & `relative_dose_1d-0.1.6/src/relative_dose_1d/tools.py`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/PKG-INFO` & `relative_dose_1d-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: relative-dose-1d
-Version: 0.1.5
+Name: relative_dose_1d
+Version: 0.1.6
 Summary: Python package to read 1-dimensional dose profile from a text file to perform subtraction and gamma analysis.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://relative-dose-1d.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d/issues
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
@@ -101,13 +101,13 @@
 
 May-2023 Version 0.1.2
   * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
 May-2023 Version 0.1.3
   * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
 
-Jul-2023 Version 0.1.4 - 0.1.5
+Jul-2023 Version 0.1.4 - 0.1.6
 * Two new functions, [build_from_array_and_step](Tools_module_label) to add physical positions, and [plot](GUI_tool_module_label) to show a GUI. 
 * [New GUI_tool module](GUI_tool_module_label).
 * Now it is possible to change tolerance parameter for gamma evaluation.
 * Pass rate, total and evaluated points are now displayed on the GUI.
 * gamma_1d function returns the number of evaluated points.
```

