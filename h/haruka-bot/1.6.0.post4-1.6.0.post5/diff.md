# Comparing `tmp/haruka-bot-1.6.0.post4.tar.gz` & `tmp/haruka-bot-1.6.0.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka-bot-1.6.0.post4.tar", last modified: Thu Jun 29 08:22:01 2023, max compression
+gzip compressed data, was "haruka-bot-1.6.0.post5.tar", last modified: Tue Jul 11 09:24:48 2023, max compression
```

## Comparing `haruka-bot-1.6.0.post4.tar` & `haruka-bot-1.6.0.post5.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0    34522 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post4/LICENSE
--rw-r--r--   0        0        0     2790 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post4/README.md
--rw-r--r--   0        0        0      695 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/__init__.py
--rw-r--r--   0        0        0       61 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/__main__.py
--rw-r--r--   0        0        0      189 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/cli/__init__.py
--rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/cli/bot.py
--rw-r--r--   0        0        0     1170 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/cli/utils.py
--rw-r--r--   0        0        0     1704 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/config.py
--rw-r--r--   0        0        0       49 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/database/__init__.py
--rw-r--r--   0        0        0    10155 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/database/db.py
--rw-r--r--   0        0        0     1936 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/database/models.py
--rw-r--r--   0        0        0       30 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/libs/__init__.py
--rw-r--r--   0        0        0     1466 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/libs/dynamic/__init__.py
--rw-r--r--   0        0        0     1085 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/libs/dynamic/card.py
--rw-r--r--   0        0        0      598 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/libs/dynamic/desc.py
--rw-r--r--   0        0        0     1024 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/libs/dynamic/display.py
--rw-r--r--   0        0        0      816 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/libs/dynamic/user_profile.py
--rw-r--r--   0        0        0      466 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/at/__init__.py
--rw-r--r--   0        0        0     1430 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/at/at_off.py
--rw-r--r--   0        0        0     1421 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/at/at_on.py
--rw-r--r--   0        0        0      678 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/auto_agree.py
--rw-r--r--   0        0        0      875 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/auto_delete.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/dynamic/__init__.py
--rw-r--r--   0        0        0     1048 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/dynamic/dynamic_off.py
--rw-r--r--   0        0        0     1039 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/dynamic/dynamic_on.py
--rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/help.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/live/__init__.py
--rw-r--r--   0        0        0      848 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/plugins/live/live_now.py
--rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/live/live_off.py
--rw-r--r--   0        0        0     1012 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/live/live_on.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/permission/__init__.py
--rw-r--r--   0        0        0     1180 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/permission/permission_off.py
--rw-r--r--   0        0        0     1201 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/permission/permission_on.py
--rw-r--r--   0        0        0       58 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/pusher/__init__.py
--rw-r--r--   0        0        0     4979 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post4/haruka_bot/plugins/pusher/dynamic_pusher.py
--rw-r--r--   0        0        0     2676 2023-06-29 08:13:05.065015 haruka-bot-1.6.0.post4/haruka_bot/plugins/pusher/live_pusher.py
--rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/sub/__init__.py
--rw-r--r--   0        0        0     2039 2023-06-29 08:13:05.065015 haruka-bot-1.6.0.post4/haruka_bot/plugins/sub/add_sub.py
--rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/sub/delete_sub.py
--rw-r--r--   0        0        0     1551 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/plugins/sub/sub_list.py
--rw-r--r--   0        0        0    11045 2023-06-29 08:13:05.065015 haruka-bot-1.6.0.post4/haruka_bot/utils/__init__.py
--rw-r--r--   0        0        0     8714 2023-06-29 08:13:05.065015 haruka-bot-1.6.0.post4/haruka_bot/utils/browser.py
--rw-r--r--   0        0        0     4947 2023-06-29 08:13:05.065015 haruka-bot-1.6.0.post4/haruka_bot/utils/captcha.py
--rw-r--r--   0        0        0      702 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post4/haruka_bot/utils/fonts_provider.py
--rw-r--r--   0        0        0     9451 2023-06-29 08:15:01.994592 haruka-bot-1.6.0.post4/haruka_bot/utils/mobile.js
--rw-r--r--   0        0        0       97 2023-06-29 08:20:21.029899 haruka-bot-1.6.0.post4/haruka_bot/version.py
--rw-r--r--   0        0        0     1579 2023-06-29 08:13:05.065015 haruka-bot-1.6.0.post4/pyproject.toml
--rw-r--r--   0        0        0     3345 1970-01-01 00:00:00.000000 haruka-bot-1.6.0.post4/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post5/LICENSE
+-rw-r--r--   0        0        0     2790 2023-06-27 09:01:29.192864 haruka-bot-1.6.0.post5/README.md
+-rw-r--r--   0        0        0      695 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post5/haruka_bot/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/__main__.py
+-rw-r--r--   0        0        0      189 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/cli/__init__.py
+-rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/cli/bot.py
+-rw-r--r--   0        0        0     1170 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post5/haruka_bot/cli/utils.py
+-rw-r--r--   0        0        0     1748 2023-07-04 17:03:22.937805 haruka-bot-1.6.0.post5/haruka_bot/config.py
+-rw-r--r--   0        0        0       49 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/database/__init__.py
+-rw-r--r--   0        0        0    10155 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/database/db.py
+-rw-r--r--   0        0        0     1936 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/database/models.py
+-rw-r--r--   0        0        0       30 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/libs/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post5/haruka_bot/libs/dynamic/__init__.py
+-rw-r--r--   0        0        0     1085 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post5/haruka_bot/libs/dynamic/card.py
+-rw-r--r--   0        0        0      598 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post5/haruka_bot/libs/dynamic/desc.py
+-rw-r--r--   0        0        0     1024 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post5/haruka_bot/libs/dynamic/display.py
+-rw-r--r--   0        0        0      816 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post5/haruka_bot/libs/dynamic/user_profile.py
+-rw-r--r--   0        0        0      466 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post5/haruka_bot/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/at/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/at/at_off.py
+-rw-r--r--   0        0        0     1421 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/at/at_on.py
+-rw-r--r--   0        0        0      678 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/auto_agree.py
+-rw-r--r--   0        0        0      875 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/auto_delete.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/dynamic/__init__.py
+-rw-r--r--   0        0        0     1048 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/dynamic/dynamic_off.py
+-rw-r--r--   0        0        0     1039 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/dynamic/dynamic_on.py
+-rw-r--r--   0        0        0      734 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/help.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/live/__init__.py
+-rw-r--r--   0        0        0      848 2023-06-29 08:13:05.061015 haruka-bot-1.6.0.post5/haruka_bot/plugins/live/live_now.py
+-rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/live/live_off.py
+-rw-r--r--   0        0        0     1012 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/live/live_on.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/permission/__init__.py
+-rw-r--r--   0        0        0     1180 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/permission/permission_off.py
+-rw-r--r--   0        0        0     1201 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/permission/permission_on.py
+-rw-r--r--   0        0        0       58 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/pusher/__init__.py
+-rw-r--r--   0        0        0     5217 2023-07-04 17:22:59.257358 haruka-bot-1.6.0.post5/haruka_bot/plugins/pusher/dynamic_pusher.py
+-rw-r--r--   0        0        0     2769 2023-07-04 17:26:27.947162 haruka-bot-1.6.0.post5/haruka_bot/plugins/pusher/live_pusher.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/sub/__init__.py
+-rw-r--r--   0        0        0     2039 2023-06-29 08:13:05.065015 haruka-bot-1.6.0.post5/haruka_bot/plugins/sub/add_sub.py
+-rw-r--r--   0        0        0     1021 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/plugins/sub/delete_sub.py
+-rw-r--r--   0        0        0     1553 2023-07-04 17:26:53.312181 haruka-bot-1.6.0.post5/haruka_bot/plugins/sub/sub_list.py
+-rw-r--r--   0        0        0    11045 2023-06-29 08:13:05.065015 haruka-bot-1.6.0.post5/haruka_bot/utils/__init__.py
+-rw-r--r--   0        0        0     8589 2023-07-11 09:23:33.715343 haruka-bot-1.6.0.post5/haruka_bot/utils/browser.py
+-rw-r--r--   0        0        0      702 2023-06-27 09:01:29.220865 haruka-bot-1.6.0.post5/haruka_bot/utils/fonts_provider.py
+-rw-r--r--   0        0        0     9460 2023-07-04 16:08:45.419616 haruka-bot-1.6.0.post5/haruka_bot/utils/mobile.js
+-rw-r--r--   0        0        0       97 2023-07-04 17:17:31.474477 haruka-bot-1.6.0.post5/haruka_bot/version.py
+-rw-r--r--   0        0        0     1619 2023-07-04 17:14:00.405091 haruka-bot-1.6.0.post5/pyproject.toml
+-rw-r--r--   0        0        0     3345 1970-01-01 00:00:00.000000 haruka-bot-1.6.0.post5/PKG-INFO
```

### Comparing `haruka-bot-1.6.0.post4/LICENSE` & `haruka-bot-1.6.0.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/README.md` & `haruka-bot-1.6.0.post5/README.md`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/__init__.py` & `haruka-bot-1.6.0.post5/haruka_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/cli/bot.py` & `haruka-bot-1.6.0.post5/haruka_bot/cli/bot.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/cli/utils.py` & `haruka-bot-1.6.0.post5/haruka_bot/cli/utils.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/config.py` & `haruka-bot-1.6.0.post5/haruka_bot/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     haruka_proxy: Optional[str] = None
     haruka_interval: int = 10
     haruka_live_interval: int = haruka_interval
     haruka_dynamic_interval: int = 0
     haruka_dynamic_at: bool = False
     haruka_screenshot_style: str = "mobile"
     haruka_captcha_address: str = "https://captcha-cd.ngworks.cn"
+    haruka_captcha_token: str = "harukabot"
     haruka_browser_ua: Optional[str] = None
     haruka_dynamic_timeout: int = 30
     haruka_dynamic_font_source: str = "system"
     haruka_dynamic_font: Optional[str] = "Noto Sans CJK SC"
     haruka_dynamic_big_image: bool = False
     haruka_command_prefix: str = ""
     # 频道管理员身份组
```

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/database/db.py` & `haruka-bot-1.6.0.post5/haruka_bot/database/db.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/database/models.py` & `haruka-bot-1.6.0.post5/haruka_bot/database/models.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/libs/dynamic/__init__.py` & `haruka-bot-1.6.0.post5/haruka_bot/libs/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/libs/dynamic/card.py` & `haruka-bot-1.6.0.post5/haruka_bot/libs/dynamic/card.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/libs/dynamic/desc.py` & `haruka-bot-1.6.0.post5/haruka_bot/libs/dynamic/desc.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/libs/dynamic/display.py` & `haruka-bot-1.6.0.post5/haruka_bot/libs/dynamic/display.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/libs/dynamic/user_profile.py` & `haruka-bot-1.6.0.post5/haruka_bot/libs/dynamic/user_profile.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/at/at_off.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/at/at_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/at/at_on.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/at/at_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/auto_agree.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/auto_agree.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/auto_delete.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/auto_delete.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/dynamic/dynamic_off.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/dynamic/dynamic_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/dynamic/dynamic_on.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/dynamic/dynamic_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/help.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/help.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/live/live_now.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/live/live_now.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/live/live_off.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/live/live_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/live/live_on.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/live/live_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/permission/permission_off.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/permission/permission_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/permission/permission_on.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/permission/permission_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/pusher/dynamic_pusher.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/pusher/dynamic_pusher.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from apscheduler.events import (
     EVENT_JOB_ERROR,
     EVENT_JOB_EXECUTED,
     EVENT_JOB_MISSED,
     EVENT_SCHEDULER_STARTED,
 )
