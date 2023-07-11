# Comparing `tmp/fastchecks-0.1.0rc8.tar.gz` & `tmp/fastchecks-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchecks-0.1.0rc8.tar", max compression
+gzip compressed data, was "fastchecks-0.2.0.tar", max compression
```

## Comparing `fastchecks-0.1.0rc8.tar` & `fastchecks-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     4889 2023-07-11 10:14:23.709259 fastchecks-0.1.0rc8/README.md
--rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.1.0rc8/fastchecks/__init__.py
--rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.1.0rc8/fastchecks/check.py
--rw-r--r--   0        0        0    11388 2023-07-11 10:09:09.131089 fastchecks-0.1.0rc8/fastchecks/cli.py
--rw-r--r--   0        0        0     3069 2023-07-11 09:12:31.873443 fastchecks-0.1.0rc8/fastchecks/conf.py
--rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.1.0rc8/fastchecks/log.py
--rw-r--r--   0        0        0      892 2023-07-11 10:03:13.456792 fastchecks-0.1.0rc8/fastchecks/meta.py
--rw-r--r--   0        0        0     6992 2023-07-11 10:23:34.114164 fastchecks-0.1.0rc8/fastchecks/runner.py
--rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.1.0rc8/fastchecks/sockets/__init__.py
--rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.1.0rc8/fastchecks/sockets/postgres/__init__.py
--rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.1.0rc8/fastchecks/sockets/postgres/schema/down.sql
--rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc8/fastchecks/sockets/postgres/schema/up.sql
--rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.1.0rc8/fastchecks/types.py
--rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.1.0rc8/fastchecks/util.py
--rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.1.0rc8/fastchecks/vutil.py
--rw-r--r--   0        0        0     1963 2023-07-11 10:24:39.451237 fastchecks-0.1.0rc8/pyproject.toml
--rw-r--r--   0        0        0     5563 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 10:41:01.033771 fastchecks-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5047 2023-07-11 10:41:01.033929 fastchecks-0.2.0/README.md
+-rw-r--r--   0        0        0      569 2023-07-11 10:41:01.034019 fastchecks-0.2.0/fastchecks/NOTICE
+-rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.2.0/fastchecks/__init__.py
+-rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.2.0/fastchecks/check.py
+-rw-r--r--   0        0        0    11388 2023-07-11 10:41:00.994591 fastchecks-0.2.0/fastchecks/cli.py
+-rw-r--r--   0        0        0     3069 2023-07-11 09:12:31.873443 fastchecks-0.2.0/fastchecks/conf.py
+-rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.2.0/fastchecks/log.py
+-rw-r--r--   0        0        0      892 2023-07-11 10:41:00.994931 fastchecks-0.2.0/fastchecks/meta.py
+-rw-r--r--   0        0        0     6992 2023-07-11 10:41:00.995276 fastchecks-0.2.0/fastchecks/runner.py
+-rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.2.0/fastchecks/sockets/__init__.py
+-rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.2.0/fastchecks/sockets/postgres/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.2.0/fastchecks/sockets/postgres/schema/down.sql
+-rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.2.0/fastchecks/sockets/postgres/schema/up.sql
+-rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.2.0/fastchecks/types.py
+-rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.2.0/fastchecks/util.py
+-rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.2.0/fastchecks/vutil.py
+-rw-r--r--   0        0        0     1974 2023-07-11 10:41:01.034139 fastchecks-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5718 1970-01-01 00:00:00.000000 fastchecks-0.2.0/PKG-INFO
```

### Comparing `fastchecks-0.1.0rc8/README.md` & `fastchecks-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -98,7 +98,17 @@
     fastchecks check_all_loop_fg  # checks without interval will run with a default (configurable by the envar: `FC_DEFAULT_CHECK_INTERVAL_SECONDS`)
     ```
 
 4. That's it! You might want to explore further options:
     * For all possibilities, run: `fastchecks -h`
     * For instance, might you want to run all checks only once (e.g. to schedule with cron), run: `fastchecks check_all_once`
     * Or run a single website check once (without registering it): `fastchecks check_website 'https://www.postgresql.org/'`
+
+
+
+## Copyright / License
+
+Copyright 2023 Dr. Juan Miguel Cejuela
+
+SPDX-License-Identifier: Apache-2.0
+
+See files: [LICENSE](./LICENSE) & [NOTICE](./NOTICE).
```

