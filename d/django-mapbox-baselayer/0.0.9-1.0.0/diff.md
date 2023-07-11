# Comparing `tmp/django-mapbox-baselayer-0.0.9.tar.gz` & `tmp/django-mapbox-baselayer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-mapbox-baselayer-0.0.9.tar", last modified: Wed Nov  9 09:22:19 2022, max compression
+gzip compressed data, was "django-mapbox-baselayer-1.0.0.tar", last modified: Tue Jul 11 12:26:50 2023, max compression
```

## Comparing `django-mapbox-baselayer-0.0.9.tar` & `django-mapbox-baselayer-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/django_mapbox_baselayer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/django_mapbox_baselayer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/django_mapbox_baselayer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/django_mapbox_baselayer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/django_mapbox_baselayer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4150 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/django_mapbox_baselayer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/VERSION.md
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/0004_auto_20191202_1834.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/0006_alter_baselayertile_id_alter_mapbaselayer_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/0003_auto_20191202_0937.py
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/0005_auto_20191202_1840.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/0002_auto_20191129_0942.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      857 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/commands/install_mapbox_baselayer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/commands/install_opentopomap_baselayer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/commands/install_ign_baselayer.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/commands/install_osm_baselayer.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3309 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/mapbox_baselayer/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4150 2022-11-09 09:22:19.000000 django-mapbox-baselayer-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-11-09 09:22:05.000000 django-mapbox-baselayer-0.0.9/CHANGES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.599796 django-mapbox-baselayer-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-11 12:26:50.599796 django-mapbox-baselayer-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.595796 django-mapbox-baselayer-1.0.0/django_mapbox_baselayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-11 12:26:50.000000 django-mapbox-baselayer-1.0.0/django_mapbox_baselayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-11 12:26:50.000000 django-mapbox-baselayer-1.0.0/django_mapbox_baselayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:26:50.000000 django-mapbox-baselayer-1.0.0/django_mapbox_baselayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 12:26:50.000000 django-mapbox-baselayer-1.0.0/django_mapbox_baselayer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 12:26:50.000000 django-mapbox-baselayer-1.0.0/django_mapbox_baselayer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.595796 django-mapbox-baselayer-1.0.0/mapbox_baselayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/VERSION.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.595796 django-mapbox-baselayer-1.0.0/mapbox_baselayer/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.595796 django-mapbox-baselayer-1.0.0/mapbox_baselayer/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.599796 django-mapbox-baselayer-1.0.0/mapbox_baselayer/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.595796 django-mapbox-baselayer-1.0.0/mapbox_baselayer/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.599796 django-mapbox-baselayer-1.0.0/mapbox_baselayer/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.599796 django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.599796 django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/commands/install_ign_baselayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/commands/install_mapbox_baselayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/commands/install_opentopomap_baselayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/commands/install_osm_baselayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.599796 django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0002_auto_20191129_0942.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0003_auto_20191202_0937.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0004_auto_20191202_1834.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0005_auto_20191202_1840.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0006_alter_baselayertile_id_alter_mapbaselayer_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0007_alter_mapbaselayer_attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:50.599796 django-mapbox-baselayer-1.0.0/mapbox_baselayer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/mapbox_baselayer/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:26:50.599796 django-mapbox-baselayer-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-11 12:26:42.000000 django-mapbox-baselayer-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-mapbox-baselayer-0.0.9/README.md` & `django-mapbox-baselayer-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/django_mapbox_baselayer.egg-info/SOURCES.txt` & `django-mapbox-baselayer-1.0.0/django_mapbox_baselayer.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -24,12 +24,13 @@
 mapbox_baselayer/management/commands/install_osm_baselayer.py
 mapbox_baselayer/migrations/0001_initial.py
 mapbox_baselayer/migrations/0002_auto_20191129_0942.py
 mapbox_baselayer/migrations/0003_auto_20191202_0937.py
 mapbox_baselayer/migrations/0004_auto_20191202_1834.py
 mapbox_baselayer/migrations/0005_auto_20191202_1840.py
 mapbox_baselayer/migrations/0006_alter_baselayertile_id_alter_mapbaselayer_id_and_more.py
+mapbox_baselayer/migrations/0007_alter_mapbaselayer_attribution.py
 mapbox_baselayer/migrations/__init__.py
 mapbox_baselayer/tests/__init__.py
 mapbox_baselayer/tests/test_commands.py
 mapbox_baselayer/tests/test_models.py
 mapbox_baselayer/tests/test_views.py
