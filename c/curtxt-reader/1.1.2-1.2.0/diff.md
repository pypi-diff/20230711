# Comparing `tmp/curtxt-reader-1.1.2.tar.gz` & `tmp/curtxt-reader-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curtxt-reader-1.1.2.tar", last modified: Fri Jul  7 15:24:33 2023, max compression
+gzip compressed data, was "curtxt-reader-1.2.0.tar", last modified: Tue Jul 11 17:19:45 2023, max compression
```

## Comparing `curtxt-reader-1.1.2.tar` & `curtxt-reader-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-07-07 15:24:33.226285 curtxt-reader-1.1.2/
--rw-r--r--   0 iris      (1000) iris      (1000)    16725 2023-06-19 15:58:49.000000 curtxt-reader-1.1.2/LICENSE
--rw-r--r--   0 iris      (1000) iris      (1000)    21772 2023-07-07 15:24:33.222951 curtxt-reader-1.1.2/PKG-INFO
--rw-r--r--   0 iris      (1000) iris      (1000)     1326 2023-07-07 13:59:44.000000 curtxt-reader-1.1.2/README.md
--rwxr-xr-x   0 iris      (1000) iris      (1000)     9797 2023-07-07 15:23:03.000000 curtxt-reader-1.1.2/curtxt.py
-drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-07-07 15:24:33.222951 curtxt-reader-1.1.2/curtxt_reader.egg-info/
--rw-r--r--   0 iris      (1000) iris      (1000)    21772 2023-07-07 15:24:33.000000 curtxt-reader-1.1.2/curtxt_reader.egg-info/PKG-INFO
--rw-r--r--   0 iris      (1000) iris      (1000)      230 2023-07-07 15:24:33.000000 curtxt-reader-1.1.2/curtxt_reader.egg-info/SOURCES.txt
--rw-r--r--   0 iris      (1000) iris      (1000)        1 2023-07-07 15:24:33.000000 curtxt-reader-1.1.2/curtxt_reader.egg-info/dependency_links.txt
--rw-r--r--   0 iris      (1000) iris      (1000)       39 2023-07-07 15:24:33.000000 curtxt-reader-1.1.2/curtxt_reader.egg-info/entry_points.txt
--rw-r--r--   0 iris      (1000) iris      (1000)        7 2023-07-07 15:24:33.000000 curtxt-reader-1.1.2/curtxt_reader.egg-info/top_level.txt
--rw-r--r--   0 iris      (1000) iris      (1000)      889 2023-07-01 09:14:12.000000 curtxt-reader-1.1.2/pyproject.toml
--rw-r--r--   0 iris      (1000) iris      (1000)       38 2023-07-07 15:24:33.226285 curtxt-reader-1.1.2/setup.cfg
+drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-07-11 17:19:45.257047 curtxt-reader-1.2.0/
+-rw-r--r--   0 iris      (1000) iris      (1000)    16725 2023-06-19 15:58:49.000000 curtxt-reader-1.2.0/LICENSE
+-rw-r--r--   0 iris      (1000) iris      (1000)    21719 2023-07-11 17:19:45.257047 curtxt-reader-1.2.0/PKG-INFO
+-rw-r--r--   0 iris      (1000) iris      (1000)     1260 2023-07-11 17:04:49.000000 curtxt-reader-1.2.0/README.md
+-rwxr-xr-x   0 iris      (1000) iris      (1000)    11017 2023-07-11 17:01:08.000000 curtxt-reader-1.2.0/curtxt.py
+drwxr-xr-x   0 iris      (1000) iris      (1000)        0 2023-07-11 17:19:45.257047 curtxt-reader-1.2.0/curtxt_reader.egg-info/
+-rw-r--r--   0 iris      (1000) iris      (1000)    21719 2023-07-11 17:19:45.000000 curtxt-reader-1.2.0/curtxt_reader.egg-info/PKG-INFO
+-rw-r--r--   0 iris      (1000) iris      (1000)      230 2023-07-11 17:19:45.000000 curtxt-reader-1.2.0/curtxt_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)        1 2023-07-11 17:19:45.000000 curtxt-reader-1.2.0/curtxt_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)       39 2023-07-11 17:19:45.000000 curtxt-reader-1.2.0/curtxt_reader.egg-info/entry_points.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)        7 2023-07-11 17:19:45.000000 curtxt-reader-1.2.0/curtxt_reader.egg-info/top_level.txt
+-rw-r--r--   0 iris      (1000) iris      (1000)      902 2023-07-11 17:06:35.000000 curtxt-reader-1.2.0/pyproject.toml
+-rw-r--r--   0 iris      (1000) iris      (1000)       38 2023-07-11 17:19:45.257047 curtxt-reader-1.2.0/setup.cfg
```

### Comparing `curtxt-reader-1.1.2/LICENSE` & `curtxt-reader-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `curtxt-reader-1.1.2/PKG-INFO` & `curtxt-reader-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtxt-reader
-Version: 1.1.2
+Version: 1.2.0
 Summary: A simple ncurses-based plain text reader
 Author-email: 1256-bits <128bit@eclipso.eu>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -379,15 +379,15 @@
         
 Project-URL: Homepage, https://github.com/1256-bits/curses-txt-reader
 Project-URL: Source, https://github.com/1256-bits/curses-txt-reader
 Keywords: reader,plain text,txt,text,ncurses
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Curses txt reader
@@ -425,12 +425,8 @@
 * B - toggle progress bar
 * Home - got to the first page
 * End - go to the last page
 ### Command line options:
 
     -h, --help - pring help message and exit
     -v, --version - print version number and exit
-
-### Feature roadmap
-- Bookmarks
-- Resize the window if the terminal is resized
-- Clear history option
+    -c, --clear - clear history file
```

