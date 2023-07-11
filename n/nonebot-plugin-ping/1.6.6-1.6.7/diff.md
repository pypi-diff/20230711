# Comparing `tmp/nonebot_plugin_ping-1.6.6.tar.gz` & `tmp/nonebot_plugin_ping-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ping-1.6.6.tar", last modified: Sat Apr 22 03:20:28 2023, max compression
+gzip compressed data, was "nonebot_plugin_ping-1.6.7.tar", last modified: Tue Jul 11 01:12:18 2023, max compression
```

## Comparing `nonebot_plugin_ping-1.6.6.tar` & `nonebot_plugin_ping-1.6.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 03:20:28.530537 nonebot_plugin_ping-1.6.6/
--rw-rw-rw-   0        0        0     1088 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.6/LICENSE
--rw-rw-rw-   0        0        0     1659 2023-04-22 03:20:28.530537 nonebot_plugin_ping-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 03:20:28.524021 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping/
--rw-rw-rw-   0        0        0     3837 2023-04-22 03:18:23.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 03:20:28.529137 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/
--rw-rw-rw-   0        0        0     1659 2023-04-22 03:20:28.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-04-22 03:20:28.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 03:20:28.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-22 03:20:28.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-22 03:20:28.000000 nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 03:20:28.530537 nonebot_plugin_ping-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     3944 2023-04-22 03:19:33.000000 nonebot_plugin_ping-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:12:18.411209 nonebot_plugin_ping-1.6.7/
+-rw-rw-rw-   0        0        0     1088 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.7/LICENSE
+-rw-rw-rw-   0        0        0     1659 2023-07-11 01:12:18.410208 nonebot_plugin_ping-1.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 01:12:18.403693 nonebot_plugin_ping-1.6.7/nonebot_plugin_ping/
+-rw-rw-rw-   0        0        0     4242 2023-07-11 01:11:50.000000 nonebot_plugin_ping-1.6.7/nonebot_plugin_ping/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:12:18.409210 nonebot_plugin_ping-1.6.7/nonebot_plugin_ping.egg-info/
+-rw-rw-rw-   0        0        0     1659 2023-07-11 01:12:18.000000 nonebot_plugin_ping-1.6.7/nonebot_plugin_ping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-11 01:12:18.000000 nonebot_plugin_ping-1.6.7/nonebot_plugin_ping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 01:12:18.000000 nonebot_plugin_ping-1.6.7/nonebot_plugin_ping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-11 01:12:18.000000 nonebot_plugin_ping-1.6.7/nonebot_plugin_ping.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-11 01:12:18.000000 nonebot_plugin_ping-1.6.7/nonebot_plugin_ping.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 01:12:18.411209 nonebot_plugin_ping-1.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     3944 2023-07-11 01:12:07.000000 nonebot_plugin_ping-1.6.7/setup.py
```

### Comparing `nonebot_plugin_ping-1.6.6/LICENSE` & `nonebot_plugin_ping-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ping-1.6.6/PKG-INFO` & `nonebot_plugin_ping-1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_ping
-Version: 1.6.6
+Version: 1.6.7
 Summary: ping
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_ping-1.6.6/README.md` & `nonebot_plugin_ping-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ping-1.6.6/nonebot_plugin_ping/__init__.py` & `nonebot_plugin_ping-1.6.7/nonebot_plugin_ping/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,36 @@
-﻿from nonebot.plugin.on import on_command
+﻿﻿from nonebot.plugin.on import on_command
+from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot.params import CommandArg
 from httpx import AsyncClient
 import nonebot
 import asyncio
 import platform
 
 try:
     model: int = nonebot.get_driver().config.ping
 except:
     model: int = 1
 
+__plugin_meta__ = PluginMetadata(
+    name="PING",
+    description="PING/QRCODE/WHOIS",
+    usage=("""
+ping + url: ping 一个网址
+qrcode + url: 给网址生成一个二维码
+whois + url: 查询一个网址的 whois 信息
+"""
+    ),
+    extra={
+        "author": "zhulinyv <zhulinyv2005@outlook.com>",
+        "version": "1.6.6",
+    },
+)
+
 
 
 """PING网址"""
 ping = on_command('ping', aliases={'Ping'}, priority=60, block=True)
 @ping.handle()
 async def _(msg: Message = CommandArg()):
     url = msg.extract_plain_text().strip()
```

### Comparing `nonebot_plugin_ping-1.6.6/nonebot_plugin_ping.egg-info/PKG-INFO` & `nonebot_plugin_ping-1.6.7/nonebot_plugin_ping.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ping
-Version: 1.6.6
+Version: 1.6.7
 Summary: ping
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_ping-1.6.6/setup.py` & `nonebot_plugin_ping-1.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_ping'
 DESCRIPTION = 'ping'
 URL = 'https://github.com/zhulinyv/nonebot_plugin_ping'
 EMAIL = 'zhulinyv2005@outlook.com'
 AUTHOR = '(๑•小丫头片子•๑)'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.6.6'
+VERSION = '1.6.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nonebot2', 'nonebot-adapter-onebot', 'httpx',
 ]
 
 # What packages are optional?
```

