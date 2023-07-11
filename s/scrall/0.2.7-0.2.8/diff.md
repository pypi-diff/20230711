# Comparing `tmp/scrall-0.2.7.tar.gz` & `tmp/scrall-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrall-0.2.7.tar", last modified: Tue Jul 11 00:03:17 2023, max compression
+gzip compressed data, was "scrall-0.2.8.tar", last modified: Tue Jul 11 16:35:59 2023, max compression
```

## Comparing `scrall-0.2.7.tar` & `scrall-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 00:03:17.873925 scrall-0.2.7/
--rw-r--r--   0 starr      (501) staff       (20)     1072 2023-07-04 22:05:28.000000 scrall-0.2.7/LICENSE
--rw-r--r--   0 starr      (501) staff       (20)       58 2023-07-11 00:01:55.000000 scrall-0.2.7/MANIFEST.in
--rw-r--r--   0 starr      (501) staff       (20)     4431 2023-07-11 00:03:17.873838 scrall-0.2.7/PKG-INFO
--rw-r--r--   0 starr      (501) staff       (20)     2509 2023-07-04 22:05:28.000000 scrall-0.2.7/README.md
--rw-r--r--   0 starr      (501) staff       (20)      977 2023-07-11 00:02:50.000000 scrall-0.2.7/pyproject.toml
--rw-r--r--   0 starr      (501) staff       (20)       38 2023-07-11 00:03:17.873956 scrall-0.2.7/setup.cfg
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 00:03:17.871780 scrall-0.2.7/src/
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 00:03:17.872735 scrall-0.2.7/src/scrall/
--rw-r--r--   0 starr      (501) staff       (20)       17 2023-07-11 00:02:50.000000 scrall-0.2.7/src/scrall/__init__.py
--rw-r--r--   0 starr      (501) staff       (20)     1779 2023-07-10 15:11:24.000000 scrall-0.2.7/src/scrall/__main__.py
--rw-r--r--   0 starr      (501) staff       (20)     1764 2023-07-09 14:59:46.000000 scrall-0.2.7/src/scrall/exceptions.py
--rw-r--r--   0 starr      (501) staff       (20)      827 2023-07-09 14:59:46.000000 scrall-0.2.7/src/scrall/log.conf
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 00:03:17.873665 scrall-0.2.7/src/scrall/parse/
--rw-r--r--   0 starr      (501) staff       (20)        0 2023-07-09 14:59:46.000000 scrall-0.2.7/src/scrall/parse/__init__.py
--rw-r--r--   0 starr      (501) staff       (20)     4984 2023-07-11 00:01:55.000000 scrall-0.2.7/src/scrall/parse/parser.py
--rw-r--r--   0 starr      (501) staff       (20)    34598 2023-07-11 00:01:55.000000 scrall-0.2.7/src/scrall/parse/visitor.py
--rw-r--r--   0 starr      (501) staff       (20)     7533 2023-07-11 00:01:55.000000 scrall-0.2.7/src/scrall/scrall.peg
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 00:03:17.873383 scrall-0.2.7/src/scrall.egg-info/
--rw-r--r--   0 starr      (501) staff       (20)     4431 2023-07-11 00:03:17.000000 scrall-0.2.7/src/scrall.egg-info/PKG-INFO
--rw-r--r--   0 starr      (501) staff       (20)      447 2023-07-11 00:03:17.000000 scrall-0.2.7/src/scrall.egg-info/SOURCES.txt
--rw-r--r--   0 starr      (501) staff       (20)        1 2023-07-11 00:03:17.000000 scrall-0.2.7/src/scrall.egg-info/dependency_links.txt
--rw-r--r--   0 starr      (501) staff       (20)       48 2023-07-11 00:03:17.000000 scrall-0.2.7/src/scrall.egg-info/entry_points.txt
--rw-r--r--   0 starr      (501) staff       (20)       91 2023-07-11 00:03:17.000000 scrall-0.2.7/src/scrall.egg-info/requires.txt
--rw-r--r--   0 starr      (501) staff       (20)        7 2023-07-11 00:03:17.000000 scrall-0.2.7/src/scrall.egg-info/top_level.txt
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 16:35:59.141660 scrall-0.2.8/
+-rw-r--r--   0 starr      (501) staff       (20)     1072 2023-07-04 22:05:28.000000 scrall-0.2.8/LICENSE
+-rw-r--r--   0 starr      (501) staff       (20)       58 2023-07-11 00:01:55.000000 scrall-0.2.8/MANIFEST.in
+-rw-r--r--   0 starr      (501) staff       (20)     4431 2023-07-11 16:35:59.141568 scrall-0.2.8/PKG-INFO
+-rw-r--r--   0 starr      (501) staff       (20)     2509 2023-07-04 22:05:28.000000 scrall-0.2.8/README.md
+-rw-r--r--   0 starr      (501) staff       (20)      977 2023-07-11 16:35:29.000000 scrall-0.2.8/pyproject.toml
+-rw-r--r--   0 starr      (501) staff       (20)       38 2023-07-11 16:35:59.141691 scrall-0.2.8/setup.cfg
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 16:35:59.138965 scrall-0.2.8/src/
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 16:35:59.140123 scrall-0.2.8/src/scrall/
+-rw-r--r--   0 starr      (501) staff       (20)       17 2023-07-11 16:35:29.000000 scrall-0.2.8/src/scrall/__init__.py
+-rw-r--r--   0 starr      (501) staff       (20)     1779 2023-07-10 15:11:24.000000 scrall-0.2.8/src/scrall/__main__.py
+-rw-r--r--   0 starr      (501) staff       (20)     1764 2023-07-09 14:59:46.000000 scrall-0.2.8/src/scrall/exceptions.py
+-rw-r--r--   0 starr      (501) staff       (20)      827 2023-07-09 14:59:46.000000 scrall-0.2.8/src/scrall/log.conf
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 16:35:59.141211 scrall-0.2.8/src/scrall/parse/
+-rw-r--r--   0 starr      (501) staff       (20)        0 2023-07-09 14:59:46.000000 scrall-0.2.8/src/scrall/parse/__init__.py
+-rw-r--r--   0 starr      (501) staff       (20)     5014 2023-07-11 16:35:14.000000 scrall-0.2.8/src/scrall/parse/parser.py
+-rw-r--r--   0 starr      (501) staff       (20)    34598 2023-07-11 00:01:55.000000 scrall-0.2.8/src/scrall/parse/visitor.py
+-rw-r--r--   0 starr      (501) staff       (20)     7533 2023-07-11 00:01:55.000000 scrall-0.2.8/src/scrall/scrall.peg
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 16:35:59.140923 scrall-0.2.8/src/scrall.egg-info/
+-rw-r--r--   0 starr      (501) staff       (20)     4431 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/PKG-INFO
+-rw-r--r--   0 starr      (501) staff       (20)      447 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/SOURCES.txt
+-rw-r--r--   0 starr      (501) staff       (20)        1 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/dependency_links.txt
+-rw-r--r--   0 starr      (501) staff       (20)       48 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/entry_points.txt
+-rw-r--r--   0 starr      (501) staff       (20)       91 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/requires.txt
+-rw-r--r--   0 starr      (501) staff       (20)        7 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/top_level.txt
```

### Comparing `scrall-0.2.7/LICENSE` & `scrall-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scrall-0.2.7/PKG-INFO` & `scrall-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrall
-Version: 0.2.7
+Version: 0.2.8
 Summary: Starr's Concise Relational Action Language - For Shlaer-Mellor Executable UML
 Author-email: Leon Starr <leon_starr@modelint.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Leon Starr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `scrall-0.2.7/README.md` & `scrall-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `scrall-0.2.7/pyproject.toml` & `scrall-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scrall"
