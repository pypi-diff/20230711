# Comparing `tmp/quao-0.2.9.tar.gz` & `tmp/quao-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.2.9.tar", last modified: Tue Jun 20 02:35:13 2023, max compression
+gzip compressed data, was "quao-0.3.0.tar", last modified: Tue Jul 11 10:42:30 2023, max compression
```

## Comparing `quao-0.2.9.tar` & `quao-0.3.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.709144 quao-0.2.9/
--rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-06-20 02:35:13.708144 quao-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.2.9/README.md
--rw-rw-rw-   0        0        0      952 2023-06-20 02:34:43.000000 quao-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 02:35:13.709144 quao-0.2.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.650045 quao-0.2.9/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.9/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.653043 quao-0.2.9/src/quao/
--rw-rw-rw-   0        0        0      203 2023-06-20 02:34:43.000000 quao-0.2.9/src/quao/__init__.py
--rw-rw-rw-   0        0        0     6636 2023-06-19 01:49:45.000000 quao-0.2.9/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.661045 quao-0.2.9/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.2.9/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      193 2023-06-15 04:25:14.000000 quao-0.2.9/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.662044 quao-0.2.9/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.663044 quao-0.2.9/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      942 2023-06-19 01:49:45.000000 quao-0.2.9/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.665044 quao-0.2.9/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      680 2023-06-16 07:14:53.000000 quao-0.2.9/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.677044 quao-0.2.9/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      185 2023-06-15 04:16:49.000000 quao-0.2.9/src/quao/enum/http_header.py
--rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.2.9/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-13 03:37:41.000000 quao-0.2.9/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/enum/sdk.py
--rw-rw-rw-   0        0        0      169 2023-06-16 09:12:10.000000 quao-0.2.9/src/quao/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.681045 quao-0.2.9/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.2.9/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.2.9/src/quao/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.682045 quao-0.2.9/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.691950 quao-0.2.9/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     1612 2023-06-19 02:14:23.000000 quao-0.2.9/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3198 2023-06-19 02:14:23.000000 quao-0.2.9/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1015 2023-06-15 04:25:14.000000 quao-0.2.9/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      795 2023-06-15 04:25:14.000000 quao-0.2.9/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0      876 2023-06-19 02:14:23.000000 quao-0.2.9/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     2734 2023-06-19 02:14:23.000000 quao-0.2.9/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.693951 quao-0.2.9/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     2693 2023-06-02 10:41:04.000000 quao-0.2.9/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.701954 quao-0.2.9/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1258 2023-06-15 04:25:14.000000 quao-0.2.9/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1011 2023-06-15 04:25:14.000000 quao-0.2.9/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      881 2023-06-15 04:25:14.000000 quao-0.2.9/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.2.9/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1456 2023-06-16 07:07:16.000000 quao-0.2.9/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.705953 quao-0.2.9/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.2.9/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.2.9/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1568 2023-06-19 01:49:45.000000 quao-0.2.9/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 02:35:13.658045 quao-0.2.9/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-06-20 02:35:13.000000 quao-0.2.9/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1537 2023-06-20 02:35:13.000000 quao-0.2.9/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 02:35:13.000000 quao-0.2.9/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      194 2023-06-20 02:35:13.000000 quao-0.2.9/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-20 02:35:13.000000 quao-0.2.9/src/quao.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.365906 quao-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-07-10 09:49:01.000000 quao-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-11 10:42:30.365906 quao-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-10 09:49:01.000000 quao-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-07-11 10:42:07.000000 quao-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 10:42:30.365906 quao-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.353906 quao-0.3.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.353906 quao-0.3.0/src/quao/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-11 10:42:07.000000 quao-0.3.0/src/quao/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6752 2023-07-11 10:42:07.000000 quao-0.3.0/src/quao/backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.353906 quao-0.3.0/src/quao/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/config/logging_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.357906 quao-0.3.0/src/quao/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.357906 quao-0.3.0/src/quao/data/job/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/data/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/data/job/job_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.357906 quao-0.3.0/src/quao/data/request/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/data/request/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/data/request/request_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.357906 quao-0.3.0/src/quao/enum/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/enum/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/enum/http_header.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/enum/http_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/enum/job_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/enum/media_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/enum/provider_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/enum/sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/enum/token_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.357906 quao-0.3.0/src/quao/factory/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/factory/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/factory/device_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/factory/provider_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.361906 quao-0.3.0/src/quao/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.361906 quao-0.3.0/src/quao/model/device/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/device/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2245 2023-07-11 10:42:07.000000 quao-0.3.0/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/device/device.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/device/quao_device.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.361906 quao-0.3.0/src/quao/model/job/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2023-07-11 10:42:07.000000 quao-0.3.0/src/quao/model/job/qiskit_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.365906 quao-0.3.0/src/quao/model/provider/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      968 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/provider/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/model/provider/quao_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.365906 quao-0.3.0/src/quao/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-10 09:49:01.000000 quao-0.3.0/src/quao/util/response_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:42:30.353906 quao-0.3.0/src/quao.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-11 10:42:30.000000 quao-0.3.0/src/quao.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-07-11 10:42:30.000000 quao-0.3.0/src/quao.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 10:42:30.000000 quao-0.3.0/src/quao.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      201 2023-07-11 10:42:30.000000 quao-0.3.0/src/quao.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 10:42:30.000000 quao-0.3.0/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.2.9/LICENSE` & `quao-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-The MIT License (MIT)
-Copyright © CITYNOW Co. Ltd. All rights reserved.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+The MIT License (MIT)
+Copyright © CITYNOW Co. Ltd. All rights reserved.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `quao-0.2.9/PKG-INFO` & `quao-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-Metadata-Version: 2.1
-Name: quao
-Version: 0.2.9
-Summary: Quao Library supporting Quao Platform for Quantum Computing
-Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
-License: The MIT License (MIT)
-        Copyright © CITYNOW Co. Ltd. All rights reserved.
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Homepage, https://citynow.vn/
-Keywords: quao,quantum
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-
-# quao 
-
-quao is a supporting library for Quantum Computing.
-
-
-
-## Installation
-
-Install quao with pip (Python >=3.10)
-
-```bash
-  pip install quao
-```
-    
-## Usage/Examples
-
-```javascript
-from quao import Backend, RequestData, Utils
-
-# Define sdk name
-sdk = "qiskit"
-
-# Pre-processing input data
-def pre_process(input):
-    data = RequestData(input, sdk)
-    return data
-
-# Post-processing output data
-def post_process(job):
-    output = Utils.counts_post_process(job)
-    return output
-
-
-def handle(event, context):
-    # 1. Pre-processing
-    requestData = pre_process(event)
-
-    # 2. Generate Quantum Circuit
-    qc = generate_circuit(requestData.input)
-
-    # 3. Verify and get Backend information
-    backend = Backend(requestData, qc)
-
-    # 4. Submit job and wait up to 1 min for job to complete.
-    job = backend.submit_job(qc)
-
-    # 5. Post-process
-    if job.jobResult:
-        job = post_process(job)
-    response = Utils.generate_response(job)
-
-    # 6. Send back the result
-    return response
-```
-
-
-## Authors
-
-- [CITYNOW Co. Ltd.](https://citynow.vn/)
-
-
-## Documentation
-
-TBA
-
+Metadata-Version: 2.1
+Name: quao
+Version: 0.3.0
+Summary: Quao Library supporting Quao Platform for Quantum Computing
+Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
+License: The MIT License (MIT)
+        Copyright © CITYNOW Co. Ltd. All rights reserved.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: Homepage, https://citynow.vn/
+Keywords: quao,quantum
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+
+# quao 
+
+quao is a supporting library for Quantum Computing.
+
+
+
+## Installation
+
+Install quao with pip (Python >=3.10)
+
+```bash
+  pip install quao
+```
+    
+## Usage/Examples
+
+```javascript
+from quao import Backend, RequestData, Utils
+
+# Define sdk name
+sdk = "qiskit"
+
+# Pre-processing input data
+def pre_process(input):
+    data = RequestData(input, sdk)
+    return data
+
+# Post-processing output data
+def post_process(job):
+    output = Utils.counts_post_process(job)
+    return output
+
+
+def handle(event, context):
+    # 1. Pre-processing
+    requestData = pre_process(event)
+
+    # 2. Generate Quantum Circuit
+    qc = generate_circuit(requestData.input)
+
+    # 3. Verify and get Backend information
+    backend = Backend(requestData, qc)
+
+    # 4. Submit job and wait up to 1 min for job to complete.
+    job = backend.submit_job(qc)
+
+    # 5. Post-process
+    if job.jobResult:
+        job = post_process(job)
+    response = Utils.generate_response(job)
+
+    # 6. Send back the result
+    return response
+```
+
+
+## Authors
+
+- [CITYNOW Co. Ltd.](https://citynow.vn/)
+
+
+## Documentation
+
+TBA
+
```

