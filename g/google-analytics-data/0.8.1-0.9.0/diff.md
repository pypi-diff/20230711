# Comparing `tmp/google-analytics-data-0.8.1.tar.gz` & `tmp/google-analytics-data-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/google-analytics-data-0.8.1.tar", last modified: Mon Sep 27 16:02:19 2021, max compression
+gzip compressed data, was "google-analytics-data-0.9.0.tar", last modified: Mon Oct 11 16:52:38 2021, max compression
```

## Comparing `google-analytics-data-0.8.1.tar` & `google-analytics-data-0.9.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.491820 google-analytics-data-0.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     3593 2021-09-27 16:02:19.491820 google-analytics-data-0.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2895 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.479814 google-analytics-data-0.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.479814 google-analytics-data-0.8.1/google/analytics/
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.483816 google-analytics-data-0.8.1/google/analytics/data/
--rw-rw-r--   0 root         (0)     1003     5396 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data/__init__.py
--rw-rw-r--   0 root         (0)     1003       82 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.483816 google-analytics-data-0.8.1/google/analytics/data_v1alpha/
--rw-rw-r--   0 root         (0)     1003     3544 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003     2075 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       82 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.483816 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.483816 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/
--rw-rw-r--   0 root         (0)     1003      785 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/__init__.py
--rw-rw-r--   0 root         (0)     1003    21184 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/async_client.py
--rw-rw-r--   0 root         (0)     1003    30082 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.483816 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/
--rw-rw-r--   0 root         (0)     1003     1238 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9327 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19046 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19474 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.483816 google-analytics-data-0.8.1/google/analytics/data_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     2443 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    25506 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/types/analytics_data_api.py
--rw-rw-r--   0 root         (0)     1003    38831 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1alpha/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.487818 google-analytics-data-0.8.1/google/analytics/data_v1beta/
--rw-rw-r--   0 root         (0)     1003     3951 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     2334 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       82 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.487818 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.487818 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/
--rw-rw-r--   0 root         (0)     1003      781 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/__init__.py
--rw-rw-r--   0 root         (0)     1003    24902 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/async_client.py
--rw-rw-r--   0 root         (0)     1003    34050 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.487818 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/transports/
--rw-rw-r--   0 root         (0)     1003     1221 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9825 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20854 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21303 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.487818 google-analytics-data-0.8.1/google/analytics/data_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     2733 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    33556 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/types/analytics_data_api.py
--rw-rw-r--   0 root         (0)     1003    43811 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/google/analytics/data_v1beta/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.487818 google-analytics-data-0.8.1/google_analytics_data.egg-info/
--rw-r--r--   0 root         (0)     1003     3593 2021-09-27 16:02:19.000000 google-analytics-data-0.8.1/google_analytics_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2440 2021-09-27 16:02:19.000000 google-analytics-data-0.8.1/google_analytics_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2021-09-27 16:02:19.000000 google-analytics-data-0.8.1/google_analytics_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       24 2021-09-27 16:02:19.000000 google-analytics-data-0.8.1/google_analytics_data.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2021-09-27 16:02:19.000000 google-analytics-data-0.8.1/google_analytics_data.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003       88 2021-09-27 16:02:19.000000 google-analytics-data-0.8.1/google_analytics_data.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2021-09-27 16:02:19.000000 google-analytics-data-0.8.1/google_analytics_data.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2021-09-27 16:02:19.491820 google-analytics-data-0.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2235 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.487818 google-analytics-data-0.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.487818 google-analytics-data-0.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.487818 google-analytics-data-0.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.491820 google-analytics-data-0.8.1/tests/unit/gapic/data_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/tests/unit/gapic/data_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003    68446 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/tests/unit/gapic/data_v1alpha/test_alpha_analytics_data.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-27 16:02:19.491820 google-analytics-data-0.8.1/tests/unit/gapic/data_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/tests/unit/gapic/data_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    82790 2021-09-27 15:59:36.000000 google-analytics-data-0.8.1/tests/unit/gapic/data_v1beta/test_beta_analytics_data.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     3694 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2895 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.944594 google-analytics-data-0.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.944594 google-analytics-data-0.9.0/google/analytics/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.944594 google-analytics-data-0.9.0/google/analytics/data/
+-rw-rw-r--   0 root         (0)     1003     5396 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data/__init__.py
+-rw-rw-r--   0 root         (0)     1003       82 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.944594 google-analytics-data-0.9.0/google/analytics/data_v1alpha/
+-rw-rw-r--   0 root         (0)     1003     3544 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2075 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       82 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.948592 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.948592 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/
+-rw-rw-r--   0 root         (0)     1003      785 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21184 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/async_client.py
+-rw-rw-r--   0 root         (0)     1003    30082 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.948592 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/
+-rw-rw-r--   0 root         (0)     1003     1238 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9327 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19046 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19474 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.948592 google-analytics-data-0.9.0/google/analytics/data_v1alpha/types/
+-rw-rw-r--   0 root         (0)     1003     2443 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25506 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/types/analytics_data_api.py
+-rw-rw-r--   0 root         (0)     1003    38831 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1alpha/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.948592 google-analytics-data-0.9.0/google/analytics/data_v1beta/
+-rw-rw-r--   0 root         (0)     1003     3951 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2334 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       82 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.948592 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.948592 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/
+-rw-rw-r--   0 root         (0)     1003      781 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25043 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/async_client.py
+-rw-rw-r--   0 root         (0)     1003    34298 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/transports/
+-rw-rw-r--   0 root         (0)     1003     1221 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10113 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20910 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21366 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/google/analytics/data_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     2733 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    33565 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/types/analytics_data_api.py
+-rw-rw-r--   0 root         (0)     1003    43833 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/google/analytics/data_v1beta/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/google_analytics_data.egg-info/
+-rw-r--r--   0 root         (0)     1003     3694 2021-10-11 16:52:38.000000 google-analytics-data-0.9.0/google_analytics_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2440 2021-10-11 16:52:38.000000 google-analytics-data-0.9.0/google_analytics_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-10-11 16:52:38.000000 google-analytics-data-0.9.0/google_analytics_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       24 2021-10-11 16:52:38.000000 google-analytics-data-0.9.0/google_analytics_data.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-10-11 16:52:38.000000 google-analytics-data-0.9.0/google_analytics_data.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003       88 2021-10-11 16:52:38.000000 google-analytics-data-0.9.0/google_analytics_data.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2021-10-11 16:52:38.000000 google-analytics-data-0.9.0/google_analytics_data.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2334 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/tests/unit/gapic/data_v1alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/tests/unit/gapic/data_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003    68446 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/tests/unit/gapic/data_v1alpha/test_alpha_analytics_data.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-11 16:52:38.952590 google-analytics-data-0.9.0/tests/unit/gapic/data_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/tests/unit/gapic/data_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    84286 2021-10-11 16:50:04.000000 google-analytics-data-0.9.0/tests/unit/gapic/data_v1beta/test_beta_analytics_data.py
```

### Comparing `google-analytics-data-0.8.1/LICENSE` & `google-analytics-data-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/MANIFEST.in` & `google-analytics-data-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/PKG-INFO` & `google-analytics-data-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: google-analytics-data
-Version: 0.8.1
+Version: 0.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/googleapis/python-analytics-data
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: LICENSE
 
 Python Client for Analytics Data
 =================================================
