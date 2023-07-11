# Comparing `tmp/entest-0.1.8.tar.gz` & `tmp/entest-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entest-0.1.8.tar", max compression
+gzip compressed data, was "entest-0.1.9.tar", max compression
```

## Comparing `entest-0.1.8.tar` & `entest-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1212 2022-06-14 07:12:02.374023 entest-0.1.8/README.md
--rw-r--r--   0        0        0      401 2022-06-13 12:07:53.970565 entest-0.1.8/entest/__init__.py
--rwxr-xr-x   0        0        0      991 2022-06-13 11:54:34.442121 entest-0.1.8/entest/cli.py
--rw-r--r--   0        0        0      943 2022-06-13 12:07:53.974223 entest-0.1.8/entest/const.py
--rw-r--r--   0        0        0     7756 2022-06-13 13:53:30.680045 entest-0.1.8/entest/dependency_decorator.py
--rw-r--r--   0        0        0     1486 2022-06-13 13:43:10.252408 entest-0.1.8/entest/graph.py
--rw-r--r--   0        0        0        0 2022-06-10 12:26:07.255051 entest-0.1.8/entest/py.typed
--rw-r--r--   0        0        0     1055 2022-06-13 13:29:00.638940 entest-0.1.8/entest/runner.py
--rw-r--r--   0        0        0      920 2022-06-14 07:23:14.240123 entest-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1931 2022-06-14 07:24:02.222302 entest-0.1.8/setup.py
--rw-r--r--   0        0        0     1892 2022-06-14 07:24:02.222517 entest-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1092 2022-06-14 07:27:40.001403 entest-0.1.9/README.md
+-rw-r--r--   0        0        0      401 2022-06-13 12:07:53.970565 entest-0.1.9/entest/__init__.py
+-rwxr-xr-x   0        0        0      991 2022-06-13 11:54:34.442121 entest-0.1.9/entest/cli.py
+-rw-r--r--   0        0        0      943 2022-06-13 12:07:53.974223 entest-0.1.9/entest/const.py
+-rw-r--r--   0        0        0     7756 2022-06-13 13:53:30.680045 entest-0.1.9/entest/dependency_decorator.py
+-rw-r--r--   0        0        0     1486 2022-06-13 13:43:10.252408 entest-0.1.9/entest/graph.py
+-rw-r--r--   0        0        0        0 2022-06-10 12:26:07.255051 entest-0.1.9/entest/py.typed
+-rw-r--r--   0        0        0     1055 2022-06-13 13:29:00.638940 entest-0.1.9/entest/runner.py
+-rw-r--r--   0        0        0      920 2022-06-14 07:28:02.816797 entest-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1811 2022-06-14 07:28:09.636346 entest-0.1.9/setup.py
+-rw-r--r--   0        0        0     1772 2022-06-14 07:28:09.636567 entest-0.1.9/PKG-INFO
```

### Comparing `entest-0.1.8/README.md` & `entest-0.1.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 
 I would like to change a lot of things structure-wise, but API will stay the same. In particular:
 - `depends_on` decorator with kwargs `previous`, `run_last` and `without`.
 - `STATUS` classificator. I see how it can be misused easily, but I will still ship this footgun.
 
 ## Run tests
 ```
-entest tests/onboarding_api/test_happy_path.py --graph
-entest tests/onboarding_api/test_happy_path.py
-entest tests/onboarding_api/test_happy_path.py --env env_name tests/spam_users.py
+entest --graph
+entest
+entest --env env_name tests/spam_users.py
 ```
```

### Comparing `entest-0.1.8/entest/cli.py` & `entest-0.1.9/entest/cli.py`

 * *Files identical despite different names*

### Comparing `entest-0.1.8/entest/const.py` & `entest-0.1.9/entest/const.py`

 * *Files identical despite different names*

### Comparing `entest-0.1.8/entest/dependency_decorator.py` & `entest-0.1.9/entest/dependency_decorator.py`

 * *Files identical despite different names*

### Comparing `entest-0.1.8/entest/graph.py` & `entest-0.1.9/entest/graph.py`

 * *Files identical despite different names*

### Comparing `entest-0.1.8/entest/runner.py` & `entest-0.1.9/entest/runner.py`

 * *Files identical despite different names*

### Comparing `entest-0.1.8/pyproject.toml` & `entest-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entest"
-version = "0.1.8"
+version = "0.1.9"
 description = "Write dependent integration tests. See my pycon talk."
 authors = ["Peteris Ratnieks <peteris.ratnieks@zealid.com>"]
 readme = "README.md"
 repository = "https://github.com/peteris-zealid/entest"
 keywords = ["test", "integration-test"]
 classifiers = ["Topic :: Software Development :: Testing", "Typing :: Typed"]
 include = ["entest/py.typed"]
