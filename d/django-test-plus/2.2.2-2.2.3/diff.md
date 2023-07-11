# Comparing `tmp/django-test-plus-2.2.2.tar.gz` & `tmp/django-test-plus-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-test-plus-2.2.2.tar", last modified: Tue Jun 27 18:51:55 2023, max compression
+gzip compressed data, was "django-test-plus-2.2.3.tar", last modified: Tue Jul 11 11:43:36 2023, max compression
```

## Comparing `django-test-plus-2.2.2.tar` & `django-test-plus-2.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-06-27 18:51:55.744766 django-test-plus-2.2.2/
--rw-r--r--   0 frank      (501) staff       (20)      752 2023-05-17 13:29:22.000000 django-test-plus-2.2.2/AUTHORS.txt
--rw-r--r--   0 frank      (501) staff       (20)     4649 2023-06-27 18:42:38.000000 django-test-plus-2.2.2/CHANGELOG.md
--rw-r--r--   0 frank      (501) staff       (20)     1559 2015-05-23 16:37:20.000000 django-test-plus-2.2.2/LICENSE
--rw-r--r--   0 frank      (501) staff       (20)      136 2023-05-17 13:26:35.000000 django-test-plus-2.2.2/MANIFEST.in
--rw-r--r--   0 frank      (501) staff       (20)    20239 2023-06-27 18:51:55.744843 django-test-plus-2.2.2/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)    19007 2023-05-17 13:26:35.000000 django-test-plus-2.2.2/README.md
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-06-27 18:51:55.743691 django-test-plus-2.2.2/django_test_plus.egg-info/
--rw-r--r--   0 frank      (501) staff       (20)    20239 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)      491 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/SOURCES.txt
--rw-r--r--   0 frank      (501) staff       (20)        1 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/dependency_links.txt
--rw-r--r--   0 frank      (501) staff       (20)       40 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/entry_points.txt
--rw-r--r--   0 frank      (501) staff       (20)        1 2019-05-12 15:19:09.000000 django-test-plus-2.2.2/django_test_plus.egg-info/not-zip-safe
--rw-r--r--   0 frank      (501) staff       (20)       86 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/requires.txt
--rw-r--r--   0 frank      (501) staff       (20)       10 2023-06-27 18:51:55.000000 django-test-plus-2.2.2/django_test_plus.egg-info/top_level.txt
--rw-r--r--   0 frank      (501) staff       (20)      229 2023-05-17 13:26:35.000000 django-test-plus-2.2.2/pytest.ini
--rw-r--r--   0 frank      (501) staff       (20)     1584 2023-06-27 18:51:55.745262 django-test-plus-2.2.2/setup.cfg
--rw-r--r--   0 frank      (501) staff       (20)       38 2022-10-12 15:57:24.000000 django-test-plus-2.2.2/setup.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-06-27 18:51:55.744653 django-test-plus-2.2.2/test_plus/
--rw-r--r--   0 frank      (501) staff       (20)       90 2022-01-27 21:26:25.000000 django-test-plus-2.2.2/test_plus/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)      890 2022-10-12 15:57:24.000000 django-test-plus-2.2.2/test_plus/compat.py
--rw-r--r--   0 frank      (501) staff       (20)      632 2022-10-12 15:57:24.000000 django-test-plus-2.2.2/test_plus/plugin.py
--rw-r--r--   0 frank      (501) staff       (20)      556 2017-10-24 13:55:52.000000 django-test-plus-2.2.2/test_plus/runner.py
--rw-r--r--   0 frank      (501) staff       (20)     9316 2022-10-12 15:57:24.000000 django-test-plus-2.2.2/test_plus/status_codes.py
--rw-r--r--   0 frank      (501) staff       (20)    19587 2023-06-27 18:36:37.000000 django-test-plus-2.2.2/test_plus/test.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-07-11 11:43:36.410457 django-test-plus-2.2.3/
+-rw-r--r--   0 frank      (501) staff       (20)      752 2023-05-17 13:29:22.000000 django-test-plus-2.2.3/AUTHORS.txt
+-rw-r--r--   0 frank      (501) staff       (20)     4752 2023-07-11 11:36:28.000000 django-test-plus-2.2.3/CHANGELOG.md
+-rw-r--r--   0 frank      (501) staff       (20)     1559 2015-05-23 16:37:20.000000 django-test-plus-2.2.3/LICENSE
+-rw-r--r--   0 frank      (501) staff       (20)      136 2023-05-17 13:26:35.000000 django-test-plus-2.2.3/MANIFEST.in
+-rw-r--r--   0 frank      (501) staff       (20)    20132 2023-07-11 11:43:36.410531 django-test-plus-2.2.3/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)    18900 2023-06-27 18:59:49.000000 django-test-plus-2.2.3/README.md
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-07-11 11:43:36.409773 django-test-plus-2.2.3/django_test_plus.egg-info/
+-rw-r--r--   0 frank      (501) staff       (20)    20132 2023-07-11 11:43:36.000000 django-test-plus-2.2.3/django_test_plus.egg-info/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)      491 2023-07-11 11:43:36.000000 django-test-plus-2.2.3/django_test_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2023-07-11 11:43:36.000000 django-test-plus-2.2.3/django_test_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 frank      (501) staff       (20)       40 2023-07-11 11:43:36.000000 django-test-plus-2.2.3/django_test_plus.egg-info/entry_points.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2019-05-12 15:19:09.000000 django-test-plus-2.2.3/django_test_plus.egg-info/not-zip-safe
+-rw-r--r--   0 frank      (501) staff       (20)       86 2023-07-11 11:43:36.000000 django-test-plus-2.2.3/django_test_plus.egg-info/requires.txt
+-rw-r--r--   0 frank      (501) staff       (20)       10 2023-07-11 11:43:36.000000 django-test-plus-2.2.3/django_test_plus.egg-info/top_level.txt
+-rw-r--r--   0 frank      (501) staff       (20)      229 2023-05-17 13:26:35.000000 django-test-plus-2.2.3/pytest.ini
+-rw-r--r--   0 frank      (501) staff       (20)     1584 2023-07-11 11:43:36.410948 django-test-plus-2.2.3/setup.cfg
+-rw-r--r--   0 frank      (501) staff       (20)       38 2022-10-12 15:57:24.000000 django-test-plus-2.2.3/setup.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-07-11 11:43:36.410347 django-test-plus-2.2.3/test_plus/
+-rw-r--r--   0 frank      (501) staff       (20)       90 2022-01-27 21:26:25.000000 django-test-plus-2.2.3/test_plus/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)      890 2022-10-12 15:57:24.000000 django-test-plus-2.2.3/test_plus/compat.py
+-rw-r--r--   0 frank      (501) staff       (20)      632 2022-10-12 15:57:24.000000 django-test-plus-2.2.3/test_plus/plugin.py
+-rw-r--r--   0 frank      (501) staff       (20)      556 2017-10-24 13:55:52.000000 django-test-plus-2.2.3/test_plus/runner.py
+-rw-r--r--   0 frank      (501) staff       (20)     9316 2022-10-12 15:57:24.000000 django-test-plus-2.2.3/test_plus/status_codes.py
+-rw-r--r--   0 frank      (501) staff       (20)    19810 2023-07-11 11:35:33.000000 django-test-plus-2.2.3/test_plus/test.py
```

### Comparing `django-test-plus-2.2.2/AUTHORS.txt` & `django-test-plus-2.2.3/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.2/CHANGELOG.md` & `django-test-plus-2.2.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changes
 