```

### Comparing `google-analytics-data-0.8.1/README.rst` & `google-analytics-data-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/gapic_metadata.json` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/async_client.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/async_client.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/client.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/client.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/base.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/grpc.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/grpc_asyncio.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/services/alpha_analytics_data/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/types/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/types/analytics_data_api.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/types/analytics_data_api.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1alpha/types/data.py` & `google-analytics-data-0.9.0/google/analytics/data_v1alpha/types/data.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/gapic_metadata.json` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/services/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/async_client.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,14 +574,20 @@
 
         # Send the request.
         response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        await self.transport.close()
+
 
 try:
     DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
         gapic_version=pkg_resources.get_distribution("google-analytics-data",).version,
     )
 except pkg_resources.DistributionNotFound:
     DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
```

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/client.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,18 +337,15 @@
                 credentials=credentials,
                 credentials_file=client_options.credentials_file,
                 host=api_endpoint,
                 scopes=client_options.scopes,
                 client_cert_source_for_mtls=client_cert_source_func,
                 quota_project_id=client_options.quota_project_id,
                 client_info=client_info,
-                always_use_jwt_access=(
-                    Transport == type(self).get_transport_class("grpc")
-                    or Transport == type(self).get_transport_class("grpc_asyncio")
-                ),
+                always_use_jwt_access=True,
             )
 
     def run_report(
         self,
         request: Union[analytics_data_api.RunReportRequest, dict] = None,
         *,
         retry: retries.Retry = gapic_v1.method.DEFAULT,
@@ -766,14 +763,27 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, type, value, traceback):
+        """Releases underlying transport's resources.
+
+        .. warning::
+            ONLY use as a context manager if the transport is NOT shared
+            with other clients! Exiting the with block will CLOSE the transport
+            and may cause errors in other clients!
+        """
+        self.transport.close()
+
 
 try:
     DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
         gapic_version=pkg_resources.get_distribution("google-analytics-data",).version,
     )
 except pkg_resources.DistributionNotFound:
     DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
```

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/transports/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/transports/base.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/transports/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,14 +176,23 @@
                 self.run_realtime_report, default_timeout=60.0, client_info=client_info,
             ),
             self.check_compatibility: gapic_v1.method.wrap_method(
                 self.check_compatibility, default_timeout=None, client_info=client_info,
             ),
         }
 
