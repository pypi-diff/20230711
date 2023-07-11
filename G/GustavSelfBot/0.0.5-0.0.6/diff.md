# Comparing `tmp/gustavselfbot-0.0.5.tar.gz` & `tmp/gustavselfbot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gustavselfbot-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gustavselfbot-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gustavselfbot-0.0.5.tar` & `gustavselfbot-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     3185 2023-07-10 21:22:00.617362 gustavselfbot-0.0.5/.gitignore
--rw-r--r--   0        0        0      380 2023-07-10 21:34:48.787151 gustavselfbot-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      205 2023-07-10 20:59:21.677937 gustavselfbot-0.0.5/GustavSelfBot/Commands/Functions/__init__.py
--rw-r--r--   0        0        0     1997 2023-07-10 17:55:43.890956 gustavselfbot-0.0.5/GustavSelfBot/Commands/Functions/__ping__.py
--rw-r--r--   0        0        0     3788 2023-07-10 21:32:30.543724 gustavselfbot-0.0.5/GustavSelfBot/Commands/Functions/__quote__.py
--rw-r--r--   0        0        0     1017 2023-07-10 21:32:30.510390 gustavselfbot-0.0.5/GustavSelfBot/Commands/__commands__.py
--rw-r--r--   0        0        0      126 2023-07-10 20:59:21.681270 gustavselfbot-0.0.5/GustavSelfBot/Commands/__init__.py
--rw-r--r--   0        0        0      276 2023-07-10 20:59:21.691270 gustavselfbot-0.0.5/GustavSelfBot/Events/__init__.py
--rw-r--r--   0        0        0     1679 2023-07-10 21:49:04.191223 gustavselfbot-0.0.5/GustavSelfBot/Events/__on_message__.py
--rw-r--r--   0        0        0      184 2023-07-10 18:12:52.724373 gustavselfbot-0.0.5/GustavSelfBot/Events/__on_ready__.py
--rw-r--r--   0        0        0     4233 2023-07-10 21:32:30.503723 gustavselfbot-0.0.5/GustavSelfBot/Events/__on_voice_state_update__.py
--rw-r--r--   0        0        0      655 2023-07-10 21:32:30.520390 gustavselfbot-0.0.5/GustavSelfBot/__bot__.py
--rw-r--r--   0        0        0      265 2023-07-10 21:07:11.012427 gustavselfbot-0.0.5/GustavSelfBot/__config__.py
--rw-r--r--   0        0        0      633 2023-07-10 21:55:07.906734 gustavselfbot-0.0.5/GustavSelfBot/__init__.py
--rw-r--r--   0        0        0     1489 2023-07-10 21:07:11.009094 gustavselfbot-0.0.5/GustavSelfBot/__logging__.py
--rw-r--r--   0        0        0        0 2023-07-10 21:15:47.984536 gustavselfbot-0.0.5/LICENSE
--rw-r--r--   0        0        0      707 2023-07-10 21:55:07.903400 gustavselfbot-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.5/_chatlogs/PLACEHOLDER
--rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.5/_recordings/PLACEHOLDER
--rw-r--r--   0        0        0       87 2023-07-10 12:32:13.422010 gustavselfbot-0.0.5/config.json
--rw-r--r--   0        0        0      246 2023-07-10 21:49:04.177889 gustavselfbot-0.0.5/main.py
--rw-r--r--   0        0        0      613 2023-07-10 21:32:16.773381 gustavselfbot-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       48 2023-07-10 21:31:18.695261 gustavselfbot-0.0.5/requirements.txt
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 gustavselfbot-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3185 2023-07-10 21:22:00.617362 gustavselfbot-0.0.6/.gitignore
+-rw-r--r--   0        0        0      380 2023-07-10 21:34:48.787151 gustavselfbot-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      204 2023-07-11 12:19:26.566571 gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/__init__.py
+-rw-r--r--   0        0        0      536 2023-07-11 12:17:58.120362 gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/__ping__.py
+-rw-r--r--   0        0        0     2338 2023-07-11 12:19:26.576571 gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/__quote__.py
+-rw-r--r--   0        0        0     2019 2023-07-11 12:14:55.350254 gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/helpers/__embed__.py
+-rw-r--r--   0        0        0      151 2023-07-11 12:19:26.583238 gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/helpers/__init__.py
+-rw-r--r--   0        0        0     1017 2023-07-10 21:32:30.510390 gustavselfbot-0.0.6/GustavSelfBot/Commands/__commands__.py
+-rw-r--r--   0        0        0      126 2023-07-10 20:59:21.681270 gustavselfbot-0.0.6/GustavSelfBot/Commands/__init__.py
+-rw-r--r--   0        0        0      276 2023-07-10 20:59:21.691270 gustavselfbot-0.0.6/GustavSelfBot/Events/__init__.py
+-rw-r--r--   0        0        0     1679 2023-07-10 21:49:04.191223 gustavselfbot-0.0.6/GustavSelfBot/Events/__on_message__.py
+-rw-r--r--   0        0        0      184 2023-07-10 18:12:52.724373 gustavselfbot-0.0.6/GustavSelfBot/Events/__on_ready__.py
+-rw-r--r--   0        0        0     4233 2023-07-10 21:32:30.503723 gustavselfbot-0.0.6/GustavSelfBot/Events/__on_voice_state_update__.py
+-rw-r--r--   0        0        0      655 2023-07-10 21:32:30.520390 gustavselfbot-0.0.6/GustavSelfBot/__bot__.py
+-rw-r--r--   0        0        0      265 2023-07-10 21:07:11.012427 gustavselfbot-0.0.6/GustavSelfBot/__config__.py
+-rw-r--r--   0        0        0      633 2023-07-11 12:21:38.110246 gustavselfbot-0.0.6/GustavSelfBot/__init__.py
+-rw-r--r--   0        0        0     1489 2023-07-10 21:07:11.009094 gustavselfbot-0.0.6/GustavSelfBot/__logging__.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:15:47.984536 gustavselfbot-0.0.6/LICENSE
+-rw-r--r--   0        0        0      707 2023-07-10 21:55:07.903400 gustavselfbot-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.6/_chatlogs/PLACEHOLDER
+-rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.6/_recordings/PLACEHOLDER
+-rw-r--r--   0        0        0       87 2023-07-10 12:32:13.422010 gustavselfbot-0.0.6/config.json
+-rw-r--r--   0        0        0      246 2023-07-10 21:49:04.177889 gustavselfbot-0.0.6/main.py
+-rw-r--r--   0        0        0      613 2023-07-10 21:32:16.773381 gustavselfbot-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-07-10 21:31:18.695261 gustavselfbot-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 gustavselfbot-0.0.6/PKG-INFO
```

### Comparing `gustavselfbot-0.0.5/.gitignore` & `gustavselfbot-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.5/GustavSelfBot/Commands/__commands__.py` & `gustavselfbot-0.0.6/GustavSelfBot/Commands/__commands__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.5/GustavSelfBot/Events/__on_message__.py` & `gustavselfbot-0.0.6/GustavSelfBot/Events/__on_message__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.5/GustavSelfBot/Events/__on_voice_state_update__.py` & `gustavselfbot-0.0.6/GustavSelfBot/Events/__on_voice_state_update__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.5/GustavSelfBot/__bot__.py` & `gustavselfbot-0.0.6/GustavSelfBot/__bot__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.5/GustavSelfBot/__init__.py` & `gustavselfbot-0.0.6/GustavSelfBot/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 My self bot!
 Current implementation of GustavSelfBot includes chat logs and commands.
 TODO: make custom command and hooks possible
 """
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 import os
 
 from GustavSelfBot.__logging__ import *
 from GustavSelfBot.__config__ import Config
 from GustavSelfBot.__bot__ import bot
```

### Comparing `gustavselfbot-0.0.5/GustavSelfBot/__logging__.py` & `gustavselfbot-0.0.6/GustavSelfBot/__logging__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.5/README.md` & `gustavselfbot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.5/pyproject.toml` & `gustavselfbot-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.5/PKG-INFO` & `gustavselfbot-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GustavSelfBot
-Version: 0.0.5
+Version: 0.0.6
 Summary: My self bot!
 Author-email: Gustavo Schip <gustavoschip@proton.me>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: discord.py-self[voice]
 Requires-Dist: aiohttp
```

