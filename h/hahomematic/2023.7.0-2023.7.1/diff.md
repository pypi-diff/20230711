# Comparing `tmp/hahomematic-2023.7.0.tar.gz` & `tmp/hahomematic-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.7.0.tar", last modified: Fri Jul  7 13:16:51 2023, max compression
+gzip compressed data, was "hahomematic-2023.7.1.tar", last modified: Tue Jul 11 11:07:04 2023, max compression
```

## Comparing `hahomematic-2023.7.0.tar` & `hahomematic-2023.7.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.464514 hahomematic-2023.7.0/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.468515 hahomematic-2023.7.0/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    50689 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    46635 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.468515 hahomematic-2023.7.0/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.468515 hahomematic-2023.7.0/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34412 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.468515 hahomematic-2023.7.0/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-07 13:16:50.000000 hahomematic-2023.7.0/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-07 13:16:51.000000 hahomematic-2023.7.0/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:16:50.000000 hahomematic-2023.7.0/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:16:49.000000 hahomematic-2023.7.0/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-07 13:16:51.000000 hahomematic-2023.7.0/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 13:16:51.000000 hahomematic-2023.7.0/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.373333 hahomematic-2023.7.1/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.373333 hahomematic-2023.7.1/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52761 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46789 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.373333 hahomematic-2023.7.1/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34412 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.373333 hahomematic-2023.7.1/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-11 11:07:03.000000 hahomematic-2023.7.1/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-11 11:07:04.000000 hahomematic-2023.7.1/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:07:03.000000 hahomematic-2023.7.1/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:07:02.000000 hahomematic-2023.7.1/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 11:07:04.000000 hahomematic-2023.7.1/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 11:07:04.000000 hahomematic-2023.7.1/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/setup.cfg
```

### Comparing `hahomematic-2023.7.0/LICENSE` & `hahomematic-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/PKG-INFO` & `hahomematic-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.0/README.md` & `hahomematic-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/__init__.py` & `hahomematic-2023.7.1/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/backport.py` & `hahomematic-2023.7.1/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/caches/dynamic.py` & `hahomematic-2023.7.1/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/caches/persistent.py` & `hahomematic-2023.7.1/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/caches/visibility.py` & `hahomematic-2023.7.1/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/central_unit.py` & `hahomematic-2023.7.1/hahomematic/central_unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from hahomematic.caches.visibility import ParameterVisibilityCache
 from hahomematic.const import (
     ATTR_INTERFACE_ID,
     ATTR_TYPE,
     ATTR_VALUE,
     DEFAULT_TLS,
     DEFAULT_VERIFY_TLS,
+    EVENT_PONG,
     HH_EVENT_DELETE_DEVICES,
     HH_EVENT_DEVICES_CREATED,
     HH_EVENT_LIST_DEVICES,
     HH_EVENT_NEW_DEVICES,
     HM_ADDRESS,
     IF_PRIMARY,
     LOCAL_INTERFACE,
@@ -84,14 +85,18 @@
 
 
 class CentralUnit:
     """Central unit that collects everything to handle communication from/to CCU/Homegear."""
 
     def __init__(self, central_config: CentralConfig) -> None:
         """Init the central unit."""
+        self._ping_count: Final[dict[str, int]] = {}
+        self._ping_pong_error_logged: bool = False
+        self._sema_ping_count: Final = threading.Semaphore()
+
         self._sema_add_devices: Final = asyncio.Semaphore()
         self._tasks: Final[set[asyncio.Future[Any]]] = set()
         # Keep the config for the central #CC
         self.config: Final = central_config
         self._attr_name: Final = central_config.name
         self._attr_model: str | None = None
         self._connection_state: Final = central_config.connection_state
@@ -738,15 +743,17 @@
             str(value),
         )
         if not self.has_client(interface_id=interface_id):
             return
 
         self.last_events[interface_id] = datetime.now()
         # No need to check the response of a XmlRPC-PING
-        if parameter == "PONG":
+        if parameter == EVENT_PONG:
+            if value == interface_id:
+                self._reduce_ping_count(interface_id=interface_id)
             return
         if (channel_address, parameter) in self._entity_event_subscriptions:
             try:
                 for callback in self._entity_event_subscriptions[(channel_address, parameter)]:
                     callback(value)
             except RuntimeError as rte:  # pragma: no cover
                 _LOGGER.debug(
@@ -821,14 +828,50 @@
         ):
             del self._entity_event_subscriptions[(entity.channel_address, entity.parameter)]
 
     def has_entity(self, unique_identifier: str) -> bool:
         """Check if unique_identifier is already added."""
         return unique_identifier in self._entities
 
