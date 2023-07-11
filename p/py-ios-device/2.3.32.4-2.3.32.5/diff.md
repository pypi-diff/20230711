# Comparing `tmp/py_ios_device-2.3.32.4.tar.gz` & `tmp/py_ios_device-2.3.32.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ios_device-2.3.32.4.tar", last modified: Fri Jun 16 01:58:43 2023, max compression
+gzip compressed data, was "py_ios_device-2.3.32.5.tar", last modified: Tue Jul 11 11:49:00 2023, max compression
```

## Comparing `py_ios_device-2.3.32.4.tar` & `py_ios_device-2.3.32.5.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.118786 py_ios_device-2.3.32.4/
--rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/LICENSE
--rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/MANIFEST.in
--rw-r--r--   0 rongcloud   (501) staff       (20)    11417 2023-06-16 01:58:43.118579 py_ios_device-2.3.32.4/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)    10950 2023-05-24 02:33:49.000000 py_ios_device-2.3.32.4/README.md
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.102994 py_ios_device-2.3.32.4/demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/demo/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/demo/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 py_ios_device-2.3.32.4/demo/installation_proxy.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.106148 py_ios_device-2.3.32.4/demo/instrument_demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/instrument_demo/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/instrument_demo/activity.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.4/demo/instrument_demo/app_lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/instrument_demo/applictionListing.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.4/demo/instrument_demo/channel.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.4/demo/instrument_demo/coreprofilesessiontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.4/demo/instrument_demo/coreprofilesessiontap_parse.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.4/demo/instrument_demo/deviceinfo.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.4/demo/instrument_demo/energy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-05-08 09:42:27.000000 py_ios_device-2.3.32.4/demo/instrument_demo/gpu.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.4/demo/instrument_demo/graphics.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.4/demo/instrument_demo/launchAPP.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 py_ios_device-2.3.32.4/demo/instrument_demo/mobileNotifications.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.4/demo/instrument_demo/netstatPID.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.4/demo/instrument_demo/networking.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.4/demo/instrument_demo/sysmontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/instrument_demo/xcuitest.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/demo/mobile_config.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/demo/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/demo/syslog.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.106753 py_ios_device-2.3.32.4/ios_device/
--rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)       25 2023-06-16 01:58:41.000000 py_ios_device-2.3.32.4/ios_device/__version__.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.108377 py_ios_device-2.3.32.4/ios_device/cli/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/cli/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    31554 2023-05-24 02:44:13.000000 py_ios_device-2.3.32.4/ios_device/cli/base.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-04-07 02:33:45.000000 py_ios_device-2.3.32.4/ios_device/cli/cli.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    19122 2023-05-24 02:30:31.000000 py_ios_device-2.3.32.4/ios_device/cli/instruments.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11223 2023-04-26 06:21:46.000000 py_ios_device-2.3.32.4/ios_device/cli/mobile.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/main.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.4/ios_device/py_ios_device.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.112736 py_ios_device-2.3.32.4/ios_device/servers/
--rw-r--r--   0 rongcloud   (501) staff       (20)     7287 2023-04-26 03:35:04.000000 py_ios_device-2.3.32.4/ios_device/servers/Installation.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.4/ios_device/servers/Instrument.py
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/servers/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/amfi.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      993 2023-05-22 06:59:19.000000 py_ios_device-2.3.32.4/ios_device/servers/diagnostics_relay.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.4/ios_device/servers/dvt.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 py_ios_device-2.3.32.4/ios_device/servers/house_arrest.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/image_mounter.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 py_ios_device-2.3.32.4/ios_device/servers/mc_install.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/notification_proxy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-04-20 02:31:19.000000 py_ios_device-2.3.32.4/ios_device/servers/os_trace.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 py_ios_device-2.3.32.4/ios_device/servers/simulate_location.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 py_ios_device-2.3.32.4/ios_device/servers/spring_board.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 py_ios_device-2.3.32.4/ios_device/servers/syslog.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-04-17 09:44:17.000000 py_ios_device-2.3.32.4/ios_device/servers/testmanagerd.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.117568 py_ios_device-2.3.32.4/ios_device/util/
--rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/util/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/util/api_util.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 py_ios_device-2.3.32.4/ios_device/util/bpylist2.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/util/ca.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/util/constants.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2023-06-16 01:57:52.000000 py_ios_device-2.3.32.4/ios_device/util/dtx_msg.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/util/exceptions.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/util/forward.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 py_ios_device-2.3.32.4/ios_device/util/gpu_decode.py
--rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.4/ios_device/util/kc_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.4/ios_device/util/kperf_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.4/ios_device/util/lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 py_ios_device-2.3.32.4/ios_device/util/lockdown.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/util/plist_service.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2023-04-26 02:45:02.000000 py_ios_device-2.3.32.4/ios_device/util/plistlib.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 py_ios_device-2.3.32.4/ios_device/util/usbmux.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     9547 2023-06-16 01:52:25.000000 py_ios_device-2.3.32.4/ios_device/util/utils.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 py_ios_device-2.3.32.4/ios_device/util/variables.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.118376 py_ios_device-2.3.32.4/py_ios_device.egg-info/
--rw-r--r--   0 rongcloud   (501) staff       (20)    11417 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)     2406 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/SOURCES.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/dependency_links.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/entry_points.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/requires.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       16 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/top_level.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.4/requirements.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-06-16 01:58:43.118836 py_ios_device-2.3.32.4/setup.cfg
--rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.4/setup.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      958 2023-05-24 02:53:19.000000 py_ios_device-2.3.32.4/setup2.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-07-11 11:49:00.104325 py_ios_device-2.3.32.5/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/LICENSE
+-rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/MANIFEST.in
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11417 2023-07-11 11:49:00.104123 py_ios_device-2.3.32.5/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)    10950 2023-05-24 02:33:49.000000 py_ios_device-2.3.32.5/README.md
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-07-11 11:49:00.087429 py_ios_device-2.3.32.5/demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/demo/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.5/demo/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.5/demo/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 py_ios_device-2.3.32.5/demo/installation_proxy.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-07-11 11:49:00.091402 py_ios_device-2.3.32.5/demo/instrument_demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/demo/instrument_demo/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/demo/instrument_demo/activity.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.5/demo/instrument_demo/app_lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/demo/instrument_demo/applictionListing.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.5/demo/instrument_demo/channel.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.5/demo/instrument_demo/coreprofilesessiontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.5/demo/instrument_demo/coreprofilesessiontap_parse.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-07-11 11:46:22.000000 py_ios_device-2.3.32.5/demo/instrument_demo/deviceinfo.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.5/demo/instrument_demo/energy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-07-11 11:46:22.000000 py_ios_device-2.3.32.5/demo/instrument_demo/gpu.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.5/demo/instrument_demo/graphics.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-07-11 11:46:22.000000 py_ios_device-2.3.32.5/demo/instrument_demo/launchAPP.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1188 2023-06-21 09:40:35.000000 py_ios_device-2.3.32.5/demo/instrument_demo/leaks.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 py_ios_device-2.3.32.5/demo/instrument_demo/mobileNotifications.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.5/demo/instrument_demo/netstatPID.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-07-11 11:46:22.000000 py_ios_device-2.3.32.5/demo/instrument_demo/networking.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-06-28 11:51:15.000000 py_ios_device-2.3.32.5/demo/instrument_demo/sysmontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/demo/instrument_demo/xcuitest.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.5/demo/mobile_config.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/demo/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.5/demo/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.5/demo/syslog.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-07-11 11:49:00.092136 py_ios_device-2.3.32.5/ios_device/
+-rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/ios_device/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)       25 2023-07-11 11:48:58.000000 py_ios_device-2.3.32.5/ios_device/__version__.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-07-11 11:49:00.093513 py_ios_device-2.3.32.5/ios_device/cli/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/ios_device/cli/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    31682 2023-07-11 11:43:58.000000 py_ios_device-2.3.32.5/ios_device/cli/base.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-06-28 10:07:29.000000 py_ios_device-2.3.32.5/ios_device/cli/cli.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    19129 2023-07-11 11:29:38.000000 py_ios_device-2.3.32.5/ios_device/cli/instruments.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11238 2023-07-11 11:47:18.000000 py_ios_device-2.3.32.5/ios_device/cli/mobile.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/ios_device/main.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.5/ios_device/py_ios_device.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-07-11 11:49:00.097826 py_ios_device-2.3.32.5/ios_device/servers/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7287 2023-04-26 03:35:04.000000 py_ios_device-2.3.32.5/ios_device/servers/Installation.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.5/ios_device/servers/Instrument.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/ios_device/servers/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2023-07-11 11:27:10.000000 py_ios_device-2.3.32.5/ios_device/servers/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.5/ios_device/servers/amfi.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2023-06-28 10:07:29.000000 py_ios_device-2.3.32.5/ios_device/servers/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      993 2023-07-11 11:27:10.000000 py_ios_device-2.3.32.5/ios_device/servers/diagnostics_relay.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.5/ios_device/servers/dvt.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-06-28 10:07:29.000000 py_ios_device-2.3.32.5/ios_device/servers/house_arrest.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2023-06-28 10:07:29.000000 py_ios_device-2.3.32.5/ios_device/servers/image_mounter.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-06-28 10:07:29.000000 py_ios_device-2.3.32.5/ios_device/servers/mc_install.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.5/ios_device/servers/notification_proxy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-06-28 10:07:29.000000 py_ios_device-2.3.32.5/ios_device/servers/os_trace.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.5/ios_device/servers/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2023-06-28 10:07:29.000000 py_ios_device-2.3.32.5/ios_device/servers/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 py_ios_device-2.3.32.5/ios_device/servers/simulate_location.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 py_ios_device-2.3.32.5/ios_device/servers/spring_board.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 py_ios_device-2.3.32.5/ios_device/servers/syslog.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-06-28 10:07:29.000000 py_ios_device-2.3.32.5/ios_device/servers/testmanagerd.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-07-11 11:49:00.102849 py_ios_device-2.3.32.5/ios_device/util/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/ios_device/util/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.5/ios_device/util/api_util.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 py_ios_device-2.3.32.5/ios_device/util/bpylist2.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/ios_device/util/ca.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/ios_device/util/constants.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2023-06-16 01:57:52.000000 py_ios_device-2.3.32.5/ios_device/util/dtx_msg.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/ios_device/util/exceptions.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.5/ios_device/util/forward.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-07-07 08:52:08.000000 py_ios_device-2.3.32.5/ios_device/util/gpu_decode.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.5/ios_device/util/kc_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.5/ios_device/util/kperf_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.5/ios_device/util/lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 py_ios_device-2.3.32.5/ios_device/util/lockdown.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.5/ios_device/util/plist_service.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2023-04-26 02:45:02.000000 py_ios_device-2.3.32.5/ios_device/util/plistlib.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 py_ios_device-2.3.32.5/ios_device/util/usbmux.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     9547 2023-06-16 02:01:06.000000 py_ios_device-2.3.32.5/ios_device/util/utils.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 py_ios_device-2.3.32.5/ios_device/util/variables.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-07-11 11:49:00.103910 py_ios_device-2.3.32.5/py_ios_device.egg-info/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11417 2023-07-11 11:49:00.000000 py_ios_device-2.3.32.5/py_ios_device.egg-info/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2436 2023-07-11 11:49:00.000000 py_ios_device-2.3.32.5/py_ios_device.egg-info/SOURCES.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-07-11 11:49:00.000000 py_ios_device-2.3.32.5/py_ios_device.egg-info/dependency_links.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-07-11 11:49:00.000000 py_ios_device-2.3.32.5/py_ios_device.egg-info/entry_points.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-07-11 11:49:00.000000 py_ios_device-2.3.32.5/py_ios_device.egg-info/requires.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       16 2023-07-11 11:49:00.000000 py_ios_device-2.3.32.5/py_ios_device.egg-info/top_level.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.5/requirements.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-07-11 11:49:00.104370 py_ios_device-2.3.32.5/setup.cfg
+-rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.5/setup.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      958 2023-05-24 02:53:19.000000 py_ios_device-2.3.32.5/setup2.py
```

### Comparing `py_ios_device-2.3.32.4/LICENSE` & `py_ios_device-2.3.32.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/PKG-INFO` & `py_ios_device-2.3.32.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ios_device
-Version: 2.3.32.4
+Version: 2.3.32.5
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 Maintainer: chenpeijie
 Maintainer-email: 
 License: UNKNOWN
