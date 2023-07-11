# Comparing `tmp/remotemanager-0.8.2.tar.gz` & `tmp/remotemanager-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.8.2.tar", last modified: Wed Jul  5 08:46:33 2023, max compression
+gzip compressed data, was "remotemanager-0.8.3.tar", last modified: Tue Jul 11 15:06:14 2023, max compression
```

## Comparing `remotemanager-0.8.2.tar` & `remotemanager-0.8.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.595770 remotemanager-0.8.2/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-05 08:46:33.591771 remotemanager-0.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-03 15:08:03.000000 remotemanager-0.8.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-03 15:08:03.000000 remotemanager-0.8.2/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.2/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12788 2023-06-29 14:39:51.000000 remotemanager-0.8.2/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.2/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.2/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.2/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.2/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    25712 2023-07-04 13:31:41.000000 remotemanager-0.8.2/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49554 2023-07-05 08:03:59.000000 remotemanager-0.8.2/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     4029 2023-06-26 08:49:48.000000 remotemanager-0.8.2/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    26063 2023-07-04 09:09:29.000000 remotemanager-0.8.2/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.2/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4922 2023-07-03 15:08:03.000000 remotemanager-0.8.2/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.591771 remotemanager-0.8.2/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.2/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.2/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.2/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.2/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.591771 remotemanager-0.8.2/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.2/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.2/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.2/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.591771 remotemanager-0.8.2/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.2/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.2/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-04 13:31:41.000000 remotemanager-0.8.2/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.591771 remotemanager-0.8.2/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.2/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.2/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9435 2023-06-26 08:49:48.000000 remotemanager-0.8.2/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.591771 remotemanager-0.8.2/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-05 08:46:33.000000 remotemanager-0.8.2/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-07-05 08:46:33.000000 remotemanager-0.8.2/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:46:33.000000 remotemanager-0.8.2/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-05 08:46:33.000000 remotemanager-0.8.2/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-05 08:46:33.000000 remotemanager-0.8.2/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:46:33.595770 remotemanager-0.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.258884 remotemanager-0.8.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-11 15:06:14.258884 remotemanager-0.8.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-11 12:30:54.000000 remotemanager-0.8.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.250884 remotemanager-0.8.3/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.250884 remotemanager-0.8.3/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.3/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.254884 remotemanager-0.8.3/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.8.3/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.3/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.3/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.3/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.3/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    25712 2023-07-04 13:31:41.000000 remotemanager-0.8.3/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.254884 remotemanager-0.8.3/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49329 2023-07-11 13:37:44.000000 remotemanager-0.8.3/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    26112 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.254884 remotemanager-0.8.3/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.3/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4922 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.254884 remotemanager-0.8.3/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.3/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.3/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.3/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.3/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.254884 remotemanager-0.8.3/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.3/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.3/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.3/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.258884 remotemanager-0.8.3/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.3/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.3/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.258884 remotemanager-0.8.3/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.3/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.3/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9435 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.258884 remotemanager-0.8.3/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2023-07-11 13:37:44.000000 remotemanager-0.8.3/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.250884 remotemanager-0.8.3/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-11 15:06:14.000000 remotemanager-0.8.3/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-07-11 15:06:14.000000 remotemanager-0.8.3/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:06:14.000000 remotemanager-0.8.3/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-11 15:06:14.000000 remotemanager-0.8.3/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 15:06:14.000000 remotemanager-0.8.3/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 15:06:14.258884 remotemanager-0.8.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.3/setup.py
```

### Comparing `remotemanager-0.8.2/LICENSE` & `remotemanager-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/PKG-INFO` & `remotemanager-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.8.2
+Version: 0.8.3
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.8.2/README.md` & `remotemanager-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/pyproject.toml` & `remotemanager-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.8.2"
+current_version = "0.8.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.8.2/remotemanager/connection/cmd.py` & `remotemanager-0.8.3/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/connection/computers/base.py` & `remotemanager-0.8.3/remotemanager/connection/computers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,18 @@
                 attribute = optional(**args)
             else:
                 attribute = required(**args)
 
             computer.__setattr__(field, attribute)
 
         # create a new class, primed with the hostname and parser