+    def close(self):
+        """Closes resources associated with the transport.
+
+       .. warning::
+            Only call this method if the transport is NOT shared
+            with other clients - this may cause errors in other clients!
+        """
+        raise NotImplementedError()
+
     @property
     def run_report(
         self,
     ) -> Callable[
         [analytics_data_api.RunReportRequest],
         Union[
             analytics_data_api.RunReportResponse,
```

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/transports/grpc.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,9 +458,12 @@
             self._stubs["check_compatibility"] = self.grpc_channel.unary_unary(
                 "/google.analytics.data.v1beta.BetaAnalyticsData/CheckCompatibility",
                 request_serializer=analytics_data_api.CheckCompatibilityRequest.serialize,
                 response_deserializer=analytics_data_api.CheckCompatibilityResponse.deserialize,
             )
         return self._stubs["check_compatibility"]
 
+    def close(self):
+        self.grpc_channel.close()
+
 
 __all__ = ("BetaAnalyticsDataGrpcTransport",)
```

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/services/beta_analytics_data/transports/grpc_asyncio.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/services/beta_analytics_data/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,9 +464,12 @@
             self._stubs["check_compatibility"] = self.grpc_channel.unary_unary(
                 "/google.analytics.data.v1beta.BetaAnalyticsData/CheckCompatibility",
                 request_serializer=analytics_data_api.CheckCompatibilityRequest.serialize,
                 response_deserializer=analytics_data_api.CheckCompatibilityResponse.deserialize,
             )
         return self._stubs["check_compatibility"]
 
+    def close(self):
+        return self.grpc_channel.close()
+
 
 __all__ = ("BetaAnalyticsDataGrpcAsyncIOTransport",)
```

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/types/__init__.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/types/analytics_data_api.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/types/analytics_data_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
         proto.MESSAGE, number=1, message=data.DimensionMetadata,
     )
     metrics = proto.RepeatedField(proto.MESSAGE, number=2, message=data.MetricMetadata,)
 
 
 class RunReportRequest(proto.Message):
     r"""The request to generate a report.
+
     Attributes:
         property (str):
             A Google Analytics GA4 property identifier whose events are
             tracked. Specified in the URL path and not the body. To
             learn more, see `where to find your Property
             ID <https://developers.google.com/analytics/devguides/reporting/data/v1/property-id>`__.
             Within a batch request, this property should either be
@@ -231,14 +232,15 @@
     cohort_spec = proto.Field(proto.MESSAGE, number=12, message=data.CohortSpec,)
     keep_empty_rows = proto.Field(proto.BOOL, number=13,)
     return_property_quota = proto.Field(proto.BOOL, number=14,)
 
 
 class RunReportResponse(proto.Message):
     r"""The response report table corresponding to a request.
+
     Attributes:
         dimension_headers (Sequence[google.analytics.data_v1beta.types.DimensionHeader]):
             Describes dimension columns. The number of
             DimensionHeaders and ordering of
             DimensionHeaders matches the dimensions present
             in rows.
         metric_headers (Sequence[google.analytics.data_v1beta.types.MetricHeader]):
@@ -291,14 +293,15 @@
     metadata = proto.Field(proto.MESSAGE, number=8, message=data.ResponseMetaData,)
     property_quota = proto.Field(proto.MESSAGE, number=9, message=data.PropertyQuota,)
     kind = proto.Field(proto.STRING, number=10,)
 
 
 class RunPivotReportRequest(proto.Message):
     r"""The request to generate a pivot report.
+
     Attributes:
         property (str):
             A Google Analytics GA4 property identifier whose events are
             tracked. Specified in the URL path and not the body. To
             learn more, see `where to find your Property
             ID <https://developers.google.com/analytics/devguides/reporting/data/v1/property-id>`__.
             Within a batch request, this property should either be
@@ -463,14 +466,15 @@
     metadata = proto.Field(proto.MESSAGE, number=6, message=data.ResponseMetaData,)
     property_quota = proto.Field(proto.MESSAGE, number=7, message=data.PropertyQuota,)
     kind = proto.Field(proto.STRING, number=8,)
 
 
 class BatchRunReportsRequest(proto.Message):
     r"""The batch request containing multiple report requests.
+
     Attributes:
         property (str):
             A Google Analytics GA4 property identifier whose events are
             tracked. Specified in the URL path and not the body. To
             learn more, see `where to find your Property
             ID <https://developers.google.com/analytics/devguides/reporting/data/v1/property-id>`__.
             This property must be specified for the batch. The property
@@ -486,14 +490,15 @@
 
     property = proto.Field(proto.STRING, number=1,)
     requests = proto.RepeatedField(proto.MESSAGE, number=2, message="RunReportRequest",)
 
 
 class BatchRunReportsResponse(proto.Message):
     r"""The batch response containing multiple reports.
+
     Attributes:
         reports (Sequence[google.analytics.data_v1beta.types.RunReportResponse]):
             Individual responses. Each response has a
             separate report request.
         kind (str):
             Identifies what kind of resource this message is. This
             ``kind`` is always the fixed string
@@ -503,14 +508,15 @@
 
     reports = proto.RepeatedField(proto.MESSAGE, number=1, message="RunReportResponse",)
     kind = proto.Field(proto.STRING, number=2,)
 
 
 class BatchRunPivotReportsRequest(proto.Message):
     r"""The batch request containing multiple pivot report requests.
+
     Attributes:
         property (str):
             A Google Analytics GA4 property identifier whose events are
             tracked. Specified in the URL path and not the body. To
             learn more, see `where to find your Property
             ID <https://developers.google.com/analytics/devguides/reporting/data/v1/property-id>`__.
             This property must be specified for the batch. The property
@@ -528,14 +534,15 @@
     requests = proto.RepeatedField(
         proto.MESSAGE, number=2, message="RunPivotReportRequest",
     )
 
 
 class BatchRunPivotReportsResponse(proto.Message):
     r"""The batch response containing multiple pivot reports.
+
     Attributes:
         pivot_reports (Sequence[google.analytics.data_v1beta.types.RunPivotReportResponse]):
             Individual responses. Each response has a
             separate pivot report request.
         kind (str):
             Identifies what kind of resource this message is. This
             ``kind`` is always the fixed string
@@ -547,14 +554,15 @@
         proto.MESSAGE, number=1, message="RunPivotReportResponse",
     )
     kind = proto.Field(proto.STRING, number=2,)
 
 
 class GetMetadataRequest(proto.Message):
     r"""Request for a property's dimension and metric metadata.
+
     Attributes:
         name (str):
             Required. The resource name of the metadata to retrieve.
             This name field is specified in the URL path and not URL
             parameters. Property is a numeric Google Analytics GA4
             Property identifier. To learn more, see `where to find your
             Property
@@ -568,14 +576,15 @@
     """
 
     name = proto.Field(proto.STRING, number=1,)
 
 
 class RunRealtimeReportRequest(proto.Message):
     r"""The request to generate a realtime report.
+
     Attributes:
         property (str):
             A Google Analytics GA4 property identifier whose events are
             tracked. Specified in the URL path and not the body. To
             learn more, see `where to find your Property
             ID <https://developers.google.com/analytics/devguides/reporting/data/v1/property-id>`__.
```

### Comparing `google-analytics-data-0.8.1/google/analytics/data_v1beta/types/data.py` & `google-analytics-data-0.9.0/google/analytics/data_v1beta/types/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,24 +214,26 @@
             Used to combine dimension values to a single
             dimension. For example, dimension "country,
             city": concatenate(country, ", ", city).
     """
 
     class CaseExpression(proto.Message):
         r"""Used to convert a dimension value to a single case.
+
         Attributes:
             dimension_name (str):
                 Name of a dimension. The name must refer back
                 to a name in dimensions field of the request.
         """
 
         dimension_name = proto.Field(proto.STRING, number=1,)
 
     class ConcatenateExpression(proto.Message):
         r"""Used to combine dimension values to a single dimension.
+
         Attributes:
             dimension_names (Sequence[str]):
                 Names of dimensions. The names must refer
                 back to names in the dimensions field of the
                 request.
             delimiter (str):
                 The delimiter placed between dimension names.
@@ -322,26 +324,28 @@
         proto.MESSAGE, number=3, oneof="expr", message="FilterExpression",
     )
     filter = proto.Field(proto.MESSAGE, number=4, oneof="expr", message="Filter",)
 
 
 class FilterExpressionList(proto.Message):
     r"""A list of filter expressions.
+
     Attributes:
         expressions (Sequence[google.analytics.data_v1beta.types.FilterExpression]):
             A list of filter expressions.
     """
 
     expressions = proto.RepeatedField(
         proto.MESSAGE, number=1, message="FilterExpression",
     )
 
 
 class Filter(proto.Message):
     r"""An expression to filter dimension or metric values.
+
     Attributes:
         field_name (str):
             The dimension name or metric name. Must be a
             name defined in dimensions or metrics.
         string_filter (google.analytics.data_v1beta.types.Filter.StringFilter):
             Strings related filter.
         in_list_filter (google.analytics.data_v1beta.types.Filter.InListFilter):
@@ -350,14 +354,15 @@
             A filter for numeric or date values.
         between_filter (google.analytics.data_v1beta.types.Filter.BetweenFilter):
             A filter for two values.
     """
 
     class StringFilter(proto.Message):
         r"""The filter for string
+
         Attributes:
             match_type (google.analytics.data_v1beta.types.Filter.StringFilter.MatchType):
                 The match type for this filter.
             value (str):
                 The string value used for the matching.
             case_sensitive (bool):
                 If true, the string value is case sensitive.
@@ -377,27 +382,29 @@
             proto.ENUM, number=1, enum="Filter.StringFilter.MatchType",
         )
         value = proto.Field(proto.STRING, number=2,)
         case_sensitive = proto.Field(proto.BOOL, number=3,)
 
     class InListFilter(proto.Message):
         r"""The result needs to be in a list of string values.
+
         Attributes:
             values (Sequence[str]):
                 The list of string values.
                 Must be non-empty.
             case_sensitive (bool):
                 If true, the string value is case sensitive.
         """
 
         values = proto.RepeatedField(proto.STRING, number=1,)
         case_sensitive = proto.Field(proto.BOOL, number=2,)
 
     class NumericFilter(proto.Message):
         r"""Filters for numeric or date values.
+
         Attributes:
             operation (google.analytics.data_v1beta.types.Filter.NumericFilter.Operation):
                 The operation type for this filter.
             value (google.analytics.data_v1beta.types.NumericValue):
                 A numeric value or a date value.
         """
 