```

### Comparing `py_ios_device-2.3.32.4/README.md` & `py_ios_device-2.3.32.5/README.md`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/afc.py` & `py_ios_device-2.3.32.5/demo/afc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/crash_log.py` & `py_ios_device-2.3.32.5/demo/crash_log.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/installation_proxy.py` & `py_ios_device-2.3.32.5/demo/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/activity.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/activity.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/app_lifecycle.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/app_lifecycle.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/applictionListing.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/applictionListing.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/coreprofilesessiontap.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/coreprofilesessiontap.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/coreprofilesessiontap_parse.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/coreprofilesessiontap_parse.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/deviceinfo.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/deviceinfo.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/gpu.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/gpu.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/graphics.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/graphics.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/launchAPP.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/launchAPP.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/mobileNotifications.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/mobileNotifications.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/netstatPID.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/netstatPID.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/networking.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/networking.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/sysmontap.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/sysmontap.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/instrument_demo/xcuitest.py` & `py_ios_device-2.3.32.5/demo/instrument_demo/xcuitest.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/mobile_config.py` & `py_ios_device-2.3.32.5/demo/mobile_config.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/pcapd.py` & `py_ios_device-2.3.32.5/demo/pcapd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/screenshotr.py` & `py_ios_device-2.3.32.5/demo/screenshotr.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/demo/syslog.py` & `py_ios_device-2.3.32.5/demo/syslog.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/cli/base.py` & `py_ios_device-2.3.32.5/ios_device/cli/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,18 +248,20 @@
         Get the list of installed applications; 获取已安装应用列表
         @param bundle_id:  bundle id
         @return:
         """
         applist = self.instruments.call(InstrumentsService.ApplicationListing,
                                         "installedApplicationsMatching:registerUpdateToken:",
                                         {}, "").selector
-        if bundle_id:
+        if bundle_id is not None:
             for app in applist:
                 if app.get('CFBundleIdentifier') == bundle_id:
                     return app
+            else:
+                return None
         return applist
 
     def sysmontap(self,
                   callback: callable,
                   time: int = 1000,
                   stopSignal: threading.Event = threading.Event(),
                   system_attributes=None,
@@ -275,17 +277,19 @@
         """
         config = {
             'ur': time,
             'bm': 0,
             'cpuUsage': True,
             'sampleInterval': time * 1000000}
         _system_attributes = self.system_attributes or system_attributes
-        config['sysAttrs'] = _system_attributes
+        if _system_attributes:
+            config['sysAttrs'] = _system_attributes
         process_attributes = self.process_attributes or process_attributes
-        config['procAttrs'] = process_attributes
+        if process_attributes:
+            config['procAttrs'] = process_attributes
         self.instruments.call(InstrumentsService.Sysmontap, "setConfig:", config)
         self.instruments.register_channel_callback(InstrumentsService.Sysmontap, callback)
         self.instruments.call(InstrumentsService.Sysmontap, "start")
         log.info(f'Sysmontap start ...')
         log.info(f'wait for data ...')
         while not stopSignal.wait(1):
             pass
```

