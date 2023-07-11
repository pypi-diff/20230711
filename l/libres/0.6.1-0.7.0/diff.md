# Comparing `tmp/libres-0.6.1.tar.gz` & `tmp/libres-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libres-0.6.1.tar", last modified: Wed Mar 29 11:44:06 2023, max compression
+gzip compressed data, was "libres-0.7.0.tar", last modified: Tue Jul 11 10:00:45 2023, max compression
```

## Comparing `libres-0.6.1.tar` & `libres-0.7.0.tar`

### file list

```diff
@@ -1,75 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.354101 libres-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-03-29 11:43:55.000000 libres-0.6.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-29 11:43:55.000000 libres-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-29 11:43:55.000000 libres-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-03-29 11:44:06.350101 libres-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-29 11:43:55.000000 libres-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.346101 libres-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-03-29 11:43:55.000000 libres-0.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.346101 libres-0.6.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-29 11:43:55.000000 libres-0.6.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    31729 2023-03-29 11:43:55.000000 libres-0.6.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-03-29 11:43:55.000000 libres-0.6.1/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-29 11:43:55.000000 libres-0.6.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-03-29 11:43:55.000000 libres-0.6.1/docs/concepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-03-29 11:43:55.000000 libres-0.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-29 11:43:55.000000 libres-0.6.1/docs/customizations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-29 11:43:55.000000 libres-0.6.1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-03-29 11:43:55.000000 libres-0.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-29 11:43:55.000000 libres-0.6.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-29 11:43:55.000000 libres-0.6.1/docs/under_the_hood.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.346101 libres-0.6.1/libres/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-29 11:43:55.000000 libres-0.6.1/libres/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-29 11:43:55.000000 libres-0.6.1/libres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.350101 libres-0.6.1/libres/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 11:43:55.000000 libres-0.6.1/libres/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-03-29 11:43:55.000000 libres-0.6.1/libres/context/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-29 11:43:55.000000 libres-0.6.1/libres/context/exposure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-03-29 11:43:55.000000 libres-0.6.1/libres/context/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-29 11:43:55.000000 libres-0.6.1/libres/context/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-29 11:43:55.000000 libres-0.6.1/libres/context/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.350101 libres-0.6.1/libres/db/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.350101 libres-0.6.1/libres/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24705 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/reserved_slot.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.350101 libres-0.6.1/libres/db/models/types/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/types/json_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/types/utcdatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/models/types/uuid_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    56463 2023-03-29 11:43:55.000000 libres-0.6.1/libres/db/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.350101 libres-0.6.1/libres/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-29 11:43:55.000000 libres-0.6.1/libres/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-29 11:43:55.000000 libres-0.6.1/libres/modules/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-29 11:43:55.000000 libres-0.6.1/libres/modules/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-03-29 11:43:55.000000 libres-0.6.1/libres/modules/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-03-29 11:43:55.000000 libres-0.6.1/libres/modules/rasterizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-29 11:43:55.000000 libres-0.6.1/libres/modules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.350101 libres-0.6.1/libres/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13563 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/test_allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/test_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/test_reserved_slot.py
--rw-r--r--   0 runner    (1001) docker     (123)    68024 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-29 11:43:55.000000 libres-0.6.1/libres/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:44:06.350101 libres-0.6.1/libres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-03-29 11:44:06.000000 libres-0.6.1/libres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-29 11:44:06.000000 libres-0.6.1/libres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 11:44:06.000000 libres-0.6.1/libres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 11:44:06.000000 libres-0.6.1/libres.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-29 11:44:06.000000 libres-0.6.1/libres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-29 11:44:06.000000 libres-0.6.1/libres.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 11:44:06.354101 libres-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-29 11:43:55.000000 libres-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.276064 libres-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-11 10:00:30.000000 libres-0.7.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 10:00:30.000000 libres-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-11 10:00:30.000000 libres-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-07-11 10:00:45.276064 libres-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-11 10:00:30.000000 libres-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.272064 libres-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-11 10:00:30.000000 libres-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.272064 libres-0.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-11 10:00:30.000000 libres-0.7.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    31729 2023-07-11 10:00:30.000000 libres-0.7.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-11 10:00:30.000000 libres-0.7.0/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-11 10:00:30.000000 libres-0.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-11 10:00:30.000000 libres-0.7.0/docs/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-11 10:00:30.000000 libres-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-11 10:00:30.000000 libres-0.7.0/docs/customizations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-11 10:00:30.000000 libres-0.7.0/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-11 10:00:30.000000 libres-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 10:00:30.000000 libres-0.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-11 10:00:30.000000 libres-0.7.0/docs/under_the_hood.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-11 10:00:30.000000 libres-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 10:00:45.276064 libres-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.268064 libres-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.272064 libres-0.7.0/src/libres/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.272064 libres-0.7.0/src/libres/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/context/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/context/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/context/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/context/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/context/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.272064 libres-0.7.0/src/libres/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.276064 libres-0.7.0/src/libres/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28675 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/reserved_slot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.276064 libres-0.7.0/src/libres/db/models/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/types/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/types/utcdatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/models/types/uuid_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64510 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/db/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.276064 libres-0.7.0/src/libres/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/modules/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/modules/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/modules/rasterizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:30.000000 libres-0.7.0/src/libres/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.272064 libres-0.7.0/src/libres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-07-11 10:00:45.000000 libres-0.7.0/src/libres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-11 10:00:45.000000 libres-0.7.0/src/libres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:00:45.000000 libres-0.7.0/src/libres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:00:45.000000 libres-0.7.0/src/libres.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-11 10:00:45.000000 libres-0.7.0/src/libres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 10:00:45.000000 libres-0.7.0/src/libres.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:00:45.276064 libres-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13563 2023-07-11 10:00:30.000000 libres-0.7.0/tests/test_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-11 10:00:30.000000 libres-0.7.0/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-11 10:00:30.000000 libres-0.7.0/tests/test_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-11 10:00:30.000000 libres-0.7.0/tests/test_reserved_slot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68359 2023-07-11 10:00:30.000000 libres-0.7.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-11 10:00:30.000000 libres-0.7.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-11 10:00:30.000000 libres-0.7.0/tests/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-11 10:00:30.000000 libres-0.7.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-11 10:00:30.000000 libres-0.7.0/tests/test_utils.py
```

### Comparing `libres-0.6.1/HISTORY.rst` & `libres-0.7.0/HISTORY.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,32 @@
 Changelog
 ---------
 
+0.7.0 (2023-07-11)
+~~~~~~~~~~~~~~~~~~~
+
+- Drops support for Python 3.7 and adds support for 3.11
+  [Daverball]
+
+- Switches to ``pyproject.toml``
+  [Daverball]
+
+- Adds type annotations
+  [Daverball]
+
+- Changes ``Scheduler.allocate`` to avoid hundreds of separate
+  SQL queries when passing in hundreds of datetime ranges in
+  order to identify existing overlapping allocations.
+
+  Performance could still be a concern, since the query contains
+  a lot of datetime comparisons. It might be quicker in the common case to filter to the minimum and maximum dates that
+  have been passed in and doing the overlap checks entirely in
+  Python. We will need to keep an eye on this.
+  [Daverball]
+
 0.6.1 (2023-03-29)
 ~~~~~~~~~~~~~~~~~~~
 
 - Adds additional parameters to ``Scheduler.remove_unused allocations``
   to filter the to be removed Allocations by weekday or
   whether or not they belong to a group.
   [Daverball]
```

### Comparing `libres-0.6.1/LICENSE` & `libres-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/PKG-INFO` & `libres-0.7.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: libres
-Version: 0.6.1
+Version: 0.7.0
 Summary: A library to reserve things
 Home-page: http://github.com/seantis/libres/
 Author: Denis Krienbühl
 Author-email: denis@href.ch
+Maintainer: Seantis GmbH
+Maintainer-email: info@seantis.ch
 License: BSD
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: mypy
 License-File: LICENSE
 
 Libres
 ======
 
 Libres is a reservations management library to reserve things like tables at
-a restaurant or tickets at an event. It works with Python 3.7+
+a restaurant or tickets at an event. It works with Python 3.8+
 and requires Postgresql 9.1+.
 
 `Documentation <http://libres.readthedocs.org/en/latest/>`_ | `Source <http://github.com/seantis/libres/>`_ | `Bugs <http://github.com/seantis/libres/issues>`_
 
 **This library is at an experimental stage and not yet suitable for production**
 
 .. image:: https://github.com/seantis/libres/actions/workflows/python-tox.yaml/badge.svg
@@ -36,17 +45,102 @@
   :target: https://codecov.io/gh/seantis/libres
   :alt:    Coverage
 
 .. image:: https://img.shields.io/pypi/v/libres.svg
   :target: https://pypi.python.org/pypi/libres
   :alt:    Release
 
+.. < package description
+
+Run the Example
+---------------
+
+Go to examples/flask and install the requirements::
+
+    cd examples/flask
+    pip install -r requirements.txt
+
+Run the example::
+
+    python run.py
+
+Open http://localhost:5000 and click around.
+
+Run the Tests
+-------------
+
+Install tox and run it::
+
+    pip install tox
+    tox
+
+Limit the tests to a specific python version::
+
+    tox -e py27
+
+Conventions
+-----------
+
+Libres follows PEP8 as close as possible. To test for it run::
+
+    tox -e pep8
+
+Libres uses `Semantic Versioning <http://semver.org/>`_
+
+Build the Docs
+--------------
+
+Go to docs and install the requirements::
+
+    cd docs
+    pip install -r requirements.txt
+
+Build the docs::
+
+    make html
+
+Open the docs::
+
+    open build/html/index.html
+
+Making a new Release
+--------------------
+
+Make sure all changes are in the HISTORY.rst, then bump the version::
+
+    bump2version major|minor|patch
+    git push && git push --tags
+
+After this, create a new release on Github.
+
 Changelog
 ---------
 
+0.7.0 (2023-07-11)
+~~~~~~~~~~~~~~~~~~~
+
+- Drops support for Python 3.7 and adds support for 3.11
+  [Daverball]
+
+- Switches to ``pyproject.toml``
+  [Daverball]
+
+- Adds type annotations
+  [Daverball]
+
+- Changes ``Scheduler.allocate`` to avoid hundreds of separate
+  SQL queries when passing in hundreds of datetime ranges in
+  order to identify existing overlapping allocations.
+
+  Performance could still be a concern, since the query contains
+  a lot of datetime comparisons. It might be quicker in the common case to filter to the minimum and maximum dates that
+  have been passed in and doing the overlap checks entirely in
+  Python. We will need to keep an eye on this.
+  [Daverball]
+
 0.6.1 (2023-03-29)
 ~~~~~~~~~~~~~~~~~~~
 
 - Adds additional parameters to ``Scheduler.remove_unused allocations``
   to filter the to be removed Allocations by weekday or
   whether or not they belong to a group.
   [Daverball]
```

### Comparing `libres-0.6.1/README.rst` & `libres-0.7.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Libres
 ======
 
 Libres is a reservations management library to reserve things like tables at
-a restaurant or tickets at an event. It works with Python 3.7+
+a restaurant or tickets at an event. It works with Python 3.8+
 and requires Postgresql 9.1+.
 
 `Documentation <http://libres.readthedocs.org/en/latest/>`_ | `Source <http://github.com/seantis/libres/>`_ | `Bugs <http://github.com/seantis/libres/issues>`_
 
 **This library is at an experimental stage and not yet suitable for production**
 
 .. image:: https://github.com/seantis/libres/actions/workflows/python-tox.yaml/badge.svg
```

### Comparing `libres-0.6.1/docs/Makefile` & `libres-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/docs/_static/custom.css` & `libres-0.7.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/docs/_static/favicon.ico` & `libres-0.7.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/docs/_static/logo.svg` & `libres-0.7.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/docs/api.rst` & `libres-0.7.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/docs/concepts.rst` & `libres-0.7.0/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/docs/conf.py` & `libres-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/docs/customizations.rst` & `libres-0.7.0/docs/customizations.rst`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/docs/faq.rst` & `libres-0.7.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/docs/index.rst` & `libres-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/docs/under_the_hood.rst` & `libres-0.7.0/docs/under_the_hood.rst`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/libres/context/core.py` & `libres-0.7.0/src/libres/context/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,75 @@
+import enum
 import libres
 import threading
 
-from cached_property import cached_property
 from contextlib import contextmanager
+from functools import cached_property
+
 from libres.modules import errors
 
 
-missing = object()
-required = object()
+import typing as _t
+if _t.TYPE_CHECKING:
+    from sqlalchemy.orm import Session
+    from sqlalchemy.orm.session import SessionTransaction
+    from uuid import UUID
+
+    from libres.context.registry import Registry
+    from libres.context.session import SessionProvider
+    from libres.db.models import Allocation
+
+
+class _Marker(enum.Enum):
+    missing = enum.auto()
+    required = enum.auto()
 
 
-class StoppableService(object):
+missing_t = _t.Literal[_Marker.missing]
+required_t = _t.Literal[_Marker.required]
+missing: missing_t = _Marker.missing
+required: required_t = _Marker.required
+
+
+class StoppableService:
     """ Services inheriting from this class have their stop_service method
     called when the service is discarded.
 
     Note that this only happens when a service is replaced with a new one
     and not when libres is stopped (i.e. this is *not* a deconstructor).
 
     """
 
-    def stop_service(self):
+    def stop_service(self) -> None:
         pass
 
 
-class ContextServicesMixin(object):
+class ContextServicesMixin:
     """ Provides access methods to the context's services. Expects
     the class that uses the mixin to provide self.context.
 
     The results are cached for performance.
 
     """
 
+    context: 'Context'
+
     @cached_property
-    def is_allocation_exposed(self):
+    def is_allocation_exposed(self) -> _t.Callable[['Allocation'], bool]:
         return self.context.get_service('exposure').is_allocation_exposed
 
     @cached_property
-    def generate_uuid(self):
+    def generate_uuid(self) -> _t.Callable[[str], 'UUID']:
         return self.context.get_service('uuid_generator')
 
     @cached_property
-    def validate_email(self):
+    def validate_email(self) -> _t.Callable[[str], bool]:
         return self.context.get_service('email_validator')
 
-    def clear_cache(self):
+    def clear_cache(self) -> None:
         """ Clears the cache of the mixin. """
 
         try:
             del self.is_allocation_exposed
         except AttributeError:
             pass
 
@@ -58,38 +80,38 @@
 
         try:
             del self.validate_email
         except AttributeError:
             pass
 
     @property
-    def session_provider(self):
+    def session_provider(self) -> 'SessionProvider':
         return self.context.get_service('session_provider')
 
     @property
-    def session(self):
+    def session(self) -> 'Session':
         """ Returns the current session. """
         return self.session_provider.session()
 
-    def close(self):
+    def close(self) -> None:
         """ Closes the current session. """
         self.session.close()
 
     @property
-    def begin_nested(self):
+    def begin_nested(self) -> _t.Callable[[], 'SessionTransaction']:
         return self.session.begin_nested
 
-    def commit(self):
-        return self.session.commit()
+    def commit(self) -> None:
+        self.session.commit()
 
-    def rollback(self):
-        return self.session.rollback()
+    def rollback(self) -> None:
+        self.session.rollback()
 
 
-class Context(object):
+class Context:
     """ Used throughout Libres, the context holds settings like the database
     connection string and services like the json dumps/loads functions that
     should be used.
 
     Contexts allow consumers of the Libres library to override these settings /
     services as they wish. It also makes sure that multiple consumers of Libres
     can co-exist in a single process, as each consumer must operate on it's
@@ -114,71 +136,77 @@
         from libres import registry
         my_context = registry.register_context('my_app')
 
     See also :class:`~libres.context.registry.Registry`
 
     """
 
-    def __init__(self, name, registry=None, parent=None, locked=False):
+    def __init__(
+        self,
+        name: str,
+        registry: _t.Optional['Registry'] = None,
+        parent: _t.Optional['Context'] = None,
+        locked: bool = False
+    ):
         self.name = name
         self.registry = registry or libres.registry
-        self.values = {}
+        self.values: _t.Dict[str, _t.Any] = {}
         self.parent = parent
         self.locked = False
         self.thread_lock = threading.RLock()
 
-    def __repr__(self):
-        return "<Libres Context(name='{}')>".format(self.name)
+    def __repr__(self) -> str:
+        return f"<Libres Context(name='{self.name}')>"
 
     @contextmanager
-    def as_current_context(self):
+    def as_current_context(self) -> _t.Iterator[None]:
         with self.registry.context(self.name):
             yield
 
-    def switch_to(self):
+    def switch_to(self) -> None:
         self.registry.switch_context(self.name)
 
-    def lock(self):
+    def lock(self) -> None:
         with self.thread_lock:
             self.locked = True
 
-    def unlock(self):
+    def unlock(self) -> None:
         with self.thread_lock:
             self.locked = False
 
-    def get(self, key):
+    def get(self, key: str) -> _t.Union[_t.Any, missing_t]:
         if key in self.values:
             return self.values[key]
         elif self.parent:
             return self.parent.get(key)
         else:
             return missing
 
-    def set(self, key, value):
+    def set(self, key: str, value: _t.Any) -> None:
         if self.locked:
             raise errors.ContextIsLocked
 
         with self.thread_lock:
 
             # If a value already exists it could be a stoppable service.
             # Stoppable services are called before they are stop so they
             # can clean up after themselves without having to wait for the GC.
             if isinstance(self.values.get(key), StoppableService):
                 self.values[key].stop_service()
 
             self.values[key] = value
 
-    def get_setting(self, name):
-        return self.get('settings.{}'.format(name))
+    def get_setting(self, name: str) -> _t.Any:
+        return self.get(f'settings.{name}')
 
-    def set_setting(self, name, value):
+    def set_setting(self, name: str, value: _t.Any) -> None:
         with self.thread_lock:
-            self.set('settings.{}'.format(name), value)
+            self.set(f'settings.{name}', value)
 
-    def get_service(self, name):
+    def get_service(self, name: str) -> _t.Any:
         service_id = '/'.join(('service', name))
         service = self.get(service_id)
 
         if service is missing:
             raise errors.UnknownService(service_id)
 
         cache_id = '/'.join(('service', name, 'cache'))
@@ -191,15 +219,20 @@
             # first call, cache it!
             if cache is required:
                 self.set(cache_id, service(self))
 
             # nth call, use cached value
             return self.get(cache_id)
 
-    def set_service(self, name, factory, cache=False):
+    def set_service(
+        self,
+        name: str,
+        factory: _t.Callable[..., _t.Any],
+        cache: bool = False
+    ) -> None:
         with self.thread_lock:
             service_id = '/'.join(('service', name))
             self.set(service_id, factory)
 
             if cache:
                 cache_id = '/'.join(('service', name, 'cache'))
                 self.set(cache_id, required)
```

### Comparing `libres-0.6.1/libres/context/registry.py` & `libres-0.7.0/src/libres/context/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,64 +2,70 @@
 
 from contextlib import contextmanager
 
 from libres.modules import errors
 from libres.context.core import Context
 
 
-def create_default_registry():
+import typing as _t
+if _t.TYPE_CHECKING:
+    from uuid import UUID
+
+
+def create_default_registry() -> 'Registry':
     """ Creates the default registry for libres. """
 
     import re
 
     from libres.context.registry import Registry
     from libres.context.session import SessionProvider
     from libres.context.settings import set_default_settings
     from libres.context.exposure import Exposure
 
     from uuid import uuid5 as new_namespace_uuid
 
     registry = Registry()
 
-    def session_provider(context):
+    def session_provider(context: Context) -> SessionProvider:
         return SessionProvider(context.get_setting('dsn'))
 
-    def email_validator_factory(context):
+    def email_validator_factory(context: Context) -> _t.Callable[[str], bool]:
         # A very simple and stupid email validator. It's way too simple, but
         # it can be extended to do more powerful checks.
-        def is_valid_email(email):
-            return re.match(r'[^@]+@[^@]+\.[^@]+', email)
+        def is_valid_email(email: str) -> bool:
+            return bool(re.match(r'[^@]+@[^@]+\.[^@]+', email))
 
         return is_valid_email
 
-    def exposure_factory(context):
+    def exposure_factory(context: Context) -> Exposure:
         return Exposure()
 
-    def uuid_generator_factory(context):
-        def uuid_generator(name):
+    def uuid_generator_factory(context: Context) -> _t.Callable[[str], 'UUID']:
+        def uuid_generator(name: str) -> 'UUID':
             return new_namespace_uuid(
                 context.get_setting('uuid_namespace'),
                 '/'.join((context.name, name))
             )
         return uuid_generator
 
     master = registry.master_context
+    assert master is not None
     master.set_service('email_validator', email_validator_factory)
     master.set_service('session_provider', session_provider, cache=True)
     master.set_service('exposure', exposure_factory)
     master.set_service('uuid_generator', uuid_generator_factory)
 
     set_default_settings(master)
 
     master.lock()
 
     return registry
 
 
-class Registry(object):
+class Registry:
     """ Holds a number of contexts, managing their creation and defining
     the currently active context.
 
     A global registry instance is found in libres::
 
         from libres import registry
 
@@ -67,48 +73,49 @@
     your own version of the registry::
 
         from libres.context.registry import create_default_registry
         registry = create_default_registry()
 
     """
 
