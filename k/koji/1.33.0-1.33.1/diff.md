# Comparing `tmp/koji-1.33.0.tar.gz` & `tmp/koji-1.33.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koji-1.33.0.tar", last modified: Tue May 23 15:24:58 2023, max compression
+gzip compressed data, was "koji-1.33.1.tar", last modified: Tue Jul 11 14:30:11 2023, max compression
```

## Comparing `koji-1.33.0.tar` & `koji-1.33.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.643170 koji-1.33.0/
--rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)      796 2021-05-31 13:08:21.000000 koji-1.33.0/COPYING
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2023-05-23 15:24:58.643170 koji-1.33.0/PKG-INFO
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2216 2023-03-13 16:13:03.000000 koji-1.33.0/README.md
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.634170 koji-1.33.0/cli/
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    13338 2023-03-13 16:13:03.000000 koji-1.33.0/cli/koji
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.636170 koji-1.33.0/cli/koji_cli/
--rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)        0 2021-05-31 13:15:50.000000 koji-1.33.0/cli/koji_cli/__init__.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   343204 2023-05-23 15:21:00.000000 koji-1.33.0/cli/koji_cli/commands.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    32560 2023-05-23 15:20:44.000000 koji-1.33.0/cli/koji_cli/lib.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.639170 koji-1.33.0/koji/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   137022 2023-05-22 08:03:48.000000 koji-1.33.0/koji/__init__.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       89 2023-05-23 15:21:07.000000 koji-1.33.0/koji/_version.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    14256 2023-03-13 16:13:03.000000 koji-1.33.0/koji/arch.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2634 2023-03-13 16:13:03.000000 koji-1.33.0/koji/context.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    63517 2023-05-23 15:20:44.000000 koji-1.33.0/koji/daemon.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     7535 2023-03-13 16:13:03.000000 koji-1.33.0/koji/plugin.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    12060 2023-04-17 07:29:52.000000 koji-1.33.0/koji/policy.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     9441 2023-03-14 12:56:33.000000 koji-1.33.0/koji/rpmdiff.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1154 2023-03-14 12:56:33.000000 koji-1.33.0/koji/server.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    33947 2023-03-14 12:56:33.000000 koji-1.33.0/koji/tasks.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    30372 2023-05-22 08:03:48.000000 koji-1.33.0/koji/util.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3575 2023-03-14 12:56:33.000000 koji-1.33.0/koji/xmlrpcplus.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.640170 koji-1.33.0/koji.egg-info/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2023-05-23 15:24:58.000000 koji-1.33.0/koji.egg-info/PKG-INFO
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      656 2023-05-23 15:24:58.000000 koji-1.33.0/koji.egg-info/SOURCES.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        1 2023-05-23 15:24:58.000000 koji-1.33.0/koji.egg-info/dependency_links.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       45 2023-05-23 15:24:58.000000 koji-1.33.0/koji.egg-info/requires.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       31 2023-05-23 15:24:58.000000 koji-1.33.0/koji.egg-info/top_level.txt
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.633170 koji-1.33.0/plugins/
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.641170 koji-1.33.0/plugins/cli/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3165 2023-03-14 12:56:33.000000 koji-1.33.0/plugins/cli/dud.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3607 2023-03-14 12:56:33.000000 koji-1.33.0/plugins/cli/kiwi.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4759 2023-03-13 16:13:03.000000 koji-1.33.0/plugins/cli/runroot.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2631 2023-03-13 16:13:03.000000 koji-1.33.0/plugins/cli/save_failed_tree.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4972 2023-05-22 08:03:48.000000 koji-1.33.0/plugins/cli/sidetag_cli.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       38 2023-05-23 15:24:58.643170 koji-1.33.0/setup.cfg
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)     2467 2023-03-21 11:20:32.000000 koji-1.33.0/setup.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.641170 koji-1.33.0/tests/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1467 2023-03-13 16:13:03.000000 koji-1.33.0/tests/test_docs_version.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    26795 2023-03-14 12:56:33.000000 koji-1.33.0/tests/test_scm.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.642170 koji-1.33.0/util/
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    41460 2023-05-22 08:03:48.000000 koji-1.33.0/util/koji-gc
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    53664 2023-03-14 12:56:33.000000 koji-1.33.0/util/koji-shadow
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    10290 2023-05-23 15:20:44.000000 koji-1.33.0/util/koji-sweep-db
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    56166 2023-05-22 08:03:48.000000 koji-1.33.0/util/kojira
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-07-11 14:30:11.519313 koji-1.33.1/
+-rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)      796 2021-05-31 13:08:21.000000 koji-1.33.1/COPYING
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2023-07-11 14:30:11.519313 koji-1.33.1/PKG-INFO
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2216 2023-03-13 16:13:03.000000 koji-1.33.1/README.md
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-07-11 14:30:11.515313 koji-1.33.1/cli/
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    13338 2023-03-13 16:13:03.000000 koji-1.33.1/cli/koji
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-07-11 14:30:11.516313 koji-1.33.1/cli/koji_cli/
+-rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)        0 2021-05-31 13:15:50.000000 koji-1.33.1/cli/koji_cli/__init__.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   344503 2023-07-11 14:30:02.000000 koji-1.33.1/cli/koji_cli/commands.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    32560 2023-06-19 07:16:30.000000 koji-1.33.1/cli/koji_cli/lib.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-07-11 14:30:11.517313 koji-1.33.1/koji/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   137022 2023-07-11 14:30:02.000000 koji-1.33.1/koji/__init__.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       89 2023-07-11 14:13:38.000000 koji-1.33.1/koji/_version.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    14256 2023-03-13 16:13:03.000000 koji-1.33.1/koji/arch.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2634 2023-03-13 16:13:03.000000 koji-1.33.1/koji/context.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    63517 2023-06-12 12:56:07.000000 koji-1.33.1/koji/daemon.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     7535 2023-03-13 16:13:03.000000 koji-1.33.1/koji/plugin.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    12060 2023-04-17 07:29:52.000000 koji-1.33.1/koji/policy.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     9441 2023-06-12 12:56:07.000000 koji-1.33.1/koji/rpmdiff.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1154 2023-03-14 12:56:33.000000 koji-1.33.1/koji/server.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    33947 2023-06-12 12:56:07.000000 koji-1.33.1/koji/tasks.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    30372 2023-06-22 13:32:27.000000 koji-1.33.1/koji/util.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3575 2023-03-14 12:56:33.000000 koji-1.33.1/koji/xmlrpcplus.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-07-11 14:30:11.518313 koji-1.33.1/koji.egg-info/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2023-07-11 14:30:11.000000 koji-1.33.1/koji.egg-info/PKG-INFO
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      656 2023-07-11 14:30:11.000000 koji-1.33.1/koji.egg-info/SOURCES.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        1 2023-07-11 14:30:11.000000 koji-1.33.1/koji.egg-info/dependency_links.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       45 2023-07-11 14:30:11.000000 koji-1.33.1/koji.egg-info/requires.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       31 2023-07-11 14:30:11.000000 koji-1.33.1/koji.egg-info/top_level.txt
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-07-11 14:30:11.515313 koji-1.33.1/plugins/
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-07-11 14:30:11.518313 koji-1.33.1/plugins/cli/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3165 2023-03-14 12:56:33.000000 koji-1.33.1/plugins/cli/dud.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3607 2023-06-12 12:56:07.000000 koji-1.33.1/plugins/cli/kiwi.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4759 2023-03-13 16:13:03.000000 koji-1.33.1/plugins/cli/runroot.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2631 2023-03-13 16:13:03.000000 koji-1.33.1/plugins/cli/save_failed_tree.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4972 2023-06-20 13:13:20.000000 koji-1.33.1/plugins/cli/sidetag_cli.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       38 2023-07-11 14:30:11.519313 koji-1.33.1/setup.cfg
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)     2467 2023-06-22 12:13:19.000000 koji-1.33.1/setup.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-07-11 14:30:11.518313 koji-1.33.1/tests/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1467 2023-03-13 16:13:03.000000 koji-1.33.1/tests/test_docs_version.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    26795 2023-06-12 12:56:07.000000 koji-1.33.1/tests/test_scm.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-07-11 14:30:11.519313 koji-1.33.1/util/
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    41460 2023-06-19 07:16:30.000000 koji-1.33.1/util/koji-gc
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    53664 2023-03-14 12:56:33.000000 koji-1.33.1/util/koji-shadow
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    10290 2023-06-19 07:16:30.000000 koji-1.33.1/util/koji-sweep-db
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    56166 2023-07-11 14:30:02.000000 koji-1.33.1/util/kojira
```

### Comparing `koji-1.33.0/COPYING` & `koji-1.33.1/COPYING`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/PKG-INFO` & `koji-1.33.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji
-Version: 1.33.0
+Version: 1.33.1
 Summary: Koji is a system for building and tracking RPMS. The base package contains shared libraries and the command-line interface.
 Home-page: http://pagure.io/koji/
 Author: Koji developers
 Author-email: koji-devel@lists.fedorahosted.org
 License: LGPLv2 and GPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `koji-1.33.0/README.md` & `koji-1.33.1/README.md`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/cli/koji` & `koji-1.33.1/cli/koji`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/cli/koji_cli/commands.py` & `koji-1.33.1/cli/koji_cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -959,47 +959,85 @@
 
 
 def handle_call(goptions, session, args):
     "Execute an arbitrary XML-RPC call"
     usage = """\
         usage: %prog call [options] <name> [<arg> ...]
 
+        <arg> values of the form NAME=VALUE are treated as keyword arguments
         Note, that you can use global option --noauth for anonymous calls here"""
     usage = textwrap.dedent(usage)
     parser = OptionParser(usage=get_usage_str(usage))
