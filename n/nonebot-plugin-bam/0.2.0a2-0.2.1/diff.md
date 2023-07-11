# Comparing `tmp/nonebot_plugin_bam-0.2.0a2.tar.gz` & `tmp/nonebot_plugin_bam-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bam-0.2.0a2.tar", max compression
+gzip compressed data, was "nonebot_plugin_bam-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_bam-0.2.0a2.tar` & `nonebot_plugin_bam-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1059 2023-06-14 06:44:18.264807 nonebot_plugin_bam-0.2.0a2/LICENSE
--rw-r--r--   0        0        0     4854 2023-06-16 08:56:03.559872 nonebot_plugin_bam-0.2.0a2/README.md
--rw-r--r--   0        0        0      663 2023-06-16 09:21:09.846465 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/__init__.py
--rw-r--r--   0        0        0     1574 2023-06-16 08:56:03.560453 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/activity.py
--rw-r--r--   0        0        0        0 2023-06-14 06:44:18.265535 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/__init__.py
--rw-r--r--   0        0        0    11587 2023-06-16 08:56:03.560845 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/activity.py
--rw-r--r--   0        0        0     2623 2023-06-16 08:56:03.561388 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/api.py
--rw-r--r--   0        0        0      766 2023-06-14 06:44:18.266043 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/live1.py
--rw-r--r--   0        0        0      832 2023-06-14 07:53:56.620081 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/live2.py
--rw-r--r--   0        0        0      624 2023-06-14 07:52:16.640215 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/user.py
--rw-r--r--   0        0        0     1836 2023-06-16 08:56:03.561693 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/wbi.py
--rw-r--r--   0        0        0     1229 2023-06-16 09:18:53.017876 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/common.py
--rw-r--r--   0        0        0      371 2023-06-14 09:43:07.419841 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/config.py
--rw-r--r--   0        0        0       91 2023-06-14 06:44:18.266730 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/__init__.py
--rw-r--r--   0        0        0     1404 2023-06-15 09:41:09.332144 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/db.py
--rw-r--r--   0        0        0     3454 2023-06-16 08:56:03.562014 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/helper.py
--rw-r--r--   0        0        0      154 2023-06-14 06:44:18.267190 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/tables/__init__.py
--rw-r--r--   0        0        0      336 2023-06-14 06:44:18.267312 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/tables/bilibili_user.py
--rw-r--r--   0        0        0      468 2023-06-14 06:44:18.267419 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/tables/bilibili_user_status.py
--rw-r--r--   0        0        0      481 2023-06-14 06:44:18.267541 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/tables/follow_link.py
--rw-r--r--   0        0        0      311 2023-06-14 06:44:18.267650 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/tables/group.py
--rw-r--r--   0        0        0     5533 2023-06-16 08:56:03.562318 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/follow.py
--rw-r--r--   0        0        0     3192 2023-06-16 08:56:03.562951 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/group.py
--rw-r--r--   0        0        0        0 2023-06-14 06:44:18.268036 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/tasks/__init__.py
--rw-r--r--   0        0        0     4694 2023-06-16 09:19:56.392130 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/tasks/activity_monitor.py
--rw-r--r--   0        0        0     4017 2023-06-16 09:20:24.425842 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/tasks/live_monitor.py
--rw-r--r--   0        0        0     1131 2023-06-16 08:56:03.564006 nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/user.py
--rw-r--r--   0        0        0     1315 2023-06-16 09:21:15.341132 nonebot_plugin_bam-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0     5994 1970-01-01 00:00:00.000000 nonebot_plugin_bam-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-14 06:44:18.264807 nonebot_plugin_bam-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5116 2023-07-11 06:52:15.727280 nonebot_plugin_bam-0.2.1/README.md
+-rw-r--r--   0        0        0      661 2023-07-11 06:54:02.588140 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/__init__.py
+-rw-r--r--   0        0        0     1574 2023-06-16 08:56:03.560453 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/activity.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:44:18.265535 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/__init__.py
+-rw-r--r--   0        0        0    11587 2023-06-16 08:56:03.560845 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/activity.py
+-rw-r--r--   0        0        0     2623 2023-06-16 08:56:03.561388 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/api.py
+-rw-r--r--   0        0        0      766 2023-06-14 06:44:18.266043 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/live1.py
+-rw-r--r--   0        0        0      832 2023-06-14 07:53:56.620081 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/live2.py
+-rw-r--r--   0        0        0      624 2023-06-14 07:52:16.640215 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/user.py
+-rw-r--r--   0        0        0     1836 2023-06-16 08:56:03.561693 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/wbi.py
+-rw-r--r--   0        0        0     1229 2023-06-16 09:37:00.201981 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/common.py
+-rw-r--r--   0        0        0      620 2023-07-11 06:51:57.149020 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/config.py
+-rw-r--r--   0        0        0       91 2023-06-14 06:44:18.266730 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/database/__init__.py
+-rw-r--r--   0        0        0     1404 2023-06-15 09:41:09.332144 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/database/db.py
+-rw-r--r--   0        0        0     3454 2023-06-16 08:56:03.562014 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/database/helper.py
+-rw-r--r--   0        0        0      154 2023-06-14 06:44:18.267190 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/database/tables/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-14 06:44:18.267312 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/database/tables/bilibili_user.py
+-rw-r--r--   0        0        0      468 2023-06-14 06:44:18.267419 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/database/tables/bilibili_user_status.py
+-rw-r--r--   0        0        0      481 2023-06-14 06:44:18.267541 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/database/tables/follow_link.py
+-rw-r--r--   0        0        0      311 2023-06-14 06:44:18.267650 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/database/tables/group.py
+-rw-r--r--   0        0        0     5533 2023-06-16 08:56:03.562318 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/follow.py
+-rw-r--r--   0        0        0     3192 2023-06-16 08:56:03.562951 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/group.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:44:18.268036 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/tasks/__init__.py
+-rw-r--r--   0        0        0     4768 2023-07-11 06:53:04.961168 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/tasks/activity_monitor.py
+-rw-r--r--   0        0        0     4087 2023-07-11 06:53:19.900394 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/tasks/live_monitor.py
+-rw-r--r--   0        0        0     1131 2023-06-16 08:56:03.564006 nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/user.py
+-rw-r--r--   0        0        0     1313 2023-07-11 06:53:55.552091 nonebot_plugin_bam-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6254 1970-01-01 00:00:00.000000 nonebot_plugin_bam-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_bam-0.2.0a2/LICENSE` & `nonebot_plugin_bam-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/README.md` & `nonebot_plugin_bam-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Bilibili Activity Monitor
 
 B 站用户监视器，自动监控用户的动态和直播状态，在有新动态和直播状态改变时向关注群发送提示信息。
 
 可多群共用，每个群可以有不同的关注列表。自带数据落地存储机制，重启后可保留各群关注状态。
 
