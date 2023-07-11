# Comparing `tmp/clera-0.0.8.tar.gz` & `tmp/clera-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clera-0.0.8.tar", last modified: Tue Jul  4 00:45:44 2023, max compression
+gzip compressed data, was "clera-0.1.0.tar", last modified: Tue Jul 11 00:33:43 2023, max compression
```

## Comparing `clera-0.0.8.tar` & `clera-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,46 @@
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-04 00:45:44.778245 clera-0.0.8/
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1127 2023-07-03 21:26:01.000000 clera-0.0.8/CHANGELOG.md
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-04-23 00:22:42.000000 clera-0.0.8/LICENCE.txt
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)       42 2023-04-01 11:31:56.000000 clera-0.0.8/MANIFEST.in
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3024 2023-07-04 00:45:44.778245 clera-0.0.8/PKG-INFO
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1259 2023-07-04 00:37:32.000000 clera-0.0.8/README.md
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-04 00:45:44.770248 clera-0.0.8/clera/
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      160 2023-07-03 21:11:09.000000 clera-0.0.8/clera/__init__.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    60519 2023-07-03 20:55:43.000000 clera-0.0.8/clera/core.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-04 00:45:44.774246 clera-0.0.8/clera/icons/
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)   290225 2023-02-13 13:07:36.000000 clera-0.0.8/clera/icons/hand-drawn-icon.png
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)    41561 2023-04-25 04:20:56.000000 clera-0.0.8/clera/icons/toon-icon.ico
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-04 00:45:44.774246 clera-0.0.8/clera/utils/
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      121 2023-03-19 13:16:12.000000 clera-0.0.8/clera/utils/__init__.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      129 2023-03-24 12:03:54.000000 clera-0.0.8/clera/utils/exceptions.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    18834 2023-07-02 22:56:52.000000 clera-0.0.8/clera/utils/handlers.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     1071 2023-03-19 13:17:06.000000 clera-0.0.8/clera/utils/keys.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     6431 2023-07-02 16:17:50.000000 clera-0.0.8/clera/utils/procr.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     4295 2023-07-03 00:25:19.000000 clera-0.0.8/clera/utils/style.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    27761 2023-07-03 00:12:08.000000 clera-0.0.8/clera/widgets.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-04 00:45:44.774246 clera-0.0.8/clera.egg-info/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3024 2023-07-04 00:45:44.000000 clera-0.0.8/clera.egg-info/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      442 2023-07-04 00:45:44.000000 clera-0.0.8/clera.egg-info/SOURCES.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-04 00:45:44.000000 clera-0.0.8/clera.egg-info/dependency_links.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        8 2023-07-04 00:45:44.000000 clera-0.0.8/clera.egg-info/requires.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        6 2023-07-04 00:45:44.000000 clera-0.0.8/clera.egg-info/top_level.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-04 00:45:44.778245 clera-0.0.8/setup.cfg
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1267 2023-07-03 21:16:42.000000 clera-0.0.8/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.433447 clera-0.1.0/
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1550 2023-07-11 00:15:16.000000 clera-0.1.0/CHANGELOG.md
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-04-23 00:22:42.000000 clera-0.1.0/LICENCE.txt
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)       48 2023-07-04 11:33:56.000000 clera-0.1.0/MANIFEST.in
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3467 2023-07-11 00:33:43.433447 clera-0.1.0/PKG-INFO
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1279 2023-07-08 18:13:25.000000 clera-0.1.0/README.md
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.389447 clera-0.1.0/clera/
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      194 2023-07-11 00:18:50.000000 clera-0.1.0/clera/__init__.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    61327 2023-07-09 14:12:05.000000 clera-0.1.0/clera/core.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.425447 clera-0.1.0/clera/icons/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       65 2023-07-04 11:49:49.000000 clera-0.1.0/clera/icons/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16293 2023-06-19 11:40:22.000000 clera-0.1.0/clera/icons/add-file.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13782 2023-06-19 03:37:40.000000 clera-0.1.0/clera/icons/close.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13430 2023-06-19 11:40:48.000000 clera-0.1.0/clera/icons/document.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16420 2023-06-19 03:41:00.000000 clera-0.1.0/clera/icons/documents.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15098 2023-06-19 03:38:16.000000 clera-0.1.0/clera/icons/gear.png
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)   290225 2023-02-13 13:07:36.000000 clera-0.1.0/clera/icons/hand-drawn-icon.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13536 2023-06-19 03:36:08.000000 clera-0.1.0/clera/icons/off.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    14518 2023-06-19 03:36:42.000000 clera-0.1.0/clera/icons/on.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15585 2023-06-19 03:38:52.000000 clera-0.1.0/clera/icons/save-as.png
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13421 2023-06-19 03:38:40.000000 clera-0.1.0/clera/icons/save.png
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)    41561 2023-04-25 04:20:56.000000 clera-0.1.0/clera/icons/toon-icon.ico
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.425447 clera-0.1.0/clera/scripts/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16531 2023-07-11 00:26:54.000000 clera-0.1.0/clera/scripts/editor.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.429447 clera-0.1.0/clera/stubs/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-03 14:47:26.000000 clera-0.1.0/clera/stubs/__init__.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    11965 2023-07-04 17:11:17.000000 clera-0.1.0/clera/stubs/core.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1176 2023-07-11 00:25:50.000000 clera-0.1.0/clera/stubs/handlers.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     7669 2023-07-08 14:35:34.000000 clera-0.1.0/clera/stubs/widgets.pyi
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.433447 clera-0.1.0/clera/utils/
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      120 2023-07-04 11:49:58.000000 clera-0.1.0/clera/utils/__init__.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      129 2023-03-24 12:03:54.000000 clera-0.1.0/clera/utils/exceptions.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    19722 2023-07-05 13:58:59.000000 clera-0.1.0/clera/utils/handlers.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     1071 2023-03-19 13:17:06.000000 clera-0.1.0/clera/utils/keys.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     6431 2023-07-02 16:17:50.000000 clera-0.1.0/clera/utils/procr.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     4295 2023-07-03 00:25:19.000000 clera-0.1.0/clera/utils/style.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    27822 2023-07-09 13:18:50.000000 clera-0.1.0/clera/widgets.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 00:33:43.389447 clera-0.1.0/clera.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3467 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      820 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       46 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/entry_points.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        8 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/requires.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        6 2023-07-11 00:33:42.000000 clera-0.1.0/clera.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-11 00:33:43.433447 clera-0.1.0/setup.cfg
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1340 2023-07-11 00:24:55.000000 clera-0.1.0/setup.py
```

### Comparing `clera-0.0.8/CHANGELOG.md` & `clera-0.1.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # **:- Change Log -:**
 
 > **0.0.1** -- [ 11 APRIL 2023 ]  
 > [ NOTICE ]  
 > [ ! ] - Initial Release
 