-    parser.add_option("--python", action="store_true",
+    parser.add_option("-p", "--python", action="store_true",
                       help="Use python syntax for RPC parameter values")
     parser.add_option("--kwargs",
-                      help="Specify keyword arguments as a dictionary (implies --python)")
+                      help="Specify keyword arguments as a dictionary (implies --python or "
+                           "--json-input)")
+    parser.add_option("-j", "--json", action="store_true",
+                      help="Use JSON syntax for input and output")
+    parser.add_option("--json-input", action="store_true", help="Use JSON syntax for input")
     parser.add_option("--json-output", action="store_true", help="Use JSON syntax for output")
+    parser.add_option("-b", "--bare-strings", action="store_true",
+                      help="Treat invalid json/python as bare strings")
     (options, args) = parser.parse_args(args)
     if len(args) < 1:
         parser.error("Please specify the name of the XML-RPC method")
-    if options.kwargs:
+    if options.json:
+        options.json_input = True
+        options.json_output = True
+    if options.python and options.json_input:
+        parser.error('The --python option conflicts with using --json-input')
+    if options.kwargs and not options.json_input:
+        # for backwards compatibility, --python is implied
         options.python = True
     if options.python and ast is None:
         parser.error("The ast module is required to read python syntax")
-    if options.json_output and json is None:
-        parser.error("The json module is required to output JSON syntax")
-    activate_session(session, goptions)
+    if (options.json_output or options.json_input) and json is None:
+        parser.error("The json module is required to use JSON syntax")
+
+    def parse_arg(arg):
+        try:
+            if options.python:
+                return ast.literal_eval(arg)
+            elif options.json_input:
+                return json.loads(arg)
+            else:
+                return arg_filter(arg)
+        except ValueError:
+            if options.bare_strings:
+                return arg
+            else:
+                parser.error("Invalid value: %r" % arg)
+
+    # the method to call
     name = args[0]
