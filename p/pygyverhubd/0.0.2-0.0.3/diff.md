# Comparing `tmp/pygyverhubd-0.0.2.tar.gz` & `tmp/pygyverhubd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygyverhubd-0.0.2.tar", last modified: Tue Jun 27 07:17:04 2023, max compression
+gzip compressed data, was "pygyverhubd-0.0.3.tar", last modified: Tue Jul 11 16:30:49 2023, max compression
```

## Comparing `pygyverhubd-0.0.2.tar` & `pygyverhubd-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.294826 pygyverhubd-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-27 07:17:04.294826 pygyverhubd-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.286826 pygyverhubd-0.0.2/gyverhubd/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.290826 pygyverhubd-0.0.2/gyverhubd/proto/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/proto/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/proto/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.290826 pygyverhubd-0.0.2/gyverhubd/ui/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.294826 pygyverhubd-0.0.2/gyverhubd/ui/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/controls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/prompt_confirm.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/components/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/ui/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/gyverhubd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:04.294826 pygyverhubd-0.0.2/pygyverhubd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-27 07:17:04.000000 pygyverhubd-0.0.2/pygyverhubd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-27 07:17:04.000000 pygyverhubd-0.0.2/pygyverhubd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:17:04.000000 pygyverhubd-0.0.2/pygyverhubd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 07:17:04.000000 pygyverhubd-0.0.2/pygyverhubd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 07:17:04.000000 pygyverhubd-0.0.2/pygyverhubd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-27 07:16:43.000000 pygyverhubd-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:17:04.294826 pygyverhubd-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.378908 pygyverhubd-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-11 16:30:49.378908 pygyverhubd-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.374907 pygyverhubd-0.0.3/gyverhubd/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.374907 pygyverhubd-0.0.3/gyverhubd/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/cli/new_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/cli/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/device_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.374907 pygyverhubd-0.0.3/gyverhubd/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/mapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/mapped_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/union.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/vfspath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/virtual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/virtual_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.374907 pygyverhubd-0.0.3/gyverhubd/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/proto/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/proto/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/proto/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/proto/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.374907 pygyverhubd-0.0.3/gyverhubd/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.378908 pygyverhubd-0.0.3/gyverhubd/ui/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/prompt_confirm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.378908 pygyverhubd-0.0.3/pygyverhubd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-11 16:30:49.000000 pygyverhubd-0.0.3/pygyverhubd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-11 16:30:49.000000 pygyverhubd-0.0.3/pygyverhubd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:30:49.000000 pygyverhubd-0.0.3/pygyverhubd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 16:30:49.000000 pygyverhubd-0.0.3/pygyverhubd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 16:30:49.000000 pygyverhubd-0.0.3/pygyverhubd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:30:49.378908 pygyverhubd-0.0.3/setup.cfg
```

### Comparing `pygyverhubd-0.0.2/LICENSE` & `pygyverhubd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.2/PKG-INFO` & `pygyverhubd-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygyverhubd
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python implementation of GyverHub device
 Author-email: NekoNekoNyan <me@neko-dev.ru>
 License: MIT License
         
         Copyright (c) 2023 NekoNekoNyan <neko-dev.ru>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,46 +35,44 @@
 License-File: LICENSE
 
 
 # Реализация сервера (устройства) GyverHub на python
 
 ## Проект находится в стадии активной разработки, api может быть изменено без уведомления!
 
-На данный момент работает только WebSocket
-
-Текущая версия клиента - https://github.com/GyverLibs/GyverHub/tree/7dbb3ae82193ef4aa6c43be3a936ae97554a0594
+Текущая версия клиента - https://github.com/GyverLibs/GyverHub/tree/8f81922dd3a19e5e7666789a54b3a08d0334019b
 (кроме передачи файлов по http)
 
-Пример использования [здесь](examples/components_ui.py)
+Пример использования [здесь](examples/ui.py)
 
 # Текущий прогресс
 ## Сеть
 - [x] Интерфейс: WebSocket
-- [ ] Интерфейс: MQTT
+- [x] Интерфейс: MQTT
 - [ ] Интерфейс: Bluetooth
-- [ ] Интерфейс: Serial
+- [x] Интерфейс: Serial
 - [x] Device discovery
 - [ ] Встроенный клиент
 
 ## GUI
 - [x] Базовые компоненты