+> **0.0.2 - 0.0.5**  
+> [ INFO ]  
+> [+] Upload and Import Error
+
 > **0.0.6** -- [ 11 APRIL 2023 ]  
 > [ NOTICE ]  
 > [+] Module Install fixed
 
 > **0.0.7** -- [ 25 APRIL 2023 ]  
 > [ ADDED ]  
 > [+] Cursor change on titlebar drag  
@@ -22,21 +26,34 @@
 > [+] Window glitch using "Titlebar" element, "add" > and "update" method
 >
 > [ REMOVED ]  
 > [+] Clera default titlebar style
 
 > **0.0.8** -- [ 04 JULY 2023 ]  
 > [ ADDED ]  
-> [+] Extra controls of Window
-> [+] Stack Element for multi page development
-> [+] Extraction, Styling and Linking of Textarea scrollbar
-> [+] Wordwrap for Textarea
+> [+] Extra controls of Window  
+> [+] Stack Element for multi page development  
+> [+] Extraction, Styling and Linking of Textarea scrollbar  
+> [+] Wordwrap for Textarea  
 > [+] Popup Window lock
 >
 > [ FIXED ]  
 > [+] Windows style control icon  
-> [+] Fusion style control icon
+> [+] Fusion style control icon  
 > [+] File Element filter definition error
 >
 > [ CHANGED ]  
-> [+] Default window spacing and content margin
+> [+] Default window spacing and content margin  
 > [+] Stylesheet linking extension. Now only useds ".cx" extension