-        computer = cls(host=spec.get("host", None), **url_args)
+        if "host" not in url_args:
+            url_args["host"] = spec.get("host", None)
+        computer = cls(**url_args)
+
         computer.parser = spec.get("resource_parser")
         computer.submitter = spec.get("submitter", None)
         computer.python = spec.get("python", None)
 
         # add the resource storing objects to the class
         required_resources = spec.get("resources")
         selected_resources = spec.get("required_or", [])
```

### Comparing `remotemanager-0.8.2/remotemanager/connection/computers/example.py` & `remotemanager-0.8.3/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/connection/computers/options.py` & `remotemanager-0.8.3/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/connection/computers/parsers.py` & `remotemanager-0.8.3/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/connection/testing_object.py` & `remotemanager-0.8.3/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/connection/url.py` & `remotemanager-0.8.3/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/dataset/dataset.py` & `remotemanager-0.8.3/remotemanager/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from remotemanager.storage.database import Database
 from remotemanager.storage.function import Function
 from remotemanager.dataset.runner import Runner, localwinerror
 import remotemanager.transport as tp
 import remotemanager.serialisation as sr
 from remotemanager.storage import SendableMixin, TrackedFile
 from remotemanager.utils.uuid import generate_uuid
-from remotemanager.utils import ensure_list, ensure_filetype
+from remotemanager.utils import ensure_list, ensure_filetype, check_dir_is_child
 from remotemanager.logging.utils import format_iterable
 from remotemanager.dataset.dependency import Dependency
 from remotemanager.logging import LoggingMixin
 from remotemanager.logging.verbosity import Verbosity
 from remotemanager.logging.quiet import Quiet
 
 
