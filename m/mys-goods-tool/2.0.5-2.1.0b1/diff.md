# Comparing `tmp/mys_goods_tool-2.0.5.tar.gz` & `tmp/mys_goods_tool-2.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mys_goods_tool-2.0.5.tar", max compression
+gzip compressed data, was "mys_goods_tool-2.1.0b1.tar", max compression
```

## Comparing `mys_goods_tool-2.0.5.tar` & `mys_goods_tool-2.1.0b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/LICENSE
--rw-r--r--   0        0        0     3734 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/mys_goods_tool/__init__.py
--rw-r--r--   0        0        0     2226 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/mys_goods_tool/__main__.py
--rw-r--r--   0        0        0    57821 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/mys_goods_tool/api.py
--rw-r--r--   0        0        0     5536 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/mys_goods_tool/custom_css.py
--rw-r--r--   0        0        0     7599 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/custom_widget.py
--rw-r--r--   0        0        0     9681 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/data_model.py
--rw-r--r--   0        0        0    17597 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/exchange_mode.py
--rw-r--r--   0        0        0    43495 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/exchange_plan_view.py
--rw-r--r--   0        0        0     6910 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/gt3-localized.html
--rw-r--r--   0        0        0     6840 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/gt3.html
--rw-r--r--   0        0        0     6890 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/index.html
--rw-r--r--   0        0        0    10861 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/gt.js
--rw-r--r--   0        0        0    14792 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/gt4.js
--rw-r--r--   0        0        0   366500 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/jquery.js
--rw-r--r--   0        0        0     6831 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/localized.html
--rw-r--r--   0        0        0    10717 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest.py
--rw-r--r--   0        0        0    22213 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/login_view.py
--rw-r--r--   0        0        0    12814 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/tui.py
--rw-r--r--   0        0        0    17901 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/user_data.py
--rw-r--r--   0        0        0    10056 2023-06-23 14:24:06.811754 mys_goods_tool-2.0.5/mys_goods_tool/utils.py
--rw-r--r--   0        0        0     1639 2023-06-23 14:24:06.811754 mys_goods_tool-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     5119 1970-01-01 00:00:00.000000 mys_goods_tool-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/LICENSE
+-rw-r--r--   0        0        0     4258 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/__init__.py
+-rw-r--r--   0        0        0     2278 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/__main__.py
+-rw-r--r--   0        0        0    60902 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/api.py
+-rw-r--r--   0        0        0     5536 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/custom_css.py
+-rw-r--r--   0        0        0     7599 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/custom_widget.py
+-rw-r--r--   0        0        0     9816 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/data_model.py
+-rw-r--r--   0        0        0    17998 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/exchange_mode.py
+-rw-r--r--   0        0        0    43948 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/exchange_plan_view.py
+-rw-r--r--   0        0        0     6910 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/gt3-localized.html
+-rw-r--r--   0        0        0     6840 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/gt3.html
+-rw-r--r--   0        0        0     6890 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/index.html
+-rw-r--r--   0        0        0    10861 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/gt.js
+-rw-r--r--   0        0        0    14792 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/gt4.js
+-rw-r--r--   0        0        0   366500 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/jquery.js
+-rw-r--r--   0        0        0     6831 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/localized.html
+-rw-r--r--   0        0        0    10717 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest.py
+-rw-r--r--   0        0        0    22069 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/login_view.py
+-rw-r--r--   0        0        0    13749 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/tui.py
+-rw-r--r--   0        0        0    19168 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/user_data.py
+-rw-r--r--   0        0        0    10534 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/utils.py
+-rw-r--r--   0        0        0     1646 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     5645 1970-01-01 00:00:00.000000 mys_goods_tool-2.1.0b1/PKG-INFO
```

### Comparing `mys_goods_tool-2.0.5/LICENSE` & `mys_goods_tool-2.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/README.md` & `mys_goods_tool-2.1.0b1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -12,15 +12,21 @@
   <img alt="代码行数" src="https://img.shields.io/tokei/lines/github/Ljzd-PRO/Mys_Goods_Tool?style=for-the-badge">
   <img alt="构建结果" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/build-v2.yml?event=pull_request&style=for-the-badge">
   <img alt="Python版本兼容性测试" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/python-package.yml?event=pull_request&label=Versions%20Test&style=for-the-badge">
 </div>
 
 ### 更新说明
 