+
+> **0.1.0** -- [ 11 JULY 2023 ]  
+> [ ADDED ]  
+> [+] Quick argument values  
+> [+] Clera Style Editor
+>
+> [ CHANGED ]  
+> [+] sizepolicy declaration
+>
+> [ FIXED ]  
+> [+] ModuleNotFoundError: No module named 'clera.stubs'  
+> [+] Window icon display  
+> [+] AttributeError: 'MainWindow' object has no attribute 'old_position'
```

### Comparing `clera-0.0.8/LICENCE.txt` & `clera-0.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `clera-0.0.8/PKG-INFO` & `clera-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clera
-Version: 0.0.8
+Version: 0.1.0
 Summary: Write Simple and Quick Python GUI Application
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: GNU LGPLv3
 Keywords: gui,clera,simple,simplegui,pyside,pyside6,python,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -21,17 +21,17 @@
 ---
 
 _"This project is dedicated to my cousin who was like a mother to me. Though you are no longer with us, you will never be forgotten. May your memory be forever held in this project."_  
 -- **Bridget Trinity Vedjesu** --
 
 <br>
 
-<img src="https://github.com/cleragui/pypi/blob/main/image/icon.png?raw=true" style="width: 100px; margin: 0px auto; display: block;">
-
-<br>
+<div align="center">
+<img src="https://github.com/cleragui/pypi/blob/main/image/logo-with-name.png?raw=true">
+</div>
 
 ## **Clera - GUI Development with Python**
 
 ---
 
 Clera provides platform for developing python GUI quickly and simply with low learning curve.
 
@@ -74,26 +74,34 @@
 
 ### **OS Support**
 
 - Windows
 - Mac
 - Linux
 
----
+<br>
 
-### **SORRY😥, DOCUMENTATION NOT AVAILABLE YET❗**
+> INFO: Visit https://cleragui.github.io/ for documentation and more information.
+
+<br>
+
+---
 
 
 
 # **:- Change Log -:**
 
 > **0.0.1** -- [ 11 APRIL 2023 ]  
 > [ NOTICE ]  
 > [ ! ] - Initial Release
 
+> **0.0.2 - 0.0.5**  
+> [ INFO ]  
+> [+] Upload and Import Error
+
 > **0.0.6** -- [ 11 APRIL 2023 ]  
 > [ NOTICE ]  
 > [+] Module Install fixed
 
 > **0.0.7** -- [ 25 APRIL 2023 ]  
 > [ ADDED ]  
 > [+] Cursor change on titlebar drag  
@@ -108,21 +116,34 @@
 > [+] Window glitch using "Titlebar" element, "add" > and "update" method
 >
 > [ REMOVED ]  
 > [+] Clera default titlebar style
 
 > **0.0.8** -- [ 04 JULY 2023 ]  
 > [ ADDED ]  
-> [+] Extra controls of Window
-> [+] Stack Element for multi page development
-> [+] Extraction, Styling and Linking of Textarea scrollbar
-> [+] Wordwrap for Textarea
+> [+] Extra controls of Window  
+> [+] Stack Element for multi page development  
+> [+] Extraction, Styling and Linking of Textarea scrollbar  
+> [+] Wordwrap for Textarea  
 > [+] Popup Window lock
 >
 > [ FIXED ]  
 > [+] Windows style control icon  
-> [+] Fusion style control icon
+> [+] Fusion style control icon  
 > [+] File Element filter definition error
 >
 > [ CHANGED ]  
-> [+] Default window spacing and content margin
+> [+] Default window spacing and content margin  
 > [+] Stylesheet linking extension. Now only useds ".cx" extension
+
+> **0.1.0** -- [ 11 JULY 2023 ]  
+> [ ADDED ]  
+> [+] Quick argument values  
+> [+] Clera Style Editor
+>
+> [ CHANGED ]  
+> [+] sizepolicy declaration
+>
+> [ FIXED ]  
+> [+] ModuleNotFoundError: No module named 'clera.stubs'  
+> [+] Window icon display  
+> [+] AttributeError: 'MainWindow' object has no attribute 'old_position'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `clera-0.0.8/clera/core.py` & `clera-0.1.0/clera/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     'Menubar', 'menubar', 'Statusbar', 'statusbar', 'GET', 'get', 'Button', 'button', 'Input',
     'input', 'Text', 'text', 'Image', 'image', 'CheckBox', 'checkbox', 'RadioButton', 'radiobutton',
     'Textarea', 'textarea', 'item', 'empty', 'separator', 'Exit', 'exit', 'Copy', 'copy', 'Cut', 'cut',
     'Paste', 'paste', 'Undo', 'undo', 'Redo', 'redo', 'link', 'ListWidget', 'listwidget', 'ListItem',
     'tab', 'TabWidget', 'tabwidget', 'Select', 'select', 'option', 'ProgressBar', 'progressbar',
     'Slider', 'slider', 'Dial', 'dial', 'Popup', 'popup', 'call', 'Titlebar', 'titlebar', 'File', 'file',
     'Folder', 'folder', 'ScrollArea', 'scrollarea', 'minimize', 'maximize', 'close', 'title', 'Highlight',
-    'r', 'Stack'
+    'r', 'Stack', 'expand', 'fixed', 'vertical', 'horizontal', 'top', 'bottom', 'left', 'right', 'center',
+    'vcenter', 'hcenter', 'justify', 'static', 'normal', 'standard', 'password', 'noecho', 'extended',
+    'noselection', 'multi', 'single', 'windows', 'fusion', 'curve', 'breeze', 'oxygen','circle', 'square'
 ]
 
 
 app = start()
 
 DEFAULT_WINDOW_LAYOUT = QWidget()
 
@@ -171,23 +173,24 @@
 
         width, height = size
         if width != None or height != None:
             toolbar.setIconSize(QSize(width, height))
 
         toolbar_position = position.lower()
 
-        if toolbar_position == 'top':
-            self.addToolBar(Qt.TopToolBarArea, toolbar)
-        elif toolbar_position == 'bottom':
-            self.addToolBar(Qt.BottomToolBarArea, toolbar)
-        elif toolbar_position == 'left':
-            self.addToolBar(Qt.LeftToolBarArea, toolbar)
-        elif toolbar_position == 'right':
-            self.addToolBar(Qt.RightToolBarArea, toolbar)
-        else:
+        positions = {
+            top     : Qt.TopToolBarArea,
+            bottom  : Qt.BottomToolBarArea,
+            left    : Qt.LeftToolBarArea,
+            right   : Qt.RightToolBarArea
+        }
+
+        try:
+            self.addToolBar(positions[toolbar_position], toolbar)
+        except:
             raise ValueError(position)
 
         if tool_items != None:
             for item in tool_items:
                 if type(item) != type(list()):
                     widget_type, widget_items = check_func(item)
                     LayItOut(toolbar, widget_type, widget_items)
@@ -209,19 +212,30 @@
 
                     else:
                         pass
                         # DO NOTHING FOR NOW. SETUP LATER
 
         toolbar.setMovable(movable)
 
