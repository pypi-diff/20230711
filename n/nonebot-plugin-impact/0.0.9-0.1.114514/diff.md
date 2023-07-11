# Comparing `tmp/nonebot_plugin_impact-0.0.9.tar.gz` & `tmp/nonebot_plugin_impact-0.1.114514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_impact-0.0.9.tar", last modified: Tue Jun  6 14:47:52 2023, max compression
+gzip compressed data, was "nonebot_plugin_impact-0.1.114514.tar", last modified: Tue Jul 11 19:57:05 2023, max compression
```

## Comparing `nonebot_plugin_impact-0.0.9.tar` & `nonebot_plugin_impact-0.1.114514.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 14:47:52.262724 nonebot_plugin_impact-0.0.9/
--rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      283 2023-06-06 14:47:52.261723 nonebot_plugin_impact-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 14:47:52.254724 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/
--rw-rw-rw-   0        0        0     1667 2023-06-06 14:37:05.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/__init__.py
--rw-rw-rw-   0        0        0    19722 2023-06-06 14:39:44.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/handle.py
--rw-rw-rw-   0        0        0     2041 2023-06-06 14:34:38.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/txt2img.py
--rw-rw-rw-   0        0        0     8376 2023-06-06 14:34:38.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 14:47:52.260722 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/
--rw-rw-rw-   0        0        0      283 2023-06-06 14:47:52.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-06-06 14:47:52.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 14:47:52.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-06 14:47:52.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-06 14:47:52.000000 nonebot_plugin_impact-0.0.9/nonebot_plugin_impact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 14:47:52.262724 nonebot_plugin_impact-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      503 2023-06-06 14:47:26.000000 nonebot_plugin_impact-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:57:05.342784 nonebot_plugin_impact-0.1.114514/
+-rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.1.114514/LICENSE
+-rw-rw-rw-   0        0        0      306 2023-07-11 19:57:05.341784 nonebot_plugin_impact-0.1.114514/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 19:57:05.334574 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/
+-rw-rw-rw-   0        0        0     2047 2023-07-11 19:53:35.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/__init__.py
+-rw-rw-rw-   0        0        0    20576 2023-07-11 19:49:13.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/handle.py
+-rw-rw-rw-   0        0        0     2041 2023-07-11 19:49:23.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/txt2img.py
+-rw-rw-rw-   0        0        0     8628 2023-07-11 19:54:40.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:57:05.340783 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/
+-rw-rw-rw-   0        0        0      306 2023-07-11 19:57:05.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-07-11 19:57:05.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 19:57:05.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-11 19:57:05.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-11 19:57:05.000000 nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 19:57:05.342784 nonebot_plugin_impact-0.1.114514/setup.cfg
+-rw-rw-rw-   0        0        0      485 2023-07-11 19:56:34.000000 nonebot_plugin_impact-0.1.114514/setup.py
```

### Comparing `nonebot_plugin_impact-0.0.9/LICENSE` & `nonebot_plugin_impact-0.1.114514/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/handle.py` & `nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/handle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,270 +1,310 @@
 import asyncio
 import random
 import time
 from random import choice
 from typing import Tuple
 
-from nonebot.adapters.onebot.v11 import (Bot, GroupMessageEvent, Message,
-                                         MessageSegment)
+from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, Message, MessageSegment
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, RegexGroup
 
 from .txt2img import txt_to_img
 from .utils import utils
 
 
 class Impart:
-    def __init__(self) -> None:
-        """好像没什么东西要初始化的"""
-        ...
-
-
-    async def pk(
-        self,
-        matcher: Matcher,
-        event: GroupMessageEvent
-    ) -> None:
+    @staticmethod
+    async def pk(matcher: Matcher, event: GroupMessageEvent) -> None:
         """pk的响应器"""
         if not (await utils.check_group_allow(str(event.group_id))):
             await matcher.finish(utils.not_allow, at_sender=True)
         uid: str = event.get_user_id()
-        allow: bool = await utils.pkcd_check(uid)     # CD是否允许pk
-        if not allow:       # 如果不允许pk, 则返回
-            await matcher.finish(f"你已经pk不动了喵, 请等待{round(utils.pk_cd_time-(time.time() - utils.pk_cd_data[uid]),3)}秒后再pk喵", at_sender=True)
-        utils.pk_cd_data.update({uid: time.time()})    # 更新CD时间
-        at = await utils.get_at(event)            # 获取at的id, 类型为str
-        if at == uid:   # 如果at的id和uid相同, 则返回
+        allow: bool = await utils.pkcd_check(uid)  # CD是否允许pk
+        if not allow:  # 如果不允许pk, 则返回
+            await matcher.finish(
+                f"你已经pk不动了喵, 请等待{round(utils.pk_cd_time-(time.time() - utils.pk_cd_data[uid]),3)}秒后再pk喵",
+                at_sender=True,
+            )
+        utils.pk_cd_data.update({uid: time.time()})  # 更新CD时间
+        at = await utils.get_at(event)  # 获取at的id, 类型为str
+        if at == uid:  # 如果at的id和uid相同, 则返回
             await matcher.finish("你不能pk自己喵", at_sender=True)
         # rule规定了必须有at, 所以不用判断at是否为寄
         if uid in utils.userdata and at in utils.userdata:  # 如果两个都在userdata里面
-            random_num = random.random()    # 生成一个随机数
+            random_num = random.random()  # 生成一个随机数
             # 如果random_num大于0.5, 则胜利, 否则失败
             if random_num > 0.5:
                 random_num: float = utils.get_random_num()  # 重新生成一个随机数
                 utils.userdata.update(
-                    {uid: round(utils.userdata[uid] + (random_num/2), 3)})  # 更新userdata
+                    {uid: round(utils.userdata[uid] + (random_num / 2), 3)}
+                )  # 更新userdata
                 # 更新userdata
                 utils.userdata.update({at: round(utils.userdata[at] - random_num, 3)})
