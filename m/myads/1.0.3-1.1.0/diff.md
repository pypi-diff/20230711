# Comparing `tmp/myads-1.0.3.tar.gz` & `tmp/myads-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myads-1.0.3.tar", last modified: Mon Jun  5 16:59:51 2023, max compression
+gzip compressed data, was "myads-1.1.0.tar", last modified: Tue Jul 11 16:11:53 2023, max compression
```

## Comparing `myads-1.0.3.tar` & `myads-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4735 2023-06-05 16:59:51.447956 myads-1.0.3/PKG-INFO
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4241 2023-06-05 01:04:37.000000 myads-1.0.3/README.md
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      865 2023-06-05 16:58:49.000000 myads-1.0.3/pyproject.toml
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       38 2023-06-05 16:59:51.447956 myads-1.0.3/setup.cfg
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/src/
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/src/myads/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      769 2023-03-12 18:51:04.000000 myads-1.0.3/src/myads/__init__.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/src/myads/cite_tracker/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      614 2023-06-05 00:53:50.000000 myads-1.0.3/src/myads/cite_tracker/__init__.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     6631 2023-06-05 01:10:30.000000 myads-1.0.3/src/myads/cite_tracker/check.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2276 2023-04-19 21:46:53.000000 myads-1.0.3/src/myads/cite_tracker/report.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     3282 2023-06-05 00:51:56.000000 myads-1.0.3/src/myads/cite_tracker/users.py
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     9957 2023-04-19 21:46:45.000000 myads-1.0.3/src/myads/query.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/src/myads/scripts/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2622 2023-06-05 16:57:37.000000 myads-1.0.3/src/myads/scripts/myads.py
-drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-06-05 16:59:51.447956 myads-1.0.3/src/myads.egg-info/
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4735 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/PKG-INFO
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      424 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/SOURCES.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        1 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/dependency_links.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       51 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/entry_points.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       30 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/requires.txt
--rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        6 2023-06-05 16:59:51.000000 myads-1.0.3/src/myads.egg-info/top_level.txt
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-07-11 16:11:53.090417 myads-1.1.0/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4738 2023-07-11 16:11:53.090417 myads-1.1.0/PKG-INFO
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4244 2023-07-11 16:09:32.000000 myads-1.1.0/README.md
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      994 2023-07-11 15:42:53.000000 myads-1.1.0/pyproject.toml
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       38 2023-07-11 16:11:53.090417 myads-1.1.0/setup.cfg
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-07-11 16:11:53.086417 myads-1.1.0/src/
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-07-11 16:11:53.086417 myads-1.1.0/src/myads/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      803 2023-07-11 15:42:53.000000 myads-1.1.0/src/myads/__init__.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       22 2023-07-11 16:09:32.000000 myads-1.1.0/src/myads/_version.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-07-11 16:11:53.090417 myads-1.1.0/src/myads/cite_tracker/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     1623 2023-07-11 16:09:32.000000 myads-1.1.0/src/myads/cite_tracker/__init__.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)    11011 2023-07-11 15:42:53.000000 myads-1.1.0/src/myads/cite_tracker/check.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2526 2023-07-11 16:09:32.000000 myads-1.1.0/src/myads/cite_tracker/report.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     2780 2023-07-11 15:42:53.000000 myads-1.1.0/src/myads/cite_tracker/tracked_authors.py
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)    10093 2023-07-11 16:09:32.000000 myads-1.1.0/src/myads/query.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-07-11 16:11:53.090417 myads-1.1.0/src/myads/scripts/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     3135 2023-07-11 16:09:32.000000 myads-1.1.0/src/myads/scripts/myads.py
+drwxrwxr-x   0 mcalpine  (1000) mcalpine  (1000)        0 2023-07-11 16:11:53.090417 myads-1.1.0/src/myads.egg-info/
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)     4738 2023-07-11 16:11:53.000000 myads-1.1.0/src/myads.egg-info/PKG-INFO
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)      456 2023-07-11 16:11:53.000000 myads-1.1.0/src/myads.egg-info/SOURCES.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        1 2023-07-11 16:11:53.000000 myads-1.1.0/src/myads.egg-info/dependency_links.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       51 2023-07-11 16:11:53.000000 myads-1.1.0/src/myads.egg-info/entry_points.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)       30 2023-07-11 16:11:53.000000 myads-1.1.0/src/myads.egg-info/requires.txt
+-rw-rw-r--   0 mcalpine  (1000) mcalpine  (1000)        6 2023-07-11 16:11:53.000000 myads-1.1.0/src/myads.egg-info/top_level.txt
```

### Comparing `myads-1.0.3/PKG-INFO` & `myads-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myads
-Version: 1.0.3
+Version: 1.1.0
 Summary: Simple ADS API query package and citation tracker
 Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/stuartmcalpine/myADS
 Project-URL: repository, https://github.com/stuartmcalpine/myADS
 Keywords: nasa-ads,citations,astronomy,ads,python,arxiv
 Classifier: Programming Language :: Python :: 3
