# Comparing `tmp/etcd-sdk-python-0.0.2.tar.gz` & `tmp/etcd-sdk-python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etcd-sdk-python-0.0.2.tar", last modified: Tue Jun  6 09:12:17 2023, max compression
+gzip compressed data, was "etcd-sdk-python-0.0.3.tar", last modified: Tue Jul 11 03:13:54 2023, max compression
```

## Comparing `etcd-sdk-python-0.0.2.tar` & `etcd-sdk-python-0.0.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-06 09:12:17.548185 etcd-sdk-python-0.0.2/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       92 2023-06-06 09:05:46.000000 etcd-sdk-python-0.0.2/.gitignore
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      270 2023-04-10 06:46:04.000000 etcd-sdk-python-0.0.2/AUTHORS.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      207 2023-04-11 06:23:12.000000 etcd-sdk-python-0.0.2/CONTRIBUTING.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11367 2023-04-10 06:48:42.000000 etcd-sdk-python-0.0.2/LICENSE
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3552 2023-06-06 09:12:17.544185 etcd-sdk-python-0.0.2/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2911 2023-06-06 09:10:20.000000 etcd-sdk-python-0.0.2/README.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      449 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.2/docker-compose.yml
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-06 09:12:17.536186 etcd-sdk-python-0.0.2/docs/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      638 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/docs/Makefile
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1858 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/docs/README.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      799 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/docs/make.bat
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-06 09:12:17.540186 etcd-sdk-python-0.0.2/docs/source/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-06 09:12:17.540186 etcd-sdk-python-0.0.2/docs/source/_templates/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       98 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/docs/source/_templates/autosummaryclass.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      389 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/docs/source/_templates/layout.html
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       56 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/docs/source/authors.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3184 2023-04-10 09:41:40.000000 etcd-sdk-python-0.0.2/docs/source/conf.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       76 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/docs/source/contributing.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      237 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/docs/source/index.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      521 2023-04-10 10:04:46.000000 etcd-sdk-python-0.0.2/docs/source/install.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       52 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/docs/source/readme.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1260 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/docs/source/usage.rst
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-06 09:12:17.540186 etcd-sdk-python-0.0.2/etcd_sdk_python.egg-info/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3552 2023-06-06 09:12:17.000000 etcd-sdk-python-0.0.2/etcd_sdk_python.egg-info/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1336 2023-06-06 09:12:17.000000 etcd-sdk-python-0.0.2/etcd_sdk_python.egg-info/SOURCES.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        1 2023-06-06 09:12:17.000000 etcd-sdk-python-0.0.2/etcd_sdk_python.egg-info/dependency_links.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       54 2023-06-06 09:12:17.000000 etcd-sdk-python-0.0.2/etcd_sdk_python.egg-info/requires.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        7 2023-06-06 09:12:17.000000 etcd-sdk-python-0.0.2/etcd_sdk_python.egg-info/top_level.txt
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-06 09:12:17.540186 etcd-sdk-python-0.0.2/pyetcd/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      531 2023-04-11 06:17:37.000000 etcd-sdk-python-0.0.2/pyetcd/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      211 2023-06-06 09:07:20.000000 etcd-sdk-python-0.0.2/pyetcd/__version__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    48403 2023-04-25 02:57:06.000000 etcd-sdk-python-0.0.2/pyetcd/client.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-06 09:12:17.544185 etcd-sdk-python-0.0.2/pyetcd/etcdrpc/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       75 2023-04-11 05:43:20.000000 etcd-sdk-python-0.0.2/pyetcd/etcdrpc/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1678 2023-04-11 05:43:20.000000 etcd-sdk-python-0.0.2/pyetcd/etcdrpc/auth_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1829 2023-04-11 05:43:20.000000 etcd-sdk-python-0.0.2/pyetcd/etcdrpc/auth_pb2.pyi
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1656 2023-04-11 05:43:20.000000 etcd-sdk-python-0.0.2/pyetcd/etcdrpc/kv_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1631 2023-04-11 05:43:20.000000 etcd-sdk-python-0.0.2/pyetcd/etcdrpc/kv_pb2.pyi
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    26274 2023-04-11 05:43:20.000000 etcd-sdk-python-0.0.2/pyetcd/etcdrpc/rpc_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    32187 2023-04-11 05:43:20.000000 etcd-sdk-python-0.0.2/pyetcd/etcdrpc/rpc_pb2.pyi
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    63388 2023-04-11 05:43:20.000000 etcd-sdk-python-0.0.2/pyetcd/etcdrpc/rpc_pb2_grpc.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1061 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/pyetcd/events.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      681 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/pyetcd/exceptions.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      858 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/pyetcd/leases.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4437 2023-04-17 12:26:35.000000 etcd-sdk-python-0.0.2/pyetcd/locks.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1503 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/pyetcd/members.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-06 09:12:17.544185 etcd-sdk-python-0.0.2/pyetcd/proto/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1170 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/pyetcd/proto/auth.proto
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2078 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/pyetcd/proto/kv.proto
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    29842 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/pyetcd/proto/rpc.proto
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2987 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/pyetcd/transactions.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1132 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.2/pyetcd/utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8161 2023-04-17 13:22:33.000000 etcd-sdk-python-0.0.2/pyetcd/watch.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1456 2023-06-06 09:08:57.000000 etcd-sdk-python-0.0.2/pyproject.toml
--rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1711 2023-04-11 05:44:56.000000 etcd-sdk-python-0.0.2/python_gen.sh
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      396 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.2/requirements.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       38 2023-06-06 09:12:17.548185 etcd-sdk-python-0.0.2/setup.cfg
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-06-06 09:12:17.544185 etcd-sdk-python-0.0.2/tests/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       24 2023-04-10 08:02:48.000000 etcd-sdk-python-0.0.2/tests/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1919 2023-04-10 06:30:33.000000 etcd-sdk-python-0.0.2/tests/ca.crt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1793 2023-04-10 06:30:33.000000 etcd-sdk-python-0.0.2/tests/client.crt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3243 2023-04-10 06:30:33.000000 etcd-sdk-python-0.0.2/tests/client.key
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      755 2023-04-17 12:48:24.000000 etcd-sdk-python-0.0.2/tests/conftest.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1471 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.2/tests/test_alarms.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4199 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.2/tests/test_client.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2410 2023-04-17 12:39:05.000000 etcd-sdk-python-0.0.2/tests/test_compares.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      345 2023-04-17 12:40:16.000000 etcd-sdk-python-0.0.2/tests/test_credentials.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3828 2023-04-17 12:48:23.000000 etcd-sdk-python-0.0.2/tests/test_failover.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    37953 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.2/tests/test_pyetcd.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      599 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.2/tests/test_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1046 2023-04-26 03:17:29.000000 etcd-sdk-python-0.0.2/tox.ini
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-07-11 03:13:54.169890 etcd-sdk-python-0.0.3/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       92 2023-07-11 03:04:13.000000 etcd-sdk-python-0.0.3/.gitignore
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      270 2023-04-10 06:46:04.000000 etcd-sdk-python-0.0.3/AUTHORS.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      207 2023-04-11 06:23:12.000000 etcd-sdk-python-0.0.3/CONTRIBUTING.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11367 2023-04-10 06:48:42.000000 etcd-sdk-python-0.0.3/LICENSE
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3552 2023-07-11 03:13:54.169890 etcd-sdk-python-0.0.3/PKG-INFO
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2911 2023-07-11 03:04:13.000000 etcd-sdk-python-0.0.3/README.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      449 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.3/docker-compose.yml
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-07-11 03:13:54.165890 etcd-sdk-python-0.0.3/docs/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      638 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/docs/Makefile
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1858 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/docs/README.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      799 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/docs/make.bat
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-07-11 03:13:54.165890 etcd-sdk-python-0.0.3/docs/source/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-07-11 03:13:54.165890 etcd-sdk-python-0.0.3/docs/source/_templates/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       98 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/docs/source/_templates/autosummaryclass.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      389 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/docs/source/_templates/layout.html
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       56 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/docs/source/authors.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3184 2023-04-10 09:41:40.000000 etcd-sdk-python-0.0.3/docs/source/conf.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       76 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/docs/source/contributing.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      237 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/docs/source/index.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      521 2023-04-10 10:04:46.000000 etcd-sdk-python-0.0.3/docs/source/install.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       52 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/docs/source/readme.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1260 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/docs/source/usage.rst
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-07-11 03:13:54.165890 etcd-sdk-python-0.0.3/etcd_sdk_python.egg-info/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3552 2023-07-11 03:13:54.000000 etcd-sdk-python-0.0.3/etcd_sdk_python.egg-info/PKG-INFO
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1336 2023-07-11 03:13:54.000000 etcd-sdk-python-0.0.3/etcd_sdk_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        1 2023-07-11 03:13:54.000000 etcd-sdk-python-0.0.3/etcd_sdk_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       54 2023-07-11 03:13:54.000000 etcd-sdk-python-0.0.3/etcd_sdk_python.egg-info/requires.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        7 2023-07-11 03:13:54.000000 etcd-sdk-python-0.0.3/etcd_sdk_python.egg-info/top_level.txt
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-07-11 03:13:54.165890 etcd-sdk-python-0.0.3/pyetcd/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      531 2023-04-11 06:17:37.000000 etcd-sdk-python-0.0.3/pyetcd/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      211 2023-06-06 09:07:20.000000 etcd-sdk-python-0.0.3/pyetcd/__version__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    48403 2023-04-25 02:57:06.000000 etcd-sdk-python-0.0.3/pyetcd/client.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-07-11 03:13:54.169890 etcd-sdk-python-0.0.3/pyetcd/etcdrpc/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       75 2023-07-11 03:10:01.000000 etcd-sdk-python-0.0.3/pyetcd/etcdrpc/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1793 2023-07-11 03:10:01.000000 etcd-sdk-python-0.0.3/pyetcd/etcdrpc/auth_pb2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1958 2023-07-11 03:10:01.000000 etcd-sdk-python-0.0.3/pyetcd/etcdrpc/auth_pb2.pyi
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1747 2023-07-11 03:10:01.000000 etcd-sdk-python-0.0.3/pyetcd/etcdrpc/kv_pb2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1714 2023-07-11 03:10:01.000000 etcd-sdk-python-0.0.3/pyetcd/etcdrpc/kv_pb2.pyi
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    28597 2023-07-11 03:10:01.000000 etcd-sdk-python-0.0.3/pyetcd/etcdrpc/rpc_pb2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    33362 2023-07-11 03:10:01.000000 etcd-sdk-python-0.0.3/pyetcd/etcdrpc/rpc_pb2.pyi
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    63388 2023-07-11 03:10:01.000000 etcd-sdk-python-0.0.3/pyetcd/etcdrpc/rpc_pb2_grpc.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1061 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/pyetcd/events.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      681 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/pyetcd/exceptions.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      858 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/pyetcd/leases.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4437 2023-04-17 12:26:35.000000 etcd-sdk-python-0.0.3/pyetcd/locks.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1503 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/pyetcd/members.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-07-11 03:13:54.169890 etcd-sdk-python-0.0.3/pyetcd/proto/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1170 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/pyetcd/proto/auth.proto
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2078 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/pyetcd/proto/kv.proto
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    29842 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/pyetcd/proto/rpc.proto
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2987 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/pyetcd/transactions.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1132 2023-04-10 09:22:28.000000 etcd-sdk-python-0.0.3/pyetcd/utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8161 2023-04-17 13:22:33.000000 etcd-sdk-python-0.0.3/pyetcd/watch.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1429 2023-07-11 03:11:08.000000 etcd-sdk-python-0.0.3/pyproject.toml
+-rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1711 2023-04-11 05:44:56.000000 etcd-sdk-python-0.0.3/python_gen.sh
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      396 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.3/requirements.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       38 2023-07-11 03:13:54.169890 etcd-sdk-python-0.0.3/setup.cfg
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-07-11 03:13:54.169890 etcd-sdk-python-0.0.3/tests/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       24 2023-04-10 08:02:48.000000 etcd-sdk-python-0.0.3/tests/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1919 2023-04-10 06:30:33.000000 etcd-sdk-python-0.0.3/tests/ca.crt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1793 2023-04-10 06:30:33.000000 etcd-sdk-python-0.0.3/tests/client.crt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3243 2023-04-10 06:30:33.000000 etcd-sdk-python-0.0.3/tests/client.key
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      755 2023-04-17 12:48:24.000000 etcd-sdk-python-0.0.3/tests/conftest.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1471 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.3/tests/test_alarms.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4199 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.3/tests/test_client.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2410 2023-04-17 12:39:05.000000 etcd-sdk-python-0.0.3/tests/test_compares.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      345 2023-04-17 12:40:16.000000 etcd-sdk-python-0.0.3/tests/test_credentials.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3828 2023-04-17 12:48:23.000000 etcd-sdk-python-0.0.3/tests/test_failover.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    37953 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.3/tests/test_pyetcd.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      599 2023-06-06 09:04:54.000000 etcd-sdk-python-0.0.3/tests/test_utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1046 2023-07-11 03:10:48.000000 etcd-sdk-python-0.0.3/tox.ini
```

### Comparing `etcd-sdk-python-0.0.2/LICENSE` & `etcd-sdk-python-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/PKG-INFO` & `etcd-sdk-python-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etcd-sdk-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python client for the etcd v3 API for python >= 3.7
 Author-email: XuanYang-cn <jumpthepig@gmail.com>
 Project-URL: Homepage, https://github.com/XuanYang-cn/pyetcd
 Project-URL: Docs: User Guide, https://pyetcd-docs.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/XuanYang-cn/pyetcd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `etcd-sdk-python-0.0.2/README.md` & `etcd-sdk-python-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/docs/Makefile` & `etcd-sdk-python-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/docs/README.md` & `etcd-sdk-python-0.0.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/docs/make.bat` & `etcd-sdk-python-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/docs/source/conf.py` & `etcd-sdk-python-0.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/docs/source/install.rst` & `etcd-sdk-python-0.0.3/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/docs/source/usage.rst` & `etcd-sdk-python-0.0.3/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/etcd_sdk_python.egg-info/PKG-INFO` & `etcd-sdk-python-0.0.3/etcd_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etcd-sdk-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python client for the etcd v3 API for python >= 3.7
 Author-email: XuanYang-cn <jumpthepig@gmail.com>
 Project-URL: Homepage, https://github.com/XuanYang-cn/pyetcd
 Project-URL: Docs: User Guide, https://pyetcd-docs.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/XuanYang-cn/pyetcd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `etcd-sdk-python-0.0.2/etcd_sdk_python.egg-info/SOURCES.txt` & `etcd-sdk-python-0.0.3/etcd_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/__init__.py` & `etcd-sdk-python-0.0.3/pyetcd/__init__.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/client.py` & `etcd-sdk-python-0.0.3/pyetcd/client.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/etcdrpc/auth_pb2.py` & `etcd-sdk-python-0.0.3/pyetcd/etcdrpc/auth_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: auth.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nauth.proto\x12\x06\x61uthpb\"5\n\x04User\x12\x0c\n\x04name\x18\x01 \x01(\x0c\x12\x10\n\x08password\x18\x02 \x01(\x0c\x12\r\n\x05roles\x18\x03 \x03(\t\"\x83\x01\n\nPermission\x12)\n\x08permType\x18\x01 \x01(\x0e\x32\x17.authpb.Permission.Type\x12\x0b\n\x03key\x18\x02 \x01(\x0c\x12\x11\n\trange_end\x18\x03 \x01(\x0c\"*\n\x04Type\x12\x08\n\x04READ\x10\x00\x12\t\n\x05WRITE\x10\x01\x12\r\n\tREADWRITE\x10\x02\"?\n\x04Role\x12\x0c\n\x04name\x18\x01 \x01(\x0c\x12)\n\rkeyPermission\x18\x02 \x03(\x0b\x32\x12.authpb.PermissionB\x15\n\x11io.etcd.jetcd.apiP\x01\x62\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'auth_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'auth_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021io.etcd.jetcd.apiP\001'
