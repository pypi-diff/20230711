# Comparing `tmp/qqbot_linger-0.2.0a1.tar.gz` & `tmp/qqbot_linger-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qqbot_linger-0.2.0a1.tar", max compression
+gzip compressed data, was "qqbot_linger-0.2.1.tar", max compression
```

## Comparing `qqbot_linger-0.2.0a1.tar` & `qqbot_linger-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1081 2023-06-15 15:28:05.364651 qqbot_linger-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-15 14:33:17.187189 qqbot_linger-0.2.0a1/qqbot_linger/__init__.py
--rw-r--r--   0        0        0      429 2023-06-15 15:28:41.514858 qqbot_linger-0.2.0a1/qqbot_linger/main.py
--rw-r--r--   0        0        0      588 2023-06-14 17:38:38.474357 qqbot_linger-0.2.0a1/README.md
--rw-r--r--   0        0        0     1211 2023-06-14 17:38:38.474357 qqbot_linger-0.2.0a1/UNLICENSE
--rw-r--r--   0        0        0     1554 1970-01-01 00:00:00.000000 qqbot_linger-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0      801 2023-06-21 03:57:15.670771 qqbot_linger-0.2.1/README.md
+-rw-r--r--   0        0        0     1211 2023-06-15 09:40:22.667442 qqbot_linger-0.2.1/UNLICENSE
+-rw-r--r--   0        0        0     1075 2023-07-11 06:56:15.751103 qqbot_linger-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-11 06:56:20.804451 qqbot_linger-0.2.1/qqbot_linger/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-21 03:51:41.939913 qqbot_linger-0.2.1/qqbot_linger/main.py
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 qqbot_linger-0.2.1/PKG-INFO
```

### Comparing `qqbot_linger-0.2.0a1/pyproject.toml` & `qqbot_linger-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qqbot-linger"
-version = "0.2.0a1"
+version = "0.2.1"
 description = "My QQ Bot for personal use"
 authors = ["7sDream <i@7sdre.am>"]
 license = "Unlicense"
 readme = "README.md"
 homepage = "https://github.com/7sDream/qqbot-linger"
 repository = "https://github.com/7sDream/qqbot-linger"
 keywords = ["nonebot", "bilibili", "qqbot"]
@@ -20,16 +20,16 @@
     "UNLICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "1.10.9"
 nonebot2 = {extras = ["fastapi"], version = "2.0.0"}
-nonebot-plugin-7s-roll = "^0.2.0a1"
-nonebot-plugin-bam = "^0.2.0a1"
+nonebot-plugin-7s-roll = "^0.2.0"
+nonebot-plugin-bam = "^0.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
 black = "^23.3.0"
 rope = "^1.8.0"
 
 [tool.poetry.scripts]
```

### Comparing `qqbot_linger-0.2.0a1/UNLICENSE` & `qqbot_linger-0.2.1/UNLICENSE`

 * *Files identical despite different names*

### Comparing `qqbot_linger-0.2.0a1/PKG-INFO` & `qqbot_linger-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qqbot-linger
-Version: 0.2.0a1
+Version: 0.2.1
 Summary: My QQ Bot for personal use
 Home-page: https://github.com/7sDream/qqbot-linger
 License: Unlicense
 Keywords: nonebot,bilibili,qqbot
 Author: 7sDream
 Author-email: i@7sdre.am
 Requires-Python: >=3.9,<4.0
@@ -12,16 +12,16 @@
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot-plugin-7s-roll (>=0.2.0a1,<0.3.0)
-Requires-Dist: nonebot-plugin-bam (>=0.2.0a1,<0.3.0)
+Requires-Dist: nonebot-plugin-7s-roll (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot-plugin-bam (>=0.2.1,<0.3.0)
 Requires-Dist: nonebot2[fastapi] (==2.0.0)
 Requires-Dist: pydantic (==1.10.9)
 Project-URL: Repository, https://github.com/7sDream/qqbot-linger
 Description-Content-Type: text/markdown
 
 # 玲儿
 
@@ -35,20 +35,22 @@
 ## 使用
 
 ```bash
 pip install qqbot-linger
 cd /a/path/you/want/store/config/and/database
 vim .env # edit this file, see `.env.sample file` for a example
 
-# Start cqhttp server
-# like go-cqhttp, cqhttp-mirai etc
+# Start a IM Bot Client compatible with OneBot v11 protocol
+# Like go-cqhttp, cqhttp-mirai etc
 
 linger # start the bot
 ```
 
+注意：你需要一个支持连接 OneBot V11 协议的 IM 客户端的具体实现，并将其配置为连接到此机器人的 WS 端口，才能实际使用其功能。
+
 ## 截图
 
 以后再弄。
 
 ## LICENSE
 
 Unlicense.
```