-                utils.write_user_data()    # 写入文件
-                await matcher.finish(f"对决胜利喵, 你的{choice(utils.jj_variable)}增加了{round(random_num/2,3)}cm喵, 对面则在你的阴影笼罩下减小了{random_num}cm喵", at_sender=True)
+                utils.write_user_data()  # 写入文件
+                await matcher.finish(
+                    f"对决胜利喵, 你的{choice(utils.jj_variable)}增加了{round(random_num/2,3)}cm喵, 对面则在你的阴影笼罩下减小了{random_num}cm喵",
+                    at_sender=True,
+                )
             else:
-                random_num: float = utils.get_random_num()    # 重新生成一个随机数
+                random_num: float = utils.get_random_num()  # 重新生成一个随机数
                 utils.userdata.update(
-                    {uid: round(utils.userdata[uid] - random_num, 3)})  # 更新userdata
+                    {uid: round(utils.userdata[uid] - random_num, 3)}
+                )  # 更新userdata
                 # 更新userdata
-                utils.userdata.update({at: round(utils.userdata[at] + random_num/2, 3)})
-                utils.write_user_data()    # 写入文件
-                await matcher.finish(f"对决失败喵, 在对面牛子的阴影笼罩下你的{choice(utils.jj_variable)}减小了{random_num}cm喵, 对面增加了{round(random_num/2,3)}cm喵", at_sender=True)
+                utils.userdata.update(
+                    {at: round(utils.userdata[at] + random_num / 2, 3)}
+                )
+                utils.write_user_data()  # 写入文件
+                await matcher.finish(
+                    f"对决失败喵, 在对面牛子的阴影笼罩下你的{choice(utils.jj_variable)}减小了{random_num}cm喵, 对面增加了{round(random_num/2,3)}cm喵",
+                    at_sender=True,
+                )
         else:
             # 谁不在userdata里面, 就创建谁
             if uid not in utils.userdata:
-                utils.userdata.update({uid: 10})   # 创建用户
+                utils.userdata.update({uid: 10})  # 创建用户
             if at not in utils.userdata:
-                utils.userdata.update({at: 10})    # 创建用户
-            utils.write_user_data()     # 写入文件
-            del utils.pk_cd_data[uid]   # 删除CD时间
-            await matcher.finish(f"你或对面还没有创建{choice(utils.jj_variable)}喵, 咱全帮你创建了喵, 你们的{choice(utils.jj_variable)}长度都是10cm喵", at_sender=True)
+                utils.userdata.update({at: 10})  # 创建用户
+            utils.write_user_data()  # 写入文件
+            del utils.pk_cd_data[uid]  # 删除CD时间
+            await matcher.finish(
+                f"你或对面还没有创建{choice(utils.jj_variable)}喵, 咱全帮你创建了喵, 你们的{choice(utils.jj_variable)}长度都是10cm喵",
+                at_sender=True,
+            )
 
-    async def dajiao(
-        self,
-        matcher: Matcher,
-        event: GroupMessageEvent
-    ) -> None:
+    @staticmethod
+    async def dajiao(matcher: Matcher, event: GroupMessageEvent) -> None:
         """打胶的响应器"""
         if not (await utils.check_group_allow(str(event.group_id))):
             await matcher.finish(utils.not_allow, at_sender=True)
         uid: str = event.get_user_id()
-        allow = await utils.cd_check(uid)    # CD是否允许打胶
-        if not allow:   # 如果不允许打胶, 则返回
-            await matcher.finish(f"你已经打不动了喵, 请等待{round(utils.dj_cd_time-(time.time() - utils.cd_data[uid]),3)}秒后再打喵", at_sender=True)
-        utils.cd_data.update({uid: time.time()})    # 更新CD时间
-        if uid in utils.userdata:    # 如果在userdata里面
-            random_num = utils.get_random_num()    # 生成一个随机数
+        allow = await utils.cd_check(uid)  # CD是否允许打胶
+        if not allow:  # 如果不允许打胶, 则返回
+            await matcher.finish(
+                f"你已经打不动了喵, 请等待{round(utils.dj_cd_time-(time.time() - utils.cd_data[uid]),3)}秒后再打喵",
+                at_sender=True,
+            )
+        utils.cd_data.update({uid: time.time()})  # 更新CD时间
+        if uid in utils.userdata:  # 如果在userdata里面
+            random_num = utils.get_random_num()  # 生成一个随机数
             utils.userdata.update(
-                {uid: round(utils.userdata[uid] + random_num, 3)})  # 更新userdata
-            utils.write_user_data()    # 写入文件
-            await matcher.finish(f"打胶结束喵, 你的{choice(utils.jj_variable)}很满意喵, 长了{random_num}cm喵, 目前长度为{utils.userdata[uid]}cm喵", at_sender=True)
+                {uid: round(utils.userdata[uid] + random_num, 3)}
+            )  # 更新userdata
+            utils.write_user_data()  # 写入文件
+            await matcher.finish(
+                f"打胶结束喵, 你的{choice(utils.jj_variable)}很满意喵, 长了{random_num}cm喵, 目前长度为{utils.userdata[uid]}cm喵",
+                at_sender=True,
+            )
         else:
-            utils.userdata.update({uid: 10})   # 创建用户
-            utils.write_user_data()    # 写入文件
-            del utils.cd_data[uid]     # 删除CD时间
-            await matcher.finish(f"你还没有创建{choice(utils.jj_variable)}, 咱帮你创建了喵, 目前长度是10cm喵", at_sender=True)
-                
+            utils.userdata.update({uid: 10})  # 创建用户
+            utils.write_user_data()  # 写入文件
+            del utils.cd_data[uid]  # 删除CD时间
+            await matcher.finish(
+                f"你还没有创建{choice(utils.jj_variable)}, 咱帮你创建了喵, 目前长度是10cm喵",
+                at_sender=True,
+            )
 