-version = "0.2.7"
+version = "0.2.8"
 description = "Starr's Concise Relational Action Language - For Shlaer-Mellor Executable UML"
 readme = "README.md"
 authors = [{ name = "Leon Starr", email = "leon_starr@modelint.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `scrall-0.2.7/src/scrall/__main__.py` & `scrall-0.2.8/src/scrall/__main__.py`

 * *Files identical despite different names*

### Comparing `scrall-0.2.7/src/scrall/exceptions.py` & `scrall-0.2.8/src/scrall/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrall-0.2.7/src/scrall/log.conf` & `scrall-0.2.8/src/scrall/log.conf`

 * *Files identical despite different names*

### Comparing `scrall-0.2.7/src/scrall/parse/parser.py` & `scrall-0.2.8/src/scrall/parse/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     pg_tree_dot = cwd / "peggrammar_parse_tree.dot"
     pg_model_dot = cwd / "peggrammar_parser_model.dot"
     pg_tree_pdf = diagnostics_path / "peggrammar_parse_tree.pdf"
     pg_model_pdf = diagnostics_path / "peggrammar_parser_model.pdf"
 
     @classmethod
-    def parse_file(cls, file_input: Path, debug=False):
+    def parse_file(cls, file_input: Path, debug=False) -> List:
         """
         Read and save the file contents and options and then call the parser
 
         :param file_input:  Scrall file to read
         :param debug: Run parser in debug mode
         :return:
         """
@@ -67,31 +67,31 @@
 
         if not cls.scrall_text:
             raise ScrallInputFileEmpty(file_input)
 
         if not cls.scrall_text.endswith('\n'):
             cls.scrall_text += '\n'
 
-        cls.parse()
+        return cls.parse()
 
     @classmethod
-    def parse_text(cls, scrall_text: str, debug=False):
+    def parse_text(cls, scrall_text: str, debug=False) -> List:
         """
         Save options and call the parser
 
         :param scrall_text: One or more lines of scrall_text
         :param debug: Run parser in debug mode
         :return:
         """
         cls.debug = debug
         cls.scrall_text = scrall_text
         if not cls.scrall_text.endswith('\n'):
             cls.scrall_text += '\n'
 
-        cls.parse()
+        return cls.parse()
 
     @classmethod
     def parse(cls) -> List:
         """
         Parse a Scrall activity
 
         :return: A list of parsed Scrall statements
```

### Comparing `scrall-0.2.7/src/scrall/parse/visitor.py` & `scrall-0.2.8/src/scrall/parse/visitor.py`

 * *Files identical despite different names*

### Comparing `scrall-0.2.7/src/scrall/scrall.peg` & `scrall-0.2.8/src/scrall/scrall.peg`

 * *Files identical despite different names*

### Comparing `scrall-0.2.7/src/scrall.egg-info/PKG-INFO` & `scrall-0.2.8/src/scrall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrall
-Version: 0.2.7
+Version: 0.2.8
 Summary: Starr's Concise Relational Action Language - For Shlaer-Mellor Executable UML
 Author-email: Leon Starr <leon_starr@modelint.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Leon Starr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

