# Comparing `tmp/panoptescli-1.1.4.tar.gz` & `tmp/panoptescli-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptescli-1.1.4.tar", last modified: Sat Dec  3 03:34:24 2022, max compression
+gzip compressed data, was "panoptescli-1.1.5.tar", last modified: Tue Jul 11 21:43:19 2023, max compression
```

## Comparing `panoptescli-1.1.4.tar` & `panoptescli-1.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 03:34:24.639731 panoptescli-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-03 03:34:21.000000 panoptescli-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2022-12-03 03:34:24.639731 panoptescli-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2022-12-03 03:34:21.000000 panoptescli-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 03:34:24.639731 panoptescli-1.1.4/panoptes_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 03:34:24.639731 panoptescli-1.1.4/panoptes_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/inaturalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)    20757 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/subject_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 03:34:24.639731 panoptescli-1.1.4/panoptes_cli/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/commands/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 03:34:24.639731 panoptescli-1.1.4/panoptes_cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2022-12-03 03:34:21.000000 panoptescli-1.1.4/panoptes_cli/scripts/panoptes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 03:34:24.639731 panoptescli-1.1.4/panoptescli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2022-12-03 03:34:24.000000 panoptescli-1.1.4/panoptescli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2022-12-03 03:34:24.000000 panoptescli-1.1.4/panoptescli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 03:34:24.000000 panoptescli-1.1.4/panoptescli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-03 03:34:24.000000 panoptescli-1.1.4/panoptescli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-03 03:34:24.000000 panoptescli-1.1.4/panoptescli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-03 03:34:24.000000 panoptescli-1.1.4/panoptescli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-03 03:34:24.639731 panoptescli-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      913 2022-12-03 03:34:21.000000 panoptescli-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:43:19.262840 panoptescli-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 21:43:13.000000 panoptescli-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-07-11 21:43:19.262840 panoptescli-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-11 21:43:13.000000 panoptescli-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:43:19.258840 panoptescli-1.1.5/panoptes_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:43:19.258840 panoptescli-1.1.5/panoptes_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/inaturalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/subject_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:43:19.258840 panoptescli-1.1.5/panoptes_cli/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/commands/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:43:19.258840 panoptescli-1.1.5/panoptes_cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-07-11 21:43:13.000000 panoptescli-1.1.5/panoptes_cli/scripts/panoptes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:43:19.262840 panoptescli-1.1.5/panoptescli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-07-11 21:43:19.000000 panoptescli-1.1.5/panoptescli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-11 21:43:19.000000 panoptescli-1.1.5/panoptescli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:43:19.000000 panoptescli-1.1.5/panoptescli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 21:43:19.000000 panoptescli-1.1.5/panoptescli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-11 21:43:19.000000 panoptescli-1.1.5/panoptescli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 21:43:19.000000 panoptescli-1.1.5/panoptescli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:43:19.262840 panoptescli-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-11 21:43:13.000000 panoptescli-1.1.5/setup.py
```

### Comparing `panoptescli-1.1.4/LICENSE` & `panoptescli-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/PKG-INFO` & `panoptescli-1.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptescli
-Version: 1.1.4
+Version: 1.1.5
 Summary: A command-line client for Panoptes, the API behind the Zooniverse
 Home-page: https://github.com/zooniverse/panoptes-cli
 Author: Adam McMaster / Zooniverse
 Author-email: contact@zooniverse.org
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -14,26 +14,28 @@
 
 A command-line interface for [Panoptes](https://github.com/zooniverse/Panoptes),
 the API behind [the Zooniverse](https://www.zooniverse.org/).
 
 ## Installation
 
 The Panoptes CLI is written in Python, so in order to install it you will need
-to install either Python 2 or Python 3, along with `pip`. macOS and Linux
-already come with Python installed, so run this to see if you already have
-everything you need:
+to install Python 3 along with `pip`. Please note: while still compatible with
+Python 2.7, we have ended support for use of the CLI with this deprecated version.
+macOS and Linux already come with Python installed, so run this to see if you 
+already have everything you need:
 
 ```
 $ python --version && pip --version
 ```
 
 If you see an error like `python: command not found` or `pip: command not found`
 then you will need to install this:
 
-- [Python installation](https://wiki.python.org/moin/BeginnersGuide/Download)
+- [Python installation](https://wiki.python.org/moin/BeginnersGuide/Download) 
+  (or [Miniconda installation](https://docs.conda.io/en/latest/miniconda.html))
 - [Pip installation](https://pip.pypa.io/en/stable/installing/)
 
 Once these are installed you can just use `pip` to install the latest release of
 the CLI:
 
 ```
 $ pip install panoptescli
@@ -312,14 +314,37 @@
 ### Add known subjects to a subject set
 
 ```
 # for known subjects with ids 3, 2, 1 and subject set with id 999
 $ panoptes subject-set add-subjects 999 3 2 1
 ```
 
+### Importing iNaturalist observations
+
+Importing iNaturalist observations to the Zooniverse as subjects is possible via an API endpoint, which is accessible via this client.
+
+This command initiates a background job on the Zooniverse platform to import Observations. The request will return a 200 upon success, and the import will begin as the Zooniverse and iNaturalist APIs talk to each other. Once the command is issued, the work is being done remotely and you can refresh the subject set in the project builder to check its progress. The authenticated user will receive an email when this job is completed; you don't have to keep the terminal open.
+
+This command imports “verifiable” observations, which  according to the iNat docs means “observations with a quality_grade of either `needs_id` or `research`." Project owners and collaborators can use this CLI to send a request to begin that import process:
+
+```
+# Requires an iNaturalist taxon id and a Zooniverse subject set (both integers). This will import all observations for that taxon id.
+$ panoptes inaturalist import-observations --taxon-id 46017 --subject-set-id 999999
+```
+
+Optional: include an updated_since timestamp (string) to include only observations updated after that date:
+
+```
+$ panoptes inaturalist import-observations --taxon-id 46017 --subject-set-id 999999 --updated-since 2022-12-03
+```
+
+The `--updated-since` argument is a standard ISO timestamp, such as '2022-12-03' or `2022-12-03T18:56:06+00:00'. It is passed directly to the iNat Observations v2 API as the 'updated_since' query parameter. 
+
+
+
 ## Debugging
 
 To view the various requests as sent to the Panoptes API as well as other info,
 include the env var `PANOPTES_DEBUG=true` before your command, like so:
 
 `PANOPTES_DEBUG=true panoptes workflow ls -p 1234`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `panoptescli-1.1.4/README.md` & `panoptescli-1.1.5/panoptescli.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,41 @@
+Metadata-Version: 2.1
+Name: panoptescli
+Version: 1.1.5
+Summary: A command-line client for Panoptes, the API behind the Zooniverse
+Home-page: https://github.com/zooniverse/panoptes-cli
+Author: Adam McMaster / Zooniverse
+Author-email: contact@zooniverse.org
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Panoptes CLI
 
 A command-line interface for [Panoptes](https://github.com/zooniverse/Panoptes),
 the API behind [the Zooniverse](https://www.zooniverse.org/).
 
 ## Installation
 
 The Panoptes CLI is written in Python, so in order to install it you will need
-to install either Python 2 or Python 3, along with `pip`. macOS and Linux
-already come with Python installed, so run this to see if you already have
-everything you need:
+to install Python 3 along with `pip`. Please note: while still compatible with
+Python 2.7, we have ended support for use of the CLI with this deprecated version.
+macOS and Linux already come with Python installed, so run this to see if you 
+already have everything you need:
 
 ```
 $ python --version && pip --version
 ```
 
 If you see an error like `python: command not found` or `pip: command not found`
 then you will need to install this:
 
-- [Python installation](https://wiki.python.org/moin/BeginnersGuide/Download)
+- [Python installation](https://wiki.python.org/moin/BeginnersGuide/Download) 
+  (or [Miniconda installation](https://docs.conda.io/en/latest/miniconda.html))
 - [Pip installation](https://pip.pypa.io/en/stable/installing/)
 
 Once these are installed you can just use `pip` to install the latest release of
 the CLI:
 
 ```
 $ pip install panoptescli
@@ -300,14 +314,37 @@
 ### Add known subjects to a subject set
 
 ```
 # for known subjects with ids 3, 2, 1 and subject set with id 999
 $ panoptes subject-set add-subjects 999 3 2 1
 ```
 
+### Importing iNaturalist observations
+
+Importing iNaturalist observations to the Zooniverse as subjects is possible via an API endpoint, which is accessible via this client.
+
+This command initiates a background job on the Zooniverse platform to import Observations. The request will return a 200 upon success, and the import will begin as the Zooniverse and iNaturalist APIs talk to each other. Once the command is issued, the work is being done remotely and you can refresh the subject set in the project builder to check its progress. The authenticated user will receive an email when this job is completed; you don't have to keep the terminal open.
+
+This command imports “verifiable” observations, which  according to the iNat docs means “observations with a quality_grade of either `needs_id` or `research`." Project owners and collaborators can use this CLI to send a request to begin that import process:
+
+```
+# Requires an iNaturalist taxon id and a Zooniverse subject set (both integers). This will import all observations for that taxon id.
+$ panoptes inaturalist import-observations --taxon-id 46017 --subject-set-id 999999
+```
+
+Optional: include an updated_since timestamp (string) to include only observations updated after that date:
+
+```
+$ panoptes inaturalist import-observations --taxon-id 46017 --subject-set-id 999999 --updated-since 2022-12-03
+```
+
+The `--updated-since` argument is a standard ISO timestamp, such as '2022-12-03' or `2022-12-03T18:56:06+00:00'. It is passed directly to the iNat Observations v2 API as the 'updated_since' query parameter. 
+
+
+
 ## Debugging
 
 To view the various requests as sent to the Panoptes API as well as other info,
 include the env var `PANOPTES_DEBUG=true` before your command, like so:
 
 `PANOPTES_DEBUG=true panoptes workflow ls -p 1234`
 
@@ -318,7 +355,9 @@
 2. Create and run all the containers with `docker-compose up`
 
 ### Testing
 
 1. Use docker to run a testing environment bash shell and run test commands .
     1. Run `docker-compose run --rm dev sh` to start an interactive shell in the container
     1. Run `python -m unittest discover` to run the full test suite
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `panoptescli-1.1.4/panoptes_cli/commands/configure.py` & `panoptescli-1.1.5/panoptes_cli/commands/configure.py`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/panoptes_cli/commands/inaturalist.py` & `panoptescli-1.1.5/panoptes_cli/commands/inaturalist.py`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/panoptes_cli/commands/info.py` & `panoptescli-1.1.5/panoptes_cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/panoptes_cli/commands/project.py` & `panoptescli-1.1.5/panoptes_cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/panoptes_cli/commands/subject.py` & `panoptescli-1.1.5/panoptes_cli/commands/subject.py`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/panoptes_cli/commands/subject_set.py` & `panoptescli-1.1.5/panoptes_cli/commands/subject_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         index_fields = [header.lstrip('%') for header in headers if header.startswith('%')]
         return ",".join(str(field) for field in index_fields)
 
     subject_set = SubjectSet.find(upload_state['subject_set_id'])
     if not resumed_upload:
         subject_rows = []
         for manifest_file in upload_state['manifest_files']:
-            with open(manifest_file, 'U') as manifest_f:
+            with open(manifest_file) as manifest_f:
                 file_root = os.path.dirname(manifest_file)
                 r = csv.reader(manifest_f, skipinitialspace=True)
                 headers = next(r)
                 # update set metadata for indexed sets
                 index_fields = get_index_fields(headers)
                 if index_fields:
                     subject_set.metadata['indexFields'] = index_fields
```

### Comparing `panoptescli-1.1.4/panoptes_cli/commands/tests/test_project.py` & `panoptescli-1.1.5/panoptes_cli/commands/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/panoptes_cli/commands/user.py` & `panoptescli-1.1.5/panoptes_cli/commands/user.py`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/panoptes_cli/commands/workflow.py` & `panoptescli-1.1.5/panoptes_cli/commands/workflow.py`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/panoptes_cli/scripts/panoptes.py` & `panoptescli-1.1.5/panoptes_cli/scripts/panoptes.py`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/panoptescli.egg-info/PKG-INFO` & `panoptescli-1.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-Metadata-Version: 2.1
-Name: panoptescli
-Version: 1.1.4
-Summary: A command-line client for Panoptes, the API behind the Zooniverse
-Home-page: https://github.com/zooniverse/panoptes-cli
-Author: Adam McMaster / Zooniverse
-Author-email: contact@zooniverse.org
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Panoptes CLI
 
 A command-line interface for [Panoptes](https://github.com/zooniverse/Panoptes),
 the API behind [the Zooniverse](https://www.zooniverse.org/).
 
 ## Installation
 
 The Panoptes CLI is written in Python, so in order to install it you will need
-to install either Python 2 or Python 3, along with `pip`. macOS and Linux
-already come with Python installed, so run this to see if you already have
-everything you need:
+to install Python 3 along with `pip`. Please note: while still compatible with
+Python 2.7, we have ended support for use of the CLI with this deprecated version.
+macOS and Linux already come with Python installed, so run this to see if you 
+already have everything you need:
 
 ```
 $ python --version && pip --version
 ```
 
 If you see an error like `python: command not found` or `pip: command not found`
 then you will need to install this:
 
-- [Python installation](https://wiki.python.org/moin/BeginnersGuide/Download)
+- [Python installation](https://wiki.python.org/moin/BeginnersGuide/Download) 
+  (or [Miniconda installation](https://docs.conda.io/en/latest/miniconda.html))
 - [Pip installation](https://pip.pypa.io/en/stable/installing/)
 
 Once these are installed you can just use `pip` to install the latest release of
 the CLI:
 
 ```
 $ pip install panoptescli
@@ -312,14 +302,37 @@
 ### Add known subjects to a subject set
 
 ```
 # for known subjects with ids 3, 2, 1 and subject set with id 999
 $ panoptes subject-set add-subjects 999 3 2 1
 ```
 
+### Importing iNaturalist observations
+
+Importing iNaturalist observations to the Zooniverse as subjects is possible via an API endpoint, which is accessible via this client.
+
+This command initiates a background job on the Zooniverse platform to import Observations. The request will return a 200 upon success, and the import will begin as the Zooniverse and iNaturalist APIs talk to each other. Once the command is issued, the work is being done remotely and you can refresh the subject set in the project builder to check its progress. The authenticated user will receive an email when this job is completed; you don't have to keep the terminal open.
+
+This command imports “verifiable” observations, which  according to the iNat docs means “observations with a quality_grade of either `needs_id` or `research`." Project owners and collaborators can use this CLI to send a request to begin that import process:
+
+```
+# Requires an iNaturalist taxon id and a Zooniverse subject set (both integers). This will import all observations for that taxon id.
+$ panoptes inaturalist import-observations --taxon-id 46017 --subject-set-id 999999
+```
+
+Optional: include an updated_since timestamp (string) to include only observations updated after that date:
+
+```
+$ panoptes inaturalist import-observations --taxon-id 46017 --subject-set-id 999999 --updated-since 2022-12-03
+```
+
+The `--updated-since` argument is a standard ISO timestamp, such as '2022-12-03' or `2022-12-03T18:56:06+00:00'. It is passed directly to the iNat Observations v2 API as the 'updated_since' query parameter. 
+
+
+
 ## Debugging
 
 To view the various requests as sent to the Panoptes API as well as other info,
 include the env var `PANOPTES_DEBUG=true` before your command, like so:
 
 `PANOPTES_DEBUG=true panoptes workflow ls -p 1234`
 
@@ -330,9 +343,7 @@
 2. Create and run all the containers with `docker-compose up`
 
 ### Testing
 
 1. Use docker to run a testing environment bash shell and run test commands .
     1. Run `docker-compose run --rm dev sh` to start an interactive shell in the container
     1. Run `python -m unittest discover` to run the full test suite
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `panoptescli-1.1.4/panoptescli.egg-info/SOURCES.txt` & `panoptescli-1.1.5/panoptescli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panoptescli-1.1.4/setup.py` & `panoptescli-1.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='panoptescli',
-    version='1.1.4',
+    version='1.1.5',
     url='https://github.com/zooniverse/panoptes-cli',
     author='Adam McMaster / Zooniverse',
     author_email='contact@zooniverse.org',
     description=(
         'A command-line client for Panoptes, the API behind the Zooniverse'
     ),
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'Click>=6.7,<8.2',
         'PyYAML>=5.1,<6.1',
-        'panoptes-client>=1.4,<2.0',
-        'humanize>=0.5.1,<4.5',
+        'panoptes-client>=1.6,<2.0',
+        'humanize>=0.5.1,<4.8',
         'pathvalidate>=0.29.0,<2.6',
     ],
     entry_points='''
         [console_scripts]
         panoptes=panoptes_cli.scripts.panoptes:cli
     ''',
 )
```