-    async def suo(
-        self,
-        matcher: Matcher,
-        event: GroupMessageEvent
-    ) -> None:
+    @staticmethod
+    async def suo(matcher: Matcher, event: GroupMessageEvent) -> None:
         """嗦牛子的响应器"""
         if not (await utils.check_group_allow(str(event.group_id))):
             await matcher.finish(utils.not_allow, at_sender=True)
         uid: str = event.get_user_id()
-        allow = await utils.suo_cd_check(uid)   # CD是否允许嗦
-        if not allow:   # 如果不允许嗦, 则返回
-            await matcher.finish(f"你已经嗦不动了喵, 请等待{round(utils.suo_cd_time-(time.time() - utils.suo_cd_data[uid]),3)}秒后再嗦喵", at_sender=True)
-        utils.suo_cd_data.update({uid: time.time()})    # 更新CD时间
-        at: str = await utils.get_at(event)    # 获取at的用户id, 类型为str
+        allow = await utils.suo_cd_check(uid)  # CD是否允许嗦
+        if not allow:  # 如果不允许嗦, 则返回
+            await matcher.finish(
+                f"你已经嗦不动了喵, 请等待{round(utils.suo_cd_time-(time.time() - utils.suo_cd_data[uid]),3)}秒后再嗦喵",
+                at_sender=True,
+            )
+        utils.suo_cd_data.update({uid: time.time()})  # 更新CD时间
+        at: str = await utils.get_at(event)  # 获取at的用户id, 类型为str
         if at == "寄":  # 如果没有at
-            if uid in utils.userdata:   # 如果在userdata里面
-                random_num = utils.get_random_num()    # 生成一个随机数
+            if uid in utils.userdata:  # 如果在userdata里面
+                random_num = utils.get_random_num()  # 生成一个随机数
                 utils.userdata.update(
-                    {uid: round(utils.userdata[uid] + random_num, 3)})  # 更新userdata
-                utils.write_user_data()    # 写入文件
-                await matcher.finish(f"你的{choice(utils.jj_variable)}很满意喵, 嗦长了{random_num}cm喵, 目前长度为{utils.userdata[uid]}cm喵", at_sender=True)
-            else:   # 如果不在userdata里面
-                utils.userdata.update({uid: 10})   # 创建用户
-                utils.write_user_data()    # 写入文件
-                del utils.suo_cd_data[uid]     # 删除CD时间
-                await matcher.finish(f"你还没有创建{choice(utils.jj_variable)}喵, 咱帮你创建了喵, 目前长度是10cm喵", at_sender=True)
+                    {uid: round(utils.userdata[uid] + random_num, 3)}
+                )  # 更新userdata
+                utils.write_user_data()  # 写入文件
+                await matcher.finish(
+                    f"你的{choice(utils.jj_variable)}很满意喵, 嗦长了{random_num}cm喵, 目前长度为{utils.userdata[uid]}cm喵",
+                    at_sender=True,
+                )
+            else:  # 如果不在userdata里面
+                utils.userdata.update({uid: 10})  # 创建用户
+                utils.write_user_data()  # 写入文件
+                del utils.suo_cd_data[uid]  # 删除CD时间
+                await matcher.finish(
+                    f"你还没有创建{choice(utils.jj_variable)}喵, 咱帮你创建了喵, 目前长度是10cm喵",
+                    at_sender=True,
+                )
         elif at in utils.userdata:  # 如果在userdata里面
-            random_num = utils.get_random_num()    # 生成一个随机数
+            random_num = utils.get_random_num()  # 生成一个随机数
             # 更新userdata
             utils.userdata.update({at: round(utils.userdata[at] + random_num, 3)})
-            utils.write_user_data()    # 写入文件
-            await matcher.finish(f"对方的{choice(utils.jj_variable)}很满意喵, 嗦长了{random_num}cm喵, 目前长度为{utils.userdata[at]}cm喵", at_sender=True)
+            utils.write_user_data()  # 写入文件
+            await matcher.finish(
+                f"对方的{choice(utils.jj_variable)}很满意喵, 嗦长了{random_num}cm喵, 目前长度为{utils.userdata[at]}cm喵",
+                at_sender=True,
+            )
         else:
-            utils.userdata.update({at: 10})    # 创建用户
-            utils.write_user_data()    # 写入文件
-            del utils.suo_cd_data[uid]     # 删除CD时间
-            await matcher.finish(f"他还没有创建{choice(utils.jj_variable)}喵, 咱帮他创建了喵, 目前长度是10cm喵", at_sender=True)
-
+            utils.userdata.update({at: 10})  # 创建用户
+            utils.write_user_data()  # 写入文件
+            del utils.suo_cd_data[uid]  # 删除CD时间
+            await matcher.finish(
+                f"他还没有创建{choice(utils.jj_variable)}喵, 咱帮他创建了喵, 目前长度是10cm喵",
+                at_sender=True,
+            )
 
-    async def queryjj(
-        self,
-        matcher: Matcher,
-        event: GroupMessageEvent
-    ) -> None:
+    @staticmethod
+    async def queryjj(matcher: Matcher, event: GroupMessageEvent) -> None:
         """查询某人jj的响应器"""
         if not (await utils.check_group_allow(str(event.group_id))):
             await matcher.finish(utils.not_allow, at_sender=True)