+0.2.0 版本已支持 NoneBot2 2.0 正式版 API，依赖 OneBot V11 Adapter。
+
 ## 功能示例
 
 ### 直播提醒
 
 ![screenshot-live]
 
 ### 动态提醒
@@ -60,14 +62,17 @@
 BAM_ON_STARTUP_CLEAN_LIVE_STATUS=false 
 
 # 监控任务的间隔，这里设置的是每个用户间的间隔，而不是一轮的间隔。
 # 所以如果一共关注了 N 个人（多个群关注同一个人只算一个）
 # 那对于每个人来说，两次检测之间的间隔就是 N * interval
 # 一般来说不要设置在 5 以下，可能会被 B 站 API 反爬而拒绝响应
 BAM_MONITOR_TASK_INTERVAL=5
+# 单独设置每个任务的间隔，如果没有设置，或者设置成 <= 0 的值，就会用上面那个
+BAM_ACTIVITY_MONITOR_TASK_INTERVAL=0
+BAM_LIVE_MONITOR_TASK_INTERVAL=0
 
 # 使用那一个直播间状态查询 API，默认为 2，如果发现被封禁了可以临时调到 1 试试
 BAM_LIVE_API=2
 
 # 动态内容在发送到 QQ 时的最大长度，超过长度会截断，设置为 0 或负数表示不截断
 BAM_ACTIVITY_CONTENT_MAX_LENGTH=0
 ```
```

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/__init__.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .config import Config
 from .follow import cmd_follower_add, cmd_follower_list, cmd_follower_remove
 from .group import cmd_group_add, cmd_group_list, cmd_group_remove
 from .tasks.activity_monitor import task_check_new_activity
 from .tasks.live_monitor import task_check_all_live_status
 from .user import cmd_user_fetch
 
-__version__ = "0.2.0a2"
+__version__ = "0.2.1"
 
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name = "BAM",
     description="Bilibili Activity Monitor",
     usage="Bilibili用户动态/开播监控器",