-  _USER._serialized_start=22
-  _USER._serialized_end=75
-  _PERMISSION._serialized_start=78
-  _PERMISSION._serialized_end=209
-  _PERMISSION_TYPE._serialized_start=167
-  _PERMISSION_TYPE._serialized_end=209
-  _ROLE._serialized_start=211
-  _ROLE._serialized_end=274
+  _globals['_USER']._serialized_start=22
+  _globals['_USER']._serialized_end=75
+  _globals['_PERMISSION']._serialized_start=78
+  _globals['_PERMISSION']._serialized_end=209
+  _globals['_PERMISSION_TYPE']._serialized_start=167
+  _globals['_PERMISSION_TYPE']._serialized_end=209
+  _globals['_ROLE']._serialized_start=211
+  _globals['_ROLE']._serialized_end=274
 # @@protoc_insertion_point(module_scope)
```

### Comparing `etcd-sdk-python-0.0.2/pyetcd/etcdrpc/auth_pb2.pyi` & `etcd-sdk-python-0.0.3/pyetcd/etcdrpc/auth_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,39 +2,42 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class User(_message.Message):
+    __slots__ = ["name", "password", "roles"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    ROLES_FIELD_NUMBER: _ClassVar[int]
+    name: bytes
+    password: bytes
+    roles: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, name: _Optional[bytes] = ..., password: _Optional[bytes] = ..., roles: _Optional[_Iterable[str]] = ...) -> None: ...
+
 class Permission(_message.Message):
-    __slots__ = ["key", "permType", "range_end"]
+    __slots__ = ["permType", "key", "range_end"]
     class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    PERMTYPE_FIELD_NUMBER: _ClassVar[int]
-    RANGE_END_FIELD_NUMBER: _ClassVar[int]
+        READ: _ClassVar[Permission.Type]
+        WRITE: _ClassVar[Permission.Type]
+        READWRITE: _ClassVar[Permission.Type]
     READ: Permission.Type
-    READWRITE: Permission.Type
     WRITE: Permission.Type
-    key: bytes
+    READWRITE: Permission.Type
+    PERMTYPE_FIELD_NUMBER: _ClassVar[int]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    RANGE_END_FIELD_NUMBER: _ClassVar[int]
     permType: Permission.Type
+    key: bytes
     range_end: bytes
     def __init__(self, permType: _Optional[_Union[Permission.Type, str]] = ..., key: _Optional[bytes] = ..., range_end: _Optional[bytes] = ...) -> None: ...
 
 class Role(_message.Message):
-    __slots__ = ["keyPermission", "name"]
-    KEYPERMISSION_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["name", "keyPermission"]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    keyPermission: _containers.RepeatedCompositeFieldContainer[Permission]
+    KEYPERMISSION_FIELD_NUMBER: _ClassVar[int]
     name: bytes
+    keyPermission: _containers.RepeatedCompositeFieldContainer[Permission]
     def __init__(self, name: _Optional[bytes] = ..., keyPermission: _Optional[_Iterable[_Union[Permission, _Mapping]]] = ...) -> None: ...
-
-class User(_message.Message):
-    __slots__ = ["name", "password", "roles"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PASSWORD_FIELD_NUMBER: _ClassVar[int]
-    ROLES_FIELD_NUMBER: _ClassVar[int]
-    name: bytes
-    password: bytes
-    roles: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, name: _Optional[bytes] = ..., password: _Optional[bytes] = ..., roles: _Optional[_Iterable[str]] = ...) -> None: ...
```

### Comparing `etcd-sdk-python-0.0.2/pyetcd/etcdrpc/kv_pb2.py` & `etcd-sdk-python-0.0.3/pyetcd/etcdrpc/kv_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: kv.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x08kv.proto\x12\x06mvccpb\"u\n\x08KeyValue\x12\x0b\n\x03key\x18\x01 \x01(\x0c\x12\x17\n\x0f\x63reate_revision\x18\x02 \x01(\x03\x12\x14\n\x0cmod_revision\x18\x03 \x01(\x03\x12\x0f\n\x07version\x18\x04 \x01(\x03\x12\r\n\x05value\x18\x05 \x01(\x0c\x12\r\n\x05lease\x18\x06 \x01(\x03\"\x91\x01\n\x05\x45vent\x12%\n\x04type\x18\x01 \x01(\x0e\x32\x17.mvccpb.Event.EventType\x12\x1c\n\x02kv\x18\x02 \x01(\x0b\x32\x10.mvccpb.KeyValue\x12!\n\x07prev_kv\x18\x03 \x01(\x0b\x32\x10.mvccpb.KeyValue\" \n\tEventType\x12\x07\n\x03PUT\x10\x00\x12\n\n\x06\x44\x45LETE\x10\x01\x42\x15\n\x11io.etcd.jetcd.apiP\x01\x62\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kv_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kv_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021io.etcd.jetcd.apiP\001'
-  _KEYVALUE._serialized_start=20
-  _KEYVALUE._serialized_end=137
-  _EVENT._serialized_start=140
-  _EVENT._serialized_end=285
-  _EVENT_EVENTTYPE._serialized_start=253
-  _EVENT_EVENTTYPE._serialized_end=285
+  _globals['_KEYVALUE']._serialized_start=20
+  _globals['_KEYVALUE']._serialized_end=137
+  _globals['_EVENT']._serialized_start=140
+  _globals['_EVENT']._serialized_end=285
+  _globals['_EVENT_EVENTTYPE']._serialized_start=253
+  _globals['_EVENT_EVENTTYPE']._serialized_end=285
 # @@protoc_insertion_point(module_scope)
```

### Comparing `etcd-sdk-python-0.0.2/pyetcd/etcdrpc/kv_pb2.pyi` & `etcd-sdk-python-0.0.3/pyetcd/etcdrpc/kv_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class KeyValue(_message.Message):
+    __slots__ = ["key", "create_revision", "mod_revision", "version", "value", "lease"]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    CREATE_REVISION_FIELD_NUMBER: _ClassVar[int]
+    MOD_REVISION_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    LEASE_FIELD_NUMBER: _ClassVar[int]
+    key: bytes
+    create_revision: int
+    mod_revision: int
+    version: int
+    value: bytes
+    lease: int
+    def __init__(self, key: _Optional[bytes] = ..., create_revision: _Optional[int] = ..., mod_revision: _Optional[int] = ..., version: _Optional[int] = ..., value: _Optional[bytes] = ..., lease: _Optional[int] = ...) -> None: ...
+
 class Event(_message.Message):
-    __slots__ = ["kv", "prev_kv", "type"]
+    __slots__ = ["type", "kv", "prev_kv"]
     class EventType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        PUT: _ClassVar[Event.EventType]
+        DELETE: _ClassVar[Event.EventType]
+    PUT: Event.EventType
     DELETE: Event.EventType
+    TYPE_FIELD_NUMBER: _ClassVar[int]
     KV_FIELD_NUMBER: _ClassVar[int]
     PREV_KV_FIELD_NUMBER: _ClassVar[int]
-    PUT: Event.EventType
-    TYPE_FIELD_NUMBER: _ClassVar[int]
+    type: Event.EventType
     kv: KeyValue
     prev_kv: KeyValue
-    type: Event.EventType
     def __init__(self, type: _Optional[_Union[Event.EventType, str]] = ..., kv: _Optional[_Union[KeyValue, _Mapping]] = ..., prev_kv: _Optional[_Union[KeyValue, _Mapping]] = ...) -> None: ...
