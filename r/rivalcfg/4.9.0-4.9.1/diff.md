# Comparing `tmp/rivalcfg-4.9.0.tar.gz` & `tmp/rivalcfg-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivalcfg-4.9.0.tar", last modified: Tue May 30 11:04:20 2023, max compression
+gzip compressed data, was "rivalcfg-4.9.1.tar", last modified: Tue Jul 11 10:50:48 2023, max compression
```

## Comparing `rivalcfg-4.9.0.tar` & `rivalcfg-4.9.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.554217 rivalcfg-4.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21438 2023-05-30 11:04:20.554217 rivalcfg-4.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.538217 rivalcfg-4.9.0/rivalcfg/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/color_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.550217 rivalcfg-4.9.0/rivalcfg/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox3_wireless_wired.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox3_wireless_wireless.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox5_wireless_wired.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox5_wireless_wireless.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox9_wireless_wired.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox9_wireless_wireless.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/kanav2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/kinzuv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/prime_wireless_wired.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/prime_wireless_wireless.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival100.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival110.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival300.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival300s.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival310.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival3_wireless.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival500.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival600.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival650.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival700.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival95.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/sensei310.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/sensei_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/sensei_ten.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.550217 rivalcfg-4.9.0/rivalcfg/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.550217 rivalcfg-4.9.0/rivalcfg/handlers/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/buttons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/buttons/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/buttons/layout_multimedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/buttons/layout_qwerty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/multidpi_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/none.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/range.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/reactive_rgbcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/rgbcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/rgbgradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/rgbgradientv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/mouse_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/udev.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/usbhid.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.542217 rivalcfg-4.9.0/rivalcfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21438 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:04:20.554217 rivalcfg-4.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.554217 rivalcfg-4.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_mouse_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_udev.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_usbhid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:50:48.768059 rivalcfg-4.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21703 2023-07-11 10:50:48.768059 rivalcfg-4.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:50:48.764059 rivalcfg-4.9.1/rivalcfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/color_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:50:48.764059 rivalcfg-4.9.1/rivalcfg/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/aerox3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/aerox3_wireless_wired.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/aerox3_wireless_wireless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/aerox5_wireless_wired.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/aerox5_wireless_wireless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/aerox9_wireless_wired.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/aerox9_wireless_wireless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/kanav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/kinzuv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/prime_wireless_wired.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/prime_wireless_wireless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival300.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival300s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival3_wireless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival600.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival650.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival700.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/rival95.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/sensei310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/sensei_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/devices/sensei_ten.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:50:48.764059 rivalcfg-4.9.1/rivalcfg/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:50:48.764059 rivalcfg-4.9.1/rivalcfg/handlers/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/buttons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/buttons/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/buttons/layout_multimedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/buttons/layout_qwerty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/multidpi_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/reactive_rgbcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/rgbcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/rgbgradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/handlers/rgbgradientv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/mouse_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/udev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/usbhid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/rivalcfg/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:50:48.764059 rivalcfg-4.9.1/rivalcfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21703 2023-07-11 10:50:48.000000 rivalcfg-4.9.1/rivalcfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-11 10:50:48.000000 rivalcfg-4.9.1/rivalcfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:50:48.000000 rivalcfg-4.9.1/rivalcfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 10:50:48.000000 rivalcfg-4.9.1/rivalcfg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 10:50:48.000000 rivalcfg-4.9.1/rivalcfg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 10:50:48.000000 rivalcfg-4.9.1/rivalcfg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:50:48.768059 rivalcfg-4.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:50:48.768059 rivalcfg-4.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/test/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/test/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/test/test_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/test/test_mouse_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/test/test_udev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-11 10:50:44.000000 rivalcfg-4.9.1/test/test_usbhid.py
```

### Comparing `rivalcfg-4.9.0/PKG-INFO` & `rivalcfg-4.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivalcfg
-Version: 4.9.0
+Version: 4.9.1
 Summary: Configure SteelSeries gaming mice
 Home-page: https://github.com/flozz/rivalcfg
 Author: Fabien LOISON
 License: WTFPL
 Project-URL: Source Code, https://github.com/flozz/rivalcfg
 Project-URL: Documentation, https://flozz.github.io/rivalcfg/
 Project-URL: Changelog, https://github.com/flozz/rivalcfg#changelog
