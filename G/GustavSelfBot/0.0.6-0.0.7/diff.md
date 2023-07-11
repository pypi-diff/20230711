# Comparing `tmp/gustavselfbot-0.0.6.tar.gz` & `tmp/gustavselfbot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gustavselfbot-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gustavselfbot-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gustavselfbot-0.0.6.tar` & `gustavselfbot-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     3185 2023-07-10 21:22:00.617362 gustavselfbot-0.0.6/.gitignore
--rw-r--r--   0        0        0      380 2023-07-10 21:34:48.787151 gustavselfbot-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      204 2023-07-11 12:19:26.566571 gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/__init__.py
--rw-r--r--   0        0        0      536 2023-07-11 12:17:58.120362 gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/__ping__.py
--rw-r--r--   0        0        0     2338 2023-07-11 12:19:26.576571 gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/__quote__.py
--rw-r--r--   0        0        0     2019 2023-07-11 12:14:55.350254 gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/helpers/__embed__.py
--rw-r--r--   0        0        0      151 2023-07-11 12:19:26.583238 gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/helpers/__init__.py
--rw-r--r--   0        0        0     1017 2023-07-10 21:32:30.510390 gustavselfbot-0.0.6/GustavSelfBot/Commands/__commands__.py
--rw-r--r--   0        0        0      126 2023-07-10 20:59:21.681270 gustavselfbot-0.0.6/GustavSelfBot/Commands/__init__.py
--rw-r--r--   0        0        0      276 2023-07-10 20:59:21.691270 gustavselfbot-0.0.6/GustavSelfBot/Events/__init__.py
--rw-r--r--   0        0        0     1679 2023-07-10 21:49:04.191223 gustavselfbot-0.0.6/GustavSelfBot/Events/__on_message__.py
--rw-r--r--   0        0        0      184 2023-07-10 18:12:52.724373 gustavselfbot-0.0.6/GustavSelfBot/Events/__on_ready__.py
--rw-r--r--   0        0        0     4233 2023-07-10 21:32:30.503723 gustavselfbot-0.0.6/GustavSelfBot/Events/__on_voice_state_update__.py
--rw-r--r--   0        0        0      655 2023-07-10 21:32:30.520390 gustavselfbot-0.0.6/GustavSelfBot/__bot__.py
--rw-r--r--   0        0        0      265 2023-07-10 21:07:11.012427 gustavselfbot-0.0.6/GustavSelfBot/__config__.py
--rw-r--r--   0        0        0      633 2023-07-11 12:21:38.110246 gustavselfbot-0.0.6/GustavSelfBot/__init__.py
--rw-r--r--   0        0        0     1489 2023-07-10 21:07:11.009094 gustavselfbot-0.0.6/GustavSelfBot/__logging__.py
--rw-r--r--   0        0        0        0 2023-07-10 21:15:47.984536 gustavselfbot-0.0.6/LICENSE
--rw-r--r--   0        0        0      707 2023-07-10 21:55:07.903400 gustavselfbot-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.6/_chatlogs/PLACEHOLDER
--rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.6/_recordings/PLACEHOLDER
--rw-r--r--   0        0        0       87 2023-07-10 12:32:13.422010 gustavselfbot-0.0.6/config.json
--rw-r--r--   0        0        0      246 2023-07-10 21:49:04.177889 gustavselfbot-0.0.6/main.py
--rw-r--r--   0        0        0      613 2023-07-10 21:32:16.773381 gustavselfbot-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       48 2023-07-10 21:31:18.695261 gustavselfbot-0.0.6/requirements.txt
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 gustavselfbot-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3185 2023-07-10 21:22:00.617362 gustavselfbot-0.0.7/.gitignore
+-rw-r--r--   0        0        0      380 2023-07-10 21:34:48.787151 gustavselfbot-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      336 2023-07-11 17:07:43.799643 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__init__.py
+-rw-r--r--   0        0        0     2127 2023-07-11 17:17:09.656597 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__logs__.py
+-rw-r--r--   0        0        0      578 2023-07-11 14:00:16.016242 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__ping__.py
+-rw-r--r--   0        0        0     2379 2023-07-11 14:00:16.006242 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__quote__.py
+-rw-r--r--   0        0        0     2524 2023-07-11 17:17:09.649930 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__search__.py
+-rw-r--r--   0        0        0     2030 2023-07-11 14:00:15.989575 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/helpers/__embed__.py
+-rw-r--r--   0        0        0      151 2023-07-11 12:19:26.583238 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/helpers/__init__.py
+-rw-r--r--   0        0        0     1824 2023-07-11 17:07:43.812977 gustavselfbot-0.0.7/GustavSelfBot/Commands/__commands__.py
+-rw-r--r--   0        0        0      140 2023-07-11 17:07:43.826310 gustavselfbot-0.0.7/GustavSelfBot/Commands/__init__.py
+-rw-r--r--   0        0        0      276 2023-07-10 20:59:21.691270 gustavselfbot-0.0.7/GustavSelfBot/Events/__init__.py
+-rw-r--r--   0        0        0     2160 2023-07-11 18:27:30.654611 gustavselfbot-0.0.7/GustavSelfBot/Events/__on_message__.py
+-rw-r--r--   0        0        0      195 2023-07-11 14:00:15.999575 gustavselfbot-0.0.7/GustavSelfBot/Events/__on_ready__.py
+-rw-r--r--   0        0        0     4255 2023-07-11 14:00:16.009575 gustavselfbot-0.0.7/GustavSelfBot/Events/__on_voice_state_update__.py
+-rw-r--r--   0        0        0      657 2023-07-11 16:32:51.605685 gustavselfbot-0.0.7/GustavSelfBot/__bot__.py
+-rw-r--r--   0        0        0      265 2023-07-10 21:07:11.012427 gustavselfbot-0.0.7/GustavSelfBot/__config__.py
+-rw-r--r--   0        0        0      633 2023-07-11 20:08:55.098294 gustavselfbot-0.0.7/GustavSelfBot/__init__.py
+-rw-r--r--   0        0        0     1489 2023-07-10 21:07:11.009094 gustavselfbot-0.0.7/GustavSelfBot/__logging__.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:15:47.984536 gustavselfbot-0.0.7/LICENSE
+-rw-r--r--   0        0        0      707 2023-07-10 21:55:07.903400 gustavselfbot-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.7/_chatlogs/PLACEHOLDER
+-rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.7/_recordings/PLACEHOLDER
+-rw-r--r--   0        0        0       87 2023-07-10 12:32:13.422010 gustavselfbot-0.0.7/config.json
+-rw-r--r--   0        0        0      246 2023-07-10 21:49:04.177889 gustavselfbot-0.0.7/main.py
+-rw-r--r--   0        0        0      613 2023-07-10 21:32:16.773381 gustavselfbot-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-07-10 21:31:18.695261 gustavselfbot-0.0.7/requirements.txt
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 gustavselfbot-0.0.7/PKG-INFO
```

### Comparing `gustavselfbot-0.0.6/.gitignore` & `gustavselfbot-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/__quote__.py` & `gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__quote__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import aiohttp
 import discord
 from discord.ext import commands
 