-- 修复短信验证码发送失败的问题 #105 #94 #104 - #126 by @Night-stars-1
+v2.1.0-beta.1
+
+- 兑换请求Headers增加与修改了 `Referer`, `x-rpc-device_fp`, `x-rpc-verify_key`, `Origin` 等字段，可能修复兑换失败的问题
+- 修复登陆时因为连接断开（client has been closed）而导致登陆失败的问题
+- 防止因配置文件中默认存在 `device_config`, `salt_config` 而导致更新后默认配置被原配置覆盖的问题
+- 若需要修改 `device_config` 配置，修改后还设置用户数据文件中 `preference.override_device_and_salt` 为 `true` 以覆盖默认值
+- 修复Unix下即使安装了 uvloop 也找不到，无法应用的问题
 
 ## 功能和特性
 
 - [x] 使用 [Textual](https://github.com/Textualize/textual) 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
 - [x] 短信验证码登录（只需接收一次验证码）
 - [x] 内置人机验证页面，无需前往官网验证
 - [x] 多账号支持
```

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/__main__.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 def main(textual_app: Optional[App] = None):
     arg = arg_parser.parse_args()
 
     if arg.conf is not None:
         mys_goods_tool.user_data.CONFIG_PATH = arg.conf
-        mys_goods_tool.user_data.config = load_config()
+        mys_goods_tool.user_data.config, mys_goods_tool.user_data.different_device_and_salt = load_config()
     if arg.mode == "guide":
         if textual_app is None:
             from mys_goods_tool.tui import TuiApp
             textual_app = TuiApp()
         textual_app.run()
     elif arg.mode == "exchange-simple":
         exchange_mode_simple()
```

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/api.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from typing import List, Optional, Tuple, Dict, Any, Union
+import time
+from typing import List, Optional, Tuple, Dict, Any, Union, Type
 from urllib.parse import urlencode
 
 import httpx
 import tenacity
 from pydantic import ValidationError, BaseModel
 from requests.utils import dict_from_cookiejar
 
 from mys_goods_tool.data_model import GameRecord, GameInfo, Good, Address, BaseApiStatus, MmtData, GeetestResult, \
     GetCookieStatus, \
-    CreateMobileCaptchaStatus, GetGoodDetailStatus, ExchangeStatus, GeetestResultV4
+    CreateMobileCaptchaStatus, GetGoodDetailStatus, ExchangeStatus, GeetestResultV4, GetFpStatus
 from mys_goods_tool.user_data import config as conf, UserAccount, BBSCookies, ExchangePlan, ExchangeResult
 from mys_goods_tool.utils import generate_device_id, logger, generate_ds, Subscribe, \
-    NtpTime, get_async_retry
+    NtpTime, get_async_retry, generate_seed_id, generate_fp_locally
 
 URL_LOGIN_TICKET_BY_CAPTCHA = "https://webapi.account.mihoyo.com/Api/login_by_mobilecaptcha"
 URL_LOGIN_TICKET_BY_PASSWORD = "https://webapi.account.mihoyo.com/Api/login_by_password"
 URL_MULTI_TOKEN_BY_LOGIN_TICKET = "https://api-takumi.mihoyo.com/auth/api/getMultiTokenByLoginTicket?login_ticket={0}&token_types=3&uid={1}"
 URL_COOKIE_TOKEN_BY_CAPTCHA = "https://api-takumi.mihoyo.com/account/auth/api/webLoginByMobile"
 URL_COOKIE_TOKEN_BY_STOKEN = "https://passport-api.mihoyo.com/account/auth/api/getCookieAccountInfoBySToken"
 URL_LTOKEN_BY_STOKEN = "https://passport-api.mihoyo.com/account/auth/api/getLTokenBySToken"
@@ -31,14 +32,15 @@
 URL_CHECK_GOOD = "https://api-takumi.mihoyo.com/mall/v1/web/goods/detail?app_id=1&point_sn=myb&goods_id={}"
 URL_EXCHANGE = "https://api-takumi.miyoushe.com/mall/v1/web/goods/exchange"
 URL_ADDRESS = "https://api-takumi.mihoyo.com/account/address/list?t={}"
 URL_REGISTRABLE = "https://webapi.account.mihoyo.com/Api/is_mobile_registrable?mobile={mobile}&t={t}"
 URL_CREATE_MMT = "https://webapi.account.mihoyo.com/Api/create_mmt?scene_type=1&now={now}&reason=user.mihoyo.com%2523%252Flogin%252Fcaptcha&action_type=login_by_mobile_captcha&t={t}"
 URL_CREATE_MOBILE_CAPTCHA = "https://webapi.account.mihoyo.com/Api/create_mobile_captcha"
 URL_GET_USER_INFO = "https://bbs-api.miyoushe.com/user/api/getUserFullInfo?uid={uid}"
+URL_GET_DEVICE_FP = "https://public-data-api.mihoyo.com/device-fp/api/getFp"
 
 HEADERS_WEBAPI = {
     "Host": "webapi.account.mihoyo.com",
     "Connection": "keep-alive",
     "sec-ch-ua": conf.device_config.UA,
     "DNT": "1",
     "x-rpc-device_model": conf.device_config.X_RPC_DEVICE_MODEL_PC,
@@ -191,27 +193,32 @@
     "Accept-Encoding":
         "gzip, deflate, br",
     "Accept-Language":
         "zh-CN,zh-Hans;q=0.9",
     "Connection":
         "keep-alive",
     "Content-Type":
-        "application/json;charset=utf-8",
+        "application/json",
     "Host":
         "api-takumi.miyoushe.com",
     "Origin":
-        "https://webstatic.mihoyo.com",
+        "https://webstatic.miyoushe.com",
+    "Referer":
+        "https://webstatic.miyoushe.com/",
     "User-Agent":
         conf.device_config.USER_AGENT_MOBILE,
     "x-rpc-app_version":
         conf.device_config.X_RPC_APP_VERSION,
     "x-rpc-channel":
         "appstore",
     "x-rpc-client_type":
         "1",
+    "x-rpc-verify_key":
+        "bll8iq97cem8",
+    "x-rpc-device_fp": None,
     "x-rpc-device_id": None,
     "x-rpc-device_model":
         conf.device_config.X_RPC_DEVICE_MODEL_MOBILE,
     "x-rpc-device_name":
         conf.device_config.X_RPC_DEVICE_NAME_MOBILE,
     "x-rpc-sys_version":
         conf.device_config.X_RPC_SYS_VERSION
@@ -229,23 +236,28 @@
     "Accept-Encoding": "gzip, deflate, br"
 }
 
 IncorrectReturn = (KeyError, TypeError, AttributeError, IndexError, ValidationError)
 """米游社API返回数据无效会触发的异常组合"""
 
 
-def is_incorrect_return(exception: Exception) -> bool:
-    """判断是否是米游社API返回数据无效的异常"""
+def is_incorrect_return(exception: Exception, *addition_exceptions: Type[Exception]) -> bool:
+    """
+    判断是否是米游社API返回数据无效的异常
+    :param exception: 异常对象
+    :param addition_exceptions: 额外的异常类型，用于触发判断
+    """
     """
         return exception in IncorrectReturn or
             exception.__cause__ in IncorrectReturn or
             isinstance(exception, IncorrectReturn) or
             isinstance(exception.__cause__, IncorrectReturn)
     """
-    return isinstance(exception, IncorrectReturn) or isinstance(exception.__cause__, IncorrectReturn)
+    exceptions = IncorrectReturn + addition_exceptions
+    return isinstance(exception, exceptions) or isinstance(exception.__cause__, exceptions)
 
 
 class ApiResultHandler(BaseModel):
     """
     API返回的数据处理器
     """
     content: Dict[str, Any]
@@ -341,27 +353,20 @@
     """
     获取米哈游游戏的详细信息，若返回`None`说明获取失败
 
     :param retry: 是否允许重试
     """
     headers = HEADERS_GAME_LIST.copy()
     try:
-        subscribe = Subscribe()
         async for attempt in get_async_retry(retry):
             with attempt:
                 headers["DS"] = generate_ds()
                 async with httpx.AsyncClient() as client:
                     res = await client.get(URL_GAME_LIST, headers=headers, timeout=conf.preference.timeout)
                 api_result = ApiResultHandler(res.json())
-                if api_result.invalid_ds:
-                    logger.info(
-                        f"获取游戏信息(GameInfo): DS无效，正在在线获取salt以重新生成...")
-                    await subscribe.load()
-                    headers["User-Agent"] = conf.device_config.USER_AGENT_MOBILE
-                    headers["DS"] = generate_ds()
                 return BaseApiStatus(success=True), list(
                     map(GameInfo.parse_obj, api_result.data["list"]))
     except tenacity.RetryError as e:
         if is_incorrect_return(e):
             logger.exception(f"获取游戏信息(GameInfo) - 服务器没有正确返回")
             logger.debug(f"网络请求返回: {res.text}")
             return BaseApiStatus(incorrect_return=True), None
@@ -377,15 +382,16 @@
     :param account: 用户账户数据
     :param retry: 是否允许重试
     """
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
                 async with httpx.AsyncClient() as client:
-                    res = await client.get(URL_MYB, headers=HEADERS_MYB, cookies=account.cookies.dict(),
+                    res = await client.get(URL_MYB, headers=HEADERS_MYB,
+                                           cookies=account.cookies.dict(v2_stoken=True, cookie_type=True),
                                            timeout=conf.preference.timeout)
                 api_result = ApiResultHandler(res.json())
                 if api_result.login_expired:
                     logger.info(
                         f"获取用户米游币 - 用户 {account.bbs_uid} 登录失效")
                     logger.debug(f"网络请求返回: {res.text}")
                     return BaseApiStatus(login_expired=True), None
@@ -414,33 +420,27 @@
         "os_version": "30",
         "platform": "Android",
         "registration_id": "1a0018970a5c00e814d"
     }
     headers = HEADERS_DEVICE.copy()
     headers["x-rpc-device_id"] = account.device_id_android
     try:
-        subscribe = Subscribe()
         async for attempt in get_async_retry(retry):
             with attempt:
                 headers["DS"] = generate_ds(data)
                 async with httpx.AsyncClient() as client:
                     res = await client.post(URL_DEVICE_LOGIN, headers=headers, json=data,
-                                            cookies=account.cookies.dict(),
+                                            cookies=account.cookies.dict(v2_stoken=True, cookie_type=True),
                                             timeout=conf.preference.timeout)
                 api_result = ApiResultHandler(res.json())
                 if api_result.login_expired:
                     logger.info(
                         f"设备登录(device_login) - 用户 {account.bbs_uid} 登录失效")
                     logger.debug(f"网络请求返回: {res.text}")
                     return BaseApiStatus(login_expired=True)
-                if api_result.invalid_ds:
-                    logger.info(
-                        f"设备登录(device_login): DS无效，正在在线获取salt以重新生成...")
-                    await subscribe.load()
-                    headers["DS"] = generate_ds(data)
                 if res.json()["message"] != "OK":
                     raise ValueError
                 else:
                     return BaseApiStatus(success=True)
     except tenacity.RetryError as e:
         if is_incorrect_return(e):
             logger.exception(f"设备登录(device_login) - 服务器没有正确返回")
@@ -470,26 +470,27 @@
     headers["x-rpc-device_id"] = account.device_id_android
     try:
         subscribe = Subscribe()
         async for attempt in get_async_retry(retry):
             with attempt:
                 headers["DS"] = generate_ds(data)
                 async with httpx.AsyncClient() as client:
-                    res = await client.post(URL_DEVICE_SAVE, headers=headers, json=data, cookies=account.cookies.dict(),
-                                            timeout=conf.preference.timeout)
+                    res = await client.post(
+                        URL_DEVICE_SAVE,
+                        headers=headers,
+                        json=data,
+                        cookies=account.cookies.dict(v2_stoken=True, cookie_type=True),
+                        timeout=conf.preference.timeout
+                    )
                 api_result = ApiResultHandler(res.json())
                 if api_result.login_expired:
                     logger.info(
                         f"设备保存(device_save) - 用户 {account.bbs_uid} 登录失效")
                     logger.debug(f"网络请求返回: {res.text}")
                     return BaseApiStatus(login_expired=True)
-                if api_result.invalid_ds:
-                    logger.info(
-                        f"设备保存(device_save): DS无效，正在在线获取salt以重新生成...")
-                    await subscribe.load()
                 if res.json()["message"] != "OK":
                     raise ValueError
                 else:
                     return BaseApiStatus(success=True)
     except tenacity.RetryError as e:
         if is_incorrect_return(e):
             logger.exception(f"设备保存(device_save) - 服务器没有正确返回")
@@ -607,17 +608,20 @@
     """
     headers = HEADERS_ADDRESS.copy()
     headers["x-rpc-device_id"] = account.device_id_ios
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
                 async with httpx.AsyncClient() as client:
-                    res = await client.get(URL_ADDRESS.format(
-                        round(NtpTime.time() * 1000)), headers=headers, cookies=account.cookies.dict(),
-                        timeout=conf.preference.timeout)
+                    res = await client.get(
+                        URL_ADDRESS.format(round(NtpTime.time() * 1000)),
+                        headers=headers,
+                        cookies=account.cookies.dict(v2_stoken=True, cookie_type=True),
+                        timeout=conf.preference.timeout
+                    )
                     api_result = ApiResultHandler(res.json())
                     if api_result.login_expired:
                         logger.info(
                             f"获取地址数据 - 用户 {account.bbs_uid} 登录失效")
                         logger.debug(f"网络请求返回: {res.text}")
                         return BaseApiStatus(login_expired=True), None
                 address_list = list(map(Address.parse_obj, api_result.data["list"]))
@@ -693,14 +697,15 @@
     :param retry: 是否允许重试
     :return: (API返回状态, 人机验证任务数据, 设备ID, httpx.AsyncClient连接对象)
     """
     headers = HEADERS_WEBAPI.copy()
     headers["x-rpc-device_id"] = device_id or generate_device_id()
     if use_v4:
         headers.setdefault("x-rpc-source", "accountWebsite")
+
     async def request():
         """
         发送请求的闭包函数
         """
         time_now = round(NtpTime.time() * 1000)
         # await client.options(URL_CREATE_MMT.format(now=time_now, t=time_now),
         #                      headers=headers, timeout=conf.preference.timeout)
@@ -1175,40 +1180,100 @@
             logger.debug(f"网络请求返回: {res.text}")
             return GetCookieStatus(incorrect_return=True), None
         else:
             logger.exception(f"通过 stoken 获取 ltoken: 网络请求失败")
             return GetCookieStatus(network_error=True), None
 
 
+async def get_device_fp(device_id: str, retry: bool = True) -> Tuple[GetFpStatus, Optional[str]]:
+    """
+    获取 x-rpc-device_fp
+
+    :param device_id: x-rpc-device_id 的值
+    :param retry: 是否允许重试
+
+    >>> import asyncio
+    >>> coroutine = get_device_fp(generate_device_id())
+    >>> assert asyncio.new_event_loop().run_until_complete(coroutine)[0].success is True
+    """
+    content = {
+        "seed_id": generate_seed_id(),
+        "device_id": device_id.lower(),
+        "platform": "5",
+        "seed_time": str(int(time.time() * 1000)),
+        "ext_fields": "{\"userAgent\":\"Mozilla\/5.0 (iPhone; CPU iPhone OS 16_2 like Mac OS X) AppleWebKit\/605.1.15 "
+                      f"(KHTML, like Gecko) miHoYoBBS\/{conf.device_config.X_RPC_APP_VERSION}\",\"browserScreenSize"
+                      f"\":243750,\"maxTouchPoints\":5,"
+                      "\"isTouchSupported\":true,\"browserLanguage\":\"zh-CN\",\"browserPlat\":\"iPhone\","
+                      "\"browserTimeZone\":\"Asia\/Shanghai\",\"webGlRender\":\"Apple GPU\",\"webGlVendor\":\"Apple "
+                      "Inc.\",\"numOfPlugins\":0,\"listOfPlugins\":\"unknown\",\"screenRatio\":3,"
+                      "\"deviceMemory\":\"unknown\",\"hardwareConcurrency\":\"4\",\"cpuClass\":\"unknown\","
+                      "\"ifNotTrack\":\"unknown\",\"ifAdBlock\":0,\"hasLiedResolution\":1,\"hasLiedOs\":0,"
+                      "\"hasLiedBrowser\":0}",
+        "app_name": "account_cn",
+        "device_fp": generate_fp_locally()
+    }
+    try:
+        async for attempt in get_async_retry(retry):
+            with attempt:
+                async with httpx.AsyncClient() as client:
+                    res = await client.post(
+                        URL_GET_DEVICE_FP,
+                        json=content,
+                        timeout=conf.preference.timeout
+                    )
+                api_result = ApiResultHandler(res.json())
+                if api_result.data["code"] == 403 or api_result.data["msg"] == "传入的参数有误":
+                    logger.error("传入的参数有误")
+                    return GetFpStatus(invalid_arguments=True), None
+                elif api_result.success:
+                    device_fp = api_result.data["device_fp"]
+                    if not device_fp:
+                        logger.error("获取 x-rpc-device_fp: 服务器返回的 device_fp 为空")
+                        return GetFpStatus(incorrect_return=True), None
+                    return GetFpStatus(success=True), device_fp
+
+    except tenacity.RetryError as e:
+        if is_incorrect_return(e):
+            logger.exception(f"获取 x-rpc-device_fp: 服务器没有正确返回")
+            logger.debug(f"网络请求返回: {res.text}")
+            return GetFpStatus(incorrect_return=True), None
+        else:
+            logger.exception(f"获取 x-rpc-device_fp: 网络请求失败")
+            return GetFpStatus(network_error=True), None
+
+
 async def good_exchange(plan: ExchangePlan) -> Tuple[ExchangeStatus, Optional[ExchangeResult]]:
     """
     执行米游币商品兑换
 
     :param plan: 兑换计划
     """
     headers = HEADERS_EXCHANGE
     headers["x-rpc-device_id"] = plan.account.device_id_ios
+    headers["x-rpc-device_fp"] = plan.account.device_fp or generate_fp_locally()
     content = {
         "app_id": 1,
         "point_sn": "myb",
         "goods_id": plan.good.goods_id,
-        "exchange_num": 1,
+        "exchange_num": 1
     }
     if plan.address is not None:
         content.setdefault("address_id", plan.address.id)
     if plan.game_record is not None:
         content.setdefault("uid", plan.game_record.game_role_id)
         # 例: cn_gf01
         content.setdefault("region", plan.game_record.region)
         # 例: hk4e_cn
         content.setdefault("game_biz", plan.good.game_biz)
     try:
         async with httpx.AsyncClient() as client:
             res = await client.post(
-                URL_EXCHANGE, headers=headers, json=content, cookies=plan.account.cookies.dict(),
+                URL_EXCHANGE, headers=headers, json=content,
+                cookies=plan.account.cookies.dict(cookie_type=True),
                 timeout=conf.preference.timeout)
         api_result = ApiResultHandler(res.json())
         if api_result.login_expired:
             logger.info(
                 f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 登录失效")
             logger.debug(f"网络请求返回: {res.text}")
             return ExchangeStatus(login_expired=True), None
@@ -1238,32 +1303,34 @@
     """
     执行米游币商品兑换
 
     :param plan: 兑换计划
     """
     headers = HEADERS_EXCHANGE
     headers["x-rpc-device_id"] = plan.account.device_id_ios
+    headers["x-rpc-device_fp"] = plan.account.device_fp or generate_fp_locally()
     content = {
         "app_id": 1,
         "point_sn": "myb",
         "goods_id": plan.good.goods_id,
-        "exchange_num": 1,
+        "exchange_num": 1
     }
     if plan.address is not None:
         content.setdefault("address_id", plan.address.id)
     if plan.game_record is not None:
         content.setdefault("uid", plan.game_record.game_role_id)
         # 例: cn_gf01
         content.setdefault("region", plan.game_record.region)
         # 例: hk4e_cn
         content.setdefault("game_biz", plan.good.game_biz)
     try:
         with httpx.Client() as client:
             res = client.post(
-                URL_EXCHANGE, headers=headers, json=content, cookies=plan.account.cookies.dict(),
+                URL_EXCHANGE, headers=headers, json=content,
+                cookies=plan.account.cookies.dict(cookie_type=True),
                 timeout=conf.preference.timeout)
         api_result = ApiResultHandler(res.json())
         if api_result.login_expired:
             logger.info(
                 f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 登录失效")
             logger.debug(f"网络请求返回: {res.text}")
             return ExchangeStatus(login_expired=True), None
```

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/custom_css.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/custom_css.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/custom_widget.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/custom_widget.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/data_model.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,14 +379,22 @@
     """获取用户 GameRecord 失败"""
     init_required = False
     """未进行兑换任务初始化"""
     account_not_found = False
     """账号不存在"""
 
 
+class GetFpStatus(BaseApiStatus):
+    """
+    兑换操作 返回结果
+    """
+    invalid_arguments = False
+    """参数错误"""
+
+
 GeetestResult = NamedTuple("GeetestResult", validate=str, seccode=str)
 """人机验证结果数据"""
 
 
 class GeetestResultV4(BaseModel):
     """
     GEETEST GT4 人机验证结果数据
```

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/exchange_mode.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/exchange_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from textual.events import Event
 from textual.reactive import reactive
 from textual.widgets import Static, ListView, ListItem
 
 from mys_goods_tool.api import URL_EXCHANGE, good_exchange_sync
 from mys_goods_tool.custom_widget import ControllableButton, UnClickableItem
 from mys_goods_tool.data_model import ExchangeStatus
-from mys_goods_tool.user_data import config as conf, ExchangePlan, Preference, ExchangeResult
+from mys_goods_tool.user_data import config as conf, ExchangePlan, Preference, ExchangeResult, different_device_and_salt
 from mys_goods_tool.utils import logger, LOG_FORMAT
 
 
 # TODO: ntp 时间同步
 
 def _get_api_host() -> Optional[str]:
     """
@@ -107,14 +107,19 @@
     普通文本模式（无Textual）
     """
     logger.add(sys.stdout, diagnose=True, format=LOG_FORMAT, level="DEBUG")
     if not conf.exchange_plans:
         logger.info("无兑换计划需要执行")
         return
 
+    if different_device_and_salt:
+        logger.warning("检测到设备信息配置 device_config 或 salt_config 使用了非默认值，"
+                       "如果你修改过这些配置，需要设置 preference.override_device_and_salt 为 True 以覆盖默认值并生效。"
+                       "如果继续，将可能保存默认值到配置文件。")
+
     scheduler = set_scheduler(BlockingScheduler())
     finished: Dict[ExchangePlan, List[bool]] = dict(map(lambda x: (x, []), conf.exchange_plans))
     """每个兑换计划的结果"""
     lock = threading.Lock()
 
     @lambda func: scheduler.add_listener(func, EVENT_JOB_EXECUTED)
     def on_executed(event: JobExecutionEvent):
```

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/exchange_plan_view.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/exchange_plan_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 from textual.widget import Widget
 from textual.widgets import (
     TabbedContent, TabPane, OptionList, ListView
 )
 from textual.widgets._option_list import Option, Separator
 
 from mys_goods_tool.api import get_good_list, get_address, get_game_record, good_exchange, \
-    get_good_detail, get_good_games
+    get_good_detail, get_good_games, get_device_fp
 from mys_goods_tool.custom_css import *
 from mys_goods_tool.custom_widget import StaticStatus, ControllableButton, LoadingDisplay, \
     DynamicTabbedContent, GameButton, PlanButton, UnClickableItem
 from mys_goods_tool.data_model import Good, Address, GameRecord
 from mys_goods_tool.user_data import config as conf, UserAccount, ExchangePlan
+from mys_goods_tool.utils import logger
 
 _T = TypeVar("_T")
 
 
 class BaseExchangePlan(ExchangePlanContent):
     DEFAULT_TEXT: RenderableType
     """默认提示文本内容"""
@@ -910,14 +911,19 @@
                                 account=account,
                                 game_record=record)
             if event.button.id == "button-finish-submit":
                 if plan in conf.exchange_plans:
                     self.app.notice(f"[bold yellow]该兑换计划已存在[/]")
                 else:
                     conf.exchange_plans.add(plan)