-
-class KeyValue(_message.Message):
-    __slots__ = ["create_revision", "key", "lease", "mod_revision", "value", "version"]
-    CREATE_REVISION_FIELD_NUMBER: _ClassVar[int]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    LEASE_FIELD_NUMBER: _ClassVar[int]
-    MOD_REVISION_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    create_revision: int
-    key: bytes
-    lease: int
-    mod_revision: int
-    value: bytes
-    version: int
-    def __init__(self, key: _Optional[bytes] = ..., create_revision: _Optional[int] = ..., mod_revision: _Optional[int] = ..., version: _Optional[int] = ..., value: _Optional[bytes] = ..., lease: _Optional[int] = ...) -> None: ...
```

### Comparing `etcd-sdk-python-0.0.2/pyetcd/etcdrpc/rpc_pb2.py` & `etcd-sdk-python-0.0.3/pyetcd/etcdrpc/rpc_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,218 +1,219 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: rpc.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import kv_pb2 as kv__pb2
 from . import auth_pb2 as auth__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\trpc.proto\x12\x0c\x65tcdserverpb\x1a\x08kv.proto\x1a\nauth.proto\"\\\n\x0eResponseHeader\x12\x12\n\ncluster_id\x18\x01 \x01(\x04\x12\x11\n\tmember_id\x18\x02 \x01(\x04\x12\x10\n\x08revision\x18\x03 \x01(\x03\x12\x11\n\traft_term\x18\x04 \x01(\x04\"\xe4\x03\n\x0cRangeRequest\x12\x0b\n\x03key\x18\x01 \x01(\x0c\x12\x11\n\trange_end\x18\x02 \x01(\x0c\x12\r\n\x05limit\x18\x03 \x01(\x03\x12\x10\n\x08revision\x18\x04 \x01(\x03\x12\x38\n\nsort_order\x18\x05 \x01(\x0e\x32$.etcdserverpb.RangeRequest.SortOrder\x12:\n\x0bsort_target\x18\x06 \x01(\x0e\x32%.etcdserverpb.RangeRequest.SortTarget\x12\x14\n\x0cserializable\x18\x07 \x01(\x08\x12\x11\n\tkeys_only\x18\x08 \x01(\x08\x12\x12\n\ncount_only\x18\t \x01(\x08\x12\x18\n\x10min_mod_revision\x18\n \x01(\x03\x12\x18\n\x10max_mod_revision\x18\x0b \x01(\x03\x12\x1b\n\x13min_create_revision\x18\x0c \x01(\x03\x12\x1b\n\x13max_create_revision\x18\r \x01(\x03\".\n\tSortOrder\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06\x41SCEND\x10\x01\x12\x0b\n\x07\x44\x45SCEND\x10\x02\"B\n\nSortTarget\x12\x07\n\x03KEY\x10\x00\x12\x0b\n\x07VERSION\x10\x01\x12\n\n\x06\x43REATE\x10\x02\x12\x07\n\x03MOD\x10\x03\x12\t\n\x05VALUE\x10\x04\"y\n\rRangeResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\x1d\n\x03kvs\x18\x02 \x03(\x0b\x32\x10.mvccpb.KeyValue\x12\x0c\n\x04more\x18\x03 \x01(\x08\x12\r\n\x05\x63ount\x18\x04 \x01(\x03\"t\n\nPutRequest\x12\x0b\n\x03key\x18\x01 \x01(\x0c\x12\r\n\x05value\x18\x02 \x01(\x0c\x12\r\n\x05lease\x18\x03 \x01(\x03\x12\x0f\n\x07prev_kv\x18\x04 \x01(\x08\x12\x14\n\x0cignore_value\x18\x05 \x01(\x08\x12\x14\n\x0cignore_lease\x18\x06 \x01(\x08\"^\n\x0bPutResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12!\n\x07prev_kv\x18\x02 \x01(\x0b\x32\x10.mvccpb.KeyValue\"E\n\x12\x44\x65leteRangeRequest\x12\x0b\n\x03key\x18\x01 \x01(\x0c\x12\x11\n\trange_end\x18\x02 \x01(\x0c\x12\x0f\n\x07prev_kv\x18\x03 \x01(\x08\"x\n\x13\x44\x65leteRangeResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\x0f\n\x07\x64\x65leted\x18\x02 \x01(\x03\x12\"\n\x08prev_kvs\x18\x03 \x03(\x0b\x32\x10.mvccpb.KeyValue\"\xef\x01\n\tRequestOp\x12\x33\n\rrequest_range\x18\x01 \x01(\x0b\x32\x1a.etcdserverpb.RangeRequestH\x00\x12/\n\x0brequest_put\x18\x02 \x01(\x0b\x32\x18.etcdserverpb.PutRequestH\x00\x12@\n\x14request_delete_range\x18\x03 \x01(\x0b\x32 .etcdserverpb.DeleteRangeRequestH\x00\x12/\n\x0brequest_txn\x18\x04 \x01(\x0b\x32\x18.etcdserverpb.TxnRequestH\x00\x42\t\n\x07request\"\xf9\x01\n\nResponseOp\x12\x35\n\x0eresponse_range\x18\x01 \x01(\x0b\x32\x1b.etcdserverpb.RangeResponseH\x00\x12\x31\n\x0cresponse_put\x18\x02 \x01(\x0b\x32\x19.etcdserverpb.PutResponseH\x00\x12\x42\n\x15response_delete_range\x18\x03 \x01(\x0b\x32!.etcdserverpb.DeleteRangeResponseH\x00\x12\x31\n\x0cresponse_txn\x18\x04 \x01(\x0b\x32\x19.etcdserverpb.TxnResponseH\x00\x42\n\n\x08response\"\x96\x03\n\x07\x43ompare\x12\x33\n\x06result\x18\x01 \x01(\x0e\x32#.etcdserverpb.Compare.CompareResult\x12\x33\n\x06target\x18\x02 \x01(\x0e\x32#.etcdserverpb.Compare.CompareTarget\x12\x0b\n\x03key\x18\x03 \x01(\x0c\x12\x11\n\x07version\x18\x04 \x01(\x03H\x00\x12\x19\n\x0f\x63reate_revision\x18\x05 \x01(\x03H\x00\x12\x16\n\x0cmod_revision\x18\x06 \x01(\x03H\x00\x12\x0f\n\x05value\x18\x07 \x01(\x0cH\x00\x12\x0f\n\x05lease\x18\x08 \x01(\x03H\x00\x12\x11\n\trange_end\x18@ \x01(\x0c\"@\n\rCompareResult\x12\t\n\x05\x45QUAL\x10\x00\x12\x0b\n\x07GREATER\x10\x01\x12\x08\n\x04LESS\x10\x02\x12\r\n\tNOT_EQUAL\x10\x03\"G\n\rCompareTarget\x12\x0b\n\x07VERSION\x10\x00\x12\n\n\x06\x43REATE\x10\x01\x12\x07\n\x03MOD\x10\x02\x12\t\n\x05VALUE\x10\x03\x12\t\n\x05LEASE\x10\x04\x42\x0e\n\x0ctarget_union\"\x88\x01\n\nTxnRequest\x12&\n\x07\x63ompare\x18\x01 \x03(\x0b\x32\x15.etcdserverpb.Compare\x12(\n\x07success\x18\x02 \x03(\x0b\x32\x17.etcdserverpb.RequestOp\x12(\n\x07\x66\x61ilure\x18\x03 \x03(\x0b\x32\x17.etcdserverpb.RequestOp\"{\n\x0bTxnResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\x11\n\tsucceeded\x18\x02 \x01(\x08\x12+\n\tresponses\x18\x03 \x03(\x0b\x32\x18.etcdserverpb.ResponseOp\"7\n\x11\x43ompactionRequest\x12\x10\n\x08revision\x18\x01 \x01(\x03\x12\x10\n\x08physical\x18\x02 \x01(\x08\"B\n\x12\x43ompactionResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"\r\n\x0bHashRequest\"J\n\x0cHashResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\x0c\n\x04hash\x18\x02 \x01(\r\"!\n\rHashKVRequest\x12\x10\n\x08revision\x18\x01 \x01(\x03\"f\n\x0eHashKVResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\x0c\n\x04hash\x18\x02 \x01(\r\x12\x18\n\x10\x63ompact_revision\x18\x03 \x01(\x03\"\x11\n\x0fSnapshotRequest\"g\n\x10SnapshotResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\x17\n\x0fremaining_bytes\x18\x02 \x01(\x04\x12\x0c\n\x04\x62lob\x18\x03 \x01(\x0c\"\xd7\x01\n\x0cWatchRequest\x12:\n\x0e\x63reate_request\x18\x01 \x01(\x0b\x32 .etcdserverpb.WatchCreateRequestH\x00\x12:\n\x0e\x63\x61ncel_request\x18\x02 \x01(\x0b\x32 .etcdserverpb.WatchCancelRequestH\x00\x12>\n\x10progress_request\x18\x03 \x01(\x0b\x32\".etcdserverpb.WatchProgressRequestH\x00\x42\x0f\n\rrequest_union\"\xdb\x01\n\x12WatchCreateRequest\x12\x0b\n\x03key\x18\x01 \x01(\x0c\x12\x11\n\trange_end\x18\x02 \x01(\x0c\x12\x16\n\x0estart_revision\x18\x03 \x01(\x03\x12\x17\n\x0fprogress_notify\x18\x04 \x01(\x08\x12<\n\x07\x66ilters\x18\x05 \x03(\x0e\x32+.etcdserverpb.WatchCreateRequest.FilterType\x12\x0f\n\x07prev_kv\x18\x06 \x01(\x08\"%\n\nFilterType\x12\t\n\x05NOPUT\x10\x00\x12\x0c\n\x08NODELETE\x10\x01\"&\n\x12WatchCancelRequest\x12\x10\n\x08watch_id\x18\x01 \x01(\x03\"\x16\n\x14WatchProgressRequest\"\xc2\x01\n\rWatchResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\x10\n\x08watch_id\x18\x02 \x01(\x03\x12\x0f\n\x07\x63reated\x18\x03 \x01(\x08\x12\x10\n\x08\x63\x61nceled\x18\x04 \x01(\x08\x12\x18\n\x10\x63ompact_revision\x18\x05 \x01(\x03\x12\x15\n\rcancel_reason\x18\x06 \x01(\t\x12\x1d\n\x06\x65vents\x18\x0b \x03(\x0b\x32\r.mvccpb.Event\",\n\x11LeaseGrantRequest\x12\x0b\n\x03TTL\x18\x01 \x01(\x03\x12\n\n\x02ID\x18\x02 \x01(\x03\"j\n\x12LeaseGrantResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\n\n\x02ID\x18\x02 \x01(\x03\x12\x0b\n\x03TTL\x18\x03 \x01(\x03\x12\r\n\x05\x65rror\x18\x04 \x01(\t\" \n\x12LeaseRevokeRequest\x12\n\n\x02ID\x18\x01 \x01(\x03\"C\n\x13LeaseRevokeResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"#\n\x15LeaseKeepAliveRequest\x12\n\n\x02ID\x18\x01 \x01(\x03\"_\n\x16LeaseKeepAliveResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\n\n\x02ID\x18\x02 \x01(\x03\x12\x0b\n\x03TTL\x18\x03 \x01(\x03\"2\n\x16LeaseTimeToLiveRequest\x12\n\n\x02ID\x18\x01 \x01(\x03\x12\x0c\n\x04keys\x18\x02 \x01(\x08\"\x82\x01\n\x17LeaseTimeToLiveResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\n\n\x02ID\x18\x02 \x01(\x03\x12\x0b\n\x03TTL\x18\x03 \x01(\x03\x12\x12\n\ngrantedTTL\x18\x04 \x01(\x03\x12\x0c\n\x04keys\x18\x05 \x03(\x0c\"H\n\x06Member\x12\n\n\x02ID\x18\x01 \x01(\x04\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08peerURLs\x18\x03 \x03(\t\x12\x12\n\nclientURLs\x18\x04 \x03(\t\"$\n\x10MemberAddRequest\x12\x10\n\x08peerURLs\x18\x01 \x03(\t\"\x8e\x01\n\x11MemberAddResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12$\n\x06member\x18\x02 \x01(\x0b\x32\x14.etcdserverpb.Member\x12%\n\x07members\x18\x03 \x03(\x0b\x32\x14.etcdserverpb.Member\"!\n\x13MemberRemoveRequest\x12\n\n\x02ID\x18\x01 \x01(\x04\"k\n\x14MemberRemoveResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12%\n\x07members\x18\x02 \x03(\x0b\x32\x14.etcdserverpb.Member\"3\n\x13MemberUpdateRequest\x12\n\n\x02ID\x18\x01 \x01(\x04\x12\x10\n\x08peerURLs\x18\x02 \x03(\t\"k\n\x14MemberUpdateResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12%\n\x07members\x18\x02 \x03(\x0b\x32\x14.etcdserverpb.Member\"\x13\n\x11MemberListRequest\"i\n\x12MemberListResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12%\n\x07members\x18\x02 \x03(\x0b\x32\x14.etcdserverpb.Member\"\x13\n\x11\x44\x65\x66ragmentRequest\"B\n\x12\x44\x65\x66ragmentResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"%\n\x11MoveLeaderRequest\x12\x10\n\x08targetID\x18\x01 \x01(\x04\"B\n\x12MoveLeaderResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"\xb6\x01\n\x0c\x41larmRequest\x12\x36\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32&.etcdserverpb.AlarmRequest.AlarmAction\x12\x10\n\x08memberID\x18\x02 \x01(\x04\x12&\n\x05\x61larm\x18\x03 \x01(\x0e\x32\x17.etcdserverpb.AlarmType\"4\n\x0b\x41larmAction\x12\x07\n\x03GET\x10\x00\x12\x0c\n\x08\x41\x43TIVATE\x10\x01\x12\x0e\n\nDEACTIVATE\x10\x02\"G\n\x0b\x41larmMember\x12\x10\n\x08memberID\x18\x01 \x01(\x04\x12&\n\x05\x61larm\x18\x02 \x01(\x0e\x32\x17.etcdserverpb.AlarmType\"h\n\rAlarmResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12)\n\x06\x61larms\x18\x02 \x03(\x0b\x32\x19.etcdserverpb.AlarmMember\"\x0f\n\rStatusRequest\"\x94\x01\n\x0eStatusResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x62Size\x18\x03 \x01(\x03\x12\x0e\n\x06leader\x18\x04 \x01(\x04\x12\x11\n\traftIndex\x18\x05 \x01(\x04\x12\x10\n\x08raftTerm\x18\x06 \x01(\x04\"\x13\n\x11\x41uthEnableRequest\"\x14\n\x12\x41uthDisableRequest\"5\n\x13\x41uthenticateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"4\n\x12\x41uthUserAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\"\n\x12\x41uthUserGetRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"%\n\x15\x41uthUserDeleteRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"?\n\x1d\x41uthUserChangePasswordRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"6\n\x18\x41uthUserGrantRoleRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04role\x18\x02 \x01(\t\"7\n\x19\x41uthUserRevokeRoleRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04role\x18\x02 \x01(\t\"\"\n\x12\x41uthRoleAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\"\n\x12\x41uthRoleGetRequest\x12\x0c\n\x04role\x18\x01 \x01(\t\"\x15\n\x13\x41uthUserListRequest\"\x15\n\x13\x41uthRoleListRequest\"%\n\x15\x41uthRoleDeleteRequest\x12\x0c\n\x04role\x18\x01 \x01(\t\"P\n\x1e\x41uthRoleGrantPermissionRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12 \n\x04perm\x18\x02 \x01(\x0b\x32\x12.authpb.Permission\"O\n\x1f\x41uthRoleRevokePermissionRequest\x12\x0c\n\x04role\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x11\n\trange_end\x18\x03 \x01(\t\"B\n\x12\x41uthEnableResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"C\n\x13\x41uthDisableResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"S\n\x14\x41uthenticateResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\r\n\x05token\x18\x02 \x01(\t\"C\n\x13\x41uthUserAddResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"R\n\x13\x41uthUserGetResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\r\n\x05roles\x18\x02 \x03(\t\"F\n\x16\x41uthUserDeleteResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"N\n\x1e\x41uthUserChangePasswordResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"I\n\x19\x41uthUserGrantRoleResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"J\n\x1a\x41uthUserRevokeRoleResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"C\n\x13\x41uthRoleAddResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"e\n\x13\x41uthRoleGetResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12 \n\x04perm\x18\x02 \x03(\x0b\x32\x12.authpb.Permission\"S\n\x14\x41uthRoleListResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\r\n\x05roles\x18\x02 \x03(\t\"S\n\x14\x41uthUserListResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\x12\r\n\x05users\x18\x02 \x03(\t\"F\n\x16\x41uthRoleDeleteResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"O\n\x1f\x41uthRoleGrantPermissionResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader\"P\n AuthRoleRevokePermissionResponse\x12,\n\x06header\x18\x01 \x01(\x0b\x32\x1c.etcdserverpb.ResponseHeader*\"\n\tAlarmType\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07NOSPACE\x10\x01\x32\xea\x02\n\x02KV\x12\x42\n\x05Range\x12\x1a.etcdserverpb.RangeRequest\x1a\x1b.etcdserverpb.RangeResponse\"\x00\x12<\n\x03Put\x12\x18.etcdserverpb.PutRequest\x1a\x19.etcdserverpb.PutResponse\"\x00\x12T\n\x0b\x44\x65leteRange\x12 .etcdserverpb.DeleteRangeRequest\x1a!.etcdserverpb.DeleteRangeResponse\"\x00\x12<\n\x03Txn\x12\x18.etcdserverpb.TxnRequest\x1a\x19.etcdserverpb.TxnResponse\"\x00\x12N\n\x07\x43ompact\x12\x1f.etcdserverpb.CompactionRequest\x1a .etcdserverpb.CompactionResponse\"\x00\x32\x9e\x01\n\x05Watch\x12M\n\x08Progress\x12\".etcdserverpb.WatchProgressRequest\x1a\x1b.etcdserverpb.WatchResponse\"\x00\x12\x46\n\x05Watch\x12\x1a.etcdserverpb.WatchRequest\x1a\x1b.etcdserverpb.WatchResponse\"\x00(\x01\x30\x01\x32\xf5\x02\n\x05Lease\x12Q\n\nLeaseGrant\x12\x1f.etcdserverpb.LeaseGrantRequest\x1a .etcdserverpb.LeaseGrantResponse\"\x00\x12T\n\x0bLeaseRevoke\x12 .etcdserverpb.LeaseRevokeRequest\x1a!.etcdserverpb.LeaseRevokeResponse\"\x00\x12\x61\n\x0eLeaseKeepAlive\x12#.etcdserverpb.LeaseKeepAliveRequest\x1a$.etcdserverpb.LeaseKeepAliveResponse\"\x00(\x01\x30\x01\x12`\n\x0fLeaseTimeToLive\x12$.etcdserverpb.LeaseTimeToLiveRequest\x1a%.etcdserverpb.LeaseTimeToLiveResponse\"\x00\x32\xde\x02\n\x07\x43luster\x12N\n\tMemberAdd\x12\x1e.etcdserverpb.MemberAddRequest\x1a\x1f.etcdserverpb.MemberAddResponse\"\x00\x12W\n\x0cMemberRemove\x12!.etcdserverpb.MemberRemoveRequest\x1a\".etcdserverpb.MemberRemoveResponse\"\x00\x12W\n\x0cMemberUpdate\x12!.etcdserverpb.MemberUpdateRequest\x1a\".etcdserverpb.MemberUpdateResponse\"\x00\x12Q\n\nMemberList\x12\x1f.etcdserverpb.MemberListRequest\x1a .etcdserverpb.MemberListResponse\"\x00\x32\x95\x04\n\x0bMaintenance\x12\x42\n\x05\x41larm\x12\x1a.etcdserverpb.AlarmRequest\x1a\x1b.etcdserverpb.AlarmResponse\"\x00\x12\x45\n\x06Status\x12\x1b.etcdserverpb.StatusRequest\x1a\x1c.etcdserverpb.StatusResponse\"\x00\x12Q\n\nDefragment\x12\x1f.etcdserverpb.DefragmentRequest\x1a .etcdserverpb.DefragmentResponse\"\x00\x12?\n\x04Hash\x12\x19.etcdserverpb.HashRequest\x1a\x1a.etcdserverpb.HashResponse\"\x00\x12\x45\n\x06HashKV\x12\x1b.etcdserverpb.HashKVRequest\x1a\x1c.etcdserverpb.HashKVResponse\"\x00\x12M\n\x08Snapshot\x12\x1d.etcdserverpb.SnapshotRequest\x1a\x1e.etcdserverpb.SnapshotResponse\"\x00\x30\x01\x12Q\n\nMoveLeader\x12\x1f.etcdserverpb.MoveLeaderRequest\x1a .etcdserverpb.MoveLeaderResponse\"\x00\x32\xdd\x0b\n\x04\x41uth\x12Q\n\nAuthEnable\x12\x1f.etcdserverpb.AuthEnableRequest\x1a .etcdserverpb.AuthEnableResponse\"\x00\x12T\n\x0b\x41uthDisable\x12 .etcdserverpb.AuthDisableRequest\x1a!.etcdserverpb.AuthDisableResponse\"\x00\x12W\n\x0c\x41uthenticate\x12!.etcdserverpb.AuthenticateRequest\x1a\".etcdserverpb.AuthenticateResponse\"\x00\x12P\n\x07UserAdd\x12 .etcdserverpb.AuthUserAddRequest\x1a!.etcdserverpb.AuthUserAddResponse\"\x00\x12P\n\x07UserGet\x12 .etcdserverpb.AuthUserGetRequest\x1a!.etcdserverpb.AuthUserGetResponse\"\x00\x12S\n\x08UserList\x12!.etcdserverpb.AuthUserListRequest\x1a\".etcdserverpb.AuthUserListResponse\"\x00\x12Y\n\nUserDelete\x12#.etcdserverpb.AuthUserDeleteRequest\x1a$.etcdserverpb.AuthUserDeleteResponse\"\x00\x12q\n\x12UserChangePassword\x12+.etcdserverpb.AuthUserChangePasswordRequest\x1a,.etcdserverpb.AuthUserChangePasswordResponse\"\x00\x12\x62\n\rUserGrantRole\x12&.etcdserverpb.AuthUserGrantRoleRequest\x1a\'.etcdserverpb.AuthUserGrantRoleResponse\"\x00\x12\x65\n\x0eUserRevokeRole\x12\'.etcdserverpb.AuthUserRevokeRoleRequest\x1a(.etcdserverpb.AuthUserRevokeRoleResponse\"\x00\x12P\n\x07RoleAdd\x12 .etcdserverpb.AuthRoleAddRequest\x1a!.etcdserverpb.AuthRoleAddResponse\"\x00\x12P\n\x07RoleGet\x12 .etcdserverpb.AuthRoleGetRequest\x1a!.etcdserverpb.AuthRoleGetResponse\"\x00\x12S\n\x08RoleList\x12!.etcdserverpb.AuthRoleListRequest\x1a\".etcdserverpb.AuthRoleListResponse\"\x00\x12Y\n\nRoleDelete\x12#.etcdserverpb.AuthRoleDeleteRequest\x1a$.etcdserverpb.AuthRoleDeleteResponse\"\x00\x12t\n\x13RoleGrantPermission\x12,.etcdserverpb.AuthRoleGrantPermissionRequest\x1a-.etcdserverpb.AuthRoleGrantPermissionResponse\"\x00\x12w\n\x14RoleRevokePermission\x12-.etcdserverpb.AuthRoleRevokePermissionRequest\x1a..etcdserverpb.AuthRoleRevokePermissionResponse\"\x00\x42)\n\x11io.etcd.jetcd.apiB\nJetcdProtoP\x01\xa2\x02\x05Jetcdb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rpc_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rpc_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021io.etcd.jetcd.apiB\nJetcdProtoP\001\242\002\005Jetcd'
