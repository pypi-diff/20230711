# Comparing `tmp/wavefront-sdk-python-1.9.0.tar.gz` & `tmp/wavefront-sdk-python-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavefront-sdk-python-1.9.0.tar", last modified: Thu Jun 29 17:20:44 2023, max compression
+gzip compressed data, was "wavefront-sdk-python-2.0.0.tar", last modified: Tue Jul 11 20:11:26 2023, max compression
```

## Comparing `wavefront-sdk-python-1.9.0.tar` & `wavefront-sdk-python-2.0.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25008 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.239710 wavefront-sdk-python-1.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_applicaiton_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_histogram_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_wavefront_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_wavefront_metrics_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_wavefront_python_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.243710 wavefront-sdk-python-1.9.0/wavefront_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.243710 wavefront-sdk-python-1.9.0/wavefront_sdk/common/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/application_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/connection_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/heartbeater_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.243710 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/deltacounter.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/gauge.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/proxy_connection_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26131 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/direct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.243710 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.243710 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/event/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/event/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/histogram_granularity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/histogram_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/metrics/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/tracing/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/tracing/span_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/multi_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25008 2023-06-29 17:20:44.000000 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-29 17:20:44.000000 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:20:44.000000 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 17:20:44.000000 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 17:20:44.000000 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.687744 wavefront-sdk-python-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25008 2023-07-11 20:11:26.687744 wavefront-sdk-python-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:11:26.687744 wavefront-sdk-python-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.679744 wavefront-sdk-python-2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/test/test_applicaiton_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/test/test_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/test/test_histogram_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/test/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/test/test_wavefront_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/test/test_wavefront_metrics_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/test/test_wavefront_python_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.679744 wavefront-sdk-python-2.0.0/wavefront_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.683744 wavefront-sdk-python-2.0.0/wavefront_sdk/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/application_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/connection_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/heartbeater_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.683744 wavefront-sdk-python-2.0.0/wavefront_sdk/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/metrics/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/metrics/deltacounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/metrics/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/metrics/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/proxy_connection_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26131 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/direct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.683744 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.683744 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/event/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.683744 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/histogram/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/histogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/histogram/histogram_granularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/histogram/histogram_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/histogram/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.683744 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/metrics/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.687744 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/tracing/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/entities/tracing/span_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/multi_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-07-11 20:10:40.000000 wavefront-sdk-python-2.0.0/wavefront_sdk/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:11:26.687744 wavefront-sdk-python-2.0.0/wavefront_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25008 2023-07-11 20:11:26.000000 wavefront-sdk-python-2.0.0/wavefront_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-11 20:11:26.000000 wavefront-sdk-python-2.0.0/wavefront_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:11:26.000000 wavefront-sdk-python-2.0.0/wavefront_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 20:11:26.000000 wavefront-sdk-python-2.0.0/wavefront_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 20:11:26.000000 wavefront-sdk-python-2.0.0/wavefront_sdk_python.egg-info/top_level.txt
```

### Comparing `wavefront-sdk-python-1.9.0/LICENSE` & `wavefront-sdk-python-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/PKG-INFO` & `wavefront-sdk-python-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavefront-sdk-python
-Version: 1.9.0
+Version: 2.0.0
 Summary: VMware Aria Operations for Applications Python SDK
 Home-page: https://github.com/wavefrontHQ/wavefront-sdk-python
 Author: VMware Aria Operations for Applications Team
 License: Apache-2.0
 Keywords: Aria,Aria Operations,Aria Operations for Applications,3D Observability,Distributed Tracing,Histograms,Logging,Metrics,Monitoring,Observability,Tracing,VMware Aria,VMware Aria Operations,VMware Aria Operations for Applications,Wavefront,Wavefront SDK
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wavefront-sdk-python Version: 1.9.0 Summary: VMware
+Metadata-Version: 2.1 Name: wavefront-sdk-python Version: 2.0.0 Summary: VMware
 Aria Operations for Applications Python SDK Home-page: https://github.com/
 wavefrontHQ/wavefront-sdk-python Author: VMware Aria Operations for
 Applications Team License: Apache-2.0 Keywords: Aria,Aria Operations,Aria
 Operations for Applications,3D Observability,Distributed
 Tracing,Histograms,Logging,Metrics,Monitoring,Observability,Tracing,VMware
 Aria,VMware Aria Operations,VMware Aria Operations for
 Applications,Wavefront,Wavefront SDK Classifier: Development Status :: 5 -