+                    if not plan.account.device_fp:
+                        logger.info(f"账号 {plan.account.bbs_uid} 未设置 device_fp，正在获取...")
+                        fp_status, plan.account.device_fp = await get_device_fp(plan.account.device_id_ios)
+                        if fp_status:
+                            logger.info(f"成功获取 device_fp: {plan.account.device_fp}")
                     if conf.save():
                         self.app.notice(f"[bold green]已保存兑换计划[/]")
                     else:
                         self.app.notice(f"[bold red]保存兑换计划失败[/]")
                         # TODO: 保存失败的具体原因提示
                     await ExchangePlanView.manager_content.update_data()
             elif event.button.id == "button-finish-test":
```

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/gt3-localized.html` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/gt3-localized.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/gt3.html` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/gt3.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/index.html` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/index.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/gt.js` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/gt.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/gt4.js` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/gt4.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/jquery.js` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/jquery.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/localized.html` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/localized.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/geetest.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/login_view.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/login_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import asyncio
 import queue
 from typing import NamedTuple, Tuple, Optional, Set
 from urllib.parse import urlencode
 
-import httpx
 from rich.markdown import Markdown
 from textual.app import ComposeResult
 from textual.widgets import (
     Input
 )
 
 from mys_goods_tool.api import create_mobile_captcha, create_mmt, get_login_ticket_by_captcha, \
