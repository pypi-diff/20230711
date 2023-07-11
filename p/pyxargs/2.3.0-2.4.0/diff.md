# Comparing `tmp/pyxargs-2.3.0.tar.gz` & `tmp/pyxargs-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxargs-2.3.0.tar", last modified: Mon Jul 10 06:50:21 2023, max compression
+gzip compressed data, was "pyxargs-2.4.0.tar", last modified: Tue Jul 11 17:48:11 2023, max compression
```

## Comparing `pyxargs-2.3.0.tar` & `pyxargs-2.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:50:21.660227 pyxargs-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 06:50:09.000000 pyxargs-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-10 06:50:21.660227 pyxargs-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-10 06:50:09.000000 pyxargs-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:50:21.660227 pyxargs-2.3.0/pyxargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-10 06:50:21.000000 pyxargs-2.3.0/pyxargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-10 06:50:21.000000 pyxargs-2.3.0/pyxargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:50:21.000000 pyxargs-2.3.0/pyxargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 06:50:21.000000 pyxargs-2.3.0/pyxargs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 06:50:21.000000 pyxargs-2.3.0/pyxargs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20756 2023-07-10 06:50:09.000000 pyxargs-2.3.0/pyxargs.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 06:50:21.660227 pyxargs-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-10 06:50:09.000000 pyxargs-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:48:11.277439 pyxargs-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 17:47:58.000000 pyxargs-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-11 17:48:11.277439 pyxargs-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-11 17:47:58.000000 pyxargs-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:48:11.277439 pyxargs-2.4.0/pyxargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-11 17:48:11.000000 pyxargs-2.4.0/pyxargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 17:48:11.000000 pyxargs-2.4.0/pyxargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:48:11.000000 pyxargs-2.4.0/pyxargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 17:48:11.000000 pyxargs-2.4.0/pyxargs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:48:11.000000 pyxargs-2.4.0/pyxargs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23504 2023-07-11 17:47:58.000000 pyxargs-2.4.0/pyxargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:48:11.277439 pyxargs-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-11 17:47:58.000000 pyxargs-2.4.0/setup.py
```

### Comparing `pyxargs-2.3.0/LICENSE` & `pyxargs-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxargs-2.3.0/PKG-INFO` & `pyxargs-2.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: pyxargs
-Version: 2.3.0
-Summary: A partial and opinionated implementation of xargs in python with some added features
-Home-page: https://github.com/elesiuta/pyxargs
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Utilities
-Classifier: Topic :: System :: Shells
-Classifier: Topic :: System :: System Shells
-Classifier: Topic :: Terminals
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: Environment :: Console
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyxargs
 
 This started as a simple solution to the [encoding problem with xargs](https://en.wikipedia.org/wiki/Xargs#Encoding_problem). It is a partial and opinionated implementation of xargs with the goal of being easier to use for most use cases.  
 
 It also contains some additional features which may or may not be useful, such as taking python code as arguments to be executed, or filtering input with regular expressions. No new features are planned.  
 
 You can install [pyxargs](https://github.com/elesiuta/pyxargs/) from [PyPI](https://pypi.org/project/pyxargs/).  
@@ -56,44 +34,55 @@
                         default: stdin if connected, otherwise file
   --folders             use folders instead files (for input modes: file,
                         path, abspath)
   -t, --top             do not recurse into subdirectories (for input modes:
                         file, path, abspath)
   --sym, --symlinks     follow symlinks when scanning directories (for input
                         modes: file, path, abspath)
+  -a file, --arg-file file
+                        read input items from file instead of standard input
+                        (for input mode: stdin)
   -0, --null            input items are separated by a null character instead
                         of whitespace (for input mode: stdin)
   -d delim, --delimiter delim
                         input items are separated by the specified delimiter
                         instead of whitespace (for input mode: stdin)
-  --max-chars n         omits any command line exceeding n characters, no
-                        limit by default
+  -s regex, --split regex
+                        split each input item with re.split(regex, input)
+                        before building command (after separating by
+                        delimiter), use {0}, {1}, ... to specify placement
+                        (implies --format)
+  -f, --format          format command with input using str.format() instead
+                        of appending or replacing via -I replace-str
   -I replace-str        replace occurrences of replace-str in command with
                         input, default: {}
   --resub pattern substitution replace-str
                         replace occurrences of replace-str in command with
                         re.sub(patten, substitution, input)
   -r regex              only build commands from inputs matching regex for
                         input mode stdin, and matching relative paths for all
                         other input modes, uses re.search
   -o                    omit inputs matching regex instead
   -b                    only match regex against basename of input (for input
                         modes: file, path, abspath)
-  -s, --shell           executes commands through the shell (subprocess
+  --max-chars n         omits any command line exceeding n characters, no
+                        limit by default
+  --sh, --shell         executes commands through the shell (subprocess
                         shell=True) (no effect on Windows)
   --py, --pyex          executes commands as python code using exec()
   --pyev                evaluates commands as python expressions using eval()
   --import library      executes 'import <library>' for each library
   --im library, --importstar library
                         executes 'from <library> import *' for each library
   --pre "code"          runs exec(code) before execution
   --post "code"         runs exec(code) after execution
   -P P, --procs P       split into P chunks and execute each chunk in parallel
                         as a separate process and window with byobu or tmux
   -c c, --chunk c       runs chunk c of P (0 <= c < P) (without multiplexer)
+  --no-mux              do not use a multiplexer for multiple processes
   -i, --interactive     prompt the user before executing each command, only
                         proceeds if response starts with 'y' or 'Y'
   -n, --dry-run         prints commands without executing them
   -v, --verbose         prints commands before executing them
 ```
 ## Examples
 ```bash
@@ -106,24 +95,35 @@
 # and like xargs, you can also specify the replace-str with -I
   > pyxargs -I eggs echo spam eggs spam literal {}
 
 # if stdin is connected, it will be used instead of filenames by default
   > echo bacon eggs | pyxargs echo spam
 
 # python code can be used in place of a command
-  > pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
+  > pyxargs --py "print(f'input file: {} executed in: {os.getcwd()}')"
 
 # python code can also run before or after all the commands
   > pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
 
 # regular expressions can be used to filter and modify inputs
-  > pyxargs -r \.py --resub \.py .txt {} echo {}
+  > pyxargs -r \.py --resub \.py .txt {new} echo {} -\> {new}
+
+# you can test your command first with --dry-run (-n) or --interactive (-i)
+  > pyxargs -i echo filename: {}
+
+# pyxargs can also run interactively in parallel by using byobu or tmux
+  > pyxargs -P 4 -i echo filename: {}
+
+# you can use pyxargs to create a JSON mapping of /etc/hosts
+  > cat /etc/hosts | pyxargs -d \n --im json --pre "d={}" \
+    --post "print(dumps(d))" --py "d['{}'.split()[0]] = '{}'.split()[1]"
 
-# the original inputs can easily be used with the substituted versions
-  > pyxargs -r \.py --resub \.py .txt new echo {} new
+# you can also do this with format strings and --split (-s) (uses regex)
+  > cat /etc/hosts | pyxargs -d \n -s "\s+" --im json --pre "d={}" \
+    --post "print(dumps(d))" --py "d['{0}'] = '{1}'"
 
 # this and the following examples will compare usage with find & xargs
   > find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
   > find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
 
 # pyxargs does not require '-I' to specify a replace-str (default: {})
   > find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
```

### Comparing `pyxargs-2.3.0/README.md` & `pyxargs-2.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: pyxargs
+Version: 2.4.0
+Summary: A partial and opinionated implementation of xargs in python with some added features
+Home-page: https://github.com/elesiuta/pyxargs
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Utilities
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: System :: System Shells
+Classifier: Topic :: Terminals
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Environment :: Console
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyxargs
 
 This started as a simple solution to the [encoding problem with xargs](https://en.wikipedia.org/wiki/Xargs#Encoding_problem). It is a partial and opinionated implementation of xargs with the goal of being easier to use for most use cases.  
 
 It also contains some additional features which may or may not be useful, such as taking python code as arguments to be executed, or filtering input with regular expressions. No new features are planned.  
 
 You can install [pyxargs](https://github.com/elesiuta/pyxargs/) from [PyPI](https://pypi.org/project/pyxargs/).  
@@ -34,44 +56,55 @@
                         default: stdin if connected, otherwise file
   --folders             use folders instead files (for input modes: file,
                         path, abspath)
   -t, --top             do not recurse into subdirectories (for input modes:
                         file, path, abspath)
   --sym, --symlinks     follow symlinks when scanning directories (for input
                         modes: file, path, abspath)
+  -a file, --arg-file file
+                        read input items from file instead of standard input
+                        (for input mode: stdin)
   -0, --null            input items are separated by a null character instead
                         of whitespace (for input mode: stdin)
   -d delim, --delimiter delim
                         input items are separated by the specified delimiter
                         instead of whitespace (for input mode: stdin)
-  --max-chars n         omits any command line exceeding n characters, no
-                        limit by default
+  -s regex, --split regex
+                        split each input item with re.split(regex, input)
+                        before building command (after separating by
+                        delimiter), use {0}, {1}, ... to specify placement
+                        (implies --format)
+  -f, --format          format command with input using str.format() instead
+                        of appending or replacing via -I replace-str
   -I replace-str        replace occurrences of replace-str in command with
                         input, default: {}
   --resub pattern substitution replace-str
                         replace occurrences of replace-str in command with
                         re.sub(patten, substitution, input)
   -r regex              only build commands from inputs matching regex for
                         input mode stdin, and matching relative paths for all
                         other input modes, uses re.search
   -o                    omit inputs matching regex instead
   -b                    only match regex against basename of input (for input
                         modes: file, path, abspath)
-  -s, --shell           executes commands through the shell (subprocess
+  --max-chars n         omits any command line exceeding n characters, no
+                        limit by default
+  --sh, --shell         executes commands through the shell (subprocess
                         shell=True) (no effect on Windows)
   --py, --pyex          executes commands as python code using exec()
   --pyev                evaluates commands as python expressions using eval()
   --import library      executes 'import <library>' for each library
   --im library, --importstar library
                         executes 'from <library> import *' for each library
   --pre "code"          runs exec(code) before execution
   --post "code"         runs exec(code) after execution
   -P P, --procs P       split into P chunks and execute each chunk in parallel
                         as a separate process and window with byobu or tmux
   -c c, --chunk c       runs chunk c of P (0 <= c < P) (without multiplexer)
+  --no-mux              do not use a multiplexer for multiple processes
   -i, --interactive     prompt the user before executing each command, only
                         proceeds if response starts with 'y' or 'Y'
   -n, --dry-run         prints commands without executing them
   -v, --verbose         prints commands before executing them
 ```
 ## Examples
 ```bash
@@ -84,24 +117,35 @@
 # and like xargs, you can also specify the replace-str with -I
   > pyxargs -I eggs echo spam eggs spam literal {}
 
 # if stdin is connected, it will be used instead of filenames by default
   > echo bacon eggs | pyxargs echo spam
 
 # python code can be used in place of a command
-  > pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
+  > pyxargs --py "print(f'input file: {} executed in: {os.getcwd()}')"
 
 # python code can also run before or after all the commands
   > pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
 
 # regular expressions can be used to filter and modify inputs
-  > pyxargs -r \.py --resub \.py .txt {} echo {}
+  > pyxargs -r \.py --resub \.py .txt {new} echo {} -\> {new}
+
+# you can test your command first with --dry-run (-n) or --interactive (-i)
+  > pyxargs -i echo filename: {}
+
+# pyxargs can also run interactively in parallel by using byobu or tmux
+  > pyxargs -P 4 -i echo filename: {}
+
+# you can use pyxargs to create a JSON mapping of /etc/hosts
+  > cat /etc/hosts | pyxargs -d \n --im json --pre "d={}" \
+    --post "print(dumps(d))" --py "d['{}'.split()[0]] = '{}'.split()[1]"
 
-# the original inputs can easily be used with the substituted versions
-  > pyxargs -r \.py --resub \.py .txt new echo {} new
+# you can also do this with format strings and --split (-s) (uses regex)
+  > cat /etc/hosts | pyxargs -d \n -s "\s+" --im json --pre "d={}" \
+    --post "print(dumps(d))" --py "d['{0}'] = '{1}'"
 
 # this and the following examples will compare usage with find & xargs
   > find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
   > find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
 
 # pyxargs does not require '-I' to specify a replace-str (default: {})
   > find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
```

### Comparing `pyxargs-2.3.0/pyxargs.egg-info/PKG-INFO` & `pyxargs-2.4.0/pyxargs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxargs
-Version: 2.3.0
+Version: 2.4.0
 Summary: A partial and opinionated implementation of xargs in python with some added features
 Home-page: https://github.com/elesiuta/pyxargs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Shells
@@ -56,44 +56,55 @@
                         default: stdin if connected, otherwise file
   --folders             use folders instead files (for input modes: file,
                         path, abspath)
   -t, --top             do not recurse into subdirectories (for input modes:
                         file, path, abspath)
   --sym, --symlinks     follow symlinks when scanning directories (for input
                         modes: file, path, abspath)
+  -a file, --arg-file file
+                        read input items from file instead of standard input
+                        (for input mode: stdin)
   -0, --null            input items are separated by a null character instead
                         of whitespace (for input mode: stdin)
   -d delim, --delimiter delim
                         input items are separated by the specified delimiter
                         instead of whitespace (for input mode: stdin)
-  --max-chars n         omits any command line exceeding n characters, no
-                        limit by default
+  -s regex, --split regex
+                        split each input item with re.split(regex, input)
+                        before building command (after separating by
+                        delimiter), use {0}, {1}, ... to specify placement
+                        (implies --format)
+  -f, --format          format command with input using str.format() instead
+                        of appending or replacing via -I replace-str
   -I replace-str        replace occurrences of replace-str in command with
                         input, default: {}
   --resub pattern substitution replace-str
                         replace occurrences of replace-str in command with
                         re.sub(patten, substitution, input)
   -r regex              only build commands from inputs matching regex for
                         input mode stdin, and matching relative paths for all
                         other input modes, uses re.search
   -o                    omit inputs matching regex instead
   -b                    only match regex against basename of input (for input
                         modes: file, path, abspath)
-  -s, --shell           executes commands through the shell (subprocess
+  --max-chars n         omits any command line exceeding n characters, no
+                        limit by default
+  --sh, --shell         executes commands through the shell (subprocess
                         shell=True) (no effect on Windows)
   --py, --pyex          executes commands as python code using exec()
   --pyev                evaluates commands as python expressions using eval()
   --import library      executes 'import <library>' for each library
   --im library, --importstar library
                         executes 'from <library> import *' for each library
   --pre "code"          runs exec(code) before execution
   --post "code"         runs exec(code) after execution
   -P P, --procs P       split into P chunks and execute each chunk in parallel
                         as a separate process and window with byobu or tmux
   -c c, --chunk c       runs chunk c of P (0 <= c < P) (without multiplexer)
+  --no-mux              do not use a multiplexer for multiple processes
   -i, --interactive     prompt the user before executing each command, only
                         proceeds if response starts with 'y' or 'Y'
   -n, --dry-run         prints commands without executing them
   -v, --verbose         prints commands before executing them
 ```
 ## Examples
 ```bash
@@ -106,24 +117,35 @@
 # and like xargs, you can also specify the replace-str with -I
   > pyxargs -I eggs echo spam eggs spam literal {}
 
 # if stdin is connected, it will be used instead of filenames by default
   > echo bacon eggs | pyxargs echo spam
 
 # python code can be used in place of a command
-  > pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
+  > pyxargs --py "print(f'input file: {} executed in: {os.getcwd()}')"
 
 # python code can also run before or after all the commands
   > pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
 
 # regular expressions can be used to filter and modify inputs
-  > pyxargs -r \.py --resub \.py .txt {} echo {}
+  > pyxargs -r \.py --resub \.py .txt {new} echo {} -\> {new}
+
+# you can test your command first with --dry-run (-n) or --interactive (-i)
+  > pyxargs -i echo filename: {}
+
+# pyxargs can also run interactively in parallel by using byobu or tmux
+  > pyxargs -P 4 -i echo filename: {}
+
+# you can use pyxargs to create a JSON mapping of /etc/hosts
+  > cat /etc/hosts | pyxargs -d \n --im json --pre "d={}" \
+    --post "print(dumps(d))" --py "d['{}'.split()[0]] = '{}'.split()[1]"
 
-# the original inputs can easily be used with the substituted versions
-  > pyxargs -r \.py --resub \.py .txt new echo {} new
+# you can also do this with format strings and --split (-s) (uses regex)
+  > cat /etc/hosts | pyxargs -d \n -s "\s+" --im json --pre "d={}" \
+    --post "print(dumps(d))" --py "d['{0}'] = '{1}'"
 
 # this and the following examples will compare usage with find & xargs
   > find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
   > find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
 
 # pyxargs does not require '-I' to specify a replace-str (default: {})
   > find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
```

### Comparing `pyxargs-2.3.0/pyxargs.py` & `pyxargs-2.4.0/pyxargs.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # https://github.com/elesiuta/pyxargs
 
 import argparse
+import multiprocessing
 import os
 import pickle
 import pty
 import re
 import shlex
 import shutil
 import signal
@@ -27,15 +28,15 @@
 import sys
 import tempfile
 import textwrap
 import time
 import typing
 
 
-__version__: typing.Final[str] = "2.3.0"
+__version__: typing.Final[str] = "2.4.0"
 
 
 def replace_surrogates(string: str) -> str:
     return string.encode('utf16', 'surrogatepass').decode('utf16', 'replace')
 
 
 def colour_print(string: str, colour: str) -> None:
@@ -51,15 +52,15 @@
 
 def safe_print(string: str) -> None:
     print(replace_surrogates(string))
 
 
 def build_commands(args: argparse.Namespace, stdin: str) -> list:
     command_dicts = []
-    append_input = not (args.pyex or args.pyev or args.resub) and args.replace_str is None and all("{}" not in arg for arg in args.command)
+    append_input = not (args.pyex or args.pyev or args.resub or args.format_str) and args.replace_str is None and all("{}" not in arg for arg in args.command)
     args.replace_str = "{}" if args.replace_str is None else args.replace_str
     # build commands using standard input mode or by walking the directory tree
     if args.input_mode == "stdin":
         # remove trailing whitespace and split stdin
         stdin = stdin.rstrip()
         arg_input_list = stdin.split(args.delim)
         # build commands from stdin
@@ -107,14 +108,17 @@
             run = input("> ")
             if run.lower().startswith("y"):
                 execute_command(args, command_dict, user_namespace)
             elif run.lower().startswith("n"):
                 pass
             else:
                 return 4
+    elif args.no_mux:
+        with multiprocessing.Pool(args.procs) as pool:
+            pool.starmap(execute_command, [(args, command_dict, user_namespace) for command_dict in command_dicts])
     else:
         for command_dict in command_dicts:
             execute_command(args, command_dict, user_namespace)
     # post execution tasks
     if args.post:
         exec(args.post, globals(), user_namespace)
     return 0
@@ -137,37 +141,39 @@
         if (re.search(args.regex, basename) is not None) == args.regex_omit:
             return []
     else:
         relpath = os.path.join(dir_path, basename)
         relpath = os.path.relpath(relpath, args.base_dir)
         if (re.search(args.regex, relpath) is not None) == args.regex_omit:
             return []
-    # copy command
-    command = [cmd for cmd in args.command]
+    # copy command first since some options mutate it
+    command = args.command.copy()
     # re.sub input into command
     if args.resub is not None:
-        for i in range(len(command)):
-            command[i] = command[i].replace(args.resub[2], re.sub(args.resub[0], args.resub[1], arg_input))
-    # sub input into command or append
-    if append_input:
+        command = [cmd.replace(args.resub[2], re.sub(args.resub[0], args.resub[1], arg_input)) for cmd in command]
+    # build command with input via format, append, or replace-str
+    if args.format_str:
+        arg_input_list = [arg_input]
+        if args.re_split is not None:
+            arg_input_list = re.split(args.re_split, arg_input)
+        command = [cmd.format(*arg_input_list) for cmd in command]
+    elif append_input:
         command.append(arg_input)
     else:
-        for i in range(len(command)):
-            command[i] = command[i].replace(args.replace_str, arg_input)
+        command = [cmd.replace(args.replace_str, arg_input) for cmd in command]
     # check length of command
     if args.max_chars is not None:
         if len(shlex.join(command)) > args.max_chars:
             if args.verbose:
                 colour_print(f"Command too long for: {arg_input}", "Y")
             return []
-    # join command
+    # join command if required
     if args.pyex or args.pyev or args.subprocess_shell:
         if len(command) > 1:
             command = [shlex.join(command)]
-    # and finally
     return command
 
 
 def execute_command(args: argparse.Namespace, command_dict: dict, user_namespace: dict) -> None:
     dir_path = command_dict["dir"]
     cmd = command_dict["cmd"]
     if args.input_mode == "file":
@@ -222,24 +228,35 @@
     # and like xargs, you can also specify the replace-str with -I
       > pyxargs -I eggs echo spam eggs spam literal {}
 
     # if stdin is connected, it will be used instead of filenames by default
       > echo bacon eggs | pyxargs echo spam
 
     # python code can be used in place of a command
-      > pyxargs --py "print(f'input file: {{}} executed in: {os.getcwd()}')"
+      > pyxargs --py "print(f'input file: {} executed in: {os.getcwd()}')"
 
     # python code can also run before or after all the commands
       > pyxargs --pre "n=0" --post "print(n,'files')" --py "n+=1"
 
     # regular expressions can be used to filter and modify inputs
-      > pyxargs -r \.py --resub \.py .txt {} echo {}
+      > pyxargs -r \.py --resub \.py .txt {new} echo {} -\> {new}
 
-    # the original inputs can easily be used with the substituted versions
-      > pyxargs -r \.py --resub \.py .txt new echo {} new
+    # you can test your command first with --dry-run (-n) or --interactive (-i)
+      > pyxargs -i echo filename: {}
+
+    # pyxargs can also run interactively in parallel by using byobu or tmux
+      > pyxargs -P 4 -i echo filename: {}
+
+    # you can use pyxargs to create a JSON mapping of /etc/hosts
+      > cat /etc/hosts | pyxargs -d \n --im json --pre "d={}" \
+        --post "print(dumps(d))" --py "d['{}'.split()[0]] = '{}'.split()[1]"
+
+    # you can also do this with format strings and --split (-s) (uses regex)
+      > cat /etc/hosts | pyxargs -d \n -s "\s+" --im json --pre "d={}" \
+        --post "print(dumps(d))" --py "d['{0}'] = '{1}'"
 
     # this and the following examples will compare usage with find & xargs
       > find ./ -name "*" -type f -print0 | xargs -0 -I {} echo {}
       > find ./ -name "*" -type f -print0 | pyxargs -0 -I {} echo {}
 
     # pyxargs does not require '-I' to specify a replace-str (default: {})
       > find ./ -name "*" -type f -print0 | pyxargs -0 echo {}
@@ -283,31 +300,37 @@
                              "default: stdin if connected, otherwise file")
     parser.add_argument("--folders", action="store_true", dest="folders",
                         help="use folders instead files (for input modes: file, path, abspath)")
     parser.add_argument("-t", "--top", action="store_true", dest="top_level",
                         help="do not recurse into subdirectories (for input modes: file, path, abspath)")
     parser.add_argument("--sym", "--symlinks", action="store_true", dest="symlinks",
                         help="follow symlinks when scanning directories (for input modes: file, path, abspath)")
+    parser.add_argument("-a", "--arg-file", type=str, default=None, metavar="file", dest="arg_file",
+                        help="read input items from file instead of standard input (for input mode: stdin)")
     group0.add_argument("-0", "--null", action="store_true", dest="null",
                         help="input items are separated by a null character instead of whitespace (for input mode: stdin)")
     group0.add_argument("-d", "--delimiter", type=str, default=None, metavar="delim", dest="delim",
                         help="input items are separated by the specified delimiter instead of whitespace (for input mode: stdin)")
-    parser.add_argument("--max-chars", type=int, metavar="n", dest="max_chars",
-                        help="omits any command line exceeding n characters, no limit by default")
+    parser.add_argument("-s", "--split", type=str, default=None, metavar="regex", dest="re_split",
+                        help="split each input item with re.split(regex, input) before building command (after separating by delimiter), use {0}, {1}, ... to specify placement (implies --format)")
+    parser.add_argument("-f", "--format", action="store_true", dest="format_str",
+                        help="format command with input using str.format() instead of appending or replacing via -I replace-str")
     parser.add_argument("-I", action="store", type=str, default=None, metavar="replace-str", dest="replace_str",
                         help="replace occurrences of replace-str in command with input, default: {}")
     parser.add_argument("--resub", nargs=3, type=str, metavar=("pattern", "substitution", "replace-str"), dest="resub",
                         help="replace occurrences of replace-str in command with re.sub(patten, substitution, input)")
     parser.add_argument("-r", type=str, default=".", metavar="regex", dest="regex",
                         help="only build commands from inputs matching regex for input mode stdin, and matching relative paths for all other input modes, uses re.search")
     parser.add_argument("-o", action="store_true", dest="regex_omit",
                         help="omit inputs matching regex instead")
     parser.add_argument("-b", action="store_true", dest="regex_basename",
                         help="only match regex against basename of input (for input modes: file, path, abspath)")
-    group1.add_argument("-s", "--shell", action="store_true", dest="subprocess_shell",
+    parser.add_argument("--max-chars", type=int, metavar="n", dest="max_chars",
+                        help="omits any command line exceeding n characters, no limit by default")
+    group1.add_argument("--sh", "--shell", action="store_true", dest="subprocess_shell",
                         help="executes commands through the shell (subprocess shell=True) (no effect on Windows)")
     group1.add_argument("--py", "--pyex", action="store_true", dest="pyex",
                         help="executes commands as python code using exec()")
     group1.add_argument("--pyev", action="store_true", dest="pyev",
                         help="evaluates commands as python expressions using eval()")
     parser.add_argument("--import", action="append", type=str, default=[], metavar=("library"), dest="imprt",
                         help="executes 'import <library>' for each library")
@@ -319,14 +342,16 @@
                         help="runs exec(code) after execution")
     parser.add_argument("-P", "--procs", type=int, default=None, metavar="P", dest="procs",
                         help="split into P chunks and execute each chunk in parallel as a separate process and window with byobu or tmux")
     parser.add_argument("-c", "--chunk", type=int, default=None, metavar="c", dest="chunk",
                         help="runs chunk c of P (0 <= c < P) (without multiplexer)")
     parser.add_argument("--_command_pickle", nargs=2, default=None, dest="command_pickle",
                         help=argparse.SUPPRESS)
+    parser.add_argument("--no-mux", action="store_true", dest="no_mux",
+                        help="do not use a multiplexer for multiple processes")
     parser.add_argument("-i", "--interactive", action="store_true", dest="interactive",
                         help="prompt the user before executing each command, only proceeds if response starts with 'y' or 'Y'")
     parser.add_argument("-n", "--dry-run", action="store_true", dest="dry_run",
                         help="prints commands without executing them")
     parser.add_argument("-v", "--verbose", action="store_true", dest="verbose",
                         help="prints commands before executing them")
     args = parser.parse_args()
@@ -336,55 +361,67 @@
     # determine input mode and read stdin available or required
     stdin = ""
     if args.input_mode in ["f", "p", "a", "s"]:
         short_forms = {"f": "file", "p": "path", "a": "abspath", "s": "stdin"}
         args.input_mode = short_forms[args.input_mode]
     if args.command_pickle is not None:
         args.input_mode = args.command_pickle[0]
+    elif args.arg_file is not None and (args.input_mode is None or args.input_mode == "stdin"):
+        with open(args.arg_file, "r") as f:
+            stdin = f.read()
+        args.input_mode = "stdin"
     elif args.input_mode is None:
         if not sys.stdin.isatty():
             stdin = sys.stdin.read()
             args.input_mode = "stdin"
         else:
             args.input_mode = "file"
     elif args.input_mode == "stdin":
         stdin = sys.stdin.read()
     # need to open new tty for interactive mode if input was read from stdin
-    if args.interactive and stdin:
+    if args.interactive and stdin and args.arg_file is None:
         sys.stdin = open("/dev/tty")
     # set delimiter
     if args.null:
         args.delim = "\0"
+    # enable format string mode
+    if args.re_split is not None:
+        args.format_str = True
     # enable shell on windows
     if sys.platform.startswith("win32"):
         args.subprocess_shell = True
     # check for invalid arguments
     assert os.path.isdir(args.base_dir) and os.getcwd() == args.base_dir
     if args.input_mode == "stdin":
         assert not args.folders, "invalid option --folders for input mode: stdin"
         assert not args.top_level, "invalid option --top for input mode: stdin"
         assert not args.symlinks, "invalid option --symlinks for input mode: stdin"
         assert not args.regex_basename, "invalid option -b for input mode: stdin"
     else:
         assert not args.null, f"invalid option --null for input mode: {args.input_mode}"
-        assert not args.delim, f"invalid option --delimiter for input mode: {args.input_mode}"
+        assert args.delim is None, f"invalid option --delimiter for input mode: {args.input_mode}"
+        assert args.arg_file is None, f"invalid option --arg-file for input mode: {args.input_mode}"
+    assert not args.format_str or args.replace_str is None, "invalid option --format-str: cannot specify -I replace-str"
     assert args.procs is None or args.procs > 0, "invalid option --procs: requires P > 0"
     assert args.chunk is None or args.procs is not None, "invalid option --chunk: --procs must be specified"
     assert args.chunk is None or 0 <= args.chunk < args.procs, "invalid option --chunk: requires 0 <= c < P"
     assert args.command_pickle is None or args.chunk is not None, "invalid option --_command_pickle: --chunk must be specified"
+    assert not args.no_mux or args.procs is not None, "invalid option --no-mux: --procs must be specified"
+    assert not args.no_mux or args.chunk is None, "invalid option --no-mux: --chunk must not be specified"
+    assert not args.no_mux or not args.interactive, "invalid option --no-mux: interactive mode not supported"
     # build and run commands
     if len(args.command) >= 1:
         # build commands or load them from pickle if available
         if args.command_pickle is None:
             command_dicts = build_commands(args, stdin)
         else:
             with open(args.command_pickle[1], "rb") as f:
                 command_dicts = pickle.load(f)
         # run subprocesses with multiplexer if requested
-        if args.procs is not None and args.chunk is None:
+        if args.procs is not None and args.chunk is None and not args.no_mux:
             multiplexer = "byobu" if shutil.which("byobu") else "tmux" if shutil.which("tmux") else None
             assert multiplexer is not None, "multiplexer not found: install byobu or tmux"
             session = time.strftime("pyxargs_%Y%m%d_%H%M%S")
             command_pickle = tempfile.NamedTemporaryFile()
             pickle.dump(command_dicts, command_pickle.file)
             command_pickle.file.flush()
             pyxargs_command = [sys.executable, os.path.abspath(__file__), "--chunk", "0", "--_command_pickle", args.input_mode, command_pickle.name] + sys.argv[1:]
```

### Comparing `pyxargs-2.3.0/setup.py` & `pyxargs-2.4.0/setup.py`

 * *Files identical despite different names*