-    master_context = None
+    contexts: _t.Dict[str, Context]
+    master_context: _t.Optional[Context] = None
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.thread_lock = threading.RLock()
 
         with self.thread_lock:
             self.contexts = {}
             self.local = threading.local()
 
         self.master_context = self.register_context('master')
 
     @property
-    def current_context(self):
+    def current_context(self) -> Context:
         if not hasattr(self.local, 'current_context'):
             self.local.current_context = self.master_context
 
         return self.local.current_context
 
-    def is_existing_context(self, name):
+    def is_existing_context(self, name: str) -> bool:
         return name in self.contexts
 
-    def assert_not_locked(self, name):
+    def assert_not_locked(self, name: str) -> None:
         if self.get_context(name).locked:
             raise errors.ContextIsLocked
 
-    def assert_exists(self, name):
+    def assert_exists(self, name: str) -> None:
         if not self.is_existing_context(name):
             raise errors.UnknownContext
 
-    def assert_does_not_exist(self, name):
+    def assert_does_not_exist(self, name: str) -> None:
         if self.is_existing_context(name):
             raise errors.ContextAlreadyExists
 
-    def register_context(self, name, replace=False):
+    def register_context(self, name: str, replace: bool = False) -> Context:
         """ Registers a new context with the given name and returns it.
 
         """
         with self.thread_lock:
             if replace:
                 if self.is_existing_context(name):
                     self.assert_not_locked(name)
@@ -120,29 +127,29 @@
                 registry=self,
                 parent=self.master_context,
                 locked=False
             )
 
             return self.contexts[name]
 
-    def switch_context(self, name):
+    def switch_context(self, name: str) -> None:
         with self.thread_lock:
             self.assert_exists(name)
             self.local.current_context = self.get_context(name)
 
     @contextmanager
-    def context(self, name):
+    def context(self, name: str) -> _t.Iterator[Context]:
         previous = self.current_context.name
         self.switch_context(name)
         yield self.current_context
         self.switch_context(previous)
 
-    def get_current_context(self):
+    def get_current_context(self) -> Context:
         return self.current_context
 
-    def get_context(self, name, autocreate=False):
+    def get_context(self, name: str, autocreate: bool = False) -> Context:
         if not autocreate:
             self.assert_exists(name)
         elif not self.is_existing_context(name):
             self.register_context(name)
 
         return self.contexts[name]
```

### Comparing `libres-0.6.1/libres/context/session.py` & `libres-0.7.0/src/libres/context/session.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 from sqlalchemy import create_engine
 from sqlalchemy.pool import QueuePool
 from sqlalchemy.orm import scoped_session, sessionmaker
 
 from libres.context.core import StoppableService
 
 
+import typing as _t
+
+
 SERIALIZABLE = 'SERIALIZABLE'
 
 
 class SessionProvider(StoppableService):
     """Global session utility. It provides a SERIALIZABLE session to libres.
     If you want to override this provider, be sure to set the isolation_level
     to SERIALIZABLE as well.
 
     If you don't do that, libres might run into errors as it assumes and tests
     against SERIALIZABLE connections!
 
     """
 
-    def __init__(self, dsn, engine_config={}, session_config={}):
+    def __init__(
+        self,
+        dsn: str,
+        engine_config: _t.Optional[_t.Dict[str, _t.Any]] = None,
+        session_config: _t.Optional[_t.Dict[str, _t.Any]] = None
+    ):
         self.assert_valid_postgres_version(dsn)
         self.dsn = dsn
 
         self.engine = create_engine(
             dsn, poolclass=QueuePool, pool_size=5, max_overflow=5,
             isolation_level=SERIALIZABLE,
-            **engine_config
+            **(engine_config or {})
         )
 
         self.session = scoped_session(sessionmaker(
-            bind=self.engine, **session_config
+            bind=self.engine, **(session_config or {})
         ))
 
-    def stop_service(self):
+    def stop_service(self) -> None:
         """ Called by the libres context when the session provider is being
         discarded (only in testing).
 
         This makes sure that replacing the session provider on the context
         doesn't leave behind any idle connections.
 
         """
 
         self.session().close()
         self.engine.raw_connection().invalidate()
         self.engine.dispose()
 
-    def get_postgres_version(self, dsn):
+    def get_postgres_version(self, dsn: str) -> _t.Tuple[str, int]:
         """ Returns the postgres version as a tuple (string, integer).
 
         Uses it's own connection to be independent from any session.
 
         """
         assert 'postgres' in dsn, "Not a postgres database"
 
@@ -57,19 +65,21 @@
             SELECT current_setting('server_version'),
                    current_setting('server_version_num')
         """
 
         engine = create_engine(dsn)
 
         try:
-            version, number = engine.execute(query).first()
+            result = engine.execute(query).first()
+            assert result is not None
+            version, number = result
             return version, int(number)
         finally:
             engine.dispose()
 
-    def assert_valid_postgres_version(self, dsn):
+    def assert_valid_postgres_version(self, dsn: str) -> str:
         v, n = self.get_postgres_version(dsn)
 
         if n < 90100:
-            raise RuntimeError("PostgreSQL 9.1+ is required, got {}".format(v))
+            raise RuntimeError(f"PostgreSQL 9.1+ is required, got {v}")
 
         return dsn
```

### Comparing `libres-0.6.1/libres/context/settings.py` & `libres-0.7.0/src/libres/context/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import textwrap
 from uuid import UUID
 
 
-_default = {}
+import typing as _t
+if _t.TYPE_CHECKING:
+    from libres.context.core import Context
+
+
+_default: _t.Dict[str, _t.Tuple[_t.Any, str]] = {}
 
 _default['settings.dsn'] = (
     None,
     """
     The data source name to connect to the right database. For example:
     postgresql+psycopg2://user:password@localhost:5432/database
     """
@@ -22,24 +27,24 @@
     the specific record in the database.
 
     Just leave it really.
     """
 )
 
 
-def set_default_settings(context):
-    for name, (value, help) in _default.items():
+def set_default_settings(context: 'Context') -> None:
+    for name, (value, _) in _default.items():
         context.set(name, value)
 
 
 doc = []
 
 
-for name, (value, help) in _default.items():
-    reference = '.. _{name}:\n'.format(name=name)
+for name, (value, help_str) in _default.items():
+    reference = f'.. _{name}:\n'
     title = '{name}\n{line}'.format(name=name, line='-' * len(name))
-    default = 'default: **{value}**'.format(value=repr(value))
-    help = textwrap.dedent(help)
+    default = f'default: **{repr(value)}**'
+    help_str = textwrap.dedent(help_str)
 
-    doc.append('\n'.join((reference, title, default, help)))
+    doc.append('\n'.join((reference, title, default, help_str)))
 
 __doc__ = '\n'.join(doc)
```

### Comparing `libres-0.6.1/libres/db/models/allocation.py` & `libres-0.7.0/src/libres/db/models/allocation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 import sedate
 
-from datetime import timedelta, time
+from datetime import datetime, timedelta, time
 from itertools import groupby
-
 from sqlalchemy import types
+from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.schema import Column
 from sqlalchemy.schema import Index
 from sqlalchemy.schema import UniqueConstraint
 from sqlalchemy.orm import object_session
 from sqlalchemy.orm.util import has_identity
 
+from libres.db.models import ORMBase
+from libres.db.models.types import UUID, UTCDateTime, JSON
+from libres.db.models.other import OtherModels
+from libres.db.models.timestamp import TimestampMixin
 from libres.modules import utils
 from libres.modules.rasterizer import (
     rasterize_start,
     rasterize_span,
     rasterize_end,
     iterate_span,
     MIN_RASTER
 )
 
-from libres.db.models import ORMBase
-from libres.db.models.types import UUID, UTCDateTime, JSON
-from libres.db.models.other import OtherModels
-from libres.db.models.timestamp import TimestampMixin
-from sqlalchemy.ext.hybrid import hybrid_property
+
+import typing as _t
+if _t.TYPE_CHECKING:
+    import uuid
+    from sedate.types import TzInfoOrName
+    from sqlalchemy.orm import Query
+    from typing_extensions import Self
+
+    from libres.db.models import Reservation, ReservedSlot
+    from libres.modules.rasterizer import Raster
+
+    _OptDT1 = _t.TypeVar('_OptDT1', _t.Optional[datetime], datetime, None)
+    _OptDT2 = _t.TypeVar('_OptDT2', _t.Optional[datetime], datetime, None)
 
 
 class Allocation(TimestampMixin, ORMBase, OtherModels):
     """Describes a timespan within which one or many timeslots can be
     reserved.
 
     There's an important concept to understand before working with allocations.
@@ -47,76 +59,101 @@
     :class:`.scheduler.Scheduler` class.
 
     """
 
     __tablename__ = 'allocations'
 
     #: the id of the allocation, autoincremented
-    id = Column(types.Integer(), primary_key=True, autoincrement=True)
+    id: 'Column[int]' = Column(
+        types.Integer(),
+        primary_key=True,
+        autoincrement=True
+    )
 
     #: the resource uuid of the allocation, may not be an actual resource
     #: see :class:`.models.Allocation` for more information
-    resource = Column(UUID(), nullable=False)
+    resource: 'Column[uuid.UUID]' = Column(UUID(), nullable=False)
 
     #: the polymorphic type of the allocation
-    type = Column(types.Text(), nullable=True)
+    type: 'Column[_t.Optional[str]]' = Column(types.Text(), nullable=True)
 
     #: resource of which this allocation is a mirror. If the mirror_of
     #: attribute equals the resource, this is a real resource
     #: see :class:`.models.Allocation` for more information
-    mirror_of = Column(UUID(), nullable=False)
+    mirror_of: 'Column[uuid.UUID]' = Column(UUID(), nullable=False)
 
     #: Group uuid to which this allocation belongs to. Every allocation has a
-    #: group but some allcations may be the only one in their group.
-    group = Column(UUID(), nullable=False)
+    #: group but some allocations may be the only one in their group.
+    group: 'Column[uuid.UUID]' = Column(UUID(), nullable=False)
 
     #: Number of times this allocation may be reserved
-    quota = Column(types.Integer(), default=1)
+    # FIXME: Why is this not nullable=False? For now we pretend that it is
+    quota: 'Column[int]' = Column(types.Integer(), default=1)
 
     #: Maximum number of times this allocation may be reserved with one
     #: single reservation.
-    quota_limit = Column(types.Integer(), default=0, nullable=False)
+    quota_limit: 'Column[int]' = Column(
+        types.Integer(),
+        default=0,
+        nullable=False
+    )
 
     #: Partly available allocations may be reserved partially. How They may
     #: be partitioned is defined by the allocation's raster.
-    partly_available = Column(types.Boolean(), default=False)
+    partly_available: 'Column[bool]' = Column(types.Boolean(), default=False)
 
     #: True if reservations for this allocation must be approved manually.
-    approve_manually = Column(types.Boolean(), default=False)
+    approve_manually: 'Column[bool]' = Column(types.Boolean(), default=False)
 
     #: The timezone this allocation resides in.
-    timezone = Column(types.String())
+    # FIXME: Why is this not nullable=False? A lot of properties rely on this!
+    timezone: 'Column[_t.Optional[str]]' = Column(types.String())
 
     #: Custom data reserved for the user
-    data = Column(
+    data: 'Column[_t.Optional[_t.Any]]' = Column(
         JSON(),
         nullable=True
     )
 
-    _start = Column(UTCDateTime(timezone=False), nullable=False)
-    _end = Column(UTCDateTime(timezone=False), nullable=False)
-    _raster = Column(types.Integer(), nullable=False)
+    _start: 'Column[datetime]' = Column(
+        UTCDateTime(timezone=False),
+        nullable=False
+    )
+    _end: 'Column[datetime]' = Column(
+        UTCDateTime(timezone=False),
+        nullable=False
+    )
+    _raster: 'Column[Raster]' = Column(
+        types.Integer(),  # type:ignore[arg-type]
+        nullable=False
+    )
+
+    if _t.TYPE_CHECKING:
+        # forward declare backref
+        reserved_slots: _t.List[ReservedSlot]
 
     __table_args__ = (
         Index('mirror_resource_ix', 'mirror_of', 'resource'),
         UniqueConstraint('resource', '_start', name='resource_start_ix')
     )
 
     __mapper_args__ = {
         'polymorphic_identity': None,
         'polymorphic_on': type
     }
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Allocation):
+            return False
         return self.resource == other.resource and self._start == other._start
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return id(self)
 
-    def copy(self):
+    def copy(self) -> 'Self':
         """ Creates a new copy of this allocation. """
         allocation = self.__class__()
         allocation.resource = self.resource
         allocation.mirror_of = self.mirror_of
         allocation.group = self.group
         allocation.quota = self.quota
         allocation.partly_available = self.partly_available
@@ -124,198 +161,268 @@
         allocation.timezone = self.timezone
         allocation.data = self.data
         allocation._start = self._start
         allocation._end = self._end
         allocation._raster = self._raster
         return allocation
 
-    def get_start(self):
+    def get_start(self) -> datetime:
         return self._start
 
-    def set_start(self, start):
+    def set_start(self, start: datetime) -> None:
         if not start.tzinfo:
             assert self.timezone
             start = sedate.replace_timezone(start, self.timezone)
 
         if self.raster is not None:
             self._start = rasterize_start(start, self.raster)
         else:
-            self._start = rasterize_start(start, MIN_RASTER)
+            self._start = rasterize_start(start, MIN_RASTER)  # type:ignore
 
     #: The start of this allocation. Must be timezone aware.
     #: This date is rastered by the allocation's raster.
-    start = property(get_start, set_start)
+    if _t.TYPE_CHECKING:
+        # NOTE: type checkers perform some special sauce for property
+        #       so the non-decorator style isn't well supported
+        @property
+        def start(self) -> datetime: ...
+        @start.setter
+        def start(self, value: datetime) -> None: ...
+    else:
+        start = property(get_start, set_start)
 
-    def get_end(self):
+    def get_end(self) -> datetime:
         return self._end
 
-    def set_end(self, end):
+    def set_end(self, end: datetime) -> None:
         if not end.tzinfo:
             assert self.timezone
             end = sedate.replace_timezone(end, self.timezone)
 
         if self.raster is not None:
             self._end = rasterize_end(end, self.raster)
         else:
-            self._end = rasterize_end(end, MIN_RASTER)
+            self._end = rasterize_end(end, MIN_RASTER)  # type:ignore
 
     #: The end of this allocation. Must be timezone aware.
     #: This date is rastered by the allocation's raster.
     #: The end date is stored with an offset of minues one microsecond
     #: to avoid overlaps with other allocations.
     #: That is to say an allocation that ends at 15:00 really ends at
     #: 14:59:59.999999
-    end = property(get_end, set_end)
+    if _t.TYPE_CHECKING:
+        # NOTE: type checkers perform some special sauce for property
+        #       so the non-decorator style isn't well supported
+        @property
+        def end(self) -> datetime: ...
+        @end.setter
+        def end(self, value: datetime) -> None: ...
+    else:
+        end = property(get_end, set_end)
 
-    def get_raster(self):
+    def get_raster(self) -> 'Raster':
         return self._raster
 
-    def set_raster(self, raster):
+    def set_raster(self, raster: 'Raster') -> None:
         # the raster can only be set once!
         assert not self._raster
-        self._raster = raster
+        self._raster = raster  # type:ignore[unreachable]
 
         # re-rasterize start/end - during initialization it's possible for
         # them not to be setup correctly because that's done using
         # kwargs which has a random order. So it might set start, end, raster
         # in this order one time, then raster, start, end another time.
         #
         # this should of course only happen once - hence the assertion above
         if self._start:
             self._start = rasterize_start(self._start, self.raster)
 
         if self._end:
             self._end = rasterize_end(self._end, self.raster)
 
-    raster = property(get_raster, set_raster)
-
-    def display_start(self, timezone=None):
+    if _t.TYPE_CHECKING:
+        # NOTE: type checkers perform some special sauce for property
+        #       so the non-decorator style isn't well supported
+        @property
+        def raster(self) -> Raster: ...
+        @raster.setter
+        def raster(self, value: Raster) -> None: ...
+    else:
+        raster = property(get_raster, set_raster)
+
+    def display_start(
+        self,
+        timezone: _t.Optional['TzInfoOrName'] = None
+    ) -> datetime:
         """Returns the start in either the timezone given or the timezone
         on the allocation."""
-        return sedate.to_timezone(self.start, timezone or self.timezone)
-
-    def display_end(self, timezone=None):
+        if timezone is None:
+            assert self.timezone is not None
+            timezone = self.timezone
+
+        return sedate.to_timezone(self.start, timezone)
+
+    def display_end(
+        self,
+        timezone: _t.Optional['TzInfoOrName'] = None
+    ) -> datetime:
         """Returns the end plus one microsecond in either the timezone given
         or the timezone on the allocation.
 
         """
+        if timezone is None:
+            assert self.timezone is not None
+            timezone = self.timezone
+
         end = self.end + timedelta(microseconds=1)
-        return sedate.to_timezone(end, timezone or self.timezone)
+        return sedate.to_timezone(end, timezone)
+
+    def _prepare_range(
+        self,
+        start: '_OptDT1',
+        end: '_OptDT2'
+    ) -> _t.Tuple['_OptDT1', '_OptDT2']:
 
-    def _prepare_range(self, start, end):
         if start:
+            assert self.timezone is not None
             start = sedate.standardize_date(start, self.timezone)
         if end:
+            assert self.timezone is not None
             end = sedate.standardize_date(end, self.timezone)
 
         return start, end
 
     @property
-    def whole_day(self):
+    def whole_day(self) -> bool:
         """True if the allocation is a whole-day allocation.
 
         A whole-day allocation is not really special. It's just an allocation
         which starts at 0:00 and ends at 24:00 (or 23:59:59'999). Relative
         to its timezone.
 
         As such it can actually also span multiple days, only hours and minutes
         count.
 
         The use of this is to display allocations spanning days differently.
         """
 
         s, e = self.display_start(), self.display_end()
         assert s != e  # this can never be, except when caused by cosmic rays
-
+        assert self.timezone is not None
         return sedate.is_whole_day(s, e, self.timezone)
 
-    def overlaps(self, start, end):
+    def overlaps(self, start: datetime, end: datetime) -> bool:
         """ Returns true if the allocation overlaps with the given dates. """
 
         start, end = self._prepare_range(start, end)
         start, end = rasterize_span(start, end, self.raster)
 
         return sedate.overlaps(start, end, self.start, self.end)
 
-    def contains(self, start, end):
+    def contains(self, start: datetime, end: datetime) -> bool:
         """ Returns true if the the allocation contains the given dates. """
 
         start, end = self._prepare_range(start, end)
         start, end = rasterize_span(start, end, self.raster)
 
         return self.start <= start and end <= self.end
 
-    def free_slots(self, start=None, end=None):
+    def free_slots(
+        self,
+        start: _t.Optional[datetime] = None,
+        end: _t.Optional[datetime] = None
+    ) -> _t.List[_t.Tuple[datetime, datetime]]:
         """ Returns the slots which are not yet reserved. """
-        reserved = [slot.start for slot in self.reserved_slots]
-
-        slots = []
-        for start, end in self.all_slots(start, end):
-            if start not in reserved:
-                slots.append((start, end))
-
-        return slots
+        reserved = {slot.start for slot in self.reserved_slots}
 
-    def align_dates(self, start=None, end=None):
+        return [
+            (slot_start, slot_end)
+            for slot_start, slot_end in self.all_slots(start, end)
+            if slot_start not in reserved
+        ]
+
+    def align_dates(
+        self,
+        start: _t.Optional[datetime] = None,
+        end: _t.Optional[datetime] = None
+    ) -> _t.Tuple[datetime, datetime]:
         """ Aligns the given dates to the start and end date of the allocation.
 
         """
 
         start, end = self._prepare_range(start, end)
 
         start = start or self.start
         start = start < self.start and self.start or start
 
         end = end or self.end
         end = end > self.end and self.end or end
 
         return start, end
 
-    def all_slots(self, start=None, end=None):
+    def all_slots(
+        self,
+        start: _t.Optional[datetime] = None,
+        end: _t.Optional[datetime] = None
+    ) -> '_t.Iterator[_t.Tuple[datetime, datetime]]':
         """ Returns the slots which exist with this timespan. Reserved or free.
 
         """
         start, end = self.align_dates(start, end)
 
         if self.partly_available:
-            for start, end in iterate_span(start, end, self.raster):
-                yield start, end
+            yield from iterate_span(start, end, self.raster)
         else:
             yield self.start, self.end
 
-    def count_slots(self, start=None, end=None):
+    def count_slots(
+        self,
+        start: _t.Optional[datetime] = None,
+        end: _t.Optional[datetime] = None
+    ) -> int:
         """ Returns the number of slots which exist with this timespan.
         Reserved or free.
 
         """
         if not self.partly_available:
             return 1
 
         start, end = self.align_dates(start, end)
         seconds = (end + timedelta(microseconds=1) - start).total_seconds()
 
-        return seconds // (self.raster * 60)
+        return int(seconds) // (self.raster * 60)
 