@@ -442,37 +449,40 @@
     between_filter = proto.Field(
         proto.MESSAGE, number=6, oneof="one_filter", message=BetweenFilter,
     )
 
 
 class OrderBy(proto.Message):
     r"""The sort options.
+
     Attributes:
         metric (google.analytics.data_v1beta.types.OrderBy.MetricOrderBy):
             Sorts results by a metric's values.
         dimension (google.analytics.data_v1beta.types.OrderBy.DimensionOrderBy):
             Sorts results by a dimension's values.
         pivot (google.analytics.data_v1beta.types.OrderBy.PivotOrderBy):
             Sorts results by a metric's values within a
             pivot column group.
         desc (bool):
             If true, sorts by descending order.
     """
 
     class MetricOrderBy(proto.Message):
         r"""Sorts by metric values.
+
         Attributes:
             metric_name (str):
                 A metric name in the request to order by.
         """
 
         metric_name = proto.Field(proto.STRING, number=1,)
 
     class DimensionOrderBy(proto.Message):
         r"""Sorts by dimension values.
+
         Attributes:
             dimension_name (str):
                 A dimension name in the request to order by.
             order_type (google.analytics.data_v1beta.types.OrderBy.DimensionOrderBy.OrderType):
                 Controls the rule for dimension value
                 ordering.
         """
