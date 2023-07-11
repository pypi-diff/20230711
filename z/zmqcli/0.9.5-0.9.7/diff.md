# Comparing `tmp/zmqcli-0.9.5.tar.gz` & `tmp/zmqcli-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmqcli-0.9.5.tar", max compression
+gzip compressed data, was "zmqcli-0.9.7.tar", max compression
```

## Comparing `zmqcli-0.9.5.tar` & `zmqcli-0.9.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      527 2023-07-11 11:48:38.550033 zmqcli-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     6565 2021-05-10 23:18:52.158597 zmqcli-0.9.5/README.md
--rw-r--r--   0        0        0       68 2021-04-15 21:21:42.136071 zmqcli-0.9.5/zmqcli/__main__.py
--rw-r--r--   0        0        0    15604 2023-07-11 10:04:26.485053 zmqcli-0.9.5/zmqcli/zmqcli.py
--rw-r--r--   0        0        0     7052 1970-01-01 00:00:00.000000 zmqcli-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1125 2023-07-11 19:31:05.521167 zmqcli-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     6565 2021-05-10 23:18:52.158597 zmqcli-0.9.7/README.md
+-rw-r--r--   0        0        0       68 2021-04-15 21:21:42.136071 zmqcli-0.9.7/zmqcli/__main__.py
+-rw-r--r--   0        0        0    15604 2023-07-11 10:04:26.485053 zmqcli-0.9.7/zmqcli/zmqcli.py
+-rw-r--r--   0        0        0     7648 1970-01-01 00:00:00.000000 zmqcli-0.9.7/PKG-INFO
```

### Comparing `zmqcli-0.9.5/README.md` & `zmqcli-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `zmqcli-0.9.5/zmqcli/zmqcli.py` & `zmqcli-0.9.7/zmqcli/zmqcli.py`

 * *Files identical despite different names*

### Comparing `zmqcli-0.9.5/PKG-INFO` & `zmqcli-0.9.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.1
 Name: zmqcli
-Version: 0.9.5
-Summary: A small but powerful command-line interface to ØMQ.
-License: http://unlicense.org/
+Version: 0.9.7
+Summary: A small but powerful command-line interface to ZeroMQ.
+Home-page: https://gitlab.com/tamtamresearch-public/pypi/zmqcli
+License: Unlicense
+Keywords: ZeroMQ,CLI,ØMQ,0MQ,zmq
 Author: TamTam Research s.r.o.
+Maintainer: Roman Horenovsky
 Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: Utilities
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: pyzmq (>=25.0.0,<26.0.0)
+Project-URL: Documentation, https://gitlab.com/tamtamresearch-public/pypi/zmqcli
+Project-URL: Repository, https://gitlab.com/tamtamresearch-public/pypi/zmqcli
 Description-Content-Type: text/markdown
 
 # zmqcli
 
 zmqcli is a small but powerful command-line interface to [ØMQ][zmq] written in Python 3.
 
 It allows you to create a socket of a given type, bind or connect it to multiple
```