```

### Comparing `django-mapbox-baselayer-0.0.9/django_mapbox_baselayer.egg-info/PKG-INFO` & `django-mapbox-baselayer-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: django-mapbox-baselayer
-Version: 0.0.9
+Version: 1.0.0
 Summary: Django model to store and serve mapbox base layer config
 Home-page: https://github.com/makinacorpus/django-mapbox-baselayer.git
 Author: Makina Corpus
 Author-email: geobi@makina-corpus.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -89,14 +87,22 @@
 ./manage.py install_ign_baselayer _your_api_key_ --layers ortho plan maps se-classique se-standard cadastre
 ```
 
 
 CHANGELOG
 =========
 
+1.0.0         (2023-07-11)
+--------------------------
+
+* Increase attribution size to 1024 chars.
+* Support django 4.2, drop django 2.2
+* Support python 3.11
+
+
 0.0.9         (2022-11-09)
 --------------------------
 
 * Improve install_ign_baselayer command. Add Plan IGN V2 and fix multi layer import.
 * Support django 3.2, 4.0 and 4.1
 * Support python 3.10
 
@@ -147,9 +153,7 @@
 * Increase tile url max size
 
 
 0.0.1         (2019-11-25)
 --------------------------
 
 * First release
-
-
```

### Comparing `django-mapbox-baselayer-0.0.9/setup.py` & `django-mapbox-baselayer-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/0004_auto_20191202_1834.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0004_auto_20191202_1834.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/0001_initial.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/0006_alter_baselayertile_id_alter_mapbaselayer_id_and_more.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0006_alter_baselayertile_id_alter_mapbaselayer_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/migrations/0003_auto_20191202_0937.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/migrations/0003_auto_20191202_0937.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/locale/fr/LC_MESSAGES/django.po` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/locale/en/LC_MESSAGES/django.po` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/commands/install_mapbox_baselayer.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/commands/install_mapbox_baselayer.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/commands/install_opentopomap_baselayer.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/commands/install_opentopomap_baselayer.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/commands/install_ign_baselayer.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/commands/install_ign_baselayer.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/management/commands/install_osm_baselayer.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/management/commands/install_osm_baselayer.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/tests/test_models.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/tests/test_views.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/tests/test_commands.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-mapbox-baselayer-0.0.9/mapbox_baselayer/models.py` & `django-mapbox-baselayer-1.0.0/mapbox_baselayer/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     sprite = models.CharField(max_length=255, blank=True)
     glyphs = models.CharField(max_length=255, blank=True)
     min_zoom = models.PositiveSmallIntegerField(default=0)
     max_zoom = models.PositiveSmallIntegerField(default=22)
     tile_size = models.PositiveSmallIntegerField(
         default=512, help_text=_("Raster tile size. Set 256 for 3rd party raster tilesets.")
     )
-    attribution = models.CharField(max_length=255, blank=True, default="")
+    attribution = models.CharField(max_length=1024, blank=True, default="")
 
     def __str__(self):
         return self.name
 
     def get_source(self):
         source = {
             "type": f"{self.base_layer_type}",
```

### Comparing `django-mapbox-baselayer-0.0.9/PKG-INFO` & `django-mapbox-baselayer-1.0.0/django_mapbox_baselayer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: django-mapbox-baselayer
-Version: 0.0.9
+Version: 1.0.0
 Summary: Django model to store and serve mapbox base layer config
 Home-page: https://github.com/makinacorpus/django-mapbox-baselayer.git
 Author: Makina Corpus
 Author-email: geobi@makina-corpus.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -89,14 +87,22 @@
 ./manage.py install_ign_baselayer _your_api_key_ --layers ortho plan maps se-classique se-standard cadastre
 ```
 
 
 CHANGELOG
 =========
 
+1.0.0         (2023-07-11)
+--------------------------
+
+* Increase attribution size to 1024 chars.
+* Support django 4.2, drop django 2.2
+* Support python 3.11
+
+
 0.0.9         (2022-11-09)
 --------------------------
 
 * Improve install_ign_baselayer command. Add Plan IGN V2 and fix multi layer import.
 * Support django 3.2, 4.0 and 4.1
 * Support python 3.10
 
@@ -147,9 +153,7 @@
 * Increase tile url max size
 
 
 0.0.1         (2019-11-25)
 --------------------------
 
 * First release
-
-
```

### Comparing `django-mapbox-baselayer-0.0.9/CHANGES.md` & `django-mapbox-baselayer-1.0.0/CHANGES.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGELOG
 =========
 
+1.0.0         (2023-07-11)
+--------------------------
+
+* Increase attribution size to 1024 chars.
+* Support django 4.2, drop django 2.2
+* Support python 3.11
+
+
 0.0.9         (2022-11-09)
 --------------------------
 
 * Improve install_ign_baselayer command. Add Plan IGN V2 and fix multi layer import.
 * Support django 3.2, 4.0 and 4.1
 * Support python 3.10
```

