# Comparing `tmp/fastchecks-0.1.0rc6.tar.gz` & `tmp/fastchecks-0.1.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchecks-0.1.0rc6.tar", max compression
+gzip compressed data, was "fastchecks-0.1.0rc7.tar", max compression
```

## Comparing `fastchecks-0.1.0rc6.tar` & `fastchecks-0.1.0rc7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4826 2023-07-11 09:12:31.872679 fastchecks-0.1.0rc6/README.md
--rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.1.0rc6/fastchecks/__init__.py
--rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.1.0rc6/fastchecks/check.py
--rw-r--r--   0        0        0    11388 2023-07-11 10:09:09.131089 fastchecks-0.1.0rc6/fastchecks/cli.py
--rw-r--r--   0        0        0     3069 2023-07-11 09:12:31.873443 fastchecks-0.1.0rc6/fastchecks/conf.py
--rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.1.0rc6/fastchecks/log.py
--rw-r--r--   0        0        0      892 2023-07-11 10:03:13.456792 fastchecks-0.1.0rc6/fastchecks/meta.py
--rw-r--r--   0        0        0     6958 2023-07-11 09:12:31.873884 fastchecks-0.1.0rc6/fastchecks/runner.py
--rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.1.0rc6/fastchecks/sockets/__init__.py
--rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.1.0rc6/fastchecks/sockets/postgres/__init__.py
--rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.1.0rc6/fastchecks/sockets/postgres/schema/down.sql
--rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc6/fastchecks/sockets/postgres/schema/up.sql
--rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.1.0rc6/fastchecks/types.py
--rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.1.0rc6/fastchecks/util.py
--rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.1.0rc6/fastchecks/vutil.py
--rw-r--r--   0        0        0     1963 2023-07-11 10:09:39.459757 fastchecks-0.1.0rc6/pyproject.toml
--rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc6/PKG-INFO
+-rw-r--r--   0        0        0     4889 2023-07-11 10:14:23.709259 fastchecks-0.1.0rc7/README.md
+-rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.1.0rc7/fastchecks/__init__.py
+-rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.1.0rc7/fastchecks/check.py
+-rw-r--r--   0        0        0    11388 2023-07-11 10:09:09.131089 fastchecks-0.1.0rc7/fastchecks/cli.py
+-rw-r--r--   0        0        0     3069 2023-07-11 09:12:31.873443 fastchecks-0.1.0rc7/fastchecks/conf.py
+-rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.1.0rc7/fastchecks/log.py
+-rw-r--r--   0        0        0      892 2023-07-11 10:03:13.456792 fastchecks-0.1.0rc7/fastchecks/meta.py
+-rw-r--r--   0        0        0     6958 2023-07-11 09:12:31.873884 fastchecks-0.1.0rc7/fastchecks/runner.py
+-rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.1.0rc7/fastchecks/sockets/__init__.py
+-rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.1.0rc7/fastchecks/sockets/postgres/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.1.0rc7/fastchecks/sockets/postgres/schema/down.sql
+-rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc7/fastchecks/sockets/postgres/schema/up.sql
+-rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.1.0rc7/fastchecks/types.py
+-rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.1.0rc7/fastchecks/util.py
+-rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.1.0rc7/fastchecks/vutil.py
+-rw-r--r--   0        0        0     1963 2023-07-11 10:15:39.403127 fastchecks-0.1.0rc7/pyproject.toml
+-rw-r--r--   0        0        0     5563 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc7/PKG-INFO
```

### Comparing `fastchecks-0.1.0rc6/README.md` & `fastchecks-0.1.0rc7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: fastchecks
+Version: 0.1.0rc7
+Summary: 🚥 Fast website monitoring backend service
+Home-page: https://github.com/juanmirocks/fastchecks
+Author: Dr. Juan Miguel Cejuela
+Author-email: i@juanmi.rocks
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: apscheduler (==4.0.0a2)
+Requires-Dist: google-re2 (>=1.0,<2.0)
+Requires-Dist: psycopg[binary,pool] (>=3.1.9,<4.0.0)
+Requires-Dist: pydantic (>=2.0.1,<3.0.0)
+Project-URL: Repository, https://github.com/juanmirocks/fastchecks
+Description-Content-Type: text/markdown
+
 # 🚥 Fast website monitoring backend service
 
 [![Pypy latest version](https://img.shields.io/pypi/v/fastchecks.svg?color=blue)](https://pypi.org/project/fastchecks/)
 [![test & lint](https://github.com/juanmirocks/fastchecks/actions/workflows/test_n_lint.yml/badge.svg)](https://github.com/juanmirocks/fastchecks/actions/workflows/test_n_lint.yml)
 [![Coverage Status](https://coveralls.io/repos/github/juanmirocks/fastchecks/badge.svg?branch=develop)](https://coveralls.io/github/juanmirocks/fastchecks?branch=develop)
 [![Snyk](https://img.shields.io/badge/%20Snyk_security-monitored-8742B8?logo=snyk&logoColor=white)](https://github.com/juanmirocks/fastchecks/actions)
 
@@ -10,15 +28,15 @@
 ## Features
 
 **🍀 Feature-rich**
 * Websites to check & their results are stored in postgres by default 🐘 (the library is ready for other data stores / sockets).
   * You can use postgres locally installed, running on docker, or with a DBaaS, e.g. Aiven.
 * Run stored all websites once, at configurable-scheduled intervals, or even with your system's cron.
 * The scheduling keeps running even if the computer goes to sleep!
-* CLI API (with `argparse`) & Python's (Python >= 3.11).
+* CLI API & Python's (Python >= 3.11).
   * A [webserver](https://github.com/juanmirocks/fastchecks/issues/3) is planned.
 * ...and more!
 
 
 **🚀 Speed**
 * All operations are asynchronous. This app sits on 3 giants:
   * aiohttp
@@ -38,14 +56,22 @@
 * Further type checking with Pydantic (v2).
 * Further static analysis with pyflakes.
 
 
 
 ## Install
 
+### With pip
+
+```shell
+# You need to run this with a Python 3.11 environment -- You can manage different python versions for instance with `pyenv`
+pip install -U fastchecks
+```
+
+
 ### From source
 
 You need to have [python poetry](https://python-poetry.org/docs/) installed. Then:
 
 ```shell
 # clone this repository
 _reponame="fastchecks";
@@ -76,21 +102,22 @@
     # * by setting the envar: `FC_POSTGRES_CONNINFO`
     # For simplicity, commands below assume you've set `FC_POSTGRES_CONNINFO`, e.g.:
     export FC_POSTGRES_CONNINFO='postgres://localhost/fastchecks'
     ```
 
 2. Add some website URL checks info (to do check later)
     ```shell
-    python -m fastchecks.cli upsert_check 'https://example.org'  # Add a simple URL check
-    python -m fastchecks.cli upsert_check 'https://example.org' --regex 'Example D[a-z]+'  # Update the URL check to match the response body with a regex
-    python -m fastchecks.cli upsert_check 'https://python.org' --interval 5  # Add another URL check with a specific interval (in seconds)
+    fastchecks upsert_check 'https://example.org'  # Add a simple URL check
+    fastchecks upsert_check 'https://example.org' --regex 'Example D[a-z]+'  # Update the URL check to match the response body with a regex
+    fastchecks upsert_check 'https://python.org' --interval 5  # Add another URL check with a specific interval (in seconds)
     ```
 
 3. Run the checks at the scheduled intervals in the foreground until stopped.
     ```shell
-    python -m fastchecks.cli check_all_loop_fg  # checks without interval will run with a default (configurable by the envar: `FC_DEFAULT_CHECK_INTERVAL_SECONDS`)
+    fastchecks check_all_loop_fg  # checks without interval will run with a default (configurable by the envar: `FC_DEFAULT_CHECK_INTERVAL_SECONDS`)
     ```
 
 4. That's it! You might want to explore further options:
-    * For all possibilities, run: `python -m fastchecks.cli -h`
-    * For instance, might you want to run all checks only once (e.g. to schedule with cron), run: `python -m fastchecks.cli check_all_once`
-    * Or run a single website check once (without registering it): `python -m fastchecks.cli check_website 'https://www.postgresql.org/'`
+    * For all possibilities, run: `fastchecks -h`
+    * For instance, might you want to run all checks only once (e.g. to schedule with cron), run: `fastchecks check_all_once`
+    * Or run a single website check once (without registering it): `fastchecks check_website 'https://www.postgresql.org/'`
+
```

### Comparing `fastchecks-0.1.0rc6/fastchecks/__init__.py` & `fastchecks-0.1.0rc7/fastchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/check.py` & `fastchecks-0.1.0rc7/fastchecks/check.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/cli.py` & `fastchecks-0.1.0rc7/fastchecks/cli.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/conf.py` & `fastchecks-0.1.0rc7/fastchecks/conf.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/log.py` & `fastchecks-0.1.0rc7/fastchecks/log.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/meta.py` & `fastchecks-0.1.0rc7/fastchecks/meta.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/runner.py` & `fastchecks-0.1.0rc7/fastchecks/runner.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/sockets/__init__.py` & `fastchecks-0.1.0rc7/fastchecks/sockets/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/sockets/postgres/__init__.py` & `fastchecks-0.1.0rc7/fastchecks/sockets/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/sockets/postgres/schema/down.sql` & `fastchecks-0.1.0rc7/fastchecks/sockets/postgres/schema/down.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/sockets/postgres/schema/up.sql` & `fastchecks-0.1.0rc7/fastchecks/sockets/postgres/schema/up.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/types.py` & `fastchecks-0.1.0rc7/fastchecks/types.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/util.py` & `fastchecks-0.1.0rc7/fastchecks/util.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/fastchecks/vutil.py` & `fastchecks-0.1.0rc7/fastchecks/vutil.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc6/pyproject.toml` & `fastchecks-0.1.0rc7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastchecks"
-version = "0.1.0-rc.6"
+version = "0.1.0-rc.7"
 description = "🚥 Fast website monitoring backend service"
 authors = ["Dr. Juan Miguel Cejuela <i@juanmi.rocks>"]
 readme = "README.md"
 repository = "https://github.com/juanmirocks/fastchecks"
 packages = [{ include = "fastchecks" }]
```

### Comparing `fastchecks-0.1.0rc6/PKG-INFO` & `fastchecks-0.1.0rc7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: fastchecks
-Version: 0.1.0rc6
-Summary: 🚥 Fast website monitoring backend service
-Home-page: https://github.com/juanmirocks/fastchecks
-Author: Dr. Juan Miguel Cejuela
-Author-email: i@juanmi.rocks
-Requires-Python: >=3.11,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: apscheduler (==4.0.0a2)
-Requires-Dist: google-re2 (>=1.0,<2.0)
-Requires-Dist: psycopg[binary,pool] (>=3.1.9,<4.0.0)
-Requires-Dist: pydantic (>=2.0.1,<3.0.0)
-Project-URL: Repository, https://github.com/juanmirocks/fastchecks
-Description-Content-Type: text/markdown
-
 # 🚥 Fast website monitoring backend service
 
 [![Pypy latest version](https://img.shields.io/pypi/v/fastchecks.svg?color=blue)](https://pypi.org/project/fastchecks/)
 [![test & lint](https://github.com/juanmirocks/fastchecks/actions/workflows/test_n_lint.yml/badge.svg)](https://github.com/juanmirocks/fastchecks/actions/workflows/test_n_lint.yml)
 [![Coverage Status](https://coveralls.io/repos/github/juanmirocks/fastchecks/badge.svg?branch=develop)](https://coveralls.io/github/juanmirocks/fastchecks?branch=develop)
 [![Snyk](https://img.shields.io/badge/%20Snyk_security-monitored-8742B8?logo=snyk&logoColor=white)](https://github.com/juanmirocks/fastchecks/actions)
 
@@ -28,15 +10,15 @@
 ## Features
 
 **🍀 Feature-rich**
 * Websites to check & their results are stored in postgres by default 🐘 (the library is ready for other data stores / sockets).
   * You can use postgres locally installed, running on docker, or with a DBaaS, e.g. Aiven.
 * Run stored all websites once, at configurable-scheduled intervals, or even with your system's cron.
 * The scheduling keeps running even if the computer goes to sleep!
-* CLI API (with `argparse`) & Python's (Python >= 3.11).
+* CLI API & Python's (Python >= 3.11).
   * A [webserver](https://github.com/juanmirocks/fastchecks/issues/3) is planned.
 * ...and more!
 
 
 **🚀 Speed**
 * All operations are asynchronous. This app sits on 3 giants:
   * aiohttp
@@ -56,14 +38,22 @@
 * Further type checking with Pydantic (v2).
 * Further static analysis with pyflakes.
 
 
 
 ## Install
 
+### With pip
+
+```shell
+# You need to run this with a Python 3.11 environment -- You can manage different python versions for instance with `pyenv`
+pip install -U fastchecks
+```
+
+
 ### From source
 
 You need to have [python poetry](https://python-poetry.org/docs/) installed. Then:
 
 ```shell
 # clone this repository
 _reponame="fastchecks";
@@ -94,22 +84,21 @@
     # * by setting the envar: `FC_POSTGRES_CONNINFO`
     # For simplicity, commands below assume you've set `FC_POSTGRES_CONNINFO`, e.g.:
     export FC_POSTGRES_CONNINFO='postgres://localhost/fastchecks'
     ```
 
 2. Add some website URL checks info (to do check later)
     ```shell
-    python -m fastchecks.cli upsert_check 'https://example.org'  # Add a simple URL check
-    python -m fastchecks.cli upsert_check 'https://example.org' --regex 'Example D[a-z]+'  # Update the URL check to match the response body with a regex
-    python -m fastchecks.cli upsert_check 'https://python.org' --interval 5  # Add another URL check with a specific interval (in seconds)
+    fastchecks upsert_check 'https://example.org'  # Add a simple URL check
+    fastchecks upsert_check 'https://example.org' --regex 'Example D[a-z]+'  # Update the URL check to match the response body with a regex
+    fastchecks upsert_check 'https://python.org' --interval 5  # Add another URL check with a specific interval (in seconds)
     ```
 
 3. Run the checks at the scheduled intervals in the foreground until stopped.
     ```shell
-    python -m fastchecks.cli check_all_loop_fg  # checks without interval will run with a default (configurable by the envar: `FC_DEFAULT_CHECK_INTERVAL_SECONDS`)
+    fastchecks check_all_loop_fg  # checks without interval will run with a default (configurable by the envar: `FC_DEFAULT_CHECK_INTERVAL_SECONDS`)
     ```
 
 4. That's it! You might want to explore further options:
-    * For all possibilities, run: `python -m fastchecks.cli -h`
-    * For instance, might you want to run all checks only once (e.g. to schedule with cron), run: `python -m fastchecks.cli check_all_once`
-    * Or run a single website check once (without registering it): `python -m fastchecks.cli check_website 'https://www.postgresql.org/'`
-
+    * For all possibilities, run: `fastchecks -h`
+    * For instance, might you want to run all checks only once (e.g. to schedule with cron), run: `fastchecks check_all_once`
+    * Or run a single website check once (without registering it): `fastchecks check_website 'https://www.postgresql.org/'`
```