### Comparing `fastchecks-0.1.0rc8/fastchecks/__init__.py` & `fastchecks-0.2.0/fastchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/check.py` & `fastchecks-0.2.0/fastchecks/check.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/cli.py` & `fastchecks-0.2.0/fastchecks/cli.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/conf.py` & `fastchecks-0.2.0/fastchecks/conf.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/log.py` & `fastchecks-0.2.0/fastchecks/log.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/meta.py` & `fastchecks-0.2.0/fastchecks/meta.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/runner.py` & `fastchecks-0.2.0/fastchecks/runner.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/sockets/__init__.py` & `fastchecks-0.2.0/fastchecks/sockets/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/sockets/postgres/__init__.py` & `fastchecks-0.2.0/fastchecks/sockets/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/sockets/postgres/schema/down.sql` & `fastchecks-0.2.0/fastchecks/sockets/postgres/schema/down.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/sockets/postgres/schema/up.sql` & `fastchecks-0.2.0/fastchecks/sockets/postgres/schema/up.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/types.py` & `fastchecks-0.2.0/fastchecks/types.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/util.py` & `fastchecks-0.2.0/fastchecks/util.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/fastchecks/vutil.py` & `fastchecks-0.2.0/fastchecks/vutil.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0rc8/pyproject.toml` & `fastchecks-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastchecks"
-version = "0.1.0-rc.8"
+version = "0.2.0"
 description = "🚥 Fast website monitoring backend service"
 authors = ["Dr. Juan Miguel Cejuela <i@juanmi.rocks>"]
 readme = "README.md"
 repository = "https://github.com/juanmirocks/fastchecks"
 packages = [{ include = "fastchecks" }]
 
 
@@ -51,19 +51,20 @@
 
 # poethepoet: python & shell scripts to run within poetry: https://poethepoet.natn.io/
 [tool.poe.tasks]
 # format code
 fmt = "black ."
 
 # run tests with coverage -- for now do not use xdist's `-n auto` option
-test = "pytest --cov=fastchecks --cov-report=term-missing --cov-report=lcov:.cov/coverage.lcov"  # HTML possible too: --cov-report=html:.cov/html"
+test = "pytest --cov=fastchecks --cov-report=term-missing --cov-report=lcov:.cov/coverage.lcov" # HTML possible too: --cov-report=html:.cov/html"
 
 lint_errors = "pyflakes ."
 
-lint_types.shell = "mypy || true"  # For now ignore possible non 0 exit code; but at least report
+# For now ignore possible non 0 exit code; but at least report warnings & errors
+lint_types.shell = "mypy || true"
 lint_types_strict.shell = "mypy --strict || true"
 
 lint_bandit = "bandit -c pyproject.toml -r ."
 # snyk is not installed as a python dependency, but as a shell command (see how to install Snyk CLI: https://docs.snyk.io/snyk-cli/install-the-snyk-cli)
 lint_snyk.shell = "snyk code test; snyk test"
 lint_sec = ["lint_bandit", "lint_snyk"]
```

### Comparing `fastchecks-0.1.0rc8/PKG-INFO` & `fastchecks-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastchecks
-Version: 0.1.0rc8
+Version: 0.2.0
 Summary: 🚥 Fast website monitoring backend service
 Home-page: https://github.com/juanmirocks/fastchecks
 Author: Dr. Juan Miguel Cejuela
 Author-email: i@juanmi.rocks
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -117,7 +117,17 @@
     ```
 
 4. That's it! You might want to explore further options:
     * For all possibilities, run: `fastchecks -h`
     * For instance, might you want to run all checks only once (e.g. to schedule with cron), run: `fastchecks check_all_once`
     * Or run a single website check once (without registering it): `fastchecks check_website 'https://www.postgresql.org/'`
 
+
+
+## Copyright / License
+
+Copyright 2023 Dr. Juan Miguel Cejuela
+
+SPDX-License-Identifier: Apache-2.0
+
+See files: [LICENSE](./LICENSE) & [NOTICE](./NOTICE).
+
```