-    def is_available(self, start=None, end=None):
+    def is_available(
+        self,
+        start: _t.Optional[datetime] = None,
+        end: _t.Optional[datetime] = None
+    ) -> bool:
         """ Returns true if the given daterange is completely available. """
 
         if not (start and end):
             start, end = self.start, self.end
 
         assert self.overlaps(start, end)
         reserved = {slot.start for slot in self.reserved_slots}
 
-        for start, end in self.all_slots(start, end):
-            if start in reserved:
+        for slot_start, _ in self.all_slots(start, end):
+            if slot_start in reserved:
                 return False
 
         return True
 
-    def limit_timespan(self, start, end, timezone=None, is_dst=False,
-                       raise_non_existent=False, raise_ambiguous=False):
+    def limit_timespan(
+        self,
+        start: time,
+        end: time,
+        timezone: _t.Optional['TzInfoOrName'] = None,
+        is_dst: bool = False,
+        raise_non_existent: bool = False,
+        raise_ambiguous: bool = False
+    ) -> _t.Tuple[datetime, datetime]:
         """ Takes the given timespan and moves the start/end date to
         the closest reservable slot. So if 10:00 - 11:00 is requested it will
 
         - on a partly available allocation return 10:00 - 11:00 if the raster
           allows for that
 
         - on a non-partly available allocation return the start/end date of
@@ -354,53 +461,53 @@
             s, e = rasterize_span(s, e, self.raster)
 
             return s, e + timedelta(microseconds=1)
         else:
             return self.display_start(timezone), self.display_end(timezone)
 
     @property
-    def pending_reservations(self):
+    def pending_reservations(self) -> 'Query[Reservation]':
         """ Returns the pending reservations query for this allocation.
         As the pending reservations target the group and not a specific
         allocation this function returns the same value for masters and
         mirrors.
 
         """
         assert not self.is_transient, (
             "Don't call if the allocation does not yet exist"
         )
 
         Reservation = self.models.Reservation
         query = object_session(self).query(Reservation.id)
         query = query.filter(Reservation.target == self.group)
-        query = query.filter(Reservation.status == u'pending')
+        query = query.filter(Reservation.status == 'pending')
 
         return query
 
     @property
-    def waitinglist_length(self):
+    def waitinglist_length(self) -> int:
         return self.pending_reservations.count()
 
     @property
-    def availability(self):
+    def availability(self) -> float:
         """Returns the availability in percent."""
 
         total = self.count_slots()
         used = len(self.reserved_slots)
 
         if total == used:
             return 0.0
 
         if used == 0:
             return 100.0
 
         return 100.0 - (float(used) / float(total) * 100.0)
 
     @property
-    def normalized_availability(self):
+    def normalized_availability(self) -> float:
         """Most of the time this will be the same value as
         ``availability``.
 
         For timezones with daylight savings it will treat the transition
         days with 23 and 25 hours respectively like a 24 hour day by either
         adding an imaginary unavailable hour or skipping the first ambiguous
         hour, that way the percentage will visually match what we return from
@@ -444,40 +551,44 @@
 
         if total == used:
             return 0.0
 
         return 100.0 - (float(used) / float(total) * 100.0)
 
     @property
-    def in_group(self):
+    def in_group(self) -> int:
         """True if the event is in any group."""
 
         query = object_session(self).query(Allocation.id)
         query = query.filter(Allocation.resource == self.resource)
         query = query.filter(Allocation.group == self.group)
         query = query.limit(2)
 
         return len(query.all()) > 1
 
     @property
-    def quota_left(self):
+    def quota_left(self) -> int:
         # this can be done quickly if this is a master with a quota of 1
         if self.is_master and self.quota == 1:
             return 1 if self.is_available() else 0
 
         # if not we need to go through the mirrors
         free_quota = 0
 
         for mirror in self.siblings():
             if mirror.is_available():
                 free_quota += 1
 
         return free_quota
 
-    def find_spot(self, start, end):
+    def find_spot(
+        self,
+        start: datetime,
+        end: datetime
+    ) -> _t.Optional['Self ']:
         """ Returns the first free allocation spot amongst the master and the
         mirrors. Honors the quota set on the master and will only try the
         master if the quota is set to 1.
 
         If no spot can be found, None is returned.
 
         """
@@ -494,28 +605,32 @@
             if mirror.is_available(start, end):
                 return mirror
 
             if tries >= 1:
                 tries -= 1
             else:
                 return None
+        return None
 
     @property
-    def is_separate(self):
+    def is_separate(self) -> bool:
         """True if available separately (as opposed to available only as
         part of a group)."""
         if self.partly_available:
             return True
 
         if self.in_group:
             return False
 
         return True
 
-    def normalized_slots(self):
+    def normalized_slots(self) -> _t.Iterator[_t.Union[
+        _t.Tuple[datetime, datetime],
+        _t.Tuple[None, None]
+    ]]:
         """Most of the times this will return the same thing as all_slots
         however for DST timezones it will ensure the transitions days with
         23 and 25 hours respectively still return 24 hours worth of slots.
         This is achieved by inserting imaginary slots for the non-existent
         hour or removing an hours worth of the ambiguous slots (skipping DST)
 
         The non-existent time slots will all be a tuple of ``None, None``
@@ -568,15 +683,18 @@
             for s, e in self.all_slots():
                 if s == imaginary_start:
                     for _ in range(num_slots):
                         # insert the imaginary slots
                         yield None, None
                 yield s, e
 
-    def availability_partitions(self, normalize_dst=True):
+    def availability_partitions(
+        self,
+        normalize_dst: bool = True
+    ) -> _t.List[_t.Tuple[float, bool]]:
         """Partitions the space between start and end into blocks of either
         free or reserved time. Each block has a percentage representing the
         space the block occupies compared to the size of the whole allocation.
 
         The blocks are ordered from start to end. Each block is an item with
         two values. The first being the percentage, the second being true if
         the block is reserved.
@@ -627,15 +745,15 @@
 
         # Create an entry for each slot with either True or False
         pieces = tuple(s is None or s in reserved for s in slots)
 
         # Group by the true/false values in the pieces and sum up the
         # percentage
         partitions = []
-        total = 0
+        total = 0.0
 
         for flag, group in groupby(pieces, key=lambda p: p):
             percentage = sum(1 for item in group) * step
             partitions.append((percentage, flag))
             total += percentage
 
         # Make sure to get rid of floating point rounding errors
@@ -643,15 +761,15 @@
         if partitions:
             percentage, flag = partitions[-1]
             partitions[-1] = (percentage - diff, flag)
 
         return partitions
 
     @property
-    def is_transient(self):
+    def is_transient(self) -> bool:
         """True if the allocation does not exist in the database, and is not
         about to be written to the database. If an allocation is transient it
         means that the given instance only exists in memory.
 
         See:
         http://www.sqlalchemy.org/docs/orm/session.html
         #quickie-intro-to-object-states
@@ -659,62 +777,64 @@
         sqlalchemy-get-object-instance-state
 
         """
 
         return object_session(self) is None and not has_identity(self)
 
     @hybrid_property
-    def is_master(self):
+    def is_master(self) -> bool:
         """True if the allocation is a master allocation."""
 
         return self.resource == self.mirror_of
 
-    def get_master(self):
+    def get_master(self) -> 'Self':
         if self.is_master:
             return self
         else:
             query = object_session(self).query(Allocation)
             query = query.filter(Allocation._start == self._start)
             query = query.filter(Allocation.resource == self.mirror_of)
 
             return query.one()
 
-    def siblings(self, imaginary=True):
+    def siblings(self, imaginary: bool = True) -> _t.List['Self']:
         """Returns the master/mirrors group this allocation is part of.
 
         If 'imaginary' is true, inexistant mirrors are created on the fly.
         those mirrors are transient (see self.is_transient)
 
         """
 
         # this function should always have itself in the result
         if not imaginary and self.is_transient:
-            assert False, "the resulting list wouldn't contain this allocation"
+            raise AssertionError(
+                "the resulting list wouldn't contain this allocation"
+            )
 
         if self.quota == 1:
             assert self.is_master
             return [self]
 
         query = object_session(self).query(Allocation)
         query = query.filter(Allocation.mirror_of == self.mirror_of)
         query = query.filter(Allocation._start == self._start)
 
-        existing = dict(((e.resource, e) for e in query))
+        existing = {e.resource: e for e in query}
 
         master = self.is_master and self or existing[self.mirror_of]
         existing[master.resource] = master
 
-        uuids = utils.generate_uuids(master.resource, master.quota)
-        imaginary = imaginary and (master.quota - len(existing)) or 0
+        uids = utils.generate_uuids(master.resource, master.quota)
+        imaginary_len = imaginary and (master.quota - len(existing)) or 0
 
         siblings = [master]
-        for uuid in uuids:
-            if uuid in existing:
-                siblings.append(existing[uuid])
-            elif imaginary > 0:
+        for uid in uids:
+            if uid in existing:
+                siblings.append(existing[uid])
+            elif imaginary_len > 0:
                 allocation = master.copy()
-                allocation.resource = uuid
+                allocation.resource = uid
                 siblings.append(allocation)
 
-                imaginary -= 1
+                imaginary_len -= 1
 
         return siblings
```

### Comparing `libres-0.6.1/libres/db/models/reservation.py` & `libres-0.7.0/src/libres/db/models/reservation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,117 +1,131 @@
 import sedate
 
-from collections import namedtuple
-from datetime import timedelta
+from datetime import datetime, timedelta
 
 from sqlalchemy import types
 from sqlalchemy.orm import object_session, deferred
 from sqlalchemy.schema import Column
 from sqlalchemy.schema import Index
 
 from libres.db.models import ORMBase
 from libres.db.models.types import UUID, UTCDateTime, JSON
 from libres.db.models.other import OtherModels
 from libres.db.models.timestamp import TimestampMixin
 
 
-Timespan = namedtuple(
-    'Timespan', ('start', 'end')
-)
+import typing as _t
+if _t.TYPE_CHECKING:
+    import uuid
+    from sedate.types import TzInfoOrName
+    from sqlalchemy.orm import Query
+
+    from libres.db.models import Allocation
+
+
+class Timespan(_t.NamedTuple):
+    start: datetime
+    end: datetime
 
 
 class Reservation(TimestampMixin, ORMBase, OtherModels):
     """Describes a pending or approved reservation.
 
     """
 
     __tablename__ = 'reservations'
 