+from GustavSelfBot import log
 from GustavSelfBot.Commands.Functions.helpers import embed
 
 
+@log.catch
 async def func_quote(bot: commands.Bot, ctx: commands.Context, message: discord.Message):
     async with aiohttp.ClientSession() as session:
         try:
             async with session.get(
                     url="https://clashy-besi.ddns.net/api/quote",
                     headers={"Accept": "application/json"},
             ) as resp:
```

### Comparing `gustavselfbot-0.0.6/GustavSelfBot/Commands/Functions/helpers/__embed__.py` & `gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/helpers/__embed__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import urllib.parse
 
 from GustavSelfBot import log
 
 
+@log.catch
 async def embed(
         author: str, title: str, description: str, color: str, redirect: str
 ) -> str:
     encoded_title = urllib.parse.quote(title)
     encoded_author = urllib.parse.quote(author)
     encoded_description = urllib.parse.quote(description)
     encoded_color = urllib.parse.quote(color)
```

### Comparing `gustavselfbot-0.0.6/GustavSelfBot/Events/__on_message__.py` & `gustavselfbot-0.0.7/GustavSelfBot/Events/__on_message__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 from datetime import datetime
 
 import discord
 from discord.ext import commands
 
-from GustavSelfBot.Commands import quote, ping
+from GustavSelfBot.Commands import quote, ping, logs, search
 from GustavSelfBot import log, os
 
 
 timestamp = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
 
 
+@log.catch
 async def func_on_message(bot: commands.Bot, message: discord.Message):
     if bot.user in message.mentions:
         if message.author.id == bot.user.id:
             return
         else:
-            log.info(f"Message received from {message.author.display_name} (ID: {message.author.id}): {message.content}")
+            log.info(f"Mention received from {message.author.display_name} (ID: {message.author.id}): {message.content}")
 
     if message.content.startswith(">"):
         if message.author.id != bot.user.id:
-            return
+            if not message.author.is_friend():
+                return
+            else:
+                if message.channel.type != discord.ChannelType.private:
+                    return
         if message.author.id == bot.user.id:
             if message.content.__contains__("|") or message.content.__contains__("||"):
                 return
         if message.content.__contains__("ping"):
             ctx = await bot.get_context(message)
             await ping(bot, ctx, message)
         elif message.content.__contains__("quote"):
             ctx = await bot.get_context(message)
             await quote(bot, ctx, message)
+        elif message.content.__contains__("logs"):
+            ctx = await bot.get_context(message)
+            await logs(bot, ctx, message)
+        elif message.content.__contains__("search"):
+            ctx = await bot.get_context(message)
+            await search(bot, ctx, message)
     if message.guild is not None:
         guild_folder = f"_chatlogs/{message.guild.name}_{message.guild.id}"
         channel_folder = f"{guild_folder}/{message.channel.name}_{message.channel.id}"
     else:
         guild_folder = f"_chatlogs/_DMS"
         channel_folder = f"{guild_folder}/{message.channel.recipient.display_name}_{message.channel.id}"
     log_filename = f"{channel_folder}/{timestamp}.log"
```

### Comparing `gustavselfbot-0.0.6/GustavSelfBot/Events/__on_voice_state_update__.py` & `gustavselfbot-0.0.7/GustavSelfBot/Events/__on_voice_state_update__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # import os
 # import asyncio
 import discord
 from discord.ext import commands
 
 # from datetime import datetime
-# from GustavSelfBot import log
+from GustavSelfBot import log
 
 
+# @log.catch
 # async def save_recording(audio_source):
 #     # Save the recorded audio to an MP3 file with a unique filename
 #     timestamp = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
 #     folder = "_recordings"
 #     if not os.path.exists(folder):
 #         os.makedirs(folder)
 #
@@ -30,14 +31,15 @@
 #             executable=ffmpeg_options["executable"],
 #         )
 #         log.info("Recording saved.")
 #     except Exception as e:
 #         log.error(f"Error converting recording to MP3: {str(e)}")
 
 
+@log.catch
 async def func_on_voice_state_update(bot: commands.Bot, member: discord.Member, before: discord.VoiceState, after: discord.VoiceState):
     # if member.id == bot.user.id:
     #     if after.channel is not None:
     #         log.info(
     #             f"{member.display_name} (ID: {member.id}) Joined VC: {after.channel.name} {after.channel.guild.name} (ID: {after.channel.guild.id})"
     #         )
     #         channel: discord.VoiceChannel = bot.get_channel(after.channel.id)
```

### Comparing `gustavselfbot-0.0.6/GustavSelfBot/__bot__.py` & `gustavselfbot-0.0.7/GustavSelfBot/__bot__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import discord
 from discord.ext import commands
 
 from GustavSelfBot import log
 
-from GustavSelfBot.Events import func_on_message
-from GustavSelfBot.Events import func_on_ready
+from GustavSelfBot.Events import func_on_message, func_on_ready
 
 # from GustavSelfBot.Events import func_on_voice_state_update
 
 bot = commands.Bot(command_prefix=">", self_bot=True)
 
 
+@log.catch
 @bot.event
 async def on_ready():
     await func_on_ready(bot)
 
 
+@log.catch
 @bot.event
 async def on_message(message: discord.Message):
     await func_on_message(bot, message)
 
-
+# @log.catch
 # @bot.event
 # async def on_voice_state_update(member: discord.Member, before: discord.VoiceState, after: discord.VoiceState):
 #     await func_on_voice_state_update(bot, member, before, after)
```

### Comparing `gustavselfbot-0.0.6/GustavSelfBot/__init__.py` & `gustavselfbot-0.0.7/GustavSelfBot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 My self bot!
 Current implementation of GustavSelfBot includes chat logs and commands.
 TODO: make custom command and hooks possible
 """
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 import os
 
 from GustavSelfBot.__logging__ import *
 from GustavSelfBot.__config__ import Config
 from GustavSelfBot.__bot__ import bot
```

### Comparing `gustavselfbot-0.0.6/GustavSelfBot/__logging__.py` & `gustavselfbot-0.0.7/GustavSelfBot/__logging__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.6/README.md` & `gustavselfbot-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.6/pyproject.toml` & `gustavselfbot-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.6/PKG-INFO` & `gustavselfbot-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GustavSelfBot
-Version: 0.0.6
+Version: 0.0.7
 Summary: My self bot!
 Author-email: Gustavo Schip <gustavoschip@proton.me>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: discord.py-self[voice]
 Requires-Dist: aiohttp
```