+    def increase_ping_count(self, interface_id: str) -> None:
+        """Increase the number of send ping events."""
+        with self._sema_ping_count:
+            if (ping_count := self._ping_count.get(interface_id)) is not None:
+                ping_count += 1
+                self._ping_count[interface_id] = ping_count
+                if ping_count > 5:
+                    self._log_ping_pong_error_once()
+                _LOGGER.debug("Increase Ping count: %s, %i", interface_id, ping_count)
+            else:
+                self._ping_count[interface_id] = 1
+
+    def _reduce_ping_count(self, interface_id: str) -> None:
+        """Reduce the number of send ping events, by a received pong event."""
+        with self._sema_ping_count:
+            if (ping_count := self._ping_count.get(interface_id)) is not None:
+                ping_count -= 1
+                self._ping_count[interface_id] = ping_count
+                if ping_count < -5:
+                    self._log_ping_pong_error_once()
+                _LOGGER.debug("Reduce Ping count: %s, %i", interface_id, ping_count)
+            else:
+                self._ping_count[interface_id] = 0
+
+    def _log_ping_pong_error_once(self) -> None:
+        """Log an error about the ping/pong count mismatch."""
+        if self._ping_pong_error_logged:
+            return
+        _LOGGER.error(
+            "There is a mismatch between send ping events and received pong events for HA instance %s. "
+            "Looks like you are running multiple instances of HA with the same instance name configured for this integration. "
+            "Re-add one instance! Otherwise one HA instance will not receive update events from your CCU.",
+            self.config.name,
+        )
+        self._ping_pong_error_logged = True
+
     def create_task(self, target: Awaitable, name: str) -> None:
         """Add task to the executor pool."""
         try:
             self._loop.call_soon_threadsafe(self._async_create_task, target, name)
         except CancelledError:
             _LOGGER.debug(
                 "create_task: task cancelled for %s",
```

### Comparing `hahomematic-2023.7.0/hahomematic/client.py` & `hahomematic-2023.7.1/hahomematic/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -691,14 +691,15 @@
             )
 
     async def check_connection_availability(self) -> bool:
         """Check if _proxy is still initialized."""
         try:
             await self._proxy.ping(self.interface_id)
             self.last_updated = datetime.now()
+            self.central.increase_ping_count(interface_id=self.interface_id)
             return True
         except BaseHomematicException as hhe:
             _LOGGER.debug("CHECK_CONNECTION_AVAILABILITY failed: %s [%s]", hhe.name, hhe.args)
         self.last_updated = INIT_DATETIME
         return False
 
     async def execute_program(self, pid: str) -> bool:
@@ -796,14 +797,15 @@
                 )
 
     async def check_connection_availability(self) -> bool:
         """Check if proxy is still initialized."""
         try:
             await self._proxy.clientServerInitialized(self.interface_id)
             self.last_updated = datetime.now()
+            self.central.increase_ping_count(interface_id=self.interface_id)
             return True
         except BaseHomematicException as hhe:
             _LOGGER.debug("CHECK_CONNECTION_AVAILABILITY failed: %s [%s]", hhe.name, hhe.args)
         self.last_updated = INIT_DATETIME
         return False
 
     async def execute_program(self, pid: str) -> bool:
```

### Comparing `hahomematic-2023.7.0/hahomematic/const.py` & `hahomematic-2023.7.1/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/decorators.py` & `hahomematic-2023.7.1/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/exceptions.py` & `hahomematic-2023.7.1/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/exporter.py` & `hahomematic-2023.7.1/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/hmcli.py` & `hahomematic-2023.7.1/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/json_rpc_client.py` & `hahomematic-2023.7.1/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/__init__.py` & `hahomematic-2023.7.1/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/const.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/light.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/support.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.7.1/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/device.py` & `hahomematic-2023.7.1/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/entity.py` & `hahomematic-2023.7.1/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/event.py` & `hahomematic-2023.7.1/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.7.1/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/generic/action.py` & `hahomematic-2023.7.1/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.7.1/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/generic/button.py` & `hahomematic-2023.7.1/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.7.1/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/generic/number.py` & `hahomematic-2023.7.1/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/generic/select.py` & `hahomematic-2023.7.1/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.7.1/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.7.1/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.7.1/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.7.1/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/hub/button.py` & `hahomematic-2023.7.1/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.7.1/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/hub/number.py` & `hahomematic-2023.7.1/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/hub/select.py` & `hahomematic-2023.7.1/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.7.1/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/hub/text.py` & `hahomematic-2023.7.1/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/support.py` & `hahomematic-2023.7.1/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/platforms/update.py` & `hahomematic-2023.7.1/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.7.1/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.7.1/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.7.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/support.py` & `hahomematic-2023.7.1/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.7.1/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic/xml_rpc_server.py` & `hahomematic-2023.7.1/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.7.1/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.0/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.7.1/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.0/pyproject.toml` & `hahomematic-2023.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.7.0"
+version     = "2023.7.1"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Home Automation",
 ]
 requires-python = ">=3.10.0"
 dependencies    = [
     "aiohttp>=3.8.4",
-    "orjson>=3.8.7",
+    "orjson>=3.9.1",
     "python-slugify>=4.0.1",
     "voluptuous>=0.13.1",
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/danielperna84/hahomematic"
 "Bug Reports" = "https://github.com/danielperna84/hahomematic/issues"
```