@@ -301,14 +301,22 @@
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` that have not been released yet):
 
   * Nothing yet ;)
 
+* **v4.9.1:**
+
+  * Improved device profile generation (@airblast-dev, #211)
+  * Fixed battery level reported at 630% when the mouse is off
+    (@LennardKittner, #187, #212)
+  * Unrecognized arguments error when no device is found (@LennardKittner,
+    #213, #214)
+
 * **v4.9.0:**
 
   * Added Aerox 5 Wireless Destiny 2 Editon support (@flozz, #205)
   * Added Aerox 5 Wireless Diablo IV Edition support (@flozz, #206)
   * Updated HIDAPI to v0.14 to fix a macOS Ventura issue (@flozz, #200)
   * Removed the default lighting option for the Prime mouse (reported not
     working and not needed on this device) (@flozz, #196)
```

### Comparing `rivalcfg-4.9.0/README.rst` & `rivalcfg-4.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -282,14 +282,22 @@
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` that have not been released yet):
 
   * Nothing yet ;)
 
+* **v4.9.1:**
+
+  * Improved device profile generation (@airblast-dev, #211)
+  * Fixed battery level reported at 630% when the mouse is off
+    (@LennardKittner, #187, #212)
+  * Unrecognized arguments error when no device is found (@LennardKittner,
+    #213, #214)
+
 * **v4.9.0:**
 
   * Added Aerox 5 Wireless Destiny 2 Editon support (@flozz, #205)
   * Added Aerox 5 Wireless Diablo IV Edition support (@flozz, #206)
   * Updated HIDAPI to v0.14 to fix a macOS Ventura issue (@flozz, #200)
   * Removed the default lighting option for the Prime mouse (reported not
     working and not needed on this device) (@flozz, #196)
```

### Comparing `rivalcfg-4.9.0/rivalcfg/__init__.py` & `rivalcfg-4.9.1/rivalcfg/__init__.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/__main__.py` & `rivalcfg-4.9.1/rivalcfg/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,43 +47,47 @@
     if is_charging is not None:
         result.append("Charging" if is_charging else "Discharging")
 
     if level is not None:
         result.append("[%-10s] %i %%" % ("=" * int(level / 10), level))
 
     if is_charging is None and level is None:
-        result.append("Unable to get the battery level")
+        result.append("Unable to get the battery level. Is the mouse turned on?")
 
     return " ".join(result)
 
 
 def main(args=sys.argv[1:]):
     # Display a message when no argument given
-    if len(sys.argv) == 1:
+    if not args:
         print("USAGE:\n  rivalcfg --help")
         sys.exit(1)
 
     # On Linux: check udev rules
     _check_linux()
 
     # Try to open a mouse
     mouse = None
     if (
-        "--print-debug" not in sys.argv
-        and "--list" not in sys.argv
-        and "--version" not in sys.argv
-        and "--update-udev" not in sys.argv
-        and "--print-udev" not in sys.argv
+        "--print-debug" not in args
+        and "--list" not in args
+        and "--version" not in args
+        and "--update-udev" not in args
+        and "--print-udev" not in args
     ):
         try:
             mouse = get_first_mouse()
         except IOError as error:
-            if "--help" not in sys.argv and "-h" not in sys.argv:
+            if "--help" not in args and "-h" not in args:
                 raise error
 