@@ -487,14 +497,15 @@
         dimension_name = proto.Field(proto.STRING, number=1,)
         order_type = proto.Field(
             proto.ENUM, number=2, enum="OrderBy.DimensionOrderBy.OrderType",
         )
 
     class PivotOrderBy(proto.Message):
         r"""Sorts by a pivot column group.
+
         Attributes:
             metric_name (str):
                 In the response to order by, order rows by
                 this column. Must be a metric name from the
                 request.
             pivot_selections (Sequence[google.analytics.data_v1beta.types.OrderBy.PivotOrderBy.PivotSelection]):
                 Used to select a dimension name and value
@@ -743,14 +754,15 @@
     granularity = proto.Field(proto.ENUM, number=1, enum=Granularity,)
     start_offset = proto.Field(proto.INT32, number=2,)
     end_offset = proto.Field(proto.INT32, number=3,)
 
 
 class CohortReportSettings(proto.Message):
     r"""Optional settings of a cohort report.
+
     Attributes:
         accumulate (bool):
             If true, accumulates the result from first touch day to the
             end day. Not supported in ``RunReportRequest``.
     """
 
     accumulate = proto.Field(proto.BOOL, number=1,)
@@ -801,14 +813,15 @@
 
     name = proto.Field(proto.STRING, number=1,)
     type_ = proto.Field(proto.ENUM, number=2, enum="MetricType",)
 
 
 class PivotHeader(proto.Message):
     r"""Dimensions' values in a single pivot.
