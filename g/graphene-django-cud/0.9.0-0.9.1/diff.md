# Comparing `tmp/graphene-django-cud-0.9.0.tar.gz` & `tmp/graphene-django-cud-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-django-cud-0.9.0.tar", last modified: Mon May 24 11:58:52 2021, max compression
+gzip compressed data, was "dist/graphene-django-cud-0.9.1.tar", last modified: Wed Dec 29 18:36:35 2021, max compression
```

## Comparing `graphene-django-cud-0.9.0.tar` & `graphene-django-cud-0.9.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 tormod    (1000) tormod    (1000)        0 2021-05-24 11:58:52.083689 graphene-django-cud-0.9.0/
--rw-r--r--   0 tormod    (1000) tormod    (1000)     1054 2019-10-23 08:04:35.000000 graphene-django-cud-0.9.0/LICENSE.md
--rw-r--r--   0 tormod    (1000) tormod    (1000)     3328 2021-05-24 11:58:52.083689 graphene-django-cud-0.9.0/PKG-INFO
--rw-r--r--   0 tormod    (1000) tormod    (1000)     2221 2021-01-18 04:19:39.000000 graphene-django-cud-0.9.0/README.md
-drwxr-xr-x   0 tormod    (1000) tormod    (1000)        0 2021-05-24 11:58:52.080356 graphene-django-cud-0.9.0/graphene_django_cud/
--rw-r--r--   0 tormod    (1000) tormod    (1000)        0 2019-05-20 19:26:55.000000 graphene-django-cud-0.9.0/graphene_django_cud/__init__.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      113 2020-05-15 08:18:06.000000 graphene-django-cud-0.9.0/graphene_django_cud/consts.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)    14870 2021-04-22 15:51:37.000000 graphene-django-cud-0.9.0/graphene_django_cud/converter.py
-drwxr-xr-x   0 tormod    (1000) tormod    (1000)        0 2021-05-24 11:58:52.083689 graphene-django-cud-0.9.0/graphene_django_cud/mutations/
--rw-r--r--   0 tormod    (1000) tormod    (1000)      801 2021-01-18 04:19:39.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/__init__.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     7646 2021-04-22 15:51:37.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/batch_create.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     4148 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/batch_delete.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      981 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/batch_patch.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     8190 2021-04-22 15:51:37.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/batch_update.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)    32419 2021-04-22 15:51:37.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/core.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     6719 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/create.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     4379 2021-05-24 10:05:09.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/delete.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     6249 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/filter_delete.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     7909 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/filter_update.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      925 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/patch.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     7106 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.0/graphene_django_cud/mutations/update.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     1195 2020-04-10 10:57:09.000000 graphene-django-cud-0.9.0/graphene_django_cud/registry.py
-drwxr-xr-x   0 tormod    (1000) tormod    (1000)        0 2021-05-24 11:58:52.083689 graphene-django-cud-0.9.0/graphene_django_cud/tests/
--rw-r--r--   0 tormod    (1000) tormod    (1000)        0 2019-05-20 19:53:50.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/__init__.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     3016 2021-05-24 10:05:09.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/factories.py
-drwxr-xr-x   0 tormod    (1000) tormod    (1000)        0 2021-05-24 11:58:52.083689 graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/
--rw-r--r--   0 tormod    (1000) tormod    (1000)     4382 2019-11-17 20:54:10.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0001_initial.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      451 2019-12-10 10:49:10.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0002_dog_tag.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      574 2019-12-10 10:49:10.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0003_dog_breed.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      543 2019-12-10 10:49:10.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0004_mouse_keeper.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      699 2020-05-15 08:18:06.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0005_dogregistration.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      379 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0006_dog_bark_count.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      342 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0007_auto_20210102_0320.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)        0 2019-10-23 08:04:35.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/__init__.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     1615 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/models.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     7410 2021-05-24 10:02:54.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/schema.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)        0 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_batch_create_mutation.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     3153 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_batch_delete_mutation.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     2196 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_batch_patch_mutation.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     2533 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_batch_update_mutation.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     4365 2021-04-22 15:51:37.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_converter.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)    21791 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_create_mutation.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     4140 2021-05-24 10:05:09.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_delete_mutation.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)        0 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_filter_delete_mutation.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     1976 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_filter_update_mutation.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)    49469 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_patch_mutation.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)    50066 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/test_update_mutation.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      184 2019-10-23 08:04:35.000000 graphene-django-cud-0.9.0/graphene_django_cud/tests/urls.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)     1569 2021-02-18 06:44:20.000000 graphene-django-cud-0.9.0/graphene_django_cud/types.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      891 2019-10-23 08:04:35.000000 graphene-django-cud-0.9.0/graphene_django_cud/urls.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)    20772 2021-05-24 10:01:34.000000 graphene-django-cud-0.9.0/graphene_django_cud/util.py
--rw-r--r--   0 tormod    (1000) tormod    (1000)      415 2019-05-20 19:26:55.000000 graphene-django-cud-0.9.0/graphene_django_cud/wsgi.py
-drwxr-xr-x   0 tormod    (1000) tormod    (1000)        0 2021-05-24 11:58:52.080356 graphene-django-cud-0.9.0/graphene_django_cud.egg-info/
--rw-r--r--   0 tormod    (1000) tormod    (1000)     3328 2021-05-24 11:58:52.000000 graphene-django-cud-0.9.0/graphene_django_cud.egg-info/PKG-INFO
--rw-r--r--   0 tormod    (1000) tormod    (1000)     2230 2021-05-24 11:58:52.000000 graphene-django-cud-0.9.0/graphene_django_cud.egg-info/SOURCES.txt
--rw-r--r--   0 tormod    (1000) tormod    (1000)        1 2021-05-24 11:58:52.000000 graphene-django-cud-0.9.0/graphene_django_cud.egg-info/dependency_links.txt
--rw-r--r--   0 tormod    (1000) tormod    (1000)       47 2021-05-24 11:58:52.000000 graphene-django-cud-0.9.0/graphene_django_cud.egg-info/requires.txt
--rw-r--r--   0 tormod    (1000) tormod    (1000)       20 2021-05-24 11:58:52.000000 graphene-django-cud-0.9.0/graphene_django_cud.egg-info/top_level.txt
--rw-r--r--   0 tormod    (1000) tormod    (1000)      478 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.0/pyproject.toml
--rw-r--r--   0 tormod    (1000) tormod    (1000)       38 2021-05-24 11:58:52.083689 graphene-django-cud-0.9.0/setup.cfg
--rw-r--r--   0 tormod    (1000) tormod    (1000)      763 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.0/setup.py
+drwxr-xr-x   0 tormodhaugland   (501) staff       (20)        0 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     3328 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/PKG-INFO
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     1054 2019-10-23 08:04:35.000000 graphene-django-cud-0.9.1/LICENSE.md
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      478 2021-12-29 17:59:21.000000 graphene-django-cud-0.9.1/pyproject.toml
+drwxr-xr-x   0 tormodhaugland   (501) staff       (20)        0 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/graphene_django_cud.egg-info/
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     3328 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/graphene_django_cud.egg-info/PKG-INFO
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     2230 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/graphene_django_cud.egg-info/SOURCES.txt
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)       47 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/graphene_django_cud.egg-info/requires.txt
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)       20 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/graphene_django_cud.egg-info/top_level.txt
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)        1 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/graphene_django_cud.egg-info/dependency_links.txt
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     2221 2021-01-18 04:19:39.000000 graphene-django-cud-0.9.1/README.md
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      763 2021-12-29 17:57:10.000000 graphene-django-cud-0.9.1/setup.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)       38 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/setup.cfg
+drwxr-xr-x   0 tormodhaugland   (501) staff       (20)        0 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/graphene_django_cud/
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     1195 2020-04-10 10:57:09.000000 graphene-django-cud-0.9.1/graphene_django_cud/registry.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)    20772 2021-05-24 10:01:34.000000 graphene-django-cud-0.9.1/graphene_django_cud/util.py
+drwxr-xr-x   0 tormodhaugland   (501) staff       (20)        0 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     7154 2021-12-29 17:57:01.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/update.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     4379 2021-05-24 10:05:09.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/delete.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      925 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/patch.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     8190 2021-04-22 15:51:37.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/batch_update.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     4148 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/batch_delete.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     7646 2021-04-22 15:51:37.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/batch_create.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     6719 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/create.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      801 2021-01-18 04:19:39.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/__init__.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)    32419 2021-04-22 15:51:37.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/core.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     6249 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/filter_delete.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     7909 2021-05-24 11:58:04.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/filter_update.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      981 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.1/graphene_django_cud/mutations/batch_patch.py
+drwxr-xr-x   0 tormodhaugland   (501) staff       (20)        0 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/
+drwxr-xr-x   0 tormodhaugland   (501) staff       (20)        0 2021-12-29 18:36:35.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      574 2019-12-10 10:49:10.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0003_dog_breed.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      451 2019-12-10 10:49:10.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0002_dog_tag.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      699 2020-05-15 08:18:06.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0005_dogregistration.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      342 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0007_auto_20210102_0320.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)        0 2019-10-23 08:04:35.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/__init__.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      543 2019-12-10 10:49:10.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0004_mouse_keeper.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     4382 2019-11-17 20:54:10.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0001_initial.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      379 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0006_dog_bark_count.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     2196 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_batch_patch_mutation.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     1976 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_filter_update_mutation.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     1615 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/models.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)    49469 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_patch_mutation.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)        0 2019-05-20 19:53:50.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/__init__.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)        0 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_filter_delete_mutation.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     3016 2021-05-24 10:05:09.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/factories.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     4140 2021-05-24 10:05:09.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_delete_mutation.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     3153 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_batch_delete_mutation.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)    21791 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_create_mutation.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)        0 2021-01-02 18:01:19.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_batch_create_mutation.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     4365 2021-04-22 15:51:37.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_converter.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)    50066 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_update_mutation.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      184 2019-10-23 08:04:35.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/urls.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     2533 2021-02-01 19:50:07.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/test_batch_update_mutation.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     7410 2021-05-24 10:02:54.000000 graphene-django-cud-0.9.1/graphene_django_cud/tests/schema.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)    14870 2021-04-22 15:51:37.000000 graphene-django-cud-0.9.1/graphene_django_cud/converter.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)        0 2019-05-20 19:26:55.000000 graphene-django-cud-0.9.1/graphene_django_cud/__init__.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)     1569 2021-02-18 06:44:20.000000 graphene-django-cud-0.9.1/graphene_django_cud/types.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      113 2020-05-15 08:18:06.000000 graphene-django-cud-0.9.1/graphene_django_cud/consts.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      891 2019-10-23 08:04:35.000000 graphene-django-cud-0.9.1/graphene_django_cud/urls.py
+-rw-r--r--   0 tormodhaugland   (501) staff       (20)      415 2019-05-20 19:26:55.000000 graphene-django-cud-0.9.1/graphene_django_cud/wsgi.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `graphene-django-cud-0.9.0/LICENSE.md` & `graphene-django-cud-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/PKG-INFO` & `graphene-django-cud-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-cud
-Version: 0.9.0
+Version: 0.9.1
 Summary: Create, update and delete mutations for graphene-django
 Home-page: https://github.com/tOgg1/graphene-django-cud
 Author: Tormod Haugland
 Author-email: tormod.haugland@gmail.com
 License: UNKNOWN
 Description: # Graphene Django CUD
```