### Comparing `curtxt-reader-1.1.2/README.md` & `curtxt-reader-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,12 +33,8 @@
 * B - toggle progress bar
 * Home - got to the first page
 * End - go to the last page
 ### Command line options:
 
     -h, --help - pring help message and exit
     -v, --version - print version number and exit
-
-### Feature roadmap
-- Bookmarks
-- Resize the window if the terminal is resized
-- Clear history option
+    -c, --clear - clear history file
```

### Comparing `curtxt-reader-1.1.2/curtxt.py` & `curtxt-reader-1.2.0/curtxt.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,30 +12,42 @@
 class main_window:
     # SUMS of both left and right margins
     MARGINS_X = 4
     MARGINS_Y = 8
 
     def __init__(self):
         # COLS and LINES count from 1, height and width count from 1
-        self.height = curses.LINES - main_window.MARGINS_Y
+        self.height = curses.LINES - main_window.MARGINS_Y if curses.LINES > 40 else curses.LINES - 4
         self.input_raw = self.__get_raw_input()
         self.hash = md5("".join(self.input_raw).encode("UTF-8")).hexdigest()
         self.output_lines = self.__get_output_lines()
         self.longest_line_len = len(max(self.output_lines, key=len)) or 80
         # The number of pages that fit on the screen
         self.page_count = self.__get_page_count()
         self.width = (self.longest_line_len + 1) * self.page_count + 3
         self.start_x = trunc((curses.COLS - self.longest_line_len * self.page_count - 4) / 2)
-        self.start_y = trunc(main_window.MARGINS_Y / 2)
+        self.start_y = trunc(main_window.MARGINS_Y / 2) if curses.LINES > 40 else 2
         # The actual pages with text. len() them for actual page count
         self.pages = self.__fill_pages()
         self.current_page = 0
         del self.output_lines
         self.__create_window()
 