+## Version 2.2.3 - July 11th, 2023
+
+  - Fix bug where email addresses were not created by make_user()
+
 ## Version 2.2.2 - June 27, 2023
 
   - Fix issue with User creation helper when User model doesn't have a username field
   - Improve assertNumQueriesLessThan
   - Add assertInContext
 
 ## version 2.2.1 - October 12, 2022
```

### Comparing `django-test-plus-2.2.2/LICENSE` & `django-test-plus-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.2/PKG-INFO` & `django-test-plus-2.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-test-plus
-Version: 2.2.2
+Version: 2.2.3
 Summary: "django-test-plus provides useful additions to Django's default TestCase"
 Home-page: https://github.com/revsys/django-test-plus/
 Author: Frank Wiles
 Author-email: frank@revsys.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -41,14 +41,18 @@
 
 Let's face it, writing tests isn't always fun. Part of the reason for
 that is all of the boilerplate you end up writing. django-test-plus is
 an attempt to cut down on some of that when writing Django tests. We
 guarantee it will increase the time before you get carpal tunnel by at
 least 3 weeks!
 
+If you would like to get started testing your Django apps or improve how your
+team is testing we offer [TestStart](https://www.revsys.com/teststart/)
+to help your team dramatically improve your productivity.
+
 ## Support
 
 Supports: Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11.
 
 Supports Django Versions: 2.0, 2.1, 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, and 4.2.
 
 ## Documentation
@@ -91,15 +95,15 @@
 ```python
 from myproject.test import TestCase
 
 class MyViewTests(TestCase):
     ...
 ```
 
-This import, which is similar to the way you would import Django's TestCase, 
+This import, which is similar to the way you would import Django's TestCase,
 is also valid:
 
 ```python
 from test_plus import TestCase
 ```
 
 ## pytest Usage
@@ -260,15 +264,15 @@
     self.assert_http_200_ok(response)
 ```
 
 Django-test-plus provides a majority of the status codes assertions for you. The status assertions
 can be found in their own [mixin](https://github.com/revsys/django-test-plus/blob/main/test_plus/status_codes.py)
 and should be searchable if you're using an IDE like pycharm. It should be noted that in previous
 versions, django-test-plus had assertion methods in the pattern of `response_###()`, which are still
-available but have since been deprecated. See below for a list of those methods. 
+available but have since been deprecated. See below for a list of those methods.
 
 Each of the assertion methods takes an optional Django test client `response` and a string `msg` argument
 that, if specified, is used as the error message when a failure occurs. The methods,
 `assert_http_301_moved_permanently` and `assert_http_302_found` also take an optional `url` argument that
 if passed, will check to make sure the `response.url` matches.
 
 If it's available, the `assert_http_###_<status_name>` methods will use the last response. So you
@@ -278,30 +282,30 @@
 def test_status(self):
     self.get('my-url-name')
     self.assert_http_200_ok()
 ```
 
 Which is a bit shorter.
 
-The `response_###()` methods that are deprecated, but still available for use, include: 
+The `response_###()` methods that are deprecated, but still available for use, include:
 
 - `response_200()`
-- `response_201()` 
-- `response_204()` 
+- `response_201()`
+- `response_204()`
 - `response_301()`
-- `response_302()` 
+- `response_302()`
 - `response_400()`
-- `response_401()` 
+- `response_401()`
 - `response_403()`
-- `response_404()` 
+- `response_404()`
 - `response_405()`
 - `response_409()`
 - `response_410()`
 
-All of which take an optional Django test client response and a str msg argument that, if specified, is used as the error message when a failure occurs. Just like the `assert_http_###_<status_name>()` methods, these methods will use the last response if it's available. 
+All of which take an optional Django test client response and a str msg argument that, if specified, is used as the error message when a failure occurs. Just like the `assert_http_###_<status_name>()` methods, these methods will use the last response if it's available.
 
 ## `get_check_200(url_name, *args, **kwargs)`
 
 GETing and checking views return status 200 is a common test. This method makes it more convenient::
 
 ```python
 def test_even_better_status(self):
@@ -436,15 +440,15 @@
 ## Ensuring low query counts
 
 ### `assertNumQueriesLessThan(number)` - context
 
 Django provides
 [`assertNumQueries`](https://docs.djangoproject.com/en/1.8/topics/testing/tools/#django.test.TransactionTestCase.assertNumQueries)
 which is great when your code generates a specific number of
-queries. However, if this number varies due to the nature of your data, with 
+queries. However, if this number varies due to the nature of your data, with
 this method you can still test to ensure the code doesn't start producing a ton
 more queries than you expect:
 
 ```python
 def test_something_out(self):
 
     with self.assertNumQueriesLessThan(7):
@@ -633,9 +637,7 @@
 ## Keep in touch!
 
 If you have a question about this project, please open a GitHub issue. If you love us and want to keep track of our goings-on, here's where you can find us online:
 
 <a href="https://revsys.com?utm_medium=github&utm_source=django-test-plus"><img src="https://pbs.twimg.com/profile_images/915928618840285185/sUdRGIn1_400x400.jpg" height="50" /></a>
 <a href="https://twitter.com/revsys"><img src="https://cdn1.iconfinder.com/data/icons/new_twitter_icon/256/bird_twitter_new_simple.png" height="43" /></a>
 <a href="https://www.facebook.com/revsysllc/"><img src="https://cdn3.iconfinder.com/data/icons/picons-social/57/06-facebook-512.png" height="50" /></a>
-<a href="https://github.com/revsys/"><img src="https://assets-cdn.github.com/images/modules/logos_page/GitHub-Mark.png" height="53" /></a>
-<a href="https://gitlab.com/revsys"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/GitLab_Logo.svg/2000px-GitLab_Logo.svg.png" height="44" /></a>
```

### Comparing `django-test-plus-2.2.2/README.md` & `django-test-plus-2.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 Let's face it, writing tests isn't always fun. Part of the reason for
 that is all of the boilerplate you end up writing. django-test-plus is
 an attempt to cut down on some of that when writing Django tests. We
 guarantee it will increase the time before you get carpal tunnel by at
 least 3 weeks!
 
+If you would like to get started testing your Django apps or improve how your
+team is testing we offer [TestStart](https://www.revsys.com/teststart/)
+to help your team dramatically improve your productivity.
+
 ## Support
 
 Supports: Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11.
 
 Supports Django Versions: 2.0, 2.1, 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, and 4.2.
 
 ## Documentation
@@ -59,15 +63,15 @@
 ```python
 from myproject.test import TestCase
 
 class MyViewTests(TestCase):
     ...
 ```
 
-This import, which is similar to the way you would import Django's TestCase, 
+This import, which is similar to the way you would import Django's TestCase,
 is also valid:
 
 ```python
 from test_plus import TestCase
 ```
 
 ## pytest Usage
@@ -228,15 +232,15 @@
     self.assert_http_200_ok(response)
 ```
 
 Django-test-plus provides a majority of the status codes assertions for you. The status assertions
 can be found in their own [mixin](https://github.com/revsys/django-test-plus/blob/main/test_plus/status_codes.py)
 and should be searchable if you're using an IDE like pycharm. It should be noted that in previous
 versions, django-test-plus had assertion methods in the pattern of `response_###()`, which are still
-available but have since been deprecated. See below for a list of those methods. 
+available but have since been deprecated. See below for a list of those methods.
 
 Each of the assertion methods takes an optional Django test client `response` and a string `msg` argument
 that, if specified, is used as the error message when a failure occurs. The methods,
 `assert_http_301_moved_permanently` and `assert_http_302_found` also take an optional `url` argument that
 if passed, will check to make sure the `response.url` matches.
 
 If it's available, the `assert_http_###_<status_name>` methods will use the last response. So you
@@ -246,30 +250,30 @@
 def test_status(self):
     self.get('my-url-name')
     self.assert_http_200_ok()
 ```
 
 Which is a bit shorter.
 
-The `response_###()` methods that are deprecated, but still available for use, include: 
+The `response_###()` methods that are deprecated, but still available for use, include:
 
 - `response_200()`
-- `response_201()` 
-- `response_204()` 
+- `response_201()`
+- `response_204()`
 - `response_301()`
-- `response_302()` 
+- `response_302()`
 - `response_400()`
-- `response_401()` 
+- `response_401()`
 - `response_403()`
-- `response_404()` 
+- `response_404()`
 - `response_405()`
 - `response_409()`
 - `response_410()`
 
-All of which take an optional Django test client response and a str msg argument that, if specified, is used as the error message when a failure occurs. Just like the `assert_http_###_<status_name>()` methods, these methods will use the last response if it's available. 
+All of which take an optional Django test client response and a str msg argument that, if specified, is used as the error message when a failure occurs. Just like the `assert_http_###_<status_name>()` methods, these methods will use the last response if it's available.
 
 ## `get_check_200(url_name, *args, **kwargs)`
 
 GETing and checking views return status 200 is a common test. This method makes it more convenient::
 
 ```python
 def test_even_better_status(self):
@@ -404,15 +408,15 @@
 ## Ensuring low query counts
 
 ### `assertNumQueriesLessThan(number)` - context
 
 Django provides
 [`assertNumQueries`](https://docs.djangoproject.com/en/1.8/topics/testing/tools/#django.test.TransactionTestCase.assertNumQueries)
 which is great when your code generates a specific number of
-queries. However, if this number varies due to the nature of your data, with 
+queries. However, if this number varies due to the nature of your data, with
 this method you can still test to ensure the code doesn't start producing a ton
 more queries than you expect:
 
 ```python
 def test_something_out(self):
 
     with self.assertNumQueriesLessThan(7):
@@ -601,9 +605,7 @@
 ## Keep in touch!
 
 If you have a question about this project, please open a GitHub issue. If you love us and want to keep track of our goings-on, here's where you can find us online:
 
 <a href="https://revsys.com?utm_medium=github&utm_source=django-test-plus"><img src="https://pbs.twimg.com/profile_images/915928618840285185/sUdRGIn1_400x400.jpg" height="50" /></a>
 <a href="https://twitter.com/revsys"><img src="https://cdn1.iconfinder.com/data/icons/new_twitter_icon/256/bird_twitter_new_simple.png" height="43" /></a>
 <a href="https://www.facebook.com/revsysllc/"><img src="https://cdn3.iconfinder.com/data/icons/picons-social/57/06-facebook-512.png" height="50" /></a>
-<a href="https://github.com/revsys/"><img src="https://assets-cdn.github.com/images/modules/logos_page/GitHub-Mark.png" height="53" /></a>
-<a href="https://gitlab.com/revsys"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/GitLab_Logo.svg/2000px-GitLab_Logo.svg.png" height="44" /></a>
```

### Comparing `django-test-plus-2.2.2/django_test_plus.egg-info/PKG-INFO` & `django-test-plus-2.2.3/django_test_plus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-test-plus
-Version: 2.2.2
+Version: 2.2.3
 Summary: "django-test-plus provides useful additions to Django's default TestCase"
 Home-page: https://github.com/revsys/django-test-plus/
 Author: Frank Wiles
 Author-email: frank@revsys.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -41,14 +41,18 @@
 
 Let's face it, writing tests isn't always fun. Part of the reason for
 that is all of the boilerplate you end up writing. django-test-plus is
 an attempt to cut down on some of that when writing Django tests. We
 guarantee it will increase the time before you get carpal tunnel by at
 least 3 weeks!
 
+If you would like to get started testing your Django apps or improve how your
+team is testing we offer [TestStart](https://www.revsys.com/teststart/)
+to help your team dramatically improve your productivity.
+
 ## Support
 
 Supports: Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11.
 
 Supports Django Versions: 2.0, 2.1, 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, and 4.2.
 
 ## Documentation
@@ -91,15 +95,15 @@
 ```python
 from myproject.test import TestCase
 
 class MyViewTests(TestCase):
     ...
 ```
 
-This import, which is similar to the way you would import Django's TestCase, 
+This import, which is similar to the way you would import Django's TestCase,
 is also valid:
 
 ```python
 from test_plus import TestCase
 ```
 
 ## pytest Usage
@@ -260,15 +264,15 @@
     self.assert_http_200_ok(response)
 ```
 
 Django-test-plus provides a majority of the status codes assertions for you. The status assertions
 can be found in their own [mixin](https://github.com/revsys/django-test-plus/blob/main/test_plus/status_codes.py)
 and should be searchable if you're using an IDE like pycharm. It should be noted that in previous
 versions, django-test-plus had assertion methods in the pattern of `response_###()`, which are still
-available but have since been deprecated. See below for a list of those methods. 
+available but have since been deprecated. See below for a list of those methods.
 
 Each of the assertion methods takes an optional Django test client `response` and a string `msg` argument
 that, if specified, is used as the error message when a failure occurs. The methods,
 `assert_http_301_moved_permanently` and `assert_http_302_found` also take an optional `url` argument that
 if passed, will check to make sure the `response.url` matches.
 
 If it's available, the `assert_http_###_<status_name>` methods will use the last response. So you
@@ -278,30 +282,30 @@
 def test_status(self):
     self.get('my-url-name')
     self.assert_http_200_ok()
 ```
 
 Which is a bit shorter.
 
-The `response_###()` methods that are deprecated, but still available for use, include: 
+The `response_###()` methods that are deprecated, but still available for use, include:
 
 - `response_200()`
-- `response_201()` 
-- `response_204()` 
+- `response_201()`
+- `response_204()`
 - `response_301()`
-- `response_302()` 
+- `response_302()`
 - `response_400()`
-- `response_401()` 
+- `response_401()`
 - `response_403()`
-- `response_404()` 
+- `response_404()`
 - `response_405()`
 - `response_409()`
 - `response_410()`
 
-All of which take an optional Django test client response and a str msg argument that, if specified, is used as the error message when a failure occurs. Just like the `assert_http_###_<status_name>()` methods, these methods will use the last response if it's available. 
+All of which take an optional Django test client response and a str msg argument that, if specified, is used as the error message when a failure occurs. Just like the `assert_http_###_<status_name>()` methods, these methods will use the last response if it's available.
 
 ## `get_check_200(url_name, *args, **kwargs)`
 
 GETing and checking views return status 200 is a common test. This method makes it more convenient::
 
 ```python
 def test_even_better_status(self):
@@ -436,15 +440,15 @@
 ## Ensuring low query counts
 
 ### `assertNumQueriesLessThan(number)` - context
 
 Django provides
 [`assertNumQueries`](https://docs.djangoproject.com/en/1.8/topics/testing/tools/#django.test.TransactionTestCase.assertNumQueries)
 which is great when your code generates a specific number of
-queries. However, if this number varies due to the nature of your data, with 
+queries. However, if this number varies due to the nature of your data, with
 this method you can still test to ensure the code doesn't start producing a ton
 more queries than you expect:
 
 ```python
 def test_something_out(self):
 
     with self.assertNumQueriesLessThan(7):
@@ -633,9 +637,7 @@
 ## Keep in touch!
 
 If you have a question about this project, please open a GitHub issue. If you love us and want to keep track of our goings-on, here's where you can find us online:
 
 <a href="https://revsys.com?utm_medium=github&utm_source=django-test-plus"><img src="https://pbs.twimg.com/profile_images/915928618840285185/sUdRGIn1_400x400.jpg" height="50" /></a>
 <a href="https://twitter.com/revsys"><img src="https://cdn1.iconfinder.com/data/icons/new_twitter_icon/256/bird_twitter_new_simple.png" height="43" /></a>
 <a href="https://www.facebook.com/revsysllc/"><img src="https://cdn3.iconfinder.com/data/icons/picons-social/57/06-facebook-512.png" height="50" /></a>
-<a href="https://github.com/revsys/"><img src="https://assets-cdn.github.com/images/modules/logos_page/GitHub-Mark.png" height="53" /></a>
-<a href="https://gitlab.com/revsys"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/GitLab_Logo.svg/2000px-GitLab_Logo.svg.png" height="44" /></a>
```

### Comparing `django-test-plus-2.2.2/setup.cfg` & `django-test-plus-2.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [bumpversion]
-current_version = 2.2.2
+current_version = 2.2.3
 commit = True
 tag = True
 
 [metadata]
 name = django-test-plus
-version = 2.2.2
+version = 2.2.3
 description = "django-test-plus provides useful additions to Django's default TestCase"
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Frank Wiles
 author_email = frank@revsys.com
 url = https://github.com/revsys/django-test-plus/
 classifiers =
```

### Comparing `django-test-plus-2.2.2/test_plus/compat.py` & `django-test-plus-2.2.3/test_plus/compat.py`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.2/test_plus/plugin.py` & `django-test-plus-2.2.3/test_plus/plugin.py`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.2/test_plus/runner.py` & `django-test-plus-2.2.3/test_plus/runner.py`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.2/test_plus/status_codes.py` & `django-test-plus-2.2.3/test_plus/status_codes.py`

 * *Files identical despite different names*

### Comparing `django-test-plus-2.2.2/test_plus/test.py` & `django-test-plus-2.2.3/test_plus/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,19 @@
             User = cls.user_factory._meta.model
             user_factory = cls.user_factory
         else:
             User = get_user_model()
             user_factory = User.objects.create_user
 
         USERNAME_FIELD = getattr(User, 'USERNAME_FIELD', 'username')
-        test_user = user_factory(**{USERNAME_FIELD: username})
+        user_data = {USERNAME_FIELD: username}
+        EMAIL_FIELD = getattr(User, 'EMAIL_FIELD', None)
+        if EMAIL_FIELD is not None and cls.user_factory is None:
+            user_data[EMAIL_FIELD] = '{}@example.com'.format(username)
+        test_user = user_factory(**user_data)
         test_user.set_password(password)
         test_user.save()
 
         if perms:
             from django.contrib.auth.models import Permission
             _filter = Q()
             for perm in perms:
```