-        uid: str = event.get_user_id()   # 获取用户id, 类型为str
-        at: str = await utils.get_at(event)    # 获取at的用户id, 类型为str
+        uid: str = event.get_user_id()  # 获取用户id, 类型为str
+        at: str = await utils.get_at(event)  # 获取at的用户id, 类型为str
         if at == "寄":  # 如果没有at
             if uid in utils.userdata:  # 如果在userdata里面
-                await matcher.finish(f"你的{choice(utils.jj_variable)}目前长度为{utils.userdata[uid]}cm喵", at_sender=True)
+                await matcher.finish(
+                    f"你的{choice(utils.jj_variable)}目前长度为{utils.userdata[uid]}cm喵",
+                    at_sender=True,
+                )
             else:
-                utils.userdata.update({uid: 10})   # 创建用户
-                utils.write_user_data()    # 写入文件
-                await matcher.finish(f"你还没有创建{choice(utils.jj_variable)}喵, 咱帮你创建了喵, 目前长度是10cm喵", at_sender=True)
+                utils.userdata.update({uid: 10})  # 创建用户
+                utils.write_user_data()  # 写入文件
+                await matcher.finish(
+                    f"你还没有创建{choice(utils.jj_variable)}喵, 咱帮你创建了喵, 目前长度是10cm喵",
+                    at_sender=True,
+                )
         elif at in utils.userdata:  # 如果在userdata里面
-            await matcher.finish(f"他的{choice(utils.jj_variable)}目前长度为{utils.userdata[at]}cm喵", at_sender=True)
+            await matcher.finish(
+                f"他的{choice(utils.jj_variable)}目前长度为{utils.userdata[at]}cm喵",
+                at_sender=True,
+            )
         else:
-            utils.userdata.update({at: 10})    # 创建用户
-            utils.write_user_data()    # 写入文件
-            await matcher.finish(f"他还没有创建{choice(utils.jj_variable)}喵, 咱帮他创建了喵, 目前长度是10cm喵", at_sender=True)
-
+            utils.userdata.update({at: 10})  # 创建用户
+            utils.write_user_data()  # 写入文件
+            await matcher.finish(
+                f"他还没有创建{choice(utils.jj_variable)}喵, 咱帮他创建了喵, 目前长度是10cm喵",
+                at_sender=True,
+            )
 
-    async def jjrank(
-        self,
-        bot: Bot, 
-        matcher: Matcher,
-        event: GroupMessageEvent
-    ) -> None:
+    @staticmethod
+    async def jjrank(bot: Bot, matcher: Matcher, event: GroupMessageEvent) -> None:
         """输出前五后五和自己的排名"""
         if not (await utils.check_group_allow(str(event.group_id))):
             await matcher.finish(utils.not_allow, at_sender=True)
         uid: str = event.get_user_id()
-        rankdata: list = sorted(utils.userdata.items(),
-                        key=lambda x: x[1], reverse=True)   # 排序
+        rankdata: list = sorted(
+            utils.userdata.items(), key=lambda x: x[1], reverse=True
+        )  # 排序
         if len(rankdata) < 5:
             await matcher.finish("目前记录的数据量小于5, 无法显示rank喵")
-        top5: list = rankdata[:5]    # 取前5
-        last5: list = rankdata[-5:]   # 取后5
+        top5: list = rankdata[:5]  # 取前5
+        last5: list = rankdata[-5:]  # 取后5
         index = [i for i, x in enumerate(rankdata) if x[0] == uid]  # 获取用户排名
-        if not index:   # 如果用户没有创建JJ
-            utils.userdata.update({uid: 10})   # 创建用户
-            utils.write_user_data()    # 写入文件
-            await matcher.finish(f"你还没有创建{choice(utils.jj_variable)}看不到rank喵, 咱帮你创建了喵, 目前长度是10cm喵", at_sender=True)
+        if not index:  # 如果用户没有创建JJ
+            utils.userdata.update({uid: 10})  # 创建用户
+            utils.write_user_data()  # 写入文件
+            await matcher.finish(
+                f"你还没有创建{choice(utils.jj_variable)}看不到rank喵, 咱帮你创建了喵, 目前长度是10cm喵",
+                at_sender=True,
+            )
         # top5和end5的信息，然后获取其网名
         top5info = [await bot.get_stranger_info(user_id=int(name[0])) for name in top5]
-        last5info = [await bot.get_stranger_info(user_id=int(name[0])) for name in last5]
+        last5info = [
+            await bot.get_stranger_info(user_id=int(name[0])) for name in last5
+        ]
         top5names = [name["nickname"] for name in top5info]
         last5names = [name["nickname"] for name in last5info]
         # 构造消息，手搓
         reply = "咱只展示前五名和后五名喵\n"
         top5txt = f"{top5names[0]} ------> {top5[0][1]}cm\n{top5names[1]} ------> {top5[1][1]}cm\n{top5names[2]} ------> {top5[2][1]}cm\n{top5names[3]} ------> {top5[3][1]}cm\n{top5names[4]} ------> {top5[4][1]}cm\n"
         last5txt = f"{last5names[0]} ------> {last5[0][1]}cm\n{last5names[1]} ------> {last5[1][1]}cm\n{last5names[2]} ------> {last5[2][1]}cm\n{last5names[3]} ------> {last5[3][1]}cm\n{last5names[4]} ------> {last5[4][1]}cm\n"
         img_bytes = await txt_to_img.txt_to_img(
-            top5txt+".................................\n"*3+last5txt)    # 生成图片
+            top5txt + ".................................\n" * 3 + last5txt
+        )  # 生成图片
         reply2 = f"你的排名为{index[0]+1}喵"
-        await matcher.finish(reply+MessageSegment.image(img_bytes)+reply2, at_sender=True)
-
+        await matcher.finish(
+            reply + MessageSegment.image(img_bytes) + reply2, at_sender=True
+        )
 