+
     Attributes:
         pivot_dimension_headers (Sequence[google.analytics.data_v1beta.types.PivotDimensionHeader]):
             The size is the same as the cardinality of
             the corresponding dimension combinations.
         row_count (int):
             The cardinality of the pivot. The total number of rows for
             this pivot's fields regardless of how the parameters
@@ -819,14 +832,15 @@
         proto.MESSAGE, number=1, message="PivotDimensionHeader",
     )
     row_count = proto.Field(proto.INT32, number=2,)
 
 
 class PivotDimensionHeader(proto.Message):
     r"""Summarizes dimension values from a row for this pivot.
+
     Attributes:
         dimension_values (Sequence[google.analytics.data_v1beta.types.DimensionValue]):
             Values of multiple dimensions in a pivot.
     """
 
     dimension_values = proto.RepeatedField(
         proto.MESSAGE, number=1, message="DimensionValue",
@@ -884,35 +898,38 @@
         proto.MESSAGE, number=1, message="DimensionValue",
     )
     metric_values = proto.RepeatedField(proto.MESSAGE, number=2, message="MetricValue",)
 
 
 class DimensionValue(proto.Message):
     r"""The value of a dimension.
+
     Attributes:
         value (str):
             Value as a string if the dimension type is a
             string.
     """
 
     value = proto.Field(proto.STRING, number=1, oneof="one_value",)
 
 
 class MetricValue(proto.Message):
     r"""The value of a metric.
+
     Attributes:
         value (str):
             Measurement value. See MetricHeader for type.
     """
 
     value = proto.Field(proto.STRING, number=4, oneof="one_value",)
 
 
 class NumericValue(proto.Message):
     r"""To represent a number.
+
     Attributes:
         int64_value (int):
             Integer value
         double_value (float):
             Double value
     """
 