```

### Comparing `entest-0.1.8/setup.py` & `entest-0.1.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['entest = entest.cli:main']}
 
 setup_kwargs = {
     'name': 'entest',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Write dependent integration tests. See my pycon talk.',
-    'long_description': '# Entest\nSee `tests/example.py`.\n\nTo have a test implicitly depend on all other tests use `run_last` flag. This is the case for teardown of critical resources for example users.\n\nTo have all tests implicitly depend on a given test place it closer to the root of the graph.\nUse `setup_setup` to take advantage of `depends_on` default behavior. (i.e. for the first decorated function in a module `TEST_ROOT` is taken do be the previous test)\n\nTo have a test depend on another test NOT being run use `without` flag. This is usefull for testing error flows.\n** Right now this does not work correctly **\n\n## Contributing\nPlease do not maintain a fork! Make a pull request and if it is not obviously bad I will merge it in a timely manner.\n\nI would like to change a lot of things structure-wise, but API will stay the same. In particular:\n- `depends_on` decorator with kwargs `previous`, `run_last` and `without`.\n- `STATUS` classificator. I see how it can be misused easily, but I will still ship this footgun.\n\n## Run tests\n```\nentest tests/onboarding_api/test_happy_path.py --graph\nentest tests/onboarding_api/test_happy_path.py\nentest tests/onboarding_api/test_happy_path.py --env env_name tests/spam_users.py\n```\n',
+    'long_description': '# Entest\nSee `tests/example.py`.\n\nTo have a test implicitly depend on all other tests use `run_last` flag. This is the case for teardown of critical resources for example users.\n\nTo have all tests implicitly depend on a given test place it closer to the root of the graph.\nUse `setup_setup` to take advantage of `depends_on` default behavior. (i.e. for the first decorated function in a module `TEST_ROOT` is taken do be the previous test)\n\nTo have a test depend on another test NOT being run use `without` flag. This is usefull for testing error flows.\n** Right now this does not work correctly **\n\n## Contributing\nPlease do not maintain a fork! Make a pull request and if it is not obviously bad I will merge it in a timely manner.\n\nI would like to change a lot of things structure-wise, but API will stay the same. In particular:\n- `depends_on` decorator with kwargs `previous`, `run_last` and `without`.\n- `STATUS` classificator. I see how it can be misused easily, but I will still ship this footgun.\n\n## Run tests\n```\nentest --graph\nentest\nentest --env env_name tests/spam_users.py\n```\n',
     'author': 'Peteris Ratnieks',
     'author_email': 'peteris.ratnieks@zealid.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/peteris-zealid/entest',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `entest-0.1.8/PKG-INFO` & `entest-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entest
-Version: 0.1.8
+Version: 0.1.9
 Summary: Write dependent integration tests. See my pycon talk.
 Home-page: https://github.com/peteris-zealid/entest
 Keywords: test,integration-test
 Author: Peteris Ratnieks
 Author-email: peteris.ratnieks@zealid.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -32,12 +32,12 @@
 
 I would like to change a lot of things structure-wise, but API will stay the same. In particular:
 - `depends_on` decorator with kwargs `previous`, `run_last` and `without`.
 - `STATUS` classificator. I see how it can be misused easily, but I will still ship this footgun.
 
 ## Run tests
 ```
-entest tests/onboarding_api/test_happy_path.py --graph
-entest tests/onboarding_api/test_happy_path.py
-entest tests/onboarding_api/test_happy_path.py --env env_name tests/spam_users.py
+entest --graph
+entest
+entest --env env_name tests/spam_users.py
 ```
```

