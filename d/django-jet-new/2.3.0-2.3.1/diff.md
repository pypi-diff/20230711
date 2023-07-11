# Comparing `tmp/django-jet-new-2.3.0.tar.gz` & `tmp/django-jet-new-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-jet-new-2.3.0.tar", last modified: Tue Jul 11 00:23:49 2023, max compression
+gzip compressed data, was "django-jet-new-2.3.1.tar", last modified: Tue Jul 11 00:48:52 2023, max compression
```

## Comparing `django-jet-new-2.3.0.tar` & `django-jet-new-2.3.1.tar`

### file list

```diff
@@ -1,564 +1,564 @@
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.757026 django-jet-new-2.3.0/
--rw-r--r--   0 munisisazade   (501) staff       (20)    34520 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/LICENSE
--rw-r--r--   0 munisisazade   (501) staff       (20)      257 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/MANIFEST.in
--rw-r--r--   0 munisisazade   (501) staff       (20)     8014 2023-07-11 00:23:49.756860 django-jet-new-2.3.0/PKG-INFO
--rw-r--r--   0 munisisazade   (501) staff       (20)     6613 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/README.rst
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.668010 django-jet-new-2.3.0/django_jet_new.egg-info/
--rw-r--r--   0 munisisazade   (501) staff       (20)     8014 2023-07-11 00:23:49.000000 django-jet-new-2.3.0/django_jet_new.egg-info/PKG-INFO
--rw-r--r--   0 munisisazade   (501) staff       (20)    20881 2023-07-11 00:23:49.000000 django-jet-new-2.3.0/django_jet_new.egg-info/SOURCES.txt
--rw-r--r--   0 munisisazade   (501) staff       (20)        1 2023-07-11 00:23:49.000000 django-jet-new-2.3.0/django_jet_new.egg-info/dependency_links.txt
--rw-r--r--   0 munisisazade   (501) staff       (20)        1 2023-07-11 00:23:49.000000 django-jet-new-2.3.0/django_jet_new.egg-info/not-zip-safe
--rw-r--r--   0 munisisazade   (501) staff       (20)        7 2023-07-11 00:23:49.000000 django-jet-new-2.3.0/django_jet_new.egg-info/requires.txt
--rw-r--r--   0 munisisazade   (501) staff       (20)        4 2023-07-11 00:23:49.000000 django-jet-new-2.3.0/django_jet_new.egg-info/top_level.txt
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.670086 django-jet-new-2.3.0/jet/
--rw-r--r--   0 munisisazade   (501) staff       (20)       18 2023-07-11 00:23:22.000000 django-jet-new-2.3.0/jet/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      136 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/admin.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.672219 django-jet-new-2.3.0/jet/dashboard/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     9833 2023-07-11 00:15:37.000000 django-jet-new-2.3.0/jet/dashboard/dashboard.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.673330 django-jet-new-2.3.0/jet/dashboard/dashboard_modules/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/dashboard_modules/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)    15761 2023-07-11 00:15:37.000000 django-jet-new-2.3.0/jet/dashboard/dashboard_modules/google_analytics.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2423 2023-07-11 00:15:37.000000 django-jet-new-2.3.0/jet/dashboard/dashboard_modules/google_analytics_views.py
--rw-r--r--   0 munisisazade   (501) staff       (20)    13642 2023-07-11 00:15:37.000000 django-jet-new-2.3.0/jet/dashboard/dashboard_modules/yandex_metrika.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2142 2023-07-11 00:15:37.000000 django-jet-new-2.3.0/jet/dashboard/dashboard_modules/yandex_metrika_views.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     5577 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/forms.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.660675 django-jet-new-2.3.0/jet/dashboard/locale/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.659518 django-jet-new-2.3.0/jet/dashboard/locale/ar/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.674223 django-jet-new-2.3.0/jet/dashboard/locale/ar/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     6102 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    13370 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      473 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      852 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.659633 django-jet-new-2.3.0/jet/dashboard/locale/cs/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.674815 django-jet-new-2.3.0/jet/dashboard/locale/cs/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     4470 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    12226 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      471 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      843 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.659752 django-jet-new-2.3.0/jet/dashboard/locale/de/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.675361 django-jet-new-2.3.0/jet/dashboard/locale/de/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     4947 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     6200 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      393 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      842 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.659870 django-jet-new-2.3.0/jet/dashboard/locale/en/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.676025 django-jet-new-2.3.0/jet/dashboard/locale/en/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)      495 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    10871 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      378 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      827 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.659992 django-jet-new-2.3.0/jet/dashboard/locale/es/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.676560 django-jet-new-2.3.0/jet/dashboard/locale/es/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     6524 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    15268 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      474 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      846 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.660105 django-jet-new-2.3.0/jet/dashboard/locale/fa/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.676823 django-jet-new-2.3.0/jet/dashboard/locale/fa/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)    16058 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      851 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/fa/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.660219 django-jet-new-2.3.0/jet/dashboard/locale/fr/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.677104 django-jet-new-2.3.0/jet/dashboard/locale/fr/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)    12295 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      845 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.660331 django-jet-new-2.3.0/jet/dashboard/locale/pl/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.677393 django-jet-new-2.3.0/jet/dashboard/locale/pl/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     4327 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    14998 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.660466 django-jet-new-2.3.0/jet/dashboard/locale/pt-br/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.678132 django-jet-new-2.3.0/jet/dashboard/locale/pt-br/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     5245 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/pt-br/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    12513 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/pt-br/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      499 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      871 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.660600 django-jet-new-2.3.0/jet/dashboard/locale/ru/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.678755 django-jet-new-2.3.0/jet/dashboard/locale/ru/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     6409 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    13673 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      485 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      857 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.660724 django-jet-new-2.3.0/jet/dashboard/locale/zh_cn/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.679038 django-jet-new-2.3.0/jet/dashboard/locale/zh_cn/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     3891 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    12159 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.679333 django-jet-new-2.3.0/jet/dashboard/migrations/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1445 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/migrations/0001_initial.py
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/migrations/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2061 2023-07-11 00:15:37.000000 django-jet-new-2.3.0/jet/dashboard/models.py
--rw-r--r--   0 munisisazade   (501) staff       (20)    19375 2023-07-11 00:15:37.000000 django-jet-new-2.3.0/jet/dashboard/modules.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      280 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/settings.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.679565 django-jet-new-2.3.0/jet/dashboard/south_migrations/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2561 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/south_migrations/0001_initial.py
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/south_migrations/__init__.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.661043 django-jet-new-2.3.0/jet/dashboard/static/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.661169 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.679807 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/dashboard_modules/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2424 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/dashboard_modules/google_analytics.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     2422 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/dashboard_modules/yandex_metrika.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.661217 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.681033 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     2991 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/CONTRIBUTING.md
--rwxr-xr-x   0 munisisazade   (501) staff       (20)   109612 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.js
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    52091 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.min.js
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     1060 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/LICENSE.md
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     1144 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/README.md
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.661407 django-jet-new-2.3.0/jet/dashboard/templates/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.681326 django-jet-new-2.3.0/jet/dashboard/templates/admin/
--rw-r--r--   0 munisisazade   (501) staff       (20)      949 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/admin/app_index.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      938 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/admin/index.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.682048 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1411 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/dashboard.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     2060 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/dashboard_tools.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     2163 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/module.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.683531 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1473 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/app_list.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      587 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/feed.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     1056 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/google_analytics_period_visitors.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     1099 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_chart.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      597 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_totals.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      922 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/link_list.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      804 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/model_list.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     1667 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/recent_actions.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     1050 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_period_visitors.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     1097 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_chart.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      597 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_totals.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     4140 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/update_module.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      950 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/update_module_fieldset.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.683756 django-jet-new-2.3.0/jet/dashboard/templatetags/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templatetags/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      738 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/templatetags/jet_dashboard_tags.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1694 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/urls.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      562 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/dashboard/utils.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     8113 2023-07-11 00:15:37.000000 django-jet-new-2.3.0/jet/dashboard/views.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     3084 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/filters.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     5221 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/forms.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.662779 django-jet-new-2.3.0/jet/locale/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.661708 django-jet-new-2.3.0/jet/locale/ar/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.684432 django-jet-new-2.3.0/jet/locale/ar/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1242 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1877 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      739 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1389 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.661821 django-jet-new-2.3.0/jet/locale/cs/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.685008 django-jet-new-2.3.0/jet/locale/cs/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1148 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1779 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      703 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1343 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.661931 django-jet-new-2.3.0/jet/locale/de/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.685630 django-jet-new-2.3.0/jet/locale/de/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1418 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1867 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      622 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1347 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.662040 django-jet-new-2.3.0/jet/locale/en/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.686200 django-jet-new-2.3.0/jet/locale/en/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)      495 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1592 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      378 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1253 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.662152 django-jet-new-2.3.0/jet/locale/es/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.686797 django-jet-new-2.3.0/jet/locale/es/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1770 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     2860 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      724 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.662260 django-jet-new-2.3.0/jet/locale/fa/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.687094 django-jet-new-2.3.0/jet/locale/fa/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     3933 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)     1401 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/fa/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.662366 django-jet-new-2.3.0/jet/locale/fr/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.687483 django-jet-new-2.3.0/jet/locale/fr/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1770 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)     1379 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.662475 django-jet-new-2.3.0/jet/locale/pl/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.688130 django-jet-new-2.3.0/jet/locale/pl/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1926 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     3852 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      479 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      751 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.662595 django-jet-new-2.3.0/jet/locale/pt_BR/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.688857 django-jet-new-2.3.0/jet/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1197 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1828 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      761 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1401 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.662713 django-jet-new-2.3.0/jet/locale/ru/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.689561 django-jet-new-2.3.0/jet/locale/ru/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1305 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1936 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      787 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1427 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.662837 django-jet-new-2.3.0/jet/locale/zh_CN/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.689934 django-jet-new-2.3.0/jet/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2005 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     3729 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.690094 django-jet-new-2.3.0/jet/management/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/management/__init__.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.690506 django-jet-new-2.3.0/jet/management/commands/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/management/commands/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1430 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/management/commands/jet_custom_apps_example.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1509 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/management/commands/jet_side_menu_items_example.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.690976 django-jet-new-2.3.0/jet/migrations/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2930 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/migrations/0001_initial.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      317 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/migrations/0002_delete_userdashboardmodule.py
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/migrations/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1210 2023-07-11 00:15:37.000000 django-jet-new-2.3.0/jet/models.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1648 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/ordered_set.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      509 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/settings.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.691436 django-jet-new-2.3.0/jet/south_migrations/
--rw-r--r--   0 munisisazade   (501) staff       (20)     4874 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/south_migrations/0001_initial.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2532 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/south_migrations/0002_auto__del_userdashboardmodule.py
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/south_migrations/__init__.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.665571 django-jet-new-2.3.0/jet/static/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.663417 django-jet-new-2.3.0/jet/static/admin/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.692336 django-jet-new-2.3.0/jet/static/admin/css/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/css/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/css/changelists.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/css/dashboard.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/css/fonts.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/css/forms.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/css/login.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/css/rtl.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/css/widgets.css
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.692625 django-jet-new-2.3.0/jet/static/admin/js/
--rw-r--r--   0 munisisazade   (501) staff       (20)       85 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/js/SelectFilter2.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.692852 django-jet-new-2.3.0/jet/static/admin/js/admin/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/js/admin/DateTimeShortcuts.js
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/js/admin/RelatedObjectLookups.js
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/admin/js/related-widget-wrapper.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.664769 django-jet-new-2.3.0/jet/static/jet/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.696221 django-jet-new-2.3.0/jet/static/jet/css/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2211 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_base.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)      880 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_breadcrumbs.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)    17750 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_changeform.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     7749 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_changelist.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     4029 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_content.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     8804 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_dashboard.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     1783 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_delete-confirmation.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     3534 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_forms.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)       67 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_globals.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     5165 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_header.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     4119 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_helpers.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     1959 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_login.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     1656 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_messages.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)      740 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_modules.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     1042 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_object-tools.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     2051 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_relatedpopup.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)    11150 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_sidebar.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     3249 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_tables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     6284 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/_variables.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.696957 django-jet-new-2.3.0/jet/static/jet/css/icons/
--rwxr-xr-x   0 munisisazade   (501) staff       (20)      800 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/icons/_variables.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.697721 django-jet-new-2.3.0/jet/static/jet/css/icons/fonts/
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6412 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/icons/fonts/jet-icons.eot
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    19664 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/icons/fonts/jet-icons.svg
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6240 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/icons/fonts/jet-icons.ttf
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6316 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/icons/fonts/jet-icons.woff
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     2248 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/icons/style.css
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.697885 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     3192 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/_jquery-ui.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.700095 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/
--rw-r--r--   0 munisisazade   (501) staff       (20)      180 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      178 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-bg_flat_75_ffffff_40x100.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      120 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      105 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      111 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      110 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      119 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      101 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-icons_222222_256x240.png
--rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-icons_454545_256x240.png
--rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-icons_888888_256x240.png
--rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-icons_cd0a0a_256x240.png
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.700597 django-jet-new-2.3.0/jet/static/jet/css/select2/
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     3095 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/select2/_layout.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     1662 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/select2/_multiple.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)      937 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/select2/_single.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.664677 django-jet-new-2.3.0/jet/static/jet/css/themes/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.703507 django-jet-new-2.3.0/jet/static/jet/css/themes/default/
--rw-r--r--   0 munisisazade   (501) staff       (20)       66 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/default/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178918 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/default/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   303057 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/default/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/default/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6760 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/default/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    23121 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/default/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/default/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23574 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/default/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    44244 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/default/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/default/select2.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.706273 django-jet-new-2.3.0/jet/static/jet/css/themes/green/
--rw-r--r--   0 munisisazade   (501) staff       (20)     4956 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/green/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178918 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/green/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   308261 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/green/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/green/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6760 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/green/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    21794 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/green/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/green/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23574 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/green/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    49427 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/green/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/green/select2.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.709390 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/
--rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178850 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   308602 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    22166 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23571 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    49792 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/select2.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.713644 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/
--rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178844 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   308599 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    22166 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23569 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    49791 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/select2.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.720563 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/
--rw-r--r--   0 munisisazade   (501) staff       (20)     5318 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178844 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   308610 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    22177 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23569 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    49802 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/select2.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.725616 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/
--rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178805 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   308556 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    22172 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23573 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    49799 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/select2.theme.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)    53889 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/css/vendor.css
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.665206 django-jet-new-2.3.0/jet/static/jet/js/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.725759 django-jet-new-2.3.0/jet/static/jet/js/build/
--rw-r--r--   0 munisisazade   (501) staff       (20)   417084 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/build/bundle.min.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.665133 django-jet-new-2.3.0/jet/static/jet/js/i18n/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.738036 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1144 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-af.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1458 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ar-DZ.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1458 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ar.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1168 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-az.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1394 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-be.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1371 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-bg.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1092 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-bs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1122 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ca.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1171 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-cs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1155 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-cy-GB.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-da.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1129 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-de.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1436 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-el.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1148 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-en-AU.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1125 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-en-GB.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1150 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-en-NZ.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1141 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-eo.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1136 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-es.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1199 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-et.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1091 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-eu.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1382 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fa.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1193 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1166 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fo.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1161 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CA.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1208 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CH.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1289 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-gl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1264 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-he.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1561 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-hi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-hr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1140 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-hu.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1422 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-hy.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1130 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-id.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1194 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-is.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1169 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-it-CH.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1160 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-it.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1150 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ja.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1664 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ka.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-kk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1578 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-km.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1159 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ko.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1356 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ky.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1182 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-lb.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1209 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-lt.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1190 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-lv.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1305 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-mk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1684 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ml.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1139 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ms.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1145 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-nb.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1169 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-nl-BE.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1167 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-nl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1142 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-nn.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1137 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-no.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1165 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-pl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1196 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-pt-BR.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1116 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-pt.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1155 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-rm.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1237 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ro.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ru.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1153 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1191 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1135 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sq.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1099 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sr-SR.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1285 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sv.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1744 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ta.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1522 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-th.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1322 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-tj.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1131 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-tr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1431 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-uk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1342 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-vi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1234 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-CN.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1232 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-HK.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1228 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-TW.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.740482 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/
--rw-r--r--   0 munisisazade   (501) staff       (20)      480 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-cs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      462 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-de.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      493 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-es.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      550 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-fr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      503 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-hr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      458 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-hu.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      485 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-it.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      500 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ja.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      510 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-mk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      424 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-nl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      457 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-pl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      480 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-pt-BR.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      520 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ru.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      492 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-sl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      468 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-sv.js
--rwxr-xr-x   0 munisisazade   (501) staff       (20)      503 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-tr.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.747228 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/
--rw-r--r--   0 munisisazade   (501) staff       (20)      701 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/az.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      906 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/bg.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      876 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/ca.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1236 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/cs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      816 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/da.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      775 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/de.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      827 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/en.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      871 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/es.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      775 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/et.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      844 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/eu.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1004 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/fa.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      703 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/fi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      823 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/fr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      800 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/gl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      894 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/he.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1125 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/hi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      780 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/hr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      727 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/hu.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      693 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/id.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      773 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/is.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      876 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/it.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      854 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/ko.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      878 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/lt.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      872 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/lv.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      979 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/mk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      723 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/nb.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      867 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/nl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      926 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/pl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      853 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/pt-BR.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      859 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/pt.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      834 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/ro.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1127 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/ru.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1184 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/sk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      880 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/sr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      786 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/sv.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      948 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/th.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      720 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/tr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/uk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      801 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/vi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      769 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/zh-CN.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      708 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/zh-TW.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.747414 django-jet-new-2.3.0/jet/static/jet/js/src/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.750642 django-jet-new-2.3.0/jet/static/jet/js/src/features/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2852 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/changeform-tabs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1354 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/changeform.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     3803 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/changelist.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/checkboxes.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     6694 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/compact-inline.js
--rw-r--r--   0 munisisazade   (501) staff       (20)    11563 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/dashboard.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     4309 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/date-time-widgets.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     2350 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/filters.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      895 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/inlines.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     8343 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/related-popups.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      824 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/scroll-to-bottom-detector.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     8381 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/selects.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      575 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/siblings.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.751216 django-jet-new-2.3.0/jet/static/jet/js/src/features/sidebar/
--rw-r--r--   0 munisisazade   (501) staff       (20)     3652 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/sidebar/application-pinning.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     4219 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/sidebar/bookmarks.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     3391 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/sidebar/main.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     7484 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/sidebar/popup.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1952 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/themes.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      709 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/tooltips.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      986 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/features/touchmove-non-scrollable.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.753107 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1529 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/actions.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      746 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/branding.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1050 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/breadcrumbs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     2552 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/changeform-tabs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      449 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/delete-confirmation.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      730 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/icons.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      367 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/object-tools.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     2635 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/paginator.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1187 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/related-widget-wrapper.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      857 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/stacked-inline.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1226 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/tabular-inline.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     4842 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/toolbar.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1445 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/user-tools.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1199 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/main.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.753698 django-jet-new-2.3.0/jet/static/jet/js/src/utils/
--rw-r--r--   0 munisisazade   (501) staff       (20)      206 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/utils/jquery-icontains.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      178 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/utils/jquery-slidefade.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      132 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/utils/translate.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      779 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/jet/js/src/utils/window-storage.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.665625 django-jet-new-2.3.0/jet/static/range_filter/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.753835 django-jet-new-2.3.0/jet/static/range_filter/css/
--rw-r--r--   0 munisisazade   (501) staff       (20)      244 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/static/range_filter/css/style.css
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.666115 django-jet-new-2.3.0/jet/templates/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.754162 django-jet-new-2.3.0/jet/templates/admin/
--rw-r--r--   0 munisisazade   (501) staff       (20)    21995 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/templates/admin/base.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.754299 django-jet-new-2.3.0/jet/templates/admin/edit_inline/
--rw-r--r--   0 munisisazade   (501) staff       (20)     3630 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/templates/admin/edit_inline/compact.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.754429 django-jet-new-2.3.0/jet/templates/admin/includes/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1808 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/templates/admin/includes/fieldset.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      379 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/templates/admin/popup_response.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.754566 django-jet-new-2.3.0/jet/templates/jet/
--rw-r--r--   0 munisisazade   (501) staff       (20)      450 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/templates/jet/related_field_ajax_list_filter.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.754697 django-jet-new-2.3.0/jet/templates/rangefilter/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1940 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/templates/rangefilter/date_filter.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.754921 django-jet-new-2.3.0/jet/templatetags/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/templatetags/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     7761 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/templatetags/jet_tags.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:23:49.756583 django-jet-new-2.3.0/jet/tests/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      347 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/admin.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1735 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/dashboard.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      806 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/models.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1945 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/settings.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     3085 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/test_dashboard.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2230 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/test_filters.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2003 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/test_ordered_set.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     3711 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/test_tags.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2371 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/test_utils.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     8951 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/test_views.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      858 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/tests/urls.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1030 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/urls.py
--rw-r--r--   0 munisisazade   (501) staff       (20)    16158 2023-07-11 00:15:37.000000 django-jet-new-2.3.0/jet/utils.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1698 2023-07-11 00:08:01.000000 django-jet-new-2.3.0/jet/views.py
--rw-r--r--   0 munisisazade   (501) staff       (20)       38 2023-07-11 00:23:49.757065 django-jet-new-2.3.0/setup.cfg
--rw-r--r--   0 munisisazade   (501) staff       (20)     2170 2023-07-11 00:23:06.000000 django-jet-new-2.3.0/setup.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.667862 django-jet-new-2.3.1/
+-rw-r--r--   0 munisisazade   (501) staff       (20)    34520 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/LICENSE
+-rw-r--r--   0 munisisazade   (501) staff       (20)      257 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/MANIFEST.in
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8014 2023-07-11 00:48:52.667200 django-jet-new-2.3.1/PKG-INFO
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6613 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/README.rst
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.558297 django-jet-new-2.3.1/django_jet_new.egg-info/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8014 2023-07-11 00:48:52.000000 django-jet-new-2.3.1/django_jet_new.egg-info/PKG-INFO
+-rw-r--r--   0 munisisazade   (501) staff       (20)    20881 2023-07-11 00:48:52.000000 django-jet-new-2.3.1/django_jet_new.egg-info/SOURCES.txt
+-rw-r--r--   0 munisisazade   (501) staff       (20)        1 2023-07-11 00:48:52.000000 django-jet-new-2.3.1/django_jet_new.egg-info/dependency_links.txt
+-rw-r--r--   0 munisisazade   (501) staff       (20)        1 2023-07-11 00:48:52.000000 django-jet-new-2.3.1/django_jet_new.egg-info/not-zip-safe
+-rw-r--r--   0 munisisazade   (501) staff       (20)        7 2023-07-11 00:48:52.000000 django-jet-new-2.3.1/django_jet_new.egg-info/requires.txt
+-rw-r--r--   0 munisisazade   (501) staff       (20)        4 2023-07-11 00:48:52.000000 django-jet-new-2.3.1/django_jet_new.egg-info/top_level.txt
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.562466 django-jet-new-2.3.1/jet/
+-rw-r--r--   0 munisisazade   (501) staff       (20)       18 2023-07-11 00:48:15.000000 django-jet-new-2.3.1/jet/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      136 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/admin.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.567668 django-jet-new-2.3.1/jet/dashboard/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     9833 2023-07-11 00:15:37.000000 django-jet-new-2.3.1/jet/dashboard/dashboard.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.569399 django-jet-new-2.3.1/jet/dashboard/dashboard_modules/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/dashboard_modules/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)    15759 2023-07-11 00:44:55.000000 django-jet-new-2.3.1/jet/dashboard/dashboard_modules/google_analytics.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2423 2023-07-11 00:15:37.000000 django-jet-new-2.3.1/jet/dashboard/dashboard_modules/google_analytics_views.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)    13641 2023-07-11 00:44:55.000000 django-jet-new-2.3.1/jet/dashboard/dashboard_modules/yandex_metrika.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2142 2023-07-11 00:15:37.000000 django-jet-new-2.3.1/jet/dashboard/dashboard_modules/yandex_metrika_views.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5577 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/forms.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.551169 django-jet-new-2.3.1/jet/dashboard/locale/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.550080 django-jet-new-2.3.1/jet/dashboard/locale/ar/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.572408 django-jet-new-2.3.1/jet/dashboard/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6102 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)    13370 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      473 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      852 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.550193 django-jet-new-2.3.1/jet/dashboard/locale/cs/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.573889 django-jet-new-2.3.1/jet/dashboard/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4470 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)    12226 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      471 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      843 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.550307 django-jet-new-2.3.1/jet/dashboard/locale/de/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.574454 django-jet-new-2.3.1/jet/dashboard/locale/de/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4947 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6200 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      393 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      842 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.550422 django-jet-new-2.3.1/jet/dashboard/locale/en/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.575150 django-jet-new-2.3.1/jet/dashboard/locale/en/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      495 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)    10871 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      378 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      827 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.550538 django-jet-new-2.3.1/jet/dashboard/locale/es/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.575697 django-jet-new-2.3.1/jet/dashboard/locale/es/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6524 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)    15268 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      474 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      846 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.550649 django-jet-new-2.3.1/jet/dashboard/locale/fa/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.575974 django-jet-new-2.3.1/jet/dashboard/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)    16058 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      851 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/fa/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.550765 django-jet-new-2.3.1/jet/dashboard/locale/fr/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.576249 django-jet-new-2.3.1/jet/dashboard/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)    12295 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      845 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.550880 django-jet-new-2.3.1/jet/dashboard/locale/pl/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.576534 django-jet-new-2.3.1/jet/dashboard/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4327 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)    14998 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.550993 django-jet-new-2.3.1/jet/dashboard/locale/pt-br/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.577215 django-jet-new-2.3.1/jet/dashboard/locale/pt-br/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5245 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/pt-br/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)    12513 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/pt-br/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      499 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      871 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.551106 django-jet-new-2.3.1/jet/dashboard/locale/ru/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.577760 django-jet-new-2.3.1/jet/dashboard/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6409 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)    13673 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      485 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      857 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.551218 django-jet-new-2.3.1/jet/dashboard/locale/zh_cn/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.578050 django-jet-new-2.3.1/jet/dashboard/locale/zh_cn/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3891 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)    12159 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.578323 django-jet-new-2.3.1/jet/dashboard/migrations/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1445 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/migrations/0001_initial.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/migrations/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1972 2023-07-11 00:41:50.000000 django-jet-new-2.3.1/jet/dashboard/models.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)    19375 2023-07-11 00:15:37.000000 django-jet-new-2.3.1/jet/dashboard/modules.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      280 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/settings.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.578557 django-jet-new-2.3.1/jet/dashboard/south_migrations/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2561 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/south_migrations/0001_initial.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/south_migrations/__init__.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.551467 django-jet-new-2.3.1/jet/dashboard/static/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.551580 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.578796 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/dashboard_modules/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2424 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/dashboard_modules/google_analytics.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2422 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/dashboard_modules/yandex_metrika.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.551627 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.579948 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     2991 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/CONTRIBUTING.md
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)   109612 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.js
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    52091 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.min.js
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     1060 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/LICENSE.md
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     1144 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/README.md
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.551802 django-jet-new-2.3.1/jet/dashboard/templates/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.580220 django-jet-new-2.3.1/jet/dashboard/templates/admin/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      949 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/admin/app_index.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      938 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/admin/index.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.580925 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1411 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/dashboard.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2060 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/dashboard_tools.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2163 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/module.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.582457 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1473 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/app_list.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      587 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/feed.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1056 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/google_analytics_period_visitors.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1099 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_chart.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      597 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_totals.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      922 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/link_list.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      804 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/model_list.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1667 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/recent_actions.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1050 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_period_visitors.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1097 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_chart.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      597 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_totals.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4140 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/update_module.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      950 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/update_module_fieldset.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.582690 django-jet-new-2.3.1/jet/dashboard/templatetags/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templatetags/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      738 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/templatetags/jet_dashboard_tags.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1694 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/urls.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      562 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/dashboard/utils.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8113 2023-07-11 00:15:37.000000 django-jet-new-2.3.1/jet/dashboard/views.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3097 2023-07-11 00:42:46.000000 django-jet-new-2.3.1/jet/filters.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5221 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/forms.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.553427 django-jet-new-2.3.1/jet/locale/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.552094 django-jet-new-2.3.1/jet/locale/ar/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.583477 django-jet-new-2.3.1/jet/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1242 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1877 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      739 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1389 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.552205 django-jet-new-2.3.1/jet/locale/cs/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.584067 django-jet-new-2.3.1/jet/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1148 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1779 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      703 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1343 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/cs/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.552315 django-jet-new-2.3.1/jet/locale/de/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.584588 django-jet-new-2.3.1/jet/locale/de/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1418 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1867 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      622 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1347 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.552424 django-jet-new-2.3.1/jet/locale/en/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.585147 django-jet-new-2.3.1/jet/locale/en/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      495 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1592 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      378 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1253 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.552555 django-jet-new-2.3.1/jet/locale/es/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.585675 django-jet-new-2.3.1/jet/locale/es/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1770 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2860 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      724 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.552690 django-jet-new-2.3.1/jet/locale/fa/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.585948 django-jet-new-2.3.1/jet/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3933 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1401 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/fa/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.552835 django-jet-new-2.3.1/jet/locale/fr/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.586245 django-jet-new-2.3.1/jet/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1770 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1379 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.552990 django-jet-new-2.3.1/jet/locale/pl/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.586799 django-jet-new-2.3.1/jet/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1926 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3852 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      479 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      751 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.553151 django-jet-new-2.3.1/jet/locale/pt_BR/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.587461 django-jet-new-2.3.1/jet/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1197 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1828 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      761 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1401 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.553323 django-jet-new-2.3.1/jet/locale/ru/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.588220 django-jet-new-2.3.1/jet/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1305 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1936 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      787 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1427 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.553496 django-jet-new-2.3.1/jet/locale/zh_CN/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.588540 django-jet-new-2.3.1/jet/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2005 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3729 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.588686 django-jet-new-2.3.1/jet/management/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/management/__init__.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.589092 django-jet-new-2.3.1/jet/management/commands/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/management/commands/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1430 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/management/commands/jet_custom_apps_example.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1509 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/management/commands/jet_side_menu_items_example.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.589510 django-jet-new-2.3.1/jet/migrations/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2930 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/migrations/0001_initial.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      317 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/migrations/0002_delete_userdashboardmodule.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/migrations/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1093 2023-07-11 00:41:50.000000 django-jet-new-2.3.1/jet/models.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1652 2023-07-11 00:47:03.000000 django-jet-new-2.3.1/jet/ordered_set.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      509 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/settings.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.589928 django-jet-new-2.3.1/jet/south_migrations/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4874 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/south_migrations/0001_initial.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2532 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/south_migrations/0002_auto__del_userdashboardmodule.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/south_migrations/__init__.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.555994 django-jet-new-2.3.1/jet/static/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.554173 django-jet-new-2.3.1/jet/static/admin/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.590768 django-jet-new-2.3.1/jet/static/admin/css/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/css/base.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/css/changelists.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/css/dashboard.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/css/fonts.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/css/forms.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/css/login.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/css/rtl.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/css/widgets.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.591032 django-jet-new-2.3.1/jet/static/admin/js/
+-rw-r--r--   0 munisisazade   (501) staff       (20)       85 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/js/SelectFilter2.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.591263 django-jet-new-2.3.1/jet/static/admin/js/admin/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/js/admin/DateTimeShortcuts.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/js/admin/RelatedObjectLookups.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/admin/js/related-widget-wrapper.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.555313 django-jet-new-2.3.1/jet/static/jet/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.594739 django-jet-new-2.3.1/jet/static/jet/css/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2211 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_base.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)      880 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_breadcrumbs.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)    17750 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_changeform.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     7749 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_changelist.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4029 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_content.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8804 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_dashboard.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1783 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_delete-confirmation.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3534 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_forms.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)       67 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_globals.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5165 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_header.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4119 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_helpers.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1959 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_login.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1656 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_messages.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)      740 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_modules.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1042 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_object-tools.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2051 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_relatedpopup.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)    11150 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_sidebar.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3249 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_tables.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6284 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/_variables.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.595463 django-jet-new-2.3.1/jet/static/jet/css/icons/
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)      800 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/icons/_variables.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.596270 django-jet-new-2.3.1/jet/static/jet/css/icons/fonts/
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6412 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/icons/fonts/jet-icons.eot
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    19664 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/icons/fonts/jet-icons.svg
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6240 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/icons/fonts/jet-icons.ttf
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6316 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/icons/fonts/jet-icons.woff
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     2248 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/icons/style.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.596446 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     3192 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/_jquery-ui.theme.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.601118 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      180 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      178 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      120 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      105 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      111 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      110 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      119 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      101 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-icons_cd0a0a_256x240.png
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.602292 django-jet-new-2.3.1/jet/static/jet/css/select2/
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     3095 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/select2/_layout.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     1662 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/select2/_multiple.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)      937 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/select2/_single.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.555233 django-jet-new-2.3.1/jet/static/jet/css/themes/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.608342 django-jet-new-2.3.1/jet/static/jet/css/themes/default/
+-rw-r--r--   0 munisisazade   (501) staff       (20)       66 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/default/_variables.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178918 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/default/base.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)   303057 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/default/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/default/base.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6760 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/default/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    23121 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/default/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/default/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23574 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/default/select2.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    44244 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/default/select2.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/default/select2.theme.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.611395 django-jet-new-2.3.1/jet/static/jet/css/themes/green/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4956 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/green/_variables.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178918 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/green/base.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)   308261 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/green/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/green/base.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6760 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/green/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    21794 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/green/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/green/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23574 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/green/select2.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    49427 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/green/select2.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/green/select2.theme.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.614718 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/_variables.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178850 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/base.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)   308602 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/base.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    22166 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23571 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/select2.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    49792 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/select2.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/select2.theme.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.617812 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/_variables.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178844 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/base.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)   308599 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/base.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    22166 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23569 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/select2.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    49791 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/select2.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/select2.theme.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.623903 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5318 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/_variables.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178844 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/base.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)   308610 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/base.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    22177 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23569 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/select2.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    49802 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/select2.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/select2.theme.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.626871 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/_variables.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178805 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/base.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)   308556 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/base.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    22172 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23573 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/select2.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    49799 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/select2.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/select2.theme.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)    53889 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/css/vendor.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.555663 django-jet-new-2.3.1/jet/static/jet/js/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.627026 django-jet-new-2.3.1/jet/static/jet/js/build/
+-rw-r--r--   0 munisisazade   (501) staff       (20)   417084 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/build/bundle.min.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.555602 django-jet-new-2.3.1/jet/static/jet/js/i18n/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.644779 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1144 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-af.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1458 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ar-DZ.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1458 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ar.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1168 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-az.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1394 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-be.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1371 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-bg.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1092 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-bs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1122 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ca.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1171 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-cs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1155 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-cy-GB.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-da.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1129 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-de.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1436 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-el.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1148 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-en-AU.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1125 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-en-GB.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1150 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-en-NZ.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1141 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-eo.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1136 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-es.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1199 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-et.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1091 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-eu.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1382 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fa.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1193 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1166 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fo.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1161 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CA.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1208 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CH.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1289 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-gl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1264 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-he.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1561 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-hi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-hr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1140 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-hu.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1422 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-hy.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1130 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-id.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1194 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-is.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1169 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-it-CH.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1160 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-it.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1150 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ja.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1664 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ka.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-kk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1578 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-km.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1159 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ko.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1356 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ky.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1182 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-lb.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1209 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-lt.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1190 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-lv.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1305 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-mk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1684 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ml.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1139 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ms.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1145 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-nb.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1169 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-nl-BE.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1167 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-nl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1142 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-nn.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1137 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-no.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1165 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-pl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1196 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-pt-BR.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1116 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-pt.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1155 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-rm.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1237 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ro.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ru.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1153 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1191 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1135 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sq.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1099 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sr-SR.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1285 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sv.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1744 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ta.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1522 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-th.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1322 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-tj.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1131 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-tr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1431 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-uk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1342 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-vi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1234 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-CN.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1232 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-HK.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1228 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-TW.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.647126 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      480 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-cs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      462 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-de.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      493 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-es.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      550 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-fr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      503 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-hr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      458 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-hu.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      485 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-it.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      500 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ja.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      510 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-mk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      424 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-nl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      457 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-pl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      480 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-pt-BR.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      520 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ru.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      492 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-sl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      468 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-sv.js
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)      503 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-tr.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.654906 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      701 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/az.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      906 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/bg.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      876 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/ca.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1236 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/cs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      816 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/da.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      775 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/de.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      827 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/en.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      871 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/es.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      775 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/et.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      844 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/eu.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1004 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/fa.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      703 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/fi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      823 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/fr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      800 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/gl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      894 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/he.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1125 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/hi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      780 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/hr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      727 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/hu.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      693 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/id.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      773 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/is.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      876 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/it.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      854 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/ko.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      878 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/lt.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      872 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/lv.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      979 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/mk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      723 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/nb.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      867 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/nl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      926 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/pl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      853 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/pt-BR.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      859 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/pt.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      834 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/ro.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1127 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/ru.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1184 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/sk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      880 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/sr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      786 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/sv.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      948 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/th.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      720 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/tr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/uk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      801 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/vi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      769 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/zh-CN.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      708 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/zh-TW.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.655071 django-jet-new-2.3.1/jet/static/jet/js/src/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.657826 django-jet-new-2.3.1/jet/static/jet/js/src/features/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2852 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/changeform-tabs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1354 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/changeform.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3803 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/changelist.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/checkboxes.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6694 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/compact-inline.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)    11563 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/dashboard.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4309 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/date-time-widgets.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2350 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/filters.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      895 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/inlines.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8343 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/related-popups.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      824 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/scroll-to-bottom-detector.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8381 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/selects.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      575 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/siblings.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.658376 django-jet-new-2.3.1/jet/static/jet/js/src/features/sidebar/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3652 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/sidebar/application-pinning.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4219 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/sidebar/bookmarks.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3391 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/sidebar/main.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     7484 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/sidebar/popup.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1952 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/themes.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      709 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/tooltips.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      986 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/features/touchmove-non-scrollable.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.660442 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1529 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/actions.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      746 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/branding.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1050 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/breadcrumbs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2552 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/changeform-tabs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      449 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/delete-confirmation.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      730 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/icons.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      367 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/object-tools.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2635 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/paginator.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1187 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/related-widget-wrapper.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      857 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/stacked-inline.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1226 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/tabular-inline.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4842 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/toolbar.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1445 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/user-tools.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1199 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/main.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.661214 django-jet-new-2.3.1/jet/static/jet/js/src/utils/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      206 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/utils/jquery-icontains.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      178 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/utils/jquery-slidefade.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      132 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/utils/translate.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      779 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/jet/js/src/utils/window-storage.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.556040 django-jet-new-2.3.1/jet/static/range_filter/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.661394 django-jet-new-2.3.1/jet/static/range_filter/css/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      244 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/static/range_filter/css/style.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.556410 django-jet-new-2.3.1/jet/templates/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.661982 django-jet-new-2.3.1/jet/templates/admin/
+-rw-r--r--   0 munisisazade   (501) staff       (20)    21995 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/templates/admin/base.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.662123 django-jet-new-2.3.1/jet/templates/admin/edit_inline/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3630 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/templates/admin/edit_inline/compact.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.662283 django-jet-new-2.3.1/jet/templates/admin/includes/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1808 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/templates/admin/includes/fieldset.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      379 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/templates/admin/popup_response.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.662443 django-jet-new-2.3.1/jet/templates/jet/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      450 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/templates/jet/related_field_ajax_list_filter.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.662613 django-jet-new-2.3.1/jet/templates/rangefilter/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1940 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/templates/rangefilter/date_filter.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.662897 django-jet-new-2.3.1/jet/templatetags/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/templatetags/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     7774 2023-07-11 00:42:46.000000 django-jet-new-2.3.1/jet/templatetags/jet_tags.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:48:52.666703 django-jet-new-2.3.1/jet/tests/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/tests/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      347 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/tests/admin.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1735 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/tests/dashboard.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      661 2023-07-11 00:41:50.000000 django-jet-new-2.3.1/jet/tests/models.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1945 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/tests/settings.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3085 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/tests/test_dashboard.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2243 2023-07-11 00:42:46.000000 django-jet-new-2.3.1/jet/tests/test_filters.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2003 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/tests/test_ordered_set.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3711 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/tests/test_tags.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2371 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/tests/test_utils.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8951 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/tests/test_views.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      858 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/tests/urls.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1030 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/urls.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)    16170 2023-07-11 00:44:55.000000 django-jet-new-2.3.1/jet/utils.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1698 2023-07-11 00:08:01.000000 django-jet-new-2.3.1/jet/views.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)       38 2023-07-11 00:48:52.667946 django-jet-new-2.3.1/setup.cfg
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2170 2023-07-11 00:23:06.000000 django-jet-new-2.3.1/setup.py
```

### Comparing `django-jet-new-2.3.0/LICENSE` & `django-jet-new-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/PKG-INFO` & `django-jet-new-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jet-new
-Version: 2.3.0
+Version: 2.3.1
 Summary: Modern template for Django admin interface with improved functionality
 Home-page: https://github.com/geex-arts/django-jet
 Author: Denis Kildishev
 Author-email: support@jet.geex-arts.com
 License: AGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 4.2