@@ -966,27 +983,29 @@
     potentially_thresholded_requests_per_hour = proto.Field(
         proto.MESSAGE, number=5, message="QuotaStatus",
     )
 
 
 class QuotaStatus(proto.Message):
     r"""Current state for a particular quota group.
+
     Attributes:
         consumed (int):
             Quota consumed by this request.
         remaining (int):
             Quota remaining after this request.
     """
 
     consumed = proto.Field(proto.INT32, number=1,)
     remaining = proto.Field(proto.INT32, number=2,)
 
 
 class DimensionMetadata(proto.Message):
     r"""Explains a dimension.
+
     Attributes:
         api_name (str):
             This dimension's name. Useable in
             `Dimension <#Dimension>`__'s ``name``. For example,
             ``eventName``.
         ui_name (str):
             This dimension's name within the Google Analytics user
@@ -1015,14 +1034,15 @@
     deprecated_api_names = proto.RepeatedField(proto.STRING, number=4,)
     custom_definition = proto.Field(proto.BOOL, number=5,)
     category = proto.Field(proto.STRING, number=7,)
 
 
 class MetricMetadata(proto.Message):
     r"""Explains a metric.
+
     Attributes:
         api_name (str):
             A metric name. Useable in `Metric <#Metric>`__'s ``name``.
             For example, ``eventCount``.
         ui_name (str):
             This metric's name within the Google Analytics user
             interface. For example, ``Event count``.
@@ -1059,14 +1079,15 @@
     expression = proto.Field(proto.STRING, number=6,)
     custom_definition = proto.Field(proto.BOOL, number=7,)
     category = proto.Field(proto.STRING, number=10,)
 
 
 class DimensionCompatibility(proto.Message):
     r"""The compatibility for a single dimension.
+
     Attributes:
         dimension_metadata (google.analytics.data_v1beta.types.DimensionMetadata):
             The dimension metadata contains the API name
             for this compatibility information. The
             dimension metadata also contains other helpful
             information like the UI name and description.
         compatibility (google.analytics.data_v1beta.types.Compatibility):
@@ -1081,14 +1102,15 @@
     compatibility = proto.Field(
         proto.ENUM, number=2, optional=True, enum="Compatibility",
     )
 
 
 class MetricCompatibility(proto.Message):
     r"""The compatibility for a single metric.
+
     Attributes:
         metric_metadata (google.analytics.data_v1beta.types.MetricMetadata):
             The metric metadata contains the API name for
             this compatibility information. The metric
             metadata also contains other helpful information
             like the UI name and description.
         compatibility (google.analytics.data_v1beta.types.Compatibility):