```

### Comparing `wavefront-sdk-python-1.9.0/README.md` & `wavefront-sdk-python-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/setup.py` & `wavefront-sdk-python-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),
                        'README.md')) as fd:
     LONG_DESCRIPTION = fd.read()
 
 setuptools.setup(
     name='wavefront-sdk-python',
-    version='1.9.0',  # Please update with each pull request.
+    version='2.0.0',  # Please update with each pull request.
     author='VMware Aria Operations for Applications Team',
     url='https://github.com/wavefrontHQ/wavefront-sdk-python',
     license='Apache-2.0',
     description='VMware Aria Operations for Applications Python SDK',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     keywords=[
```

### Comparing `wavefront-sdk-python-1.9.0/test/test_applicaiton_tags.py` & `wavefront-sdk-python-2.0.0/test/test_applicaiton_tags.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/test/test_client.py` & `wavefront-sdk-python-2.0.0/test/test_client.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/test/test_direct.py` & `wavefront-sdk-python-2.0.0/test/test_direct.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/test/test_histogram_impl.py` & `wavefront-sdk-python-2.0.0/test/test_histogram_impl.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/test/test_proxy.py` & `wavefront-sdk-python-2.0.0/test/test_proxy.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/test/test_wavefront_client.py` & `wavefront-sdk-python-2.0.0/test/test_wavefront_client.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/test/test_wavefront_metrics_registry.py` & `wavefront-sdk-python-2.0.0/test/test_wavefront_metrics_registry.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/test/test_wavefront_python_sdk.py` & `wavefront-sdk-python-2.0.0/test/test_wavefront_python_sdk.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/__init__.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/client.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/client.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/client_factory.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/client_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 
     Create wavefront direct/proxy data ingestion client.
     """
 
     PROXY_SCHEME = "proxy"
     HTTP_PROXY_SCHEME = "http"
     DIRECT_DATA_INGESTION_SCHEME = "https"
-    clients = []
+
+    def __init__(self):
+        """Keep track of initialized clients on instance level."""
+        self.clients = []
 
     # pylint: disable=too-many-arguments
-    def add_client(self, url, max_queue_size=50000,
-                   batch_size=10000,
-                   flush_interval_seconds=5,
-                   enable_internal_metrics=True,
+    def add_client(self, url, max_queue_size=50000, batch_size=10000,
+                   flush_interval_seconds=5, enable_internal_metrics=True,
                    queue_impl=queue.Queue):
         """Create a unique client."""
         server, token = self.get_server_info_from_endpoint(url)
 
         if self.existing_client(server):
             raise RuntimeError("client with id " + url + " already exists.")
 
@@ -48,20 +49,20 @@
         """Get Server and API token from the end point.
 
         Return None for token if URL belongs to proxy.
         """
         base_url = urlparse(url)
         scheme = base_url.scheme
         if scheme == self.DIRECT_DATA_INGESTION_SCHEME:
-            server = f'{self.DIRECT_DATA_INGESTION_SCHEME}://' \
-                     f'{base_url.hostname}'
+            server = (f'{self.DIRECT_DATA_INGESTION_SCHEME}://'
+                      f'{base_url.hostname}')
             token = base_url.username
         elif scheme in (self.PROXY_SCHEME, self.HTTP_PROXY_SCHEME):
-            server = f'{self.HTTP_PROXY_SCHEME}://' \
-                     f'{base_url.hostname}:{base_url.port}'
+            server = (f'{self.HTTP_PROXY_SCHEME}://'
+                      f'{base_url.hostname}:{base_url.port}')
             token = None
         else:
             raise RuntimeError("Unknown scheme specified while attempting to"
                                " create a client " + str(scheme))
         return server, token
 
     def existing_client(self, server):
```

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/common/__init__.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/common/__init__.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/common/application_tags.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/common/application_tags.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/common/connection_handler.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/common/connection_handler.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/common/constants.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/common/constants.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/common/heartbeater_service.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/common/heartbeater_service.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/counter.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/common/metrics/counter.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/gauge.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/common/metrics/gauge.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/registry.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/common/metrics/registry.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/common/proxy_connection_handler.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/common/proxy_connection_handler.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/common/utils.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/common/utils.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/direct.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/direct.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/__init__.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/event/sender.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/entities/event/sender.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/histogram_impl.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/entities/histogram/histogram_impl.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/sender.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/entities/histogram/sender.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/metrics/sender.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/entities/metrics/sender.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/tracing/sender.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/entities/tracing/sender.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/multi_clients.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/multi_clients.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk/proxy.py` & `wavefront-sdk-python-2.0.0/wavefront_sdk/proxy.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/PKG-INFO` & `wavefront-sdk-python-2.0.0/wavefront_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavefront-sdk-python
-Version: 1.9.0
+Version: 2.0.0
 Summary: VMware Aria Operations for Applications Python SDK
 Home-page: https://github.com/wavefrontHQ/wavefront-sdk-python
 Author: VMware Aria Operations for Applications Team
 License: Apache-2.0
 Keywords: Aria,Aria Operations,Aria Operations for Applications,3D Observability,Distributed Tracing,Histograms,Logging,Metrics,Monitoring,Observability,Tracing,VMware Aria,VMware Aria Operations,VMware Aria Operations for Applications,Wavefront,Wavefront SDK
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wavefront-sdk-python Version: 1.9.0 Summary: VMware
+Metadata-Version: 2.1 Name: wavefront-sdk-python Version: 2.0.0 Summary: VMware
 Aria Operations for Applications Python SDK Home-page: https://github.com/
 wavefrontHQ/wavefront-sdk-python Author: VMware Aria Operations for
 Applications Team License: Apache-2.0 Keywords: Aria,Aria Operations,Aria
 Operations for Applications,3D Observability,Distributed
 Tracing,Histograms,Logging,Metrics,Monitoring,Observability,Tracing,VMware
 Aria,VMware Aria Operations,VMware Aria Operations for
 Applications,Wavefront,Wavefront SDK Classifier: Development Status :: 5 -
```

### Comparing `wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/SOURCES.txt` & `wavefront-sdk-python-2.0.0/wavefront_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

