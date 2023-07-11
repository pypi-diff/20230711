# Comparing `tmp/airtouch2-0.7.4.tar.gz` & `tmp/airtouch2-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch2-0.7.4.tar", last modified: Mon Jul 10 11:52:51 2023, max compression
+gzip compressed data, was "airtouch2-0.7.5.tar", last modified: Tue Jul 11 11:36:57 2023, max compression
```

## Comparing `airtouch2-0.7.4.tar` & `airtouch2-0.7.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.465098 airtouch2-0.7.4/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7.4/LICENSE
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-07-10 11:52:51.465098 airtouch2-0.7.4/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)      271 2023-01-10 07:31:33.000000 airtouch2-0.7.4/README.md
--rw-r--r--   0 nathan    (1000) nathan    (1000)      852 2023-07-10 11:38:29.000000 airtouch2-0.7.4/pyproject.toml
--rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-07-10 11:52:51.465098 airtouch2-0.7.4/setup.cfg
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.461098 airtouch2-0.7.4/src/
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.461098 airtouch2-0.7.4/src/airtouch2/
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.461098 airtouch2-0.7.4/src/airtouch2/at2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     5511 2023-06-28 10:35:59.000000 airtouch2-0.7.4/src/airtouch2/at2/At2Aircon.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3713 2023-07-10 10:06:21.000000 airtouch2-0.7.4/src/airtouch2/at2/At2Client.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3301 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/at2/At2Group.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      204 2023-07-10 10:42:42.000000 airtouch2-0.7.4/src/airtouch2/at2/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.461098 airtouch2-0.7.4/src/airtouch2/at2plus/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2789 2023-06-28 10:35:27.000000 airtouch2-0.7.4/src/airtouch2/at2plus/At2PlusAircon.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     8229 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/at2plus/At2PlusClient.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      190 2023-07-10 11:17:26.000000 airtouch2-0.7.4/src/airtouch2/at2plus/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.461098 airtouch2-0.7.4/src/airtouch2/common/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2227 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/common/Buffer.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4764 2023-07-10 10:07:01.000000 airtouch2-0.7.4/src/airtouch2/common/NetClient.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/common/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      428 2023-07-09 02:16:01.000000 airtouch2-0.7.4/src/airtouch2/common/interfaces.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.461098 airtouch2-0.7.4/src/airtouch2/helpers/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/helpers/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/helpers/diff_bytes.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.461098 airtouch2-0.7.4/src/airtouch2/protocol/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7.4/src/airtouch2/protocol/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.465098 airtouch2-0.7.4/src/airtouch2/protocol/at2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2584 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/constants.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2773 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/conversions.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      647 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/enums.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/lookups.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      307 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/message_common.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.465098 airtouch2-0.7.4/src/airtouch2/protocol/at2/messages/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/messages/RequestState.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     5046 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/messages/ResponseMessage.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      339 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/messages/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2861 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/messages/ac_commands.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2/messages/group_commands.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.465098 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/constants.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2768 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/control_status_common.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/conversions.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/crc16_modbus.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/enums.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/extended_common.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3941 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/message_common.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.465098 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/messages/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/messages/AcControl.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7.4/src/airtouch2/protocol/at2plus/messages/AcStatus.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-10 11:52:51.461098 airtouch2-0.7.4/src/airtouch2.egg-info/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-07-10 11:52:51.000000 airtouch2-0.7.4/src/airtouch2.egg-info/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1649 2023-07-10 11:52:51.000000 airtouch2-0.7.4/src/airtouch2.egg-info/SOURCES.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-07-10 11:52:51.000000 airtouch2-0.7.4/src/airtouch2.egg-info/dependency_links.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-07-10 11:52:51.000000 airtouch2-0.7.4/src/airtouch2.egg-info/top_level.txt
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.201552 airtouch2-0.7.5/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7.5/LICENSE
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-07-11 11:36:57.201552 airtouch2-0.7.5/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      271 2023-01-10 07:31:33.000000 airtouch2-0.7.5/README.md
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      852 2023-07-11 11:35:30.000000 airtouch2-0.7.5/pyproject.toml
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-07-11 11:36:57.201552 airtouch2-0.7.5/setup.cfg
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     5511 2023-06-28 10:35:59.000000 airtouch2-0.7.5/src/airtouch2/at2/At2Aircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3713 2023-07-10 10:06:21.000000 airtouch2-0.7.5/src/airtouch2/at2/At2Client.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3301 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/at2/At2Group.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      204 2023-07-10 10:42:42.000000 airtouch2-0.7.5/src/airtouch2/at2/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2789 2023-06-28 10:35:27.000000 airtouch2-0.7.5/src/airtouch2/at2plus/At2PlusAircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     8381 2023-07-11 11:17:00.000000 airtouch2-0.7.5/src/airtouch2/at2plus/At2PlusClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      190 2023-07-10 11:17:26.000000 airtouch2-0.7.5/src/airtouch2/at2plus/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/common/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2457 2023-07-11 11:20:25.000000 airtouch2-0.7.5/src/airtouch2/common/Buffer.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4764 2023-07-10 10:07:01.000000 airtouch2-0.7.5/src/airtouch2/common/NetClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/common/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      428 2023-07-09 02:16:01.000000 airtouch2-0.7.5/src/airtouch2/common/interfaces.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/helpers/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/helpers/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/helpers/diff_bytes.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/protocol/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7.5/src/airtouch2/protocol/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/protocol/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2584 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2773 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      647 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/lookups.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      308 2023-07-11 11:17:00.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/RequestState.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     5046 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/ResponseMessage.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      339 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2861 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/ac_commands.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/group_commands.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.201552 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2768 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/control_status_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/crc16_modbus.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/extended_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3942 2023-07-11 11:17:00.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.201552 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcControl.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcStatus.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2.egg-info/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-07-11 11:36:57.000000 airtouch2-0.7.5/src/airtouch2.egg-info/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1649 2023-07-11 11:36:57.000000 airtouch2-0.7.5/src/airtouch2.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-07-11 11:36:57.000000 airtouch2-0.7.5/src/airtouch2.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-07-11 11:36:57.000000 airtouch2-0.7.5/src/airtouch2.egg-info/top_level.txt
```

### Comparing `airtouch2-0.7.4/LICENSE` & `airtouch2-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/PKG-INFO` & `airtouch2-0.7.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.7.4
+Version: 0.7.5
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `airtouch2-0.7.4/pyproject.toml` & `airtouch2-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtouch2"
 description = "API for the monitoring and control of a Polyaire Airtouch 2 system over the local network"
-version = "0.7.4"
+version = "0.7.5"
 authors = [{ name = "Nathan Van der Hoek", email = "nathan.vanderhoek@student.adelaide.edu.au" }]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `airtouch2-0.7.4/src/airtouch2/at2/At2Aircon.py` & `airtouch2-0.7.5/src/airtouch2/at2/At2Aircon.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/at2/At2Client.py` & `airtouch2-0.7.5/src/airtouch2/at2/At2Client.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/at2/At2Group.py` & `airtouch2-0.7.5/src/airtouch2/at2/At2Group.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/at2plus/At2PlusAircon.py` & `airtouch2-0.7.5/src/airtouch2/at2plus/At2PlusAircon.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/at2plus/At2PlusClient.py` & `airtouch2-0.7.5/src/airtouch2/at2plus/At2PlusClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,21 +116,23 @@
         header, header_bytes = await self._read_header()
         buffer = Buffer(header.data_length)
 
         data_bytes = await self._client.read_bytes(header.data_length)
         if not data_bytes:
             # interrupted during data reading
             return None