-    non_kw = []
+
+    # base kw args
+    # we update with name=value args later
     kw = {}
-    if options.python:
-        non_kw = [ast.literal_eval(a) for a in args[1:]]
-        if options.kwargs:
-            kw = ast.literal_eval(options.kwargs)
-    else:
-        for arg in args[1:]:
-            if arg.find('=') != -1:
-                key, value = arg.split('=', 1)
-                kw[key] = arg_filter(value)
-            else:
-                non_kw.append(arg_filter(arg))
+    if options.kwargs:
+        kw = parse_arg(options.kwargs)
+
+    kw_pat = re.compile(r'^([^\W0-9]\w*)=(.*)$')
+
+    # read the args
+    non_kw = []
+    for arg in args[1:]:
+        m = kw_pat.match(arg)
+        if m:
+            key, value = m.groups()
+            kw[key] = parse_arg(value)
+        else:
+            non_kw.append(parse_arg(arg))
+
+    # make the call
+    activate_session(session, goptions)
     response = getattr(session, name).__call__(*non_kw, **kw)
+
+    # print the result
     if options.json_output:
         print(json.dumps(response, indent=2, separators=(',', ': '), cls=DatetimeJSONEncoder))
     else:
         pprint.pprint(response)
 
 
 def anon_handle_mock_config(goptions, session, args):