```

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/activity.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/activity.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/activity.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/activity.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/api.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/live1.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/live1.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/live2.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/live2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/user.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/bilibili/wbi.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/bilibili/wbi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/common.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/db.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/database/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/database/helper.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/database/helper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/follow.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/follow.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/group.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/tasks/activity_monitor.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/tasks/activity_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 from ..config import CONF
 from ..database import helper
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 JOB_ID = "activity_monitor"
 LOGNAME = "BTASK:ACTIVITY"
-INTERVAL = CONF.bam_monitor_task_interval
+INTERVAL = CONF.bam_activity_monitor_task_interval
+if INTERVAL <= 0:
+    INTERVAL = CONF.bam_monitor_task_interval 
 
 
 @scheduler.scheduled_job(
     "interval",
     seconds=0,
     id=JOB_ID,
     next_run_time=datetime.now() + timedelta(seconds=INTERVAL / 2.0),
```

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/tasks/live_monitor.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/tasks/live_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from ..config import CONF
 from ..database import helper
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 JOB_ID = "live_monitor"
 LOGNAME = "BTASK:LIVE"
-INTERVAL = CONF.bam_monitor_task_interval
+INTERVAL = CONF.bam_live_monitor_task_interval
+if INTERVAL <= 0:
+    INTERVAL = CONF.bam_monitor_task_interval 
 
 if CONF.bam_live_api == 1:
     from ..bilibili.live1 import RoomInfo, room_info
 elif CONF.bam_live_api == 2:
     from ..bilibili.live2 import RoomInfo, room_info
 else:
     logger.error("Invalid `BAM_LIVE_API` configure value")
```

### Comparing `nonebot_plugin_bam-0.2.0a2/nonebot_plugin_bam/user.py` & `nonebot_plugin_bam-0.2.1/nonebot_plugin_bam/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bam-0.2.0a2/pyproject.toml` & `nonebot_plugin_bam-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bam"
-version = "0.2.0a2"
+version = "0.2.1"
 description = "Bilibili activity monitor plugin for nonebot"
 authors = ["7sDream <i@7sdre.am>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/7sDream/nonebot-plugin-bam"
 repository = "https://github.com/7sDream/nonebot-plugin-bam"
 keywords = ["nonebot", "bilibili", "qqbot"]
```

### Comparing `nonebot_plugin_bam-0.2.0a2/PKG-INFO` & `nonebot_plugin_bam-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bam
-Version: 0.2.0a2
+Version: 0.2.1
 Summary: Bilibili activity monitor plugin for nonebot
 Home-page: https://github.com/7sDream/nonebot-plugin-bam
 License: MIT
 Keywords: nonebot,bilibili,qqbot
 Author: 7sDream
 Author-email: i@7sdre.am
 Requires-Python: >=3.9,<4.0
@@ -28,14 +28,16 @@
 
 # Bilibili Activity Monitor
 
 B 站用户监视器，自动监控用户的动态和直播状态，在有新动态和直播状态改变时向关注群发送提示信息。
 
 可多群共用，每个群可以有不同的关注列表。自带数据落地存储机制，重启后可保留各群关注状态。
 
+0.2.0 版本已支持 NoneBot2 2.0 正式版 API，依赖 OneBot V11 Adapter。
+
 ## 功能示例
 
 ### 直播提醒
 
 ![screenshot-live]
 
 ### 动态提醒
@@ -88,14 +90,17 @@
 BAM_ON_STARTUP_CLEAN_LIVE_STATUS=false 
 
 # 监控任务的间隔，这里设置的是每个用户间的间隔，而不是一轮的间隔。
 # 所以如果一共关注了 N 个人（多个群关注同一个人只算一个）
 # 那对于每个人来说，两次检测之间的间隔就是 N * interval
 # 一般来说不要设置在 5 以下，可能会被 B 站 API 反爬而拒绝响应
 BAM_MONITOR_TASK_INTERVAL=5
+# 单独设置每个任务的间隔，如果没有设置，或者设置成 <= 0 的值，就会用上面那个
+BAM_ACTIVITY_MONITOR_TASK_INTERVAL=0
+BAM_LIVE_MONITOR_TASK_INTERVAL=0
 
 # 使用那一个直播间状态查询 API，默认为 2，如果发现被封禁了可以临时调到 1 试试
 BAM_LIVE_API=2
 
 # 动态内容在发送到 QQ 时的最大长度，超过长度会截断，设置为 0 或负数表示不截断
 BAM_ACTIVITY_CONTENT_MAX_LENGTH=0
 ```
```

