# Comparing `tmp/nonebot_plugin_easy_group_manager-0.3.1.tar.gz` & `tmp/nonebot_plugin_easy_group_manager-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_easy_group_manager-0.3.1.tar", last modified: Sat Feb 11 07:31:57 2023, max compression
+gzip compressed data, was "nonebot_plugin_easy_group_manager-0.3.2.tar", last modified: Tue Jul 11 01:08:24 2023, max compression
```

## Comparing `nonebot_plugin_easy_group_manager-0.3.1.tar` & `nonebot_plugin_easy_group_manager-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-11 07:31:57.058408 nonebot_plugin_easy_group_manager-0.3.1/
--rw-rw-rw-   0        0        0     1088 2022-12-24 04:11:04.000000 nonebot_plugin_easy_group_manager-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     3404 2023-02-11 07:31:57.058408 nonebot_plugin_easy_group_manager-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2637 2023-01-26 11:31:33.000000 nonebot_plugin_easy_group_manager-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-11 07:31:57.052597 nonebot_plugin_easy_group_manager-0.3.1/nonebot_plugin_easy_group_manager/
--rw-rw-rw-   0        0        0     6260 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.3.1/nonebot_plugin_easy_group_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-11 07:31:57.057401 nonebot_plugin_easy_group_manager-0.3.1/nonebot_plugin_easy_group_manager.egg-info/
--rw-rw-rw-   0        0        0     3404 2023-02-11 07:31:56.000000 nonebot_plugin_easy_group_manager-0.3.1/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-02-11 07:31:56.000000 nonebot_plugin_easy_group_manager-0.3.1/nonebot_plugin_easy_group_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-11 07:31:56.000000 nonebot_plugin_easy_group_manager-0.3.1/nonebot_plugin_easy_group_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-02-11 07:31:56.000000 nonebot_plugin_easy_group_manager-0.3.1/nonebot_plugin_easy_group_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-02-11 07:31:56.000000 nonebot_plugin_easy_group_manager-0.3.1/nonebot_plugin_easy_group_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-11 07:31:57.059406 nonebot_plugin_easy_group_manager-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     3993 2023-02-11 07:30:23.000000 nonebot_plugin_easy_group_manager-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:08:24.651000 nonebot_plugin_easy_group_manager-0.3.2/
+-rw-rw-rw-   0        0        0     1088 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     3468 2023-07-11 01:08:24.649997 nonebot_plugin_easy_group_manager-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2698 2023-02-11 06:14:26.000000 nonebot_plugin_easy_group_manager-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 01:08:24.643487 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager/
+-rw-rw-rw-   0        0        0     6946 2023-07-11 01:02:20.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 01:08:24.648991 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/
+-rw-rw-rw-   0        0        0     3468 2023-07-11 01:08:24.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-11 01:08:24.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 01:08:24.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-11 01:08:24.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-07-11 01:08:24.000000 nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 01:08:24.651000 nonebot_plugin_easy_group_manager-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     3993 2023-07-11 01:07:47.000000 nonebot_plugin_easy_group_manager-0.3.2/setup.py
```

### Comparing `nonebot_plugin_easy_group_manager-0.3.1/LICENSE` & `nonebot_plugin_easy_group_manager-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_easy_group_manager-0.3.1/PKG-INFO` & `nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot_plugin_easy_group_manager
-Version: 0.3.1
+Name: nonebot-plugin-easy-group-manager
+Version: 0.3.2
 Summary: 简易群管，管理员设置新方案
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -26,15 +26,15 @@
 <div align="center">
 
 # nonebot_plugin_easy_group_manager
 ✨女生自用 99 新简易群管✨
 
 </div>
 
-### 📣前言
+### 📣 前言
 
 女生自用 99 新简易群管，管理员设置新方案，BOT 不再必须为群主才能设置管理员。
 
 ## ⭐ 安装
     1.pip install nonebot-plugin-easy-group-manager
     2.nb plugin install nonebot-plugin-easy-group-manager
     3.Download zip