```

### Comparing `django-jet-new-2.3.0/README.rst` & `django-jet-new-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/django_jet_new.egg-info/PKG-INFO` & `django-jet-new-2.3.1/django_jet_new.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jet-new
-Version: 2.3.0
+Version: 2.3.1
 Summary: Modern template for Django admin interface with improved functionality
 Home-page: https://github.com/geex-arts/django-jet
 Author: Denis Kildishev
 Author-email: support@jet.geex-arts.com
 License: AGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 4.2
```

### Comparing `django-jet-new-2.3.0/django_jet_new.egg-info/SOURCES.txt` & `django-jet-new-2.3.1/django_jet_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/dashboard.py` & `django-jet-new-2.3.1/jet/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/dashboard_modules/google_analytics.py` & `django-jet-new-2.3.1/jet/dashboard/dashboard_modules/google_analytics.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 from django.utils.text import capfirst
 from googleapiclient.discovery import build
 import httplib2
 from jet.dashboard.modules import DashboardModule
 from oauth2client.client import flow_from_clientsecrets, OAuth2Credentials, AccessTokenRefreshError, Storage
 from django.utils.translation import gettext_lazy as _
 from django.conf import settings
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 try:
     from django.utils.encoding import force_unicode
 except ImportError:
-    from django.utils.encoding import force_text as force_unicode
+    from django.utils.encoding import force_str as force_unicode
 
 try:
     from django.forms.utils import flatatt
 except ImportError:
     from django.forms.util import flatatt
 
 JET_MODULE_GOOGLE_ANALYTICS_CLIENT_SECRETS_FILE = getattr(
```

### Comparing `django-jet-new-2.3.0/jet/dashboard/dashboard_modules/google_analytics_views.py` & `django-jet-new-2.3.1/jet/dashboard/dashboard_modules/google_analytics_views.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/dashboard_modules/yandex_metrika.py` & `django-jet-new-2.3.1/jet/dashboard/dashboard_modules/yandex_metrika.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from django.utils import formats
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.text import capfirst
 from jet.dashboard.modules import DashboardModule
 from django.utils.translation import gettext_lazy as _
 from django.conf import settings
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 try:
     from urllib import request
     from urllib.parse import urlencode
     from urllib.error import URLError, HTTPError
 except ImportError:
     import urllib2 as request
```

### Comparing `django-jet-new-2.3.0/jet/dashboard/dashboard_modules/yandex_metrika_views.py` & `django-jet-new-2.3.1/jet/dashboard/dashboard_modules/yandex_metrika_views.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/forms.py` & `django-jet-new-2.3.1/jet/dashboard/forms.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/ar/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/dashboard/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/ar/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/cs/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/dashboard/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/cs/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/de/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/dashboard/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/de/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/de/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/dashboard/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/en/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/en/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/dashboard/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/es/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/dashboard/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/es/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/es/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/dashboard/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/fa/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/fa/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/dashboard/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/fr/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/fr/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/dashboard/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/pl/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/dashboard/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/pl/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/pt-br/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/dashboard/locale/pt-br/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/pt-br/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/pt-br/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/ru/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/dashboard/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/ru/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/migrations/0001_initial.py` & `django-jet-new-2.3.1/jet/dashboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/models.py` & `django-jet-new-2.3.1/jet/dashboard/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from importlib import import_module
 import json
 from django.db import models
-from django.utils.encoding import python_2_unicode_compatible
+
 from django.utils.translation import gettext_lazy as _
 from jet.utils import LazyDateTimeEncoder
 
 
-@python_2_unicode_compatible
+
 class UserDashboardModule(models.Model):
     title = models.CharField(verbose_name=_('Title'), max_length=255)
     module = models.CharField(verbose_name=_('module'), max_length=255)
     app_label = models.CharField(verbose_name=_('application name'), max_length=255, null=True, blank=True)
     user = models.PositiveIntegerField(verbose_name=_('user'))
     column = models.PositiveIntegerField(verbose_name=_('column'))
     order = models.IntegerField(verbose_name=_('order'))
```

### Comparing `django-jet-new-2.3.0/jet/dashboard/modules.py` & `django-jet-new-2.3.1/jet/dashboard/modules.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/south_migrations/0001_initial.py` & `django-jet-new-2.3.1/jet/dashboard/south_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/dashboard_modules/google_analytics.js` & `django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/dashboard_modules/google_analytics.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/dashboard_modules/yandex_metrika.js` & `django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/dashboard_modules/yandex_metrika.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/CONTRIBUTING.md` & `django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.js` & `django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.min.js` & `django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/LICENSE.md` & `django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/static/jet.dashboard/vendor/chart.js/README.md` & `django-jet-new-2.3.1/jet/dashboard/static/jet.dashboard/vendor/chart.js/README.md`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/admin/app_index.html` & `django-jet-new-2.3.1/jet/dashboard/templates/admin/app_index.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/admin/index.html` & `django-jet-new-2.3.1/jet/dashboard/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/dashboard.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/dashboard_tools.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/dashboard_tools.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/module.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/module.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/app_list.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/app_list.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/feed.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/feed.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/google_analytics_period_visitors.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/google_analytics_period_visitors.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_chart.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_chart.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_totals.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_totals.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/link_list.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/link_list.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/model_list.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/model_list.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/recent_actions.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/recent_actions.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_period_visitors.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_period_visitors.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_chart.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_chart.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_totals.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_totals.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/update_module.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/update_module.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templates/jet.dashboard/update_module_fieldset.html` & `django-jet-new-2.3.1/jet/dashboard/templates/jet.dashboard/update_module_fieldset.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/templatetags/jet_dashboard_tags.py` & `django-jet-new-2.3.1/jet/dashboard/templatetags/jet_dashboard_tags.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/urls.py` & `django-jet-new-2.3.1/jet/dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/utils.py` & `django-jet-new-2.3.1/jet/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/dashboard/views.py` & `django-jet-new-2.3.1/jet/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/filters.py` & `django-jet-new-2.3.1/jet/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.contrib.admin import RelatedFieldListFilter
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str as smart_text
 from django.utils.html import format_html
 try:
     from django.core.urlresolvers import reverse
 except ImportError: # Django 1.11
     from django.urls import reverse
 
 try:
```

### Comparing `django-jet-new-2.3.0/jet/forms.py` & `django-jet-new-2.3.1/jet/forms.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/ar/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/ar/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/ar/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.1/jet/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/ar/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/cs/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/cs/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/cs/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.1/jet/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/cs/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/de/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/de/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/de/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.1/jet/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/de/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/en/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/en/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/es/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/es/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/es/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.1/jet/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/es/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/fa/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/fa/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/fr/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/fr/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/pl/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/pl/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/pl/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/pt_BR/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/pt_BR/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.1/jet/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/pt_BR/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/ru/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/ru/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/ru/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.1/jet/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/ru/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.1/jet/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/zh_CN/LC_MESSAGES/django.mo` & `django-jet-new-2.3.1/jet/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/locale/zh_CN/LC_MESSAGES/django.po` & `django-jet-new-2.3.1/jet/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/management/commands/jet_custom_apps_example.py` & `django-jet-new-2.3.1/jet/management/commands/jet_custom_apps_example.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/management/commands/jet_side_menu_items_example.py` & `django-jet-new-2.3.1/jet/management/commands/jet_side_menu_items_example.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/migrations/0001_initial.py` & `django-jet-new-2.3.1/jet/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/models.py` & `django-jet-new-2.3.1/jet/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.db import models
 from django.utils import timezone
-from django.utils.encoding import python_2_unicode_compatible
+
 from django.utils.translation import gettext_lazy as _
 
 
-@python_2_unicode_compatible
+
 class Bookmark(models.Model):
     url = models.URLField(verbose_name=_('URL'))
     title = models.CharField(verbose_name=_('title'), max_length=255)
     user = models.PositiveIntegerField(verbose_name=_('user'))
     date_add = models.DateTimeField(verbose_name=_('date created'), default=timezone.now)
 
     class Meta:
@@ -16,15 +16,15 @@
         verbose_name_plural = _('bookmarks')
         ordering = ('date_add',)
 
     def __str__(self):
         return self.title
 
 
-@python_2_unicode_compatible
+
 class PinnedApplication(models.Model):
     app_label = models.CharField(verbose_name=_('application name'), max_length=255)
     user = models.PositiveIntegerField(verbose_name=_('user'))
     date_add = models.DateTimeField(verbose_name=_('date created'), default=timezone.now)
 
     class Meta:
         verbose_name = _('pinned application')
```

### Comparing `django-jet-new-2.3.0/jet/ordered_set.py` & `django-jet-new-2.3.1/jet/ordered_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections
 
 
-class OrderedSet(collections.MutableSet):
+class OrderedSet(collections.abc.MutableSet):
     def __init__(self, iterable=None):
         self.end = end = []
         end += [None, end, end]         # sentinel node for doubly linked list
         self.map = {}                   # key --> [key, prev, next]
         if iterable is not None:
             self |= iterable
```

### Comparing `django-jet-new-2.3.0/jet/south_migrations/0001_initial.py` & `django-jet-new-2.3.1/jet/south_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/south_migrations/0002_auto__del_userdashboardmodule.py` & `django-jet-new-2.3.1/jet/south_migrations/0002_auto__del_userdashboardmodule.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_base.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_base.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_breadcrumbs.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_changeform.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_changeform.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_changelist.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_changelist.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_content.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_content.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_dashboard.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_dashboard.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_delete-confirmation.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_delete-confirmation.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_forms.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_forms.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_header.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_header.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_helpers.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_helpers.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_login.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_login.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_messages.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_messages.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_modules.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_modules.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_object-tools.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_object-tools.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_relatedpopup.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_relatedpopup.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_sidebar.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_tables.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_tables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/_variables.scss` & `django-jet-new-2.3.1/jet/static/jet/css/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/icons/_variables.scss` & `django-jet-new-2.3.1/jet/static/jet/css/icons/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/icons/fonts/jet-icons.eot` & `django-jet-new-2.3.1/jet/static/jet/css/icons/fonts/jet-icons.eot`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/icons/fonts/jet-icons.svg` & `django-jet-new-2.3.1/jet/static/jet/css/icons/fonts/jet-icons.svg`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/icons/fonts/jet-icons.ttf` & `django-jet-new-2.3.1/jet/static/jet/css/icons/fonts/jet-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/icons/fonts/jet-icons.woff` & `django-jet-new-2.3.1/jet/static/jet/css/icons/fonts/jet-icons.woff`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/icons/style.css` & `django-jet-new-2.3.1/jet/static/jet/css/icons/style.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/_jquery-ui.theme.scss` & `django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/_jquery-ui.theme.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-icons_222222_256x240.png` & `django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-icons_2e83ff_256x240.png` & `django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-icons_454545_256x240.png` & `django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-icons_888888_256x240.png` & `django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/jquery-ui/images/ui-icons_cd0a0a_256x240.png` & `django-jet-new-2.3.1/jet/static/jet/css/jquery-ui/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/select2/_layout.scss` & `django-jet-new-2.3.1/jet/static/jet/css/select2/_layout.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/select2/_multiple.scss` & `django-jet-new-2.3.1/jet/static/jet/css/select2/_multiple.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/select2/_single.scss` & `django-jet-new-2.3.1/jet/static/jet/css/select2/_single.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/default/base.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/default/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/default/base.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/default/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/default/jquery-ui.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/default/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/default/jquery-ui.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/default/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/default/select2.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/default/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/default/select2.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/default/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/green/_variables.scss` & `django-jet-new-2.3.1/jet/static/jet/css/themes/green/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/green/base.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/green/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/green/base.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/green/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/green/jquery-ui.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/green/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/green/jquery-ui.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/green/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/green/select2.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/green/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/green/select2.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/green/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/_variables.scss` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/base.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/base.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/select2.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-blue/select2.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-blue/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/_variables.scss` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/base.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/base.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/select2.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-gray/select2.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-gray/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/_variables.scss` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/base.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/base.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/jquery-ui.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/jquery-ui.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/select2.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-green/select2.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-green/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/_variables.scss` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/base.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/base.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/select2.theme.css` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/themes/light-violet/select2.theme.css.map` & `django-jet-new-2.3.1/jet/static/jet/css/themes/light-violet/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/css/vendor.css` & `django-jet-new-2.3.1/jet/static/jet/css/vendor.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/build/bundle.min.js` & `django-jet-new-2.3.1/jet/static/jet/js/build/bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-af.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-af.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ar-DZ.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ar-DZ.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ar.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ar.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-az.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-az.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-be.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-be.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-bg.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-bg.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-bs.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-bs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ca.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ca.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-cs.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-cs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-cy-GB.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-cy-GB.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-da.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-da.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-de.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-de.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-el.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-el.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-en-AU.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-en-AU.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-en-GB.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-en-GB.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-en-NZ.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-en-NZ.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-eo.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-eo.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-es.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-es.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-et.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-et.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-eu.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-eu.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fa.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fa.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fi.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fo.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fo.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CA.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CA.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CH.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CH.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-fr.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-fr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-gl.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-gl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-he.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-he.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-hi.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-hi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-hr.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-hr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-hu.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-hu.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-hy.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-hy.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-id.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-id.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-is.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-is.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-it-CH.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-it-CH.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-it.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-it.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ja.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ja.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ka.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ka.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-kk.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-kk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-km.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-km.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ko.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ko.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ky.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ky.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-lb.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-lb.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-lt.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-lt.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-lv.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-lv.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-mk.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-mk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ml.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ml.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ms.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ms.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-nb.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-nb.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-nl-BE.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-nl-BE.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-nl.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-nl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-nn.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-nn.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-no.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-no.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-pl.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-pl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-pt-BR.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-pt.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-pt.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-rm.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-rm.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ro.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ro.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ru.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ru.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sk.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sl.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sq.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sq.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sr-SR.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sr-SR.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sr.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-sv.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-sv.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-ta.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-ta.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-th.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-th.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-tj.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-tj.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-tr.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-tr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-uk.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-uk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-vi.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-vi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-CN.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-HK.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-HK.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-TW.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-fr.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-fr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ru.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ru.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/az.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/az.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/bg.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/bg.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/ca.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/ca.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/cs.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/cs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/da.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/da.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/de.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/de.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/en.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/en.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/es.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/es.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/et.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/et.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/eu.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/eu.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/fa.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/fa.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/fi.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/fi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/fr.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/fr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/gl.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/gl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/he.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/he.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/hi.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/hi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/hr.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/hr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/hu.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/hu.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/id.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/id.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/is.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/is.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/it.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/it.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/ko.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/ko.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/lt.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/lt.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/lv.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/lv.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/mk.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/mk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/nb.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/nb.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/nl.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/nl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/pl.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/pl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/pt-BR.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/pt.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/pt.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/ro.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/ro.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/ru.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/ru.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/sk.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/sk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/sr.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/sr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/sv.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/sv.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/th.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/th.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/tr.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/tr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/uk.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/uk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/vi.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/vi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/zh-CN.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/i18n/select2/zh-TW.js` & `django-jet-new-2.3.1/jet/static/jet/js/i18n/select2/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/changeform-tabs.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/changeform-tabs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/changeform.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/changeform.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/changelist.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/changelist.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/checkboxes.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/checkboxes.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/compact-inline.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/compact-inline.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/dashboard.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/date-time-widgets.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/date-time-widgets.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/filters.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/filters.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/inlines.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/inlines.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/related-popups.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/related-popups.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/scroll-to-bottom-detector.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/scroll-to-bottom-detector.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/selects.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/selects.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/siblings.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/siblings.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/sidebar/application-pinning.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/sidebar/application-pinning.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/sidebar/bookmarks.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/sidebar/bookmarks.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/sidebar/main.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/sidebar/main.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/sidebar/popup.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/sidebar/popup.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/themes.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/themes.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/tooltips.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/tooltips.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/features/touchmove-non-scrollable.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/features/touchmove-non-scrollable.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/actions.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/actions.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/branding.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/branding.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/breadcrumbs.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/breadcrumbs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/changeform-tabs.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/changeform-tabs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/icons.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/icons.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/paginator.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/paginator.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/related-widget-wrapper.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/related-widget-wrapper.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/stacked-inline.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/stacked-inline.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/tabular-inline.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/tabular-inline.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/toolbar.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/toolbar.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/layout-updaters/user-tools.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/layout-updaters/user-tools.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/main.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/main.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/static/jet/js/src/utils/window-storage.js` & `django-jet-new-2.3.1/jet/static/jet/js/src/utils/window-storage.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/templates/admin/base.html` & `django-jet-new-2.3.1/jet/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/templates/admin/edit_inline/compact.html` & `django-jet-new-2.3.1/jet/templates/admin/edit_inline/compact.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/templates/admin/includes/fieldset.html` & `django-jet-new-2.3.1/jet/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/templates/rangefilter/date_filter.html` & `django-jet-new-2.3.1/jet/templates/rangefilter/date_filter.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/templatetags/jet_tags.py` & `django-jet-new-2.3.1/jet/templatetags/jet_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 except ImportError: # Django 1.11
     from django.urls import reverse
 
 from django.forms import CheckboxInput, ModelChoiceField, Select, ModelMultipleChoiceField, SelectMultiple
 from django.contrib.admin.widgets import RelatedFieldWidgetWrapper
 from django.utils.formats import get_format
 from django.utils.safestring import mark_safe
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str as smart_text
 from jet import settings, VERSION
 from jet.models import Bookmark
 from jet.utils import get_model_instance_label, get_model_queryset, get_possible_language_codes, \
     get_admin_site, get_menu_items
 
 try:
     from urllib.parse import parse_qsl
```

### Comparing `django-jet-new-2.3.0/jet/tests/dashboard.py` & `django-jet-new-2.3.1/jet/tests/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/tests/models.py` & `django-jet-new-2.3.1/jet/tests/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from django.db import models
-from django.utils.encoding import python_2_unicode_compatible
 
 
-@python_2_unicode_compatible
+
+
 class TestModel(models.Model):
     field1 = models.CharField(max_length=255)
     field2 = models.IntegerField()
 
     def __str__(self):
         return '%s%d' % (self.field1, self.field2)
 
 
-@python_2_unicode_compatible
+
 class RelatedToTestModel(models.Model):
     field = models.ForeignKey(TestModel, on_delete=models.CASCADE)
 
     def __str__(self):
         return self.field
 
 
-@python_2_unicode_compatible
+
 class SearchableTestModel(models.Model):
     field1 = models.CharField(max_length=255)
     field2 = models.IntegerField()
 
     def __str__(self):
         return '%s%d' % (self.field1, self.field2)
```

### Comparing `django-jet-new-2.3.0/jet/tests/settings.py` & `django-jet-new-2.3.1/jet/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/tests/test_dashboard.py` & `django-jet-new-2.3.1/jet/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/tests/test_filters.py` & `django-jet-new-2.3.1/jet/tests/test_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.contrib import admin
 from django.test import TestCase, RequestFactory
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str as smart_text
 from jet.filters import RelatedFieldAjaxListFilter
 from jet.tests.models import RelatedToTestModel, TestModel
 
 try:
     from django.contrib.admin.utils import get_fields_from_path
 except ImportError: # Django 1.6
     from django.contrib.admin.util import get_fields_from_path
```

### Comparing `django-jet-new-2.3.0/jet/tests/test_ordered_set.py` & `django-jet-new-2.3.1/jet/tests/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/tests/test_tags.py` & `django-jet-new-2.3.1/jet/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/tests/test_utils.py` & `django-jet-new-2.3.1/jet/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/tests/test_views.py` & `django-jet-new-2.3.1/jet/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/tests/urls.py` & `django-jet-new-2.3.1/jet/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/urls.py` & `django-jet-new-2.3.1/jet/urls.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/jet/utils.py` & `django-jet-new-2.3.1/jet/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from django.http import HttpResponse
 try:
     from django.core.urlresolvers import reverse, resolve, NoReverseMatch
 except ImportError: # Django 1.11
     from django.urls import reverse, resolve, NoReverseMatch
 
 from django.contrib.admin import AdminSite
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str as smart_text
 from django.utils.text import capfirst
 from django.contrib import messages
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.functional import Promise
 from django.contrib.admin.options import IncorrectLookupParameters
 from django.contrib import admin
 from django.utils.translation import gettext_lazy as _
 from django.utils.text import slugify
 
 try:
```

### Comparing `django-jet-new-2.3.0/jet/views.py` & `django-jet-new-2.3.1/jet/views.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.0/setup.py` & `django-jet-new-2.3.1/setup.py`

 * *Files identical despite different names*