### Comparing `graphene-django-cud-0.9.0/README.md` & `graphene-django-cud-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/converter.py` & `graphene-django-cud-0.9.1/graphene_django_cud/converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/__init__.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/batch_create.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/batch_create.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/batch_delete.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/batch_delete.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/batch_patch.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/batch_patch.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/batch_update.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/batch_update.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/core.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/core.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/create.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/create.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/delete.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/delete.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/filter_delete.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/filter_delete.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/filter_update.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/filter_update.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/patch.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/patch.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/mutations/update.py` & `graphene-django-cud-0.9.1/graphene_django_cud/mutations/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,26 +173,26 @@
         updated_input = cls.before_mutate(root, info, input, id)
         if updated_input:
             input = updated_input
 
         if cls._meta.login_required and not info.context.user.is_authenticated:
             raise GraphQLError("Must be logged in to access this mutation.")
 
+        with transaction.atomic():
 
-        id = cls.resolve_id(id)
-        Model = cls._meta.model
-        queryset = cls.get_queryset(root, info, input, id)
-        obj = queryset.get(pk=id)
-        auto_context_fields = cls._meta.auto_context_fields or {}
+            id = cls.resolve_id(id)
+            Model = cls._meta.model
+            queryset = cls.get_queryset(root, info, input, id)
+            obj = queryset.select_for_update().get(pk=id)
+            auto_context_fields = cls._meta.auto_context_fields or {}
 
