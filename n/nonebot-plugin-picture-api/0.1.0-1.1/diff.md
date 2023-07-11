# Comparing `tmp/nonebot_plugin_picture_api-0.1.0.tar.gz` & `tmp/nonebot_plugin_picture_api-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_picture_api-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_picture_api-1.1.tar", max compression
```

## Comparing `nonebot_plugin_picture_api-0.1.0.tar` & `nonebot_plugin_picture_api-1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-07-11 08:25:30.713103 nonebot_plugin_picture_api-0.1.0/LICENSE
--rw-r--r--   0        0        0     4592 2023-07-11 08:25:30.713103 nonebot_plugin_picture_api-0.1.0/README.md
--rw-r--r--   0        0        0     2586 2023-07-11 08:25:30.713103 nonebot_plugin_picture_api-0.1.0/nonebot_plugin_picture_api/__init__.py
--rw-r--r--   0        0        0     2026 2023-07-11 08:25:30.713103 nonebot_plugin_picture_api-0.1.0/nonebot_plugin_picture_api/config.py
--rw-r--r--   0        0        0      500 2023-07-11 08:25:30.713103 nonebot_plugin_picture_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 nonebot_plugin_picture_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-11 09:10:15.108174 nonebot_plugin_picture_api-1.1/LICENSE
+-rw-r--r--   0        0        0     4592 2023-07-11 09:10:15.108174 nonebot_plugin_picture_api-1.1/README.md
+-rw-r--r--   0        0        0     3539 2023-07-11 09:10:15.108174 nonebot_plugin_picture_api-1.1/nonebot_plugin_picture_api/__init__.py
+-rw-r--r--   0        0        0     2026 2023-07-11 09:10:15.108174 nonebot_plugin_picture_api-1.1/nonebot_plugin_picture_api/config.py
+-rw-r--r--   0        0        0      497 2023-07-11 09:10:15.108174 nonebot_plugin_picture_api-1.1/pyproject.toml
+-rw-r--r--   0        0        0     5150 1970-01-01 00:00:00.000000 nonebot_plugin_picture_api-1.1/PKG-INFO
```

### Comparing `nonebot_plugin_picture_api-0.1.0/LICENSE` & `nonebot_plugin_picture_api-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picture_api-0.1.0/README.md` & `nonebot_plugin_picture_api-1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picture_api-0.1.0/nonebot_plugin_picture_api/__init__.py` & `nonebot_plugin_picture_api-1.1/nonebot_plugin_picture_api/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,38 @@
 from nonebot import get_driver
 from nonebot import on_fullmatch
 from .config import Config
 from nonebot.adapters.onebot.v11 import MessageSegment
 from nonebot.params import Fullmatch
 import httpx
 from random import choice
+from nonebot.plugin import PluginMetadata
 
+__plugin_meta__ = PluginMetadata(
+    name="nonebot-plugin-picture-api",
+    description="一款可以自由增删图片指令和api的插件",
+    usage="配置好后发送相应的指令即可，配置文件在cofig/picture_api_config",
+
+
+    type="application",
+    # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
+
+
+    homepage="https://github.com/Q1351998764/nonebot-plugin-picture-api",
+    # 发布必填。
+
+
+    config=Config,
+    # 插件配置项类，如无需配置可不填写。
+
+
+    supported_adapters={"~onebot.v11"},
+    # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
+    # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
+)
 plugin_config = Config.parse_obj(get_driver().config)
 cmds_config = plugin_config.data
 
 cmds = []
 for i in cmds_config:
     if '|' in i:
         cmds = cmds + (i.split('|'))
```

### Comparing `nonebot_plugin_picture_api-0.1.0/nonebot_plugin_picture_api/config.py` & `nonebot_plugin_picture_api-1.1/nonebot_plugin_picture_api/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picture_api-0.1.0/PKG-INFO` & `nonebot_plugin_picture_api-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-picture-api
-Version: 0.1.0
+Version: 1.1
 Summary: 
 Author: Q1351998764
 Author-email: 57926506+Q1351998764@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3)
-Requires-Dist: nonebot-adapters-onebot (>=2.2.3)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3)
 Requires-Dist: nonebot2 (>=2.0.0)
 Requires-Dist: pydantic (>=1.10.7)
 Requires-Dist: pyyaml (>=6.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-picture-api Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-picture-api Version: 1.1 Summary:
 Author: Q1351998764 Author-email: 57926506+Q1351998764@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.3) Requires-Dist:
-nonebot-adapters-onebot (>=2.2.3) Requires-Dist: nonebot2 (>=2.0.0) Requires-
+nonebot-adapter-onebot (>=2.2.3) Requires-Dist: nonebot2 (>=2.0.0) Requires-
 Dist: pydantic (>=1.10.7) Requires-Dist: pyyaml (>=6.0) Description-Content-
 Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                        # nonebot-plugin-picture-api _â¨
   ä¸æ¬¾å¯ä»¥èªç±å¢å å¾çæä»¤åapiçæä»¶ â¨_ [license] [pypi]
                                    [python]
```