@@ -663,14 +663,20 @@
             files_only (bool):
                 delete individual files instead of whole folders (preserves
                 extra files)
 
         Returns:
             None
         """
+        if not check_dir_is_child:
+            raise RuntimeError(
+                f"local dir {self.local_dir} is not a child directory, "
+                f"deleting could have catastrophic effects"
+            )
+
         if not files_only:
             locals = self._collect_files("local_dir")
             self._logger.warning(f"removing remote_dir(s): {locals}")
 
             for local in locals:
                 try:
                     shutil.rmtree(local)
@@ -1229,31 +1235,14 @@
             if len(cached_functions) > 0:
                 o.write("### cached functions ###\n")
 
                 for fname, f in cached_functions.items():
                     o.write(f.source + "\n")
                 o.write("\n")
 
-            if self.is_parent:
-                o.write("### dependency functions ###\n")
-
-                o.write(
-                    """
-def submit_child(file, stderr):
-    import subprocess
-    subprocess.Popen(f"bash '{file}'",
-                     stdout=subprocess.PIPE,
-                     stderr=open(stderr, "w+"),
-                     shell=True,
-                     universal_newlines=True)
-\n"""
-                )
-
-                o.write("\n")
-
             o.write("### primary function ###\n")
             o.write(self.function.source)
 
             o.write("\n### serialiser functions ###")
             o.write(self.serialiser.dumpfunc())
             o.write("\n")
             o.write(self.serialiser.loadfunc())
```

### Comparing `remotemanager-0.8.2/remotemanager/dataset/dependency.py` & `remotemanager-0.8.3/remotemanager/dataset/dependency.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,21 +103,20 @@
                     f'repo.loaded = repo.load("'
                     f'{parent.runners[-1].resultfile.name}")'
                 )
                 ds.runners[-1]._dependency_info["parent_import"] = lstr
 
             tmp = []
             for child in self.get_children(ds):
-                tmp.append(f"import time")
-                tmp.append(f"time.sleep(1)")
+                runner = child.runners[-1]
                 tmp.append(
-                    f'repo.submit_child("'
-                    f'{child.runners[-1].jobscript.name}", '
-                    f'"{child.runners[-1].errorfile.name}")\n'
+                    f"{child.url.submitter} {runner.jobscript.name} "
+                    f"2>> {runner.errorfile.name}"
                 )
+
             ds.runners[-1]._dependency_info["child_submit"] = tmp
 
             ds.database.update(ds.pack())
 
     def run(self, *args, **kwargs):
         self._logger.info("dependency internal run call")
```

### Comparing `remotemanager-0.8.2/remotemanager/dataset/runner.py` & `remotemanager-0.8.3/remotemanager/dataset/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -710,17 +710,14 @@
             argline,
             f"result = repo.{dataset.function.name}(**kwargs)",
             f"repo.dump(result, '{self.resultfile.name}')",
         ]
 
         if dataset.is_child:
             runscript.insert(2, self._dependency_info["parent_import"])
-        if dataset.is_parent:
-            for line in self._dependency_info["child_submit"]:
-                runscript.append(line)
 
         output = "\n".join(runscript)
         if write_file:
             if not os.path.isdir(self.local_dir):
                 self._logger.info(f"creating local dir {self.local_dir}")
                 os.makedirs(self.local_dir)
             with open(self.runfile.local, "w+") as o:
@@ -758,14 +755,19 @@
         else:
             runline = f"{python} {self.runfile.name} 2>> {self.errorfile.name}"
             self._logger.debug(f"directly appending line {runline}")
             cmd = runline  # run file
 
         tmp.append(cmd)
 
+        if self.parent.is_parent:
+            tmp.append("\n#### child submission")
+            for line in self._dependency_info["child_submit"]:
+                tmp.append(line)
+
         path = self.jobscript.local
         output = "\n".join(tmp)
         if write_file:
             self._logger.info(f"writing run script to {path}")
             with open(path, "w+") as o:
                 o.write(output)
                 # Make sure the script ends with a line break
```

### Comparing `remotemanager-0.8.2/remotemanager/jupyter/magic.py` & `remotemanager-0.8.3/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/logging/__init__.py` & `remotemanager-0.8.3/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/logging/log.py` & `remotemanager-0.8.3/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/logging/utils.py` & `remotemanager-0.8.3/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/logging/verbosity.py` & `remotemanager-0.8.3/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/serialisation/__init__.py` & `remotemanager-0.8.3/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/serialisation/serial.py` & `remotemanager-0.8.3/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.8.3/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.8.3/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/storage/database.py` & `remotemanager-0.8.3/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/storage/function.py` & `remotemanager-0.8.3/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/storage/remotefunction.py` & `remotemanager-0.8.3/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/storage/sendablemixin.py` & `remotemanager-0.8.3/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/storage/trackedfile.py` & `remotemanager-0.8.3/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/transport/cp.py` & `remotemanager-0.8.3/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/transport/rsync.py` & `remotemanager-0.8.3/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/transport/scp.py` & `remotemanager-0.8.3/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/transport/transport.py` & `remotemanager-0.8.3/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/utils/__init__.py` & `remotemanager-0.8.3/remotemanager/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -181,7 +181,36 @@
             if obj.__class__.__name__ == name:
                 if obj.uuid == uuid:
                     return obj
         except AttributeError:
             pass
 
     raise ValueError(f"could not find {object} in memory with UUID {uuid}")
+
+
+def check_dir_is_child(base: str, test: str) -> bool:
+    """
+    Makes sure that `test` is a child leaf directory than `base`
+
+    Args:
+        base:
+            base directory to test from
+        test:
+            directory to query
+
+    Returns:
+        bool
+    """
+    # make sure we have abspaths for commonprefix
+    base = os.path.abspath(base)
+    test = os.path.abspath(test)
+    # if the paths are equal, return False
+    if base == test:
+        return False
+    # get the common part of the path to remove
+    mix = os.path.commonpath([base, test])
+    # delete the common from both paths
+    diff_neg = base.replace(mix, "").split(os.sep)
+
+    diff_num = 1 - len(diff_neg)
+    print(diff_num)
+    return diff_num >= 0
```

### Comparing `remotemanager-0.8.2/remotemanager/utils/flags.py` & `remotemanager-0.8.3/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager/utils/version.py` & `remotemanager-0.8.3/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.2/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.8.3/remotemanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.8.2
+Version: 0.8.3
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.8.2/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.8.3/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