+    def resize(self):
+        self.height = curses.LINES - main_window.MARGINS_Y if curses.LINES > 40 else curses.LINES - 4
+        self.output_lines = self.__get_output_lines()
+        self.longest_line_len = len(max(self.output_lines, key=len)) or 80
+        self.page_count = self.__get_page_count()
+        self.width = (self.longest_line_len + 1) * self.page_count + 3
+        self.start_x = trunc((curses.COLS - self.longest_line_len * self.page_count - 4) / 2)
+        self.start_y = trunc(main_window.MARGINS_Y / 2) if curses.LINES > 40 else 2
+        self.pages = self.__fill_pages()
+        del self.output_lines
+        self.__create_window()
+
     def __get_raw_input(self):
         # How are you going to resize if you keep it inside of the class?
         if (len(argv) > 1) and not (os.path.exists(argv[1])):
             curses.endwin()
             print(f'File {argv[1]} not found')
             exit()
         if (len(argv) > 1):
@@ -215,14 +227,23 @@
                 bar_win.toggle_bar()
             case "KEY_HOME":
                 window.go_to_line(0)
                 bar_win.update_bar(window.get_current_page())
             case "KEY_END":
                 window.go_to_page(window.get_last_page())
                 bar_win.update_bar(window.get_current_page())
+            case "KEY_RESIZE":
+                if (curses.is_term_resized(curses.LINES, curses.COLS)):
+                    y, x = scr.getmaxyx()
+                    curses.resizeterm(y, x)
+                    scr.clear()
+                    scr.refresh()
+                    window.resize()
+                    del bar_win
+                    bar_win = bar(window.get_text_page_count(), window.get_current_page())
             case _:
                 if (re.match(r"\d+", char)):
                     page_num = [char]
                     while (not char.lower() == "g"):
                         char = scr.getkey()
                         if (re.match(r"\d+", char)):
                             page_num.append(char)
@@ -240,21 +261,24 @@
     if (os.path.isfile(histfile_path)):
         return yaml.load(open(histfile_path).read(), yaml.SafeLoader) or {}
     open(histfile_path, "x").close()
     return {}
 
 
 def init():
-    help_text = """Usage:
+    help_text = """Curses txt reader
+Usage:
     command | curtxt
     curtxt file
 Options:
     -h, --help - pring this message and exit
-    -v, --version - print version number and exit"""
+    -v, --version - print version number and exit
+    -c, --clear - clear history file"""
     if os.isatty(0) and (len(argv) == 1):
+        print(help_text)
         exit()
     match argv[1]:
         case "--version" | "-v":
             print("Version 1.1.2")
             exit()
         case "--help" | "-h":
             print(help_text)
```

### Comparing `curtxt-reader-1.1.2/curtxt_reader.egg-info/PKG-INFO` & `curtxt-reader-1.2.0/curtxt_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtxt-reader
-Version: 1.1.2
+Version: 1.2.0
 Summary: A simple ncurses-based plain text reader
 Author-email: 1256-bits <128bit@eclipso.eu>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -379,15 +379,15 @@
         
 Project-URL: Homepage, https://github.com/1256-bits/curses-txt-reader
 Project-URL: Source, https://github.com/1256-bits/curses-txt-reader
 Keywords: reader,plain text,txt,text,ncurses
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Curses txt reader
@@ -425,12 +425,8 @@
 * B - toggle progress bar
 * Home - got to the first page
 * End - go to the last page
 ### Command line options:
 
     -h, --help - pring help message and exit
     -v, --version - print version number and exit
-
-### Feature roadmap
-- Bookmarks
-- Resize the window if the terminal is resized
-- Clear history option
+    -c, --clear - clear history file
```

### Comparing `curtxt-reader-1.1.2/pyproject.toml` & `curtxt-reader-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "curtxt-reader"
-version = "1.1.2"
+version = "1.2.0"
 description = "A simple ncurses-based plain text reader"
 readme = "README.md"
 authors = [{ name = "1256-bits" , email = "128bit@eclipso.eu" }]
 classifiers = [
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console :: Curses",
     "Intended Audience :: End Users/Desktop"
 ]
 keywords = ["reader", "plain text", "txt", "text", "ncurses"]
 requires-python = ">=3.10"
 
 [project.license]
```