-    get_multi_token_by_login_ticket, get_cookie_token_by_stoken, get_stoken_v2_by_v1, get_ltoken_by_stoken
+    get_multi_token_by_login_ticket, get_cookie_token_by_stoken, get_stoken_v2_by_v1, get_ltoken_by_stoken, \
+    get_device_fp
 from mys_goods_tool.custom_css import *
 from mys_goods_tool.custom_widget import RadioStatus, StaticStatus, ControllableButton, LoadingDisplay
 from mys_goods_tool.data_model import GeetestResult, MmtData, GetCookieStatus
 from mys_goods_tool.exchange_plan_view import ExchangePlanView
 from mys_goods_tool.geetest import GeetestProcessManager, SetAddressProcessManager
 from mys_goods_tool.user_data import config as conf, UserAccount, CONFIG_PATH
 from mys_goods_tool.utils import logger
@@ -105,16 +105,14 @@
     """
     手机号 表单
     """
     input = Input(placeholder="手机号", id="login_phone")
     """手机号输入框"""
     device_id: Optional[str] = None
     """人机验证过程的设备ID"""
-    client: Optional[httpx.AsyncClient] = None
-    """人机验证过程的连接对象"""
 
     ButtonTuple = NamedTuple("ButtonTuple",
                              send=ControllableButton,
                              stop_geetest=ControllableButton,
                              success=ControllableButton,
                              error=ControllableButton)
 