-  _ALARMTYPE._serialized_start=7482
-  _ALARMTYPE._serialized_end=7516
-  _RESPONSEHEADER._serialized_start=49
-  _RESPONSEHEADER._serialized_end=141
-  _RANGEREQUEST._serialized_start=144
-  _RANGEREQUEST._serialized_end=628
-  _RANGEREQUEST_SORTORDER._serialized_start=514
-  _RANGEREQUEST_SORTORDER._serialized_end=560
-  _RANGEREQUEST_SORTTARGET._serialized_start=562
-  _RANGEREQUEST_SORTTARGET._serialized_end=628
-  _RANGERESPONSE._serialized_start=630
-  _RANGERESPONSE._serialized_end=751
-  _PUTREQUEST._serialized_start=753
-  _PUTREQUEST._serialized_end=869
-  _PUTRESPONSE._serialized_start=871
-  _PUTRESPONSE._serialized_end=965
-  _DELETERANGEREQUEST._serialized_start=967
-  _DELETERANGEREQUEST._serialized_end=1036
-  _DELETERANGERESPONSE._serialized_start=1038
-  _DELETERANGERESPONSE._serialized_end=1158
-  _REQUESTOP._serialized_start=1161
-  _REQUESTOP._serialized_end=1400
-  _RESPONSEOP._serialized_start=1403
-  _RESPONSEOP._serialized_end=1652
-  _COMPARE._serialized_start=1655
-  _COMPARE._serialized_end=2061
-  _COMPARE_COMPARERESULT._serialized_start=1908
-  _COMPARE_COMPARERESULT._serialized_end=1972
-  _COMPARE_COMPARETARGET._serialized_start=1974
-  _COMPARE_COMPARETARGET._serialized_end=2045
-  _TXNREQUEST._serialized_start=2064
-  _TXNREQUEST._serialized_end=2200
-  _TXNRESPONSE._serialized_start=2202
-  _TXNRESPONSE._serialized_end=2325
-  _COMPACTIONREQUEST._serialized_start=2327
-  _COMPACTIONREQUEST._serialized_end=2382
-  _COMPACTIONRESPONSE._serialized_start=2384
-  _COMPACTIONRESPONSE._serialized_end=2450
-  _HASHREQUEST._serialized_start=2452
-  _HASHREQUEST._serialized_end=2465
-  _HASHRESPONSE._serialized_start=2467
-  _HASHRESPONSE._serialized_end=2541
-  _HASHKVREQUEST._serialized_start=2543
-  _HASHKVREQUEST._serialized_end=2576
-  _HASHKVRESPONSE._serialized_start=2578
-  _HASHKVRESPONSE._serialized_end=2680
-  _SNAPSHOTREQUEST._serialized_start=2682
-  _SNAPSHOTREQUEST._serialized_end=2699
-  _SNAPSHOTRESPONSE._serialized_start=2701
-  _SNAPSHOTRESPONSE._serialized_end=2804
-  _WATCHREQUEST._serialized_start=2807
-  _WATCHREQUEST._serialized_end=3022
-  _WATCHCREATEREQUEST._serialized_start=3025
-  _WATCHCREATEREQUEST._serialized_end=3244
-  _WATCHCREATEREQUEST_FILTERTYPE._serialized_start=3207
-  _WATCHCREATEREQUEST_FILTERTYPE._serialized_end=3244
-  _WATCHCANCELREQUEST._serialized_start=3246
-  _WATCHCANCELREQUEST._serialized_end=3284
-  _WATCHPROGRESSREQUEST._serialized_start=3286
-  _WATCHPROGRESSREQUEST._serialized_end=3308
-  _WATCHRESPONSE._serialized_start=3311
-  _WATCHRESPONSE._serialized_end=3505
-  _LEASEGRANTREQUEST._serialized_start=3507
-  _LEASEGRANTREQUEST._serialized_end=3551
-  _LEASEGRANTRESPONSE._serialized_start=3553
-  _LEASEGRANTRESPONSE._serialized_end=3659
-  _LEASEREVOKEREQUEST._serialized_start=3661
-  _LEASEREVOKEREQUEST._serialized_end=3693
-  _LEASEREVOKERESPONSE._serialized_start=3695
-  _LEASEREVOKERESPONSE._serialized_end=3762
-  _LEASEKEEPALIVEREQUEST._serialized_start=3764
-  _LEASEKEEPALIVEREQUEST._serialized_end=3799
-  _LEASEKEEPALIVERESPONSE._serialized_start=3801
-  _LEASEKEEPALIVERESPONSE._serialized_end=3896
-  _LEASETIMETOLIVEREQUEST._serialized_start=3898
-  _LEASETIMETOLIVEREQUEST._serialized_end=3948
-  _LEASETIMETOLIVERESPONSE._serialized_start=3951
-  _LEASETIMETOLIVERESPONSE._serialized_end=4081
-  _MEMBER._serialized_start=4083
-  _MEMBER._serialized_end=4155
-  _MEMBERADDREQUEST._serialized_start=4157
-  _MEMBERADDREQUEST._serialized_end=4193
-  _MEMBERADDRESPONSE._serialized_start=4196
-  _MEMBERADDRESPONSE._serialized_end=4338
-  _MEMBERREMOVEREQUEST._serialized_start=4340
-  _MEMBERREMOVEREQUEST._serialized_end=4373
-  _MEMBERREMOVERESPONSE._serialized_start=4375
-  _MEMBERREMOVERESPONSE._serialized_end=4482
-  _MEMBERUPDATEREQUEST._serialized_start=4484
-  _MEMBERUPDATEREQUEST._serialized_end=4535
-  _MEMBERUPDATERESPONSE._serialized_start=4537
-  _MEMBERUPDATERESPONSE._serialized_end=4644
-  _MEMBERLISTREQUEST._serialized_start=4646
-  _MEMBERLISTREQUEST._serialized_end=4665
-  _MEMBERLISTRESPONSE._serialized_start=4667
-  _MEMBERLISTRESPONSE._serialized_end=4772
-  _DEFRAGMENTREQUEST._serialized_start=4774
-  _DEFRAGMENTREQUEST._serialized_end=4793
-  _DEFRAGMENTRESPONSE._serialized_start=4795
-  _DEFRAGMENTRESPONSE._serialized_end=4861
-  _MOVELEADERREQUEST._serialized_start=4863
-  _MOVELEADERREQUEST._serialized_end=4900
-  _MOVELEADERRESPONSE._serialized_start=4902
-  _MOVELEADERRESPONSE._serialized_end=4968
-  _ALARMREQUEST._serialized_start=4971
-  _ALARMREQUEST._serialized_end=5153
-  _ALARMREQUEST_ALARMACTION._serialized_start=5101
-  _ALARMREQUEST_ALARMACTION._serialized_end=5153
-  _ALARMMEMBER._serialized_start=5155
-  _ALARMMEMBER._serialized_end=5226
-  _ALARMRESPONSE._serialized_start=5228
-  _ALARMRESPONSE._serialized_end=5332
-  _STATUSREQUEST._serialized_start=5334
-  _STATUSREQUEST._serialized_end=5349
-  _STATUSRESPONSE._serialized_start=5352
-  _STATUSRESPONSE._serialized_end=5500
-  _AUTHENABLEREQUEST._serialized_start=5502
-  _AUTHENABLEREQUEST._serialized_end=5521
-  _AUTHDISABLEREQUEST._serialized_start=5523
-  _AUTHDISABLEREQUEST._serialized_end=5543
-  _AUTHENTICATEREQUEST._serialized_start=5545
-  _AUTHENTICATEREQUEST._serialized_end=5598
-  _AUTHUSERADDREQUEST._serialized_start=5600
-  _AUTHUSERADDREQUEST._serialized_end=5652
-  _AUTHUSERGETREQUEST._serialized_start=5654
-  _AUTHUSERGETREQUEST._serialized_end=5688
-  _AUTHUSERDELETEREQUEST._serialized_start=5690
-  _AUTHUSERDELETEREQUEST._serialized_end=5727
-  _AUTHUSERCHANGEPASSWORDREQUEST._serialized_start=5729
-  _AUTHUSERCHANGEPASSWORDREQUEST._serialized_end=5792
-  _AUTHUSERGRANTROLEREQUEST._serialized_start=5794
-  _AUTHUSERGRANTROLEREQUEST._serialized_end=5848
-  _AUTHUSERREVOKEROLEREQUEST._serialized_start=5850
-  _AUTHUSERREVOKEROLEREQUEST._serialized_end=5905
-  _AUTHROLEADDREQUEST._serialized_start=5907
-  _AUTHROLEADDREQUEST._serialized_end=5941
-  _AUTHROLEGETREQUEST._serialized_start=5943
-  _AUTHROLEGETREQUEST._serialized_end=5977
-  _AUTHUSERLISTREQUEST._serialized_start=5979
-  _AUTHUSERLISTREQUEST._serialized_end=6000
-  _AUTHROLELISTREQUEST._serialized_start=6002
-  _AUTHROLELISTREQUEST._serialized_end=6023
-  _AUTHROLEDELETEREQUEST._serialized_start=6025
-  _AUTHROLEDELETEREQUEST._serialized_end=6062
-  _AUTHROLEGRANTPERMISSIONREQUEST._serialized_start=6064
-  _AUTHROLEGRANTPERMISSIONREQUEST._serialized_end=6144
-  _AUTHROLEREVOKEPERMISSIONREQUEST._serialized_start=6146
-  _AUTHROLEREVOKEPERMISSIONREQUEST._serialized_end=6225
-  _AUTHENABLERESPONSE._serialized_start=6227
-  _AUTHENABLERESPONSE._serialized_end=6293
-  _AUTHDISABLERESPONSE._serialized_start=6295
-  _AUTHDISABLERESPONSE._serialized_end=6362
-  _AUTHENTICATERESPONSE._serialized_start=6364
-  _AUTHENTICATERESPONSE._serialized_end=6447
-  _AUTHUSERADDRESPONSE._serialized_start=6449
-  _AUTHUSERADDRESPONSE._serialized_end=6516
-  _AUTHUSERGETRESPONSE._serialized_start=6518
-  _AUTHUSERGETRESPONSE._serialized_end=6600
-  _AUTHUSERDELETERESPONSE._serialized_start=6602
-  _AUTHUSERDELETERESPONSE._serialized_end=6672
-  _AUTHUSERCHANGEPASSWORDRESPONSE._serialized_start=6674
-  _AUTHUSERCHANGEPASSWORDRESPONSE._serialized_end=6752
-  _AUTHUSERGRANTROLERESPONSE._serialized_start=6754
-  _AUTHUSERGRANTROLERESPONSE._serialized_end=6827
-  _AUTHUSERREVOKEROLERESPONSE._serialized_start=6829
-  _AUTHUSERREVOKEROLERESPONSE._serialized_end=6903
-  _AUTHROLEADDRESPONSE._serialized_start=6905
-  _AUTHROLEADDRESPONSE._serialized_end=6972
-  _AUTHROLEGETRESPONSE._serialized_start=6974
-  _AUTHROLEGETRESPONSE._serialized_end=7075
-  _AUTHROLELISTRESPONSE._serialized_start=7077
-  _AUTHROLELISTRESPONSE._serialized_end=7160
-  _AUTHUSERLISTRESPONSE._serialized_start=7162
-  _AUTHUSERLISTRESPONSE._serialized_end=7245
-  _AUTHROLEDELETERESPONSE._serialized_start=7247
-  _AUTHROLEDELETERESPONSE._serialized_end=7317
-  _AUTHROLEGRANTPERMISSIONRESPONSE._serialized_start=7319
-  _AUTHROLEGRANTPERMISSIONRESPONSE._serialized_end=7398
-  _AUTHROLEREVOKEPERMISSIONRESPONSE._serialized_start=7400
-  _AUTHROLEREVOKEPERMISSIONRESPONSE._serialized_end=7480
-  _KV._serialized_start=7519
-  _KV._serialized_end=7881
-  _WATCH._serialized_start=7884
-  _WATCH._serialized_end=8042
-  _LEASE._serialized_start=8045
-  _LEASE._serialized_end=8418
-  _CLUSTER._serialized_start=8421
-  _CLUSTER._serialized_end=8771
-  _MAINTENANCE._serialized_start=8774
-  _MAINTENANCE._serialized_end=9307
-  _AUTH._serialized_start=9310
-  _AUTH._serialized_end=10811
+  _globals['_ALARMTYPE']._serialized_start=7482
+  _globals['_ALARMTYPE']._serialized_end=7516
+  _globals['_RESPONSEHEADER']._serialized_start=49
+  _globals['_RESPONSEHEADER']._serialized_end=141
+  _globals['_RANGEREQUEST']._serialized_start=144
+  _globals['_RANGEREQUEST']._serialized_end=628
+  _globals['_RANGEREQUEST_SORTORDER']._serialized_start=514
+  _globals['_RANGEREQUEST_SORTORDER']._serialized_end=560
+  _globals['_RANGEREQUEST_SORTTARGET']._serialized_start=562
+  _globals['_RANGEREQUEST_SORTTARGET']._serialized_end=628
+  _globals['_RANGERESPONSE']._serialized_start=630
+  _globals['_RANGERESPONSE']._serialized_end=751
+  _globals['_PUTREQUEST']._serialized_start=753
+  _globals['_PUTREQUEST']._serialized_end=869
+  _globals['_PUTRESPONSE']._serialized_start=871
+  _globals['_PUTRESPONSE']._serialized_end=965
+  _globals['_DELETERANGEREQUEST']._serialized_start=967
+  _globals['_DELETERANGEREQUEST']._serialized_end=1036
+  _globals['_DELETERANGERESPONSE']._serialized_start=1038
+  _globals['_DELETERANGERESPONSE']._serialized_end=1158
+  _globals['_REQUESTOP']._serialized_start=1161
+  _globals['_REQUESTOP']._serialized_end=1400
+  _globals['_RESPONSEOP']._serialized_start=1403
+  _globals['_RESPONSEOP']._serialized_end=1652
+  _globals['_COMPARE']._serialized_start=1655
+  _globals['_COMPARE']._serialized_end=2061
+  _globals['_COMPARE_COMPARERESULT']._serialized_start=1908
+  _globals['_COMPARE_COMPARERESULT']._serialized_end=1972
+  _globals['_COMPARE_COMPARETARGET']._serialized_start=1974
+  _globals['_COMPARE_COMPARETARGET']._serialized_end=2045
+  _globals['_TXNREQUEST']._serialized_start=2064
+  _globals['_TXNREQUEST']._serialized_end=2200
+  _globals['_TXNRESPONSE']._serialized_start=2202
+  _globals['_TXNRESPONSE']._serialized_end=2325
+  _globals['_COMPACTIONREQUEST']._serialized_start=2327
+  _globals['_COMPACTIONREQUEST']._serialized_end=2382
+  _globals['_COMPACTIONRESPONSE']._serialized_start=2384
+  _globals['_COMPACTIONRESPONSE']._serialized_end=2450
+  _globals['_HASHREQUEST']._serialized_start=2452
+  _globals['_HASHREQUEST']._serialized_end=2465
+  _globals['_HASHRESPONSE']._serialized_start=2467
+  _globals['_HASHRESPONSE']._serialized_end=2541
+  _globals['_HASHKVREQUEST']._serialized_start=2543
+  _globals['_HASHKVREQUEST']._serialized_end=2576
+  _globals['_HASHKVRESPONSE']._serialized_start=2578
+  _globals['_HASHKVRESPONSE']._serialized_end=2680
+  _globals['_SNAPSHOTREQUEST']._serialized_start=2682
+  _globals['_SNAPSHOTREQUEST']._serialized_end=2699
+  _globals['_SNAPSHOTRESPONSE']._serialized_start=2701
+  _globals['_SNAPSHOTRESPONSE']._serialized_end=2804
+  _globals['_WATCHREQUEST']._serialized_start=2807
+  _globals['_WATCHREQUEST']._serialized_end=3022
+  _globals['_WATCHCREATEREQUEST']._serialized_start=3025
+  _globals['_WATCHCREATEREQUEST']._serialized_end=3244
+  _globals['_WATCHCREATEREQUEST_FILTERTYPE']._serialized_start=3207
+  _globals['_WATCHCREATEREQUEST_FILTERTYPE']._serialized_end=3244
+  _globals['_WATCHCANCELREQUEST']._serialized_start=3246
+  _globals['_WATCHCANCELREQUEST']._serialized_end=3284
+  _globals['_WATCHPROGRESSREQUEST']._serialized_start=3286
+  _globals['_WATCHPROGRESSREQUEST']._serialized_end=3308
+  _globals['_WATCHRESPONSE']._serialized_start=3311
+  _globals['_WATCHRESPONSE']._serialized_end=3505
+  _globals['_LEASEGRANTREQUEST']._serialized_start=3507
+  _globals['_LEASEGRANTREQUEST']._serialized_end=3551
+  _globals['_LEASEGRANTRESPONSE']._serialized_start=3553
+  _globals['_LEASEGRANTRESPONSE']._serialized_end=3659
+  _globals['_LEASEREVOKEREQUEST']._serialized_start=3661
+  _globals['_LEASEREVOKEREQUEST']._serialized_end=3693
+  _globals['_LEASEREVOKERESPONSE']._serialized_start=3695
+  _globals['_LEASEREVOKERESPONSE']._serialized_end=3762
+  _globals['_LEASEKEEPALIVEREQUEST']._serialized_start=3764
+  _globals['_LEASEKEEPALIVEREQUEST']._serialized_end=3799
+  _globals['_LEASEKEEPALIVERESPONSE']._serialized_start=3801
+  _globals['_LEASEKEEPALIVERESPONSE']._serialized_end=3896
+  _globals['_LEASETIMETOLIVEREQUEST']._serialized_start=3898
+  _globals['_LEASETIMETOLIVEREQUEST']._serialized_end=3948
+  _globals['_LEASETIMETOLIVERESPONSE']._serialized_start=3951
+  _globals['_LEASETIMETOLIVERESPONSE']._serialized_end=4081
+  _globals['_MEMBER']._serialized_start=4083
+  _globals['_MEMBER']._serialized_end=4155
+  _globals['_MEMBERADDREQUEST']._serialized_start=4157
+  _globals['_MEMBERADDREQUEST']._serialized_end=4193
+  _globals['_MEMBERADDRESPONSE']._serialized_start=4196
+  _globals['_MEMBERADDRESPONSE']._serialized_end=4338
+  _globals['_MEMBERREMOVEREQUEST']._serialized_start=4340
+  _globals['_MEMBERREMOVEREQUEST']._serialized_end=4373
+  _globals['_MEMBERREMOVERESPONSE']._serialized_start=4375
+  _globals['_MEMBERREMOVERESPONSE']._serialized_end=4482
+  _globals['_MEMBERUPDATEREQUEST']._serialized_start=4484
+  _globals['_MEMBERUPDATEREQUEST']._serialized_end=4535
+  _globals['_MEMBERUPDATERESPONSE']._serialized_start=4537
+  _globals['_MEMBERUPDATERESPONSE']._serialized_end=4644
+  _globals['_MEMBERLISTREQUEST']._serialized_start=4646
+  _globals['_MEMBERLISTREQUEST']._serialized_end=4665
+  _globals['_MEMBERLISTRESPONSE']._serialized_start=4667
+  _globals['_MEMBERLISTRESPONSE']._serialized_end=4772
+  _globals['_DEFRAGMENTREQUEST']._serialized_start=4774
+  _globals['_DEFRAGMENTREQUEST']._serialized_end=4793
+  _globals['_DEFRAGMENTRESPONSE']._serialized_start=4795
+  _globals['_DEFRAGMENTRESPONSE']._serialized_end=4861
+  _globals['_MOVELEADERREQUEST']._serialized_start=4863
+  _globals['_MOVELEADERREQUEST']._serialized_end=4900
+  _globals['_MOVELEADERRESPONSE']._serialized_start=4902
+  _globals['_MOVELEADERRESPONSE']._serialized_end=4968
+  _globals['_ALARMREQUEST']._serialized_start=4971
+  _globals['_ALARMREQUEST']._serialized_end=5153
+  _globals['_ALARMREQUEST_ALARMACTION']._serialized_start=5101
+  _globals['_ALARMREQUEST_ALARMACTION']._serialized_end=5153
+  _globals['_ALARMMEMBER']._serialized_start=5155
+  _globals['_ALARMMEMBER']._serialized_end=5226
+  _globals['_ALARMRESPONSE']._serialized_start=5228
+  _globals['_ALARMRESPONSE']._serialized_end=5332
+  _globals['_STATUSREQUEST']._serialized_start=5334
+  _globals['_STATUSREQUEST']._serialized_end=5349
+  _globals['_STATUSRESPONSE']._serialized_start=5352
+  _globals['_STATUSRESPONSE']._serialized_end=5500
+  _globals['_AUTHENABLEREQUEST']._serialized_start=5502
+  _globals['_AUTHENABLEREQUEST']._serialized_end=5521
+  _globals['_AUTHDISABLEREQUEST']._serialized_start=5523
+  _globals['_AUTHDISABLEREQUEST']._serialized_end=5543
+  _globals['_AUTHENTICATEREQUEST']._serialized_start=5545
+  _globals['_AUTHENTICATEREQUEST']._serialized_end=5598
+  _globals['_AUTHUSERADDREQUEST']._serialized_start=5600
+  _globals['_AUTHUSERADDREQUEST']._serialized_end=5652
+  _globals['_AUTHUSERGETREQUEST']._serialized_start=5654
+  _globals['_AUTHUSERGETREQUEST']._serialized_end=5688
+  _globals['_AUTHUSERDELETEREQUEST']._serialized_start=5690
+  _globals['_AUTHUSERDELETEREQUEST']._serialized_end=5727
+  _globals['_AUTHUSERCHANGEPASSWORDREQUEST']._serialized_start=5729
+  _globals['_AUTHUSERCHANGEPASSWORDREQUEST']._serialized_end=5792
+  _globals['_AUTHUSERGRANTROLEREQUEST']._serialized_start=5794
+  _globals['_AUTHUSERGRANTROLEREQUEST']._serialized_end=5848
+  _globals['_AUTHUSERREVOKEROLEREQUEST']._serialized_start=5850
+  _globals['_AUTHUSERREVOKEROLEREQUEST']._serialized_end=5905
+  _globals['_AUTHROLEADDREQUEST']._serialized_start=5907
+  _globals['_AUTHROLEADDREQUEST']._serialized_end=5941
+  _globals['_AUTHROLEGETREQUEST']._serialized_start=5943
+  _globals['_AUTHROLEGETREQUEST']._serialized_end=5977
+  _globals['_AUTHUSERLISTREQUEST']._serialized_start=5979
+  _globals['_AUTHUSERLISTREQUEST']._serialized_end=6000
+  _globals['_AUTHROLELISTREQUEST']._serialized_start=6002
+  _globals['_AUTHROLELISTREQUEST']._serialized_end=6023
+  _globals['_AUTHROLEDELETEREQUEST']._serialized_start=6025
+  _globals['_AUTHROLEDELETEREQUEST']._serialized_end=6062
+  _globals['_AUTHROLEGRANTPERMISSIONREQUEST']._serialized_start=6064
+  _globals['_AUTHROLEGRANTPERMISSIONREQUEST']._serialized_end=6144
+  _globals['_AUTHROLEREVOKEPERMISSIONREQUEST']._serialized_start=6146
+  _globals['_AUTHROLEREVOKEPERMISSIONREQUEST']._serialized_end=6225
+  _globals['_AUTHENABLERESPONSE']._serialized_start=6227
+  _globals['_AUTHENABLERESPONSE']._serialized_end=6293
+  _globals['_AUTHDISABLERESPONSE']._serialized_start=6295
+  _globals['_AUTHDISABLERESPONSE']._serialized_end=6362
+  _globals['_AUTHENTICATERESPONSE']._serialized_start=6364
+  _globals['_AUTHENTICATERESPONSE']._serialized_end=6447
+  _globals['_AUTHUSERADDRESPONSE']._serialized_start=6449
+  _globals['_AUTHUSERADDRESPONSE']._serialized_end=6516
+  _globals['_AUTHUSERGETRESPONSE']._serialized_start=6518
+  _globals['_AUTHUSERGETRESPONSE']._serialized_end=6600
+  _globals['_AUTHUSERDELETERESPONSE']._serialized_start=6602
+  _globals['_AUTHUSERDELETERESPONSE']._serialized_end=6672
+  _globals['_AUTHUSERCHANGEPASSWORDRESPONSE']._serialized_start=6674
+  _globals['_AUTHUSERCHANGEPASSWORDRESPONSE']._serialized_end=6752
+  _globals['_AUTHUSERGRANTROLERESPONSE']._serialized_start=6754
+  _globals['_AUTHUSERGRANTROLERESPONSE']._serialized_end=6827
+  _globals['_AUTHUSERREVOKEROLERESPONSE']._serialized_start=6829
+  _globals['_AUTHUSERREVOKEROLERESPONSE']._serialized_end=6903
+  _globals['_AUTHROLEADDRESPONSE']._serialized_start=6905
+  _globals['_AUTHROLEADDRESPONSE']._serialized_end=6972
+  _globals['_AUTHROLEGETRESPONSE']._serialized_start=6974
+  _globals['_AUTHROLEGETRESPONSE']._serialized_end=7075
+  _globals['_AUTHROLELISTRESPONSE']._serialized_start=7077
+  _globals['_AUTHROLELISTRESPONSE']._serialized_end=7160
+  _globals['_AUTHUSERLISTRESPONSE']._serialized_start=7162
+  _globals['_AUTHUSERLISTRESPONSE']._serialized_end=7245
+  _globals['_AUTHROLEDELETERESPONSE']._serialized_start=7247
+  _globals['_AUTHROLEDELETERESPONSE']._serialized_end=7317
+  _globals['_AUTHROLEGRANTPERMISSIONRESPONSE']._serialized_start=7319
+  _globals['_AUTHROLEGRANTPERMISSIONRESPONSE']._serialized_end=7398
+  _globals['_AUTHROLEREVOKEPERMISSIONRESPONSE']._serialized_start=7400
+  _globals['_AUTHROLEREVOKEPERMISSIONRESPONSE']._serialized_end=7480
+  _globals['_KV']._serialized_start=7519
+  _globals['_KV']._serialized_end=7881
+  _globals['_WATCH']._serialized_start=7884
+  _globals['_WATCH']._serialized_end=8042
+  _globals['_LEASE']._serialized_start=8045
+  _globals['_LEASE']._serialized_end=8418
+  _globals['_CLUSTER']._serialized_start=8421
+  _globals['_CLUSTER']._serialized_end=8771
+  _globals['_MAINTENANCE']._serialized_start=8774
+  _globals['_MAINTENANCE']._serialized_end=9307
+  _globals['_AUTH']._serialized_start=9310
+  _globals['_AUTH']._serialized_end=10811
 # @@protoc_insertion_point(module_scope)