-        cls.check_permissions(root, info, input, id, obj)
+            cls.check_permissions(root, info, input, id, obj)
 
-        cls.validate(root, info, input, id, obj)
+            cls.validate(root, info, input, id, obj)
 
-        with transaction.atomic():
             obj = cls.update_obj(
                 obj,
                 input,
                 info,
                 auto_context_fields,
                 cls._meta.many_to_many_extras,
                 cls._meta.foreign_key_extras,
```

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/registry.py` & `graphene-django-cud-0.9.1/graphene_django_cud/registry.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/factories.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/factories.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0001_initial.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0003_dog_breed.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0003_dog_breed.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0004_mouse_keeper.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0004_mouse_keeper.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/migrations/0005_dogregistration.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/migrations/0005_dogregistration.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/models.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/models.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/schema.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/test_batch_delete_mutation.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/test_batch_delete_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/test_batch_patch_mutation.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/test_batch_patch_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/test_batch_update_mutation.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/test_batch_update_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/test_converter.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/test_create_mutation.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/test_create_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/test_delete_mutation.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/test_delete_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/test_filter_update_mutation.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/test_filter_update_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/test_patch_mutation.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/test_patch_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/tests/test_update_mutation.py` & `graphene-django-cud-0.9.1/graphene_django_cud/tests/test_update_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/types.py` & `graphene-django-cud-0.9.1/graphene_django_cud/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/urls.py` & `graphene-django-cud-0.9.1/graphene_django_cud/urls.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud/util.py` & `graphene-django-cud-0.9.1/graphene_django_cud/util.py`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud.egg-info/PKG-INFO` & `graphene-django-cud-0.9.1/graphene_django_cud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-cud
-Version: 0.9.0
+Version: 0.9.1
 Summary: Create, update and delete mutations for graphene-django
 Home-page: https://github.com/tOgg1/graphene-django-cud
 Author: Tormod Haugland
 Author-email: tormod.haugland@gmail.com
 License: UNKNOWN
 Description: # Graphene Django CUD
```

### Comparing `graphene-django-cud-0.9.0/graphene_django_cud.egg-info/SOURCES.txt` & `graphene-django-cud-0.9.1/graphene_django_cud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphene-django-cud-0.9.0/setup.py` & `graphene-django-cud-0.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="graphene-django-cud",
-    version="0.9.0",
+    version="0.9.1",
     author="Tormod Haugland",
     author_email="tormod.haugland@gmail.com",
     description="Create, update and delete mutations for graphene-django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tOgg1/graphene-django-cud",
     packages=setuptools.find_packages(),
```