### Comparing `py_ios_device-2.3.32.4/ios_device/cli/cli.py` & `py_ios_device-2.3.32.5/ios_device/cli/cli.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/cli/instruments.py` & `py_ios_device-2.3.32.5/ios_device/cli/instruments.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
 
 @instruments.command('appmonitor', cls=Command)
 @click.option('-t', '--time', type=click.INT, default=1000, help='Output interval time (ms)')
 @click.option('-b', '--bundle_id', required=True, help='Process app bundleId to filter')
 def cmd_appmonitor(udid, network, format, time, bundle_id):
     """ Get application performance data """
-    proc_filter = ['Pid','Name', 'CPU', 'Memory','DiskReads','DiskWrites','Threads']
+    proc_filter = ['Pid', 'Name', 'CPU', 'Memory', 'DiskReads', 'DiskWrites', 'Threads']
     process_attributes = dataclasses.make_dataclass('SystemProcessAttributes', proc_filter)
     ios_version = 0
 
     def on_callback_message(res):
         if isinstance(res.selector, list):
             for index, row in enumerate(res.selector):
                 if 'Processes' in row:
@@ -178,16 +178,16 @@
                         attrs.Memory = convertBytes(attrs.Memory)
                         attrs.DiskReads = convertBytes(attrs.DiskReads)
                         attrs.DiskWrites = convertBytes(attrs.DiskWrites)
                         print_json(attrs.__dict__, format)
 
     with InstrumentsBase(udid=udid, network=network) as rpc:
         ios_version = rpc.lockdown.ios_version
