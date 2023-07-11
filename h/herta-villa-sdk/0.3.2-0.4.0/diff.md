# Comparing `tmp/herta_villa_sdk-0.3.2.tar.gz` & `tmp/herta_villa_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.3.2.tar", last modified: Sun Jun 25 10:54:13 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.4.0.tar", last modified: Tue Jul 11 03:10:57 2023, max compression
```

## Comparing `herta_villa_sdk-0.3.2.tar` & `herta_villa_sdk-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,30 @@
--rw-r--r--   0        0        0     1069 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/LICENSE
--rw-r--r--   0        0        0     2039 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/README.md
--rw-r--r--   0        0        0      555 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/__init__.py
--rw-r--r--   0        0        0    11250 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/bot.py
--rw-r--r--   0        0        0     4842 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/event.py
--rw-r--r--   0        0        0      738 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/exception.py
--rw-r--r--   0        0        0     1481 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/match.py
--rw-r--r--   0        0        0      353 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/__init__.py
--rw-r--r--   0        0        0     3799 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/chain.py
--rw-r--r--   0        0        0     1414 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/image.py
--rw-r--r--   0        0        0      927 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/post.py
--rw-r--r--   0        0        0     6289 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/text.py
--rw-r--r--   0        0        0      442 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/message/types.py
--rw-r--r--   0        0        0     2396 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/model.py
--rw-r--r--   0        0        0     2932 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/server.py
--rw-r--r--   0        0        0      564 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/typing.py
--rw-r--r--   0        0        0      563 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/hertavilla/version.py
--rw-r--r--   0        0        0     2128 2023-06-25 10:54:13.204465 herta_villa_sdk-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      528 2023-06-25 10:53:46.908332 herta_villa_sdk-0.3.2/tests/test_utils.py
--rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 herta_villa_sdk-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3954 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/README.md
+-rw-r--r--   0        0        0      555 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/__init__.py
+-rw-r--r--   0        0        0      782 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/auth.py
+-rw-r--r--   0        0        0     1387 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/base.py
+-rw-r--r--   0        0        0      520 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/emoticon.py
+-rw-r--r--   0        0        0     2174 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/member.py
+-rw-r--r--   0        0        0     2710 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/message.py
+-rw-r--r--   0        0        0     4422 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/role.py
+-rw-r--r--   0        0        0     4190 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/room.py
+-rw-r--r--   0        0        0      645 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/apis/villa.py
+-rw-r--r--   0        0        0     7235 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/bot.py
+-rw-r--r--   0        0        0     5398 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/event.py
+-rw-r--r--   0        0        0      738 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/exception.py
+-rw-r--r--   0        0        0     1481 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/match.py
+-rw-r--r--   0        0        0      353 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     3799 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1414 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/image.py
+-rw-r--r--   0        0        0      927 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6289 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/text.py
+-rw-r--r--   0        0        0      442 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/message/types.py
+-rw-r--r--   0        0        0     6280 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/model.py
+-rw-r--r--   0        0        0     2602 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/server.py
+-rw-r--r--   0        0        0      564 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/typing.py
+-rw-r--r--   0        0        0      563 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/utils.py
+-rw-r--r--   0        0        0       58 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/hertavilla/version.py
+-rw-r--r--   0        0        0     2144 2023-07-11 03:10:57.239067 herta_villa_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      528 2023-07-11 03:10:30.459122 herta_villa_sdk-0.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0     4589 1970-01-01 00:00:00.000000 herta_villa_sdk-0.4.0/PKG-INFO
```

### Comparing `herta_villa_sdk-0.3.2/LICENSE` & `herta_villa_sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.2/hertavilla/__init__.py` & `herta_villa_sdk-0.4.0/hertavilla/__init__.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.2/hertavilla/event.py` & `herta_villa_sdk-0.4.0/hertavilla/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -187,14 +187,47 @@
         return json.loads(v)
 
     @property
     def message(self) -> MessageChain:
         return self.content.content
 
 