+        if not mouse and "--help" not in args and "-h" not in args:
+            print("E: No supported device found.")
+            sys.exit(1)
+
     cli_parser = argparse.ArgumentParser(prog="rivalcfg", epilog=_EPILOG)
     cli.add_main_cli(cli_parser)
 
     if mouse:
         mouse_profile = devices.get_profile(
             vendor_id=mouse.vendor_id,
             product_id=mouse.product_id,
```

### Comparing `rivalcfg-4.9.0/rivalcfg/cli.py` & `rivalcfg-4.9.1/rivalcfg/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     def __call__(self, parser, namespace, value, option_string=None):
         print(udev.generate_rules())
         sys.exit(0)
 
 
 class PrintDebugAction(argparse.Action):
-    """Prints debug informations and exit."""
+    """Prints debug information and exit."""
 
     def __call__(self, parser, namespace, value, option_string=None):
         print(debug.get_debug_info())
         sys.exit(0)
 
 
 def add_main_cli(cli_parser):
@@ -122,15 +122,15 @@
         help="Prints udev rules and exit",
         nargs=0,
         action=PrintUdevRulesAction,
     )
 
     cli_parser.add_argument(
         "--print-debug",
-        help="Prints debug informations and exit",
+        help="Prints debug information and exit",
         nargs=0,
         action=PrintDebugAction,
     )
 
 
 def add_mouse_cli(cli_parser, mouse_profile):
     """Adds the CLI options for the given mouse profile.
```

### Comparing `rivalcfg-4.9.0/rivalcfg/color_helpers.py` & `rivalcfg-4.9.1/rivalcfg/color_helpers.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/debug.py` & `rivalcfg-4.9.1/rivalcfg/debug.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/aerox3.py` & `rivalcfg-4.9.1/rivalcfg/devices/aerox3.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/aerox3_wireless_wired.py` & `rivalcfg-4.9.1/rivalcfg/devices/aerox3_wireless_wired.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/aerox3_wireless_wireless.py` & `rivalcfg-4.9.1/rivalcfg/devices/aerox3_wireless_wireless.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/aerox5_wireless_wired.py` & `rivalcfg-4.9.1/rivalcfg/devices/aerox5_wireless_wired.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/aerox5_wireless_wireless.py` & `rivalcfg-4.9.1/rivalcfg/devices/aerox5_wireless_wireless.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/aerox9_wireless_wired.py` & `rivalcfg-4.9.1/rivalcfg/devices/aerox9_wireless_wired.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/aerox9_wireless_wireless.py` & `rivalcfg-4.9.1/rivalcfg/devices/aerox9_wireless_wireless.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/kanav2.py` & `rivalcfg-4.9.1/rivalcfg/devices/kanav2.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/kinzuv2.py` & `rivalcfg-4.9.1/rivalcfg/devices/kinzuv2.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/prime.py` & `rivalcfg-4.9.1/rivalcfg/devices/prime.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/prime_wireless_wired.py` & `rivalcfg-4.9.1/rivalcfg/devices/prime_wireless_wired.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/prime_wireless_wireless.py` & `rivalcfg-4.9.1/rivalcfg/devices/prime_wireless_wireless.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival100.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival100.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival110.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival110.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival3.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival3.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival300.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival300.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival310.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival310.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival3_wireless.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival3_wireless.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival500.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival500.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival600.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival600.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival650.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival650.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival700.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival700.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/rival95.py` & `rivalcfg-4.9.1/rivalcfg/devices/rival95.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/sensei310.py` & `rivalcfg-4.9.1/rivalcfg/devices/sensei310.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/sensei_raw.py` & `rivalcfg-4.9.1/rivalcfg/devices/sensei_raw.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/devices/sensei_ten.py` & `rivalcfg-4.9.1/rivalcfg/devices/sensei_ten.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/buttons/buttons.py` & `rivalcfg-4.9.1/rivalcfg/handlers/buttons/buttons.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/buttons/layout_multimedia.py` & `rivalcfg-4.9.1/rivalcfg/handlers/buttons/layout_multimedia.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/buttons/layout_qwerty.py` & `rivalcfg-4.9.1/rivalcfg/handlers/buttons/layout_qwerty.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/choice.py` & `rivalcfg-4.9.1/rivalcfg/handlers/choice.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/multidpi_range.py` & `rivalcfg-4.9.1/rivalcfg/handlers/multidpi_range.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/none.py` & `rivalcfg-4.9.1/rivalcfg/handlers/none.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/range.py` & `rivalcfg-4.9.1/rivalcfg/handlers/range.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/reactive_rgbcolor.py` & `rivalcfg-4.9.1/rivalcfg/handlers/reactive_rgbcolor.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/rgbcolor.py` & `rivalcfg-4.9.1/rivalcfg/handlers/rgbcolor.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/rgbgradient.py` & `rivalcfg-4.9.1/rivalcfg/handlers/rgbgradient.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/handlers/rgbgradientv2.py` & `rivalcfg-4.9.1/rivalcfg/handlers/rgbgradientv2.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/helpers.py` & `rivalcfg-4.9.1/rivalcfg/helpers.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/mouse.py` & `rivalcfg-4.9.1/rivalcfg/mouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         """Information about the device battery.
 
         :rtype: dict
         :return: ``{"is_charging": True|False|None, "level": int(0-100)|None}``.
 
         .. NOTE::
 
