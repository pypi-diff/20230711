# Comparing `tmp/dnspropagation-0.0.3.tar.gz` & `tmp/dnspropagation-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnspropagation-0.0.3.tar", last modified: Sat Mar 18 21:20:29 2023, max compression
+gzip compressed data, was "dnspropagation-0.0.4.tar", last modified: Mon Jul 10 21:59:50 2023, max compression
```

## Comparing `dnspropagation-0.0.3.tar` & `dnspropagation-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 berkas1   (1000) berkas1   (1000)        0 2023-03-18 21:20:29.105882 dnspropagation-0.0.3/
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)     1068 2023-03-18 15:51:04.000000 dnspropagation-0.0.3/LICENSE.md
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)     1918 2023-03-18 21:20:29.105882 dnspropagation-0.0.3/PKG-INFO
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)     1403 2023-03-18 18:47:08.000000 dnspropagation-0.0.3/README.md
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)      646 2023-03-18 21:18:46.000000 dnspropagation-0.0.3/pyproject.toml
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)       66 2023-02-12 12:28:48.000000 dnspropagation-0.0.3/requirements.txt
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)       38 2023-03-18 21:20:29.105882 dnspropagation-0.0.3/setup.cfg
-drwxrwxr-x   0 berkas1   (1000) berkas1   (1000)        0 2023-03-18 21:20:29.105882 dnspropagation-0.0.3/src/
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)        0 2023-02-17 13:08:49.000000 dnspropagation-0.0.3/src/__init__.py
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)     4942 2023-03-18 21:18:41.000000 dnspropagation-0.0.3/src/cli.py
-drwxrwxr-x   0 berkas1   (1000) berkas1   (1000)        0 2023-03-18 21:20:29.105882 dnspropagation-0.0.3/src/dnspropagation.egg-info/
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)     1918 2023-03-18 21:20:29.000000 dnspropagation-0.0.3/src/dnspropagation.egg-info/PKG-INFO
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)      355 2023-03-18 21:20:29.000000 dnspropagation-0.0.3/src/dnspropagation.egg-info/SOURCES.txt
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)        1 2023-03-18 21:20:29.000000 dnspropagation-0.0.3/src/dnspropagation.egg-info/dependency_links.txt
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)       44 2023-03-18 21:20:29.000000 dnspropagation-0.0.3/src/dnspropagation.egg-info/entry_points.txt
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)       67 2023-03-18 21:20:29.000000 dnspropagation-0.0.3/src/dnspropagation.egg-info/requires.txt
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)       28 2023-03-18 21:20:29.000000 dnspropagation-0.0.3/src/dnspropagation.egg-info/top_level.txt
--rw-rw-r--   0 berkas1   (1000) berkas1   (1000)     4743 2023-03-18 15:48:40.000000 dnspropagation-0.0.3/src/dnspropagation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:59:50.809501 dnspropagation-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-10 21:59:32.000000 dnspropagation-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-10 21:59:50.809501 dnspropagation-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-10 21:59:32.000000 dnspropagation-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-10 21:59:32.000000 dnspropagation-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 21:59:32.000000 dnspropagation-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:59:50.809501 dnspropagation-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:59:50.805501 dnspropagation-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:59:32.000000 dnspropagation-0.0.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-07-10 21:59:32.000000 dnspropagation-0.0.4/src/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:59:50.805501 dnspropagation-0.0.4/src/dnspropagation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-10 21:59:50.000000 dnspropagation-0.0.4/src/dnspropagation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 21:59:50.000000 dnspropagation-0.0.4/src/dnspropagation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:59:50.000000 dnspropagation-0.0.4/src/dnspropagation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 21:59:50.000000 dnspropagation-0.0.4/src/dnspropagation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 21:59:50.000000 dnspropagation-0.0.4/src/dnspropagation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 21:59:50.000000 dnspropagation-0.0.4/src/dnspropagation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-10 21:59:32.000000 dnspropagation-0.0.4/src/dnspropagation.py
```

### Comparing `dnspropagation-0.0.3/LICENSE.md` & `dnspropagation-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dnspropagation-0.0.3/PKG-INFO` & `dnspropagation-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnspropagation
-Version: 0.0.3
+Version: 0.0.4
 Summary: DNS propagation checker
 Author-email: Simon Berka <berka@berkasimon.com>
 Project-URL: Homepage, https://github.com/berkas1/dnspropagation
 Project-URL: Bug Tracker, https://github.com/berkas1/dnspropagation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,24 +21,29 @@
 pip install dnspropagation
 ```
 
 ## Usage
 In the most simple form you can just specify type of record and domain name:
 ```
 dnspropagation a google.com
+
+# or you can use docker version
+docker run berkas1/dnspropagation a google.com
 ```
 
 It will check entries for a given type and domain name using five default public nameservers. It returns a human-readable colorful table. You can use `--json` or `--yaml` parameters to make it machine-readable.
 
 ![Table 1](extras/table1.png)
 
 ### Custom DNS servers
 You can either supply custom DNS server to query using the `--server` parameter, which can be used multiple times:
 ```shell
 dnspropagation --server 1.1.1.1 --server 8.8.8.8 a google.com
