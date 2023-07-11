# Comparing `tmp/circadian_desktops-0.0.3.tar.gz` & `tmp/circadian_desktops-0.0.4.tar.gz`

## Comparing `circadian_desktops-0.0.3.tar` & `circadian_desktops-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/requirements.txt
--rw-r--r--   0        0        0   297003 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/screenshot.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/__main__.py
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/app.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/custom_qt.py
--rw-r--r--   0        0        0    19137 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/desktopUi.ui
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/functions.py
--rw-r--r--   0        0        0    18146 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/ui_mainwindow.py
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/clock.png
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/clock_32.png
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/clock_50.png
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/dawn.png
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/dawn_64.png
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/dawn_80.png
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/day.png
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/day_64.png
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/day_80.png
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/dusk.png
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/dusk_64.png
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/dusk_80.png
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/logo.ico
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/logo.png
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/night.png
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/night_64.png
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/night_80.png
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/preferences.png
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/preferences_32.png
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/preferences_50.png
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/screen.png
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/screen_32.png
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/src/circadian_desktops/Icons/screen_50.png
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/LICENSE
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 circadian_desktops-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/requirements.txt
+-rw-r--r--   0        0        0   297003 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/screenshot.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/__main__.py
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/app.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/custom_qt.py
+-rw-r--r--   0        0        0    19137 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/desktopUi.ui
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/functions.py
+-rw-r--r--   0        0        0    18146 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/ui_mainwindow.py
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/clock.png
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/clock_32.png
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/clock_50.png
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/dawn.png
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/dawn_64.png
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/dawn_80.png
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/day.png
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/day_64.png
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/day_80.png
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/dusk.png
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/dusk_64.png
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/dusk_80.png
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/logo.ico
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/logo.png
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/night.png
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/night_64.png
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/night_80.png
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/preferences.png
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/preferences_32.png
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/preferences_50.png
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/screen.png
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/screen_32.png
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/src/circadian_desktops/Icons/screen_50.png
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 circadian_desktops-0.0.4/PKG-INFO
```

### Comparing `circadian_desktops-0.0.3/screenshot.png` & `circadian_desktops-0.0.4/screenshot.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/app.py` & `circadian_desktops-0.0.4/src/circadian_desktops/app.py`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/custom_qt.py` & `circadian_desktops-0.0.4/src/circadian_desktops/custom_qt.py`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/desktopUi.ui` & `circadian_desktops-0.0.4/src/circadian_desktops/desktopUi.ui`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/functions.py` & `circadian_desktops-0.0.4/src/circadian_desktops/functions.py`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/ui_mainwindow.py` & `circadian_desktops-0.0.4/src/circadian_desktops/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/clock.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/clock.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/clock_32.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/clock_32.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/clock_50.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/clock_50.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/dawn.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/dawn.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/dawn_64.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/dawn_64.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/dawn_80.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/dawn_80.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/day.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/day.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/day_64.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/day_64.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/day_80.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/day_80.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/dusk.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/dusk.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/dusk_64.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/dusk_64.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/dusk_80.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/dusk_80.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/logo.ico` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/logo.ico`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/logo.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/logo.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/night.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/night.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/night_64.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/night_64.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/night_80.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/night_80.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/preferences.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/preferences.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/preferences_32.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/preferences_32.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/preferences_50.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/preferences_50.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/src/circadian_desktops/Icons/screen.png` & `circadian_desktops-0.0.4/src/circadian_desktops/Icons/screen.png`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/LICENSE` & `circadian_desktops-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/README.md` & `circadian_desktops-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `circadian_desktops-0.0.3/pyproject.toml` & `circadian_desktops-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "circadian_desktops"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Luke Hartley", email="luke.hartley05@gmail.com" },
 ]
 description = "An app that changes your desktop background based on time of day."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `circadian_desktops-0.0.3/PKG-INFO` & `circadian_desktops-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circadian_desktops
-Version: 0.0.3
+Version: 0.0.4
 Summary: An app that changes your desktop background based on time of day.
 Project-URL: Homepage, https://github.com/Luke943/CircadianDesktops
 Project-URL: Bug Tracker, https://github.com/Luke943/CircadianDesktops/issues
 Author-email: Luke Hartley <luke.hartley05@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

