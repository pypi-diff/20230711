# Comparing `tmp/zmqcli-0.9.4.tar.gz` & `tmp/zmqcli-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmqcli-0.9.4.tar", max compression
+gzip compressed data, was "zmqcli-0.9.5.tar", max compression
```

## Comparing `zmqcli-0.9.4.tar` & `zmqcli-0.9.5.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      505 2023-07-11 10:09:59.582167 zmqcli-0.9.4/pyproject.toml
--rw-r--r--   0        0        0       68 2021-04-15 21:21:42.136071 zmqcli-0.9.4/zmqcli/__main__.py
--rw-r--r--   0        0        0    15604 2023-07-11 10:04:26.485053 zmqcli-0.9.4/zmqcli/zmqcli.py
--rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 zmqcli-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      527 2023-07-11 11:48:38.550033 zmqcli-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     6565 2021-05-10 23:18:52.158597 zmqcli-0.9.5/README.md
+-rw-r--r--   0        0        0       68 2021-04-15 21:21:42.136071 zmqcli-0.9.5/zmqcli/__main__.py
+-rw-r--r--   0        0        0    15604 2023-07-11 10:04:26.485053 zmqcli-0.9.5/zmqcli/zmqcli.py
+-rw-r--r--   0        0        0     7052 1970-01-01 00:00:00.000000 zmqcli-0.9.5/PKG-INFO
```

### Comparing `zmqcli-0.9.4/zmqcli/zmqcli.py` & `zmqcli-0.9.5/zmqcli/zmqcli.py`

 * *Files identical despite different names*