-        rpc.process_attributes = ['pid','name', 'cpuUsage', 'physFootprint',
-                                  'diskBytesRead','diskBytesWritten','threadCount']
+        rpc.process_attributes = ['pid', 'name', 'cpuUsage', 'physFootprint',
+                                  'diskBytesRead', 'diskBytesWritten', 'threadCount']
         if bundle_id:
             app = rpc.application_listing(bundle_id)
             if not app:
                 print(f"not find {bundle_id}")
                 return
             name = app.get('ExecutableName')
         rpc.sysmontap(on_callback_message, time)
```

### Comparing `py_ios_device-2.3.32.4/ios_device/cli/mobile.py` & `py_ios_device-2.3.32.5/ios_device/cli/mobile.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     crash_server = CrashLogService(udid=udid, network=network, logger=log)
     crash_server.shell()
 
 
 #######################################################################
 
 @cli.command('sandbox', cls=Command)
-@click.option('-b', '--bundle_id', default=None, help='Process app bundleId to filter')
+@click.option('-b', '--bundle_id', default=None, help='Process app bundleId to filter', required=True)
 @click.option('-a', '--access_type', default='VendDocuments', type=click.Choice(['VendDocuments', 'VendContainer']),
               help='Type of access sandbox')
 def sandbox(udid, network, format, bundle_id, access_type):
     """ open an AFC shell for given bundle_id, assuming its profile is installed """
     HouseArrestService(udid=udid, network=network, logger=log).shell(bundle_id, cmd=access_type)