-        if orientation.lower() in DEFAULT_VERTICAL_TYPES:
-            toolbar.setOrientation(Qt.Vertical)
-        elif orientation.lower() in DEFAULT_HORIZONTAL_TYPES:
-            toolbar.setOrientation(Qt.Horizontal)
-        else:
+        orientations = {
+            vertical: Qt.Vertical,
+            horizontal: Qt.Horizontal
+        }
+
+        try:
+            if orientation.lower() in ['v', 'h']:
+                change = {
+                    'v': vertical,
+                    'h': horizontal
+                }
+
+                orientation = change[orientation.lower()]
+
+            toolbar.setOrientation(orientations[orientation.lower()])
+        except:
             raise ValueError(orientation)
 
         if border == False:
             toolbar.setStyleSheet('border-bottom: 0px')
 
     # Status bar functions
 
@@ -256,22 +270,25 @@
         if self._movable == True:
             window.setCursor(Qt.SizeAllCursor)
 
         self.old_position = event.globalPos()
         return self.old_position
 
     def mouseMoveEvent(self, event):
-        omega = QPoint(event.globalPos() - self.old_position)
+        try:
+            omega = QPoint(event.globalPos() - self.old_position)
 
-        if self._custom_title_bar == False and self._movable == True and self._frame == False:
-            self.move(self.x() + omega.x(), self.y() + omega.y())
-            self.old_position = event.globalPos()
-        else:
-            return omega
-    
+            if self._custom_title_bar == False and self._movable == True and self._frame == False:
+                self.move(self.x() + omega.x(), self.y() + omega.y())
+                self.old_position = event.globalPos()
+            else:
+                return omega
+        except:
+            ...
+        
     def mouseReleaseEvent(self, event: QMouseEvent):
         window.setCursor(Qt.ArrowCursor)
 
     def WindowTitlebar(self, icon, title, widgets, alignment, backgound_color,  text_color, height,
                        button_style):
         current_window_style = window.style().name().lower()
 
@@ -401,20 +418,24 @@
                     LayItOut(titlebar, widget_type, widget_items)
                     # titlebar.addWidget(widget)
 
             titlebar.setOrientation(Qt.Horizontal)
 
             button_style_query = button_style.lower()
 
-            if button_style_query == 'circle':
-                control_button_style = CONTROL_BUTTON_CIRCLE
-            elif button_style_query == 'square':
-                control_button_style = CONTROL_BUTTON_SQUARE
-            else:
+            button_styles = {
+                circle: CONTROL_BUTTON_CIRCLE,
+                square: CONTROL_BUTTON_SQUARE 
+            }
+
+            try:
+                control_button_style = button_styles[button_style_query]
+            except:
                 ...
+                # raise an error
 
             title = GET(TITLE_TEXT_ID)
             minimize = GET(MINIMIZE_BUTTON_ID)
             maximize = GET(MAXIMIZE_BUTTON_ID)
             close = GET(CLOSE_BUTTON_ID)
 
             def init_title_icon(icon, value: str = 'left'):
@@ -513,14 +534,15 @@
                 menu_bar = window.menuBar()
                 menu_bar.clear()
 
         except:
             ...
 
         app.exec()
+        self.quit()
 
     def quit(self):
         app.quit()
 
     def update(self, remove_id, widget):
         replace_widget = WIDGET_ID_SAFE[remove_id]
 
@@ -548,18 +570,21 @@
     def details(self):
         screen = window.screen().virtualSize()
         _title = window.windowTitle()
 
         if len(_title) == 0:
             _title = None
 
+        size = window.size()
+
         window_details = {
             'position': window.geometry().getCoords()[:2],
             'screen': (screen.width(), screen.height()),
             'style': window.style().name(),
+            'size': (size.width(), size.height()),
             'title': _title,
             'system_styles': QStyleFactory().keys()
         }
 
         return window_details
 
     def title(self, value: any = None):
@@ -890,31 +915,31 @@
 class titlebar(Titlebar):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class Toolbar:
     def __init__(self, name, tool_items: list | None = None, movable: bool = False,
-                 align: str = 'TOP', id: None = None, iconsize: tuple = (None, None),
+                 position: str = top, id: None = None, iconsize: tuple = (None, None),
                  border: bool = True, orientation: str = SET_HORIZONTAL, newline: bool = False):
         '''
         Toolbar Element
 
         :param name:
         :param tool_items:
         :param movable:
-        :param align:
+        :param position:
         :param id:
         :param iconsize:
         :param border:
         :param orientation:
         :param newline:
         '''
 
-        window.WindowToolbar(name,  tool_items, movable,  align,  id,  iconsize,  border,
+        window.WindowToolbar(name,  tool_items, movable,  position,  id,  iconsize,  border,
                              orientation, newline)
 
 
 class toolbar(Toolbar):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -1465,19 +1490,23 @@
             self.widget.paste()
 
     def clear(self):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA,
             GET_ELEM_TYPE_LISTWIDGET,
             GET_ELEM_TYPE_SELECT,
-            GET_ELEM_TYPE_TAB_WIDGET
+            GET_ELEM_TYPE_TAB_WIDGET,
+
+            GET_ELEM_TYPE_INPUT
         ]
 