-           A value of ``None`` means the featue is not supported.
+           A value of ``None`` means the feature is not supported or that the mouse is turned off.
         """
         result = {
             "is_charging": None,
             "level": None,
         }
         if "battery_level" not in self.mouse_profile:
             return result
@@ -161,14 +161,17 @@
 
         try:
             if "level" in self.mouse_profile["battery_level"]:
                 result["level"] = self.mouse_profile["battery_level"]["level"](data)
         except Exception:
             pass
 
+        if result["level"] > 100 or result["level"] < 0:
+            return {"is_charging": None, "level": None}
+
         return result
 
     def reset_settings(self):
         """Sets all settings to their factory default values."""
         for name, setting_info in self.mouse_profile["settings"].items():
             method_name = "set_%s" % name
             method = getattr(self, method_name)
```

### Comparing `rivalcfg-4.9.0/rivalcfg/mouse_settings.py` & `rivalcfg-4.9.1/rivalcfg/mouse_settings.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/udev.py` & `rivalcfg-4.9.1/rivalcfg/udev.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg/usbhid.py` & `rivalcfg-4.9.1/rivalcfg/usbhid.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/rivalcfg.egg-info/PKG-INFO` & `rivalcfg-4.9.1/rivalcfg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivalcfg
-Version: 4.9.0
+Version: 4.9.1
 Summary: Configure SteelSeries gaming mice
 Home-page: https://github.com/flozz/rivalcfg
 Author: Fabien LOISON
 License: WTFPL
 Project-URL: Source Code, https://github.com/flozz/rivalcfg
 Project-URL: Documentation, https://flozz.github.io/rivalcfg/
 Project-URL: Changelog, https://github.com/flozz/rivalcfg#changelog
@@ -301,14 +301,22 @@
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` that have not been released yet):
 
   * Nothing yet ;)
 
+* **v4.9.1:**
+
+  * Improved device profile generation (@airblast-dev, #211)
+  * Fixed battery level reported at 630% when the mouse is off
+    (@LennardKittner, #187, #212)
+  * Unrecognized arguments error when no device is found (@LennardKittner,
+    #213, #214)
+
 * **v4.9.0:**
 
   * Added Aerox 5 Wireless Destiny 2 Editon support (@flozz, #205)
   * Added Aerox 5 Wireless Diablo IV Edition support (@flozz, #206)
   * Updated HIDAPI to v0.14 to fix a macOS Ventura issue (@flozz, #200)
   * Removed the default lighting option for the Prime mouse (reported not
     working and not needed on this device) (@flozz, #196)
```

### Comparing `rivalcfg-4.9.0/rivalcfg.egg-info/SOURCES.txt` & `rivalcfg-4.9.1/rivalcfg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/setup.py` & `rivalcfg-4.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         long_description = open("README.rst", "r").read()
 except Exception as error:
     print("Unable to read the README file: " + str(error))
 
 
 setup(
     name="rivalcfg",
-    version="4.9.0",
+    version="4.9.1",
     description="Configure SteelSeries gaming mice",
     url="https://github.com/flozz/rivalcfg",
     project_urls={
         "Source Code": "https://github.com/flozz/rivalcfg",
         "Documentation": "https://flozz.github.io/rivalcfg/",
         "Changelog": "https://github.com/flozz/rivalcfg#changelog",
         "Issues": "https://github.com/flozz/rivalcfg/issues",
```

### Comparing `rivalcfg-4.9.0/test/test_devices.py` & `rivalcfg-4.9.1/test/test_devices.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/test/test_main.py` & `rivalcfg-4.9.1/test/test_main.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/test/test_mouse.py` & `rivalcfg-4.9.1/test/test_mouse.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/test/test_mouse_settings.py` & `rivalcfg-4.9.1/test/test_mouse_settings.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/test/test_udev.py` & `rivalcfg-4.9.1/test/test_udev.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.9.0/test/test_usbhid.py` & `rivalcfg-4.9.1/test/test_usbhid.py`

 * *Files identical despite different names*