+from bilireq.exceptions import GrpcError
 from bilireq.grpc.dynamic import grpc_get_user_dynamics
 from bilireq.grpc.protos.bilibili.app.dynamic.v2.dynamic_pb2 import DynamicType
 from grpc import StatusCode
 from grpc.aio import AioRpcError
 from nonebot.adapters.onebot.v11.message import MessageSegment
 from nonebot.log import logger
 
@@ -40,16 +41,20 @@
                 timeout=plugin_config.haruka_dynamic_timeout,
                 proxy=plugin_config.haruka_proxy,
             )
         ).list
     except AioRpcError as e:
         if e.code() == StatusCode.DEADLINE_EXCEEDED:
             logger.error(f"爬取动态超时，将在下个轮询中重试：{e.code()} {e.details()}")
-            return
-        raise
+        else:
+            logger.error(f"爬取动态失败：{e.code()} {e.details()}")
+        return
+    except GrpcError as e:
+        logger.error(f"爬取动态失败：{e.code} {e.msg}")
+        return
 
     if not dynamics:  # 没发过动态
         if uid in offset and offset[uid] == -1:  # 不记录会导致第一次发动态不推送
             offset[uid] = 0
         return
     # 更新昵称
     name = dynamics[0].modules[0].module_author.author.name
@@ -92,16 +97,17 @@
                 DynamicType.draw: "发布了新图文动态",
                 DynamicType.av: "发布了新投稿",
                 DynamicType.article: "发布了新专栏",
                 DynamicType.music: "发布了新音频",
             }
             message = (
                 f"{name} {type_msg.get(dynamic.card_type, type_msg[0])}：\n"
-                f"{f'动态图片可能截图异常：{err}' if err else ''}\n"
-                f"{MessageSegment.image(image)}\n{url}"
+                + str(f"动态图片可能截图异常：{err}\n" if err else "")
+                + MessageSegment.image(image)
+                + f"\n{url}"
             )
 
             push_list = await db.get_push_list(uid, "dynamic")
             for sets in push_list:
                 await safe_send(
                     bot_id=sets.bot_id,
                     send_type=sets.type,
```

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/pusher/live_pusher.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/pusher/live_pusher.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 live_time = {}
 
 
 @scheduler.scheduled_job(
     "interval", seconds=plugin_config.haruka_live_interval, id="live_sched"
 )
 async def live_sched():
+    # sourcery skip: use-fstring-for-concatenation
     """直播推送"""
     uids = await db.get_uid_list("live")
 
     if not uids:  # 订阅为空
         return
     logger.debug(f"爬取直播列表，目前开播{sum(status.values())}人，总共{len(uids)}人")
     res = await get_rooms_info_by_uids(uids, reqtype="web", proxies=PROXIES)
@@ -38,28 +39,30 @@
         name = info["uname"]
         if new_status:  # 开播
             live_time[uid] = info["live_time"]
             room_id = info["short_id"] or info["room_id"]
             url = f"https://live.bilibili.com/{room_id}"
             title = info["title"]
             cover = info["cover_from_user"] or info["keyframe"]
-            area_parent = info["area_v2_parent_name"]
             area = info["area_v2_name"]
+            area_parent = info["area_v2_parent_name"]
             room_area = f"{area_parent} / {area}"
             logger.info(f"检测到开播：{name}（{uid}）")
             live_msg = (
-                f"{name} 开播啦！\n分区：{room_area}\n标题：{title}\n{MessageSegment.image(cover)}\n{url}"
+                f"{name} 开播啦！\n分区：{room_area}\n标题：{title}\n"
+                + MessageSegment.image(cover)
+                + f"\n{url}"
             )
         else:  # 下播
             logger.info(f"检测到下播：{name}（{uid}）")
             if not plugin_config.haruka_live_off_notify:  # 没开下播推送
                 continue
             live_time_msg = (
-                f"，本次直播时长 {calc_time_total(time.time() - live_time[uid])}。"
-                if live_time[uid]
+                f"\n本次直播时长 {calc_time_total(time.time() - live_time[uid])}。"
+                if live_time.get(uid)
                 else "。"
             )
             live_msg = f"{name} 下播了{live_time_msg}"
 
         # 推送
         push_list = await db.get_push_list(uid, "live")
         for sets in push_list:
```

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/sub/add_sub.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/sub/add_sub.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/sub/delete_sub.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/sub/delete_sub.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/plugins/sub/sub_list.py` & `haruka-bot-1.6.0.post5/haruka_bot/plugins/sub/sub_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """发送当前位置的订阅列表"""
     message = "关注列表（所有群/好友都是分开的）\n\n"
     subs = await db.get_sub_list(event.message_type, await get_type_id(event))
     for sub in subs:
         user = await db.get_user(uid=sub.uid)
         assert user is not None
         message += (
-            f"{user.name}（{user.uid}）"
+            f"{user.name}（{user.uid}）\n"
             f"直播：{'开' if sub.live else '关'}，"
             f"动态：{'开' if sub.dynamic else '关'}，"
             # TODO 私聊不显示全体
             f"全体：{'开' if sub.at else '关'}\n"
         )
     if len(message.splitlines()) > 8 and isinstance(event, GroupMessageEvent):
         await bot.send_group_forward_msg(
```

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/utils/__init__.py` & `haruka-bot-1.6.0.post5/haruka_bot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/utils/browser.py` & `haruka-bot-1.6.0.post5/haruka_bot/utils/browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import os
 import re
 import sys
 from pathlib import Path
 from typing import Optional
 
 from nonebot.log import logger
+from aunly_captcha_solver import CaptchaInfer
 from playwright.__main__ import main
 from playwright.async_api import BrowserContext, async_playwright, Page
 
 from ..config import plugin_config
 from .fonts_provider import fill_font
-from .captcha import resolve_captcha
 from ..utils import get_path
 
 _browser: Optional[BrowserContext] = None
 mobile_js = Path(__file__).parent.joinpath("mobile.js")
 
 
 async def init_browser(proxy=plugin_config.haruka_proxy, **kwargs) -> BrowserContext:
+    logger.info("初始化浏览器")
     if proxy:
         kwargs["proxy"] = {"server": proxy}
     global _browser
     p = await async_playwright().start()
     browser_data = Path(get_path("browser"))
     browser_data.mkdir(parents=True, exist_ok=True)
     browser_context = await p.chromium.launch_persistent_context(
@@ -34,14 +35,15 @@
                 "Mozilla/5.0 (Linux; Android 10; RMX1911) AppleWebKit/537.36 "
                 "(KHTML, like Gecko) Chrome/100.0.4896.127 Mobile Safari/537.36"
             )
             if plugin_config.haruka_screenshot_style.lower() == "mobile"
             else None
         ),
         device_scale_factor=2,
+        timeout=plugin_config.haruka_dynamic_timeout * 1000,
         **kwargs,
     )
     if plugin_config.haruka_screenshot_style.lower() != "mobile":
         await browser_context.add_cookies(
             [
                 {
                     "name": "hit-dyn-v2",
@@ -53,15 +55,15 @@
         )
     _browser = browser_context
     return _browser
 
 
 async def get_browser() -> BrowserContext:
     global _browser
-    if not _browser or _browser.browser is None or not _browser.browser.is_connected():
+    if not _browser:
         _browser = await init_browser()
     return _browser
 
 
 async def get_dynamic_screenshot(dynamic_id, style=plugin_config.haruka_screenshot_style):
     """获取动态截图"""
     image: Optional[bytes] = None
@@ -74,15 +76,15 @@
             #     page, clip = await get_dynamic_screenshot_mobile(dynamic_id, page)
             # else:
             #     page, clip = await get_dynamic_screenshot_pc(dynamic_id, page)
             page, clip = await get_dynamic_screenshot_mobile(dynamic_id, page)
             clip["height"] = min(clip["height"], 32766)
             return (
                 await page.screenshot(clip=clip, full_page=True, type="jpeg", quality=98),
-                err,
+                None,
             )
         except TimeoutError:
             logger.warning(f"截图超时，重试 {i + 1}/3")
             err = "截图超时"
         except Notfound:
             logger.error(f"动态 {dynamic_id} 不存在")
             err = "动态不存在"
@@ -111,21 +113,20 @@
 
 async def get_dynamic_screenshot_mobile(dynamic_id, page: Page):
     """移动端动态截图"""
     url = f"https://m.bilibili.com/dynamic/{dynamic_id}"
     await page.set_viewport_size({"width": 460, "height": 780})
     await page.route(re.compile("^https://static.graiax/fonts/(.+)$"), fill_font)
     if plugin_config.haruka_captcha_address:
-        page = await resolve_captcha(url, page)
-    else:
-        await page.goto(
-            url,
-            wait_until="networkidle",
-            timeout=plugin_config.haruka_dynamic_timeout * 1000,
+        captcha = CaptchaInfer(
+            plugin_config.haruka_captcha_address, plugin_config.haruka_captcha_token
         )
+        page = await captcha.solve_captcha(page, url)
+    else:
+        await page.goto(url, wait_until="networkidle")
     # 动态被删除或者进审核了
     if page.url == "https://m.bilibili.com/404":
         raise Notfound
     # await page.add_script_tag(
     #     content=
     #     # 去除打开app按钮
     #     "document.getElementsByClassName('m-dynamic-float-openapp').forEach(v=>v.remove());"
@@ -133,19 +134,16 @@
     #     "document.getElementsByClassName('dyn-header__following').forEach(v=>v.remove());"
     #     # 修复字体与换行问题
     #     "const dyn=document.getElementsByClassName('dyn-card')[0];"
     #     "dyn.style.fontFamily='Noto Sans CJK SC, sans-serif';"
     #     "dyn.style.overflowWrap='break-word'"
     # )
 
-    await page.wait_for_load_state(state="domcontentloaded", timeout=20000)
-    if "opus" in page.url:
-        await page.wait_for_selector(".opus-module-author", state="visible")
-    else:
-        await page.wait_for_selector(".dyn-header__author__face", state="visible")
+    await page.wait_for_load_state(state="domcontentloaded")
+    await page.wait_for_selector(".b-img__inner, .dyn-header__author__face", state="visible")
 
     await page.add_script_tag(path=mobile_js)
 
     await page.evaluate(
         f'setFont("{plugin_config.haruka_dynamic_font}", '
         f'"{plugin_config.haruka_dynamic_font_source}")'
         if plugin_config.haruka_dynamic_font
@@ -155,15 +153,15 @@
         f"getMobileStyle({'true' if plugin_config.haruka_dynamic_big_image else 'false'})"
     )
 
     await page.wait_for_load_state("networkidle")
     await page.wait_for_load_state("domcontentloaded")
 
     await page.wait_for_timeout(
-        200 if plugin_config.haruka_dynamic_font_source == "remote" else 50
+        1000 if plugin_config.haruka_dynamic_font_source == "remote" else 200
     )
 
     # 判断字体是否加载完成
     need_wait = ["imageComplete", "fontsLoaded"]
     await asyncio.gather(*[page.wait_for_function(f"{i}()") for i in need_wait])
 
     card = await page.query_selector(".opus-modules" if "opus" in page.url else ".dyn-card")
@@ -173,19 +171,15 @@
     return page, clip
 
 
 async def get_dynamic_screenshot_pc(dynamic_id, page: Page):
     """电脑端动态截图"""
     url = f"https://t.bilibili.com/{dynamic_id}"
     await page.set_viewport_size({"width": 2560, "height": 1080})
-    await page.goto(
-        url,
-        wait_until="networkidle",
-        timeout=plugin_config.haruka_dynamic_timeout * 1000,
-    )
+    await page.goto(url, wait_until="networkidle")
     # 动态被删除或者进审核了
     if page.url == "https://www.bilibili.com/404":
         raise Notfound
     card = await page.query_selector(".card")
     assert card
     clip = await card.bounding_box()
     assert clip
```

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/utils/fonts_provider.py` & `haruka-bot-1.6.0.post5/haruka_bot/utils/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.6.0.post4/haruka_bot/utils/mobile.js` & `haruka-bot-1.6.0.post5/haruka_bot/utils/mobile.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -151,15 +151,15 @@
     }];
     const emojiFontList = ["Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"];
 
     if (font) {
         // 如果传入了字体名, 则将其添加到字体列表首位
         if (fontSource === "local") {
             needLoadFontList.unshift({
-                fontUrl: `https://fonts.bbot/${font}`,
+                fontUrl: `https://static.graiax/fonts/${font}`,
                 fontFamily: "BBot_Custom_Font",
             });
         } else if (fontSource === "remote") {
             needLoadFontList.unshift({
                 fontUrl: font,
                 fontFamily: "BBot_Custom_Font",
             });
```

### Comparing `haruka-bot-1.6.0.post4/pyproject.toml` & `haruka-bot-1.6.0.post5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,34 +6,35 @@
 dependencies = [
     "click>=8.1.3",
     "httpx>=0.24.1",
     "nonebot-adapter-onebot>=2.2.3",
     "nonebot-plugin-apscheduler>=0.3.0",
     "nonebot2[fastapi]>=2.0.0",
     "playwright>=1.35.0",
-    "pydantic>=1.10.9",
+    "pydantic>=1.10.9, <=2.0",
     "python-dotenv>=1.0.0",
     "tortoise-orm[asyncpg]>=0.19.3",
     "bilireq>=0.2.6",
     "packaging>=23.1",
     "nonebot-plugin-guild-patch>=0.2.3",
     "msvc-runtime>=14.34.31931; sys_platform == \"win32\"",
+    "aunly-captcha-solver>=0.1",
 ]
 dynamic = []
 name = "haruka-bot"
 description = "Push dynamics and live informations from bilibili to QQ. Based on nonebot2."
 readme = "README.md"
 keywords = [
     "nonebot",
     "nonebot2",
     "qqbot",
     "bilibili",
     "bot",
 ]
-version = "1.6.0.post4"
+version = "1.6.0.post5"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.urls]
 homepage = "https://github.com/SK-415/HarukaBot"
 repository = "https://github.com/SK-415/HarukaBot/tree/master/src/plugins/haruka_bot"
```

### Comparing `haruka-bot-1.6.0.post4/PKG-INFO` & `haruka-bot-1.6.0.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka-bot
-Version: 1.6.0.post4
+Version: 1.6.0.post5
 Summary: Push dynamics and live informations from bilibili to QQ. Based on nonebot2.
 License: AGPL-3.0-or-later
 Keywords: nonebot,nonebot2,qqbot,bilibili,bot
 Author-email: SK-415 <2967923486@qq.com>
 Requires-Python: >=3.8,<4.0
 Project-URL: documentation, https://github.com/SK-415/HarukaBot#readme
 Project-URL: homepage, https://github.com/SK-415/HarukaBot
```