@@ -63,7 +63,11 @@
 1、访问 [https://qun.qq.com/](https://qun.qq.com/), 并使用**群主** QQ 号登录。
 
 2、按 F12 并切换到 网络(Network) 视图。
 
 ![image.png](https://s2.loli.net/2023/01/26/a4lLFwDbJjPmfSE.png)
 
 **skey=** 和 **p_skey=** 后面的内容(**不包括**后面的分号)即为需要的 skey 和 pskey。
+
+## ✨ FUTURE
+
+- [ ] 分群设置不同的 skey 和 pskey
```

### Comparing `nonebot_plugin_easy_group_manager-0.3.1/README.md` & `nonebot_plugin_easy_group_manager-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 <div align="center">
 
 # nonebot_plugin_easy_group_manager
 ✨女生自用 99 新简易群管✨
 
 </div>
 
-### 📣前言
+### 📣 前言
 
 女生自用 99 新简易群管，管理员设置新方案，BOT 不再必须为群主才能设置管理员。
 
 ## ⭐ 安装
     1.pip install nonebot-plugin-easy-group-manager
     2.nb plugin install nonebot-plugin-easy-group-manager
     3.Download zip
@@ -43,8 +43,12 @@
 
 1、访问 [https://qun.qq.com/](https://qun.qq.com/), 并使用**群主** QQ 号登录。
 
 2、按 F12 并切换到 网络(Network) 视图。
 
 ![image.png](https://s2.loli.net/2023/01/26/a4lLFwDbJjPmfSE.png)
 
-**skey=** 和 **p_skey=** 后面的内容(**不包括**后面的分号)即为需要的 skey 和 pskey。
+**skey=** 和 **p_skey=** 后面的内容(**不包括**后面的分号)即为需要的 skey 和 pskey。
+
+## ✨ FUTURE
+
+- [ ] 分群设置不同的 skey 和 pskey
```

### Comparing `nonebot_plugin_easy_group_manager-0.3.1/nonebot_plugin_easy_group_manager/__init__.py` & `nonebot_plugin_easy_group_manager-0.3.2/nonebot_plugin_easy_group_manager/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,42 @@
 """导入依赖"""
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, ActionFailed, Message
 from nonebot.adapters.onebot.v11.permission import GROUP_OWNER, GROUP_ADMIN
+from nonebot.plugin import PluginMetadata
 from nonebot.permission import SUPERUSER
 from nonebot.params import CommandArg
 from nonebot import on_command
 from httpx import AsyncClient
 import nonebot
 import re
 try:
     import ujson as json
 except:
     import json
 
+__plugin_meta__ = PluginMetadata(
+    name="群管",
+    description="简易群管",
+    usage=("""
+设置管理员 + @somebody: 设置一个管理员
+取消管理员 + @somebody: 取消一个管理员
+禁言/口球 + @somebody + 阿拉伯数字: 禁言某人，单位分钟，需要 BOT 为管理员
+解禁 + @somebody: 解除某人禁言，需要 BOT 为管理员
+移出 + @somebody: 移出某人，需要 BOT 为管理员
+移出并拉黑 + @somebody: 移出并拉黑，需要 BOT 为管理员
+"""
+    ),
+    extra={
+        "author": "zhulinyv <zhulinyv2005@outlook.com>",
+        "version": "0.3.1",
+    },
+)
+
+
+
 """导入变量"""
 config = nonebot.get_driver().config
 admin_model: int =  getattr(config, "admin_model", 1)
 skey: str =  getattr(config, "skey", "")
 pskey: str =  getattr(config, "pskey", "")
 
 
@@ -39,15 +60,15 @@
     for owner in member_list:
         if owner['role']=='owner':
             owner_id = owner['user_id']
             break
     # 模式判断
     if admin_model == 1:
         for qid in qid_list:
-            api = f'https://ovooa.com/API/quns/api.php?qq={owner_id}&skey={skey}&pskey={pskey}&group={gid}&uin={qid}&kt=1'
+            api = f'https://ovooa.muban.plus/API/quns/api.php?qq={owner_id}&skey={skey}&pskey={pskey}&group={gid}&uin={qid}&kt=1'
             print(api)
             msg = await admin_api(api)
             await set_admin.send(f"{msg}", at_sender=True)
     elif admin_model == 2:
         for qid in qid_list:
             try:
                 await bot.set_group_admin(group_id=gid, user_id=qid, enable=True)
```

### Comparing `nonebot_plugin_easy_group_manager-0.3.1/nonebot_plugin_easy_group_manager.egg-info/PKG-INFO` & `nonebot_plugin_easy_group_manager-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-easy-group-manager
-Version: 0.3.1
+Name: nonebot_plugin_easy_group_manager
+Version: 0.3.2
 Summary: 简易群管，管理员设置新方案
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -26,15 +26,15 @@
 <div align="center">
 
 # nonebot_plugin_easy_group_manager
 ✨女生自用 99 新简易群管✨
 
 </div>
 
-### 📣前言
+### 📣 前言
 
 女生自用 99 新简易群管，管理员设置新方案，BOT 不再必须为群主才能设置管理员。
 
 ## ⭐ 安装
     1.pip install nonebot-plugin-easy-group-manager
     2.nb plugin install nonebot-plugin-easy-group-manager
     3.Download zip
@@ -63,7 +63,11 @@
 1、访问 [https://qun.qq.com/](https://qun.qq.com/), 并使用**群主** QQ 号登录。
 
 2、按 F12 并切换到 网络(Network) 视图。
 
 ![image.png](https://s2.loli.net/2023/01/26/a4lLFwDbJjPmfSE.png)
 
 **skey=** 和 **p_skey=** 后面的内容(**不包括**后面的分号)即为需要的 skey 和 pskey。
+
+## ✨ FUTURE
+
+- [ ] 分群设置不同的 skey 和 pskey
```

### Comparing `nonebot_plugin_easy_group_manager-0.3.1/setup.py` & `nonebot_plugin_easy_group_manager-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_easy_group_manager'
 DESCRIPTION = '简易群管，管理员设置新方案'
 URL = 'https://github.com/zhulinyv/nonebot_plugin_ping'
 EMAIL = 'zhulinyv2005@outlook.com'
 AUTHOR = '(๑•小丫头片子•๑)'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nonebot2', 'nonebot-adapter-onebot', 'httpx',
 ]
 
 # What packages are optional?
```

