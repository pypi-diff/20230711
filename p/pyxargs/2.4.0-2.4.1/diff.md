# Comparing `tmp/pyxargs-2.4.0.tar.gz` & `tmp/pyxargs-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxargs-2.4.0.tar", last modified: Tue Jul 11 17:48:11 2023, max compression
+gzip compressed data, was "pyxargs-2.4.1.tar", last modified: Tue Jul 11 18:35:50 2023, max compression
```

## Comparing `pyxargs-2.4.0.tar` & `pyxargs-2.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:48:11.277439 pyxargs-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 17:47:58.000000 pyxargs-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-11 17:48:11.277439 pyxargs-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-11 17:47:58.000000 pyxargs-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:48:11.277439 pyxargs-2.4.0/pyxargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-11 17:48:11.000000 pyxargs-2.4.0/pyxargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 17:48:11.000000 pyxargs-2.4.0/pyxargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:48:11.000000 pyxargs-2.4.0/pyxargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 17:48:11.000000 pyxargs-2.4.0/pyxargs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:48:11.000000 pyxargs-2.4.0/pyxargs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23504 2023-07-11 17:47:58.000000 pyxargs-2.4.0/pyxargs.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:48:11.277439 pyxargs-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-11 17:47:58.000000 pyxargs-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:35:50.156964 pyxargs-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 18:35:39.000000 pyxargs-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-11 18:35:50.156964 pyxargs-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-11 18:35:39.000000 pyxargs-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:35:50.156964 pyxargs-2.4.1/pyxargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-11 18:35:50.000000 pyxargs-2.4.1/pyxargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 18:35:50.000000 pyxargs-2.4.1/pyxargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:35:50.000000 pyxargs-2.4.1/pyxargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 18:35:50.000000 pyxargs-2.4.1/pyxargs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 18:35:50.000000 pyxargs-2.4.1/pyxargs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23563 2023-07-11 18:35:39.000000 pyxargs-2.4.1/pyxargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:35:50.156964 pyxargs-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-11 18:35:39.000000 pyxargs-2.4.1/setup.py
```

### Comparing `pyxargs-2.4.0/LICENSE` & `pyxargs-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxargs-2.4.0/PKG-INFO` & `pyxargs-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxargs
-Version: 2.4.0
+Version: 2.4.1
 Summary: A partial and opinionated implementation of xargs in python with some added features
 Home-page: https://github.com/elesiuta/pyxargs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Shells
```

### Comparing `pyxargs-2.4.0/README.md` & `pyxargs-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyxargs-2.4.0/pyxargs.egg-info/PKG-INFO` & `pyxargs-2.4.1/pyxargs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxargs
-Version: 2.4.0
+Version: 2.4.1
 Summary: A partial and opinionated implementation of xargs in python with some added features
 Home-page: https://github.com/elesiuta/pyxargs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Shells
```

### Comparing `pyxargs-2.4.0/pyxargs.py` & `pyxargs-2.4.1/pyxargs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import sys
 import tempfile
 import textwrap
 import time
 import typing
 
 
-__version__: typing.Final[str] = "2.4.0"
+__version__: typing.Final[str] = "2.4.1"
 
 
 def replace_surrogates(string: str) -> str:
     return string.encode('utf16', 'surrogatepass').decode('utf16', 'replace')
 
 
 def colour_print(string: str, colour: str) -> None:
@@ -373,16 +373,16 @@
         if not sys.stdin.isatty():
             stdin = sys.stdin.read()
             args.input_mode = "stdin"
         else:
             args.input_mode = "file"
     elif args.input_mode == "stdin":
         stdin = sys.stdin.read()
-    # need to open new tty for interactive mode if input was read from stdin
-    if args.interactive and stdin and args.arg_file is None:
+    # need to open new tty for interactive mode if input was piped to stdin (handled later if using mux)
+    if args.interactive and not sys.stdin.isatty() and args.procs is None:
         sys.stdin = open("/dev/tty")
     # set delimiter
     if args.null:
         args.delim = "\0"
     # enable format string mode
     if args.re_split is not None:
         args.format_str = True
@@ -425,15 +425,15 @@
             pickle.dump(command_dicts, command_pickle.file)
             command_pickle.file.flush()
             pyxargs_command = [sys.executable, os.path.abspath(__file__), "--chunk", "0", "--_command_pickle", args.input_mode, command_pickle.name] + sys.argv[1:]
             subprocess.run([multiplexer, "new-session", "-d", "-s", session, shlex.join(pyxargs_command)])
             for i in range(1, args.procs):
                 pyxargs_command[3] = str(i)
                 subprocess.run([multiplexer, "new-window", "-t", f"{session}:{i}", shlex.join(pyxargs_command)])
-            if stdin:
+            if not sys.stdin.isatty():
                 sys.stdin = sys.__stdin__ = open("/dev/tty")
                 os.dup2(sys.stdin.fileno(), 0)
                 pty.spawn([multiplexer, "attach-session", "-t", session])
             else:
                 subprocess.run([multiplexer, "attach-session", "-t", session])
             return 0
         # execute commands (in chunks if requested)
```

### Comparing `pyxargs-2.4.0/setup.py` & `pyxargs-2.4.1/setup.py`

 * *Files identical despite different names*