+# or
+docker run berkas1/dnspropagation --server 1.1.1.1 --server 8.8.8.8 a google.com
 ```
 
 OR you can add a yaml-formatted list of servers. This has to follow given format (as can be seen in [this](custom-list.yaml) file) and be supplied to the utility using the `--custom_list` parameter.
 
 
 ### Expected results
 You can expect a value to be returned by DNS servers. If this value is returned, its color will be green. Otherwise the value will be shown red.
```

### Comparing `dnspropagation-0.0.3/README.md` & `dnspropagation-0.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,29 @@
 pip install dnspropagation
 ```
 
 ## Usage
 In the most simple form you can just specify type of record and domain name:
 ```
 dnspropagation a google.com
+
+# or you can use docker version
+docker run berkas1/dnspropagation a google.com
 ```
 
 It will check entries for a given type and domain name using five default public nameservers. It returns a human-readable colorful table. You can use `--json` or `--yaml` parameters to make it machine-readable.
 
 ![Table 1](extras/table1.png)
 
 ### Custom DNS servers
 You can either supply custom DNS server to query using the `--server` parameter, which can be used multiple times:
 ```shell
 dnspropagation --server 1.1.1.1 --server 8.8.8.8 a google.com
+# or
+docker run berkas1/dnspropagation --server 1.1.1.1 --server 8.8.8.8 a google.com
 ```
 
 OR you can add a yaml-formatted list of servers. This has to follow given format (as can be seen in [this](custom-list.yaml) file) and be supplied to the utility using the `--custom_list` parameter.
 
 
 ### Expected results
 You can expect a value to be returned by DNS servers. If this value is returned, its color will be green. Otherwise the value will be shown red.
```

### Comparing `dnspropagation-0.0.3/pyproject.toml` & `dnspropagation-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dnspropagation"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Simon Berka", email="berka@berkasimon.com" },
 ]
 description = "DNS propagation checker"
 readme = "README.md"
 requires-python = ">=3.7"
 dynamic = ["dependencies"]
```

### Comparing `dnspropagation-0.0.3/src/cli.py` & `dnspropagation-0.0.4/src/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 
 import yaml
 import pkg_resources
 
 import dnspropagation
 
-version = "0.0.3"
+version = "0.0.4"
 
 def main():
     dns_servers = []
     args_dict = {'json': False, 'simple': False, 'debug': False, 'dnslist': None, 'random': None, 'country': None,
                  'owner': None, 'expected': None, 'server': None, 'custom_list': None, 'show_default': False}
 
     parser = argparse.ArgumentParser()
@@ -84,15 +84,18 @@
     if len(sys.argv) <= 1:
         print("You have to specify record type and domain name. Run the program with the --help to show more information.")
         exit(1)
 
     if args_dict["custom_list"] is None and args_dict["server"] is None:
         dns_servers = checker.default_dns
         if args_dict["show_default"]:
-            print(checker.default_dns)
+            if args_dict["yaml"]:
+                print(yaml.dump(checker.default_dns))
+            else:
+                print(checker.default_dns)
             exit(0)
 
     if args_dict["file"] is None and (args_dict["record_type"] is None or args_dict["domain"] is None):
         print("You have to specify record type and domain name. Run the program with the --help to show more information.")
         exit(1)
 
     if args_dict['custom_list']:
```

### Comparing `dnspropagation-0.0.3/src/dnspropagation.egg-info/PKG-INFO` & `dnspropagation-0.0.4/src/dnspropagation.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnspropagation
-Version: 0.0.3
+Version: 0.0.4
 Summary: DNS propagation checker
 Author-email: Simon Berka <berka@berkasimon.com>
 Project-URL: Homepage, https://github.com/berkas1/dnspropagation
 Project-URL: Bug Tracker, https://github.com/berkas1/dnspropagation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,24 +21,29 @@
 pip install dnspropagation
 ```
 
 ## Usage
 In the most simple form you can just specify type of record and domain name:
 ```
 dnspropagation a google.com
+
+# or you can use docker version
+docker run berkas1/dnspropagation a google.com
 ```
 
 It will check entries for a given type and domain name using five default public nameservers. It returns a human-readable colorful table. You can use `--json` or `--yaml` parameters to make it machine-readable.
 
 ![Table 1](extras/table1.png)
 
 ### Custom DNS servers
 You can either supply custom DNS server to query using the `--server` parameter, which can be used multiple times:
 ```shell
 dnspropagation --server 1.1.1.1 --server 8.8.8.8 a google.com
+# or
+docker run berkas1/dnspropagation --server 1.1.1.1 --server 8.8.8.8 a google.com
 ```
 
 OR you can add a yaml-formatted list of servers. This has to follow given format (as can be seen in [this](custom-list.yaml) file) and be supplied to the utility using the `--custom_list` parameter.
 
 
 ### Expected results
 You can expect a value to be returned by DNS servers. If this value is returned, its color will be green. Otherwise the value will be shown red.
```

### Comparing `dnspropagation-0.0.3/src/dnspropagation.py` & `dnspropagation-0.0.4/src/dnspropagation.py`

 * *Files identical despite different names*