```

### Comparing `py_ios_device-2.3.32.4/ios_device/py_ios_device.py` & `py_ios_device-2.3.32.5/ios_device/py_ios_device.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/Installation.py` & `py_ios_device-2.3.32.5/ios_device/servers/Installation.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/Instrument.py` & `py_ios_device-2.3.32.5/ios_device/servers/Instrument.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/afc.py` & `py_ios_device-2.3.32.5/ios_device/servers/afc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/amfi.py` & `py_ios_device-2.3.32.5/ios_device/servers/amfi.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/crash_log.py` & `py_ios_device-2.3.32.5/ios_device/servers/crash_log.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/diagnostics_relay.py` & `py_ios_device-2.3.32.5/ios_device/servers/diagnostics_relay.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/dvt.py` & `py_ios_device-2.3.32.5/ios_device/servers/dvt.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/house_arrest.py` & `py_ios_device-2.3.32.5/ios_device/servers/house_arrest.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/image_mounter.py` & `py_ios_device-2.3.32.5/ios_device/servers/image_mounter.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/mc_install.py` & `py_ios_device-2.3.32.5/ios_device/servers/mc_install.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/notification_proxy.py` & `py_ios_device-2.3.32.5/ios_device/servers/notification_proxy.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/os_trace.py` & `py_ios_device-2.3.32.5/ios_device/servers/os_trace.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/pcapd.py` & `py_ios_device-2.3.32.5/ios_device/servers/pcapd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/screenshotr.py` & `py_ios_device-2.3.32.5/ios_device/servers/screenshotr.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/simulate_location.py` & `py_ios_device-2.3.32.5/ios_device/servers/simulate_location.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/spring_board.py` & `py_ios_device-2.3.32.5/ios_device/servers/spring_board.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/syslog.py` & `py_ios_device-2.3.32.5/ios_device/servers/syslog.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/servers/testmanagerd.py` & `py_ios_device-2.3.32.5/ios_device/servers/testmanagerd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/__init__.py` & `py_ios_device-2.3.32.5/ios_device/util/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/api_util.py` & `py_ios_device-2.3.32.5/ios_device/util/api_util.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/bpylist2.py` & `py_ios_device-2.3.32.5/ios_device/util/bpylist2.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/ca.py` & `py_ios_device-2.3.32.5/ios_device/util/ca.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/constants.py` & `py_ios_device-2.3.32.5/ios_device/util/constants.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/dtx_msg.py` & `py_ios_device-2.3.32.5/ios_device/util/dtx_msg.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/exceptions.py` & `py_ios_device-2.3.32.5/ios_device/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/forward.py` & `py_ios_device-2.3.32.5/ios_device/util/forward.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/gpu_decode.py` & `py_ios_device-2.3.32.5/ios_device/util/gpu_decode.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/kc_data.py` & `py_ios_device-2.3.32.5/ios_device/util/kc_data.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/kperf_data.py` & `py_ios_device-2.3.32.5/ios_device/util/kperf_data.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/lifecycle.py` & `py_ios_device-2.3.32.5/ios_device/util/lifecycle.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/lockdown.py` & `py_ios_device-2.3.32.5/ios_device/util/lockdown.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/plist_service.py` & `py_ios_device-2.3.32.5/ios_device/util/plist_service.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/plistlib.py` & `py_ios_device-2.3.32.5/ios_device/util/plistlib.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/usbmux.py` & `py_ios_device-2.3.32.5/ios_device/util/usbmux.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/utils.py` & `py_ios_device-2.3.32.5/ios_device/util/utils.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/ios_device/util/variables.py` & `py_ios_device-2.3.32.5/ios_device/util/variables.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/py_ios_device.egg-info/PKG-INFO` & `py_ios_device-2.3.32.5/py_ios_device.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ios-device
-Version: 2.3.32.4
+Version: 2.3.32.5
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 Maintainer: chenpeijie
 Maintainer-email: 
 License: UNKNOWN
```

### Comparing `py_ios_device-2.3.32.4/py_ios_device.egg-info/SOURCES.txt` & `py_ios_device-2.3.32.5/py_ios_device.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 demo/instrument_demo/coreprofilesessiontap.py
 demo/instrument_demo/coreprofilesessiontap_parse.py
 demo/instrument_demo/deviceinfo.py
 demo/instrument_demo/energy.py
 demo/instrument_demo/gpu.py
 demo/instrument_demo/graphics.py
 demo/instrument_demo/launchAPP.py
+demo/instrument_demo/leaks.py
 demo/instrument_demo/mobileNotifications.py
 demo/instrument_demo/netstatPID.py
 demo/instrument_demo/networking.py
 demo/instrument_demo/sysmontap.py
 demo/instrument_demo/xcuitest.py
 ios_device/__init__.py
 ios_device/__version__.py
```

### Comparing `py_ios_device-2.3.32.4/setup.py` & `py_ios_device-2.3.32.5/setup.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.4/setup2.py` & `py_ios_device-2.3.32.5/setup2.py`

 * *Files identical despite different names*