```

### Comparing `etcd-sdk-python-0.0.2/pyetcd/etcdrpc/rpc_pb2.pyi` & `etcd-sdk-python-0.0.3/pyetcd/etcdrpc/rpc_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -3,738 +3,762 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
+
+class AlarmType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    NONE: _ClassVar[AlarmType]
+    NOSPACE: _ClassVar[AlarmType]
 NONE: AlarmType
 NOSPACE: AlarmType
 
-class AlarmMember(_message.Message):
-    __slots__ = ["alarm", "memberID"]
-    ALARM_FIELD_NUMBER: _ClassVar[int]
-    MEMBERID_FIELD_NUMBER: _ClassVar[int]
-    alarm: AlarmType
-    memberID: int
-    def __init__(self, memberID: _Optional[int] = ..., alarm: _Optional[_Union[AlarmType, str]] = ...) -> None: ...
+class ResponseHeader(_message.Message):
+    __slots__ = ["cluster_id", "member_id", "revision", "raft_term"]
+    CLUSTER_ID_FIELD_NUMBER: _ClassVar[int]
+    MEMBER_ID_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    RAFT_TERM_FIELD_NUMBER: _ClassVar[int]
+    cluster_id: int
+    member_id: int
+    revision: int
+    raft_term: int
+    def __init__(self, cluster_id: _Optional[int] = ..., member_id: _Optional[int] = ..., revision: _Optional[int] = ..., raft_term: _Optional[int] = ...) -> None: ...
 