-        buffer.append_bytes(data_bytes)
+        if not buffer.append_bytes(data_bytes):
+            _LOGGER.warning(
+                f"Received incorrect number of bytes, expected {header.data_length} but received {buffer._head}")
 
         checksum = await self._client.read_bytes(2)
         if not checksum:
             # interrupted during checksum reading
             return None
-        calculated_checksum = crc16(header_bytes[2:] + buffer.data)
+        calculated_checksum = crc16(header_bytes[2:] + buffer._data)
         if (checksum != calculated_checksum):
             _LOGGER.warning(
                 f"Checksum mismatch, ignoring message: Got {checksum.hex(':')}, expected {calculated_checksum.hex(':')}")
             return None
 
         if self._dump_responses:
             # blocks but is only used for dev and debugging
```

### Comparing `airtouch2-0.7.4/src/airtouch2/common/NetClient.py` & `airtouch2-0.7.5/src/airtouch2/common/NetClient.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/helpers/diff_bytes.py` & `airtouch2-0.7.5/src/airtouch2/helpers/diff_bytes.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2/constants.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2/constants.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2/conversions.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2/conversions.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2/enums.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2/enums.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2/lookups.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2/lookups.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2/messages/RequestState.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/RequestState.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2/messages/ResponseMessage.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/ResponseMessage.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2/messages/ac_commands.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/ac_commands.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2/messages/group_commands.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/group_commands.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2plus/control_status_common.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/control_status_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2plus/conversions.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/conversions.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2plus/crc16_modbus.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2plus/enums.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/enums.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2plus/extended_common.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/extended_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2plus/message_common.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/message_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 def prime_message_buffer(header: Header) -> Buffer:
     buffer = Buffer(header.data_length + NON_DATA_LENGTH)
     buffer.append(header)
     return buffer
 
 
 def add_checksum_message_buffer(buffer: Buffer) -> None:
-    buffer.append_bytes(crc16(buffer.data[2:-2]))
+    buffer.append_bytes(crc16(buffer._data[2:-2]))
 
 
 def add_checksum_message_bytes(data: bytearray) -> None:
     checksum = crc16(data[2:-2])
     data[-2] = checksum[0]
     data[-1] = checksum[1]
```

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2plus/messages/AcControl.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcControl.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2/protocol/at2plus/messages/AcStatus.py` & `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcStatus.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.4/src/airtouch2.egg-info/PKG-INFO` & `airtouch2-0.7.5/src/airtouch2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.7.4
+Version: 0.7.5
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `airtouch2-0.7.4/src/airtouch2.egg-info/SOURCES.txt` & `airtouch2-0.7.5/src/airtouch2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