@@ -184,19 +182,20 @@
                 geetest_result: GeetestResult = self.geetest_manager.result_queue.get_nowait()
             except queue.Empty:
                 continue
             else:
                 logger.info(f"已收到Geetest验证结果数据，将发送验证码至 {self.input.value}")
                 CaptchaLoginInformation.radio_tuple.geetest_finished.turn_on()
                 self.loading.show()
-                create_captcha_status, PhoneForm.client = await create_mobile_captcha(int(self.input.value),
-                                                                                      self.mmt_data,
-                                                                                      geetest_result,
-                                                                                      PhoneForm.client,
-                                                                                      device_id=PhoneForm.device_id)
+                create_captcha_status, _ = await create_mobile_captcha(
+                    int(self.input.value),
+                    self.mmt_data,
+                    geetest_result,
+                    device_id=PhoneForm.device_id
+                )
                 if create_captcha_status:
                     self.loading.hide()
                     logger.info(f"短信验证码已发送至 {self.input.value}")
                     CaptchaLoginInformation.radio_tuple.create_captcha.turn_on()
                     CaptchaLoginInformation.static_tuple.geetest_text.change_text(CaptchaLoginInformation.GEETEST_TEXT,
                                                                                   "center")
                     self.button.success.show()
@@ -245,15 +244,16 @@
         url_params = urlencode(params)
         link = f"http://{address[0]}:{address[1]}/index.html?{url_params}"
         link_localized = f"http://{address[0]}:{address[1]}/localized.html?{url_params}"
         CaptchaLoginInformation.static_tuple.geetest_text.change_text(
             renderable=f"\n- 请前往链接进行验证：\n"
                        f"[@click=app.open_link('{link}')]{link}[/]\n"
                        f"\n- 如果页面加载慢或者出错，尝试：\n"
-                       f"[@click=app.open_link('{link_localized}')]{link_localized}[/]",
+                       f"[@click=app.open_link('{link_localized}')]{link_localized}[/]\n"
+                       f"\n如果你在使用SSH或WSL，无法跳转链接，可前往日志文件复制验证链接",
             text_align="left")
         logger.info(f"请前往链接进行人机验证：{link}")
         logger.info(f"如果页面加载慢或者出错，尝试：{link_localized}")
 
     def set_address_error_callback(self, exception: BaseException):
         """
         可用监听地址获取失败时的回调函数
@@ -276,15 +276,15 @@
             return
         self.before_create_captcha = False
 
         [i.turn_off() for i in CaptchaLoginInformation.radio_tuple]
         self.button.send.disable()
         self.loading.show()
 
-        create_mmt_status, self.mmt_data, PhoneForm.device_id, PhoneForm.client = await create_mmt()
+        create_mmt_status, self.mmt_data, PhoneForm.device_id, _ = await create_mmt()
         if not create_mmt_status:
             self.close_create_captcha_send()
             self.button.error.show()
             self.app.notice("[red]获取Geetest行为验证任务数据失败！[/]")
             return
         else:
             logger.info(f"已成功获取Geetest行为验证任务数据 {self.mmt_data}")
@@ -386,27 +386,29 @@
         phone_number = PhoneForm.input.value
         captcha = int(self.input.value) if self.input.value.isdigit() else self.input.value
 
         # 1. 通过短信验证码获取 login_ticket / 使用已有 login_ticket
         if captcha:
             login_status, cookies = await get_login_ticket_by_captcha(phone_number,
                                                                       captcha,
-                                                                      PhoneForm.client,
                                                                       PhoneForm.device_id)
             if login_status:
                 logger.info(f"用户 {phone_number} 成功获取 login_ticket: {cookies.login_ticket}")
                 account = conf.accounts.get(cookies.bbs_uid)
                 """当前的账户数据对象"""
                 if not account or not account.cookies:
                     conf.accounts.update({
                         cookies.bbs_uid: UserAccount(phone_number=phone_number, cookies=cookies)
                     })
                     account = conf.accounts[cookies.bbs_uid]
                 else:
                     account.cookies.update(cookies)
+                fp_status, account.device_fp = await get_device_fp(account.device_id_ios)
+                if fp_status:
+                    logger.info(f"成功获取 device_fp: {account.device_fp}")
                 conf.save()
                 CaptchaLoginInformation.radio_tuple.login_ticket_by_captcha.turn_on()
         else:
             account_list = list(filter(lambda x: x.phone_number == phone_number, conf.accounts.values()))
             account = account_list[0] if account_list else None
             if not account:
                 self.app.notice(f"手机号为 [bold red]{phone_number}[/] 的账户暂未被绑定！")
```

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/tui.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/tui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import sys
-
 from io import StringIO
+
 from rich.console import RenderableType
 from rich.markdown import Markdown
 from rich.text import Text
 from textual import events
 from textual.app import App, ComposeResult, DEFAULT_COLORS
 from textual.binding import Binding
 from textual.color import Color
@@ -20,23 +20,27 @@
 )
 
 from mys_goods_tool.custom_css import *
 from mys_goods_tool.custom_widget import RadioStatus, StaticStatus
 from mys_goods_tool.exchange_mode import ExchangeModeView, EnterExchangeMode, ExitExchangeMode
 from mys_goods_tool.exchange_plan_view import ExchangePlanView
 from mys_goods_tool.login_view import LoginView
-from mys_goods_tool.user_data import ROOT_PATH, VERSION
+from mys_goods_tool.user_data import ROOT_PATH, VERSION, different_device_and_salt
 from mys_goods_tool.utils import LOG_FORMAT, logger
 
 WELCOME_MD = """
 # Mys_Goods_Tool - 米游社商品兑换工具
 
 ## 更新说明
 
