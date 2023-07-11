# Comparing `tmp/wagtail-cjk404-22.11.1.tar.gz` & `tmp/wagtail-cjk404-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cjk404-22.11.1.tar", last modified: Sat Nov 12 13:20:25 2022, max compression
+gzip compressed data, was "wagtail-cjk404-23.7.1.tar", last modified: Tue Jul 11 06:48:08 2023, max compression
```

## Comparing `wagtail-cjk404-22.11.1.tar` & `wagtail-cjk404-23.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2022-11-12 13:20:25.696238 wagtail-cjk404-22.11.1/
--rw-r--r--   0 grze      (1000) grze      (1000)     1542 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/LICENSE
--rw-r--r--   0 grze      (1000) grze      (1000)       59 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/MANIFEST.in
--rw-r--r--   0 grze      (1000) grze      (1000)     5443 2022-11-12 13:20:25.696238 wagtail-cjk404-22.11.1/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     4398 2022-11-12 12:54:14.000000 wagtail-cjk404-22.11.1/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2022-11-12 13:20:25.696238 wagtail-cjk404-22.11.1/cjk404/
--rw-r--r--   0 grze      (1000) grze      (1000)      316 2022-11-12 13:20:06.000000 wagtail-cjk404-22.11.1/cjk404/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      219 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/apps.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6701 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/middleware.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2022-11-12 13:20:25.696238 wagtail-cjk404-22.11.1/cjk404/migrations/
--rw-r--r--   0 grze      (1000) grze      (1000)     1391 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/migrations/0001_initial.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1968 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/migrations/0001_squashed_0006_auto_20211011_2219.py
--rw-r--r--   0 grze      (1000) grze      (1000)      442 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/migrations/0002_alter_pagenotfoundentry_id.py
--rw-r--r--   0 grze      (1000) grze      (1000)      680 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/migrations/0002_pagenotfoundentry_fallback_redirect.py
--rw-r--r--   0 grze      (1000) grze      (1000)      704 2022-11-12 13:16:18.000000 wagtail-cjk404-22.11.1/cjk404/migrations/0003_alter_pagenotfoundentry_redirect_to_url_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)      417 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/migrations/0003_pagenotfoundentry_regular_expression.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2007 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/migrations/0004_auto_20210830_1007.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1891 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/migrations/0005_auto_20211011_2131.py
--rw-r--r--   0 grze      (1000) grze      (1000)      820 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/migrations/0006_auto_20211011_2219.py
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/migrations/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2619 2022-11-12 12:32:50.000000 wagtail-cjk404-22.11.1/cjk404/models.py
--rw-r--r--   0 grze      (1000) grze      (1000)     7283 2022-09-04 08:40:52.000000 wagtail-cjk404-22.11.1/cjk404/tests.py
--rw-r--r--   0 grze      (1000) grze      (1000)      434 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/testsettings.py
--rw-r--r--   0 grze      (1000) grze      (1000)      802 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/cjk404/wagtail_hooks.py
--rw-r--r--   0 grze      (1000) grze      (1000)       93 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/pyproject.toml
--rw-r--r--   0 grze      (1000) grze      (1000)     1080 2022-11-12 13:20:25.696238 wagtail-cjk404-22.11.1/setup.cfg
--rw-r--r--   0 grze      (1000) grze      (1000)       38 2022-09-01 08:26:10.000000 wagtail-cjk404-22.11.1/setup.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2022-11-12 13:20:25.696238 wagtail-cjk404-22.11.1/wagtail_cjk404.egg-info/
--rw-r--r--   0 grze      (1000) grze      (1000)     5443 2022-11-12 13:20:25.000000 wagtail-cjk404-22.11.1/wagtail_cjk404.egg-info/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)      898 2022-11-12 13:20:25.000000 wagtail-cjk404-22.11.1/wagtail_cjk404.egg-info/SOURCES.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        1 2022-11-12 13:20:25.000000 wagtail-cjk404-22.11.1/wagtail_cjk404.egg-info/dependency_links.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       16 2022-11-12 13:20:25.000000 wagtail-cjk404-22.11.1/wagtail_cjk404.egg-info/requires.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        7 2022-11-12 13:20:25.000000 wagtail-cjk404-22.11.1/wagtail_cjk404.egg-info/top_level.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/LICENSE
+-rw-r--r--   0 grze      (1000) grze      (1000)       59 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/MANIFEST.in
+-rw-r--r--   0 grze      (1000) grze      (1000)     5477 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     4433 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/cjk404/
+-rw-r--r--   0 grze      (1000) grze      (1000)      315 2023-07-11 06:47:53.000000 wagtail-cjk404-23.7.1/cjk404/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      219 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/apps.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6696 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/middleware.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/cjk404/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1391 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1968 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0001_squashed_0006_auto_20211011_2219.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      442 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0002_alter_pagenotfoundentry_id.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      680 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0002_pagenotfoundentry_fallback_redirect.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      704 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0003_alter_pagenotfoundentry_redirect_to_url_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      417 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0003_pagenotfoundentry_regular_expression.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2007 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0004_auto_20210830_1007.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1891 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0005_auto_20211011_2131.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      820 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/0006_auto_20211011_2219.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/migrations/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2607 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     7278 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/tests.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      434 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/testsettings.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      802 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/cjk404/wagtail_hooks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)       93 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/pyproject.toml
+-rw-r--r--   0 grze      (1000) grze      (1000)     1079 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/setup.cfg
+-rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-07-11 06:46:54.000000 wagtail-cjk404-23.7.1/setup.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-11 06:48:08.394096 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/
+-rw-r--r--   0 grze      (1000) grze      (1000)     5477 2023-07-11 06:48:08.000000 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)      898 2023-07-11 06:48:08.000000 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/SOURCES.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-07-11 06:48:08.000000 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/dependency_links.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       15 2023-07-11 06:48:08.000000 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/requires.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-07-11 06:48:08.000000 wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/top_level.txt
```

### Comparing `wagtail-cjk404-22.11.1/LICENSE` & `wagtail-cjk404-23.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-22.11.1/PKG-INFO` & `wagtail-cjk404-23.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjk404
-Version: 22.11.1
+Version: 23.7.1
 Summary: A Wagtail app to automatically log and/or manually create of redirects for 404 pages from within Wagtail admin panel.
 Home-page: https://github.com/cjkpl/wagtail-cjk404
 Author: Grzegorz Krol, Filip Wozniak
 Author-email: gk@cjk.pl, fw@cjk.pl
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -71,20 +71,20 @@
 - wagtail.contrib.modeladmin (https://docs.wagtail.io/en/stable/reference/contrib/modeladmin/index.html)
 
 This package is used for the admin panel itself.
 
 ## Screenshots
 
 #### "All Redirects" in the Backend
+!["All Redirects" in the Backend"](https://user-images.githubusercontent.com/34211633/236237989-3c396246-53ee-4d57-91cf-31b9333fb47a.png)
 
-!["All Redirects" in the Backend"](https://raw.githubusercontent.com/cjkpl/wagtail-cjk404/main/docs/All%20Redirects.jpg)
 
 #### "Edit Redirect" in the Backend 
+!["Edit Redirect" in the Backend"](https://user-images.githubusercontent.com/34211633/236238437-33c856ca-592b-4235-9d15-5c1953d0ade3.png)
 
-!["Edit Redirect" in the Backend](https://raw.githubusercontent.com/cjkpl/wagtail-cjk404/main/docs/Edit%20Redirect.jpg)
 
 ### Usage
 
 #### Fresh install
 
 1. Get the app from PyPI:
 ```pip install wagtail-cjk404```
```

### Comparing `wagtail-cjk404-22.11.1/README.md` & `wagtail-cjk404-23.7.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 - wagtail.contrib.modeladmin (https://docs.wagtail.io/en/stable/reference/contrib/modeladmin/index.html)
 
 This package is used for the admin panel itself.
 
 ## Screenshots
 
 #### "All Redirects" in the Backend
+!["All Redirects" in the Backend"](https://user-images.githubusercontent.com/34211633/236237989-3c396246-53ee-4d57-91cf-31b9333fb47a.png)
 
-!["All Redirects" in the Backend"](https://raw.githubusercontent.com/cjkpl/wagtail-cjk404/main/docs/All%20Redirects.jpg)
 
 #### "Edit Redirect" in the Backend 
+!["Edit Redirect" in the Backend"](https://user-images.githubusercontent.com/34211633/236238437-33c856ca-592b-4235-9d15-5c1953d0ade3.png)
 
-!["Edit Redirect" in the Backend](https://raw.githubusercontent.com/cjkpl/wagtail-cjk404/main/docs/Edit%20Redirect.jpg)
 
 ### Usage
 
 #### Fresh install
 
 1. Get the app from PyPI:
 ```pip install wagtail-cjk404```
```

### Comparing `wagtail-cjk404-22.11.1/cjk404/middleware.py` & `wagtail-cjk404-23.7.1/cjk404/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.conf import settings
 from django.core.cache import cache
 from django.core.exceptions import ImproperlyConfigured
 from django.http import HttpResponsePermanentRedirect, HttpResponseRedirect
 from django.utils.timezone import now
 
 from .models import PageNotFoundEntry
-from wagtail.core.models import Site
+from wagtail.models import Site
 
 IGNORED_404S = getattr(settings, "IGNORED_404S", [r"^/static/", r"^/favicon.ico"])
 
 DJANGO_REGEX_REDIRECTS_CACHE_KEY = "django-regex-redirects-regular"
 DJANGO_REGEX_REDIRECTS_CACHE_REGEX_KEY = "django-regex-redirects-regex"
 DJANGO_REGEX_REDIRECTS_CACHE_TIMEOUT = 60
```

### Comparing `wagtail-cjk404-22.11.1/cjk404/migrations/0001_initial.py` & `wagtail-cjk404-23.7.1/cjk404/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-22.11.1/cjk404/migrations/0001_squashed_0006_auto_20211011_2219.py` & `wagtail-cjk404-23.7.1/cjk404/migrations/0001_squashed_0006_auto_20211011_2219.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-22.11.1/cjk404/migrations/0002_pagenotfoundentry_fallback_redirect.py` & `wagtail-cjk404-23.7.1/cjk404/migrations/0002_pagenotfoundentry_fallback_redirect.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-22.11.1/cjk404/migrations/0003_alter_pagenotfoundentry_redirect_to_url_and_more.py` & `wagtail-cjk404-23.7.1/cjk404/migrations/0003_alter_pagenotfoundentry_redirect_to_url_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-22.11.1/cjk404/migrations/0004_auto_20210830_1007.py` & `wagtail-cjk404-23.7.1/cjk404/migrations/0004_auto_20210830_1007.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-22.11.1/cjk404/migrations/0005_auto_20211011_2131.py` & `wagtail-cjk404-23.7.1/cjk404/migrations/0005_auto_20211011_2131.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-22.11.1/cjk404/migrations/0006_auto_20211011_2219.py` & `wagtail-cjk404-23.7.1/cjk404/migrations/0006_auto_20211011_2219.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-22.11.1/cjk404/models.py` & `wagtail-cjk404-23.7.1/cjk404/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db import models
-from wagtail.admin.edit_handlers import FieldPanel, MultiFieldPanel, PageChooserPanel
-from wagtail.core.models import Page, Site
+from wagtail.admin.panels import FieldPanel, MultiFieldPanel, PageChooserPanel
+from wagtail.models import Page, Site
 
 
 class PageNotFoundEntry(models.Model):
     site = models.ForeignKey(
         Site,
         related_name="pagenotfound_entries",
         on_delete=models.CASCADE,
```

### Comparing `wagtail-cjk404-22.11.1/cjk404/tests.py` & `wagtail-cjk404-23.7.1/cjk404/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest.case import skipUnless
 
 from django.conf import settings
 from django.test import TestCase
 from django.test.utils import override_settings
 from django.core.cache import cache
-from wagtail.core.models import Site, Page
+from wagtail.models import Site, Page
 from typing import Union, Optional
 
 from cjk404.middleware import (
     DJANGO_REGEX_REDIRECTS_CACHE_KEY,
     DJANGO_REGEX_REDIRECTS_CACHE_REGEX_KEY,
 )
 from cjk404.models import PageNotFoundEntry
```

### Comparing `wagtail-cjk404-22.11.1/cjk404/wagtail_hooks.py` & `wagtail-cjk404-23.7.1/cjk404/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjk404-22.11.1/setup.cfg` & `wagtail-cjk404-23.7.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 	Topic :: Internet :: WWW/HTTP :: Site Management
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	Wagtail >= 2.16.2
+	Wagtail >= 4.0.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wagtail-cjk404-22.11.1/wagtail_cjk404.egg-info/PKG-INFO` & `wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjk404
-Version: 22.11.1
+Version: 23.7.1
 Summary: A Wagtail app to automatically log and/or manually create of redirects for 404 pages from within Wagtail admin panel.
 Home-page: https://github.com/cjkpl/wagtail-cjk404
 Author: Grzegorz Krol, Filip Wozniak
 Author-email: gk@cjk.pl, fw@cjk.pl
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -71,20 +71,20 @@
 - wagtail.contrib.modeladmin (https://docs.wagtail.io/en/stable/reference/contrib/modeladmin/index.html)
 
 This package is used for the admin panel itself.
 
 ## Screenshots
 
 #### "All Redirects" in the Backend
+!["All Redirects" in the Backend"](https://user-images.githubusercontent.com/34211633/236237989-3c396246-53ee-4d57-91cf-31b9333fb47a.png)
 
-!["All Redirects" in the Backend"](https://raw.githubusercontent.com/cjkpl/wagtail-cjk404/main/docs/All%20Redirects.jpg)
 
 #### "Edit Redirect" in the Backend 
+!["Edit Redirect" in the Backend"](https://user-images.githubusercontent.com/34211633/236238437-33c856ca-592b-4235-9d15-5c1953d0ade3.png)
 
-!["Edit Redirect" in the Backend](https://raw.githubusercontent.com/cjkpl/wagtail-cjk404/main/docs/Edit%20Redirect.jpg)
 
 ### Usage
 
 #### Fresh install
 
 1. Get the app from PyPI:
 ```pip install wagtail-cjk404```
```

### Comparing `wagtail-cjk404-22.11.1/wagtail_cjk404.egg-info/SOURCES.txt` & `wagtail-cjk404-23.7.1/wagtail_cjk404.egg-info/SOURCES.txt`

 * *Files identical despite different names*