@@ -80,15 +80,15 @@
 
 You must add your [ADS API token](https://ui.adsabs.harvard.edu/help/api/) so
 the package can query on your behalf. 
 
 To add it run:
 
 ```bash
-myads token add <YOUR-API-TOKEN-HERE>
+myads token update <YOUR-API-TOKEN-HERE>
 ```
 
 ## Usage
 
 ### Citation reporter
 
 If you run `myads report` you will get a report of all your tracked authors
```

### Comparing `myads-1.0.3/README.md` & `myads-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 You must add your [ADS API token](https://ui.adsabs.harvard.edu/help/api/) so
 the package can query on your behalf. 
 
 To add it run:
 
 ```bash
-myads token add <YOUR-API-TOKEN-HERE>
+myads token update <YOUR-API-TOKEN-HERE>
 ```
 
 ## Usage
 
 ### Citation reporter
 
 If you run `myads report` you will get a report of all your tracked authors
```

### Comparing `myads-1.0.3/pyproject.toml` & `myads-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 ]
 dependencies = [
     'requests',
     'toml',
     'tabulate>=0.9.0'
 ]
 requires-python = ">=3.7"
-version = "1.0.3"
 keywords = ["nasa-ads", "citations", "astronomy", "ads", "python", "arxiv"]
+dynamic = ["version"] # Scrape the version dynamically from the package
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 
 [project.scripts]
 myads = "myads.scripts.myads:main"
 
 [project.urls]
 homepage = "https://github.com/stuartmcalpine/myADS"
 repository = "https://github.com/stuartmcalpine/myADS"
+
+[tool.setuptools.dynamic]
+version = {attr = "myads._version.__version__"}
```

### Comparing `myads-1.0.3/src/myads/__init__.py` & `myads-1.1.0/src/myads/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import toml
+from ._version import __version__
 
 # Working directory of ADS package (where database will be stored).
 _wd = os.path.abspath(os.path.join(os.path.dirname(__file__), "..", ".."))
 
 # See if database folder exists, if not make it.
 if not os.path.isdir(os.path.join(_wd, "database")):
     os.mkdir(os.path.join(_wd, "database"))
```

### Comparing `myads-1.0.3/src/myads/cite_tracker/report.py` & `myads-1.1.0/src/myads/cite_tracker/report.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,77 +2,92 @@
 
 import myads.cite_tracker as cite_tracker
 import toml
 from myads.query import ADSQueryWrapper
 from tabulate import tabulate
 
 
-def report():
+def report(long_report):
+    """
+    For each tracked author, print their current citation metrics.
+
+    Parameters
+    ----------
+    long_report : bool
+        True for more columns
+    """
 
-    # Load the user database.
-    assert os.path.isfile(
-        cite_tracker.USER_DATABASE
-    ), "No user database created yet, run 'myads --add_user'"
-    users = toml.load(cite_tracker.USER_DATABASE)
-    assert (
-        "ads_token" in users["metadata"].keys()
-    ), "No ADS API token has been added yet, run 'myads --set_ads_token <TOKEN>'"
+    authors = cite_tracker.load_author_list()
+    token = cite_tracker.load_ads_token()
 
     # Query object.
-    query = ADSQueryWrapper(users["metadata"]["ads_token"])
+    query = ADSQueryWrapper(token)
 
     # Loop over each user in the database.
-    for att in users.keys():
-        if "user" not in att:
+    for att in authors.keys():
+        if att == "metadata":
             continue
 
         # Extract this users information.
-        FIRST_NAME = users[att]["first_name"]
-        LAST_NAME = users[att]["last_name"]
-        ORCID = users[att]["orcid"]
+        FIRST_NAME = authors[att]["first_name"]
+        LAST_NAME = authors[att]["last_name"]
+        ORCID = authors[att]["orcid"]
         print(f"\nReporting cites for {FIRST_NAME} {LAST_NAME}...")
 
         # Query.
         if ORCID == "":
             q = f"first_author:{LAST_NAME},{FIRST_NAME}"
         else:
             q = (
                 f"orcid_pub:{ORCID} OR orcid_user:{ORCID} OR orcid_other:{ORCID} "
                 f"first_author:{LAST_NAME},{FIRST_NAME}"
             )
-
-        data = query.get(q=q, fl="title,citation_count,pubdate,bibcode")
+    
+        ret_list = "title,citation_count,pubdate,bibcode"
+        if long_report:
+            ret_list += ",read_count"
+        data = query.get(q=q, fl=ret_list)
 
         # Got a bad status code.
         if data is None:
             return
 
         # Found no papers in query.
         if len(data.papers) == 0:
             print(f"No paper hits for {FIRST_NAME} {LAST_NAME}")
             continue
 
         # Loop over each of my papers and print the number of cites.
         table = []
         for paper in data.papers:
-            table.append(
-                [
+
+            tmp = [
                     paper.title,
                     f"{paper.citation_count} ({paper.citations_per_year:.1f})",
                     paper.pubdate,
                     paper.link,
                 ]
-            )
+            
+            if long_report:
+                tmp.append(paper.read_count)
 
-        print(
-            tabulate(
-                table,
-                tablefmt="grid",
-                maxcolwidths=[50, None, None, None],
-                headers=[
+            table.append(tmp)
+
+        headers = [
                     "Title",
                     "Citations\n(per year)",
                     "Publication\nDate",
                     "Bibcode",
-                ],
+                ]
+        maxcolwidths=[50, None, None, None]
+        if long_report:
+            headers.append("Read count\n(90 days)")
+            maxcolwidths.append(None)
+
+        print(
+            tabulate(
+                table,
+                tablefmt="grid",
+                maxcolwidths=maxcolwidths,
+                headers=headers
             )
         )
```

### Comparing `myads-1.0.3/src/myads/query.py` & `myads-1.1.0/src/myads/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,31 +42,37 @@
             pubmonth = int(self.pubdate.split('-')[1])
             if pubmonth == 0:
                 pubmonth += 1
             dt = f"{pubyear}-{pubmonth}"
 
             # Compute time difference from now.
             diff = datetime.now() - datetime.strptime(dt, "%Y-%m")
+            diff = diff.total_seconds()
+
+            if diff <= 0:
+                diff = 0.0
 
             # Convert to years.
-            return diff.total_seconds() / 31536000
+            return diff / 31536000
         else:
             return None
 
     @property
     def citations_per_year(self) -> float:
         """ 
         How many citations has this paper has per year?
 
         Needs to have had "pubdate" and "citation_count" in the original query.
         """
 
         pubyears = self.get_years_since_publication()
-        if pubyears is None or not hasattr(self, "citation_count"):
+        if (pubyears is None) or (not hasattr(self, "citation_count")):
             return None
+        elif pubyears <= 1/12:
+            return 0.0
         else:
             return self.citation_count / pubyears
 
     @property
     def link(self) -> str:
         """ Return string hyperlink to ADS page for this paper """
```

### Comparing `myads-1.0.3/src/myads/scripts/myads.py` & `myads-1.1.0/src/myads/scripts/myads.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import myads.cite_tracker as cite_tracker
-
+import myads
 
 def main():
 
     # Command line options.
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(title="subcommand", dest="subcommand")
 
@@ -15,63 +15,77 @@
     token_parser = subparsers.add_parser("token", help="Add/update ADS API token")
     report_parser = subparsers.add_parser(
         "report", help="Report current citation statistics for tracked authors"
     )
     check_parser = subparsers.add_parser(
         "check", help="Check for any new cites for tracked authors"
     )
+    info_parser = subparsers.add_parser(
+        "info", help="Print info"
+    )
 
     # User options
     user_subparser = user_parser.add_subparsers(
         title="user_subparser", dest="user_subparser"
     )
     user_subparser.add_parser("add", help="Add a new author to be tracked")
     user_subparser.add_parser("list", help="List current tracked authors")
     tmp = user_subparser.add_parser("remove", help="Remove an existing tracked author")
-    tmp.add_argument("user_id", help="User ID of tracked author to remove")
+    tmp.add_argument("author_id", help="ID of tracked author to remove")
 
     # ADS API token options
     token_subparser = token_parser.add_subparsers(
         title="token_subparser", dest="token_subparser"
     )
-    tmp = token_subparser.add_parser("add", help="Add/update ADS API token")
+    tmp = token_subparser.add_parser("update", help="Add/update ADS API token")
     tmp.add_argument("ads_token", help="ADS token to add")
     token_subparser.add_parser("display", help="Display current ADS token")
 
     # Check options
     check_parser.add_argument(
         "--verbose", help="True for more output", action="store_true"
     )
 
+    # Report options
+    report_parser.add_argument(
+        "--short", help="True for less columns", action="store_true"
+    )
+
     args = parser.parse_args()
 
     if args.subcommand == "author":
 
         # Add a user to the database
         if args.user_subparser == "add":
-            cite_tracker.add_user()
+            cite_tracker.add_tracked_author()
 
         # Remove a user from the database
         elif args.user_subparser == "remove":
-            cite_tracker.remove_user(args.user_id)
+            cite_tracker.remove_tracked_author(args.author_id)
 
         # Print user list.
         elif args.user_subparser == "list":
-            cite_tracker.list_users()
+            cite_tracker.list_tracked_authors()
 
     elif args.subcommand == "token":
 
         # Set the ADS API token.
-        if args.token_subparser == "add":
-            cite_tracker.set_ads_token(args.ads_token)
+        if args.token_subparser == "update":
+            cite_tracker.update_ads_token(args.ads_token)
 
         # Display the current ADS API token.
         if args.token_subparser == "display":
-            cite_tracker.display_ads_token()
+            token = cite_tracker.load_ads_token()
+            print(f"Currently stored ADS token: {token}")
 
     # Report users current citation statistics
     elif args.subcommand == "report":
-        cite_tracker.report()
+        cite_tracker.report(not args.short)
 
     # Check if any new cites have been made to the user since last call
     elif args.subcommand == "check":
         cite_tracker.check(args.verbose)
+
+    # Print some info
+    elif args.subcommand == "info":
+        print(f"myADS version: {myads.__version__}")
+        print(f"databases located at: {cite_tracker.data_dir}")
```

### Comparing `myads-1.0.3/src/myads.egg-info/PKG-INFO` & `myads-1.1.0/src/myads.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myads
-Version: 1.0.3
+Version: 1.1.0
 Summary: Simple ADS API query package and citation tracker
 Author-email: Stuart McAlpine <stuart.mcalpine@fysik.su.se>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/stuartmcalpine/myADS
 Project-URL: repository, https://github.com/stuartmcalpine/myADS
 Keywords: nasa-ads,citations,astronomy,ads,python,arxiv
 Classifier: Programming Language :: Python :: 3
@@ -80,15 +80,15 @@
 
 You must add your [ADS API token](https://ui.adsabs.harvard.edu/help/api/) so
 the package can query on your behalf. 
 
 To add it run:
 
 ```bash
-myads token add <YOUR-API-TOKEN-HERE>
+myads token update <YOUR-API-TOKEN-HERE>
 ```
 
 ## Usage
 
 ### Citation reporter
 
 If you run `myads report` you will get a report of all your tracked authors
```