-    id = Column(
+    id: 'Column[int]' = Column(
         types.Integer(),
         primary_key=True,
         autoincrement=True
     )
 
-    token = Column(
+    token: 'Column[uuid.UUID]' = Column(
         UUID(),
         nullable=False,
     )
 
-    target = Column(
+    target: 'Column[uuid.UUID]' = Column(
         UUID(),
         nullable=False,
     )
 
-    target_type = Column(
-        types.Enum(u'group', u'allocation', name='reservation_target_type'),
+    target_type: 'Column[_t.Literal["group", "allocation"]]' = Column(
+        types.Enum(  # type:ignore[arg-type]
+            'group', 'allocation',
+            name='reservation_target_type'
+        ),
         nullable=False
     )
 
-    type = Column(
+    type: 'Column[_t.Optional[str]]' = Column(
         types.Text(),
         nullable=True
     )
 
-    resource = Column(
+    resource: 'Column[uuid.UUID]' = Column(
         UUID(),
         nullable=False
     )
 
-    start = Column(
+    start: 'Column[_t.Optional[datetime]]' = Column(
         UTCDateTime(timezone=False),
         nullable=True
     )
 
-    end = Column(
+    end: 'Column[_t.Optional[datetime]]' = Column(
         UTCDateTime(timezone=False),
         nullable=True
     )
 
-    timezone = Column(
+    timezone: 'Column[_t.Optional[str]]' = Column(
         types.String(),
         nullable=True
     )
 
-    status = Column(
-        types.Enum(u'pending', u'approved', name="reservation_status"),
+    status: 'Column[_t.Literal["pending", "approved"]]' = Column(
+        types.Enum(  # type:ignore[arg-type]
+            'pending', 'approved',
+            name="reservation_status"
+        ),
         nullable=False
     )
 
-    data = deferred(
+    data: 'Column[_t.Optional[_t.Any]]' = deferred(
         Column(
             JSON(),
             nullable=True
         )
     )
 
-    email = Column(
+    email: 'Column[str]' = Column(
         types.Unicode(254),
         nullable=False
     )
 
-    session_id = Column(
+    session_id: 'Column[_t.Optional[uuid.UUID]]' = Column(
         UUID()
     )
 
-    quota = Column(
+    quota: 'Column[int]' = Column(
         types.Integer(),
         nullable=False
     )
 
     __table_args__ = (
         Index('target_status_ix', 'status', 'target', 'id'),
     )
 
     __mapper_args__ = {
         'polymorphic_identity': None,
         'polymorphic_on': type
     }
 
-    def _target_allocations(self):
+    def _target_allocations(self) -> 'Query[Allocation]':
         """ Returns the allocations this reservation is targeting. This should
         NOT be confused with db.allocations_by_reservation. The method in
         the db module returns the actual allocations belonging to an approved
         reservation.
 
         This method only returns the master allocations to get information
         about timespans and other properties. If you don't know exactly
@@ -127,52 +141,70 @@
         query = query.filter(Allocation.resource == Allocation.mirror_of)
 
         # order by date
         query = query.order_by(Allocation._start)
 
         return query
 
-    def display_start(self, timezone=None):
+    def display_start(
+        self,
+        timezone: _t.Optional['TzInfoOrName'] = None
+    ) -> datetime:
         """Does nothing but to form a nice pair to display_end."""
-        return sedate.to_timezone(self.start, timezone or self.timezone)
-
-    def display_end(self, timezone=None):
+        assert self.start is not None
+        if timezone is None:
+            assert self.timezone is not None
+            timezone = self.timezone
+        return sedate.to_timezone(self.start, timezone)
+
+    def display_end(
+        self,
+        timezone: _t.Optional['TzInfoOrName'] = None
+    ) -> datetime:
         """Returns the end plus one microsecond (nicer display)."""
+        assert self.end is not None
+        if timezone is None:
+            assert self.timezone is not None
+            timezone = self.timezone
+
         end = self.end + timedelta(microseconds=1)
-        return sedate.to_timezone(end, timezone or self.timezone)
+        return sedate.to_timezone(end, timezone)
 
-    def timespans(self):
+    def timespans(self) -> _t.List[Timespan]:
         """ Returns the timespans targeted by this reservation.
 
         The result is a list of :class:`~libres.db.models.reservation.Timespan`
         timespans. The start and end are the start and end dates of the
         referenced allocations.
 
         The timespans are ordered by start.
 
         """
 
-        if self.target_type == u'allocation':
+        if self.target_type == 'allocation':
             # we don't need to hit the database in this case
+            assert self.start is not None
+            assert self.end is not None
             return [
                 Timespan(self.start, self.end + timedelta(microseconds=1))
             ]
-        elif self.target_type == u'group':
+        elif self.target_type == 'group':
             return [
-                Timespan(a.start, a.end) for a in self._target_allocations()
+                Timespan(allocation.start, allocation.end)
+                for allocation in self._target_allocations()
             ]
         else:
             raise NotImplementedError
 
     @property
-    def title(self):
+    def title(self) -> str:
         return self.email
 
     @property
-    def autoapprovable(self):
+    def autoapprovable(self) -> bool:
         query = self._target_allocations()
         query = query.filter(self.models.Allocation.approve_manually == True)
 
         # A reservation is deemed autoapprovable if no allocation
         # requires explicit approval
 
-        return query.first() is None
+        return object_session(self).query(~query.exists()).scalar()
```

### Comparing `libres-0.6.1/libres/db/models/reserved_slot.py` & `libres-0.7.0/src/libres/db/models/reserved_slot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sedate
 
-from datetime import timedelta
+from datetime import datetime, timedelta
 from sqlalchemy import types
 from sqlalchemy.schema import Column
 from sqlalchemy.schema import Index
 from sqlalchemy.schema import ForeignKey
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm import backref
 
@@ -14,80 +14,102 @@
 )
 
 from libres.db.models import ORMBase, Allocation
 from libres.db.models.types import UUID, UTCDateTime
 from libres.db.models.timestamp import TimestampMixin
 
 
+import typing as _t
+if _t.TYPE_CHECKING:
+    import uuid
+    from sedate.types import TzInfoOrName
+
+
 class ReservedSlot(TimestampMixin, ORMBase):
     """Describes a reserved slot within an allocated timespan."""
 
     __tablename__ = 'reserved_slots'
 
-    resource = Column(
+    resource: 'Column[uuid.UUID]' = Column(
         UUID(),
         primary_key=True,
         nullable=False,
         autoincrement=False
     )
 
-    start = Column(
+    start: 'Column[datetime]' = Column(
         UTCDateTime(timezone=False),
         primary_key=True,
         nullable=False,
         autoincrement=False
     )
 
-    end = Column(
+    end: 'Column[datetime]' = Column(
         UTCDateTime(timezone=False),
         nullable=False
     )
 
-    allocation_id = Column(
+    allocation_id: 'Column[int]' = Column(
         types.Integer(),
         ForeignKey(Allocation.id),
         nullable=False
     )
 
-    allocation = relationship(
+    allocation: 'relationship[Allocation]' = relationship(
         Allocation,
         primaryjoin=Allocation.id == allocation_id,
 
         # Reserved_slots are eagerly joined since we usually want both
         # allocation and reserved_slots. There's barely a function which does
         # not need to know about reserved slots when working with allocation.
         backref=backref(
             'reserved_slots',
             lazy='joined',
             cascade='all, delete-orphan'
         )
     )
 
-    reservation_token = Column(
+    reservation_token: 'Column[uuid.UUID]' = Column(
         UUID(),
         nullable=False
     )
 
     __table_args__ = (
         Index('reservation_resource_ix', 'reservation_token', 'resource'),
     )
 
-    def display_start(self, timezone=None):
+    def display_start(
+        self,
+        timezone: _t.Optional['TzInfoOrName'] = None
+    ) -> datetime:
+
+        if timezone is None:
+            assert self.allocation.timezone is not None
+            timezone = self.allocation.timezone
+
         start = rasterize_start(self.start, self.allocation.raster)
-        return sedate.to_timezone(
-            start, timezone or self.allocation.timezone
-        )
+        return sedate.to_timezone(start, timezone)
+
+    def display_end(
+        self,
+        timezone: _t.Optional['TzInfoOrName'] = None
+    ) -> datetime:
+
+        if timezone is None:
+            assert self.allocation.timezone is not None
+            timezone = self.allocation.timezone
 
-    def display_end(self, timezone=None):
         end = rasterize_end(self.end, self.allocation.raster)
         end += timedelta(microseconds=1)
+        return sedate.to_timezone(end, timezone)
 
-        return sedate.to_timezone(
-            end, timezone or self.allocation.timezone
-        )
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, ReservedSlot):
+            return False
 
-    def __eq__(self, other):
-        return self.start == other.start and \
+        return (
+            self.start == other.start and
             str(self.resource) == str(other.resource)
+        )
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return id(self)
```

### Comparing `libres-0.6.1/libres/db/models/timestamp.py` & `libres-0.7.0/src/libres/db/models/timestamp.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,38 +2,48 @@
 
 from libres.db.models.types import UTCDateTime
 from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy.orm import deferred
 from sqlalchemy.schema import Column
 
 
-class TimestampMixin(object):
+import typing as _t
+if _t.TYPE_CHECKING:
+    from datetime import datetime
+
+
+class TimestampMixin:
     """ Mixin providing created/modified timestamps for all records. Pretty
     much relies on the database being Postgresql but could be made to work
     with others.
 
     The columns are deferred loaded as this is primarily for logging and future
     forensics.
 
     """
 
     @staticmethod
-    def timestamp():
+    def timestamp() -> 'datetime':
         return sedate.utcnow()
 
-    @declared_attr
-    def created(cls):
-        return deferred(
-            Column(
-                UTCDateTime(timezone=False),
-                default=cls.timestamp
+    if _t.TYPE_CHECKING:
+        created: Column[datetime]
+        modified: Column[_t.Optional[datetime]]
+
+    else:
+        @declared_attr
+        def created(cls) -> 'Column[datetime]':
+            return deferred(
+                Column(
+                    UTCDateTime(timezone=False),
+                    default=cls.timestamp
+                )
             )
-        )
 
-    @declared_attr
-    def modified(cls):
-        return deferred(
-            Column(
-                UTCDateTime(timezone=False),
-                onupdate=cls.timestamp
+        @declared_attr
+        def modified(cls) -> 'Column[_t.Optional[datetime]]':
+            return deferred(
+                Column(
+                    UTCDateTime(timezone=False),
+                    onupdate=cls.timestamp
+                )
             )
-        )
```

### Comparing `libres-0.6.1/libres/db/models/types/utcdatetime.py` & `libres-0.7.0/src/libres/db/models/types/utcdatetime.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,48 @@
 import sedate
 
 from sqlalchemy import types
 
 
-class UTCDateTime(types.TypeDecorator):
+import typing as _t
+if _t.TYPE_CHECKING:
+    from datetime import datetime
+    from sqlalchemy.engine import Dialect
+
+    _Base = types.TypeDecorator[datetime]
+else:
+    _Base = types.TypeDecorator
+
+
+class UTCDateTime(_Base):
     """ Stores dates as UTC.
 
     Internally, they are stored as timezone naive, because Postgres takes
     the local timezone into account when working with timezones. We really
     want to have those dates in UTC at all times, though for convenience we
     make the dates timezone aware when retrieving the values and we make sure
     that timezone aware dates are converted to UTC before storing.
 
     """
 
     impl = types.DateTime
     cache_ok = True
 
-    def process_bind_param(self, value, engine):
+    def process_bind_param(  # type:ignore[override]
+        self,
+        value: _t.Optional['datetime'],
+        dialect: 'Dialect'
+    ) -> _t.Optional['datetime']:
+
         if value is not None:
             return sedate.to_timezone(value, 'UTC').replace(tzinfo=None)
+        return None
+
+    def process_result_value(
+        self,
+        value: _t.Optional['datetime'],
+        dialect: 'Dialect'
+    ) -> _t.Optional['datetime']:
 
-    def process_result_value(self, value, engine):
         if value is not None:
             return sedate.replace_timezone(value, 'UTC')
+        return None
```

### Comparing `libres-0.6.1/libres/db/models/types/uuid_type.py` & `libres-0.7.0/src/libres/db/models/types/uuid_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,67 @@
 import uuid
 
-from libres.modules.compat import string_types
-
 from sqlalchemy.types import TypeDecorator
 from sqlalchemy.dialects import postgresql
 
 
+import typing as _t
+if _t.TYPE_CHECKING:
+    from sqlalchemy.engine import Dialect
+
+    _Base = TypeDecorator['SoftUUID']
+else:
+    _Base = TypeDecorator
+
+
 class SoftUUID(uuid.UUID):
     """ Behaves just like the UUID class, but allows strings to be compared
     with it, so that SoftUUID('my-uuid') == 'my-uuid' equals True.
 
     """
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
 
-        if isinstance(other, string_types):
+        if isinstance(other, str):
             return self.hex == other.replace('-', '').strip()
 
         if isinstance(other, uuid.UUID):
             return self.int == other.int
 
         return False
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
-    def __hash__(self):
-        # this function is not inherited in python 2
+    def __hash__(self) -> int:
         return hash(self.int)
 
 
-class UUID(TypeDecorator):
+class UUID(_Base):
     """ Same as the Postgres UUID type, but returning SoftUUIDs instead
     of UUIDs on bind.
 
     """
     impl = postgresql.UUID
     cache_ok = True
 
-    def process_bind_param(self, value, dialect):
+    def process_bind_param(
+        self,
+        value: _t.Optional[uuid.UUID],
+        dialect: 'Dialect'
+    ) -> _t.Optional[str]:
+
         if value is not None:
             return str(value)
+        return None
 
-    def process_result_value(self, value, dialect):
+    def process_result_value(
+        self,
+        value: _t.Optional[str],
+        dialect: 'Dialect'
+    ) -> _t.Optional[SoftUUID]:
         if value is not None:
             # Postgres always returns the uuid in the same format, so we
             # can turn it into an int immediately, avoiding some checks
             # and extra code run by UUID
             return SoftUUID(int=int(value.replace('-', ''), 16))
+        return None
```

### Comparing `libres-0.6.1/libres/db/queries.py` & `libres-0.7.0/src/libres/db/queries.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 import logging
 import sedate
 
-from datetime import timedelta
+from datetime import date, datetime, timedelta
 from itertools import groupby
 from libres.context.core import ContextServicesMixin
 from libres.db.models import Allocation, Reservation, ReservedSlot
 from libres.modules import errors, events
-from sqlalchemy import func, null
+from sqlalchemy import func
 from sqlalchemy.orm import joinedload
 from sqlalchemy.sql import and_, or_
 
 
+import typing as _t
+if _t.TYPE_CHECKING:
+    from sqlalchemy.orm import Query
+    from uuid import UUID
+
+    from libres.context.core import Context
+
+_T = _t.TypeVar('_T')
+
+
 log = logging.getLogger('libres')
 
 
 class Queries(ContextServicesMixin):
     """ Contains helper methods independent of the resource (as owned by
     :class:`.scheduler.Scheduler`)
 
     Some contained methods require the current context (for the session).
     Some contained methods do not require any context, they are marked
     as staticmethods.
 
     """
 
-    def __init__(self, context):
+    def __init__(self, context: 'Context'):
         self.context = context
 
-    def all_allocations_in_range(self, start, end):
+    def all_allocations_in_range(
+        self,
+        start: datetime,
+        end: datetime
+    ) -> 'Query[Allocation]':
         return self.allocations_in_range(
             self.session.query(Allocation), start, end
         )
 
     @staticmethod
-    def allocations_in_range(query, start, end):
+    def allocations_in_range(
+        query: 'Query[_T]',
+        start: datetime,
+        end: datetime
+    ) -> 'Query[_T]':
         """ Takes an allocation query and limits it to the allocations
         overlapping with start and end.
 
         """
         return query.filter(
             or_(
                 and_(
@@ -48,22 +66,47 @@
                     start <= Allocation._start,
                     Allocation._start <= end
                 )
             )
         )
 
     @staticmethod
-    def availability_by_allocations(allocations):
-        """Takes any iterator with alloctions and calculates the availability.
+    def overlapping_allocations(
+        query: 'Query[_T]',
+        dates: _t.Iterable[_t.Tuple[datetime, datetime]]
+    ) -> 'Query[_T]':
+        """ Takes an allocation query and limits it to the allocations
+        overlapping with any of the passed in datetime ranges
+
+        """
+        return query.filter(or_(*(
+            or_(
+                and_(
+                    Allocation._start <= start,
+                    start <= Allocation._end
+                ),
+                and_(
+                    start <= Allocation._start,
+                    Allocation._start <= end
+                )
+            )
+            for start, end in dates
+        )))
+
+    @staticmethod
+    def availability_by_allocations(
+        allocations: _t.Iterable['Allocation']
+    ) -> float:
+        """Takes any iterable with alloctions and calculates the availability.
         Counts missing mirrors as 100% free and returns a value between 0-100
         in any case.
         For single allocations check the allocation.availability property.
 
         """
-        total, expected_count, count = 0, 0, 0
+        total, expected_count, count = 0.0, 0, 0
         for allocation in allocations:
             total += allocation.availability
             count += 1
 
             # Sum up the expected number of allocations. Missing allocations
             # indicate mirrors that have not yet been physically created.
             if allocation.is_master:
@@ -73,29 +116,39 @@
             return 0
 
         missing = expected_count - count
         total += missing * 100
 
         return total / expected_count
 
-    def availability_by_range(self, start, end, resources):
+    def availability_by_range(
+        self,
+        start: datetime,
+        end: datetime,
+        resources: _t.Collection['UUID']
+    ) -> float:
         """Returns the availability for the given resources in the given range.
         The exposure is used to check if the allocation is visible.
 
         """
 
         query = self.all_allocations_in_range(start, end)
         query = query.filter(Allocation.mirror_of.in_(resources))
         query = query.options(joinedload(Allocation.reserved_slots))
 
         allocations = (a for a in query if self.is_allocation_exposed(a))
 
         return self.availability_by_allocations(allocations)
 
-    def availability_by_day(self, start, end, resources):
+    def availability_by_day(
+        self,
+        start: datetime,
+        end: datetime,
+        resources: _t.Collection['UUID']
+    ) -> _t.Dict[date, _t.Tuple[float, _t.Set['UUID']]]:
         """Availability by range with a twist. Instead of returning a grand
         total, a dictionary is returned with each day in the range as key and
         a tuple of availability and the resources counted for that day.
 
         WARNING, this function should run as linearly as possible as a lot
         of records might be processed.
 
@@ -122,15 +175,18 @@
 
             total = self.availability_by_allocations(exposed)
 
             days[day] = (total, members)
 
         return days
 
-    def reservations_by_session(self, session_id):
+    def reservations_by_session(
+        self,
+        session_id: _t.Optional['UUID']
+    ) -> 'Query[Reservation]':
 
         # be sure to not query for all reservations. since a query should be
         # returned in any case we just use an impossible clause
 
         # this is mainly a security feature
         if not session_id:
             log.warn('empty session id')
@@ -138,40 +194,48 @@
 
         query = self.session.query(Reservation)
         query = query.filter(Reservation.session_id == session_id)
         query = query.order_by(Reservation.created)
 
         return query
 
-    def confirm_reservations_for_session(self, session_id, token=None):
+    def confirm_reservations_for_session(
+        self,
+        session_id: 'UUID',
+        token: _t.Optional['UUID'] = None
+    ) -> None:
         """ Confirms all reservations of the given session id. Optionally
         confirms only the reservations with the given token. All if None.
 
         """
 
         assert session_id
 
-        reservations = self.reservations_by_session(session_id)
+        res_query = self.reservations_by_session(session_id)
 
         if token:
-            reservations = reservations.filter(Reservation.token == token)
+            res_query = res_query.filter(Reservation.token == token)
 
-        reservations = reservations.all()
+        reservations = res_query.all()
 
         if not reservations:
             raise errors.NoReservationsToConfirm
 
         for reservation in reservations:
             reservation.session_id = None
 
         events.on_reservations_confirmed(
             self.context, reservations, session_id
         )
 
-    def remove_reservation_from_session(self, session_id, token):
+    def remove_reservation_from_session(
+        self,
+        session_id: 'UUID',
+        token: 'UUID'
+    ) -> None:
         """ Removes the reservation with the given session_id and token. """
 
         assert token and session_id
 
         query = self.reservations_by_session(session_id)
         query = query.filter(Reservation.token == token)
 
@@ -196,59 +260,58 @@
         # already old enough to be counted as expired.
 
         query = self.session.query(Reservation)
         query = query.filter(Reservation.session_id == session_id)
 
         query.update({"modified": sedate.utcnow()})
 
-    def find_expired_reservation_sessions(self, expiration_date):
+    def find_expired_reservation_sessions(
+        self,
+        expiration_date: _t.Optional[datetime]
+    ) -> _t.List['UUID']:
         """ Goes through all reservations and returns the session ids of the
         unconfirmed ones which are older than the given expiration date.
         By default the expiration date is now - 15 minutes.
 
         Note that this method goes through ALL RESERVATIONS OF THE CURRENT
         SESSION. This is NOT limited to a specific context or scheduler.
 
         """
 
         expiration_date = expiration_date or (
             sedate.utcnow() - timedelta(minutes=15)
         )
 
         # first get the session ids which are expired
+        query: 'Query[_t.Tuple[UUID, datetime, _t.Optional[datetime]]]'
         query = self.session.query(
             Reservation.session_id,
             func.max(Reservation.created),
             func.max(Reservation.modified)
         )
-
         query = query.group_by(Reservation.session_id)
 
-        # != null() because != None is not allowed by PEP8
-        query = query.filter(Reservation.session_id != null())
+        query = query.filter(Reservation.session_id.isnot(None))
 
         # only pending reservations are considered
         query = query.filter(Reservation.status == 'pending')
 
         # the idea is to remove all reservations belonging to sessions whose
         # latest update is expired - either delete the whole session or let
         # all of it be
-        expired_sessions = []
-
-        for session_id, created, modified in query.all():
-
-            modified = modified or created
-            assert created and modified
-
-            if max(created, modified) < expiration_date:
-                expired_sessions.append(session_id)
-
-        return expired_sessions
-
-    def remove_expired_reservation_sessions(self, expiration_date=None):
+        return [
+            session_id
+            for session_id, created, modified in query
+            if max(created, modified or created) < expiration_date
+        ]
+
+    def remove_expired_reservation_sessions(
+        self,
+        expiration_date: _t.Optional[datetime] = None
+    ) -> _t.List['UUID']:
         """ Removes all reservations which have an expired session id.
         By default the expiration date is now - 15 minutes.
 
         See :func:`find_expired_reservation_sessions`
 
         Note that this method goes through ALL RESERVATIONS OF THE CURRENT
         SESSION. This is NOT limited to a specific context or scheduler.
```

### Comparing `libres-0.6.1/libres/db/scheduler.py` & `libres-0.7.0/src/libres/db/scheduler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,59 @@
 import sedate
 
-from datetime import datetime, timedelta
+from datetime import datetime, time, timedelta
+from operator import attrgetter
+from sqlalchemy import func
+from sqlalchemy.orm import exc
+from sqlalchemy.sql import and_, not_
+from uuid import uuid4 as new_uuid, UUID
 
 from libres.context.core import ContextServicesMixin
 from libres.db.models import ORMBase, Allocation, ReservedSlot, Reservation
 from libres.db.queries import Queries
-from libres.modules import compat
 from libres.modules import errors
 from libres.modules import events
 from libres.modules import rasterizer
 from libres.modules import utils
 
-from sqlalchemy import func
-from sqlalchemy.orm import exc
-from sqlalchemy.sql import and_, not_
 
-from uuid import uuid4 as new_uuid
+import typing as _t
+if _t.TYPE_CHECKING:
+    from sqlalchemy.orm import Query
+    from typing_extensions import NotRequired, Self, TypeAlias, TypedDict
+
+    from libres.context.core import Context
+    from libres.modules.rasterizer import Raster
+
+    _dtrange: TypeAlias = _t.Tuple[datetime, datetime]
+
+    class _ReserveArgs1(TypedDict):
+        email: str
+        dates: _t.Union['_dtrange', _t.Collection['_dtrange']]
+        data: NotRequired[_t.Optional[_t.Any]]
+        session_id: NotRequired[_t.Optional[UUID]]
+        quota: NotRequired[int]
+        single_token_per_session: NotRequired[bool]
+
+    class _ReserveArgs2(TypedDict):
+        email: str
+        group: UUID
+        data: NotRequired[_t.Optional[_t.Any]]
+        session_id: NotRequired[_t.Optional[UUID]]
+        quota: NotRequired[int]
+        single_token_per_session: NotRequired[bool]
+
+    _ReserveArgs: TypeAlias = _t.Union[_ReserveArgs1, _ReserveArgs2]
 
 
 missing = object()
-DAYS_MAP = {
+
+Day = _t.Literal['mo', 'tu', 'we', 'th', 'fr', 'sa', 'su']
+DayNumber = _t.Literal[0, 1, 2, 3, 4, 5, 6]
+DAYS_MAP: _t.Dict[Day, DayNumber] = {
     'mo': 0,
     'tu': 1,
     'we': 2,
     'th': 3,
     'fr': 4,
     'sa': 5,
     'su': 6
@@ -31,16 +61,23 @@
 
 
 class Scheduler(ContextServicesMixin):
     """ The Scheduler is responsible for talking to the backend of the given
     context to create reservations. It is the main part of the API.
     """
 
-    def __init__(self, context, name, timezone,
-                 allocation_cls=Allocation, reservation_cls=Reservation):
+    def __init__(
+        self,
+        context: 'Context',
+        name: str,
+        # FIXME: Not quite sure why we don't allow a PyTzInfo
+        timezone: str,
+        allocation_cls: _t.Type[Allocation] = Allocation,
+        reservation_cls: _t.Type[Reservation] = Reservation
+    ):
         """ Initializeds a new Scheduler instance.
 
         :context:
             The :class:`libres.context.core.Context` this scheduler should
             operate on. Acquire a context by using
             :func:`libres.context.registry.Registry.register_context`.
 
@@ -59,122 +96,151 @@
             assumed to be of this timezone!
 
             This timezone cannot change after allocations have been created!
             If it does, a migration has to be written (as of yet no such
             migration exists).
         """
 
-        assert isinstance(timezone, compat.string_types)
+        assert isinstance(timezone, str)
 
         self.context = context
         self.queries = Queries(context)
 
         self.name = name
         self.timezone = timezone
 
         self.allocation_cls = allocation_cls
         self.reservation_cls = reservation_cls
 
-    def clone(self):
+    def clone(self) -> 'Self':
         """ Clones the scheduler. The result will be a new scheduler using the
         same context, name, settings and attributes.
 
         """
 
-        return Scheduler(self.context, self.name, self.timezone)
+        return self.__class__(
+            self.context,
+            self.name,
+            self.timezone,
+            self.allocation_cls,
+            self.reservation_cls
+        )
 
     @property
-    def resource(self):
+    def resource(self) -> UUID:
         """ The resource that belongs to this scheduler. The resource is
         a uuid created from the name and context of this scheduler, based
         on the namespace uuid defined in :ref:`settings.uuid_namespace`
 
         """
         return self.generate_uuid(self.name)
 
-    def setup_database(self):
+    def setup_database(self) -> None:
         """ Creates the tables and indices required for libres. This needs
         to be called once per database. Multiple invocations won't hurt but
         they are unnecessary.
 
         """
         ORMBase.metadata.create_all(self.session.bind)
 
-    def _prepare_dates(self, dates):
+    def _prepare_dates(
+        self,
+        dates: 'utils._NestedIterable[datetime]'
+    ) -> _t.List[_t.Tuple[datetime, datetime]]:
         return [
             (
                 sedate.standardize_date(s, self.timezone),
                 sedate.standardize_date(e, self.timezone)
             ) for s, e in utils.pairs(dates)
         ]
 
-    def _prepare_range(self, start, end):
+    def _prepare_range(
+        self,
+        start: datetime,
+        end: datetime
+    ) -> _t.Tuple[datetime, datetime]:
         return (
             sedate.standardize_date(start, self.timezone),
             sedate.standardize_date(end, self.timezone)
         )
 
-    def managed_allocations(self):
+    def managed_allocations(self) -> 'Query[Allocation]':
         """ The allocations managed by this scheduler / resource. """
         query = self.session.query(Allocation)
         query = query.filter(Allocation.mirror_of == self.resource)
 
         return query
 
-    def managed_reserved_slots(self):
+    def managed_reserved_slots(self) -> 'Query[ReservedSlot]':
         """ The reserved_slots managed by this scheduler / resource. """
         uuids = self.managed_allocations().with_entities(Allocation.resource)
 
         query = self.session.query(ReservedSlot)
         query = query.filter(ReservedSlot.resource.in_(uuids))
 
         return query
 
-    def managed_reservations(self):
+    def managed_reservations(self) -> 'Query[Reservation]':
         """ The reservations managed by this scheduler / resource. """
         query = self.session.query(Reservation)
         query = query.filter(Reservation.resource == self.resource)
 
         return query
 
-    def extinguish_managed_records(self):
+    def extinguish_managed_records(self) -> None:
         """ WARNING:
         Completely removes any trace of the records managed by this scheduler.
         That means all reservations, reserved slots and allocations!
 
         """
         self.managed_reservations().delete('fetch')
         self.managed_reserved_slots().delete('fetch')
         self.managed_allocations().delete('fetch')
 
-    def allocation_by_id(self, id):
+    def allocation_by_id(self, id: int) -> Allocation:
         query = self.managed_allocations()
         query = query.filter(Allocation.mirror_of == self.resource)
         query = query.filter(Allocation.id == id)
         return query.one()
 
-    def allocations_by_ids(self, ids):
+    def allocations_by_ids(
+        self,
+        ids: _t.Collection[UUID]
+    ) -> 'Query[Allocation]':
         query = self.managed_allocations()
         query = query.filter(Allocation.id.in_(ids))
         query = query.order_by(Allocation._start)
         return query
 
-    def allocations_by_group(self, group, masters_only=True):
+    def allocations_by_group(
+        self,
+        group: UUID,
+        masters_only: bool = True
+    ) -> 'Query[Allocation]':
         return self.allocations_by_groups([group], masters_only=masters_only)
 
-    def allocations_by_groups(self, groups, masters_only=True):
+    def allocations_by_groups(
+        self,
+        groups: _t.Collection[UUID],
+        masters_only: bool = True
+    ) -> 'Query[Allocation]':
+
         query = self.managed_allocations()
         query = query.filter(Allocation.group.in_(groups))
 
         if masters_only:
             query = query.filter(Allocation.resource == self.resource)
 
         return query
 
-    def allocations_by_reservation(self, token, id=None):
+    def allocations_by_reservation(
+        self,
+        token: UUID,
+        id: _t.Optional[int] = None
+    ) -> 'Query[Allocation]':
         """ Returns the allocations for the reservation if it was *approved*,
         pending reservations return nothing. If you need to get the allocation
         a pending reservation might be targeting, use _target_allocations
         in model.reservation.
 
         """
 
@@ -200,69 +266,86 @@
             ReservedSlot.reservation_token == token
         )
         query = query.filter(
             ReservedSlot.allocation_id.in_(allocations)
         )
         return query
 
-    def allocations_in_range(self, start, end, masters_only=True):
+    def allocations_in_range(
+        self,
+        start: datetime,
+        end: datetime,
+        masters_only: bool = True
+    ) -> 'Query[Allocation]':
+
         start, end = self._prepare_range(start, end)
 
         query = self.managed_allocations()
         query = self.queries.allocations_in_range(query, start, end)
 
         if masters_only:
             query = query.filter(Allocation.resource == self.resource)
 
         return query
 
-    def allocation_by_date(self, start, end):
+    def allocation_by_date(self, start: datetime, end: datetime) -> Allocation:
         query = self.allocations_in_range(start, end)
         return query.one()
 
-    def allocation_dates_by_group(self, group):
-        query = self.allocations_by_group(group)
-        query = query.with_entities(Allocation._start, Allocation._end)
+    def allocation_dates_by_group(
+        self,
+        group: UUID
+    ) -> _t.List[_t.Tuple[datetime, datetime]]:
 
-        return query.all()
+        query = self.allocations_by_group(group)
+        dates_query = query.with_entities(Allocation._start, Allocation._end)
+        return dates_query.all()
 
-    def allocation_mirrors_by_master(self, master):
+    def allocation_mirrors_by_master(
+        self,
+        master: Allocation
+    ) -> _t.List[Allocation]:
         return [s for s in master.siblings() if not s.is_master]
 
-    def allocation_dates_by_ids(self, ids, start_time=None, end_time=None):
+    def allocation_dates_by_ids(
+        self,
+        ids: _t.Collection[UUID],
+        start_time: _t.Optional[time] = None,
+        end_time: _t.Optional[time] = None
+    ) -> _t.Iterator[_t.Tuple[datetime, datetime]]:
 
         for allocation in self.allocations_by_ids(ids).all():
 
             s = start_time or allocation.display_start().time()
             e = end_time or allocation.display_end().time()
 
-            s, e = allocation.limit_timespan(s, e)
+            s_dt, e_dt = allocation.limit_timespan(s, e)
 
-            yield s, e - timedelta(microseconds=1)
+            yield s_dt, e_dt - timedelta(microseconds=1)
 
-    def manual_approval_required(self, ids):
+    def manual_approval_required(self, ids: _t.Collection[UUID]) -> bool:
         """ Returns True if any of the allocations require manual approval. """
         query = self.allocations_by_ids(ids)
         query = query.filter(Allocation.approve_manually == True)
 
-        return query.first() and True or False
+        return self.session.query(query.exists()).scalar()
 
     def allocate(
         self,
-        dates,
-        partly_available=False,
-        raster=rasterizer.MIN_RASTER,
-        whole_day=False,
-        quota=None,
-        quota_limit=0,
-        grouped=False,
-        data=None,
-        approve_manually=False,
-        skip_overlapping=False,
-    ):
+        dates: _t.Union['_dtrange', _t.Iterable['_dtrange']],
+        partly_available: bool = False,
+        raster: 'Raster' = rasterizer.MIN_RASTER,
+        whole_day: bool = False,
+        quota: _t.Optional[int] = None,
+        quota_limit: int = 0,
+        grouped: bool = False,
+        data: _t.Optional[_t.Any] = None,
+        approve_manually: bool = False,
+        skip_overlapping: bool = False,
+    ) -> _t.List[Allocation]:
         """ Allocates a spot in the sedate.
 
         An allocation defines a timerange which can be reserved. No
         reservations can exist outside of existing allocations. In fact any
         reserved slot will link to an allocation.
 
         :dates:
@@ -388,30 +471,49 @@
                 )
 
         # Ensure that the list of dates contains no overlaps inside
         rasterized_dates = [
             rasterizer.rasterize_span(s, e, raster) for s, e in dates
         ]
 
+        # We can early out here, since this will create no allocations
+        # that way we also don't have to worry about calling min/max
+        # with an empty iterable
+        if not rasterized_dates:
+            return []
+
         for start, end in rasterized_dates:
             if sedate.count_overlaps(rasterized_dates, start, end) > 1:
                 raise errors.InvalidAllocationError
             if end < start:
                 raise errors.InvalidAllocationError
 
         # Make sure that this span does not overlap another master
         skipped = set()
 
-        for start, end in rasterized_dates:
-            existing = self.allocations_in_range(start, end).first()
+        # Find existing overlapping (master) allocations
+        query = self.managed_allocations()
+        query = self.queries.overlapping_allocations(query, rasterized_dates)
+        query = query.filter(Allocation.resource == self.resource)
+        for existing in query:
+            # we are doing a bit of redundant work here, since the
+            # query doesn't tell us which range(s) the existing
+            # allocation overlaps with
+            for start, end in rasterized_dates:
+                if not sedate.overlaps(
+                    start, end,
+                    existing.start, existing.end
+                ):
+                    continue
 
-            if existing and not skip_overlapping:
-                raise errors.OverlappingAllocationError(start, end, existing)
-            elif existing and skip_overlapping:
-                skipped.add((start, end))
+                if not skip_overlapping:
+                    raise errors.OverlappingAllocationError(
+                        start, end, existing)
+                else:
+                    skipped.add((start, end))
 
         # Write the master allocations
         allocations = []
         for start, end in dates:
 
             if rasterizer.rasterize_span(start, end, raster) in skipped:
                 continue
@@ -439,15 +541,15 @@
         self.session.add_all(allocations)
         self.session.flush()
 
         events.on_allocations_added(self.context, allocations)
 
         return allocations
 
-    def change_quota(self, master, new_quota):
+    def change_quota(self, master: Allocation, new_quota: int) -> None:
         """ Changes the quota of a master allocation.
 
         Fails if the quota is already exhausted.
 
         When the quota is decreased a reorganization of the mirrors is
         triggered. Reorganizing means eliminating gaps in the chain of mirrors
         that emerge when reservations are removed:
@@ -506,24 +608,25 @@
         mirrors = self.allocation_mirrors_by_master(master)
         allocations = [master] + mirrors
 
         free_allocations = [a for a in allocations if a.is_available()]
 
         required = master.quota - new_quota
         if len(free_allocations) < required:
+            # FIXME: This seems like a strange error to emit here
             raise errors.AffectedReservationError(None)
 
         # get a map pointing from the existing uuid to the newly assigned uuid
         reordered = self.reordered_keylist(allocations, new_quota)
 
         # unused keys are the ones not present in the newly assignd uuid list
-        unused = set(reordered.keys()) - set(reordered.values()) - set((None,))
+        unused = set(reordered.keys()) - set(reordered.values()) - {None}
 
         # get a map for resource_uuid -> allocation.id
-        ids = dict(((a.resource, a.id) for a in allocations))
+        ids = {a.resource: a.id for a in allocations}
 
         for allocation in allocations:
 
             # change the quota for all allocations
             allocation.quota = new_quota
 
             # the value is None if the allocation is not mapped to a new uuid
@@ -556,65 +659,85 @@
         if unused:
             query = self.session.query(Allocation)
             query = query.filter(Allocation.resource.in_(unused))
             query = query.filter(Allocation.id != master.id)
             query = query.filter(Allocation._start == master._start)
             query.delete('fetch')
 
-    def reordered_keylist(self, allocations, new_quota):
+    def reordered_keylist(
+        self,
+        allocations: _t.Collection[Allocation],
+        new_quota: int
+    ) -> _t.Dict[UUID, _t.Optional[UUID]]:
         """ Creates the map for the keylist reorganzation.
 
         Each key of the returned dictionary is a resource uuid pointing to the
         resource uuid it should be moved to. If the allocation should not be
-        moved they key-value is None.
+        moved then key-value is None.
 
         """
         masters = [a for a in allocations if a.is_master]
         assert len(masters) == 1
 
         master = masters[0]
-        allocations = dict(((a.resource, a) for a in allocations))
+        allocation_from_key = {a.resource: a for a in allocations}
 
         # generate the keylist (the allocation resources may be unordered)
         keylist = [master.resource]
         keylist.extend(utils.generate_uuids(master.resource, master.quota))
 
         # prefill the map
-        reordered = dict(((k, None) for k in keylist))
+        reordered: _t.Dict[UUID, _t.Optional[UUID]] = {
+            k: None
+            for k in keylist
+        }
 
         # each free allocation increases the offset by which the next key
         # for a non-free allocation is acquired
         offset = 0
         for ix, key in enumerate(keylist):
-            if allocations[key].is_available():
+            if allocation_from_key[key].is_available():
                 offset += 1
             else:
                 reordered[key] = keylist[ix - offset]
 
         return reordered
 
-    def availability(self, start=None, end=None):
+    def availability(
+        self,
+        start: _t.Optional[datetime] = None,
+        end: _t.Optional[datetime] = None
+    ) -> float:
         """Goes through all allocations and sums up the availability."""
 
         start = start if start else sedate.mindatetime
         end = end if end else sedate.maxdatetime
 
         start, end = self._prepare_range(start, end)
 
         return self.queries.availability_by_range(start, end, [self.resource])
 
     def move_allocation(
-            self, master_id, new_start=None, new_end=None,
-            group=None, new_quota=None, approve_manually=None,
-            quota_limit=0, whole_day=None, data=missing):
+        self,
+        master_id: int,
+        new_start: _t.Optional[datetime] = None,
+        new_end: _t.Optional[datetime] = None,
+        group: _t.Optional[UUID] = None,
+        new_quota: _t.Optional[int] = None,
+        approve_manually: _t.Optional[bool] = None,
+        quota_limit: int = 0,
+        whole_day: _t.Optional[bool] = None,
+        data: _t.Optional[_t.Any] = missing
+    ) -> None:
 
         assert master_id
         assert any([new_start and new_end, group, new_quota])
 
-        new_start, new_end = self._prepare_range(new_start, new_end)
+        if new_start is not None and new_end is not None:
+            new_start, new_end = self._prepare_range(new_start, new_end)
 
         # Find allocation
         master = self.allocation_by_id(master_id)
         mirrors = self.allocation_mirrors_by_master(master)
 
         changing = [master] + mirrors
         ids = [c.id for c in changing]
@@ -635,15 +758,15 @@
             new_start, new_end = sedate.align_range_to_day(
                 new_start, new_end, self.timezone
             )
 
         if new_end < new_start:
             raise errors.InvalidAllocationError
 
-        new = self.allocation_cls(
+        new = self.allocation_cls(  # type:ignore[misc]
             start=new_start,
             end=new_end,
             raster=master.raster,
             timezone=self.timezone
         )
 
         # Ensure that the new span does not overlap an existing one
@@ -704,16 +827,37 @@
             change.start = new.start
             change.end = new.end
             change.group = group or master.group
 
             if data is not missing:
                 change.data = data
 
-    def remove_allocation(self, id=None, groups=None):
+    @_t.overload
+    def remove_allocation(self, id: int) -> None: ...
+
+    @_t.overload
+    def remove_allocation(
+        self,
+        id: None = ...,
+        *,
+        groups: _t.Collection[UUID]
+    ) -> None: ...
+
+    def remove_allocation(
+        self,
+        id: _t.Optional[int] = None,
+        groups: _t.Optional[_t.Collection[UUID]] = None
+    ) -> None:
+
+        allocations: _t.Iterable[Allocation]
         if id:
+            # FIXME: We probably should `assert groups is None`
+            #        since the parameter does nothing if `id` is
+            #        given. But we might break some existing code
+            #        which has been using this incorrectly...
             master = self.allocation_by_id(id)
             allocations = [master]
             allocations.extend(self.allocation_mirrors_by_master(master))
         elif groups:
             allocations = self.allocations_by_groups(
                 groups, masters_only=False
             )
@@ -742,17 +886,20 @@
                 )
 
         for allocation in allocations:
             if not allocation.is_transient:
                 self.session.delete(allocation)
 
     def remove_unused_allocations(
-        self, start, end,
-        days=None, exclude_groups=False
-    ):
+        self,
+        start: datetime,
+        end: datetime,
+        days: _t.Optional[_t.Iterable[_t.Union['Day', 'DayNumber']]] = None,
+        exclude_groups: bool = False
+    ) -> int:
         """ Removes all allocations without reservations between start and
         end and returns the number of allocations that were deleted.
 
         Groups which are partially inside the daterange are not included.
 
         :days:
             List of days which should be considered, a subset of:
@@ -768,23 +915,29 @@
         """
 
         start, end = self._prepare_range(
             sedate.as_datetime(start),
             sedate.as_datetime(end)
         )
 
+        day_numbers: _t.Optional[_t.Set[DayNumber]] = None
         if days:
             # get the day from the map - if impossible take the verbatim value
             # this allows for using strings or integers
-            days = {DAYS_MAP.get(day, day) for day in days}
-            if days.issuperset(DAYS_MAP.values()):
+            day_numbers = {
+                DAYS_MAP.get(day, day)  # type:ignore[arg-type]
+                for day in days
+            }
+            if day_numbers.issuperset(DAYS_MAP.values()):
                 # if all days are allowed we just unset the filter
-                days = None
+                day_numbers = None
 
             exclude_groups = True
+        else:
+            day_numbers = None
 
         # all the slots
         slots = self.managed_reserved_slots()
         slots = slots.with_entities(ReservedSlot.allocation_id)
 
         # all the reservations
         reservations = self.managed_reservations()
@@ -826,39 +979,76 @@
         candidates = candidates.filter(
             not_(Allocation.group.in_(reservations))
         )
 
         # .. including only the groups fully inside the required scope
         allocations = candidates.filter(Allocation.group.in_(groups))
 
-        if not days:
+        if not day_numbers:
             # we can just emit a simple DELETE query
             return allocations.delete('fetch')
 
         # we need to filter by weekday which we cannot easily do in SQL
         # so we fetch first and delete the allocations that match
         deleted = 0
         for allocation in allocations:
-            if allocation.display_start().weekday() not in days:
+            if allocation.display_start().weekday() not in day_numbers:
                 continue
 
             self.session.delete(allocation)
             deleted += 1
         return deleted
 
+    @_t.overload
     def reserve(
         self,
-        email,
-        dates=None,
-        group=None,
-        data=None,
-        session_id=None,
-        quota=1,
-        single_token_per_session=False
-    ):
+        email: str,
+        dates: _t.Union['_dtrange', _t.Collection['_dtrange']],
+        group: None = ...,
+        data: _t.Optional[_t.Any] = ...,
+        session_id: _t.Optional[UUID] = ...,
+        quota: int = ...,
+        single_token_per_session: bool = ...
+    ) -> UUID: ...
+
+    @_t.overload
+    def reserve(
+        self,
+        email: str,
+        dates: None,
+        group: UUID,
+        data: _t.Optional[_t.Any] = ...,
+        session_id: _t.Optional[UUID] = ...,
+        quota: int = ...,
+        single_token_per_session: bool = ...
+    ) -> UUID: ...
+
+    @_t.overload
+    def reserve(
+        self,
+        email: str,
+        dates: None = ...,
+        *,
+        group: UUID,
+        data: _t.Optional[_t.Any] = ...,
+        session_id: _t.Optional[UUID] = ...,
+        quota: int = ...,
+        single_token_per_session: bool = ...
+    ) -> UUID: ...
+
+    def reserve(
+        self,
+        email: str,
+        dates: _t.Union['_dtrange', _t.Collection['_dtrange'], None] = None,
+        group: _t.Optional[UUID] = None,
+        data: _t.Optional[_t.Any] = None,
+        session_id: _t.Optional[UUID] = None,
+        quota: int = 1,
+        single_token_per_session: bool = False
+    ) -> UUID:
         """ Reserves one or many allocations. Returns a token that needs
         to be passed to :meth:`approve_reservations` to complete the
         reservation.
 
         That is to say, Libres uses a two-step reservation process. The first
         step is reserving what is either an open spot or a place on the
         waiting list (see ``approve_manually`` of
@@ -939,14 +1129,15 @@
 
         if not self.validate_email(email):
             raise errors.InvalidEmailAddress
 
         if group:
             dates = self.allocation_dates_by_group(group)
 
+        assert dates is not None
         dates = self._prepare_dates(dates)
         timezone = self.timezone
 
         # First, the request is checked for saneness. If any requested
         # date cannot be reserved the request as a whole fails.
         for start, end in dates:
 
@@ -992,36 +1183,40 @@
         # ok, we're good to go
         if single_token_per_session and session_id:
             existing = self.queries.reservations_by_session(session_id).first()
             token = existing and existing.token or new_uuid()
         else:
             token = new_uuid()
 
-        reservations = []
-
         # groups are reserved by group-identifier - so all members of a group
         # or none of them. As such there's no start / end date which is defined
         # implicitly by the allocation
-        def new_reservations_by_group(group):
+        def new_reservations_by_group(
+            group: _t.Optional[UUID]
+        ) -> _t.Iterator[Reservation]:
+
             if group:
                 reservation = self.reservation_cls()
                 reservation.token = token
                 reservation.target = group
-                reservation.status = u'pending'
-                reservation.target_type = u'group'
+                reservation.status = 'pending'
+                reservation.target_type = 'group'
                 reservation.resource = self.resource
                 reservation.data = data
                 reservation.session_id = session_id
                 reservation.email = email.strip()
                 reservation.quota = quota
 
                 yield reservation
 
         # all other reservations are reserved by start/end date
-        def new_reservations_by_dates(dates):
+        def new_reservations_by_dates(
+            dates: _t.List[_t.Tuple[datetime, datetime]]
+        ) -> _t.Iterator[Reservation]:
+
             already_reserved_groups = set()
 
             for start, end in dates:
                 for allocation in self.allocations_in_range(start, end):
                     if allocation.group in already_reserved_groups:
                         continue
 
@@ -1029,28 +1224,26 @@
                         continue
 
                     # automatically reserve the whole group if the allocation
                     # is part of a group
                     if allocation.in_group:
                         already_reserved_groups.add(allocation.group)
 
-                        # I really want to use 'yield from'. Python 3 ftw!
-                        for r in new_reservations_by_group(allocation.group):
-                            yield r
+                        yield from new_reservations_by_group(allocation.group)
                     else:
                         reservation = self.reservation_cls()
                         reservation.token = token
                         reservation.start, reservation.end\
                             = rasterizer.rasterize_span(
                                 start, end, allocation.raster
                             )
                         reservation.timezone = allocation.timezone
                         reservation.target = allocation.group
-                        reservation.status = u'pending'
-                        reservation.target_type = u'allocation'
+                        reservation.status = 'pending'
+                        reservation.target_type = 'allocation'
                         reservation.resource = self.resource
                         reservation.data = data
                         reservation.session_id = session_id
                         reservation.email = email.strip()
                         reservation.quota = quota
 
                         yield reservation
@@ -1067,34 +1260,41 @@
         # have a very simple overlap check for reservations, it's not important
         # that this catches *all* possible problems - that's being handled
         # by the reservation slots - but it should stop us from adding the same
         # reservation twice on a single session
         if session_id:
             found = self.queries.reservations_by_session(session_id)
             found = found.with_entities(Reservation.target, Reservation.start)
-            found = set(found.all())
+            found_set = set(found)
 
             for reservation in reservations:
-                if (reservation.target, reservation.start) in found:
+                if (reservation.target, reservation.start) in found_set:
                     raise errors.OverlappingReservationError
 
         for reservation in reservations:
             self.session.add(reservation)
 
         events.on_reservations_made(self.context, reservations)
 
         return token
 
-    def _approve_reservation_record(self, reservation):
+    def _approve_reservation_record(
+        self,
+        reservation: Reservation
+    ) -> _t.List[ReservedSlot]:
+
         # write out the slots
         slots_to_reserve = []
 
-        if reservation.target_type == u'group':
+        dates: _t.Union[_t.Tuple['_dtrange', ...], _t.List['_dtrange']]
+        if reservation.target_type == 'group':
             dates = self.allocation_dates_by_group(reservation.target)
         else:
+            assert reservation.start is not None
+            assert reservation.end is not None
             dates = ((reservation.start, reservation.end),)
 
         # the reservation quota is simply implemented by multiplying the
         # dates which are approved
 
         dates = dates * reservation.quota
 
@@ -1116,22 +1316,22 @@
                     slots_to_reserve.append(slot)
 
                 # the allocation may be a fake one, in which case we
                 # must make it realz yo
                 if allocation.is_transient:
                     self.session.add(allocation)
 
-        reservation.status = u'approved'
+        reservation.status = 'approved'
 
         if not slots_to_reserve:
             raise errors.NotReservableError
 
         return slots_to_reserve
 
-    def approve_reservations(self, token):
+    def approve_reservations(self, token: UUID) -> _t.List[ReservedSlot]:
         """ This function approves an existing reservation and writes the
         reserved slots accordingly.
 
         Returns a list with the reserved slots.
 
         """
 
@@ -1148,30 +1348,34 @@
                 e.reservation = reservation
                 raise e
 
         events.on_reservations_approved(self.context, reservations)
 
         return slots_to_reserve
 
-    def deny_reservation(self, token):
+    def deny_reservation(self, token: UUID) -> None:
         """ Denies a pending reservation, removing it from the records and
         sending an email to the reservee.
 
         """
 
         query = self.reservations_by_token(token)
-        query = query.filter(Reservation.status == u'pending')
+        query = query.filter(Reservation.status == 'pending')
 
         reservations = query.all()
 
         query.delete()
 
         events.on_reservations_denied(self.context, reservations)
 
-    def remove_reservation(self, token, id=None):
+    def remove_reservation(
+        self,
+        token: UUID,
+        id: _t.Optional[int] = None
+    ) -> None:
         """ Removes all reserved slots of the given reservation token.
 
         Note that removing a reservation does not let the reservee know that
         his reservation has been removed.
 
         If you want to let the reservee know what happened,
         use revoke_reservation.
@@ -1192,25 +1396,32 @@
             self.session.delete(reservation)
 
         # some allocations still reference reserved_slots if not for this
         self.session.expire_all()
 
         events.on_reservations_removed(self.context, reservations)
 
-    def change_email(self, token, new_email):
+    def change_email(self, token: UUID, new_email: str) -> None:
 
         for reservation in self.reservations_by_token(token).all():
             reservation.email = new_email
 
-    def change_reservation_data(self, token, data):
+    def change_reservation_data(
+        self,
+        token: UUID,
+        data: _t.Optional[_t.Any]
+    ) -> None:
 
         for reservation in self.reservations_by_token(token).all():
             reservation.data = data
 
-    def change_reservation_time_candidates(self, tokens=None):
+    def change_reservation_time_candidates(
+        self,
+        tokens: _t.Optional[_t.Collection[UUID]] = None
+    ) -> 'Query[Reservation]':
         """ Returns the reservations that fullfill the restrictions
         imposed by change_reservation_time.
 
         Pass a list of reservation tokens to further limit the results.
 
         """
 
@@ -1224,30 +1435,50 @@
         query = query.filter(Reservation.target.in_(groups))
 
         if tokens:
             query = query.filter(Reservation.token.in_(tokens))
 
         return query
 
-    def change_reservation_time(self, token, id, new_start, new_end):
+    def change_reservation_time(
+        self,
+        token: UUID,
+        id: int,
+        new_start: datetime,
+        new_end: datetime
+    ) -> _t.Optional[Reservation]:
         """ Kept for backwards compatibility, use :meth:`change_reservation`
         instead.
 
         """
+        import warnings
+        warnings.warn(
+            'change_reservation_time is deprecated and will be removed '
+            'in a future version, please use change_reservation instead.',
+            DeprecationWarning,
+            stacklevel=2
+        )
         return self.change_reservation(token, id, new_start, new_end)
 
-    def change_reservation(self, token, id, new_start, new_end, quota=None):
+    def change_reservation(
+        self,
+        token: UUID,
+        id: int,
+        new_start: datetime,
+        new_end: datetime,
+        quota: _t.Optional[int] = None
+    ) -> _t.Optional[Reservation]:
         """ Allows to change the timespan of a reservation under certain
         conditions:
 
         - The new timespan must be reservable inside the existing allocation.
           (So you cannot use this method to reserve another allocation)
         - The referenced allocation must not be in a group.
 
-        Returns True if a change was made.
+        Returns the new reservation if a change was made and None instead.
 
         Just like revoke_reservation, this function raises an event which
         includes a send_email flag and a reason which may be used to inform
         the user of the changes to his reservation.
 
         """
 
@@ -1260,31 +1491,33 @@
 
         # if there's nothing to change, do not change
         if quota is None or existing_reservation.quota == quota:
             if existing_reservation.start == new_start:
                 ends = (new_end, new_end - timedelta(microseconds=1))
 
                 if existing_reservation.end in ends:
-                    return False
+                    return None
 
         # will return raise a MultipleResultsFound exception if this is a group
         if existing_reservation.status == 'approved':
             allocation = self.allocations_by_reservation(token, id).one()
         else:
-            allocation = existing_reservation._target_allocations().first()
+            _allocation = existing_reservation._target_allocations().first()
+            assert _allocation is not None
+            allocation = _allocation
 
         if not allocation.contains(new_start, new_end):
             raise errors.TimerangeTooLong()
 
-        reservation_arguments = dict(
-            email=existing_reservation.email,
-            dates=(new_start, new_end),
-            data=existing_reservation.data,
-            quota=quota or existing_reservation.quota
-        )
+        reservation_arguments: '_ReserveArgs' = {
+            'email': existing_reservation.email,
+            'dates': (new_start, new_end),
+            'data': existing_reservation.data,
+            'quota': quota or existing_reservation.quota
+        }
 
         old_start = existing_reservation.display_start()
         old_end = existing_reservation.display_end()
 
         with self.begin_nested():
             self.remove_reservation(token, id)
 
@@ -1306,22 +1539,24 @@
                     new_reservation.display_end()
                 ),
             )
 
         return new_reservation
 
     def search_allocations(
-        self, start, end,
-        days=None,
-        minspots=0,
-        available_only=False,
-        whole_day='any',
-        groups='any',
-        strict=False
-    ):
+        self,
+        start: datetime,
+        end: datetime,
+        days: _t.Optional[_t.Collection[_t.Union[Day, DayNumber]]] = None,
+        minspots: int = 0,
+        available_only: bool = False,
+        whole_day: _t.Literal['any', 'yes', 'no'] = 'any',
+        groups: _t.Literal['any', 'yes', 'no'] = 'any',
+        strict: bool = False
+    ) -> _t.List[Allocation]:
         """ Search allocations using a number of options. The date is split
         into date/time. All allocations between start and end date within
         the given time (on each day) are included.
 
         For example, start=01.01.2012 12:00 end=31.01.2012 14:00 will include
         all allocations in January 2012 which OVERLAP the given times. So an
         allocation starting at 11:00 and ending at 12:00 will be included!
@@ -1381,18 +1616,24 @@
         assert end
 
         start, end = self._prepare_range(start, end)
 
         assert whole_day in ('yes', 'no', 'any')
         assert groups in ('yes', 'no', 'any')
 
+        day_numbers: _t.Optional[_t.Set[DayNumber]]
         if days:
             # get the day from the map - if impossible take the verbatim value
             # this allows for using strings or integers
-            days = {DAYS_MAP.get(day, day) for day in days}
+            day_numbers = {
+                DAYS_MAP.get(day, day)  # type:ignore[arg-type]
+                for day in days
+            }
+        else:
+            day_numbers = None
 
         query = self.allocations_in_range(start, end)
         query = query.order_by(Allocation._start)
 
         allocations = []
 
         known_groups = set()
@@ -1402,22 +1643,23 @@
 
             if not self.is_allocation_exposed(allocation):
                 continue
 
             s = datetime.combine(allocation.start.date(), start.time())
             e = datetime.combine(allocation.end.date(), end.time())
 
-            s = sedate.replace_timezone(s, allocation.start.tzname())
-            e = sedate.replace_timezone(e, allocation.start.tzname())
+            # the raw dates will be UTC
+            s = sedate.replace_timezone(s, 'UTC')
+            e = sedate.replace_timezone(e, 'UTC')
 
             if not allocation.overlaps(s, e):
                 continue
 
-            if days:
-                if allocation.display_start().weekday() not in days:
+            if day_numbers:
+                if allocation.display_start().weekday() not in day_numbers:
                     continue
 
             if whole_day != 'any':
                 if whole_day == 'yes' and not allocation.whole_day:
                     continue
                 if whole_day == 'no' and allocation.whole_day:
                     continue
@@ -1465,22 +1707,27 @@
 
         if not strict and groups != 'no' and known_ids and known_groups:
             query = self.managed_allocations()
             query = query.filter(not_(Allocation.id.in_(known_ids)))
             query = query.filter(Allocation.group.in_(known_groups))
 
             for allocation in query.all():
-                allocation.is_extra_result = True
+                allocation.is_extra_result = True  # type:ignore[attr-defined]
                 allocations.append(allocation)
 
-            allocations.sort(key=lambda a: a._start)
+            allocations.sort(key=attrgetter('_start'))
 
         return allocations
 
-    def free_allocations_count(self, master_allocation, start, end):
+    def free_allocations_count(
+        self,
+        master_allocation: Allocation,
+        start: datetime,
+        end: datetime
+    ) -> int:
         """ Returns the number of free allocations between master_allocation
         and it's mirrors.
 
         """
 
         free_allocations = 0
 
@@ -1492,15 +1739,19 @@
 
         for mirror in self.allocation_mirrors_by_master(master_allocation):
             if mirror.is_available(start, end):
                 free_allocations += 1
 
         return free_allocations
 
-    def reservation_targets(self, start, end):
+    def reservation_targets(
+        self,
+        start: datetime,
+        end: datetime
+    ) -> _t.List[Allocation]:
         """ Returns a list of allocations that are free within start and end.
         These allocations may come from the master or any of the mirrors.
 
         """
         targets = []
 
         query = self.queries.all_allocations_in_range(start, end)
@@ -1516,51 +1767,63 @@
             if not found:
                 raise errors.AlreadyReservedError
 
             targets.append(found)
 
         return targets
 
-    def reserved_slots_by_reservation(self, token, id=None):
+    def reserved_slots_by_reservation(
+        self,
+        token: UUID,
+        id: _t.Optional[int] = None
+    ) -> 'Query[ReservedSlot]':
         """ Returns all reserved slots of the given reservation.
         The id is optional and may be used only return the slots from a
         specific reservation matching token and id.
         """
 
         assert token
 
         query = self.managed_reserved_slots()
         query = query.filter(ReservedSlot.reservation_token == token)
 
         if id is None:
             return query
         else:
-            ids = self.allocations_by_reservation(token, id)
-            ids = ids.with_entities(Allocation.id)
+            allocations = self.allocations_by_reservation(token, id)
+            ids = allocations.with_entities(Allocation.id)
             return query.filter(ReservedSlot.allocation_id.in_(ids))
 
-    def reservations_by_group(self, group):
+    def reservations_by_group(self, group: UUID) -> 'Query[Reservation]':
         tokens = self.managed_reservations().with_entities(Reservation.token)
         tokens = tokens.filter(Reservation.target == group)
 
         return self.managed_reservations().filter(
             Reservation.token.in_(tokens)
         )
 
-    def reservations_by_allocation(self, allocation_id):
-        master = self.allocation_by_id(allocation_id)
+    def reservations_by_allocation(
+        self,
+        allocation_id: int
+    ) -> 'Query[Reservation]':
 
+        master = self.allocation_by_id(allocation_id)
         return self.reservations_by_group(master.group)
 
-    def reservations_by_token(self, token, id=None):
+    def reservations_by_token(
+        self,
+        token: UUID,
+        id: _t.Optional[int] = None
+    ) -> 'Query[Reservation]':
+
         query = self.managed_reservations()
         query = query.filter(Reservation.token == token)
 
         if id:
             query = query.filter(Reservation.id == id)
 
         try:
             query.first()
         except exc.NoResultFound:
-            raise errors.InvalidReservationToken
+            raise errors.InvalidReservationToken from None
 
         return query
```

### Comparing `libres-0.6.1/libres/modules/rasterizer.py` & `libres-0.7.0/src/libres/modules/rasterizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,57 +23,73 @@
 or 19:29 (end). The end time is actually 19:30 minus one microsecond.
 
 If we now have a key on the start time and this time is rastered we can block
 overlapping reservations on the database level.
 
 """
 
-from datetime import timedelta
+from datetime import datetime, timedelta
+
+
+import typing as _t
+if _t.TYPE_CHECKING:
+    from typing_extensions import TypeGuard
+
+
+Raster = _t.Literal[5, 10, 15, 30, 60]
 
 # The raster values must divide an hour without any remaining minutes
-VALID_RASTER = (5, 10, 15, 30, 60)
-MIN_RASTER = min(VALID_RASTER)
-MAX_RASTER = max(VALID_RASTER)
+VALID_RASTER: _t.Tuple[Raster, ...] = (5, 10, 15, 30, 60)
+MIN_RASTER: Raster = min(VALID_RASTER)
+MAX_RASTER: Raster = max(VALID_RASTER)
 
 
-def is_valid_raster(raster):
+def is_valid_raster(raster: int) -> 'TypeGuard[Raster]':
     return raster in VALID_RASTER
 
 
-def rasterize_start(date, raster):
+def rasterize_start(date: datetime, raster: Raster) -> datetime:
     """Get a date and snap it to the beginning of the raster."""
 
     assert is_valid_raster(raster)
 
     delta = timedelta(minutes=date.minute % raster,
                       seconds=date.second,
                       microseconds=date.microsecond)
 
     return date - delta
 
 
-def rasterize_end(date, raster):
+def rasterize_end(date: datetime, raster: Raster) -> datetime:
     """Get a date and snap it to the end of the raster. Note that
     the resulting time is the start of the next raster minus one microsecond.
 
     """
     if date.minute % raster:
         date = rasterize_start(date, raster)
         delta = timedelta(microseconds=-1, minutes=raster)
     else:
         delta = timedelta(microseconds=-1)
     return date + delta
 
 
-def rasterize_span(start, end, raster):
+def rasterize_span(
+    start: datetime,
+    end: datetime,
+    raster: Raster
+) -> _t.Tuple[datetime, datetime]:
     """Rasterizes both a start and an end date."""
     return rasterize_start(start, raster), rasterize_end(end, raster)
 
 
-def iterate_span(start, end, raster):
+def iterate_span(
+    start: datetime,
+    end: datetime,
+    raster: Raster
+) -> '_t.Iterator[_t.Tuple[datetime, datetime]]':
     """Iterates through all raster blocks within a certain timespan."""
     start, end = rasterize_span(start, end, raster)
 
     step = start
-    while (step <= end):
+    while step <= end:
         yield step, step + timedelta(microseconds=-1, minutes=raster)
         step += timedelta(seconds=raster * 60)
```

### Comparing `libres-0.6.1/libres/tests/test_allocation.py` & `libres-0.7.0/tests/test_allocation.py`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/libres/tests/test_registry.py` & `libres-0.7.0/tests/test_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
             self.result = self.registry.get_current_context().name
 
         def join(self):
             threading.Thread.join(self)
             return self.result
 
-    for i in range(0, 100):
+    for _ in range(0, 100):
 
         threads = [
             Application('one', r),
             Application('two', r),
             Application('three', r),
             Application('four', r)
         ]
```

### Comparing `libres-0.6.1/libres/tests/test_reservation.py` & `libres-0.7.0/tests/test_reservation.py`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/libres/tests/test_reserved_slot.py` & `libres-0.7.0/tests/test_reserved_slot.py`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/libres/tests/test_scheduler.py` & `libres-0.7.0/tests/test_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sedate
 
 from copy import copy
 from datetime import date, datetime, timedelta, time
 from libres.db.models import Reservation, Allocation
 from libres.modules import errors, events
 from libres.modules import utils
-from mock import Mock
+from unittest.mock import Mock
 from sqlalchemy.exc import StatementError
 from sqlalchemy.orm.exc import MultipleResultsFound
 from uuid import uuid4 as new_uuid
 
 
 def test_rollback(scheduler):
 
@@ -310,15 +310,15 @@
 
     # 1 hour / 15 min = 4
     possible_dates = list(allocation.all_slots())
     assert len(possible_dates) == 4
 
     # reserve half of the slots
     time = (datetime(2011, 1, 1, 15), datetime(2011, 1, 1, 15, 30))
-    token = scheduler.reserve(u'test@example.org', time)
+    token = scheduler.reserve('test@example.org', time)
     slots = scheduler.approve_reservations(token)
 
     assert len(slots) == 2
 
     # commit the changes (or we'll hit the db, which at this point is dirty,
     # resulting in a DirtyReadOnlySession exception)
     scheduler.commit()
@@ -371,40 +371,40 @@
             datetime(2011, 1, 1, 15), datetime(2011, 1, 1, 16),
             datetime(2011, 1, 2, 15), datetime(2011, 1, 2, 16)
         ),
         quota=1
     )
 
     token1 = scheduler.reserve(
-        email=u'test@example.org',
+        email='test@example.org',
         dates=(a1.start, a1.end),
         session_id=session_id,
         single_token_per_session=True
     )
 
     token2 = scheduler.reserve(
-        email=u'test@example.org',
+        email='test@example.org',
         dates=(a2.start, a2.end),
         session_id=session_id,
         single_token_per_session=True
     )
 
     assert token1 == token2
 
     scheduler.remove_reservation(token1)
 
     token3 = scheduler.reserve(
-        email=u'test@example.org',
+        email='test@example.org',
         dates=(a1.start, a1.end),
         session_id=session_id,
         single_token_per_session=True
     )
 
     token4 = scheduler.reserve(
-        email=u'test@example.org',
+        email='test@example.org',
         dates=(a2.start, a2.end),
         session_id=session_id,
         single_token_per_session=True
     )
 
     assert token1 != token3
     assert token3 == token4
@@ -414,105 +414,105 @@
     # reserve multiple allocations
     dates = (
         (datetime(2014, 8, 7, 11, 0), datetime(2014, 8, 7, 12, 0)),
         (datetime(2014, 8, 8, 11, 0), datetime(2014, 8, 8, 12, 0))
     )
 
     scheduler.allocate(dates)
-    token = scheduler.reserve(u'original@example.org', dates)
+    token = scheduler.reserve('original@example.org', dates)
     scheduler.commit()
 
     assert [r.email for r in scheduler.reservations_by_token(token)]\
-        == [u'original@example.org'] * 2
+        == ['original@example.org'] * 2
 
     # change the email and ensure that all reservation records are changed
-    scheduler.change_email(token, u'newmail@example.org')
+    scheduler.change_email(token, 'newmail@example.org')
     scheduler.commit()
 
     assert [r.email for r in scheduler.reservations_by_token(token)]\
-        == [u'newmail@example.org'] * 2
+        == ['newmail@example.org'] * 2
 
     # approve the reservation and change again
     scheduler.approve_reservations(token)
-    scheduler.change_email(token, u'another@example.org')
+    scheduler.change_email(token, 'another@example.org')
     scheduler.commit()
 
     assert [r.email for r in scheduler.reservations_by_token(token)]\
-        == [u'another@example.org'] * 2
+        == ['another@example.org'] * 2
 
 
 def test_change_reservation_assertions(scheduler):
     reservation_changed = Mock()
     events.on_reservation_time_changed.append(reservation_changed)
 
     dates = (datetime(2014, 8, 7, 8, 0), datetime(2014, 8, 7, 17, 0))
 
     scheduler.allocate(dates, partly_available=False)
-    token = scheduler.reserve(u'original@example.org', dates)
+    token = scheduler.reserve('original@example.org', dates)
     scheduler.commit()
 
     reservation = scheduler.reservations_by_token(token).one()
     scheduler.approve_reservations(token)
     scheduler.commit()
 
     dates = (
         (datetime(2014, 8, 10, 11, 0), datetime(2014, 8, 10, 12, 0)),
         (datetime(2014, 8, 11, 11, 0), datetime(2014, 8, 11, 12, 0))
     )
 
     scheduler.allocate(dates, grouped=True)
-    token = scheduler.reserve(u'original@example.org', dates)
+    token = scheduler.reserve('original@example.org', dates)
     scheduler.commit()
 
     reservation = scheduler.reservations_by_token(token).one()
     scheduler.approve_reservations(token)
     scheduler.commit()
 
     with pytest.raises(MultipleResultsFound):
-        scheduler.change_reservation_time(
+        scheduler.change_reservation(
             token, reservation.id, datetime.now(), datetime.now()
         )
 
     assert scheduler.change_reservation_time_candidates().count() == 0
     assert not reservation_changed.called
 
     # fail if the dates are outside the allocation
     dates = (datetime(2014, 3, 7, 8, 0), datetime(2014, 3, 7, 17, 0))
 
     scheduler.allocate(dates, partly_available=True)
-    token = scheduler.reserve(u'original@example.org', dates)
+    token = scheduler.reserve('original@example.org', dates)
     scheduler.commit()
 
     reservation = scheduler.reservations_by_token(token).one()
     scheduler.approve_reservations(token)
     scheduler.commit()
 
     assert scheduler.change_reservation_time_candidates().count() == 1
     assert not reservation_changed.called
 
     # make sure that the timerange given fits inside the allocation
     with pytest.raises(errors.TimerangeTooLong):
-        scheduler.change_reservation_time(
+        scheduler.change_reservation(
             token, reservation.id,
             datetime(2014, 3, 7, 7, 0), datetime(2014, 3, 7, 17, 0)
         )
 
     with pytest.raises(errors.TimerangeTooLong):
-        scheduler.change_reservation_time(
+        scheduler.change_reservation(
             token, reservation.id,
             datetime(2014, 3, 7, 8, 0), datetime(2014, 3, 7, 17, 1)
         )
 
 
 def test_change_unapproved_reservation_quota(scheduler):
     dates = (datetime(2014, 8, 7, 8, 0), datetime(2014, 8, 7, 10, 0))
     scheduler.allocate(dates, quota=2)
 
     token = scheduler.reserve(
-        u'original@example.org', dates, session_id=new_uuid().hex
+        'original@example.org', dates, session_id=new_uuid().hex
     )
 
     scheduler.commit()
 
     reservation = scheduler.reservations_by_token(token).one()
     assert not scheduler.change_reservation(
         token=token,
@@ -542,45 +542,45 @@
     dates = (datetime(2014, 8, 7, 8, 0), datetime(2014, 8, 7, 10, 0))
 
     scheduler.allocate(dates, partly_available=True)
 
     data = {
         'foo': 'bar'
     }
-    token = scheduler.reserve(u'original@example.org', (
+    token = scheduler.reserve('original@example.org', (
         datetime(2014, 8, 7, 8, 0), datetime(2014, 8, 7, 9)
     ), data=data)
 
     scheduler.commit()
 
     reservation = scheduler.reservations_by_token(token).one()
     original_id = reservation.id
 
     scheduler.approve_reservations(token)
     scheduler.commit()
 
     assert scheduler.change_reservation_time_candidates().count() == 1
 
     # make sure that no changes are made in these cases
-    assert not scheduler.change_reservation_time(
+    assert not scheduler.change_reservation(
         token, reservation.id,
         datetime(2014, 8, 7, 8, 0),
         datetime(2014, 8, 7, 9)
     )
 
-    assert not scheduler.change_reservation_time(
+    assert not scheduler.change_reservation(
         token, reservation.id,
         datetime(2014, 8, 7, 8, 0),
         datetime(2014, 8, 7, 9) - timedelta(microseconds=1)
     )
 
     assert not reservation_changed.called
 
     # make sure the change is propagated
-    scheduler.change_reservation_time(
+    scheduler.change_reservation(
         token, reservation.id,
         datetime(2014, 8, 7, 8, 0),
         datetime(2014, 8, 7, 10)
     )
     scheduler.commit()
 
     assert reservation_changed.called
@@ -598,32 +598,32 @@
     assert reservation.end == sedate.standardize_date(
         datetime(2014, 8, 7, 10, 0) - timedelta(microseconds=1),
         scheduler.timezone
     )
 
     # the data must stay the same
     assert reservation.data == data
-    assert reservation.email == u'original@example.org'
+    assert reservation.email == 'original@example.org'
     assert reservation.id == original_id
     assert reservation.token == token
 
-    scheduler.change_reservation_time(
+    scheduler.change_reservation(
         token, reservation.id,
         datetime(2014, 8, 7, 9, 0),
         datetime(2014, 8, 7, 10, 0)
     )
 
     scheduler.approve_reservations(
-        scheduler.reserve(u'original@example.org', (
+        scheduler.reserve('original@example.org', (
             datetime(2014, 8, 7, 8, 0), datetime(2014, 8, 7, 9)
         ))
     )
 
     with pytest.raises(errors.AlreadyReservedError):
-        scheduler.change_reservation_time(
+        scheduler.change_reservation(
             token, reservation.id,
             datetime(2014, 8, 7, 8, 0),
             datetime(2014, 8, 7, 10, 0)
         )
 
 
 def test_change_reservation_quota(scheduler):
@@ -632,21 +632,21 @@
     )
 
     scheduler.allocate(dates, partly_available=True, quota=2)
 
     # have three reservations, one occupying the whole allocation,
     # two others occupying one half each (1 + .5 +.5 = 2 (quota))
     tokens = [
-        scheduler.reserve(u'original@example.org', (
+        scheduler.reserve('original@example.org', (
             datetime(2014, 8, 7, 8, 0), datetime(2014, 8, 7, 10, 0)
         )),
-        scheduler.reserve(u'original@example.org', (
+        scheduler.reserve('original@example.org', (
             datetime(2014, 8, 7, 8, 0), datetime(2014, 8, 7, 9, 0)
         )),
-        scheduler.reserve(u'original@example.org', (
+        scheduler.reserve('original@example.org', (
             datetime(2014, 8, 7, 9, 0), datetime(2014, 8, 7, 10, 0)
         ))
     ]
     scheduler.commit()
 
     assert scheduler.change_reservation_time_candidates().count() == 0
 
@@ -656,36 +656,36 @@
     scheduler.commit()
 
     assert scheduler.change_reservation_time_candidates().count() == 3
     reservation = scheduler.reservations_by_token(tokens[2]).one()
 
     # with 100% occupancy we can't change one of the small reservations
     with pytest.raises(errors.AlreadyReservedError):
-        scheduler.change_reservation_time(
+        scheduler.change_reservation(
             tokens[2], reservation.id,
             datetime(2014, 8, 7, 8, 0),
             datetime(2014, 8, 7, 10, 0)
         )
 
     # ensure that the failed removal didn't affect the reservations
     # (a rollback should have occured)
     for token in tokens:
         assert scheduler.reservations_by_token(token).one().token == token
 
     # removing the big reservation allows us to scale the other two
     scheduler.remove_reservation(tokens[0])
 
-    assert scheduler.change_reservation_time(
+    assert scheduler.change_reservation(
         tokens[2], reservation.id,
         datetime(2014, 8, 7, 8, 0),
         datetime(2014, 8, 7, 10, 0)
     )
 
     reservation = scheduler.reservations_by_token(tokens[1]).one()
-    assert scheduler.change_reservation_time(
+    assert scheduler.change_reservation(
         tokens[1], reservation.id,
         datetime(2014, 8, 7, 8, 0),
         datetime(2014, 8, 7, 10, 0)
     )
 
 
 def test_group_reserve(scheduler):
@@ -700,15 +700,15 @@
 
     assert len(allocations) == 2
 
     group = allocations[0].group
 
     # reserve the same thing three times, which should yield equal results
     def reserve():
-        token = scheduler.reserve(u'test@example.com', group=group)
+        token = scheduler.reserve('test@example.com', group=group)
         scheduler.commit()
 
         reservation = scheduler.reservations_by_token(token).one()
 
         targets = reservation._target_allocations().all()
         assert len(targets) == 2
 
@@ -728,15 +728,15 @@
 
 
 def test_session_expiration(scheduler):
     session_id = new_uuid()
 
     start, end = datetime(2013, 5, 1, 13, 0), datetime(2013, 5, 1, 14)
     scheduler.allocate(dates=(start, end), approve_manually=True)
-    scheduler.reserve(u'test@example.com', (start, end), session_id=session_id)
+    scheduler.reserve('test@example.com', (start, end), session_id=session_id)
     scheduler.commit()
 
     created = sedate.utcnow()
 
     res = scheduler.session.query(Reservation)
     res = res.filter(Reservation.session_id == session_id)
     res.update({'created': created, 'modified': None})
@@ -774,15 +774,15 @@
 
 
 def test_session_removal(scheduler):
     start, end = datetime(2013, 9, 27, 9, 0), datetime(2013, 9, 27, 10)
     scheduler.allocate(dates=(start, end))
     session_id = new_uuid()
 
-    scheduler.reserve(u'test@example.org', (start, end), session_id=session_id)
+    scheduler.reserve('test@example.org', (start, end), session_id=session_id)
     scheduler.commit()
 
     assert scheduler.session.query(Reservation).count() == 1
     assert scheduler.session.query(Allocation).count() == 1
 
     scheduler.queries.remove_expired_reservation_sessions(
         expiration_date=sedate.utcnow() + timedelta(seconds=15 * 60)
@@ -802,28 +802,28 @@
     rstart = datetime(2012, 2, 1, 15, 0)
     rend = datetime(2012, 2, 1, 16, 0)
     rdates = (rstart, rend)
 
     scheduler.allocate(dates=adates, approve_manually=True)
 
     with pytest.raises(errors.InvalidReservationError):
-        scheduler.reserve(u'test@example.org', rdates)
+        scheduler.reserve('test@example.org', rdates)
 
 
 def test_waitinglist(scheduler):
     start = datetime(2012, 2, 29, 15, 0)
     end = datetime(2012, 2, 29, 19, 0)
     dates = (start, end)
 
     # let's create an allocation with a waitinglist
     allocation = scheduler.allocate(dates, approve_manually=True)[0]
     assert allocation.waitinglist_length == 0
 
     # reservation should work
-    approval_token = scheduler.reserve(u'test@example.org', dates)
+    approval_token = scheduler.reserve('test@example.org', dates)
     scheduler.commit()
 
     reservation = scheduler.reservations_by_token(approval_token).one()
 
     assert not reservation.autoapprovable
     assert allocation.is_available(start, end)
     assert allocation.waitinglist_length == 1
@@ -832,15 +832,15 @@
     scheduler.approve_reservations(approval_token)
     scheduler.commit()
 
     assert not allocation.is_available(start, end)
     assert allocation.waitinglist_length == 0
 
     # at this point we can only reserve, not approve
-    waiting_token = scheduler.reserve(u'test@example.org', dates)
+    waiting_token = scheduler.reserve('test@example.org', dates)
     with pytest.raises(errors.AlreadyReservedError):
         scheduler.approve_reservations(waiting_token)
 
     assert allocation.waitinglist_length == 1
 
     # try to illegally move the allocation now
     with pytest.raises(errors.AffectedReservationError):
@@ -875,16 +875,16 @@
 
     scheduler.commit()
 
     assert not a1.overlaps(*d2)
     assert not a2.overlaps(*d1)
 
     # expect no exceptions
-    scheduler.reserve(u'test@example.org', d2)
-    scheduler.reserve(u'test@example.org', d1)
+    scheduler.reserve('test@example.org', d2)
+    scheduler.reserve('test@example.org', d1)
 
 
 def test_waitinglist_group(scheduler):
     from dateutil.rrule import rrule, DAILY, MO
 
     days = list(rrule(
         DAILY, count=5, byweekday=(MO,), dtstart=datetime(2012, 1, 1)
@@ -902,32 +902,32 @@
         dates, grouped=True, approve_manually=True
     )
     assert len(allocations) == 5
 
     group = allocations[0].group
 
     # reserving groups is no different than single allocations
-    maintoken = scheduler.reserve(u'test@example.org', group=group)
+    maintoken = scheduler.reserve('test@example.org', group=group)
     scheduler.commit()
 
     reservation = scheduler.reservations_by_token(maintoken).one()
 
     assert not reservation.autoapprovable
 
     for allocation in allocations:
         assert allocation.waitinglist_length == 1
 
     scheduler.approve_reservations(maintoken)
     scheduler.commit()
 
-    token = scheduler.reserve(u'test@example.org', group=group)
+    token = scheduler.reserve('test@example.org', group=group)
     with pytest.raises(errors.AlreadyReservedError):
         scheduler.approve_reservations(token)
 
-    token = scheduler.reserve(u'test@example.org', group=group)
+    token = scheduler.reserve('test@example.org', group=group)
     with pytest.raises(errors.AlreadyReservedError):
         scheduler.approve_reservations(token)
 
     scheduler.remove_reservation(maintoken)
     scheduler.approve_reservations(token)
 
 
@@ -971,15 +971,15 @@
         for allocation in a.siblings():
             # can't check transient allocations for siblings as it requires
             # the session to be set -> this test worked in seantis.reservation
             # because it always operated under one session
             if not allocation.is_transient:
                 assert len(allocation.siblings()) == 2
 
-    token = scheduler.reserve(u'test@example.com', group=allocations[0].group)
+    token = scheduler.reserve('test@example.com', group=allocations[0].group)
     scheduler.approve_reservations(token)
     scheduler.commit()
 
     group_allocations = scheduler.allocations_by_group(
         allocations[0].group).all()
     assert len(group_allocations) == 2
 
@@ -995,15 +995,15 @@
         allocations[0].group).all()
     all = list(utils.flatten([a.siblings() for a in group_allocations]))
     assert scheduler.queries.availability_by_allocations(all) == 0.0
 
     scheduler.move_allocation(allocations[0].id, newstart, newend, new_quota=2)
     scheduler.commit()
 
-    token = scheduler.reserve(u'test@example.com', group=allocations[0].group)
+    token = scheduler.reserve('test@example.com', group=allocations[0].group)
     scheduler.approve_reservations(token)
     scheduler.commit()
 
     group_allocations = scheduler.allocations_by_group(
         allocations[0].group).all()
     all = list(utils.flatten([a.siblings() for a in group_allocations]))
     assert scheduler.queries.availability_by_allocations(all) == 0.0
@@ -1028,56 +1028,56 @@
 
     assert allocation.waitinglist_length == 0
 
     # the first reservation kinda gets us in a waiting list, though
     # this time there can be only one spot in the list as long as there's
     # no reservation
 
-    token = scheduler.reserve(u'test@example.org', dates)
+    token = scheduler.reserve('test@example.org', dates)
     scheduler.commit()
 
     assert scheduler.reservations_by_token(token).one().autoapprovable
     scheduler.approve_reservations(token)
     scheduler.commit()
 
     # it is now that we should have a problem reserving
     with pytest.raises(errors.AlreadyReservedError):
-        scheduler.reserve(u'test@example.org', dates)
+        scheduler.reserve('test@example.org', dates)
     assert allocation.waitinglist_length == 0
 
     # until we delete the existing reservation
     scheduler.remove_reservation(token)
-    scheduler.reserve(u'test@example.org', dates)
+    scheduler.reserve('test@example.org', dates)
 
 
 def test_quota_waitinglist(scheduler):
     start = datetime(2012, 3, 4, 2, 0)
     end = datetime(2012, 3, 4, 3, 0)
     dates = (start, end)
 
     # in this example the waiting list will kick in only after
     # the quota has been filled
 
     allocation = scheduler.allocate(dates, quota=2, approve_manually=True)[0]
     assert allocation.waitinglist_length == 0
 
-    t1 = scheduler.reserve(u'test@example.org', dates)
-    t2 = scheduler.reserve(u'test@example.org', dates)
+    t1 = scheduler.reserve('test@example.org', dates)
+    t2 = scheduler.reserve('test@example.org', dates)
     scheduler.commit()
 
     assert allocation.waitinglist_length == 2
 
     scheduler.approve_reservations(t1)
     scheduler.approve_reservations(t2)
     scheduler.commit()
 
     assert allocation.waitinglist_length == 0
 
-    t3 = scheduler.reserve(u'test@example.org', dates)
-    t4 = scheduler.reserve(u'test@example.org', dates)
+    t3 = scheduler.reserve('test@example.org', dates)
+    t4 = scheduler.reserve('test@example.org', dates)
     scheduler.commit()
 
     assert allocation.waitinglist_length == 2
 
     with pytest.raises(errors.AlreadyReservedError):
         scheduler.approve_reservations(t3)
 
@@ -1093,15 +1093,15 @@
     # that we have to look at how to stop the user from reserving one year
     # with a single form.
 
     start = datetime(2011, 1, 1, 15, 0)
     end = start + timedelta(days=1)
 
     with pytest.raises(errors.ReservationTooLong):
-        scheduler.reserve(u'test@example.org', (start, end))
+        scheduler.reserve('test@example.org', (start, end))
 
 
 def test_allocation_overlap(scheduler):
 
     sc1 = scheduler
     sc2 = scheduler.clone()
     sc2.name = 'clone'
@@ -1114,14 +1114,23 @@
 
     sc2.allocate((start, end), raster=15)
     sc2.commit()
 
     with pytest.raises(errors.OverlappingAllocationError):
         sc1.allocate((start, end), raster=15)
 
+    # even with 10 dates being passed in we should get an
+    # OverlappingAllocationError
+    with pytest.raises(errors.OverlappingAllocationError):
+        sc1.allocate((
+            (start + timedelta(days=days), end + timedelta(days=days))
+            for days in range(0, 10)
+
+        ), raster=15)
+
     # there's another way this could happen, which is illegal usage
     # of scheduler.allocate - we stop this befor it hits the database
     sc3 = scheduler.clone()
     sc3.name = 'another_clone'
 
     dates = [
         (datetime(2013, 1, 1, 12, 0), datetime(2013, 1, 1, 13, 0)),
@@ -1170,15 +1179,15 @@
     partitions = allocation.availability_partitions()
     assert len(partitions) == 1
     assert partitions[0][0] == 100.0
     assert partitions[0][1] == False
 
     start, end = datetime(2011, 1, 1, 8, 30), datetime(2011, 1, 1, 9, 00)
 
-    token = scheduler.reserve(u'test@example.org', (start, end))
+    token = scheduler.reserve('test@example.org', (start, end))
     scheduler.approve_reservations(token)
     scheduler.commit()
 
     partitions = allocation.availability_partitions()
     assert len(partitions) == 3
     assert partitions[0][0] == 25.00
     assert partitions[0][1] == False
@@ -1209,21 +1218,21 @@
     assert slot[1] == allocation.end
 
     slot = list(allocation.free_slots())[0]
     assert slot[0] == allocation.start
     assert slot[1] == allocation.end
 
     token = scheduler.reserve(
-        u'info@example.org',
+        'info@example.org',
         (datetime(2011, 1, 1, 16, 0), datetime(2011, 1, 1, 18, 0))
     )
     scheduler.approve_reservations(token)
 
     with pytest.raises(errors.AlreadyReservedError):
-        scheduler.reserve(u'info@example.org', (
+        scheduler.reserve('info@example.org', (
             datetime(2011, 1, 1, 8, 0), datetime(2011, 1, 1, 9, 0)
         ))
 
 
 def test_allocation_by_ids(scheduler):
     dates = [
         (datetime(2015, 1, 1, 15, 0), datetime(2015, 1, 1, 16, 0)),
@@ -1283,23 +1292,23 @@
     scheduler.commit()
 
     # which should give us ten allocations (-1 as the master is not
     # counted)
     assert len(scheduler.allocation_mirrors_by_master(allocation)) == 9
 
     # the same reservation can now be made ten times
-    for i in range(0, 10):
+    for _ in range(0, 10):
         scheduler.approve_reservations(
-            scheduler.reserve(u'test@example.org', (start, end))
+            scheduler.reserve('test@example.org', (start, end))
         )
     scheduler.commit()
 
     # the 11th time it'll fail
     with pytest.raises(errors.AlreadyReservedError):
-        scheduler.reserve(u'test@example.org', [(start, end)])
+        scheduler.reserve('test@example.org', [(start, end)])
 
     other = scheduler.clone()
     other.name = 'other'
 
     # setup an allocation with five spots
     allocations = other.allocate(
         [(start, end)], raster=15, quota=5, partly_available=True,
@@ -1307,32 +1316,32 @@
     )
     allocation = allocations[0]
 
     assert len(other.allocation_mirrors_by_master(allocation)) == 4
 
     # we can do ten reservations if every reservation only occupies half
     # of the allocation
-    for i in range(0, 5):
+    for _ in range(0, 5):
         other.approve_reservations(
             other.reserve(
-                u'test@example.org',
+                'test@example.org',
                 (datetime(2011, 1, 1, 15, 0), datetime(2011, 1, 1, 15, 30))
             )
         )
         other.approve_reservations(
             other.reserve(
-                u'test@example.org',
+                'test@example.org',
                 (datetime(2011, 1, 1, 15, 30), datetime(2011, 1, 1, 16, 0))
             )
         )
 
     scheduler.commit()
 
     with pytest.raises(errors.AlreadyReservedError):
-        other.reserve(u'test@example.org', (
+        other.reserve('test@example.org', (
             (datetime(2011, 1, 1, 15, 30), datetime(2011, 1, 1, 16, 0))
         ))
 
     # test some queries
     allocations = scheduler.allocations_in_range(start, end)
     assert allocations.count() == 1
 
@@ -1353,28 +1362,28 @@
 
 def test_fragmentation(scheduler):
     start = datetime(2011, 1, 1, 15, 0)
     end = datetime(2011, 1, 1, 16, 0)
     daterange = (start, end)
 
     allocation = scheduler.allocate(daterange, quota=3)[0]
-    reservation = scheduler.reserve(u'test@example.org', daterange)
+    reservation = scheduler.reserve('test@example.org', daterange)
     slots = scheduler.approve_reservations(reservation)
 
     assert all(True for s in slots if s.resource == scheduler.resource)
 
     slots = scheduler.approve_reservations(
-        scheduler.reserve(u'test@example.org', daterange)
+        scheduler.reserve('test@example.org', daterange)
     )
     assert not any(False for s in slots if s.resource == scheduler.resource)
 
     scheduler.remove_reservation(reservation)
 
     slots = scheduler.approve_reservations(
-        scheduler.reserve(u'test@example.org', daterange)
+        scheduler.reserve('test@example.org', daterange)
     )
     assert all(True for s in slots if s.resource == scheduler.resource)
 
     with pytest.raises(errors.AffectedReservationError):
         scheduler.remove_allocation(allocation.id)
 
 
@@ -1392,43 +1401,43 @@
     assert len(allocation.siblings()) == 3
 
     masters = len([m for m in mirrors if m.is_master])
     assert masters == 0
     assert len([s for s in allocation.siblings(imaginary=False)]) == 1
 
     scheduler.approve_reservations(
-        scheduler.reserve(u'test@example.org', daterange)
+        scheduler.reserve('test@example.org', daterange)
     )
     mirrors = scheduler.allocation_mirrors_by_master(allocation)
     imaginary = len([m for m in mirrors if m.is_transient])
     assert imaginary == 2
 
     scheduler.approve_reservations(
-        scheduler.reserve(u'test@example.org', daterange)
+        scheduler.reserve('test@example.org', daterange)
     )
     mirrors = scheduler.allocation_mirrors_by_master(allocation)
     imaginary = len([m for m in mirrors if m.is_transient])
     assert imaginary == 1
 
     scheduler.approve_reservations(
-        scheduler.reserve(u'test@example.org', daterange)
+        scheduler.reserve('test@example.org', daterange)
     )
     mirrors = scheduler.allocation_mirrors_by_master(allocation)
     imaginary = len([m for m in mirrors if m.is_transient])
     assert imaginary == 0
     assert len(mirrors) + 1 == len(allocation.siblings())
 
 
 def test_allocations_by_reservation(scheduler):
     start = datetime(2013, 12, 3, 13, 0)
     end = datetime(2013, 12, 3, 15, 0)
     daterange = (start, end)
 
     allocations = scheduler.allocate(daterange, approve_manually=True)
-    token = scheduler.reserve(u'test@example.org', daterange)
+    token = scheduler.reserve('test@example.org', daterange)
     scheduler.commit()
 
     # pending reservations return empty
     assert scheduler.allocations_by_reservation(token).all() == []
 
     # on the reservation itself, the target can be found however
     reservation = scheduler.reservations_by_token(token).one()
@@ -1452,15 +1461,15 @@
 
     allocations = []
     for start, end in ranges:
         allocations.extend(
             scheduler.allocate((start, end), approve_manually=True)
         )
 
-    token = scheduler.reserve(u'test@example.org', ranges)
+    token = scheduler.reserve('test@example.org', ranges)
     scheduler.approve_reservations(token)
     scheduler.commit()
 
     # we now have multiple reservations pointing to multiple tokens
     # bound together in one reservation token
     assert len(scheduler.allocations_by_reservation(token).all()) == 2
 
@@ -1478,16 +1487,16 @@
     start = datetime(2011, 1, 1, 15, 0)
     end = datetime(2011, 1, 1, 16, 0)
     daterange = (start, end)
     master = scheduler.allocate(daterange, quota=5)[0]
     assert master.quota_left == 5
 
     reservations = []
-    for i in range(0, 5):
-        reservations.append(scheduler.reserve(u'test@example.org', daterange))
+    for _ in range(0, 5):
+        reservations.append(scheduler.reserve('test@example.org', daterange))
 
     for r in reservations:
         scheduler.approve_reservations(r)
 
     scheduler.commit()
 
     mirrors = scheduler.allocation_mirrors_by_master(master)
@@ -1540,51 +1549,54 @@
     start = datetime(2011, 1, 1, 15, 0)
     end = datetime(2011, 1, 1, 16, 0)
     daterange = (start, end)
 
     master = scheduler.allocate(daterange, quota=7)[0]
 
     scheduler.change_quota(master, 7)
-    scheduler.reserve(u'test@example.org', daterange)
-    r2 = scheduler.reserve(u'test@example.org', daterange)
-    r3 = scheduler.reserve(u'test@example.org', daterange)
-    r4 = scheduler.reserve(u'test@example.org', daterange)
-    r5 = scheduler.reserve(u'test@example.org', daterange)
-    r6 = scheduler.reserve(u'test@example.org', daterange)
-    r7 = scheduler.reserve(u'test@example.org', daterange)
+    r1 = scheduler.reserve('test@example.org', daterange)
+    r2 = scheduler.reserve('test@example.org', daterange)
+    r3 = scheduler.reserve('test@example.org', daterange)
+    r4 = scheduler.reserve('test@example.org', daterange)
+    r5 = scheduler.reserve('test@example.org', daterange)
+    r6 = scheduler.reserve('test@example.org', daterange)
+    r7 = scheduler.reserve('test@example.org', daterange)
 
-    for r in [r2, r3, r4, r5, r6, r7]:
+    for r in [r1, r2, r3, r4, r5, r6, r7]:
         scheduler.approve_reservations(r)
 
     scheduler.commit()
 
-    master.quota_left == 0
+    assert master.quota_left == 0
 
+    a1 = scheduler.allocations_by_reservation(r1).one().id
     a2 = scheduler.allocations_by_reservation(r2).one().id
     a3 = scheduler.allocations_by_reservation(r3).one().id
     a4 = scheduler.allocations_by_reservation(r4).one().id
     a5 = scheduler.allocations_by_reservation(r5).one().id
     a7 = scheduler.allocations_by_reservation(r7).one().id
 
     scheduler.remove_reservation(r3)
     scheduler.remove_reservation(r4)
     scheduler.remove_reservation(r6)
     scheduler.commit()
 
-    master.quota_left == 3
+    assert master.quota_left == 3
 
     scheduler.change_quota(master, 4)
     scheduler.commit()
 
-    master.quota_left == 0
+    assert master.quota_left == 0
 
+    a1_ = scheduler.allocations_by_reservation(r1).one().id
     a2_ = scheduler.allocations_by_reservation(r2).one().id
     a5_ = scheduler.allocations_by_reservation(r5).one().id
     a7_ = scheduler.allocations_by_reservation(r7).one().id
 
+    assert a1_ == a1
     assert a2_ == a2
 
     assert a5_ == a3
     assert a5_ != a5
 
     assert a7_ == a4
     assert a7_ != a7
@@ -1595,82 +1607,82 @@
     end = datetime(2011, 1, 1, 16, 0)
 
     a = scheduler.allocate(
         (start, end), raster=15, partly_available=True)[0]
 
     scheduler.approve_reservations(
         scheduler.reserve(
-            u'test@example.org',
+            'test@example.org',
             (datetime(2011, 1, 1, 15, 0), datetime(2011, 1, 1, 15, 15))
         )
     )
     scheduler.commit()
 
     assert a.availability == 75.0
     assert a.availability == scheduler.availability()
 
     scheduler.approve_reservations(
         scheduler.reserve(
-            u'test@example.org',
+            'test@example.org',
             (datetime(2011, 1, 1, 15, 45), datetime(2011, 1, 1, 16, 0))
         )
     )
     scheduler.commit()
 
     assert a.availability == 50.0
     assert a.availability == scheduler.availability()
 
     scheduler.approve_reservations(
         scheduler.reserve(
-            u'test@example.org',
+            'test@example.org',
             (datetime(2011, 1, 1, 15, 15), datetime(2011, 1, 1, 15, 30))
         )
     )
     scheduler.commit()
 
     assert a.availability == 25.0
     assert a.availability == scheduler.availability()
 
     scheduler.approve_reservations(
         scheduler.reserve(
-            u'test@example.org',
+            'test@example.org',
             (datetime(2011, 1, 1, 15, 30), datetime(2011, 1, 1, 15, 45))
         )
     )
     scheduler.commit()
 
     assert a.availability == 0.0
     assert a.availability == scheduler.availability()
 
     sc2 = scheduler.clone()
     sc2.name = 'clone'
 
     a = sc2.allocate((start, end), quota=4)[0]
     assert a.availability == 100.0  # master only!
 
-    sc2.approve_reservations(sc2.reserve(u'test@example.org', (start, end)))
+    sc2.approve_reservations(sc2.reserve('test@example.org', (start, end)))
     sc2.commit()
 
     assert sc2.availability() == 75.0
     assert a.availability == 0.0  # master only!
 
     sc2.approve_reservations(
-        sc2.reserve(u'test@example.org', (start, end))
+        sc2.reserve('test@example.org', (start, end))
     )
     sc2.commit()
     assert sc2.availability() == 50.0
 
     sc2.approve_reservations(
-        sc2.reserve(u'test@example.org', (start, end))
+        sc2.reserve('test@example.org', (start, end))
     )
     sc2.commit()
     assert sc2.availability() == 25.0
 
     sc2.approve_reservations(
-        sc2.reserve(u'test@example.org', (start, end))
+        sc2.reserve('test@example.org', (start, end))
     )
     sc2.commit()
     assert sc2.availability() == 0.0
 
     sc2.extinguish_managed_records()
     sc2.commit()
 
@@ -1709,15 +1721,15 @@
     scheduler.allocate(dates, approve_manually=True)
     assert allocations_added.called
     assert allocations_added.call_args[0][0].name == scheduler.context.name
     assert len(allocations_added.call_args[0][1]) == 1
 
     # create reservations
 
-    token = scheduler.reserve(u'test@example.org', dates)
+    token = scheduler.reserve('test@example.org', dates)
     assert reservations_made.called
     assert reservations_made.call_args[0][0].name == scheduler.context.name
     assert reservations_made.call_args[0][0].name == scheduler.context.name
     assert reservations_made.call_args[0][1][0].token == token
 
     reservations_made.reset_mock()
 
@@ -1734,15 +1746,15 @@
     reservations_denied.reset_mock()
 
     # remove the reservation and deny the next one
     scheduler.remove_reservation(token)
     assert reservations_removed.called
     assert reservations_removed.call_args[0][0].name == scheduler.context.name
 
-    token = scheduler.reserve(u'test@example.org', dates)
+    token = scheduler.reserve('test@example.org', dates)
     assert reservations_made.called
     assert reservations_made.call_args[0][0].name == scheduler.context.name
 
     scheduler.deny_reservation(token)
 
     assert not reservations_approved.called
     assert reservations_denied.call_args[0][0].name == scheduler.context.name
@@ -1763,15 +1775,15 @@
             datetime(2014, 1, 1, 14, 0),
             datetime(2014, 1, 1, 14, 0),
             datetime(2014, 1, 1, 14, 0),
             {
                 'str': [
                     datetime(2014, 1, 1, 14, 0),
                 ],
-                u'unicode': datetime(2014, 1, 1, 14, 0)
+                'unicode': datetime(2014, 1, 1, 14, 0)
             }
         ],
         'nothing': None
     }
     data['nested'] = list(map(copy, (data, data)))
 
     start = datetime(2014, 1, 30, 15, 0)
@@ -1816,15 +1828,15 @@
     start = datetime(2014, 3, 25, 14, 0)
     end = datetime(2014, 3, 25, 16, 0)
     dates = (start, end)
 
     session_id = new_uuid()
 
     scheduler.allocate(dates, approve_manually=False)
-    scheduler.reserve(u'test@example.org', dates, session_id=session_id)
+    scheduler.reserve('test@example.org', dates, session_id=session_id)
 
     # note the new session_id
     with pytest.raises(errors.NoReservationsToConfirm):
         scheduler.queries.confirm_reservations_for_session(
             session_id=new_uuid()
         )
 
@@ -1855,15 +1867,15 @@
     assert len(scheduler.search_allocations(*adjusted)) == 0
 
     # test days
     assert len(scheduler.search_allocations(*daterange, days=['su'])) == 1
     assert len(scheduler.search_allocations(*daterange, days=['mo'])) == 0
 
     # make sure the exposure is taken into account..
-    class MockExposure(object):
+    class MockExposure:
 
         def __init__(self, return_value):
             self.return_value = return_value
 
         def is_allocation_exposed(self, allocation):
             return self.return_value
 
@@ -1875,17 +1887,17 @@
     scheduler.clear_cache()
     assert len(scheduler.search_allocations(*daterange)) == 1
 
     # test available only
     assert len(scheduler.search_allocations(
         *daterange, available_only=True)) == 1
 
-    for i in range(0, 4):
+    for _ in range(0, 4):
         scheduler.approve_reservations(
-            scheduler.reserve(u'test@example.org', daterange)
+            scheduler.reserve('test@example.org', daterange)
         )
         scheduler.commit()
 
     assert len(scheduler.search_allocations(
         *daterange, available_only=True)) == 0
 
     # test minspots (takes quota_limit into account)
@@ -1951,15 +1963,15 @@
 def test_search_whole_day_regression(scheduler):
     # https://github.com/seantis/seantis.reservation/issues/162
     s, e = datetime(2014, 8, 18, 0, 0), datetime(2014, 8, 18, 0, 0)
 
     scheduler.allocate((s, e), whole_day=True, partly_available=True)
     scheduler.approve_reservations(
         scheduler.reserve(
-            u'test@example.org', (
+            'test@example.org', (
                 datetime(2014, 8, 18, 10, 0), datetime(2014, 8, 18, 11, 0)
             )
         )
     )
     scheduler.commit()
 
     # the error only manifests itself if the search is limited to a time
@@ -1975,16 +1987,16 @@
 
 def test_remove_reservation_from_session(scheduler):
     dates = (datetime(2014, 11, 26, 13, 0), datetime(2014, 11, 26, 14))
     scheduler.allocate(dates)
 
     sessions = [new_uuid(), new_uuid()]
     tokens = [
-        scheduler.reserve(u'test@example.com', dates, session_id=sessions[0]),
-        scheduler.reserve(u'test@example.com', dates, session_id=sessions[1])
+        scheduler.reserve('test@example.com', dates, session_id=sessions[0]),
+        scheduler.reserve('test@example.com', dates, session_id=sessions[1])
     ]
 
     scheduler.commit()
 
     assert scheduler.queries.reservations_by_session(sessions[0]).count() == 1
     assert scheduler.queries.reservations_by_session(sessions[1]).count() == 1
 
@@ -1996,15 +2008,15 @@
 
 
 def test_availability_by_day(scheduler):
     dates = (datetime(2014, 11, 26, 13, 0), datetime(2014, 11, 26, 14))
 
     allocation = scheduler.allocate(dates)[0]
     scheduler.approve_reservations(
-        scheduler.reserve(u'test@example.com', dates)
+        scheduler.reserve('test@example.com', dates)
     )
     scheduler.commit()
 
     sc2 = scheduler.clone()
     sc2.name = 'clone'
 
     sc2.allocate(dates)
@@ -2030,32 +2042,32 @@
 
 
 def test_remove_unused_allocations(scheduler):
 
     # create one allocation with a pending reservation
     daterange = (datetime(2013, 12, 3, 13, 0), datetime(2013, 12, 3, 15, 0))
     scheduler.allocate(daterange)
-    scheduler.reserve(u'test@example.org', daterange)
+    scheduler.reserve('test@example.org', daterange)
     scheduler.commit()
 
     # create one allocation with a finished reservation
     daterange = (datetime(2014, 12, 3, 13, 0), datetime(2014, 12, 3, 15, 0))
     scheduler.allocate(daterange)
     scheduler.approve_reservations(
-        scheduler.reserve(u'test@example.org', daterange)
+        scheduler.reserve('test@example.org', daterange)
     )
     scheduler.commit()
 
     # create a group of allocations with a pending reservation
     daterange = [
         (datetime(2015, 12, 3, 13, 0), datetime(2015, 12, 3, 15, 0)),
         (datetime(2015, 12, 4, 13, 0), datetime(2015, 12, 4, 15, 0))
     ]
     scheduler.allocate(daterange, grouped=True)
-    scheduler.reserve(u'test@example.org', daterange)
+    scheduler.reserve('test@example.org', daterange)
     scheduler.commit()
 
     # create one unused allocation
     daterange = (datetime(2016, 12, 3, 13, 0), datetime(2016, 12, 3, 15, 0))
     scheduler.allocate(daterange)
     scheduler.commit()
```

### Comparing `libres-0.6.1/libres/tests/test_session.py` & `libres-0.7.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/libres/tests/test_test.py` & `libres-0.7.0/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/libres/tests/test_utils.py` & `libres-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `libres-0.6.1/libres.egg-info/PKG-INFO` & `libres-0.7.0/src/libres.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: libres
-Version: 0.6.1
+Version: 0.7.0
 Summary: A library to reserve things
 Home-page: http://github.com/seantis/libres/
 Author: Denis Krienbühl
 Author-email: denis@href.ch
+Maintainer: Seantis GmbH
+Maintainer-email: info@seantis.ch
 License: BSD
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: mypy
 License-File: LICENSE
 
 Libres
 ======
 
 Libres is a reservations management library to reserve things like tables at
-a restaurant or tickets at an event. It works with Python 3.7+
+a restaurant or tickets at an event. It works with Python 3.8+
 and requires Postgresql 9.1+.
 
 `Documentation <http://libres.readthedocs.org/en/latest/>`_ | `Source <http://github.com/seantis/libres/>`_ | `Bugs <http://github.com/seantis/libres/issues>`_
 
 **This library is at an experimental stage and not yet suitable for production**
 
 .. image:: https://github.com/seantis/libres/actions/workflows/python-tox.yaml/badge.svg
@@ -36,17 +45,102 @@
   :target: https://codecov.io/gh/seantis/libres
   :alt:    Coverage
 
 .. image:: https://img.shields.io/pypi/v/libres.svg
   :target: https://pypi.python.org/pypi/libres
   :alt:    Release
 
+.. < package description
+
+Run the Example
+---------------
+
+Go to examples/flask and install the requirements::
+
+    cd examples/flask
+    pip install -r requirements.txt
+
+Run the example::
+
+    python run.py
+
+Open http://localhost:5000 and click around.
+
+Run the Tests
+-------------
+
+Install tox and run it::
+
+    pip install tox
+    tox
+
+Limit the tests to a specific python version::
+
+    tox -e py27
+
+Conventions
+-----------
+
+Libres follows PEP8 as close as possible. To test for it run::
+
+    tox -e pep8
+
+Libres uses `Semantic Versioning <http://semver.org/>`_
+
+Build the Docs
+--------------
+
+Go to docs and install the requirements::
+
+    cd docs
+    pip install -r requirements.txt
+
+Build the docs::
+
+    make html
+
+Open the docs::
+
+    open build/html/index.html
+
+Making a new Release
+--------------------
+
+Make sure all changes are in the HISTORY.rst, then bump the version::
+
+    bump2version major|minor|patch
+    git push && git push --tags
+
+After this, create a new release on Github.
+
 Changelog
 ---------
 
+0.7.0 (2023-07-11)
+~~~~~~~~~~~~~~~~~~~
+
+- Drops support for Python 3.7 and adds support for 3.11
+  [Daverball]
+
+- Switches to ``pyproject.toml``
+  [Daverball]
+
+- Adds type annotations
+  [Daverball]
+
+- Changes ``Scheduler.allocate`` to avoid hundreds of separate
+  SQL queries when passing in hundreds of datetime ranges in
+  order to identify existing overlapping allocations.
+
+  Performance could still be a concern, since the query contains
+  a lot of datetime comparisons. It might be quicker in the common case to filter to the minimum and maximum dates that
+  have been passed in and doing the overlap checks entirely in
+  Python. We will need to keep an eye on this.
+  [Daverball]
+
 0.6.1 (2023-03-29)
 ~~~~~~~~~~~~~~~~~~~
 
 - Adds additional parameters to ``Scheduler.remove_unused allocations``
   to filter the to be removed Allocations by weekday or
   whether or not they belong to a group.
   [Daverball]
```

### Comparing `libres-0.6.1/libres.egg-info/SOURCES.txt` & `libres-0.7.0/src/libres.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
-setup.py
+pyproject.toml
+setup.cfg
 docs/Makefile
 docs/api.rst
 docs/concepts.rst
 docs/conf.py
 docs/customizations.rst
 docs/faq.rst
 docs/index.rst
 docs/requirements.txt
 docs/under_the_hood.rst
 docs/_static/custom.css
 docs/_static/favicon.ico
 docs/_static/logo.svg
-libres/.gitignore
-libres/__init__.py
-libres.egg-info/PKG-INFO
-libres.egg-info/SOURCES.txt
-libres.egg-info/dependency_links.txt
-libres.egg-info/not-zip-safe
-libres.egg-info/requires.txt
-libres.egg-info/top_level.txt
-libres/context/__init__.py
-libres/context/core.py
-libres/context/exposure.py
-libres/context/registry.py
-libres/context/session.py
-libres/context/settings.py
-libres/db/__init__.py
-libres/db/queries.py
-libres/db/scheduler.py
-libres/db/models/__init__.py
-libres/db/models/allocation.py
-libres/db/models/base.py
-libres/db/models/other.py
-libres/db/models/reservation.py
-libres/db/models/reserved_slot.py
-libres/db/models/timestamp.py
-libres/db/models/types/__init__.py
-libres/db/models/types/json_type.py
-libres/db/models/types/utcdatetime.py
-libres/db/models/types/uuid_type.py
-libres/modules/__init__.py
-libres/modules/compat.py
-libres/modules/errors.py
-libres/modules/events.py
-libres/modules/rasterizer.py
-libres/modules/utils.py
-libres/tests/__init__.py
-libres/tests/conftest.py
-libres/tests/test_allocation.py
-libres/tests/test_registry.py
-libres/tests/test_reservation.py
-libres/tests/test_reserved_slot.py
-libres/tests/test_scheduler.py
-libres/tests/test_session.py
-libres/tests/test_test.py
-libres/tests/test_types.py
-libres/tests/test_utils.py
+src/libres/.gitignore
+src/libres/__init__.py
+src/libres/py.typed
+src/libres.egg-info/PKG-INFO
+src/libres.egg-info/SOURCES.txt
+src/libres.egg-info/dependency_links.txt
+src/libres.egg-info/not-zip-safe
+src/libres.egg-info/requires.txt
+src/libres.egg-info/top_level.txt
+src/libres/context/__init__.py
+src/libres/context/core.py
+src/libres/context/exposure.py
+src/libres/context/registry.py
+src/libres/context/session.py
+src/libres/context/settings.py
+src/libres/db/__init__.py
+src/libres/db/queries.py
+src/libres/db/scheduler.py
+src/libres/db/models/__init__.py
+src/libres/db/models/allocation.py
+src/libres/db/models/base.py
+src/libres/db/models/other.py
+src/libres/db/models/reservation.py
+src/libres/db/models/reserved_slot.py
+src/libres/db/models/timestamp.py
+src/libres/db/models/types/__init__.py
+src/libres/db/models/types/json_type.py
+src/libres/db/models/types/utcdatetime.py
+src/libres/db/models/types/uuid_type.py
+src/libres/modules/__init__.py
+src/libres/modules/errors.py
+src/libres/modules/events.py
+src/libres/modules/rasterizer.py
+src/libres/modules/utils.py
+tests/test_allocation.py
+tests/test_registry.py
+tests/test_reservation.py
+tests/test_reserved_slot.py
+tests/test_scheduler.py
+tests/test_session.py
+tests/test_test.py
+tests/test_types.py
+tests/test_utils.py
```

