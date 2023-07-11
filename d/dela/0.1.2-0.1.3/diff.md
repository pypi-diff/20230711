# Comparing `tmp/dela-0.1.2.tar.gz` & `tmp/dela-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dela-0.1.2.tar", max compression
+gzip compressed data, was "dela-0.1.3.tar", max compression
```

## Comparing `dela-0.1.2.tar` & `dela-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1345 2023-07-10 17:19:17.322883 dela-0.1.2/README.md
--rw-r--r--   0        0        0      267 2023-07-10 17:19:17.322883 dela-0.1.2/dela/FileReader.py
--rw-r--r--   0        0        0     3615 2023-07-10 17:19:17.322883 dela-0.1.2/dela/ListCommand.py
--rw-r--r--   0        0        0     1282 2023-07-10 17:19:17.322883 dela-0.1.2/dela/Todo.py
--rw-r--r--   0        0        0      580 2023-07-10 17:19:17.322883 dela-0.1.2/dela/TodoPresentation.py
--rw-r--r--   0        0        0        0 2023-07-10 17:19:17.322883 dela-0.1.2/dela/__init__.py
--rw-r--r--   0        0        0     1948 2023-07-10 17:19:17.322883 dela-0.1.2/dela/__main__.py
--rw-r--r--   0        0        0      123 2023-07-10 17:19:17.322883 dela-0.1.2/dela/logger.py
--rw-r--r--   0        0        0      367 2023-07-10 17:19:17.326884 dela-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 dela-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1599 2023-07-11 05:47:54.958781 dela-0.1.3/README.md
+-rw-r--r--   0        0        0      267 2023-07-11 05:47:54.958781 dela-0.1.3/dela/FileReader.py
+-rw-r--r--   0        0        0     3729 2023-07-11 05:47:54.958781 dela-0.1.3/dela/ListCommand.py
+-rw-r--r--   0        0        0     1295 2023-07-11 05:47:54.958781 dela-0.1.3/dela/Todo.py
+-rw-r--r--   0        0        0      580 2023-07-11 05:47:54.958781 dela-0.1.3/dela/TodoPresentation.py
+-rw-r--r--   0        0        0        0 2023-07-11 05:47:54.958781 dela-0.1.3/dela/__init__.py
+-rw-r--r--   0        0        0     2030 2023-07-11 05:47:54.958781 dela-0.1.3/dela/__main__.py
+-rw-r--r--   0        0        0      123 2023-07-11 05:47:54.958781 dela-0.1.3/dela/logger.py
+-rw-r--r--   0        0        0      367 2023-07-11 05:47:54.966781 dela-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 dela-0.1.3/PKG-INFO
```

### Comparing `dela-0.1.2/README.md` & `dela-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 
 ```
 CLI to list todos in markdown files, like Obsidian Vaults.
 
 Usage:
   dela -h | --help
   dela --version
-  dela list [-v] [--all] [--today] [--done] [--status=<symbol>] [--sort_by=<key>] [--format=<string>] [<glob>]
+  dela list [-v] [--all] [--today] [--done] [--someday] [--status=<symbol>] [--tag=<string>...] [--sort_by=<key>] [--format=<string>] [<glob>]
 
 Options:
   -h --help                     Show this screen
   -v --verbose                  Enable logging
   -a --all                      Show all todos including closed ones
-  -t --today                    Show only today tasks
+  -t --today                    Show only tasks due today or earlier
   -d --done                     Show only done tasks
+  --someday                     Show someday tasks marked with [s] status
   -s --status=<symbol>          Filter by status (x, a, c, ~, ...)
+  -tag=<string>                 Filter by tag (#work, #home, etc)
   --sort_by=<key>               Sort by given key
   --format=<string>             Format result with given template string.
   --version                     Show version.
 
 
 Template example:
     dela list --format='- [$status] $file: $title'
@@ -50,8 +52,9 @@
     - [ ] Todo
     - [x] Done
     - [n] Next
     - [~] Pending
     - [c] Cancelled
     - [ ] 20230703 Todo with a date. If it's the day, `dela list -t` will list this guy
     - [ ] Todo with tags #tagone #tagtwo
+    - [ ] 23330101 Future task will be hidden until the day become
 ```
```

### Comparing `dela-0.1.2/dela/ListCommand.py` & `dela-0.1.3/dela/ListCommand.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class ListCommandConfig(object):
     def __init__(self, args):
         self.glob = args['<glob>'] if args['<glob>'] else '*.md'
         self.format = (
             args['--format']
             if args['--format']
-            else '\u001b[30m- \u001b[0m\u001b[01m[$status]\u001b[0m \u001b[31m$file:\u001b[0m $title \u001b[0m\u001b[34m$tags\u001b[0m'
+            else '\u001b[30m- \u001b[0m\u001b[01m[$status]\u001b[0m \u001b[31m$file:\u001b[0m $title \u001b[0m\u001b[34m$tags\u001b[0m \u001b[31m$date\u001b[0m'
         )
         self.filter_by_status = args['--status'] if args['--status'] else None
         self.show_all = True if args['--all'] else False
         self.sort_by = args['--sort_by'] if args['--sort_by'] else None
         self.only_today = True if args['--today'] else False
         self.only_done = True if args['--done'] else False
         self.only_someday = True if args['--someday'] else False