-- [ ] Canvas
-- [ ] Вкладки
+- [x] Canvas
+- [x] Вкладки
 
 ## Устройство
 - [x] Базовая информация - название, иконка
 - [x] Расширенная информация - сеть, память
 - [ ] Автоматический сбор расширенной информации
 
 ## OTA
 - [x] OTA API
-- [ ] Обновление сервера через OTA
+- [x] Обновление сервера через OTA
 - [ ] Автообновление
-- [ ] Автоматическая упаковка обновлений
+- [x] Автоматическая упаковка обновлений
 
 ## ФС
 - [x] API файловой системы
-- [ ] Отражение API ФС на реальную папку
+- [x] Отражение API ФС на реальную папку
 
 ## Другие компоненты
-- [ ] Перезапуск сервера по команде reboot
+- [x] Перезапуск сервера по команде reboot
 - [x] CLI API
```

### Comparing `pygyverhubd-0.0.2/gyverhubd/device.py` & `pygyverhubd-0.0.3/gyverhubd/device.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,39 @@
+import binascii
+import typing
 from functools import cached_property
 
-from . import Filesystem, response, DeviceUi, Module, DeviceInfo
-from ._version import __version__
+from . import Filesystem, response, DeviceUi, Module, DeviceInfo, __version__, generate_did, EventTarget, request, \
+    server
 
+__all__ = ["Device"]
 
 _FS_COMMANDS = frozenset((
     "fsbr", "format", "rename", "delete",
     "fetch", "fetch_chunk",
     "upload", "upload_chunk"
 ))
 
 
-class Device:
+class Device(EventTarget):
     name: str
-    id: str
+    id: str = None
     prefix: str = "MyDevices"
 
     icon: str = ""
-    pin: int = 0  # TODO
+    pin: typing.Optional[int] = None
     version: str = "0.0.1"
     update_info: str = ""
     update_format: str = "bin"
-    author: str | None = None
+    author: typing.Optional[str] = None
     enable_auto_update: bool = False
-    info: DeviceInfo | None = None
-    fs: Filesystem | None = None
-    ui: DeviceUi | None = None
+    info: typing.Optional[DeviceInfo] = None
+    fs: typing.Optional[Filesystem] = None
+    ui: typing.Optional[DeviceUi] = None
+    ota_parts: tuple = ()  # may contain 'fs' or 'flash'
 
     # Overridable
 
     async def on_focus(self):
         pass
 
     async def on_unfocus(self):
@@ -37,28 +41,40 @@
 
     async def on_cli(self, command: str):
         pass
 
     async def reboot(self):
         raise NotImplementedError()
 
-    async def ota_update(self, part, url: str | None = None, data: bytes | None = None, check_only: bool = False):
+    async def ota_update(self, part: str, data: bytes):
+        raise NotImplementedError()
+
+    async def ota_url(self, part: str, url: str):
         raise NotImplementedError()
 
     async def on_discover(self) -> dict:
-        return dict(name=self.name, icon=self.icon, version=self.update_info, PIN=self.pin, ota_t=self.update_format,
+        h = 0
+        if self.pin is not None:
+            for c in f"{self.pin:0>4}":
+                h = (h << 5) - h + ord(c)
+
+        return dict(name=self.name, icon=self.icon, version=self.update_info, PIN=h, ota_t=self.update_format,
                     max_upl=0xFFFF_FFFF_FFFF_FFFF, modules=self._disabled_modules)
 
     # API
 
     async def send(self, typ, **data):
-        await self.server.send(typ, **data)
+        data['id'] = self.id
+        data['type'] = typ
+        await server.send(data)
 
     async def broadcast(self, typ, **data):
-        await self.server.broadcast(typ, **data)
+        data['id'] = self.id
+        data['type'] = typ
+        await server.send(data, broadcast=True)
 
     async def send_push(self, text: str, *, broadcast=False):
         if broadcast:
             await self.broadcast("push", text=text)
         else:
             await self.send("push", text=text)
 
@@ -86,138 +102,138 @@
     def _disabled_modules(self):
         value = 0
         if self.info is None:
             value |= Module.INFO
         if type(self).reboot == Device.reboot:  # not overrided
             value |= Module.REBOOT
         if type(self).ota_update == Device.ota_update:  # not overrided
-            value |= Module.OTA | Module.OTA_URL
+            value |= Module.OTA
+        if type(self).ota_url == Device.ota_url:  # not overrided
+            value |= Module.OTA_URL
         if self.ui is None:
             value |= Module.SET
         if self.fs is None:
             value |= Module.FSBR | Module.FORMAT | Module.RENAME | Module.DELETE | Module.DOWNLOAD | Module.UPLOAD
         else:
-            fst = type(self.fs)
-            if fst.get_files_info == Filesystem.get_files_info:
-                value |= Module.FSBR
-            if fst.format == Filesystem.format:
-                value |= Module.FORMAT
-            if fst.rename == Filesystem.rename:
-                value |= Module.RENAME
-            if fst.delete == Filesystem.delete:
-                value |= Module.DELETE
-            if fst.get_contents == Filesystem.get_contents:
-                value |= Module.DOWNLOAD
-            if fst.put_contents == Filesystem.put_contents:
-                value |= Module.UPLOAD
+            value |= self.fs.disabled_modules
 
         return value
 
-    def __init__(self, server):
-        self.server = server
+    def __init__(self):
+        super().__init__()
         self._ota_data = self._ota_name = None
+        if self.id is None:
+            self.id = generate_did(type(self))
+
+        self.add_event_listener('discover', self._on_discover)
+        self.add_event_listener('request', self._on_request)
+
+    async def _on_discover(self):
+        data = await self.on_discover()
+        if data is not None:
+            data['type'] = 'discover'
+            data['id'] = self.id
+            await request.respond(data)
+
+    async def _on_request(self):
+        cmd = request.cmd
 
-    async def on_message(self, req, cmd: str, name: str | None):
         if cmd == "ping":
-            await req.respond(response("OK"))
+            await request.respond(response("OK"))
             return
 
         # # UI # #
 
         if cmd == "focus":
-            req.set_focused(True)
+            request.set_focused(True)
             await self.on_focus()
             if self.ui is None:
-                await req.respond(response("ui", controls=[]))
+                await request.respond(response("ui", controls=[]))
             else:
-                await req.respond(await self.ui.on_update())
+                await request.respond(await self.ui.on_update())
             return
 
         if cmd == "unfocus":
-            req.set_focused(False)
+            request.set_focused(False)
             await self.on_unfocus()
             return
 
         if cmd == "set":
             if self.ui is None:
-                await req.respond(response("OK"))
+                await request.respond(response("OK"))
             else:
-                await req.respond(await self.ui.on_ui_event(name, req.value))
+                await request.respond(await self.ui.on_ui_event(request.name, request.value))
             return
 
         # # INFO # #
 
         if cmd == "info":
             if self.info is None:
-                info = dict(versions=dict())
+                info = dict(version=dict(Library=__version__, Firmware=self.version))
             else:
-                info = self.info.to_json()
-
-            info = dict(info)
-            info['version'] = dict(info.get('version', {}))
-            info['version']['Library'] = __version__
-            if self.version:
-                info['version'].setdefault('Firmware', self.version)
-
-            await req.respond(response("info", info=info))
+                info = self.info.to_json(self.version)
+            await request.respond(response("info", info=info))
             return
 
         if cmd == "reboot":
             await self.reboot()
-            await req.respond(response("OK"))
+            await request.respond(response("OK"))
             return
 
         if cmd == "cli":
-            await self.on_cli(req.value)
-            await req.respond(response("OK"))
+            await self.on_cli(request.value)
+            await request.respond(response("OK"))
             return
 
         # # FILESYSTEM # #
 
         if cmd in _FS_COMMANDS:
             if self.fs is None:
-                await req.respond(response("fs_error"))
+                await request.respond(response("fs_error"))
             else:
-                await req.respond(await self.fs.on_message(req, cmd, name))
+                await request.respond(await self.fs.on_message())
             return
 
         # # OTA # #
 
         if cmd == "ota_url":
+            if request.name not in self.ota_parts:
+                await request.respond(response("ERR", text="Cant update this partition"))
+                return
+
             try:
-                await self.ota_update(name, url=req.value)
+                await self.ota_url(request.name, url=request.value)
             except Exception:
-                await req.respond(response("ota_url_err"))
+                await request.respond(response("ota_url_err"))
             else:
-                await req.respond(response("ota_url_ok"))
+                await request.respond(response("ota_url_ok"))
             return
 
         if cmd == "ota":
-            try:
-                await self.ota_update(name, check_only=True)
-            except Exception:
-                await req.respond(response("ota_err"))
-            else:
-                self._ota_name = name
-                self._ota_data = []
-                await req.respond(response("ota_start"))
+            if request.name not in self.ota_parts:
+                await request.respond(response("ERR", text="Cant update this partition"))
+                return
+
+            self._ota_name = request.name
+            self._ota_data = []
+            await request.respond(response("ota_start"))
             return
 
         if cmd == "ota_chunk":
             if self._ota_data is None:
-                await req.respond(response("ota_err"))
+                await request.respond(response("ota_err"))
                 return
 
-            self._ota_data.append(req.value)
+            self._ota_data.append(binascii.a2b_base64(request.value))
 
-            if name == 'next':
-                await req.respond(response("ota_next_chunk"))
+            if request.name == 'next':
+                await request.respond(response("ota_next_chunk"))
                 return
 
             try:
-                await self.ota_update(self._ota_name, data=b''.join(self._ota_data))
+                await self.ota_update(self._ota_name, b''.join(self._ota_data))
             except Exception:
-                await req.respond(response("ota_err"))
+                await request.respond(response("ota_err"))
             else:
                 self._ota_name = self._ota_data = None
-                await req.respond(response("ota_end"))
+                await request.respond(response("ota_end"))
             return
```

### Comparing `pygyverhubd-0.0.2/gyverhubd/info.py` & `pygyverhubd-0.0.3/gyverhubd/info.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,64 @@
 import collections
 import datetime
 import typing
 
+from . import __version__, device
+
+__all__ = ["DeviceInfo"]
+
 
 class DeviceInfo:
-    __slots__ = ('_data', '_handlers', '_device')
+    __slots__ = ('_data', '_handlers')
 
     def __init__(self):
         self._data = dict(version={}, net={}, memory={}, system={})
         self._handlers = collections.defaultdict(list)
-        self._device = None
-
-    def __get__(self, instance, owner=None):
-        if self._device is None:
-            obj = type(self)
-            obj._data = self._data
-            obj._handlers = self._handlers
-            obj._device = instance
-            return obj
-        return self
 
-    def to_json(self) -> dict[str, dict]:
+    def to_json(self, version) -> typing.Dict[str, dict]:
         data = dict(self._data)
         for group, handlers in self._handlers.items():
             for handler in handlers:
-                data[group].update(handler(self._device))
+                data[group].update(handler(device))
+
+        data['version']['Library'] = __version__
+        data['version']['Firmware'] = version
         return data
 
-    def set(self, group: str, name: str, value: str) -> typing.Self:
+    def set(self, group: str, name: str, value: str) -> 'DeviceInfo':
         self._data[group][name] = value
         return self
 
-    def version(self, name: str, value: str) -> typing.Self:
+    def version(self, name: str, value: str) -> 'DeviceInfo':
         return self.set('version', name, value)
 
-    def system(self, name: str, value: str) -> typing.Self:
+    def system(self, name: str, value: str) -> 'DeviceInfo':
         return self.set('system', name, value)
 
-    def network(self, name: str, value: str) -> typing.Self:
+    def network(self, name: str, value: str) -> 'DeviceInfo':
         return self.set('net', name, value)
 
-    def memory(self, name: str, value: str | int, total: int | None = None) -> typing.Self:
+    def memory(self, name: str, value: typing.Union[str, int], total: typing.Optional[int] = None) -> 'DeviceInfo':
         if isinstance(value, (tuple, list)) and total is None:
             value, total = value
         if isinstance(value, int):
             if total is None:
                 total = 0
             value = [value, total]
         else:
             if total is not None:
                 raise TypeError("Argument 'total' must not be set when value is str!")
         return self.set('memory', name, value)
 
-    def uptime(self, value: datetime.timedelta) -> typing.Self:
+    def uptime(self, value: datetime.timedelta) -> 'DeviceInfo':
+        # noinspection PyTypeChecker
         return self.set('system', 'Uptime', value.seconds)
 
     def set_handler(self, group: str, fn: callable):
         self._handlers[group].append(fn)
 
     def handler(self, group: str):
         def _decorator(fn):
             self.set_handler(group, fn)
             return fn
-        return _decorator
 
-    # version: dict[str, str] = dataclasses.field(default_factory=dict)  # Library, Firmware
-    # net: dict[str, str] = dataclasses.field(default_factory=dict)  # Mode, MAC, SSID, RSSI, IP
-    # memory: dict[str, tuple[int, int] | str] = dataclasses.field(default_factory=dict)  # RAM Flash Sketch
-    # system: dict[str, str] = dataclasses.field(default_factory=dict)  # Uptime (int), Model, CPU_Mhz Flash_chip
+        return _decorator
```

### Comparing `pygyverhubd-0.0.2/gyverhubd/proto/proto.py` & `pygyverhubd-0.0.3/gyverhubd/proto/proto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import typing
 
+from gyverhubd import parse_url
 
-MessageHandler = typing.Callable[['Request'], None]
+__all__ = ["Protocol", "Request"]
 
 
 class Protocol:
     focused: bool = False
-    device_id: str | None = None
 
-    def set_handler_message(self, handler: MessageHandler):
+    def bind(self, server):
         raise NotImplementedError()
 
-    async def send(self, data: str):
-        raise NotImplementedError()
-
-    async def start(self):
-        raise NotImplementedError()
-
-    async def stop(self):
+    async def send(self, data: dict):
         raise NotImplementedError()
 
 
 class Request:
-    url: str
-    value: str | None
+    prefix: str
+    clid: typing.Optional[str]
+    did: typing.Optional[str]
+    cmd: typing.Optional[str]
+    name: typing.Optional[str]
+    value: typing.Optional[str]
     protocol: Protocol
 
-    async def respond(self, data: str):
+    def __init__(self, url: str, value: str):
+        self.prefix, self.clid, self.did, self.cmd, self.name = parse_url(url)
+        self.value = value
+
+    async def respond(self, data: dict):
         raise NotImplementedError()
 
     def set_focused(self, value: bool):
         raise NotImplementedError()
```

### Comparing `pygyverhubd-0.0.2/gyverhubd/proto/ws.py` & `pygyverhubd-0.0.3/gyverhubd/proto/mqtt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,101 @@
+import asyncio
 import json
+import os
 import sys
+import typing
 
-from aiohttp import web
-from websockets import server
-from websockets.exceptions import ConnectionClosed
+import aiomqtt
 
-from gyverhubd.proto.proto import Protocol, MessageHandler, Request
+from . import Protocol, Request
 
-PYTHON_VERSION = "{}.{}".format(*sys.version_info)
-SERVER_NAME = f"Python/{PYTHON_VERSION} gyverhubd/0.0.1"
-_FOCUSED_PROP = f'__{__name__.replace(".", "")}_focused'
+__all__ = ["MqttProtocol"]
 
 
-class WSRequest(Request):
-    def __init__(self, protocol, ws, data):
-        self.protocol: WSProtocol = protocol
-        self._ws = ws
+class MqttRequest(Request):
+    def __init__(self, protocol, message: aiomqtt.Message):
+        super().__init__(message.topic.value, message.payload.decode('ascii'))
+        self.protocol: MqttProtocol = protocol
 
-        assert isinstance(data, str) and data and data[-1] == '\0'
-        url, eq, value = data[:-1].partition('=')
-        if not eq:
-            value = None
+        if not self.value:
+            self.value = None
 
-        self.url = url
-        self.value = value
+        if self.cmd is None:
+            self.clid = self.value
+            self.value = None
 
     async def respond(self, data: dict):
-        await self.protocol.send_to(self._ws, data)
+        if self.did is not None:
+            data['id'] = self.did
+        data = '\n' + json.dumps(data) + '\n'
+        await self.protocol.send_to(self, data)
 
     def set_focused(self, value: bool):
-        setattr(self._ws, _FOCUSED_PROP, value)
+        pass
 
 
-class WSProtocol(Protocol):
-    def __init__(self, host="", http_port=80, ws_port=81):
+class MqttProtocol(Protocol):
+    def __init__(self, host: str, port=1883, **kwargs):
         self._host = host
-        self._http_port = http_port
-        self._ws_port = ws_port
+        self._port = port
+        self._client_kwargs = kwargs
 
-        self._clients = {}
-        self._handler: MessageHandler = lambda x: None
-        self._ws_srv = None
-        self._http_srv = None
+        self._client: typing.Optional[aiomqtt.Client] = None
+        self._server = None
+        self._stopped = False
+        self._prefixes = []
 
     @property
     def focused(self) -> bool:
-        return any((getattr(i, _FOCUSED_PROP, False) for i in self._clients.values()))
-
-    def set_handler_message(self, handler):
-        self._handler = handler
+        return False
 
-    async def start(self):
-        self._ws_srv = await server.serve(self._handle_ws, self._host, self._ws_port, subprotocols=["hub"],
-                                          server_header=SERVER_NAME)
-
-        app = web.Application()
-        app.router.add_route('GET', '/hub_discover_all', self._discover_handler)
-        app.router.add_route('GET', '/hub_http_cfg', self._config_handler)
-
-        runner = web.AppRunner(app)
-        await runner.setup()
-        self._http_srv = web.TCPSite(runner, self._host, self._http_port)
-        await self._http_srv.start()
-
-    async def stop(self):
-        await self._http_srv.stop()
-
-        self._ws_srv.close()
-        await self._ws_srv.wait_closed()
-
-    async def _discover_handler(self, _):
-        return web.Response(text="OK", headers={'Access-Control-Allow-Origin': '*'})
-
-    async def _config_handler(self, _):
-        config = dict(upload="0", download="0", ota="0")
-        return web.Response(text=json.dumps(config), headers={'Access-Control-Allow-Origin': '*'})
-
-    async def _handle_ws(self, ws: server.WebSocketServerProtocol):
-        self._clients[ws.remote_address] = ws
-
-        try:
-            while not ws.closed:
-                try:
-                    data = await ws.recv()
-                except ConnectionClosed:
-                    pass
-                else:
-                    self._handler(WSRequest(self, ws, data))
+    def bind(self, server):
+        self._server = server
+        self._prefixes.clear()
+        server.add_event_listener('start', self.__server_start)
+        server.add_event_listener('stop', self.__server_stop)
+
+    async def __server_start(self):
+        self._client = aiomqtt.Client(self._host, self._port, **self._client_kwargs)
+        await self._client.connect()
+        asyncio.ensure_future(self._messages())
+
+        for dev in self._server.devices:
+            await self._client.subscribe(dev.prefix)
+            await self._client.subscribe(f"{dev.prefix}/{dev.id}/#")
+            await self._client.publish(f"{dev.prefix}/hub/{dev.id}/status", b'online')
+            self._prefixes.append(dev.prefix)
+
+    async def _messages(self):
+        async with self._client.messages() as messages:
+            try:
+                async for message in messages:
+                    req = MqttRequest(self, message)
+                    asyncio.ensure_future(self._server.dispatch_event('request', req))
+            except aiomqtt.MqttError as e:
+                if not self._stopped:
+                    raise e
+
+    async def __server_stop(self):
+        for dev in self._server.devices:
+            await self._client.publish(f"{dev.prefix}/hub/{dev.id}/status", b'offline')
 
-        finally:
-            del self._clients[ws.remote_address]
+        self._stopped = True
+        await self._client.disconnect()
 
     async def send(self, data: dict):
-        for i in tuple(self._clients.values()):
-            await self.send_to(i, data)
-
-    async def send_to(self, ws, data: dict):
-        data['id'] = self.device_id
         data = '\n' + json.dumps(data) + '\n'
-        await ws.send(data)
+        for prefix in self._prefixes:
+            await self._client.publish(f"{prefix}/hub", data)
+
+    async def send_to(self, req: MqttRequest, data: str):
+        if req.did is None:
+            await self._client.publish(f"{req.prefix}/hub", data)
+        else:
+            await self._client.publish(f"{req.prefix}/hub/{req.clid}/{req.did}", data)
+
+
+protocol_factory = MqttProtocol
+
+if sys.platform.lower() == "win32" or os.name.lower() == "nt":
+    # fix for aiomqtt
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
```

### Comparing `pygyverhubd-0.0.2/gyverhubd/ui/component.py` & `pygyverhubd-0.0.3/gyverhubd/ui/component.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import enum
 import typing
 
+__all__ = ["Component", "ChangeType"]
+
 
 class ChangeType(enum.Enum):
     NO = enum.auto()
     UPDATE = enum.auto()
     FULL = enum.auto()
 
 
 class Component:
-    __slots__ = ('__changed__', '__data__', '__handlers__', '__layout__')
+    __slots__ = ('__changed__', '__data__', '__handlers__', '__layout__', '__enabled__')
     __type__: str
-    __fields__: tuple[tuple[str, str, typing.Any], ...] = ()
-    __value_field__: tuple[str, str, typing.Any] | None = None
+    __fields__: typing.Tuple[typing.Tuple[str, str, typing.Any], ...] = ()
+    __value_field__: typing.Optional[typing.Tuple[str, str, typing.Any]] = None
 
     __changed__: ChangeType
     __data__: dict
-    __handlers__: list[callable]
+    __handlers__: typing.List[callable]
     __layout__: 'Layout'
+    __enabled__: bool
 
     def __init_subclass__(cls, **kwargs):
         fields = ()
         for i in cls.mro():
             fields += getattr(i, '__fields__', ())
         cls.__fields__ = fields
         return super().__init_subclass__(**kwargs)
@@ -34,22 +37,29 @@
     def __init__(self, label=None, **kwargs):
         self.__data__ = {name: kwargs.get(name, default) for name, json, default in type(self).__fields__}
         if type(self).__value_field__ is not None:
             name, json, default = type(self).__value_field__
             self.__data__[name] = kwargs.get(name, default)
         self.__handlers__ = []
         self.__changed__ = ChangeType.FULL
+        if 'disabled' in kwargs:
+            self.__enabled__ = not kwargs.pop('disabled')
+        else:
+            self.__enabled__ = True
 
         self.name = None
         self.label = label
 
     def to_json(self):
         res = {json: getattr(self, name) for name, json, default in type(self).__fields__}
         res['label'] = '_no' if self.label is None else self.label
         res['name'] = self.name
+        if hasattr(self, 'tab_w'):
+            res['tab_w'] = self.tab_w
+
         res['type'] = type(self).__type__
         if type(self).__value_field__ is not None:
             name, json, default = type(self).__value_field__
             if json is not None:
                 res[json] = self.value2event(getattr(self, name))
         self.__changed__ = ChangeType.NO
         return res
@@ -60,17 +70,19 @@
     def to_update(self):
         if type(self).__value_field__ is None or self.__changed__ != ChangeType.UPDATE:
             return None
         self.__changed__ = ChangeType.NO
         return self.value2event(getattr(self, type(self).__value_field__[0]))
 
     def __setattr__(self, key, value):
-        if key in {'__changed__', '__data__', '__handlers__', '__layout__'}:
+        if key == '__enabled__' and value != getattr(self, key, None):
+            self.__changed__ = ChangeType.FULL
+        if key in {'__changed__', '__data__', '__handlers__', '__layout__', '__enabled__'}:
             return super().__setattr__(key, value)
-        if self.__changed__ != ChangeType.FULL and value != getattr(self, key, None):
+        if self.__changed__ != ChangeType.FULL and value != getattr(self, key, None) and self.__enabled__:
             if type(self).__value_field__ is not None and key == type(self).__value_field__[0]:
                 self.__changed__ = ChangeType.UPDATE
             else:
                 self.__changed__ = ChangeType.FULL
         self.__data__[key] = value
 
     def __getattr__(self, item):
```

### Comparing `pygyverhubd-0.0.2/gyverhubd/ui/components/button.py` & `pygyverhubd-0.0.3/gyverhubd/ui/components/button.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,19 @@
     __value_field__ = ('is_pressed', None, False)
     __fields__ = (
         ('size', 'size', 12),
         ('color', 'color', None)
     )
 
     def pressed(self, fn):
-        self.add_handler(lambda self, value: fn(self) if value == '1' else None)
+        self.add_handler(lambda s, value: fn(s) if value == '1' else None)
         return fn
 
     def released(self, fn):
-        self.add_handler(lambda self, value: fn(self) if value == '0' else None)
+        self.add_handler(lambda s, value: fn(s) if value == '0' else None)
         return fn
 
     clicked = pressed
 
 
 class Button(ButtonBase):
     __type__ = 'button'
```

### Comparing `pygyverhubd-0.0.2/gyverhubd/ui/components/controls.py` & `pygyverhubd-0.0.3/gyverhubd/ui/components/controls.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 from gyverhubd import Component, Color
 
 
 class Select(Component):
     __type__ = "select"
     __value_field__ = ('index', 'value', 0)
     __fields__ = (
@@ -51,9 +53,9 @@
 
     def event2value(self, value: str):
         value = int(value)
         y = (value & 0xFFFF) - 255
         x = (value >> 16) - 255
         return x, y
 
-    def value2event(self, value: tuple[int, int]):
+    def value2event(self, value: typing.Tuple[int, int]):
         return None
```

### Comparing `pygyverhubd-0.0.2/gyverhubd/ui/components/datetime.py` & `pygyverhubd-0.0.3/gyverhubd/ui/components/datetime.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.2/gyverhubd/ui/components/text.py` & `pygyverhubd-0.0.3/gyverhubd/ui/components/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,7 +92,16 @@
         value = int(value)
         x = value >> 16
         y = value & 0xffff
         value = x, y
         self._invoke_handlers(value)
 
     clicked = Component.changed
+
+
+class Table(Component):
+    __type__ = "table"
+    __value_field__ = ('value', 'value', '')
+    __fields__ = (
+        ('align', 'align', ''),
+        ('width', 'width', ''),
+    )
```

### Comparing `pygyverhubd-0.0.2/pygyverhubd.egg-info/PKG-INFO` & `pygyverhubd-0.0.3/pygyverhubd.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygyverhubd
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python implementation of GyverHub device
 Author-email: NekoNekoNyan <me@neko-dev.ru>
 License: MIT License
         
         Copyright (c) 2023 NekoNekoNyan <neko-dev.ru>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,46 +35,44 @@
 License-File: LICENSE
 
 
 # Реализация сервера (устройства) GyverHub на python
 
 ## Проект находится в стадии активной разработки, api может быть изменено без уведомления!
 
-На данный момент работает только WebSocket
-
-Текущая версия клиента - https://github.com/GyverLibs/GyverHub/tree/7dbb3ae82193ef4aa6c43be3a936ae97554a0594
+Текущая версия клиента - https://github.com/GyverLibs/GyverHub/tree/8f81922dd3a19e5e7666789a54b3a08d0334019b
 (кроме передачи файлов по http)
 
-Пример использования [здесь](examples/components_ui.py)
+Пример использования [здесь](examples/ui.py)
 
 # Текущий прогресс
 ## Сеть
 - [x] Интерфейс: WebSocket
-- [ ] Интерфейс: MQTT
+- [x] Интерфейс: MQTT
 - [ ] Интерфейс: Bluetooth
-- [ ] Интерфейс: Serial
+- [x] Интерфейс: Serial
 - [x] Device discovery
 - [ ] Встроенный клиент
 
 ## GUI
 - [x] Базовые компоненты
-- [ ] Canvas
-- [ ] Вкладки
+- [x] Canvas
+- [x] Вкладки
 
 ## Устройство
 - [x] Базовая информация - название, иконка
 - [x] Расширенная информация - сеть, память
 - [ ] Автоматический сбор расширенной информации
 
 ## OTA
 - [x] OTA API
-- [ ] Обновление сервера через OTA
+- [x] Обновление сервера через OTA
 - [ ] Автообновление
-- [ ] Автоматическая упаковка обновлений
+- [x] Автоматическая упаковка обновлений
 
 ## ФС
 - [x] API файловой системы
-- [ ] Отражение API ФС на реальную папку
+- [x] Отражение API ФС на реальную папку
 
 ## Другие компоненты
-- [ ] Перезапуск сервера по команде reboot
+- [x] Перезапуск сервера по команде reboot
 - [x] CLI API
```

### Comparing `pygyverhubd-0.0.2/pyproject.toml` & `pygyverhubd-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -9,28 +9,33 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "aiohttp~=3.8.4",
-    "websockets~=11.0.3"
+    "websockets~=11.0.3",
+    "aiomqtt~=1.0.0",
+    "pycryptodome~=3.18.0",
+    "pyserial-asyncio~=0.6"
 ]
 dynamic = ["version", "readme"]
 
 [project.urls]
 "Homepage" = "https://github.com/neko-neko-nyan/pygyverhubd"
 "Bug Tracker" = "https://github.com/neko-neko-nyan/pygyverhubd/issues"
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "setuptools-git-versioning<2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools-git-versioning]
 enabled = true
+dev_template = "{tag}.post{ccount}"
+dirty_template = "{tag}.post{ccount}+dirty"
 
 [tool.setuptools.packages.find]
 include = ["gyverhubd*"]
 namespaces = false
 
 [tool.setuptools.dynamic]
 readme = {file = "README.md", content-type = "text/markdown"}
```