-class AlarmRequest(_message.Message):
-    __slots__ = ["action", "alarm", "memberID"]
-    class AlarmAction(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+class RangeRequest(_message.Message):
+    __slots__ = ["key", "range_end", "limit", "revision", "sort_order", "sort_target", "serializable", "keys_only", "count_only", "min_mod_revision", "max_mod_revision", "min_create_revision", "max_create_revision"]
+    class SortOrder(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    ACTION_FIELD_NUMBER: _ClassVar[int]
-    ACTIVATE: AlarmRequest.AlarmAction
-    ALARM_FIELD_NUMBER: _ClassVar[int]
-    DEACTIVATE: AlarmRequest.AlarmAction
-    GET: AlarmRequest.AlarmAction
-    MEMBERID_FIELD_NUMBER: _ClassVar[int]
-    action: AlarmRequest.AlarmAction
-    alarm: AlarmType
-    memberID: int
-    def __init__(self, action: _Optional[_Union[AlarmRequest.AlarmAction, str]] = ..., memberID: _Optional[int] = ..., alarm: _Optional[_Union[AlarmType, str]] = ...) -> None: ...
-
-class AlarmResponse(_message.Message):
-    __slots__ = ["alarms", "header"]
-    ALARMS_FIELD_NUMBER: _ClassVar[int]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    alarms: _containers.RepeatedCompositeFieldContainer[AlarmMember]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., alarms: _Optional[_Iterable[_Union[AlarmMember, _Mapping]]] = ...) -> None: ...
-
-class AuthDisableRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class AuthDisableResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
-
-class AuthEnableRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class AuthEnableResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
-
-class AuthRoleAddRequest(_message.Message):
-    __slots__ = ["name"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    def __init__(self, name: _Optional[str] = ...) -> None: ...
-
-class AuthRoleAddResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
-
-class AuthRoleDeleteRequest(_message.Message):
-    __slots__ = ["role"]
-    ROLE_FIELD_NUMBER: _ClassVar[int]
-    role: str
-    def __init__(self, role: _Optional[str] = ...) -> None: ...
-
-class AuthRoleDeleteResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
-
-class AuthRoleGetRequest(_message.Message):
-    __slots__ = ["role"]
-    ROLE_FIELD_NUMBER: _ClassVar[int]
-    role: str
-    def __init__(self, role: _Optional[str] = ...) -> None: ...
-
-class AuthRoleGetResponse(_message.Message):
-    __slots__ = ["header", "perm"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    PERM_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    perm: _containers.RepeatedCompositeFieldContainer[_auth_pb2.Permission]
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., perm: _Optional[_Iterable[_Union[_auth_pb2.Permission, _Mapping]]] = ...) -> None: ...
-
-class AuthRoleGrantPermissionRequest(_message.Message):
-    __slots__ = ["name", "perm"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PERM_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    perm: _auth_pb2.Permission
-    def __init__(self, name: _Optional[str] = ..., perm: _Optional[_Union[_auth_pb2.Permission, _Mapping]] = ...) -> None: ...
-
-class AuthRoleGrantPermissionResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
-
-class AuthRoleListRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class AuthRoleListResponse(_message.Message):
-    __slots__ = ["header", "roles"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    ROLES_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    roles: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., roles: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class AuthRoleRevokePermissionRequest(_message.Message):
-    __slots__ = ["key", "range_end", "role"]
+        NONE: _ClassVar[RangeRequest.SortOrder]
+        ASCEND: _ClassVar[RangeRequest.SortOrder]
+        DESCEND: _ClassVar[RangeRequest.SortOrder]
+    NONE: RangeRequest.SortOrder
+    ASCEND: RangeRequest.SortOrder
+    DESCEND: RangeRequest.SortOrder
+    class SortTarget(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        KEY: _ClassVar[RangeRequest.SortTarget]
+        VERSION: _ClassVar[RangeRequest.SortTarget]
+        CREATE: _ClassVar[RangeRequest.SortTarget]
+        MOD: _ClassVar[RangeRequest.SortTarget]
+        VALUE: _ClassVar[RangeRequest.SortTarget]
+    KEY: RangeRequest.SortTarget
+    VERSION: RangeRequest.SortTarget
+    CREATE: RangeRequest.SortTarget
+    MOD: RangeRequest.SortTarget
+    VALUE: RangeRequest.SortTarget
     KEY_FIELD_NUMBER: _ClassVar[int]
     RANGE_END_FIELD_NUMBER: _ClassVar[int]
-    ROLE_FIELD_NUMBER: _ClassVar[int]
-    key: str
-    range_end: str
-    role: str
-    def __init__(self, role: _Optional[str] = ..., key: _Optional[str] = ..., range_end: _Optional[str] = ...) -> None: ...
-
-class AuthRoleRevokePermissionResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
-
-class AuthUserAddRequest(_message.Message):
-    __slots__ = ["name", "password"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PASSWORD_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    password: str
-    def __init__(self, name: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
-
-class AuthUserAddResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
-
-class AuthUserChangePasswordRequest(_message.Message):
-    __slots__ = ["name", "password"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PASSWORD_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    password: str
-    def __init__(self, name: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
-
-class AuthUserChangePasswordResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
-
-class AuthUserDeleteRequest(_message.Message):
-    __slots__ = ["name"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    def __init__(self, name: _Optional[str] = ...) -> None: ...
-
-class AuthUserDeleteResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
-
-class AuthUserGetRequest(_message.Message):
-    __slots__ = ["name"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    def __init__(self, name: _Optional[str] = ...) -> None: ...
-
-class AuthUserGetResponse(_message.Message):
-    __slots__ = ["header", "roles"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    ROLES_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    roles: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., roles: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class AuthUserGrantRoleRequest(_message.Message):
-    __slots__ = ["role", "user"]
-    ROLE_FIELD_NUMBER: _ClassVar[int]
-    USER_FIELD_NUMBER: _ClassVar[int]
-    role: str
-    user: str
-    def __init__(self, user: _Optional[str] = ..., role: _Optional[str] = ...) -> None: ...
-
-class AuthUserGrantRoleResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
-
-class AuthUserListRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    SORT_ORDER_FIELD_NUMBER: _ClassVar[int]
+    SORT_TARGET_FIELD_NUMBER: _ClassVar[int]
+    SERIALIZABLE_FIELD_NUMBER: _ClassVar[int]
+    KEYS_ONLY_FIELD_NUMBER: _ClassVar[int]
+    COUNT_ONLY_FIELD_NUMBER: _ClassVar[int]
+    MIN_MOD_REVISION_FIELD_NUMBER: _ClassVar[int]
+    MAX_MOD_REVISION_FIELD_NUMBER: _ClassVar[int]
+    MIN_CREATE_REVISION_FIELD_NUMBER: _ClassVar[int]
+    MAX_CREATE_REVISION_FIELD_NUMBER: _ClassVar[int]
+    key: bytes
+    range_end: bytes
+    limit: int
+    revision: int
+    sort_order: RangeRequest.SortOrder
+    sort_target: RangeRequest.SortTarget
+    serializable: bool
+    keys_only: bool
+    count_only: bool
+    min_mod_revision: int
+    max_mod_revision: int
+    min_create_revision: int
+    max_create_revision: int
+    def __init__(self, key: _Optional[bytes] = ..., range_end: _Optional[bytes] = ..., limit: _Optional[int] = ..., revision: _Optional[int] = ..., sort_order: _Optional[_Union[RangeRequest.SortOrder, str]] = ..., sort_target: _Optional[_Union[RangeRequest.SortTarget, str]] = ..., serializable: bool = ..., keys_only: bool = ..., count_only: bool = ..., min_mod_revision: _Optional[int] = ..., max_mod_revision: _Optional[int] = ..., min_create_revision: _Optional[int] = ..., max_create_revision: _Optional[int] = ...) -> None: ...
 
-class AuthUserListResponse(_message.Message):
-    __slots__ = ["header", "users"]
+class RangeResponse(_message.Message):
+    __slots__ = ["header", "kvs", "more", "count"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    USERS_FIELD_NUMBER: _ClassVar[int]
+    KVS_FIELD_NUMBER: _ClassVar[int]
+    MORE_FIELD_NUMBER: _ClassVar[int]
+    COUNT_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
-    users: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., users: _Optional[_Iterable[str]] = ...) -> None: ...
+    kvs: _containers.RepeatedCompositeFieldContainer[_kv_pb2.KeyValue]
+    more: bool
+    count: int
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., kvs: _Optional[_Iterable[_Union[_kv_pb2.KeyValue, _Mapping]]] = ..., more: bool = ..., count: _Optional[int] = ...) -> None: ...
 
-class AuthUserRevokeRoleRequest(_message.Message):
-    __slots__ = ["name", "role"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    ROLE_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    role: str
-    def __init__(self, name: _Optional[str] = ..., role: _Optional[str] = ...) -> None: ...
+class PutRequest(_message.Message):
+    __slots__ = ["key", "value", "lease", "prev_kv", "ignore_value", "ignore_lease"]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    LEASE_FIELD_NUMBER: _ClassVar[int]
+    PREV_KV_FIELD_NUMBER: _ClassVar[int]
+    IGNORE_VALUE_FIELD_NUMBER: _ClassVar[int]
+    IGNORE_LEASE_FIELD_NUMBER: _ClassVar[int]
+    key: bytes
+    value: bytes
+    lease: int
+    prev_kv: bool
+    ignore_value: bool
+    ignore_lease: bool
+    def __init__(self, key: _Optional[bytes] = ..., value: _Optional[bytes] = ..., lease: _Optional[int] = ..., prev_kv: bool = ..., ignore_value: bool = ..., ignore_lease: bool = ...) -> None: ...
 
-class AuthUserRevokeRoleResponse(_message.Message):
-    __slots__ = ["header"]
+class PutResponse(_message.Message):
+    __slots__ = ["header", "prev_kv"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
+    PREV_KV_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+    prev_kv: _kv_pb2.KeyValue
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., prev_kv: _Optional[_Union[_kv_pb2.KeyValue, _Mapping]] = ...) -> None: ...
 
-class AuthenticateRequest(_message.Message):
-    __slots__ = ["name", "password"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PASSWORD_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    password: str
-    def __init__(self, name: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
+class DeleteRangeRequest(_message.Message):
+    __slots__ = ["key", "range_end", "prev_kv"]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    RANGE_END_FIELD_NUMBER: _ClassVar[int]
+    PREV_KV_FIELD_NUMBER: _ClassVar[int]
+    key: bytes
+    range_end: bytes
+    prev_kv: bool
+    def __init__(self, key: _Optional[bytes] = ..., range_end: _Optional[bytes] = ..., prev_kv: bool = ...) -> None: ...
 
-class AuthenticateResponse(_message.Message):
-    __slots__ = ["header", "token"]
+class DeleteRangeResponse(_message.Message):
+    __slots__ = ["header", "deleted", "prev_kvs"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    DELETED_FIELD_NUMBER: _ClassVar[int]
+    PREV_KVS_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
-    token: str
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., token: _Optional[str] = ...) -> None: ...
+    deleted: int
+    prev_kvs: _containers.RepeatedCompositeFieldContainer[_kv_pb2.KeyValue]
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., deleted: _Optional[int] = ..., prev_kvs: _Optional[_Iterable[_Union[_kv_pb2.KeyValue, _Mapping]]] = ...) -> None: ...
 
-class CompactionRequest(_message.Message):
-    __slots__ = ["physical", "revision"]
-    PHYSICAL_FIELD_NUMBER: _ClassVar[int]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    physical: bool
-    revision: int
-    def __init__(self, revision: _Optional[int] = ..., physical: bool = ...) -> None: ...
+class RequestOp(_message.Message):
+    __slots__ = ["request_range", "request_put", "request_delete_range", "request_txn"]
+    REQUEST_RANGE_FIELD_NUMBER: _ClassVar[int]
+    REQUEST_PUT_FIELD_NUMBER: _ClassVar[int]
+    REQUEST_DELETE_RANGE_FIELD_NUMBER: _ClassVar[int]
+    REQUEST_TXN_FIELD_NUMBER: _ClassVar[int]
+    request_range: RangeRequest
+    request_put: PutRequest
+    request_delete_range: DeleteRangeRequest
+    request_txn: TxnRequest
+    def __init__(self, request_range: _Optional[_Union[RangeRequest, _Mapping]] = ..., request_put: _Optional[_Union[PutRequest, _Mapping]] = ..., request_delete_range: _Optional[_Union[DeleteRangeRequest, _Mapping]] = ..., request_txn: _Optional[_Union[TxnRequest, _Mapping]] = ...) -> None: ...
 
-class CompactionResponse(_message.Message):
-    __slots__ = ["header"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+class ResponseOp(_message.Message):
+    __slots__ = ["response_range", "response_put", "response_delete_range", "response_txn"]
+    RESPONSE_RANGE_FIELD_NUMBER: _ClassVar[int]
+    RESPONSE_PUT_FIELD_NUMBER: _ClassVar[int]
+    RESPONSE_DELETE_RANGE_FIELD_NUMBER: _ClassVar[int]
+    RESPONSE_TXN_FIELD_NUMBER: _ClassVar[int]
+    response_range: RangeResponse
+    response_put: PutResponse
+    response_delete_range: DeleteRangeResponse
+    response_txn: TxnResponse
+    def __init__(self, response_range: _Optional[_Union[RangeResponse, _Mapping]] = ..., response_put: _Optional[_Union[PutResponse, _Mapping]] = ..., response_delete_range: _Optional[_Union[DeleteRangeResponse, _Mapping]] = ..., response_txn: _Optional[_Union[TxnResponse, _Mapping]] = ...) -> None: ...
 
 class Compare(_message.Message):
-    __slots__ = ["create_revision", "key", "lease", "mod_revision", "range_end", "result", "target", "value", "version"]
+    __slots__ = ["result", "target", "key", "version", "create_revision", "mod_revision", "value", "lease", "range_end"]
     class CompareResult(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    class CompareTarget(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    CREATE: Compare.CompareTarget
-    CREATE_REVISION_FIELD_NUMBER: _ClassVar[int]
+        EQUAL: _ClassVar[Compare.CompareResult]
+        GREATER: _ClassVar[Compare.CompareResult]
+        LESS: _ClassVar[Compare.CompareResult]
+        NOT_EQUAL: _ClassVar[Compare.CompareResult]
     EQUAL: Compare.CompareResult
     GREATER: Compare.CompareResult
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    LEASE: Compare.CompareTarget
-    LEASE_FIELD_NUMBER: _ClassVar[int]
     LESS: Compare.CompareResult
-    MOD: Compare.CompareTarget
-    MOD_REVISION_FIELD_NUMBER: _ClassVar[int]
     NOT_EQUAL: Compare.CompareResult
-    RANGE_END_FIELD_NUMBER: _ClassVar[int]
+    class CompareTarget(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        VERSION: _ClassVar[Compare.CompareTarget]
+        CREATE: _ClassVar[Compare.CompareTarget]
+        MOD: _ClassVar[Compare.CompareTarget]
+        VALUE: _ClassVar[Compare.CompareTarget]
+        LEASE: _ClassVar[Compare.CompareTarget]
+    VERSION: Compare.CompareTarget
+    CREATE: Compare.CompareTarget
+    MOD: Compare.CompareTarget
+    VALUE: Compare.CompareTarget
+    LEASE: Compare.CompareTarget
     RESULT_FIELD_NUMBER: _ClassVar[int]
     TARGET_FIELD_NUMBER: _ClassVar[int]
-    VALUE: Compare.CompareTarget
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    VERSION: Compare.CompareTarget
+    KEY_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
-    create_revision: int
-    key: bytes
-    lease: int
-    mod_revision: int
-    range_end: bytes
+    CREATE_REVISION_FIELD_NUMBER: _ClassVar[int]
+    MOD_REVISION_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    LEASE_FIELD_NUMBER: _ClassVar[int]
+    RANGE_END_FIELD_NUMBER: _ClassVar[int]
     result: Compare.CompareResult
     target: Compare.CompareTarget
-    value: bytes
+    key: bytes
     version: int
+    create_revision: int
+    mod_revision: int
+    value: bytes
+    lease: int
+    range_end: bytes
     def __init__(self, result: _Optional[_Union[Compare.CompareResult, str]] = ..., target: _Optional[_Union[Compare.CompareTarget, str]] = ..., key: _Optional[bytes] = ..., version: _Optional[int] = ..., create_revision: _Optional[int] = ..., mod_revision: _Optional[int] = ..., value: _Optional[bytes] = ..., lease: _Optional[int] = ..., range_end: _Optional[bytes] = ...) -> None: ...
 
-class DefragmentRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
+class TxnRequest(_message.Message):
+    __slots__ = ["compare", "success", "failure"]
+    COMPARE_FIELD_NUMBER: _ClassVar[int]
+    SUCCESS_FIELD_NUMBER: _ClassVar[int]
+    FAILURE_FIELD_NUMBER: _ClassVar[int]
+    compare: _containers.RepeatedCompositeFieldContainer[Compare]
+    success: _containers.RepeatedCompositeFieldContainer[RequestOp]
+    failure: _containers.RepeatedCompositeFieldContainer[RequestOp]
+    def __init__(self, compare: _Optional[_Iterable[_Union[Compare, _Mapping]]] = ..., success: _Optional[_Iterable[_Union[RequestOp, _Mapping]]] = ..., failure: _Optional[_Iterable[_Union[RequestOp, _Mapping]]] = ...) -> None: ...
 
-class DefragmentResponse(_message.Message):
+class TxnResponse(_message.Message):
+    __slots__ = ["header", "succeeded", "responses"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    SUCCEEDED_FIELD_NUMBER: _ClassVar[int]
+    RESPONSES_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    succeeded: bool
+    responses: _containers.RepeatedCompositeFieldContainer[ResponseOp]
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., succeeded: bool = ..., responses: _Optional[_Iterable[_Union[ResponseOp, _Mapping]]] = ...) -> None: ...
+
+class CompactionRequest(_message.Message):
+    __slots__ = ["revision", "physical"]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    PHYSICAL_FIELD_NUMBER: _ClassVar[int]
+    revision: int
+    physical: bool
+    def __init__(self, revision: _Optional[int] = ..., physical: bool = ...) -> None: ...
+
+class CompactionResponse(_message.Message):
     __slots__ = ["header"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
     def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
 
-class DeleteRangeRequest(_message.Message):
-    __slots__ = ["key", "prev_kv", "range_end"]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    PREV_KV_FIELD_NUMBER: _ClassVar[int]
-    RANGE_END_FIELD_NUMBER: _ClassVar[int]
-    key: bytes
-    prev_kv: bool
-    range_end: bytes
-    def __init__(self, key: _Optional[bytes] = ..., range_end: _Optional[bytes] = ..., prev_kv: bool = ...) -> None: ...
+class HashRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
 
-class DeleteRangeResponse(_message.Message):
-    __slots__ = ["deleted", "header", "prev_kvs"]
-    DELETED_FIELD_NUMBER: _ClassVar[int]
+class HashResponse(_message.Message):
+    __slots__ = ["header", "hash"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    PREV_KVS_FIELD_NUMBER: _ClassVar[int]
-    deleted: int
+    HASH_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
-    prev_kvs: _containers.RepeatedCompositeFieldContainer[_kv_pb2.KeyValue]
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., deleted: _Optional[int] = ..., prev_kvs: _Optional[_Iterable[_Union[_kv_pb2.KeyValue, _Mapping]]] = ...) -> None: ...
+    hash: int
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., hash: _Optional[int] = ...) -> None: ...
 
 class HashKVRequest(_message.Message):
     __slots__ = ["revision"]
     REVISION_FIELD_NUMBER: _ClassVar[int]
     revision: int
     def __init__(self, revision: _Optional[int] = ...) -> None: ...
 
 class HashKVResponse(_message.Message):
-    __slots__ = ["compact_revision", "hash", "header"]
-    COMPACT_REVISION_FIELD_NUMBER: _ClassVar[int]
-    HASH_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["header", "hash", "compact_revision"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    compact_revision: int
-    hash: int
+    HASH_FIELD_NUMBER: _ClassVar[int]
+    COMPACT_REVISION_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
+    hash: int
+    compact_revision: int
     def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., hash: _Optional[int] = ..., compact_revision: _Optional[int] = ...) -> None: ...
 
-class HashRequest(_message.Message):
+class SnapshotRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class HashResponse(_message.Message):
-    __slots__ = ["hash", "header"]
-    HASH_FIELD_NUMBER: _ClassVar[int]
+class SnapshotResponse(_message.Message):
+    __slots__ = ["header", "remaining_bytes", "blob"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    hash: int
+    REMAINING_BYTES_FIELD_NUMBER: _ClassVar[int]
+    BLOB_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., hash: _Optional[int] = ...) -> None: ...
+    remaining_bytes: int
+    blob: bytes
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., remaining_bytes: _Optional[int] = ..., blob: _Optional[bytes] = ...) -> None: ...
+
+class WatchRequest(_message.Message):
+    __slots__ = ["create_request", "cancel_request", "progress_request"]
+    CREATE_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    CANCEL_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    PROGRESS_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    create_request: WatchCreateRequest
+    cancel_request: WatchCancelRequest
+    progress_request: WatchProgressRequest
+    def __init__(self, create_request: _Optional[_Union[WatchCreateRequest, _Mapping]] = ..., cancel_request: _Optional[_Union[WatchCancelRequest, _Mapping]] = ..., progress_request: _Optional[_Union[WatchProgressRequest, _Mapping]] = ...) -> None: ...
+
+class WatchCreateRequest(_message.Message):
+    __slots__ = ["key", "range_end", "start_revision", "progress_notify", "filters", "prev_kv"]
+    class FilterType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        NOPUT: _ClassVar[WatchCreateRequest.FilterType]
+        NODELETE: _ClassVar[WatchCreateRequest.FilterType]
+    NOPUT: WatchCreateRequest.FilterType
+    NODELETE: WatchCreateRequest.FilterType
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    RANGE_END_FIELD_NUMBER: _ClassVar[int]
+    START_REVISION_FIELD_NUMBER: _ClassVar[int]
+    PROGRESS_NOTIFY_FIELD_NUMBER: _ClassVar[int]
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    PREV_KV_FIELD_NUMBER: _ClassVar[int]
+    key: bytes
+    range_end: bytes
+    start_revision: int
+    progress_notify: bool
+    filters: _containers.RepeatedScalarFieldContainer[WatchCreateRequest.FilterType]
+    prev_kv: bool
+    def __init__(self, key: _Optional[bytes] = ..., range_end: _Optional[bytes] = ..., start_revision: _Optional[int] = ..., progress_notify: bool = ..., filters: _Optional[_Iterable[_Union[WatchCreateRequest.FilterType, str]]] = ..., prev_kv: bool = ...) -> None: ...
+
+class WatchCancelRequest(_message.Message):
+    __slots__ = ["watch_id"]
+    WATCH_ID_FIELD_NUMBER: _ClassVar[int]
+    watch_id: int
+    def __init__(self, watch_id: _Optional[int] = ...) -> None: ...
+
+class WatchProgressRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
+class WatchResponse(_message.Message):
+    __slots__ = ["header", "watch_id", "created", "canceled", "compact_revision", "cancel_reason", "events"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    WATCH_ID_FIELD_NUMBER: _ClassVar[int]
+    CREATED_FIELD_NUMBER: _ClassVar[int]
+    CANCELED_FIELD_NUMBER: _ClassVar[int]
+    COMPACT_REVISION_FIELD_NUMBER: _ClassVar[int]
+    CANCEL_REASON_FIELD_NUMBER: _ClassVar[int]
+    EVENTS_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    watch_id: int
+    created: bool
+    canceled: bool
+    compact_revision: int
+    cancel_reason: str
+    events: _containers.RepeatedCompositeFieldContainer[_kv_pb2.Event]
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., watch_id: _Optional[int] = ..., created: bool = ..., canceled: bool = ..., compact_revision: _Optional[int] = ..., cancel_reason: _Optional[str] = ..., events: _Optional[_Iterable[_Union[_kv_pb2.Event, _Mapping]]] = ...) -> None: ...
 
 class LeaseGrantRequest(_message.Message):
-    __slots__ = ["ID", "TTL"]
-    ID: int
+    __slots__ = ["TTL", "ID"]
+    TTL_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     TTL: int
-    TTL_FIELD_NUMBER: _ClassVar[int]
+    ID: int
     def __init__(self, TTL: _Optional[int] = ..., ID: _Optional[int] = ...) -> None: ...
 
 class LeaseGrantResponse(_message.Message):
-    __slots__ = ["ID", "TTL", "error", "header"]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["header", "ID", "TTL", "error"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    ID: int
     ID_FIELD_NUMBER: _ClassVar[int]
-    TTL: int
     TTL_FIELD_NUMBER: _ClassVar[int]
-    error: str
+    ERROR_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
+    ID: int
+    TTL: int
+    error: str
     def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., ID: _Optional[int] = ..., TTL: _Optional[int] = ..., error: _Optional[str] = ...) -> None: ...
 
-class LeaseKeepAliveRequest(_message.Message):
+class LeaseRevokeRequest(_message.Message):
     __slots__ = ["ID"]
-    ID: int
     ID_FIELD_NUMBER: _ClassVar[int]
+    ID: int
     def __init__(self, ID: _Optional[int] = ...) -> None: ...
 
-class LeaseKeepAliveResponse(_message.Message):
-    __slots__ = ["ID", "TTL", "header"]
+class LeaseRevokeResponse(_message.Message):
+    __slots__ = ["header"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    ID: int
-    ID_FIELD_NUMBER: _ClassVar[int]
-    TTL: int
-    TTL_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., ID: _Optional[int] = ..., TTL: _Optional[int] = ...) -> None: ...
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
 
-class LeaseRevokeRequest(_message.Message):
+class LeaseKeepAliveRequest(_message.Message):
     __slots__ = ["ID"]
-    ID: int
     ID_FIELD_NUMBER: _ClassVar[int]
+    ID: int
     def __init__(self, ID: _Optional[int] = ...) -> None: ...
 
-class LeaseRevokeResponse(_message.Message):
-    __slots__ = ["header"]
+class LeaseKeepAliveResponse(_message.Message):
+    __slots__ = ["header", "ID", "TTL"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    TTL_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+    ID: int
+    TTL: int
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., ID: _Optional[int] = ..., TTL: _Optional[int] = ...) -> None: ...
 
 class LeaseTimeToLiveRequest(_message.Message):
     __slots__ = ["ID", "keys"]
-    ID: int
     ID_FIELD_NUMBER: _ClassVar[int]
     KEYS_FIELD_NUMBER: _ClassVar[int]
+    ID: int
     keys: bool
     def __init__(self, ID: _Optional[int] = ..., keys: bool = ...) -> None: ...
 
 class LeaseTimeToLiveResponse(_message.Message):
-    __slots__ = ["ID", "TTL", "grantedTTL", "header", "keys"]
-    GRANTEDTTL_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["header", "ID", "TTL", "grantedTTL", "keys"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    ID: int
     ID_FIELD_NUMBER: _ClassVar[int]
+    TTL_FIELD_NUMBER: _ClassVar[int]
+    GRANTEDTTL_FIELD_NUMBER: _ClassVar[int]
     KEYS_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    ID: int
     TTL: int
-    TTL_FIELD_NUMBER: _ClassVar[int]
     grantedTTL: int
-    header: ResponseHeader
     keys: _containers.RepeatedScalarFieldContainer[bytes]
     def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., ID: _Optional[int] = ..., TTL: _Optional[int] = ..., grantedTTL: _Optional[int] = ..., keys: _Optional[_Iterable[bytes]] = ...) -> None: ...
 
 class Member(_message.Message):
-    __slots__ = ["ID", "clientURLs", "name", "peerURLs"]
-    CLIENTURLS_FIELD_NUMBER: _ClassVar[int]
-    ID: int
+    __slots__ = ["ID", "name", "peerURLs", "clientURLs"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     PEERURLS_FIELD_NUMBER: _ClassVar[int]
-    clientURLs: _containers.RepeatedScalarFieldContainer[str]
+    CLIENTURLS_FIELD_NUMBER: _ClassVar[int]
+    ID: int
     name: str
     peerURLs: _containers.RepeatedScalarFieldContainer[str]
+    clientURLs: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, ID: _Optional[int] = ..., name: _Optional[str] = ..., peerURLs: _Optional[_Iterable[str]] = ..., clientURLs: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class MemberAddRequest(_message.Message):
     __slots__ = ["peerURLs"]
     PEERURLS_FIELD_NUMBER: _ClassVar[int]
     peerURLs: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, peerURLs: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class MemberAddResponse(_message.Message):
     __slots__ = ["header", "member", "members"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    MEMBERS_FIELD_NUMBER: _ClassVar[int]
     MEMBER_FIELD_NUMBER: _ClassVar[int]
+    MEMBERS_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
     member: Member
     members: _containers.RepeatedCompositeFieldContainer[Member]
     def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., member: _Optional[_Union[Member, _Mapping]] = ..., members: _Optional[_Iterable[_Union[Member, _Mapping]]] = ...) -> None: ...
 
-class MemberListRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class MemberListResponse(_message.Message):
-    __slots__ = ["header", "members"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    MEMBERS_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    members: _containers.RepeatedCompositeFieldContainer[Member]
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., members: _Optional[_Iterable[_Union[Member, _Mapping]]] = ...) -> None: ...
-
 class MemberRemoveRequest(_message.Message):
     __slots__ = ["ID"]
-    ID: int
     ID_FIELD_NUMBER: _ClassVar[int]
+    ID: int
     def __init__(self, ID: _Optional[int] = ...) -> None: ...
 
 class MemberRemoveResponse(_message.Message):
     __slots__ = ["header", "members"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
     MEMBERS_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
     members: _containers.RepeatedCompositeFieldContainer[Member]
     def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., members: _Optional[_Iterable[_Union[Member, _Mapping]]] = ...) -> None: ...
 
 class MemberUpdateRequest(_message.Message):
     __slots__ = ["ID", "peerURLs"]
-    ID: int
     ID_FIELD_NUMBER: _ClassVar[int]
     PEERURLS_FIELD_NUMBER: _ClassVar[int]
+    ID: int
     peerURLs: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, ID: _Optional[int] = ..., peerURLs: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class MemberUpdateResponse(_message.Message):
     __slots__ = ["header", "members"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
     MEMBERS_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
     members: _containers.RepeatedCompositeFieldContainer[Member]
     def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., members: _Optional[_Iterable[_Union[Member, _Mapping]]] = ...) -> None: ...
 
+class MemberListRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
+class MemberListResponse(_message.Message):
+    __slots__ = ["header", "members"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    MEMBERS_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    members: _containers.RepeatedCompositeFieldContainer[Member]
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., members: _Optional[_Iterable[_Union[Member, _Mapping]]] = ...) -> None: ...
+
+class DefragmentRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
+class DefragmentResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+
 class MoveLeaderRequest(_message.Message):
     __slots__ = ["targetID"]
     TARGETID_FIELD_NUMBER: _ClassVar[int]
     targetID: int
     def __init__(self, targetID: _Optional[int] = ...) -> None: ...
 
 class MoveLeaderResponse(_message.Message):
     __slots__ = ["header"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
     def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
 
-class PutRequest(_message.Message):
-    __slots__ = ["ignore_lease", "ignore_value", "key", "lease", "prev_kv", "value"]
-    IGNORE_LEASE_FIELD_NUMBER: _ClassVar[int]
-    IGNORE_VALUE_FIELD_NUMBER: _ClassVar[int]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    LEASE_FIELD_NUMBER: _ClassVar[int]
-    PREV_KV_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    ignore_lease: bool
-    ignore_value: bool
-    key: bytes
-    lease: int
-    prev_kv: bool
-    value: bytes
-    def __init__(self, key: _Optional[bytes] = ..., value: _Optional[bytes] = ..., lease: _Optional[int] = ..., prev_kv: bool = ..., ignore_value: bool = ..., ignore_lease: bool = ...) -> None: ...
-
-class PutResponse(_message.Message):
-    __slots__ = ["header", "prev_kv"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    PREV_KV_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    prev_kv: _kv_pb2.KeyValue
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., prev_kv: _Optional[_Union[_kv_pb2.KeyValue, _Mapping]] = ...) -> None: ...
-
-class RangeRequest(_message.Message):
-    __slots__ = ["count_only", "key", "keys_only", "limit", "max_create_revision", "max_mod_revision", "min_create_revision", "min_mod_revision", "range_end", "revision", "serializable", "sort_order", "sort_target"]
-    class SortOrder(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class SortTarget(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+class AlarmRequest(_message.Message):
+    __slots__ = ["action", "memberID", "alarm"]
+    class AlarmAction(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    ASCEND: RangeRequest.SortOrder
-    COUNT_ONLY_FIELD_NUMBER: _ClassVar[int]
-    CREATE: RangeRequest.SortTarget
-    DESCEND: RangeRequest.SortOrder
-    KEY: RangeRequest.SortTarget
-    KEYS_ONLY_FIELD_NUMBER: _ClassVar[int]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    LIMIT_FIELD_NUMBER: _ClassVar[int]
-    MAX_CREATE_REVISION_FIELD_NUMBER: _ClassVar[int]
-    MAX_MOD_REVISION_FIELD_NUMBER: _ClassVar[int]
-    MIN_CREATE_REVISION_FIELD_NUMBER: _ClassVar[int]
-    MIN_MOD_REVISION_FIELD_NUMBER: _ClassVar[int]
-    MOD: RangeRequest.SortTarget
-    NONE: RangeRequest.SortOrder
-    RANGE_END_FIELD_NUMBER: _ClassVar[int]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    SERIALIZABLE_FIELD_NUMBER: _ClassVar[int]
-    SORT_ORDER_FIELD_NUMBER: _ClassVar[int]
-    SORT_TARGET_FIELD_NUMBER: _ClassVar[int]
-    VALUE: RangeRequest.SortTarget
-    VERSION: RangeRequest.SortTarget
-    count_only: bool
-    key: bytes
-    keys_only: bool
-    limit: int
-    max_create_revision: int
-    max_mod_revision: int
-    min_create_revision: int
-    min_mod_revision: int
-    range_end: bytes
-    revision: int
-    serializable: bool
-    sort_order: RangeRequest.SortOrder
-    sort_target: RangeRequest.SortTarget
-    def __init__(self, key: _Optional[bytes] = ..., range_end: _Optional[bytes] = ..., limit: _Optional[int] = ..., revision: _Optional[int] = ..., sort_order: _Optional[_Union[RangeRequest.SortOrder, str]] = ..., sort_target: _Optional[_Union[RangeRequest.SortTarget, str]] = ..., serializable: bool = ..., keys_only: bool = ..., count_only: bool = ..., min_mod_revision: _Optional[int] = ..., max_mod_revision: _Optional[int] = ..., min_create_revision: _Optional[int] = ..., max_create_revision: _Optional[int] = ...) -> None: ...
-
-class RangeResponse(_message.Message):
-    __slots__ = ["count", "header", "kvs", "more"]
-    COUNT_FIELD_NUMBER: _ClassVar[int]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    KVS_FIELD_NUMBER: _ClassVar[int]
-    MORE_FIELD_NUMBER: _ClassVar[int]
-    count: int
-    header: ResponseHeader
-    kvs: _containers.RepeatedCompositeFieldContainer[_kv_pb2.KeyValue]
-    more: bool
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., kvs: _Optional[_Iterable[_Union[_kv_pb2.KeyValue, _Mapping]]] = ..., more: bool = ..., count: _Optional[int] = ...) -> None: ...
-
-class RequestOp(_message.Message):
-    __slots__ = ["request_delete_range", "request_put", "request_range", "request_txn"]
-    REQUEST_DELETE_RANGE_FIELD_NUMBER: _ClassVar[int]
-    REQUEST_PUT_FIELD_NUMBER: _ClassVar[int]
-    REQUEST_RANGE_FIELD_NUMBER: _ClassVar[int]
-    REQUEST_TXN_FIELD_NUMBER: _ClassVar[int]
-    request_delete_range: DeleteRangeRequest
-    request_put: PutRequest
-    request_range: RangeRequest
-    request_txn: TxnRequest
-    def __init__(self, request_range: _Optional[_Union[RangeRequest, _Mapping]] = ..., request_put: _Optional[_Union[PutRequest, _Mapping]] = ..., request_delete_range: _Optional[_Union[DeleteRangeRequest, _Mapping]] = ..., request_txn: _Optional[_Union[TxnRequest, _Mapping]] = ...) -> None: ...
-
-class ResponseHeader(_message.Message):
-    __slots__ = ["cluster_id", "member_id", "raft_term", "revision"]
-    CLUSTER_ID_FIELD_NUMBER: _ClassVar[int]
-    MEMBER_ID_FIELD_NUMBER: _ClassVar[int]
-    RAFT_TERM_FIELD_NUMBER: _ClassVar[int]
-    REVISION_FIELD_NUMBER: _ClassVar[int]
-    cluster_id: int
-    member_id: int
-    raft_term: int
-    revision: int
-    def __init__(self, cluster_id: _Optional[int] = ..., member_id: _Optional[int] = ..., revision: _Optional[int] = ..., raft_term: _Optional[int] = ...) -> None: ...
-
-class ResponseOp(_message.Message):
-    __slots__ = ["response_delete_range", "response_put", "response_range", "response_txn"]
-    RESPONSE_DELETE_RANGE_FIELD_NUMBER: _ClassVar[int]
-    RESPONSE_PUT_FIELD_NUMBER: _ClassVar[int]
-    RESPONSE_RANGE_FIELD_NUMBER: _ClassVar[int]
-    RESPONSE_TXN_FIELD_NUMBER: _ClassVar[int]
-    response_delete_range: DeleteRangeResponse
-    response_put: PutResponse
-    response_range: RangeResponse
-    response_txn: TxnResponse
-    def __init__(self, response_range: _Optional[_Union[RangeResponse, _Mapping]] = ..., response_put: _Optional[_Union[PutResponse, _Mapping]] = ..., response_delete_range: _Optional[_Union[DeleteRangeResponse, _Mapping]] = ..., response_txn: _Optional[_Union[TxnResponse, _Mapping]] = ...) -> None: ...
+        GET: _ClassVar[AlarmRequest.AlarmAction]
+        ACTIVATE: _ClassVar[AlarmRequest.AlarmAction]
+        DEACTIVATE: _ClassVar[AlarmRequest.AlarmAction]
+    GET: AlarmRequest.AlarmAction
+    ACTIVATE: AlarmRequest.AlarmAction
+    DEACTIVATE: AlarmRequest.AlarmAction
+    ACTION_FIELD_NUMBER: _ClassVar[int]
+    MEMBERID_FIELD_NUMBER: _ClassVar[int]
+    ALARM_FIELD_NUMBER: _ClassVar[int]
+    action: AlarmRequest.AlarmAction
+    memberID: int
+    alarm: AlarmType
+    def __init__(self, action: _Optional[_Union[AlarmRequest.AlarmAction, str]] = ..., memberID: _Optional[int] = ..., alarm: _Optional[_Union[AlarmType, str]] = ...) -> None: ...
 
-class SnapshotRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
+class AlarmMember(_message.Message):
+    __slots__ = ["memberID", "alarm"]
+    MEMBERID_FIELD_NUMBER: _ClassVar[int]
+    ALARM_FIELD_NUMBER: _ClassVar[int]
+    memberID: int
+    alarm: AlarmType
+    def __init__(self, memberID: _Optional[int] = ..., alarm: _Optional[_Union[AlarmType, str]] = ...) -> None: ...
 
-class SnapshotResponse(_message.Message):
-    __slots__ = ["blob", "header", "remaining_bytes"]
-    BLOB_FIELD_NUMBER: _ClassVar[int]
+class AlarmResponse(_message.Message):
+    __slots__ = ["header", "alarms"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    REMAINING_BYTES_FIELD_NUMBER: _ClassVar[int]
-    blob: bytes
+    ALARMS_FIELD_NUMBER: _ClassVar[int]
     header: ResponseHeader
-    remaining_bytes: int
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., remaining_bytes: _Optional[int] = ..., blob: _Optional[bytes] = ...) -> None: ...
+    alarms: _containers.RepeatedCompositeFieldContainer[AlarmMember]
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., alarms: _Optional[_Iterable[_Union[AlarmMember, _Mapping]]] = ...) -> None: ...
 
 class StatusRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class StatusResponse(_message.Message):
-    __slots__ = ["dbSize", "header", "leader", "raftIndex", "raftTerm", "version"]
-    DBSIZE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["header", "version", "dbSize", "leader", "raftIndex", "raftTerm"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    DBSIZE_FIELD_NUMBER: _ClassVar[int]
     LEADER_FIELD_NUMBER: _ClassVar[int]
     RAFTINDEX_FIELD_NUMBER: _ClassVar[int]
     RAFTTERM_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    dbSize: int
     header: ResponseHeader
+    version: str
+    dbSize: int
     leader: int
     raftIndex: int
     raftTerm: int
-    version: str
     def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., version: _Optional[str] = ..., dbSize: _Optional[int] = ..., leader: _Optional[int] = ..., raftIndex: _Optional[int] = ..., raftTerm: _Optional[int] = ...) -> None: ...
 
-class TxnRequest(_message.Message):
-    __slots__ = ["compare", "failure", "success"]
-    COMPARE_FIELD_NUMBER: _ClassVar[int]
-    FAILURE_FIELD_NUMBER: _ClassVar[int]
-    SUCCESS_FIELD_NUMBER: _ClassVar[int]
-    compare: _containers.RepeatedCompositeFieldContainer[Compare]
-    failure: _containers.RepeatedCompositeFieldContainer[RequestOp]
-    success: _containers.RepeatedCompositeFieldContainer[RequestOp]
-    def __init__(self, compare: _Optional[_Iterable[_Union[Compare, _Mapping]]] = ..., success: _Optional[_Iterable[_Union[RequestOp, _Mapping]]] = ..., failure: _Optional[_Iterable[_Union[RequestOp, _Mapping]]] = ...) -> None: ...
+class AuthEnableRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
 
-class TxnResponse(_message.Message):
-    __slots__ = ["header", "responses", "succeeded"]
-    HEADER_FIELD_NUMBER: _ClassVar[int]
-    RESPONSES_FIELD_NUMBER: _ClassVar[int]
-    SUCCEEDED_FIELD_NUMBER: _ClassVar[int]
-    header: ResponseHeader
-    responses: _containers.RepeatedCompositeFieldContainer[ResponseOp]
-    succeeded: bool
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., succeeded: bool = ..., responses: _Optional[_Iterable[_Union[ResponseOp, _Mapping]]] = ...) -> None: ...
+class AuthDisableRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
 
-class WatchCancelRequest(_message.Message):
-    __slots__ = ["watch_id"]
-    WATCH_ID_FIELD_NUMBER: _ClassVar[int]
-    watch_id: int
-    def __init__(self, watch_id: _Optional[int] = ...) -> None: ...
+class AuthenticateRequest(_message.Message):
+    __slots__ = ["name", "password"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    password: str
+    def __init__(self, name: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
 
-class WatchCreateRequest(_message.Message):
-    __slots__ = ["filters", "key", "prev_kv", "progress_notify", "range_end", "start_revision"]
-    class FilterType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    NODELETE: WatchCreateRequest.FilterType
-    NOPUT: WatchCreateRequest.FilterType
-    PREV_KV_FIELD_NUMBER: _ClassVar[int]
-    PROGRESS_NOTIFY_FIELD_NUMBER: _ClassVar[int]
-    RANGE_END_FIELD_NUMBER: _ClassVar[int]
-    START_REVISION_FIELD_NUMBER: _ClassVar[int]
-    filters: _containers.RepeatedScalarFieldContainer[WatchCreateRequest.FilterType]
-    key: bytes
-    prev_kv: bool
-    progress_notify: bool
-    range_end: bytes
-    start_revision: int
-    def __init__(self, key: _Optional[bytes] = ..., range_end: _Optional[bytes] = ..., start_revision: _Optional[int] = ..., progress_notify: bool = ..., filters: _Optional[_Iterable[_Union[WatchCreateRequest.FilterType, str]]] = ..., prev_kv: bool = ...) -> None: ...
+class AuthUserAddRequest(_message.Message):
+    __slots__ = ["name", "password"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    password: str
+    def __init__(self, name: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
 
-class WatchProgressRequest(_message.Message):
+class AuthUserGetRequest(_message.Message):
+    __slots__ = ["name"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    def __init__(self, name: _Optional[str] = ...) -> None: ...
+
+class AuthUserDeleteRequest(_message.Message):
+    __slots__ = ["name"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    def __init__(self, name: _Optional[str] = ...) -> None: ...
+
+class AuthUserChangePasswordRequest(_message.Message):
+    __slots__ = ["name", "password"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    password: str
+    def __init__(self, name: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
+
+class AuthUserGrantRoleRequest(_message.Message):
+    __slots__ = ["user", "role"]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    ROLE_FIELD_NUMBER: _ClassVar[int]
+    user: str
+    role: str
+    def __init__(self, user: _Optional[str] = ..., role: _Optional[str] = ...) -> None: ...
+
+class AuthUserRevokeRoleRequest(_message.Message):
+    __slots__ = ["name", "role"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    ROLE_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    role: str
+    def __init__(self, name: _Optional[str] = ..., role: _Optional[str] = ...) -> None: ...
+
+class AuthRoleAddRequest(_message.Message):
+    __slots__ = ["name"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    def __init__(self, name: _Optional[str] = ...) -> None: ...
+
+class AuthRoleGetRequest(_message.Message):
+    __slots__ = ["role"]
+    ROLE_FIELD_NUMBER: _ClassVar[int]
+    role: str
+    def __init__(self, role: _Optional[str] = ...) -> None: ...
+
+class AuthUserListRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class WatchRequest(_message.Message):
-    __slots__ = ["cancel_request", "create_request", "progress_request"]
-    CANCEL_REQUEST_FIELD_NUMBER: _ClassVar[int]
-    CREATE_REQUEST_FIELD_NUMBER: _ClassVar[int]
-    PROGRESS_REQUEST_FIELD_NUMBER: _ClassVar[int]
-    cancel_request: WatchCancelRequest
-    create_request: WatchCreateRequest
-    progress_request: WatchProgressRequest
-    def __init__(self, create_request: _Optional[_Union[WatchCreateRequest, _Mapping]] = ..., cancel_request: _Optional[_Union[WatchCancelRequest, _Mapping]] = ..., progress_request: _Optional[_Union[WatchProgressRequest, _Mapping]] = ...) -> None: ...
+class AuthRoleListRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
 
-class WatchResponse(_message.Message):
-    __slots__ = ["cancel_reason", "canceled", "compact_revision", "created", "events", "header", "watch_id"]
-    CANCELED_FIELD_NUMBER: _ClassVar[int]
-    CANCEL_REASON_FIELD_NUMBER: _ClassVar[int]
-    COMPACT_REVISION_FIELD_NUMBER: _ClassVar[int]
-    CREATED_FIELD_NUMBER: _ClassVar[int]
-    EVENTS_FIELD_NUMBER: _ClassVar[int]
+class AuthRoleDeleteRequest(_message.Message):
+    __slots__ = ["role"]
+    ROLE_FIELD_NUMBER: _ClassVar[int]
+    role: str
+    def __init__(self, role: _Optional[str] = ...) -> None: ...
+
+class AuthRoleGrantPermissionRequest(_message.Message):
+    __slots__ = ["name", "perm"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    PERM_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    perm: _auth_pb2.Permission
+    def __init__(self, name: _Optional[str] = ..., perm: _Optional[_Union[_auth_pb2.Permission, _Mapping]] = ...) -> None: ...
+
+class AuthRoleRevokePermissionRequest(_message.Message):
+    __slots__ = ["role", "key", "range_end"]
+    ROLE_FIELD_NUMBER: _ClassVar[int]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    RANGE_END_FIELD_NUMBER: _ClassVar[int]
+    role: str
+    key: str
+    range_end: str
+    def __init__(self, role: _Optional[str] = ..., key: _Optional[str] = ..., range_end: _Optional[str] = ...) -> None: ...
+
+class AuthEnableResponse(_message.Message):
+    __slots__ = ["header"]
     HEADER_FIELD_NUMBER: _ClassVar[int]
-    WATCH_ID_FIELD_NUMBER: _ClassVar[int]
-    cancel_reason: str
-    canceled: bool
-    compact_revision: int
-    created: bool
-    events: _containers.RepeatedCompositeFieldContainer[_kv_pb2.Event]
     header: ResponseHeader
-    watch_id: int
-    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., watch_id: _Optional[int] = ..., created: bool = ..., canceled: bool = ..., compact_revision: _Optional[int] = ..., cancel_reason: _Optional[str] = ..., events: _Optional[_Iterable[_Union[_kv_pb2.Event, _Mapping]]] = ...) -> None: ...
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
 
-class AlarmType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class AuthDisableResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+
+class AuthenticateResponse(_message.Message):
+    __slots__ = ["header", "token"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    token: str
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., token: _Optional[str] = ...) -> None: ...
+
+class AuthUserAddResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+
+class AuthUserGetResponse(_message.Message):
+    __slots__ = ["header", "roles"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    ROLES_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    roles: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., roles: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class AuthUserDeleteResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+
+class AuthUserChangePasswordResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+
+class AuthUserGrantRoleResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+
+class AuthUserRevokeRoleResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+
+class AuthRoleAddResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+
+class AuthRoleGetResponse(_message.Message):
+    __slots__ = ["header", "perm"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    PERM_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    perm: _containers.RepeatedCompositeFieldContainer[_auth_pb2.Permission]
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., perm: _Optional[_Iterable[_Union[_auth_pb2.Permission, _Mapping]]] = ...) -> None: ...
+
+class AuthRoleListResponse(_message.Message):
+    __slots__ = ["header", "roles"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    ROLES_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    roles: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., roles: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class AuthUserListResponse(_message.Message):
+    __slots__ = ["header", "users"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    USERS_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    users: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ..., users: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class AuthRoleDeleteResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+
+class AuthRoleGrantPermissionResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
+
+class AuthRoleRevokePermissionResponse(_message.Message):
+    __slots__ = ["header"]
+    HEADER_FIELD_NUMBER: _ClassVar[int]
+    header: ResponseHeader
+    def __init__(self, header: _Optional[_Union[ResponseHeader, _Mapping]] = ...) -> None: ...
```

### Comparing `etcd-sdk-python-0.0.2/pyetcd/etcdrpc/rpc_pb2_grpc.py` & `etcd-sdk-python-0.0.3/pyetcd/etcdrpc/rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/events.py` & `etcd-sdk-python-0.0.3/pyetcd/events.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/exceptions.py` & `etcd-sdk-python-0.0.3/pyetcd/exceptions.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/leases.py` & `etcd-sdk-python-0.0.3/pyetcd/leases.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/locks.py` & `etcd-sdk-python-0.0.3/pyetcd/locks.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/members.py` & `etcd-sdk-python-0.0.3/pyetcd/members.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/proto/auth.proto` & `etcd-sdk-python-0.0.3/pyetcd/proto/auth.proto`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/proto/kv.proto` & `etcd-sdk-python-0.0.3/pyetcd/proto/kv.proto`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/proto/rpc.proto` & `etcd-sdk-python-0.0.3/pyetcd/proto/rpc.proto`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/transactions.py` & `etcd-sdk-python-0.0.3/pyetcd/transactions.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/utils.py` & `etcd-sdk-python-0.0.3/pyetcd/utils.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyetcd/watch.py` & `etcd-sdk-python-0.0.3/pyetcd/watch.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/pyproject.toml` & `etcd-sdk-python-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -26,18 +26,17 @@
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies    = [
-    "grpcio>=1.49.1,<=1.53.0",
-    "grpcio-tools>=1.49.1,<=1.53.0",
+    "grpcio>=1.49.1,<=1.56.0",
+    "grpcio-tools>=1.49.1,<=1.56.0",
 ]
 
-version = "0.0.2"
+version = "0.0.3"
 
 [project.urls]
 "Homepage"          = "https://github.com/XuanYang-cn/pyetcd"
 "Docs: User Guide"  = "https://pyetcd-docs.readthedocs.io/en/latest/"
 "Source Code"       = "https://github.com/XuanYang-cn/pyetcd"
-# "Discord Server"    = ""
```

### Comparing `etcd-sdk-python-0.0.2/python_gen.sh` & `etcd-sdk-python-0.0.3/python_gen.sh`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tests/ca.crt` & `etcd-sdk-python-0.0.3/tests/ca.crt`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tests/client.crt` & `etcd-sdk-python-0.0.3/tests/client.crt`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tests/client.key` & `etcd-sdk-python-0.0.3/tests/client.key`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tests/conftest.py` & `etcd-sdk-python-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tests/test_alarms.py` & `etcd-sdk-python-0.0.3/tests/test_alarms.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tests/test_client.py` & `etcd-sdk-python-0.0.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tests/test_compares.py` & `etcd-sdk-python-0.0.3/tests/test_compares.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tests/test_failover.py` & `etcd-sdk-python-0.0.3/tests/test_failover.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tests/test_pyetcd.py` & `etcd-sdk-python-0.0.3/tests/test_pyetcd.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tests/test_utils.py` & `etcd-sdk-python-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `etcd-sdk-python-0.0.2/tox.ini` & `etcd-sdk-python-0.0.3/tox.ini`

 * *Files identical despite different names*

