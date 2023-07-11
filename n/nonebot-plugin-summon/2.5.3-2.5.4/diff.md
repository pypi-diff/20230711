# Comparing `tmp/nonebot_plugin_summon-2.5.3.tar.gz` & `tmp/nonebot_plugin_summon-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_summon-2.5.3.tar", last modified: Fri May 12 15:02:34 2023, max compression
+gzip compressed data, was "nonebot_plugin_summon-2.5.4.tar", last modified: Tue Jul 11 01:13:24 2023, max compression
```

## Comparing `nonebot_plugin_summon-2.5.3.tar` & `nonebot_plugin_summon-2.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 15:02:34.128702 nonebot_plugin_summon-2.5.3/
--rw-rw-rw-   0        0        0     1088 2023-02-17 16:11:24.000000 nonebot_plugin_summon-2.5.3/LICENSE
--rw-rw-rw-   0        0        0     2040 2023-05-12 15:02:34.128702 nonebot_plugin_summon-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1320 2023-02-17 18:30:31.000000 nonebot_plugin_summon-2.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 15:02:34.112663 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon/
--rw-rw-rw-   0        0        0     6795 2023-05-12 14:55:54.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon/__init__.py
--rw-rw-rw-   0        0        0     1166 2023-02-18 13:17:09.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:02:34.117688 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/
--rw-rw-rw-   0        0        0     2040 2023-05-12 15:02:33.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-12 15:02:34.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 15:02:33.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-12 15:02:33.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-12 15:02:33.000000 nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 15:02:34.129712 nonebot_plugin_summon-2.5.3/setup.cfg
--rw-rw-rw-   0        0        0     3954 2023-05-12 15:00:31.000000 nonebot_plugin_summon-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:13:24.644232 nonebot_plugin_summon-2.5.4/
+-rw-rw-rw-   0        0        0     1088 2023-02-17 16:11:24.000000 nonebot_plugin_summon-2.5.4/LICENSE
+-rw-rw-rw-   0        0        0     2040 2023-07-11 01:13:24.644232 nonebot_plugin_summon-2.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1320 2023-02-17 18:30:31.000000 nonebot_plugin_summon-2.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 01:13:24.637699 nonebot_plugin_summon-2.5.4/nonebot_plugin_summon/
+-rw-rw-rw-   0        0        0     7337 2023-06-22 17:21:39.000000 nonebot_plugin_summon-2.5.4/nonebot_plugin_summon/__init__.py
+-rw-rw-rw-   0        0        0     1166 2023-02-18 13:17:09.000000 nonebot_plugin_summon-2.5.4/nonebot_plugin_summon/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:13:24.643228 nonebot_plugin_summon-2.5.4/nonebot_plugin_summon.egg-info/
+-rw-rw-rw-   0        0        0     2040 2023-07-11 01:13:24.000000 nonebot_plugin_summon-2.5.4/nonebot_plugin_summon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-11 01:13:24.000000 nonebot_plugin_summon-2.5.4/nonebot_plugin_summon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 01:13:24.000000 nonebot_plugin_summon-2.5.4/nonebot_plugin_summon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-11 01:13:24.000000 nonebot_plugin_summon-2.5.4/nonebot_plugin_summon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-11 01:13:24.000000 nonebot_plugin_summon-2.5.4/nonebot_plugin_summon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 01:13:24.644232 nonebot_plugin_summon-2.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     3954 2023-07-11 01:13:14.000000 nonebot_plugin_summon-2.5.4/setup.py
```

### Comparing `nonebot_plugin_summon-2.5.3/LICENSE` & `nonebot_plugin_summon-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_summon-2.5.3/PKG-INFO` & `nonebot_plugin_summon-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_summon
-Version: 2.5.3
+Version: 2.5.4
 Summary: Groupmates summoning
 Home-page: https://github.com/zhulinyv/nonebot_plugin_summon
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_summon-2.5.3/README.md` & `nonebot_plugin_summon-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_summon-2.5.3/nonebot_plugin_summon/__init__.py` & `nonebot_plugin_summon-2.5.4/nonebot_plugin_summon/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 ﻿"""导入依赖"""
 import nonebot
 from nonebot.rule import to_me
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 from nonebot.plugin.on import on_command
+from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import Message
 
 from .utils import *
 
-
 try:
     NICKNAME: str = (str(nonebot.get_driver().config.nickname)).replace('{\'', '').replace('\'}', '')
 except:
     NICKNAME: str = "脑积水"
 
+__plugin_meta__ = PluginMetadata(
+    name="群友召唤术",
+    description="让 BOT 帮你召唤群友!",
+    usage=("""
+设置召唤+艾特(或qq号)+昵称: 设置一个召唤群友
+删除召唤+昵称: 删除一个召唤群友
+召唤+昵称: 让机器人帮你叫群友
+召唤列表: 查看已设置的昵称
+戳+昵称+次数(数字): 让机器人戳群友
+"""
+    ),
+    extra={
+        "author": "zhulinyv <zhulinyv2005@outlook.com>",
+        "version": "2.5.3",
+    },
+)
+
+
 
 """获取指令"""
 set_summoning = on_command("设置召唤", aliases={"设置召唤术"}, priority=60, block=True)
 del_summoning = on_command("删除召唤", aliases={"删除召唤术"}, rule=to_me(), priority=60, block=True)
 model_switch = on_command("切换召唤术", aliases={"切换召唤模式"}, rule=to_me(), permission=SUPERUSER, priority=60, block=True)
 list_summoning = on_command("召唤列表", aliases={"查看召唤", "查看召唤术"}, priority=60, block=True)
 summon = on_command("召唤", priority=60, block=True)
```

### Comparing `nonebot_plugin_summon-2.5.3/nonebot_plugin_summon/utils.py` & `nonebot_plugin_summon-2.5.4/nonebot_plugin_summon/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_summon-2.5.3/nonebot_plugin_summon.egg-info/PKG-INFO` & `nonebot_plugin_summon-2.5.4/nonebot_plugin_summon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-summon
-Version: 2.5.3
+Version: 2.5.4
 Summary: Groupmates summoning
 Home-page: https://github.com/zhulinyv/nonebot_plugin_summon
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_summon-2.5.3/setup.py` & `nonebot_plugin_summon-2.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_summon'
 DESCRIPTION = 'Groupmates summoning'
 URL = 'https://github.com/zhulinyv/nonebot_plugin_summon'
 EMAIL = 'zhulinyv2005@outlook.com'
 AUTHOR = '(๑•小丫头片子•๑)'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '2.5.3'
+VERSION = '2.5.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nonebot2', 'nonebot-adapter-onebot'
 ]
 
 # What packages are optional?
```