-- 修复短信验证码发送失败的问题 #105 #94 #104 - #126 by @Night-stars-1
+- 兑换请求Headers增加与修改了 `Referer`, `x-rpc-device_fp`, `x-rpc-verify_key`, `Origin` 等字段，可能修复兑换失败的问题
+- 修复登陆时因为连接断开（client has been closed）而导致登陆失败的问题
+- 防止因配置文件中默认存在 `device_config`, `salt_config` 而导致更新后默认配置被原配置覆盖的问题
+- 若需要修改 `device_config` 配置，修改后还设置用户数据文件中 `preference.override_device_and_salt` 为 `true` 以覆盖默认值
+- 修复Unix下即使安装了 uvloop 也找不到，无法应用的问题
 
 ## 功能和特性
 
 - 使用 [Textual](https://github.com/Textualize/textual) 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
 - 短信验证码登录（只需接收一次验证码）
 - 内置人机验证页面，无需前往官网验证
 - 多账号支持
@@ -394,21 +398,26 @@
             TuiApp.text_log.write(text)
 
     def _on_mount(self, _: events.Mount) -> None:
         TuiApp.app = self
         TuiApp.text_log_writer = TuiApp.TextLogWriter()
         logger.add(self.text_log_writer, diagnose=False, level="DEBUG", format=LOG_FORMAT)
         if sys.platform not in ('win32', 'cygwin', 'cli'):
-            if "uvloop" in sys.modules.copy():
+            try:
                 import uvloop
+            except ModuleNotFoundError:
+                logger.info("在非 Windows 环境下，你可以安装 uvloop 以提高性能")
+            else:
                 import asyncio
                 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
-            else:
-                logger.info("在非 Windows 环境下，你可以安装 uvloop 以提高性能")
         self.query_one("Welcome Button", Button).focus()
+        if different_device_and_salt:
+            logger.warning("检测到设备信息配置 device_config 或 salt_config 使用了非默认值，"
+                           "如果你修改过这些配置，需要设置 preference.override_device_and_salt 为 True 以覆盖默认值并生效。"
+                           "如果继续，将可能保存默认值到配置文件。")
 
     def action_screenshot(self, filename: str | None = None, path: str = str(ROOT_PATH)) -> None:
         """Save an SVG "screenshot". This action will save an SVG file containing the current contents of the screen.
 
         Args:
             filename: Filename of screenshot, or None to auto-generate. Defaults to None.
             path: Path to directory. Defaults to "./".
```

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/user_data.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/user_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+import os
 from json import JSONDecodeError
+from pathlib import Path
+from typing import List, Union, Optional, Tuple, Any, Dict, Set, Callable, TYPE_CHECKING, AbstractSet, \
+    Mapping
 
-import os
 from httpx import Cookies
 from loguru import logger
-from pathlib import Path
 from pydantic import BaseModel, Extra, ValidationError, BaseSettings, validator
-from typing import List, Union, Optional, Tuple, Any, Dict, Set, Callable, TYPE_CHECKING, AbstractSet, \
-    Mapping
 
 from mys_goods_tool.data_model import BaseModelWithSetter, Good, Address, GameRecord, BaseModelWithUpdate
 
 ROOT_PATH = Path("./")
 """程序所在目录"""
 
 CONFIG_PATH = ROOT_PATH / "user_data.json"
 """用户数据文件默认路径"""
 
-VERSION = "2.0.5"
+VERSION = "2.1.0-beta.1"
 """程序当前版本"""
 
 if TYPE_CHECKING:
     IntStr = Union[int, str]
     DictStrAny = Dict[str, Any]
     AbstractSetIntStr = AbstractSet[IntStr]
     MappingIntStrAny = Mapping[IntStr, Any]
@@ -219,14 +219,16 @@
     cookies: BBSCookies
     """Cookies"""
 
     device_id_ios: str
     """iOS设备用 deviceID"""
     device_id_android: str
     """安卓设备用 deviceID"""
+    device_fp: Optional[str]
+    """iOS设备用 deviceFp"""
 
     def __init__(self, **data: Any):
         if not data.get("device_id_ios") or not data.get("device_id_android"):
             from mys_goods_tool.utils import generate_device_id
             if not data.get("device_id_ios"):
                 data.setdefault("device_id_ios", generate_device_id())
             if not data.get("device_id_android"):
@@ -312,14 +314,16 @@
     """兑换线程数"""
     exchange_latency: Tuple[float, float] = (0, 0.2)
     """兑换时间延迟随机范围（单位：秒）（防止因为发出请求的时间过于精准而被服务器认定为非人工操作）"""
     enable_log_output: bool = True
     """是否保存日志"""
     log_path: Optional[Path] = ROOT_PATH / "logs" / "mys_goods_tool.log"
     """日志保存路径"""
+    override_device_and_salt: bool = False
+    """是否读取用户数据文件中的 device_config 设备配置 和 salt_config 配置而不是默认配置（一般情况不建议开启）"""
 
     @validator("log_path")
     def _(cls, v: Optional[Path]):
         absolute_path = v.absolute()
         if not os.path.exists(absolute_path) or not os.path.isfile(absolute_path):
             absolute_parent = absolute_path.parent
             try:
@@ -332,15 +336,15 @@
 
     class Config:
         env_prefix = "MYS_GOODS_TOOL_"  # 环境变量前缀
 
 
 class SaltConfig(BaseSettings):
     """
-    生成Headers - DS所用salt值
+    生成Headers - DS所用salt值，非必要请勿修改
     """
     SALT_IOS: str = "ulInCDohgEs557j0VsPDYnQaaz6KJcv5"
     '''生成Headers iOS DS所需的salt'''
     SALT_ANDROID: str = "n0KjuIrKgLHh08LWSCYP0WXlVXaYvV64"
     '''生成Headers Android DS所需的salt'''
     SALT_DATA: str = "t0qEgfub6cvueAPgR5m9aQWWVciEer7v"
     '''Android 设备传入content生成 DS 所需的 salt'''
@@ -352,23 +356,23 @@
         pass
 
 
 # TODO 与用户数据文件中的配置有差异时询问是否使用更新
 class DeviceConfig(BaseSettings):
     """
     设备信息
-    DS算法与设备信息有关联，非必要请勿修改
+    Headers所用的各种数据，非必要请勿修改
     """
-    USER_AGENT_MOBILE: str = "Mozilla/5.0 (iPhone; CPU iPhone OS 15_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) miHoYoBBS/2.42.1"
+    USER_AGENT_MOBILE: str = "Mozilla/5.0 (iPhone; CPU iPhone OS 15_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) miHoYoBBS/2.54.1"
     '''移动端 User-Agent(Mozilla UA)'''
     USER_AGENT_PC: str = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.0 Safari/605.1.15"
     '''桌面端 User-Agent(Mozilla UA)'''
     USER_AGENT_OTHER: str = "Hyperion/275 CFNetwork/1402.0.8 Darwin/22.2.0"
     '''获取用户 ActionTicket 时Headers所用的 User-Agent'''
-    USER_AGENT_ANDROID: str = "Mozilla/5.0 (Linux; Android 11; MI 8 SE Build/RQ3A.211001.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/104.0.5112.97 Mobile Safari/537.36 miHoYoBBS/2.36.1"
+    USER_AGENT_ANDROID: str = "Mozilla/5.0 (Linux; Android 11; MI 8 SE Build/RQ3A.211001.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/104.0.5112.97 Mobile Safari/537.36 miHoYoBBS/2.54.1"
     '''安卓端 User-Agent(Mozilla UA)'''
     USER_AGENT_ANDROID_OTHER: str = "okhttp/4.9.3"
     '''安卓端 User-Agent(专用于米游币任务等)'''
     USER_AGENT_WIDGET: str = "WidgetExtension/231 CFNetwork/1390 Darwin/22.0.0"
     '''iOS 小组件 User-Agent(原神实时便笺)'''
 
     X_RPC_DEVICE_MODEL_MOBILE: str = "iPhone10,2"
@@ -391,15 +395,15 @@
     '''安卓端 x-rpc-sys_version'''
 
     X_RPC_CHANNEL: str = "appstore"
     '''Headers所用的 x-rpc-channel'''
     X_RPC_CHANNEL_ANDROID: str = "miyousheluodi"
     '''安卓端 x-rpc-channel'''
 
-    X_RPC_APP_VERSION: str = "2.52.1"
+    X_RPC_APP_VERSION: str = "2.54.1"
     '''Headers所用的 x-rpc-app_version'''
     X_RPC_PLATFORM: str = "ios"
     '''Headers所用的 x-rpc-platform'''
     UA: str = "\".Not/A)Brand\";v=\"99\", \"Microsoft Edge\";v=\"103\", \"Chromium\";v=\"103\""
     '''Headers所用的 sec-ch-ua'''
     UA_PLATFORM: str = "\"macOS\""
     '''Headers所用的 sec-ch-ua-platform'''
@@ -486,35 +490,51 @@
         logger.exception("数据对象序列化失败，可能是数据类型错误")
         return False
     with open(CONFIG_PATH, "w", encoding="utf-8") as f:
         f.write(str_data)
     return True
 
 
-def load_config():
+def load_config() -> Tuple[UserData, bool]:
     """
     加载用户数据文件
+
+    :return: (<用户数据对象>, <device_config 或 salt_config 是否非默认值且未开启覆写>)
     """
     if os.path.exists(CONFIG_PATH) and os.path.isfile(CONFIG_PATH):
         try:
-            return UserData.parse_file(CONFIG_PATH)
+            user_data = UserData.parse_file(CONFIG_PATH)
         except (ValidationError, JSONDecodeError):
             logger.exception(f"读取用户数据文件失败，请检查用户数据文件 {CONFIG_PATH} 格式是否正确")
             exit(1)
         except:
             logger.exception(f"读取用户数据文件失败，请检查用户数据文件 {CONFIG_PATH} 是否存在且程序有权限读取和写入")
             exit(1)
+        else:
+            if not user_data.preference.override_device_and_salt:
+                default_device_config = DeviceConfig()
+                default_salt_config = SaltConfig()
+                if user_data.device_config != default_device_config or user_data.salt_config != default_salt_config:
+                    user_data.device_config = default_device_config
+                    user_data.salt_config = default_salt_config
+                    return user_data, True
+            else:
+                logger.info("已开启覆写 device_config 和 salt_config，将读取用户数据文件中的配置以覆写默认配置")
+            return user_data, False
     else:
         user_data = UserData()
         try:
             write_config_file(user_data)
         except PermissionError:
             logger.exception(f"创建用户数据文件失败，请检查程序是否有权限读取和写入 {CONFIG_PATH}")
             exit(1)
         # logger.info(f"用户数据文件 {CONFIG_PATH} 不存在，已创建默认用户数据文件。")
         # 由于会输出到标准输出流，影响TUI观感，因此暂时取消
 
-        return user_data
+        return user_data, False
 
 
-config = load_config()
+_load_config_return = load_config()
+config = _load_config_return[0]
 """程序配置对象"""
+different_device_and_salt = _load_config_return[1]
+"""device_config 或 salt_config 是否非默认值且未开启覆写"""
```

### Comparing `mys_goods_tool-2.0.5/mys_goods_tool/utils.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import time
-from multiprocessing import Pool, pool
-
 import hashlib
-import httpx
 import json
-import ntplib
 import os
 import random
 import string
-import tenacity
+import time
 import uuid
-from loguru import logger
-from pydantic import ValidationError
+from multiprocessing import Pool, pool
 from socket import socket, AF_INET, SOCK_STREAM
 from typing import Literal, Union, Dict, List, Any, Callable, Iterable, Optional
 from urllib.parse import urlencode
 
+import httpx
+import ntplib
+import tenacity
+from loguru import logger
+from pydantic import ValidationError
+
 from mys_goods_tool.user_data import config as conf
 
 LOG_FORMAT: str = (
     "<g>{time:MM-DD HH:mm:ss}</g> "
     "[<lvl>{level}</lvl>] "
     "<c><u>{name}</u></c> | "
     "{message}"
@@ -176,14 +176,34 @@
         t = str(int(time.time()))
         r = str(random.randint(100000, 200000))
         c = hashlib.md5(
             f"salt={salt}&t={t}&r={r}&b={data}&q={params}".encode()).hexdigest()
         return f"{t},{r},{c}"
 
 
+def generate_seed_id(length: int = 8) -> str:
+    """
+    生成随机的 seed_id（即长度为8的十六进制数）
+
+    :param length: 16进制数长度
+    """
+    max_num = int("FF" * length, 16)
+    return hex(random.randint(0, max_num))[2:]
+
+
+def generate_fp_locally(length: int = 13):
+    """
+    于本地生成 device_fp
+
+    :param length: device_fp 长度
+    """
+    characters = string.digits + "abcdef"
+    return ''.join(random.choices(characters, k=length))
+
+
 async def get_file(url: str, retry: bool = True):
     """
     下载文件
 
     :param url: 文件URL
     :param retry: 是否允许重试
     :return: 文件数据
```

### Comparing `mys_goods_tool-2.0.5/pyproject.toml` & `mys_goods_tool-2.1.0b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mys-goods-tool"
-version = "2.0.5"
+version = "2.1.0-beta.1"
 description = "米游社商品兑换工具|短信验证登录|终端TUI界面"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.ml>"]
 readme = "README.md"
 homepage = "https://github.com/Ljzd-PRO/Mys_Goods_Tool"
 repository = "https://github.com/Ljzd-PRO/Mys_Goods_Tool"
 documentation = "https://github.com/Ljzd-PRO/Mys_Goods_Tool/wiki"
 keywords = ["mihoyo", "mihoyobbs", "genshin impact", "textual", "tui"]
```

### Comparing `mys_goods_tool-2.0.5/PKG-INFO` & `mys_goods_tool-2.1.0b1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mys-goods-tool
-Version: 2.0.5
+Version: 2.1.0b1
 Summary: 米游社商品兑换工具|短信验证登录|终端TUI界面
 Home-page: https://github.com/Ljzd-PRO/Mys_Goods_Tool
 Keywords: mihoyo,mihoyobbs,genshin impact,textual,tui
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,15 +44,21 @@
   <img alt="代码行数" src="https://img.shields.io/tokei/lines/github/Ljzd-PRO/Mys_Goods_Tool?style=for-the-badge">
   <img alt="构建结果" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/build-v2.yml?event=pull_request&style=for-the-badge">
   <img alt="Python版本兼容性测试" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/python-package.yml?event=pull_request&label=Versions%20Test&style=for-the-badge">
 </div>
 
 ### 更新说明
 
-- 修复短信验证码发送失败的问题 #105 #94 #104 - #126 by @Night-stars-1
+v2.1.0-beta.1
+
+- 兑换请求Headers增加与修改了 `Referer`, `x-rpc-device_fp`, `x-rpc-verify_key`, `Origin` 等字段，可能修复兑换失败的问题
+- 修复登陆时因为连接断开（client has been closed）而导致登陆失败的问题
+- 防止因配置文件中默认存在 `device_config`, `salt_config` 而导致更新后默认配置被原配置覆盖的问题
+- 若需要修改 `device_config` 配置，修改后还设置用户数据文件中 `preference.override_device_and_salt` 为 `true` 以覆盖默认值
+- 修复Unix下即使安装了 uvloop 也找不到，无法应用的问题
 
 ## 功能和特性
 
 - [x] 使用 [Textual](https://github.com/Textualize/textual) 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
 - [x] 短信验证码登录（只需接收一次验证码）
 - [x] 内置人机验证页面，无需前往官网验证
 - [x] 多账号支持
```