@@ -58,25 +58,28 @@
         presentation = TodoPresentation(self.config.format)
         for i in result:
             presentation.present(i)
 
     def filter(self, todos):
         result = todos
 
+        YYYYmmDD = int(datetime.now().strftime('%Y%m%d'))
+
         if not self.config.show_all and not self.config.only_done and not self.config.only_someday:
             result = [
                 i
                 for i in result
                 if i.status
                 not in [
                     *Todo.STATUSES_DONE,
                     *Todo.STATUSES_ARCHIVED,
                     *Todo.STATUSES_CLOSED,
                     *Todo.STATUSES_SOMEDAY,
-                ]
+                ] 
+                and (not bool(i.date) or int(i.date) < YYYYmmDD)
             ]
 
         if self.config.only_someday:
             result = [i for i in result if i.status in Todo.STATUSES_SOMEDAY]
 
         if self.config.only_done:
             result = [i for i in result if i.status not in Todo.STATUSES_DONE]
@@ -88,16 +91,15 @@
 
         if self.config.filter_by_tags:
             result = [
                 i for i in result if bool(set(i.tags) & set(self.config.filter_by_tags))
             ]
 
         if self.config.only_today:
-            YYYYmmDD = datetime.now().strftime('%Y%m%d')
-            result = [i for i in result if i.date == YYYYmmDD]
+            result = [i for i in result if bool(i.date) and int(i.date) < YYYYmmDD]
 
         return result
 
     def sort(self, todos):
         result = todos
 
         if self.config.sort_by:
```

### Comparing `dela-0.1.2/dela/Todo.py` & `dela-0.1.3/dela/Todo.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             return None
 
         gd = match.groupdict()
 
         return Todo(
             title=gd['title'],
             status=gd['status'],
-            date=gd['date'] if 'date' in gd else None,
+            date=gd['date'] if 'date' in gd and gd['date'] else '',
             tags=gd['tagline'].split(' ')
             if 'tagline' in gd and gd['tagline'] is not None
             else [],
             file=file,
         )
 
     def __repr__(self):
```

### Comparing `dela-0.1.2/dela/TodoPresentation.py` & `dela-0.1.3/dela/TodoPresentation.py`

 * *Files identical despite different names*

### Comparing `dela-0.1.2/dela/__main__.py` & `dela-0.1.3/dela/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   dela --version
   dela list [-v] [--all] [--today] [--done] [--someday] [--status=<symbol>] [--tag=<string>...] [--sort_by=<key>] [--format=<string>] [<glob>]
 
 Options:
   -h --help                     Show this screen
   -v --verbose                  Enable logging
   -a --all                      Show all todos including closed ones
-  -t --today                    Show only today tasks
+  -t --today                    Show only tasks due today or earlier
   -d --done                     Show only done tasks
   --someday                     Show someday tasks marked with [s] status
   -s --status=<symbol>          Filter by status (x, a, c, ~, ...)
   -tag=<string>                 Filter by tag (#work, #home, etc)
   --sort_by=<key>               Sort by given key
   --format=<string>             Format result with given template string.
   --version                     Show version.
@@ -48,14 +48,15 @@
     - [ ] Todo
     - [x] Done
     - [n] Next
     - [~] Pending
     - [c] Cancelled
     - [ ] 20230703 Todo with a date. If it's the day, `dela list -t` will list this guy
     - [ ] Todo with tags #tagone #tagtwo
+    - [ ] 23330101 Future task will be hidden until the day become
 """
 
 version = pkg_resources.get_distribution("dela").version
 
 def main():
     args = docopt(doc, version=version)
```

### Comparing `dela-0.1.2/PKG-INFO` & `dela-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dela
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: 'Anton Shuvalov'
 Author-email: anton@shuvalov.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -30,23 +30,25 @@
 
 ```
 CLI to list todos in markdown files, like Obsidian Vaults.
 
 Usage:
   dela -h | --help
   dela --version
-  dela list [-v] [--all] [--today] [--done] [--status=<symbol>] [--sort_by=<key>] [--format=<string>] [<glob>]
+  dela list [-v] [--all] [--today] [--done] [--someday] [--status=<symbol>] [--tag=<string>...] [--sort_by=<key>] [--format=<string>] [<glob>]
 
 Options:
   -h --help                     Show this screen
   -v --verbose                  Enable logging
   -a --all                      Show all todos including closed ones
-  -t --today                    Show only today tasks
+  -t --today                    Show only tasks due today or earlier
   -d --done                     Show only done tasks
+  --someday                     Show someday tasks marked with [s] status
   -s --status=<symbol>          Filter by status (x, a, c, ~, ...)
+  -tag=<string>                 Filter by tag (#work, #home, etc)
   --sort_by=<key>               Sort by given key
   --format=<string>             Format result with given template string.
   --version                     Show version.
 
 
 Template example:
     dela list --format='- [$status] $file: $title'
@@ -68,9 +70,10 @@
     - [ ] Todo
     - [x] Done
     - [n] Next
     - [~] Pending
     - [c] Cancelled
     - [ ] 20230703 Todo with a date. If it's the day, `dela list -t` will list this guy
     - [ ] Todo with tags #tagone #tagtwo
+    - [ ] 23330101 Future task will be hidden until the day become
 ```
```