+    @staticmethod
     async def yinpa_prehandle(
-        self,
         bot: Bot,
         args: Tuple,
         matcher: Matcher,
         event: GroupMessageEvent,
     ) -> Tuple[int, int, str, str, list]:
         """透群员的预处理环节"""
-        gid, uid  = event.group_id, event.user_id
+        gid, uid = event.group_id, event.user_id
         if not (await utils.check_group_allow(str(gid))):
             await matcher.finish(utils.not_allow, at_sender=True)
         allow = await utils.fuck_cd_check(event)  # CD检查是否允许
         if not allow:
-            await matcher.finish(f"你已经榨不出来任何东西了, 请先休息{round(utils.fuck_cd_time-(time.time() - utils.ejaculation_cd[str(uid)]),3)}秒", at_sender=True)
+            await matcher.finish(
+                f"你已经榨不出来任何东西了, 请先休息{round(utils.fuck_cd_time-(time.time() - utils.ejaculation_cd[str(uid)]),3)}秒",
+                at_sender=True,
+            )
         utils.ejaculation_cd.update({str(uid): time.time()})  # 记录时间
         req_user_card = await utils.get_user_card(bot, group_id=int(gid), qid=int(uid))
         prep_list = await bot.get_group_member_list(group_id=gid)
-        return gid,uid,req_user_card, args[0],prep_list
-    
+        return gid, uid, req_user_card, args[0], prep_list
 
+    @staticmethod
     async def yinpa_member_handle(
-        self,
         prep_list: list,
         req_user_card: str,
         matcher: Matcher,
-        event: GroupMessageEvent
+        event: GroupMessageEvent,
     ) -> str:
         prep_list = [prep.get("user_id", 114514) for prep in prep_list]  # 群友列表
-        target = await utils.get_at(event)    # 获取消息有没有at
-        if target == "寄":              # 没有的话
+        target = await utils.get_at(event)  # 获取消息有没有at
+        if target == "寄":  # 没有的话
             # 随机抽取幸运成员
             prep_list.remove(event.user_id)
             lucky_user = choice(prep_list)
             await matcher.send(f"现在咱将随机抽取一位幸运裙友\n送给{req_user_card}色色！")
-        else:                           # 有的话lucky user就是at的人
+        else:  # 有的话lucky user就是at的人
             lucky_user = target
         return lucky_user
-    
+
+    @staticmethod
     async def yinpa_owner_handle(
-        self,
         uid: int,
         prep_list: list,
         req_user_card: str,
         matcher: Matcher,
     ) -> str:
         lucky_user: str = next(
-            (prep['user_id'] for prep in prep_list if prep['role'] == 'owner'),
+            (prep["user_id"] for prep in prep_list if prep["role"] == "owner"),
             str(uid),
         )
-        if int(lucky_user) == uid:      # 如果群主是自己
+        if int(lucky_user) == uid:  # 如果群主是自己
             del utils.ejaculation_cd[str(uid)]
             await matcher.finish("你透你自己?")
         await matcher.send(f"现在咱将把群主\n送给{req_user_card}色色！")
         return lucky_user
 
-
+    @staticmethod
     async def yinpa_admin_handle(
-        self,
         uid: int,
         prep_list: list,
         req_user_card: str,
         matcher: Matcher,
     ) -> str:
-        admin_id: list = [prep['user_id'] for prep in prep_list if prep['role'] == 'admin']
-        if uid in admin_id:         # 如果自己是管理的话， 移除自己
+        admin_id: list = [
+            prep["user_id"] for prep in prep_list if prep["role"] == "admin"
+        ]
+        if uid in admin_id:  # 如果自己是管理的话， 移除自己
             admin_id.remove(uid)
-        if not admin_id:          # 如果没有管理的话, del cd信息， 然后finish
+        if not admin_id:  # 如果没有管理的话, del cd信息， 然后finish
             del utils.ejaculation_cd[str(uid)]
             await matcher.finish("喵喵喵? 找不到群管理!")
-        lucky_user: str = choice(admin_id)   # random抽取一个管理
+        lucky_user: str = choice(admin_id)  # random抽取一个管理
         await matcher.send(f"现在咱将随机抽取一位幸运管理\n送给{req_user_card}色色！")
         return lucky_user
 
     async def yinpa_identity_handle(
         self,
         command: str,
         prep_list: list,
@@ -273,52 +313,59 @@
         event: GroupMessageEvent,
     ) -> str:
         uid: int = event.user_id
         if "群主" in command:  # 如果发送的命令里面含有群主， 说明在透群主
             return await self.yinpa_owner_handle(uid, prep_list, req_user_card, matcher)
         elif "管理" in command:  # 如果发送的命令里面含有管理， 说明在透管理
             return await self.yinpa_admin_handle(uid, prep_list, req_user_card, matcher)
-        else:       # 最后是群员
-            return await self.yinpa_member_handle(prep_list, req_user_card, matcher, event)
-    
+        else:  # 最后是群员
+            return await self.yinpa_member_handle(
+                prep_list, req_user_card, matcher, event
+            )
 
     async def yinpa(
         self,
-        bot: Bot, 
+        bot: Bot,
         matcher: Matcher,
-        event: GroupMessageEvent, 
-        args: Tuple = RegexGroup()
+        event: GroupMessageEvent,
+        args: Tuple = RegexGroup(),
     ) -> None:
-        gid, uid, req_user_card, command ,prep_list= await self.yinpa_prehandle(matcher=matcher, bot=bot, args=args, event=event)
-        lucky_user: str = await self.yinpa_identity_handle(command=command, prep_list=prep_list, req_user_card=req_user_card, matcher=matcher, event=event)
+        gid, uid, req_user_card, command, prep_list = await self.yinpa_prehandle(
+            matcher=matcher, bot=bot, args=args, event=event
+        )
+        lucky_user: str = await self.yinpa_identity_handle(
+            command=command,
+            prep_list=prep_list,
+            req_user_card=req_user_card,
+            matcher=matcher,
+            event=event,
+        )
         # 获取群名片或者网名
         lucky_user_card = await utils.get_user_card(bot, gid, int(lucky_user))
         # 1--100的随机数， 保留三位
         ejaculation = round(random.uniform(1, 100), 3)
         try:
             temp = (
-                utils.ejaculation_data[lucky_user][utils.get_today()][
-                    "ejaculation"
-                ]
+                utils.ejaculation_data[lucky_user][utils.get_today()]["ejaculation"]
                 + ejaculation
             )
             await utils.update_ejaculation(round(temp, 3), lucky_user)
         except Exception:
             await utils.update_ejaculation(ejaculation, lucky_user)
         await asyncio.sleep(2)  # 休眠2秒, 更有效果
         # 准备调用api, 用来获取头像
         repo_1 = f"好欸！{req_user_card}({uid})用时{random.randint(1, 20)}秒 \n给 {lucky_user_card}({lucky_user}) 注入了{ejaculation}毫升的脱氧核糖核酸, 当日总注入量为：{utils.get_today_ejaculation(lucky_user)}"
-        await matcher.send(repo_1 + MessageSegment.image(f"http://q1.qlogo.cn/g?b=qq&nk={lucky_user}&s=640"))  # 结束
-
+        await matcher.send(
+            repo_1
+            + MessageSegment.image(f"http://q1.qlogo.cn/g?b=qq&nk={lucky_user}&s=640")
+        )  # 结束
 
+    @staticmethod
     async def open_module(
-        self,
-        matcher: Matcher,
-        event: GroupMessageEvent,
-        args: Tuple = RegexGroup()
+        matcher: Matcher, event: GroupMessageEvent, args: Tuple = RegexGroup()
     ) -> None:
         """开关"""
         gid = str(event.group_id)
         command: str = args[0]
         if "开启" in command or "开始" in command:
             if gid in utils.groupdata:
                 utils.groupdata[gid]["allow"] = True
@@ -330,48 +377,49 @@
             if gid in utils.groupdata:
                 utils.groupdata[gid]["allow"] = False
             else:
                 utils.groupdata.update({gid: {"allow": False}})
             utils.write_group_data()
             await matcher.finish("功能已禁用喵")
 
-
+    @staticmethod
     async def query_injection(
-        self, 
-        matcher: Matcher,
-        event: GroupMessageEvent, 
-        args: Message = CommandArg()
+        matcher: Matcher, event: GroupMessageEvent, args: Message = CommandArg()
     ) -> None:
         """查询某人的注入量"""
         if not (await utils.check_group_allow(str(event.group_id))):
             await matcher.finish(utils.not_allow, at_sender=True)
         target = args.extract_plain_text()  # 获取命令参数
         user_id: str = event.get_user_id()
         # 判断带不带at
-        [object_id, replay1] = [await utils.get_at(event), "该用户"] if await utils.get_at(event) != "寄" else [user_id, "您"]
-        ejaculation = 0             # 先初始化0
+        [object_id, replay1] = (
+            [await utils.get_at(event), "该用户"]
+            if await utils.get_at(event) != "寄"
+            else [user_id, "您"]
+        )
+        ejaculation = 0  # 先初始化0
         if "历史" in target or "全部" in target:
             try:
                 date = utils.ejaculation_data[object_id]  # 对象不存在直接输出0
             except Exception:
                 await matcher.finish(f"{replay1}历史总被注射量为0ml")
-            pic_string: str = ""            # 文字， 准备弄成图片
-            for key in date:                # 遍历所有的日期
+            pic_string: str = ""  # 文字， 准备弄成图片
+            for key in date:  # 遍历所有的日期
                 temp = date[key]["ejaculation"]
-                ejaculation += temp             # 注入量求和
+                ejaculation += temp  # 注入量求和
                 pic_string += f"{key}\t\t{temp}\n"
-            
-            await matcher.finish(MessageSegment.text(f"{replay1}历史总被注射量为{ejaculation}ml")+MessageSegment.image(await txt_to_img.txt_to_img(pic_string)))
+
+            await matcher.finish(
+                MessageSegment.text(f"{replay1}历史总被注射量为{ejaculation}ml")
+                + MessageSegment.image(await txt_to_img.txt_to_img(pic_string))
+            )
         else:
             ejaculation = utils.get_today_ejaculation(object_id)  # 获取对象当天的注入量
             await matcher.finish(f"{replay1}当日总被注射量为{ejaculation}ml")
 
-
-    async def yinpa_introduce(
-        self,
-        matcher: Matcher
-    ) -> None:
+    @staticmethod
+    async def yinpa_introduce(matcher: Matcher) -> None:
         """输出用法"""
         await matcher.send(MessageSegment.image(await utils.plugin_usage()))
 
 
-impart = Impart()
+impart = Impart()
```

### Comparing `nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/txt2img.py` & `nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/txt2img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.0.9/nonebot_plugin_impact/utils.py` & `nonebot_plugin_impact-0.1.114514/nonebot_plugin_impact/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,168 +19,177 @@
             self.write_user_data()
             self.ejaculation_data = {}
             self.write_ejaculation_data()
             self.groupdata = {}
             self.write_group_data()
         else:
             if os.path.exists(f"{self.data_path}/userdata.json"):  # 读取用户数据
-                with open(f"{self.data_path}/userdata.json", "r", encoding="utf-8") as f:
-                    self.userdata = json.load(f)        # json结构 {"user_id":int}
-            else:   # 不存在则创建
+                with open(
+                    f"{self.data_path}/userdata.json", "r", encoding="utf-8"
+                ) as f:
+                    self.userdata = json.load(f)  # json结构 {"user_id":int}
+            else:  # 不存在则创建
                 self.userdata = {}
                 self.write_user_data()
             if os.path.exists(f"{self.data_path}/groupdata.json"):