-        if process_request(allowed, self.widget_type):
+        if process_request(allowed[0:4], self.widget_type):
             self.widget.clear()
+        elif process_request(allowed[4], self.widget_type):
+            self.widget.setText('')
 
     def add(self, items):
         allowed = [
             GET_ELEM_TYPE_LISTWIDGET,
             GET_ELEM_TYPE_SELECT,
             GET_ELEM_TYPE_TAB_WIDGET,
             GET_ELEM_TYPE_STACKED
@@ -1893,7 +1922,11 @@
 
 ###########################################################################
 ########################### CLERA STYLING EDITOR ##########################
 ###########################################################################
 
 # ------------------------------------------------------------------------#
 
+# def key():
+#     print(QStyleFactory.keys())
+
+# key()
```

### Comparing `clera-0.0.8/clera/icons/hand-drawn-icon.png` & `clera-0.1.0/clera/icons/hand-drawn-icon.png`

 * *Files identical despite different names*

### Comparing `clera-0.0.8/clera/icons/toon-icon.ico` & `clera-0.1.0/clera/icons/toon-icon.ico`

 * *Files identical despite different names*

### Comparing `clera-0.0.8/clera/utils/handlers.py` & `clera-0.1.0/clera/utils/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,41 +4,44 @@
 import inspect
 import re
 
 from PySide6.QtGui import QAction, QIcon, Qt, QTextCharFormat, QColor,QKeyEvent
 from PySide6.QtWidgets import QSizePolicy, QApplication
 from PySide6.QtWidgets import QListWidgetItem, QAbstractItemView, QComboBox
 
+from ..icons import *
 
 def start():
     app = QApplication(sys.argv)
     return app
 
 
 def call(func: None = None, *args, **kwargs):
     if func != None:
         return lambda function: func(*args, **kwargs)
 
-
 DEFAULT_WINDOW_TITLE = None
-DEFAULT_WINDOW_ICON = 'clera/icons/toon-icon.ico'
+DEFAULT_WINDOW_ICON = WINDOW_ICON
 DEFAULT_WINDOW_SIZE = (None, None)
 DEFAULT_WINDOW_FIXED_SIZE = (None, None)
 DEFAULT_WINDOW_STYLE = None
 DEFAULT_WINDOW_GEOMETRY = None
 DEFAULT_TAB_DISTANCE = 30
 
 
 WIDGET_ID_SAFE = {}
 ID_COUNT_DEFAULT = [0]
 TOOLBAR_COUNT = []
 LINK_ITEMS_INCLUDED = []
 
-SIZE_POLICY_EXPAND = 'expand'
-SIZE_POLICY_FIXED = 'fixed'
+SIZE_POLICY_EXPAND = expand = 'expand'
+SIZE_POLICY_FIXED = fixed = 'fixed'
+
+circle = 'circle'
+square = 'square'
 
 # GRAB_WIDGET = 'GrabWidget'
 
 DEFAULT_SEPARATOR_MARKER = '---'
 
 ELEM_TYPE_ITEM = 'item'
 ELEM_TYPE_SEPARATOR = 'separator'
@@ -66,50 +69,63 @@
 ELEM_TYPE_SCROLL_AREA = 'scrollarea'
 ELEM_TYPE_STACKED = 'stack'
 
 
 DEFAULT_VERTICAL_TYPES = ['vertical', 'v']
 DEFAULT_HORIZONTAL_TYPES = ['horizontal', 'h']
 
+vertical =DEFAULT_VERTICAL_TYPES[0]
+horizontal = DEFAULT_HORIZONTAL_TYPES[0]
+
 SET_HORIZONTAL = 'HORIZONTAL'
 SET_VERTICAL = 'VERTICAL'
 
-SET_NORMAL = 'NORMAL'
-SET_STATIC = 'STATIC'
+SET_NORMAL = normal = 'NORMAL'
+SET_STATIC = static ='STATIC'
 
-INPUT_TYPE_STANDARD = 'STANDARD'
-INPUT_TYPE_PASSWORD = 'PASSWORD'
-INPUT_TYPE_NO_ECHO = 'NO_ECHO'
+INPUT_TYPE_STANDARD = standard = 'STANDARD'
+INPUT_TYPE_PASSWORD = password = 'PASSWORD'
+INPUT_TYPE_NO_ECHO = noecho = 'NO_ECHO'
 
 
 GET_ELEM_TYPE_TEXTAREA = 'QTextEdit'
 GET_ELEM_TYPE_LISTWIDGET = 'QListWidget'
 GET_ELEM_TYPE_SELECT = 'QComboBox'
 GET_ELEM_TYPE_PROGRESS_BAR = 'QProgressBar'
 GET_ELEM_TYPE_SLIDER = 'QSlider'
 GET_ELEM_TYPE_DIAL = 'QDial'
 GET_ELEM_TYPE_TAB_WIDGET = 'QTabWidget'
 GET_ELEM_TYPE_POPUP = 'QDialog'
 GET_ELEM_TYPE_INPUT = 'QLineEdit'
 GET_ELEM_TYPE_STACKED = 'QStackedWidget'
 # GET_ELEM_TYPE_SCROLLAREA = 'QScrollArea'
 
-ITEM_SELECTION_MODE_EXTENDED = 'extended'
-ITEM_SELECTION_MODE_NO_SELECTION = 'no_selection'
-ITEM_SELECTION_MODE_MULTI = 'multi'
-ITEM_SELECTION_MODE_SINGLE = 'single'
+ITEM_SELECTION_MODE_EXTENDED = extended = 'extended'
+ITEM_SELECTION_MODE_NO_SELECTION = noselection= 'no_selection'
+ITEM_SELECTION_MODE_MULTI = multi = 'multi'
+ITEM_SELECTION_MODE_SINGLE = single = 'single'
 
 
 PRE_INIT_COPY = 'copy'
 PRE_INIT_CUT = 'cut'
 PRE_INIT_PASTE = 'paste'
 PRE_INIT_UNDO = 'undo'
 PRE_INIT_REDO = 'redo'
 
 
+center = 'center'
+right = 'right'
+left = 'left'
+top = 'top'
+bottom = 'bottom'
+hcenter = 'hcenter'
+vcenter = 'vcenter'
+justify = 'justify'
+
+
 CUSTOM_TITLEBAR_HEIGHT = 5
 
 CONTROL_BUTTON_CIRCLE = '10px'
 CONTROL_BUTTON_SQUARE = '0'
 
 DEFAULT_BUTTON_STYLE = 'circle'
 
@@ -118,16 +134,19 @@
 
 DEFAULT_OPEN_FILE_TYPE = OPEN_FILE_TYPE_SINGLE
 
 FILTER_SPLIT_MARKER = '&'
 
 CONTROL_CLOSE = '⨯'
 
-SYSTEM_PLATFORM_WINDOWS = 'windows'
-SYSTEM_PLATFORM_FUSION = 'fusion'
+SYSTEM_PLATFORM_WINDOWS = windows = 'windows'
+SYSTEM_PLATFORM_FUSION = fusion = 'fusion'
+SYSTEM_PLATFORM_CURVE = curve = 'qtcurve'
+SYSTEM_PLATFORM_OXYGEN = oxygen = 'oxygen'
+SYSTEM_PLATFORM_BREEZE = breeze = 'breeze'
 
 ICON_IMAGE_ID = '-clera_icon-'
 TITLE_TEXT_ID = '-clera_title-'
 MINIMIZE_BUTTON_ID = '-clera_minimize_button-'
 MAXIMIZE_BUTTON_ID = '-clera_maximize_button-'
 CLOSE_BUTTON_ID = '-clera_close_button-'
 
@@ -193,45 +212,57 @@
     if shortcut != None:
         Action.setShortcut(shortcut)
 
     return Action
 
 
 def set_size_policy(widget, sizepolicy):
-
-    horizontal_policy, vertical_policy = sizepolicy
-
-    if horizontal_policy != None and vertical_policy != None:
-        horizontal = horizontal_policy.lower()
-        vertical = vertical_policy.lower()
-
-        if horizontal == SIZE_POLICY_FIXED:
-            horizontal = QSizePolicy.Fixed
-        elif horizontal == SIZE_POLICY_EXPAND:
-            horizontal = QSizePolicy.Expanding
-        else:
-            raise ValueError(horizontal_policy)
-
-        if vertical == SIZE_POLICY_FIXED:
-            vertical = QSizePolicy.Fixed
-        elif vertical == SIZE_POLICY_EXPAND:
-            vertical = QSizePolicy.Expanding
+    policy = {
+        'fixed'     : QSizePolicy.Fixed,
+        'expand'    : QSizePolicy.Expanding
+    }
+
+    def init_single_policy(sizepolicy):
+        if sizepolicy == SIZE_POLICY_EXPAND or sizepolicy == SIZE_POLICY_FIXED:
+            return (policy[sizepolicy], policy[sizepolicy])
+
+    if type(sizepolicy) == sample_tuple:
+        if len(sizepolicy) == 2:
+            horizontal_policy, vertical_policy = sizepolicy
+
+            if horizontal_policy != None and vertical_policy != None:
+                horizontal = horizontal_policy.lower()
+                vertical = vertical_policy.lower()
+
+                try:
+                    vertical = policy[vertical]
+                    horizontal = policy[horizontal]
+                except:
+                    raise ValueError(sizepolicy)
+        elif len(sizepolicy) == 1:
+            horizontal, vertical = init_single_policy(sizepolicy)
         else:
-            raise ValueError(vertical_policy)
-
+            ...
+            # raise an error
+    elif type(sizepolicy) == sample_string:
+        horizontal, vertical = init_single_policy(sizepolicy)
+    
+    try:
         widget.setSizePolicy(horizontal, vertical)
-
+    except:
+        ...
+        # raise an error
 
 def set_widget(lyt, grid, widget, grid_pos_x, grid_pos_y):
-    gridx, gridy = grid  # horizontal and vertical occupy rule for grid widgets
+    gridy, gridx = grid  # vertical (y) and horizontal (x) occupy rule for grid widgets
 
     if type(lyt) != sample_list and type(lyt) != sample_string:
         if grid_pos_x != None and grid_pos_y != None:
             if gridx != None and gridy != None:
-                lyt.addWidget(widget, grid_pos_x, grid_pos_y, gridx, gridy)
+                lyt.addWidget(widget, grid_pos_x, grid_pos_y, gridy, gridx)
             else:
                 lyt.addWidget(widget, grid_pos_x, grid_pos_y)
         else:
             lyt.addWidget(widget)
     else:
         if len(lyt) == 2:
             lyt, _type = lyt
@@ -247,30 +278,31 @@
             if _type == 'replaceWidget':
                 layout.replaceWidget(pre_widget, widget)
 
 
 def make_alignment(widget, alignments):
     def alignCheck(widget_alignment):
         alignment = widget_alignment.lower()
-        if alignment == 'center':
-            align = Qt.AlignCenter
-        elif alignment == 'right':
-            align = Qt.AlignRight
-        elif alignment == 'left':
-            align = Qt.AlignLeft
-        elif alignment == 'bottom':
-            align = Qt.AlignBottom
-        elif alignment == 'hcenter':
-            align = Qt.AlignHCenter
-        elif alignment == 'vcenter':
-            align = Qt.AlignVCenter
-        elif alignment == 'justify':
-            align = Qt.AlignJustify
-        elif alignment == 'top':
-            align = Qt.AlignTop
+
+        alignment_map = {
+            center      : Qt.AlignCenter,
+            right       : Qt.AlignRight,
+            left        : Qt.AlignLeft,
+            top         : Qt.AlignTop,
+            bottom      : Qt.AlignBottom,
+            hcenter     : Qt.AlignHCenter,
+            vcenter     : Qt.AlignVCenter,
+            justify     : Qt.AlignJustify
+        }
+        
+        try:
+            align = alignment_map[alignment]
+        except:
+            ...
+            # raise an error
 
         return align
 
     align = alignCheck(alignments)
     widget.setAlignment(align)
 
 
@@ -493,23 +525,22 @@
 def pre_widget_process(widget_type):
     id = widget_type + str(PRE_WIDGETS_COUNT[0])
     PRE_WIDGETS_COUNT[0] += 1
 
     return ELEM_TYPE_BUTTON, id
 
 
-def sample_func():
-    pass
+def sample_func(): ...
 
 
 sample_string = type(str())
 
 sample_list = type(list())
 
-sample_function = type(sample_func())
+sample_function = type(sample_func)
 
 sample_integer = type(int())
 
 sample_tuple = type(tuple())
 
 if SYSTEM_OS_PLATFORM == 'linux':
     minimize_padding = ' padding: 1px 7px 2px 7px'
```

### Comparing `clera-0.0.8/clera/utils/keys.py` & `clera-0.1.0/clera/utils/keys.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.8/clera/utils/procr.py` & `clera-0.1.0/clera/utils/procr.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.8/clera/utils/style.py` & `clera-0.1.0/clera/utils/style.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.8/clera/widgets.py` & `clera-0.1.0/clera/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 
 
 def window_button(lyt, button_text, func, icon,
                   ID, disabled, default, sizepolicy, grid, grid_pos_x, grid_pos_y, checkable,
                   checked, hidden, focus, icon_size, statustip, tooltip, shortcut):
 
     button = INIT_WIDGET(ID, QPushButton(button_text))
-
     set_widget(lyt, grid, button, grid_pos_x, grid_pos_y)
     set_size_policy(button, sizepolicy)
 
     button.setStatusTip(statustip)
     button.setToolTip(tooltip)
     if shortcut != None:
         button.setShortcut(shortcut)
@@ -445,15 +444,15 @@
 
 
 class RadioButton:
     def __init__(self, label: any = '', checked: bool = False, id: any = None,
                  toggled: None = None, grid: tuple = (None, None),
                  sizepolicy: tuple = (None, None)):
         '''
-        Checkbox Widget
+        RadioButton Widget
 
         :param label:
         :param checked:
         :param id:
         :param stateChanged:
         :param toggled:
         :param grid:
@@ -487,17 +486,18 @@
 
     textarea = INIT_WIDGET(ID, QTextEdit())
 
     set_widget(lyt, grid, textarea, grid_pos_x, grid_pos_y)
     set_size_policy(textarea, sizepolicy)
     
     #  set word wrap for textedit
-    if wordwrap:
+    if not wordwrap:
         textarea.setLineWrapMode(textarea.LineWrapMode.NoWrap)
 
+    textarea.setHidden(hidden)
     textarea.setDisabled(disabled)
     textarea.setReadOnly(readonly)
     textarea.setText(value)
     textarea.setPlaceholderText(placeholder)
 
     textarea.textChanged.connect(text_changed)
     textarea.selectionChanged.connect(selection_changed)
@@ -524,15 +524,15 @@
     def __init__(self, id: any = None, placeholder: any = None,
                  hidden: bool = False, alignment: str = None, value: any = None,
                  disabled: bool = False, readonly: bool = False, text_changed: None = None,
                  selection_changed: None = None, undo_available: None = None,
                  redo_available: None = None, maxlength: int | None = None, font: str | None = None,
                  fontsize: int | None = None, sizepolicy: tuple = (None, None),
                  grid: tuple = (None, None), tabwidth: int = DEFAULT_TAB_DISTANCE,
-                 wordwrap: bool = False):
+                 wordwrap: bool = True):
         '''
         Textarea Widget
 
         :param id:
         :param placeholder
         :param hidden:
         :param alignment:
@@ -545,14 +545,15 @@
         :param redo_available:
         :param maxlegth:
         :param font:
         :param fontsize:
         :param sizepolicy:
         :param grid:
         :param tabWidth:
+        :param wordwrap:
         '''
         elem_type = ELEM_TYPE_TEXTAREA
         self.rtn = [elem_type, id, placeholder, hidden, alignment, value, disabled, readonly, text_changed,
                     selection_changed, undo_available, redo_available, maxlength, font, fontsize, sizepolicy, grid,
                     tabwidth, wordwrap]
 
     def __call__(self):
```

### Comparing `clera-0.0.8/clera.egg-info/PKG-INFO` & `clera-0.1.0/clera.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clera
-Version: 0.0.8
+Version: 0.1.0
 Summary: Write Simple and Quick Python GUI Application
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: GNU LGPLv3
 Keywords: gui,clera,simple,simplegui,pyside,pyside6,python,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -21,17 +21,17 @@
 ---
 
 _"This project is dedicated to my cousin who was like a mother to me. Though you are no longer with us, you will never be forgotten. May your memory be forever held in this project."_  
 -- **Bridget Trinity Vedjesu** --
 
 <br>
 
-<img src="https://github.com/cleragui/pypi/blob/main/image/icon.png?raw=true" style="width: 100px; margin: 0px auto; display: block;">
-
-<br>
+<div align="center">
+<img src="https://github.com/cleragui/pypi/blob/main/image/logo-with-name.png?raw=true">
+</div>
 
 ## **Clera - GUI Development with Python**
 
 ---
 
 Clera provides platform for developing python GUI quickly and simply with low learning curve.
 
@@ -74,26 +74,34 @@
 
 ### **OS Support**
 
 - Windows
 - Mac
 - Linux
 
----
+<br>
 
-### **SORRY😥, DOCUMENTATION NOT AVAILABLE YET❗**
+> INFO: Visit https://cleragui.github.io/ for documentation and more information.
+
+<br>
+
+---
 
 
 
 # **:- Change Log -:**
 
 > **0.0.1** -- [ 11 APRIL 2023 ]  
 > [ NOTICE ]  
 > [ ! ] - Initial Release
 
+> **0.0.2 - 0.0.5**  
+> [ INFO ]  
+> [+] Upload and Import Error
+
 > **0.0.6** -- [ 11 APRIL 2023 ]  
 > [ NOTICE ]  
 > [+] Module Install fixed
 
 > **0.0.7** -- [ 25 APRIL 2023 ]  
 > [ ADDED ]  
 > [+] Cursor change on titlebar drag  
@@ -108,21 +116,34 @@
 > [+] Window glitch using "Titlebar" element, "add" > and "update" method
 >
 > [ REMOVED ]  
 > [+] Clera default titlebar style
 
 > **0.0.8** -- [ 04 JULY 2023 ]  
 > [ ADDED ]  
-> [+] Extra controls of Window
-> [+] Stack Element for multi page development
-> [+] Extraction, Styling and Linking of Textarea scrollbar
-> [+] Wordwrap for Textarea
+> [+] Extra controls of Window  
+> [+] Stack Element for multi page development  
+> [+] Extraction, Styling and Linking of Textarea scrollbar  
+> [+] Wordwrap for Textarea  
 > [+] Popup Window lock
 >
 > [ FIXED ]  
 > [+] Windows style control icon  
-> [+] Fusion style control icon
+> [+] Fusion style control icon  
 > [+] File Element filter definition error
 >
 > [ CHANGED ]  
-> [+] Default window spacing and content margin
+> [+] Default window spacing and content margin  
 > [+] Stylesheet linking extension. Now only useds ".cx" extension
+
+> **0.1.0** -- [ 11 JULY 2023 ]  
+> [ ADDED ]  
+> [+] Quick argument values  
+> [+] Clera Style Editor
+>
+> [ CHANGED ]  
+> [+] sizepolicy declaration
+>
+> [ FIXED ]  
+> [+] ModuleNotFoundError: No module named 'clera.stubs'  
+> [+] Window icon display  
+> [+] AttributeError: 'MainWindow' object has no attribute 'old_position'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `clera-0.0.8/setup.py` & `clera-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     with codecs.open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as changelog:
         LONG_DESCRIPTION = readme.read() + '\n\n\n' + changelog.read()
 
 
-VERSION = '0.0.8'
+VERSION = '0.1.0'
 DESCRIPTION = 'Write Simple and Quick Python GUI Application'
 KEYWORDS = ['gui', 'clera', 'simple', 'simplegui', 'pyside', 'pyside6', 'python', 'easy']
 
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
@@ -34,9 +34,10 @@
     licence='GNU LGPLv3',
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=['PySide6'],
     keywords=KEYWORDS,
     classifiers=CLASSIFIERS,
-    py_modules=['clera']
+    py_modules=['clera'],
+    entry_points = {'console_scripts':['clera-editor = clera:editor']},
 )
```