```

### Comparing `google-analytics-data-0.8.1/google_analytics_data.egg-info/PKG-INFO` & `google-analytics-data-0.9.0/google_analytics_data.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: google-analytics-data
-Version: 0.8.1
+Version: 0.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/googleapis/python-analytics-data
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: LICENSE
 
 Python Client for Analytics Data
 =================================================
```

### Comparing `google-analytics-data-0.8.1/google_analytics_data.egg-info/SOURCES.txt` & `google-analytics-data-0.9.0/google_analytics_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/setup.py` & `google-analytics-data-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 #
 
 import io
 import os
 import setuptools  # type: ignore
 
-version = "0.8.1"
+version = "0.9.0"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
@@ -57,12 +57,14 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Internet",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     zip_safe=False,
 )
```

### Comparing `google-analytics-data-0.8.1/tests/__init__.py` & `google-analytics-data-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/tests/unit/__init__.py` & `google-analytics-data-0.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/tests/unit/gapic/__init__.py` & `google-analytics-data-0.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/tests/unit/gapic/data_v1alpha/__init__.py` & `google-analytics-data-0.9.0/tests/unit/gapic/data_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/tests/unit/gapic/data_v1alpha/test_alpha_analytics_data.py` & `google-analytics-data-0.9.0/tests/unit/gapic/data_v1alpha/test_alpha_analytics_data.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/tests/unit/gapic/data_v1beta/__init__.py` & `google-analytics-data-0.9.0/tests/unit/gapic/data_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-data-0.8.1/tests/unit/gapic/data_v1beta/test_beta_analytics_data.py` & `google-analytics-data-0.9.0/tests/unit/gapic/data_v1beta/test_beta_analytics_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from google.analytics.data_v1beta.types import analytics_data_api
 from google.analytics.data_v1beta.types import data
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import grpc_helpers
 from google.api_core import grpc_helpers_async
+from google.api_core import path_template
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.oauth2 import service_account
 import google.auth
 
 
 # TODO(busunkim): Once google-auth >= 1.25.0 is required transitively
@@ -1679,14 +1680,17 @@
         "run_realtime_report",
         "check_compatibility",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
+    with pytest.raises(NotImplementedError):
+        transport.close()
+
 
 @requires_google_auth_gte_1_25_0
 def test_beta_analytics_data_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
@@ -2178,7 +2182,53 @@
         transports.BetaAnalyticsDataTransport, "_prep_wrapped_messages"
     ) as prep:
         transport_class = BetaAnalyticsDataClient.get_transport_class()
         transport = transport_class(
             credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
+
+
+@pytest.mark.asyncio
+async def test_transport_close_async():
+    client = BetaAnalyticsDataAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="grpc_asyncio",
+    )
+    with mock.patch.object(
+        type(getattr(client.transport, "grpc_channel")), "close"
+    ) as close:
+        async with client:
+            close.assert_not_called()
+        close.assert_called_once()
+
+
+def test_transport_close():
+    transports = {
+        "grpc": "_grpc_channel",
+    }
+
+    for transport, close_name in transports.items():
+        client = BetaAnalyticsDataClient(
+            credentials=ga_credentials.AnonymousCredentials(), transport=transport
+        )
+        with mock.patch.object(
+            type(getattr(client.transport, close_name)), "close"
+        ) as close:
+            with client:
+                close.assert_not_called()
+            close.assert_called_once()
+
+
+def test_client_ctx():
+    transports = [
+        "grpc",
+    ]
+    for transport in transports:
+        client = BetaAnalyticsDataClient(
+            credentials=ga_credentials.AnonymousCredentials(), transport=transport
+        )
+        # Test client calls underlying transport.
+        with mock.patch.object(type(client.transport), "close") as close:
+            close.assert_not_called()
+            with client:
+                pass
+            close.assert_called()
```