-                with open(f"{self.data_path}/groupdata.json","r",encoding="utf-8") as f:
+                with open(
+                    f"{self.data_path}/groupdata.json", "r", encoding="utf-8"
+                ) as f:
                     self.groupdata = json.load(f)
             else:
                 self.groupdata = {}
-                self.write_group_data()     # json结构{"group_id": {"allow": true|false}}
+                self.write_group_data()  # json结构{"group_id": {"allow": true|false}}
             if os.path.exists(f"{self.data_path}/ejaculation_data.json"):  # 读取用户数据
-                with open(f"{self.data_path}/ejaculation_data.json", "r", encoding="utf-8")as f:
+                with open(
+                    f"{self.data_path}/ejaculation_data.json", "r", encoding="utf-8"
+                ) as f:
                     self.ejaculation_data = json.load(f)
             else:
                 self.ejaculation_data = {}
-                self.write_ejaculation_data()   # 这种结构, 不想重构也不想新建json了，所以放宽了这么多{"user_id": {"date": {"ejaculation": 123}}}
+                self.write_ejaculation_data()  # 这种结构, 不想重构也不想新建json了，所以放宽了这么多{"user_id": {"date": {"ejaculation": 123}}}
         self.usage = """指令1: 嗦牛子 (给目标牛牛增加长度, 自己或者他人, 通过艾特选择对象, 没有at时目标是自己)
-        指令2: 打胶 | 开导 (给自己牛牛增加长度)
-        指令3: pk | 对决 (普通的pk,单纯的random实现输赢, 胜利方获取败方随机数/2的牛牛长度)
-        指令4: 查询 (目标牛牛长度, 自己或者他人, 通过艾特选择对象, 没有at时目标是自己)
-        指令5: jj排行榜 | jj排名 | jj榜单 | jjrank (字面意思, 输出倒数五位和前五位, 以及自己的排名)
-        指令6: 开启淫趴|禁止淫趴 (由管理员 | 群主 | SUPERUSERS开启或者关闭淫趴)
-        指令7: 日群友|透群友|日群主|透群主|日管理|透管理  (字面意思, 当使用透群友的时候如果at了人那么直接指定)
-        指令8: 注入查询 | 摄入查询 (查询目标被透注入的量，后接(历史|全部), 可查看总被摄入的量, 无艾特的时候是自己, 有at的时候是目标)
-        指令9: 淫趴介绍 | 淫趴说明| 淫趴帮助 (输出淫趴插件的命令列表)"""
-        self.not_allow = "群内还未开启淫趴游戏, 请管理员或群主发送\"开启淫趴\", \"禁止淫趴\"以开启/关闭该功能"  # 未开启该功能的send信息
-        self.jj_variable = ["牛子", "牛牛", "丁丁", "JJ"]     # JJ变量
+指令2: 打胶 | 开导 (给自己牛牛增加长度)
+指令3: pk | 对决 (普通的pk,单纯的random实现输赢, 胜利方获取败方随机数/2的牛牛长度)
+指令4: 查询 (目标牛牛长度, 自己或者他人, 通过艾特选择对象, 没有at时目标是自己)
+指令5: jj排行榜 | jj排名 | jj榜单 | jjrank (字面意思, 输出倒数五位和前五位, 以及自己的排名)
+指令6: 开启淫趴|禁止淫趴 (由管理员 | 群主 | SUPERUSERS开启或者关闭淫趴)
+指令7: 日群友|透群友|日群主|透群主|日管理|透管理  (字面意思, 当使用透群友的时候如果at了人那么直接指定)
+指令8: 注入查询 | 摄入查询 (查询目标被透注入的量，后接(历史|全部), 可查看总被摄入的量, 无艾特的时候是自己, 有at的时候是目标)
+指令9: 淫趴介绍 | 淫趴说明| 淫趴帮助 (输出淫趴插件的命令列表)"""
+        self.not_allow = '群内还未开启淫趴游戏, 请管理员或群主发送"开启淫趴", "禁止淫趴"以开启/关闭该功能'  # 未开启该功能的send信息
+        self.jj_variable = ["牛子", "牛牛", "丁丁", "JJ"]  # JJ变量
         self.cd_data = {}  # 冷却数据
-        self.pk_cd_data = {}   # pk冷却数据
+        self.pk_cd_data = {}  # pk冷却数据
         self.suo_cd_data = {}  # 嗦牛子冷却数据
         self.ejaculation_cd = {}  # 射精CD
-        config = nonebot.get_driver().config       # 获取配置
-        self.dj_cd_time: int = getattr(config, "djcdtime", 300)     # 打胶冷却时间
-        self.pk_cd_time: int = getattr(config, "pkcdtime", 60)     # pk冷却时间
-        self.suo_cd_time: int = getattr(config, "suocdtime", 300)     # 嗦牛子冷却时间
-        self.fuck_cd_time: int = getattr(config, "fuckcdtime", 3600)     # 透群友冷却时间
-
-
+        config = nonebot.get_driver().config  # 获取配置
+        self.dj_cd_time: int = getattr(config, "djcdtime", 300)  # 打胶冷却时间
+        self.pk_cd_time: int = getattr(config, "pkcdtime", 60)  # pk冷却时间
+        self.suo_cd_time: int = getattr(config, "suocdtime", 300)  # 嗦牛子冷却时间
+        self.fuck_cd_time: int = getattr(config, "fuckcdtime", 3600)  # 透群友冷却时间
 
     def write_group_data(self) -> None:
         """写入群配置"""
         with open(f"{self.data_path}/groupdata.json", "w", encoding="utf-8") as f:
             json.dump(self.groupdata, f, indent=4, ensure_ascii=False)
 
-
     def write_user_data(self) -> None:
         """写入用户数据"""
         with open(f"{self.data_path}/userdata.json", "w", encoding="utf-8") as f:
             json.dump(self.userdata, f, indent=4)
 
-
     def write_ejaculation_data(self) -> None:
         """写入注入数据"""
-        with open(f"{self.data_path}/ejaculation_data.json", "w", encoding="utf-8") as f:
+        with open(
+            f"{self.data_path}/ejaculation_data.json", "w", encoding="utf-8"
+        ) as f:
             json.dump(self.ejaculation_data, f, indent=4, ensure_ascii=False)
 
-
-    async def rule(self, event: GroupMessageEvent) -> bool:
+    @staticmethod
+    async def rule(event: GroupMessageEvent) -> bool:
         """rule检查, 是否有at"""
         msg = event.get_message()
         return next(
-            (
-                msg_seg.data["qq"] != "all"
-                for msg_seg in msg
-                if msg_seg.type == "at"
-            ),
+            (msg_seg.data["qq"] != "all" for msg_seg in msg if msg_seg.type == "at"),
             False,
         )
 
-    async def get_at(self, event: GroupMessageEvent) -> str:
+    @staticmethod
+    async def get_at(event: GroupMessageEvent) -> str:
         """获取at的qq号, 不存在则返回寄, 类型为str"""
         msg = event.get_message()
         return next(
             (
                 "寄" if msg_seg.data["qq"] == "all" else str(msg_seg.data["qq"])
                 for msg_seg in msg
                 if msg_seg.type == "at"
             ),
             "寄",
         )
 
-
     async def cd_check(self, uid: str) -> bool:
         """冷却检查"""
-        cd = time.time() - self.cd_data[uid] if uid in self.cd_data else self.dj_cd_time+1
+        cd = (
+            time.time() - self.cd_data[uid]
+            if uid in self.cd_data
+            else self.dj_cd_time + 1
+        )
         return cd > self.dj_cd_time
 
-
     async def pkcd_check(self, uid: str) -> bool:
         """pk冷却检查"""
-        cd = time.time() - self.pk_cd_data[uid] if uid in self.pk_cd_data else self.pk_cd_time+1
+        cd = (
+            time.time() - self.pk_cd_data[uid]
+            if uid in self.pk_cd_data
+            else self.pk_cd_time + 1
+        )
         return cd > self.pk_cd_time
 
-
     async def suo_cd_check(self, uid: str) -> bool:
         """嗦牛子冷却检查"""
-        cd = time.time() - self.suo_cd_data[uid] if uid in self.suo_cd_data else self.suo_cd_time+1
+        cd = (
+            time.time() - self.suo_cd_data[uid]
+            if uid in self.suo_cd_data
+            else self.suo_cd_time + 1
+        )
         return cd > self.suo_cd_time
 
-
     async def fuck_cd_check(self, event: GroupMessageEvent) -> bool:
         """透群友检查"""
         uid = event.get_user_id()
-        cd = time.time() - self.ejaculation_cd[uid] if uid in self.ejaculation_cd else self.fuck_cd_time+1
+        cd = (
+            time.time() - self.ejaculation_cd[uid]
+            if uid in self.ejaculation_cd
+            else self.fuck_cd_time + 1
+        )
         return (
             cd > self.fuck_cd_time
             or event.get_user_id() in nonebot.get_driver().config.superusers
         )
 
-
     async def check_group_allow(self, gid: str) -> bool:
         """检查群是否允许"""
         return self.groupdata[gid]["allow"] if gid in self.groupdata else False
 
-
-    def get_today(self) -> str:
-        """获取当前年月日  2023-02-04  """
+    @staticmethod
+    def get_today() -> str:
+        """获取当前年月日  2023-02-04"""
         return time.strftime("%Y-%m-%d", time.localtime())
 
-
     async def update_ejaculation(self, ejaculation: float, lucky_user: str) -> None:
         """更新ejaculation_data数据并且写入json"""
         if lucky_user in self.ejaculation_data:
             target_dict: dict = self.ejaculation_data[lucky_user]
             target_dict[self.get_today()] = {"ejaculation": ejaculation}
             self.ejaculation_data.update({lucky_user: target_dict})
         else:
             target_dict = {lucky_user: {self.get_today(): {"ejaculation": ejaculation}}}
             self.ejaculation_data.update(target_dict)
         self.write_ejaculation_data()
 
-
     def get_today_ejaculation(self, user_id: str) -> float:
         """获取当日注入的量"""
         try:
             return self.ejaculation_data[user_id][self.get_today()]["ejaculation"]
         except Exception:
             return 0
 
-
-    def get_random_num(self) -> float:
+    @staticmethod
+    def get_random_num() -> float:
         """获取随机数 0.1的概率是1-2随机获取, 剩下0.9是0-1"""
         rand_num = random.random()
         rand_num = random.uniform(0, 1) if rand_num > 0.1 else random.uniform(1, 2)
         return round(rand_num, 3)
 
-
-    async def get_user_card(self, bot: Bot, group_id: int, qid: int) -> str:
+    @staticmethod
+    async def get_user_card(bot: Bot, group_id: int, qid: int) -> str:
         """返还用户nickname"""
-        user_info: dict = await bot.get_group_member_info(group_id=group_id, user_id=qid)
+        user_info: dict = await bot.get_group_member_info(
+            group_id=group_id, user_id=qid
+        )
         return user_info["card"] or user_info["nickname"]
 
     async def plugin_usage(self) -> bytes:
         return await txt_to_img.txt_to_img(self.usage)
 
 
-
 utils = Utils()
-
-
```