+class CreateRobotEvent(Event):
+    type: Literal[3]
+
+
+class DeleteRobotEvent(Event):
+    type: Literal[4]
+
+
+class AddQuickEmoticonEvent(Event):
+    type: Literal[5]
+
+    room_id: int
+    """房间 id"""
+
+    uid: int
+    """发送表情的用户 id"""
+
+    emoticon_id: int
+    """表情 id"""
+
+    emoticon: str
+    """表情内容"""
+
+    msg_uid: str
+    """被回复的消息 id"""
+
+    bot_msg_id: str
+    """如果被回复的消息从属于机器人，则该字段不为空字符串"""
+
+    is_cancel: bool = False
+    """是否是取消表情"""
+
+
 def parse_event(payload: dict[str, Any]) -> Event:
     type_: int = payload["type"]
     cls_, name = events[type_]
     data = payload["extend_data"]["EventData"][name]
     payload.pop("extend_data")
     payload |= data
     return cls_.parse_obj(payload)
```

### Comparing `herta_villa_sdk-0.3.2/hertavilla/exception.py` & `herta_villa_sdk-0.4.0/hertavilla/exception.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.2/hertavilla/match.py` & `herta_villa_sdk-0.4.0/hertavilla/match.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.2/hertavilla/message/chain.py` & `herta_villa_sdk-0.4.0/hertavilla/message/chain.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.2/hertavilla/message/image.py` & `herta_villa_sdk-0.4.0/hertavilla/message/image.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.2/hertavilla/message/post.py` & `herta_villa_sdk-0.4.0/hertavilla/message/post.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.2/hertavilla/message/text.py` & `herta_villa_sdk-0.4.0/hertavilla/message/text.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.2/hertavilla/server.py` & `herta_villa_sdk-0.4.0/hertavilla/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,18 @@
                 f"on bot {event.robot.template.name}"
                 f"({event.robot.template.id}) "
                 f"in villa {event.robot.villa_id}"
             ),
         )
         if bot._bot_info is None:  # noqa: SLF001
             bot.bot_info = event.robot.template
-        try:
-            task = asyncio.create_task(bot.handle_event(event))
-            background_tasks.add(task)
-            task.add_done_callback(background_tasks.discard)
-            return web.json_response({"message": "", "retcode": 0})
-        except Exception:
-            logger.exception("Raised exceptions while handling event.")
-            raise web.HTTPInternalServerError(  # noqa: B904, TRY200
-                text=json.dumps(
-                    {"retcode": -100, "message": "internal error"},
-                ),
-            )
+        task = asyncio.create_task(bot.handle_event(event))
+        background_tasks.add(task)
+        task.add_done_callback(background_tasks.discard)
+        return web.json_response({"message": "", "retcode": 0})
     logger.warning(
         f"Received event but no bot with id {event.robot.template.id}",
     )
     raise web.HTTPNotFound(
         text=json.dumps(
             {"retcode": 1, "message": "no bot with this id"},
         ),
```

### Comparing `herta_villa_sdk-0.3.2/hertavilla/typing.py` & `herta_villa_sdk-0.4.0/hertavilla/typing.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.2/hertavilla/utils.py` & `herta_villa_sdk-0.4.0/hertavilla/utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.3.2/pyproject.toml` & `herta_villa_sdk-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 name = "herta-villa-sdk"
 description = "大别野「黑塔」Python SDK"
 authors = [
     { name = "MingxuanGame", email = "MingxuanGame@outlook.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.4",
-    "pydantic>=1.10.8",
+    "pydantic>=1.10.8,<2.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "mihoyo",
     "miyoushe",
     "bot",
     "villa",
 ]
 dynamic = []
-version = "0.3.2"
+version = "0.4.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/MingxuanGame/Herta-villa-SDK"
 Documentation = "https://github.com/MingxuanGame/Herta-villa-SDK"
@@ -79,14 +79,15 @@
     "ASYNC",
 ]
 allowed-confusables = [
     "，",
     "。",
     "（",
     "）",
+    "；",
 ]
 
 [tool.ruff.isort]
 force-sort-within-sections = true
 extra-standard-library = [
     "typing_extensions",
 ]
```

### Comparing `herta_villa_sdk-0.3.2/tests/test_utils.py` & `herta_villa_sdk-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

