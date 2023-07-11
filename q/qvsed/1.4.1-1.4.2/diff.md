# Comparing `tmp/qvsed-1.4.1.tar.gz` & `tmp/qvsed-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.4.1.tar", last modified: Sun Jul  9 16:32:53 2023, max compression
+gzip compressed data, was "qvsed-1.4.2.tar", last modified: Tue Jul 11 10:30:54 2023, max compression
```

## Comparing `qvsed-1.4.1.tar` & `qvsed-1.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 16:32:53.068050 qvsed-1.4.1/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-09 16:32:53.068050 qvsed-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     7077 2023-07-09 16:31:54.000000 qvsed-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 16:32:53.029254 qvsed-1.4.1/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.4.1/qvsed/__init__.py
--rw-rw-rw-   0        0        0      477 2023-07-09 16:20:45.000000 qvsed-1.4.1/qvsed/config_default.py
--rw-rw-rw-   0        0        0    21540 2023-07-09 16:29:20.000000 qvsed-1.4.1/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.4.1/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-09 16:32:53.066260 qvsed-1.4.1/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 16:32:53.068050 qvsed-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-09 16:32:34.000000 qvsed-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:30:54.267143 qvsed-1.4.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-11 10:30:54.266131 qvsed-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7077 2023-07-09 16:31:54.000000 qvsed-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 10:30:54.232860 qvsed-1.4.2/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.4.2/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-07-11 10:13:29.000000 qvsed-1.4.2/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    22482 2023-07-11 10:27:11.000000 qvsed-1.4.2/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.4.2/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-11 10:30:54.264068 qvsed-1.4.2/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-11 10:30:54.000000 qvsed-1.4.2/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-11 10:30:54.000000 qvsed-1.4.2/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 10:30:54.000000 qvsed-1.4.2/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-11 10:30:54.000000 qvsed-1.4.2/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 10:30:54.000000 qvsed-1.4.2/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 10:30:54.000000 qvsed-1.4.2/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 10:30:54.267143 qvsed-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-11 10:28:01.000000 qvsed-1.4.2/setup.py
```

### Comparing `qvsed-1.4.1/LICENSE.txt` & `qvsed-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.1/PKG-INFO` & `qvsed-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.4.1
+Version: 1.4.2
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.4.1/README.md` & `qvsed-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.1/qvsed/qvsed.py` & `qvsed-1.4.2/qvsed/qvsed.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 A cross-platform simple and volatile text editor by Arsalan Kazmi
 See README.md or "Get Help" inside QVSED for more info
 """
 
 # pylint: disable=no-name-in-module
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=broad-exception-caught
+# pylint: disable=line-too-long
 
 import os
 import sys
 import shutil
 import importlib.util
 import pkg_resources
 from PyQt5.QtWidgets import (
@@ -65,15 +66,18 @@
         self.set_up_action_deck()
         self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
         self.load_config()
         self.set_up_fonts()
         if self.check_if_file_parameter():
             self.load_from_file(sys.argv[1])
 
-    def apply_style_sheet(self, text_color, background_color, button_color, button_hover_color, button_pressed_color, text_area_color, echo_area_color):
+    def apply_style_sheet(self, text_color, background_color, button_color,
+                          button_hover_color, button_pressed_color, text_area_color,
+                          echo_area_color, scroll_bar_color, scroll_bar_background_color,
+                          scroll_bar_hover_color, scroll_bar_pressed_color):
         """
         Generate and apply a style sheet based on the config.py file.
         """
 
         stylesheet = f"""
 QMainWindow {{
     color: {text_color};
@@ -109,26 +113,30 @@
 
 QPushButton:pressed {{
     color: {text_color};
     background: {button_pressed_color};
 }}
 
 QScrollBar:vertical {{
-    background-color: {button_hover_color};
+    background-color: {scroll_bar_background_color};
     width: 16px;
     margin: 16px 0 16px 0;
 }}
 
 QScrollBar::handle:vertical {{
-    background-color: {button_color};
+    background-color: {scroll_bar_color};
     min-height: 20px;
 }}
 
 QScrollBar::handle:vertical:hover {{
-    background-color: {button_color};
+    background-color: {scroll_bar_hover_color};
+}}
+
+QScrollBar::handle:vertical:pressed {{
+    background-color: {scroll_bar_pressed_color};
 }}
 
 QScrollBar::add-line:vertical, QScrollBar::sub-line:vertical {{
     background: none;
 }}
 
 QScrollBar::add-page:vertical, QScrollBar::sub-page:vertical {{
@@ -313,20 +321,32 @@
         self.font_family = qvsed_config.font_family
         self.font_size = qvsed_config.font_size
 
         # Load the colour scheme settings from the config file
         # We use the shorter American spellings because it's standard, I guess
         text_color = getattr(qvsed_config, 'text_color', None)
         background_color = getattr(qvsed_config, 'background_color', None)
+
         button_color = getattr(qvsed_config, 'button_color', None)
         button_hover_color = getattr(qvsed_config, 'button_hover_color', getattr(qvsed_config, 'button_focus_color', None))
         button_pressed_color = getattr(qvsed_config, 'button_pressed_color', background_color)
+
         text_area_color = getattr(qvsed_config, 'text_area_color', button_hover_color)
         echo_area_color = getattr(qvsed_config, 'echo_area_color', button_hover_color)
-        self.apply_style_sheet(text_color, background_color, button_color, button_hover_color, button_pressed_color, text_area_color, echo_area_color)
+
+        scroll_bar_color = getattr(qvsed_config, 'scroll_bar_color', button_color)
+        scroll_bar_background_color = getattr(qvsed_config, 'scroll_bar_background_color', button_hover_color)
+        scroll_bar_hover_color = getattr(qvsed_config, 'scroll_bar_hover_color', button_pressed_color)
+        scroll_bar_pressed_color = getattr(qvsed_config, 'scroll_bar_pressed_color', button_pressed_color)
+
+        self.apply_style_sheet(text_color, background_color, button_color,
+                               button_hover_color, button_pressed_color, text_area_color,
+                               echo_area_color, scroll_bar_color, scroll_bar_background_color,
+                               scroll_bar_hover_color, scroll_bar_pressed_color)
+
         if None in (text_color, background_color, button_color, button_hover_color):
             self.echo_area_update("config.py appears to be broken, generating a new one.")
             self.generate_config()
 
     def load_from_file(self, file_path = None):
         """
         Open a file dialog, and load the contents of a file into the Text Area.
```

### Comparing `qvsed-1.4.1/qvsed/qvsed.ui` & `qvsed-1.4.2/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.1/qvsed.egg-info/PKG-INFO` & `qvsed-1.4.2/qvsed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.4.1
+Version: 1.4.2
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.4.1/setup.py` & `qvsed-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.4.1',
+    version='1.4.2',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