```

### Comparing `koji-1.33.0/cli/koji_cli/lib.py` & `koji-1.33.1/cli/koji_cli/lib.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/__init__.py` & `koji-1.33.1/koji/__init__.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/arch.py` & `koji-1.33.1/koji/arch.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/context.py` & `koji-1.33.1/koji/context.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/daemon.py` & `koji-1.33.1/koji/daemon.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/plugin.py` & `koji-1.33.1/koji/plugin.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/policy.py` & `koji-1.33.1/koji/policy.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/rpmdiff.py` & `koji-1.33.1/koji/rpmdiff.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/server.py` & `koji-1.33.1/koji/server.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/tasks.py` & `koji-1.33.1/koji/tasks.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/util.py` & `koji-1.33.1/koji/util.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji/xmlrpcplus.py` & `koji-1.33.1/koji/xmlrpcplus.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/koji.egg-info/PKG-INFO` & `koji-1.33.1/koji.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji
-Version: 1.33.0
+Version: 1.33.1
 Summary: Koji is a system for building and tracking RPMS. The base package contains shared libraries and the command-line interface.
 Home-page: http://pagure.io/koji/
 Author: Koji developers
 Author-email: koji-devel@lists.fedorahosted.org
 License: LGPLv2 and GPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `koji-1.33.0/koji.egg-info/SOURCES.txt` & `koji-1.33.1/koji.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/plugins/cli/dud.py` & `koji-1.33.1/plugins/cli/dud.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/plugins/cli/kiwi.py` & `koji-1.33.1/plugins/cli/kiwi.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/plugins/cli/runroot.py` & `koji-1.33.1/plugins/cli/runroot.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/plugins/cli/save_failed_tree.py` & `koji-1.33.1/plugins/cli/save_failed_tree.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/plugins/cli/sidetag_cli.py` & `koji-1.33.1/plugins/cli/sidetag_cli.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/setup.py` & `koji-1.33.1/setup.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/tests/test_docs_version.py` & `koji-1.33.1/tests/test_docs_version.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/tests/test_scm.py` & `koji-1.33.1/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/util/koji-gc` & `koji-1.33.1/util/koji-gc`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/util/koji-shadow` & `koji-1.33.1/util/koji-shadow`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/util/koji-sweep-db` & `koji-1.33.1/util/koji-sweep-db`

 * *Files identical despite different names*

### Comparing `koji-1.33.0/util/kojira` & `koji-1.33.1/util/kojira`

 * *Files identical despite different names*