### Comparing `quao-0.2.9/README.md` & `quao-0.3.0/README.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-
-# quao 
-
-quao is a supporting library for Quantum Computing.
-
-
-
-## Installation
-
-Install quao with pip (Python >=3.10)
-
-```bash
-  pip install quao
-```
-    
-## Usage/Examples
-
-```javascript
-from quao import Backend, RequestData, Utils
-
-# Define sdk name
-sdk = "qiskit"
-
-# Pre-processing input data
-def pre_process(input):
-    data = RequestData(input, sdk)
-    return data
-
-# Post-processing output data
-def post_process(job):
-    output = Utils.counts_post_process(job)
-    return output
-
-
-def handle(event, context):
-    # 1. Pre-processing
-    requestData = pre_process(event)
-
-    # 2. Generate Quantum Circuit
-    qc = generate_circuit(requestData.input)
-
-    # 3. Verify and get Backend information
-    backend = Backend(requestData, qc)
-
-    # 4. Submit job and wait up to 1 min for job to complete.
-    job = backend.submit_job(qc)
-
-    # 5. Post-process
-    if job.jobResult:
-        job = post_process(job)
-    response = Utils.generate_response(job)
-
-    # 6. Send back the result
-    return response
-```
-
-
-## Authors
-
-- [CITYNOW Co. Ltd.](https://citynow.vn/)
-
-
-## Documentation
-
-TBA
-
+
+# quao 
+
+quao is a supporting library for Quantum Computing.
+
+
+
+## Installation
+
+Install quao with pip (Python >=3.10)
+
+```bash
+  pip install quao
+```
+    
+## Usage/Examples
+
+```javascript
+from quao import Backend, RequestData, Utils
+
+# Define sdk name
+sdk = "qiskit"
+
+# Pre-processing input data
+def pre_process(input):
+    data = RequestData(input, sdk)
+    return data
+
+# Post-processing output data
+def post_process(job):
+    output = Utils.counts_post_process(job)
+    return output
+
+
+def handle(event, context):
+    # 1. Pre-processing
+    requestData = pre_process(event)
+
+    # 2. Generate Quantum Circuit
+    qc = generate_circuit(requestData.input)
+
+    # 3. Verify and get Backend information
+    backend = Backend(requestData, qc)
+
+    # 4. Submit job and wait up to 1 min for job to complete.
+    job = backend.submit_job(qc)
+
+    # 5. Post-process
+    if job.jobResult:
+        job = post_process(job)
+    response = Utils.generate_response(job)
+
+    # 6. Send back the result
+    return response
+```
+
+
+## Authors
+
+- [CITYNOW Co. Ltd.](https://citynow.vn/)
+
+
+## Documentation
+
+TBA
+
```

### Comparing `quao-0.2.9/pyproject.toml` & `quao-0.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "quao"
-version = "0.2.9"
-description = "Quao Library supporting Quao Platform for Quantum Computing"
-readme = "README.md"
-authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
-license = { file = "LICENSE" }
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-]
-keywords = ["quao", "quantum"]
-dependencies = [
-    "qiskit==0.42.1",
-    "qiskit-aer==0.12.0",
-    "qiskit-aer-gpu",
-    "qbraid==0.4.0",
-    "amazon-braket-sdk==1.38.1",
-    "qiskit-ibm-runtime",
-    "qiskit-ibm-provider",
-    "matplotlib",
-    "pylatexenc"
-]
-requires-python = ">=3.7"
-
-[project.optional-dependencies]
-dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
-
-[project.urls]
-Homepage = "https://citynow.vn/"
-
+
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "quao"
+version = "0.3.0"
+description = "Quao Library supporting Quao Platform for Quantum Computing"
+readme = "README.md"
+authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
+license = { file = "LICENSE" }
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+]
+keywords = ["quao", "quantum"]
+dependencies = [
+    "qiskit==0.42.1",
+    "qiskit-aer==0.12.0",
+    "qiskit-aer-gpu",
+    "qbraid==0.4.0",
+    "amazon-braket-sdk==1.38.1",
+    "qiskit-ibm-runtime",
+    "qiskit-ibm-provider",
+    "matplotlib",
+    "pylatexenc",
+    "loguru"
+]
+requires-python = ">=3.7"
+
+[project.optional-dependencies]
+dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+
+[project.urls]
+Homepage = "https://citynow.vn/"
+
```

### Comparing `quao-0.2.9/src/quao/data/job/job_response.py` & `quao-0.3.0/src/quao/data/job/job_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-"""
-    QuaO Project job_response.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from ...enum.media_type import MediaType
-from ...enum.job_status import JobStatus
-
-
-class JobResponse(object):
-    def __init__(
-            self,
-            provider_job_id: str = "",
-            job_status: str = "",
-            job_result=None,
-            content_type=None,
-            job_histogram=None,
-            user_identity="",
-            user_token=""
-    ):
-        self.provider_job_id = provider_job_id if provider_job_id else ""
-        self.job_status = job_status if job_status else JobStatus.ERROR.value
-        self.job_result = job_result if job_result else None
-        self.content_type = content_type if content_type else MediaType.ALL_TYPE.value
-        self.job_histogram = job_histogram if job_histogram else None
-        self.user_identity = user_identity
-        self.user_token = user_token
+"""
+    QuaO Project job_response.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from ...enum.media_type import MediaType
+from ...enum.job_status import JobStatus
+
+
+class JobResponse(object):
+    def __init__(
+            self,
+            provider_job_id: str = "",
+            job_status: str = "",
+            job_result=None,
+            content_type=None,
+            job_histogram=None,
+            user_identity="",
+            user_token="",
+            execution_time=None
+    ):
+        self.provider_job_id = provider_job_id if provider_job_id else ""
+        self.job_status = job_status if job_status else JobStatus.ERROR.value
+        self.job_result = job_result
+        self.content_type = content_type if content_type else MediaType.ALL_TYPE.value
+        self.job_histogram = job_histogram
+        self.user_identity = user_identity
+        self.user_token = user_token
+        self.execution_time = execution_time
```

### Comparing `quao-0.2.9/src/quao/data/request/request_data.py` & `quao-0.3.0/src/quao/data/request/request_data.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""
-    QuaO Project request_data.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-
-
-class RequestData:
-
-    def __init__(self, event):
-        json_data = event.json()
-        self.data = json_data
-        self.input = json_data.get("input")
-        self.shots = json_data.get("shots")
-        self.device_id = json_data.get("deviceId")
-        self.sdk = json_data.get("sdk").lower() if json_data.get("sdk") else None
-        self.server_url = json_data.get("serverUrl")
-        self.circuit_export_url = json_data.get("circuitExportUrl")
-        self.user_token = json_data.get("userToken")
-        self.user_identity = json_data.get("userIdentity")
+"""
+    QuaO Project request_data.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+
+
+class RequestData:
+
+    def __init__(self, event):
+        json_data = event.json()
+        self.data = json_data
+        self.input = json_data.get("input")
+        self.shots = json_data.get("shots")
+        self.device_id = json_data.get("deviceId")
+        self.sdk = json_data.get("sdk").lower() if json_data.get("sdk") else None
+        self.server_url = json_data.get("serverUrl")
+        self.circuit_export_url = json_data.get("circuitExportUrl")
+        self.user_token = json_data.get("userToken")
+        self.user_identity = json_data.get("userIdentity")
```

### Comparing `quao-0.2.9/src/quao/factory/provider_factory.py` & `quao-0.3.0/src/quao/factory/provider_factory.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-    QuaO Project provider_factory.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from ..enum.provider_type import ProviderType
-from ..model.provider.aws_braket_provider import AwsBraketProvider
-from ..model.provider.ibm_cloud_provider import IbmCloudProvider
-from ..model.provider.ibm_quantum_provider import IbmQuantumProvider
-from ..model.provider.quao_provider import QuaoProvider
-
-
-class ProviderFactory:
-
-    @staticmethod
-    def create_provider(provider_type: str, authentication: dict):
-        """
-
-        @param provider_type:
-        @param authentication:
-        @return:
-        """
-
-        if ProviderType.QUAO_QUANTUM_SIMULATOR.value.__eq__(provider_type):
-            return QuaoProvider()
-
-        if ProviderType.IBM_QUANTUM.value.__eq__(provider_type):
-            return IbmQuantumProvider(authentication.get('token'))
-
-        if ProviderType.IBM_CLOUD.value.__eq__(provider_type):
-            return IbmCloudProvider(authentication.get('token'), authentication.get('crn'))
-
-        if ProviderType.AWS_BRAKET.value.__eq__(provider_type):
-            return AwsBraketProvider(
-                authentication.get('accessKey'),
-                authentication.get('secretKey'),
-                authentication.get('regionName'))
-
-        raise Exception("Unsupported provider!")
+"""
+    QuaO Project provider_factory.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from ..enum.provider_type import ProviderType
+from ..model.provider.aws_braket_provider import AwsBraketProvider
+from ..model.provider.ibm_cloud_provider import IbmCloudProvider
+from ..model.provider.ibm_quantum_provider import IbmQuantumProvider
+from ..model.provider.quao_provider import QuaoProvider
+
+
+class ProviderFactory:
+
+    @staticmethod
+    def create_provider(provider_type: str, authentication: dict):
+        """
+
+        @param provider_type:
+        @param authentication:
+        @return:
+        """
+
+        if ProviderType.QUAO_QUANTUM_SIMULATOR.value.__eq__(provider_type):
+            return QuaoProvider()
+
+        if ProviderType.IBM_QUANTUM.value.__eq__(provider_type):
+            return IbmQuantumProvider(authentication.get('token'))
+
+        if ProviderType.IBM_CLOUD.value.__eq__(provider_type):
+            return IbmCloudProvider(authentication.get('token'), authentication.get('crn'))
+
+        if ProviderType.AWS_BRAKET.value.__eq__(provider_type):
+            return AwsBraketProvider(
+                authentication.get('accessKey'),
+                authentication.get('secretKey'),
+                authentication.get('regionName'))
+
+        raise Exception("Unsupported provider!")
```

### Comparing `quao-0.2.9/src/quao/model/device/qiskit_device.py` & `quao-0.3.0/src/quao/model/device/qiskit_device.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,40 @@
-"""
-    QuaO Project qiskit_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from abc import ABC
-
-from qiskit import QiskitError
-
-from ...model.device.device import Device
-from ...config.logging_config import logging
-
-
-class QiskitDevice(Device, ABC):
-
-    def _produce_histogram_data(self, job_result) -> dict:
-        try:
-            histogram_data = job_result.get_counts()
-        except QiskitError as qiskit_error:
-            logging.debug("Can't produce histogram with error: {0}".format(str(qiskit_error)))
-            histogram_data = None
-
-        return histogram_data
-
-    def _get_provider_job_id(self, job) -> str:
-        return job.job_id()
-
-    def _get_job_status(self, job) -> str:
-        return job.status().name
-
-    def _get_name(self) -> str:
-        return str(self.device.configuration().backend_name)
+"""
+    QuaO Project qiskit_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from abc import ABC
+
+from qiskit import QiskitError
+
+from ...model.device.device import Device
+from ...config.logging_config import *
+
+
+class QiskitDevice(Device, ABC):
+
+    def _produce_histogram_data(self, job_result) -> dict:
+        try:
+            histogram_data = job_result.get_counts()
+        except QiskitError as qiskit_error:
+            logger.debug("Can't produce histogram with error: {0}".format(str(qiskit_error)))
+            histogram_data = None
+
+        return histogram_data
+
+    def _get_provider_job_id(self, job) -> str:
+        return job.job_id()
+
+    def _get_job_status(self, job) -> str:
+        return job.status().name
+
+    def _get_name(self) -> str:
+        return str(self.device.configuration().backend_name)
+
+    def _get_execution_time(self, job_result):
+        metadata = job_result['metadata']
+
+        if metadata is None:
+            return self.execution_time
+
+        self.execution_time = metadata['time_taken_execute']
+
+        return self.execution_time
```

### Comparing `quao-0.2.9/src/quao/model/provider/aws_braket_provider.py` & `quao-0.3.0/src/quao/model/provider/aws_braket_provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-    QuaO Project aws_braket_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-import boto3
-from braket.aws import AwsSession, AwsDevice
-
-from ...enum.provider_type import ProviderType
-from ...model.provider.provider import Provider
-from ...config.logging_config import logging
-
-
-class AwsBraketProvider(Provider):
-
-    def __init__(self, aws_access_key, aws_secret_access_key, region_name):
-        super().__init__(ProviderType.AWS_BRAKET)
-        self.aws_access_key = aws_access_key
-        self.aws_secret_access_key = aws_secret_access_key
-        self.region_name = region_name
-
-    def get_backend(self, device_specification: str):
-        """
-
-        @param device_specification:
-        """
-
-        session = self.collect_providers()
-        return AwsDevice(
-            arn=device_specification,
-            aws_session=session)
-
-    def collect_providers(self):
-        """
-
-        """
-
-        logging.debug('Connect to Aws Braket provider')
-        session = boto3.Session(
-            aws_access_key_id=self.aws_access_key,
-            aws_secret_access_key=self.aws_secret_access_key,
-            region_name=self.region_name)
-
-        return AwsSession(boto_session=session)
+"""
+    QuaO Project aws_braket_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+import boto3
+from braket.aws import AwsSession, AwsDevice
+
+from ...enum.provider_type import ProviderType
+from ...model.provider.provider import Provider
+from ...config.logging_config import *
+
+
+class AwsBraketProvider(Provider):
+
+    def __init__(self, aws_access_key, aws_secret_access_key, region_name):
+        super().__init__(ProviderType.AWS_BRAKET)
+        self.aws_access_key = aws_access_key
+        self.aws_secret_access_key = aws_secret_access_key
+        self.region_name = region_name
+
+    def get_backend(self, device_specification: str):
+        """
+
+        @param device_specification:
+        """
+
+        session = self.collect_providers()
+        return AwsDevice(
+            arn=device_specification,
+            aws_session=session)
+
+    def collect_providers(self):
+        """
+
+        """
+
+        logger.debug('Connect to Aws Braket provider')
+        session = boto3.Session(
+            aws_access_key_id=self.aws_access_key,
+            aws_secret_access_key=self.aws_secret_access_key,
+            region_name=self.region_name)
+
+        return AwsSession(boto_session=session)
```

### Comparing `quao-0.2.9/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.3.0/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-    QuaO Project ibm_cloud_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from qiskit_ibm_runtime import QiskitRuntimeService
-
-from ...enum.provider_type import ProviderType
-from ...model.provider.provider import Provider
-from ...config.logging_config import logging
-
-
-class IbmCloudProvider(Provider):
-
-    def __init__(self, api_key, crn):
-        super().__init__(ProviderType.IBM_CLOUD)
-        self.api_key = api_key
-        self.crn = crn
-        self.channel = 'ibm_cloud'
-
-    def get_backend(self, device_specification: str):
-        """
-
-        @param device_specification:
-        @return:
-        """
-        provider = self.collect_providers()
-
-        return provider.get_backend(name=device_specification)
-
-    def collect_providers(self):
-        """
-
-        @return:
-        """
-
-        logging.debug('Connect to Ibm Cloud provider')
-        return QiskitRuntimeService(channel=self.channel, token=self.api_key, instance=self.crn)
+"""
+    QuaO Project ibm_cloud_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from qiskit_ibm_runtime import QiskitRuntimeService
+
+from ...enum.provider_type import ProviderType
+from ...model.provider.provider import Provider
+from ...config.logging_config import *
+
+
+class IbmCloudProvider(Provider):
+
+    def __init__(self, api_key, crn):
+        super().__init__(ProviderType.IBM_CLOUD)
+        self.api_key = api_key
+        self.crn = crn
+        self.channel = 'ibm_cloud'
+
+    def get_backend(self, device_specification: str):
+        """
+
+        @param device_specification:
+        @return:
+        """
+        provider = self.collect_providers()
+
+        return provider.get_backend(name=device_specification)
+
+    def collect_providers(self):
+        """
+
+        @return:
+        """
+
+        logger.debug('Connect to Ibm Cloud provider')
+        return QiskitRuntimeService(channel=self.channel, token=self.api_key, instance=self.crn)
```

### Comparing `quao-0.2.9/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.3.0/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-    QuaO Project ibm_quantum_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from qiskit_ibm_provider import IBMProvider
-
-from ...enum.provider_type import ProviderType
-from ...model.provider.provider import Provider
-from ...config.logging_config import logging
-
-
-class IbmQuantumProvider(Provider):
-    def __init__(self, api_token):
-        super().__init__(ProviderType.IBM_QUANTUM)
-        self.api_token = api_token
-
-    def get_backend(self, device_specification: str):
-        """
-
-        @param device_specification:
-        """
-
-        provider = self.collect_providers()
-
-        return provider.get_backend(device_specification)
-
-    def collect_providers(self):
-        """
-
-        @return:
-        """
-
-        logging.debug('Connect to Ibm Quantum provider')
-        return IBMProvider(token=self.api_token)
+"""
+    QuaO Project ibm_quantum_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from qiskit_ibm_provider import IBMProvider
+
+from ...enum.provider_type import ProviderType
+from ...model.provider.provider import Provider
+from ...config.logging_config import *
+
+
+class IbmQuantumProvider(Provider):
+    def __init__(self, api_token):
+        super().__init__(ProviderType.IBM_QUANTUM)
+        self.api_token = api_token
+
+    def get_backend(self, device_specification: str):
+        """
+
+        @param device_specification:
+        """
+
+        provider = self.collect_providers()
+
+        return provider.get_backend(device_specification)
+
+    def collect_providers(self):
+        """
+
+        @return:
+        """
+
+        logger.debug('Connect to Ibm Quantum provider')
+        return IBMProvider(token=self.api_token)
```

### Comparing `quao-0.2.9/src/quao.egg-info/PKG-INFO` & `quao-0.3.0/src/quao.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-Metadata-Version: 2.1
-Name: quao
-Version: 0.2.9
-Summary: Quao Library supporting Quao Platform for Quantum Computing
-Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
-License: The MIT License (MIT)
-        Copyright © CITYNOW Co. Ltd. All rights reserved.
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Homepage, https://citynow.vn/
-Keywords: quao,quantum
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-
-# quao 
-
-quao is a supporting library for Quantum Computing.
-
-
-
-## Installation
-
-Install quao with pip (Python >=3.10)
-
-```bash
-  pip install quao
-```
-    
-## Usage/Examples
-
-```javascript
-from quao import Backend, RequestData, Utils
-
-# Define sdk name
-sdk = "qiskit"
-
-# Pre-processing input data
-def pre_process(input):
-    data = RequestData(input, sdk)
-    return data
-
-# Post-processing output data
-def post_process(job):
-    output = Utils.counts_post_process(job)
-    return output
-
-
-def handle(event, context):
-    # 1. Pre-processing
-    requestData = pre_process(event)
-
-    # 2. Generate Quantum Circuit
-    qc = generate_circuit(requestData.input)
-
-    # 3. Verify and get Backend information
-    backend = Backend(requestData, qc)
-
-    # 4. Submit job and wait up to 1 min for job to complete.
-    job = backend.submit_job(qc)
-
-    # 5. Post-process
-    if job.jobResult:
-        job = post_process(job)
-    response = Utils.generate_response(job)
-
-    # 6. Send back the result
-    return response
-```
-
-
-## Authors
-
-- [CITYNOW Co. Ltd.](https://citynow.vn/)
-
-
-## Documentation
-
-TBA
-
+Metadata-Version: 2.1
+Name: quao
+Version: 0.3.0
+Summary: Quao Library supporting Quao Platform for Quantum Computing
+Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
+License: The MIT License (MIT)
+        Copyright © CITYNOW Co. Ltd. All rights reserved.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: Homepage, https://citynow.vn/
+Keywords: quao,quantum
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+
+# quao 
+
+quao is a supporting library for Quantum Computing.
+
+
+
+## Installation
+
+Install quao with pip (Python >=3.10)
+
+```bash
+  pip install quao
+```
+    
+## Usage/Examples
+
+```javascript
+from quao import Backend, RequestData, Utils
+
+# Define sdk name
+sdk = "qiskit"
+
+# Pre-processing input data
+def pre_process(input):
+    data = RequestData(input, sdk)
+    return data
+
+# Post-processing output data
+def post_process(job):
+    output = Utils.counts_post_process(job)
+    return output
+
+
+def handle(event, context):
+    # 1. Pre-processing
+    requestData = pre_process(event)
+
+    # 2. Generate Quantum Circuit
+    qc = generate_circuit(requestData.input)
+
+    # 3. Verify and get Backend information
+    backend = Backend(requestData, qc)
+
+    # 4. Submit job and wait up to 1 min for job to complete.
+    job = backend.submit_job(qc)
+
+    # 5. Post-process
+    if job.jobResult:
+        job = post_process(job)
+    response = Utils.generate_response(job)
+
+    # 6. Send back the result
+    return response
+```
+
+
+## Authors
+
+- [CITYNOW Co. Ltd.](https://citynow.vn/)
+
+
+## Documentation
+
+TBA
+
```

### Comparing `quao-0.2.9/src/quao.egg-info/SOURCES.txt` & `quao-0.3.0/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

