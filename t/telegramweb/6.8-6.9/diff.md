# Comparing `tmp/telegramweb-6.8.tar.gz` & `tmp/telegramweb-6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-6.8.tar", last modified: Mon Jul 10 18:21:16 2023, max compression
+gzip compressed data, was "dist/telegramweb-6.9.tar", last modified: Mon Jul 10 18:35:20 2023, max compression
```

## Comparing `telegramweb-6.8.tar` & `telegramweb-6.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:21:16.502354 telegramweb-6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 18:20:55.000000 telegramweb-6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 18:20:55.000000 telegramweb-6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-10 18:21:16.502354 telegramweb-6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-10 18:20:55.000000 telegramweb-6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:21:16.502354 telegramweb-6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 18:20:55.000000 telegramweb-6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:21:16.502354 telegramweb-6.8/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 18:20:55.000000 telegramweb-6.8/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 18:20:55.000000 telegramweb-6.8/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-10 18:20:55.000000 telegramweb-6.8/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-10 18:20:55.000000 telegramweb-6.8/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 18:20:55.000000 telegramweb-6.8/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:21:16.502354 telegramweb-6.8/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 18:20:55.000000 telegramweb-6.8/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44634 2023-07-10 18:20:55.000000 telegramweb-6.8/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-10 18:20:55.000000 telegramweb-6.8/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:21:16.502354 telegramweb-6.8/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-10 18:21:16.000000 telegramweb-6.8/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 18:21:16.000000 telegramweb-6.8/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:21:16.000000 telegramweb-6.8/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 18:21:16.000000 telegramweb-6.8/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 18:21:16.000000 telegramweb-6.8/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:35:20.000000 telegramweb-6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 18:35:00.000000 telegramweb-6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 18:35:00.000000 telegramweb-6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-10 18:35:20.000000 telegramweb-6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-10 18:35:00.000000 telegramweb-6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:35:20.000000 telegramweb-6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 18:35:00.000000 telegramweb-6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:35:20.000000 telegramweb-6.9/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 18:35:00.000000 telegramweb-6.9/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 18:35:00.000000 telegramweb-6.9/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-10 18:35:00.000000 telegramweb-6.9/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-10 18:35:00.000000 telegramweb-6.9/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 18:35:00.000000 telegramweb-6.9/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:35:20.000000 telegramweb-6.9/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 18:35:00.000000 telegramweb-6.9/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44514 2023-07-10 18:35:00.000000 telegramweb-6.9/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-10 18:35:00.000000 telegramweb-6.9/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:35:20.000000 telegramweb-6.9/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-10 18:35:20.000000 telegramweb-6.9/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 18:35:20.000000 telegramweb-6.9/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:35:20.000000 telegramweb-6.9/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 18:35:20.000000 telegramweb-6.9/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 18:35:20.000000 telegramweb-6.9/telegramweb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `telegramweb-6.8/LICENSE` & `telegramweb-6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-6.8/PKG-INFO` & `telegramweb-6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 6.8
+Version: 6.9
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Description: <h1 align="center">
           <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telegramweb Version: 6.8 Summary: Python package
+Metadata-Version: 2.1 Name: telegramweb Version: 6.9 Summary: Python package
 for automatically fetching and pushing news by Telegram. Home-page: https://
 github.com/craziks-creator/telegram-web Author: craziks Author-email:
 chandrashekharpanday07@gmail.com License: MIT Description:
                             ****** [Telegram-news]
                                  Telegram-news
                                      ******
   Python package for automatically fetching and pushing news by Telegram. [!
```

### Comparing `telegramweb-6.8/README.md` & `telegramweb-6.9/README.md`

 * *Files identical despite different names*

### Comparing `telegramweb-6.8/setup.py` & `telegramweb-6.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='6.8',
+    version='6.9',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `telegramweb-6.8/telegram_news/__init__.py` & `telegramweb-6.9/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-6.8/telegram_news/constant.py` & `telegramweb-6.9/telegram_news/constant.py`

 * *Files identical despite different names*

### Comparing `telegramweb-6.8/telegram_news/displaypolicy.py` & `telegramweb-6.9/telegram_news/displaypolicy.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Display policies and id policies for different situation.
 
 Add new ones when possible.
 """
 
 import re
-from telegram import InlineKeyboardButton, InlineKeyboardMarkup
+from pyrogram.types import InlineKeyboardButton, InlineKeyboardMarkup
 import json 
 MAXLEN = 4096
 
 
 def default_policy(item, max_len=1000, max_par_num=40):
     """
     Generate formatted message from item, the default way.
@@ -59,19 +59,20 @@
     if item['link']:
         po += '<a href=\"' + item['link'] + '\">LATEST UPDATE FROM OFFICIAL WEBSITE</a>'
 
     po = po.replace('<br>', "")
 
     if len(po) > MAXLEN:
         return "Too long message!\n" + item['id'], parse_mode, disable_web_page_preview
+    reply_markup = 'InlineKeyboardMarkup([[InlineKeyboardButton(text="TEST_BUTTON", url="www.python.org")]])'
     return {
         'text': po,
         'parse_mode': parse_mode,
-        'disable_web_page_preview': disable_web_page_preview
-        #'reply_markup': reply_markup
+        'disable_web_page_preview': disable_web_page_preview,
+        'reply_markup': reply_markup
     }
 
 
 def best_effort_display_policy(item, max_len=1000, max_par_num=40, suffix='...'):
     """
     Display as more paragraphs as possible.
     If over max_len, end with suffix.
@@ -127,19 +128,20 @@
     if item['link']:
         po += '<a href=\"' + item['link'] + '\">LATEST UPDATE FROM OFFICIAL WEBSITE</a>'
 
     po = po.replace('<br>', "")
 
     if len(po) > 4096:
         return "Too long message!\n" + item['id'], parse_mode, disable_web_page_preview
+    reply_markup = 'InlineKeyboardMarkup([[InlineKeyboardButton(text="TEST_BUTTON", url="www.python.org")]])'
     return {
         'text': po,
         'parse_mode': parse_mode,
-        'disable_web_page_preview': disable_web_page_preview
-        #'reply_markup': reply_markup
+        'disable_web_page_preview': disable_web_page_preview,
+        'reply_markup': reply_markup
     }
 
 
 def default_id_policy(self, link):
     """
     Generate id from link, the default way.
```

### Comparing `telegramweb-6.8/telegram_news/ratelimit.py` & `telegramweb-6.9/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-6.8/telegram_news/template/common.py` & `telegramweb-6.9/telegram_news/template/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -992,15 +992,14 @@
             print(data)
         return data, method
 
     @sleep_and_retry
     @limits(calls=1, period=1)
     def _real_post(self, token, method, data):
         #data['reply_markup'] = InlineKeyboardMarkup([[InlineKeyboardButton(text="CLICK HERE", url="www.google.com")]])
-        data['reply_markup'] = InlineKeyboardMarkup([[InlineKeyboardButton(text="TEST_BUTTON", url="www.ssc.nic.in")]])
         # https://core.telegram.org/bots/api#sendmessage
         res = requests.post('https://api.telegram.org/bot' + token + '/' + method, data, files=data['files'], proxies=self._proxies)
         return res
 
     def _post(self, item, news_id):
 
         res = None
```

### Comparing `telegramweb-6.8/telegram_news/utils.py` & `telegramweb-6.9/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-6.8/telegramweb.egg-info/PKG-INFO` & `telegramweb-6.9/telegramweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 6.8
+Version: 6.9
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Description: <h1 align="center">
           <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telegramweb Version: 6.8 Summary: Python package
+Metadata-Version: 2.1 Name: telegramweb Version: 6.9 Summary: Python package
 for automatically fetching and pushing news by Telegram. Home-page: https://
 github.com/craziks-creator/telegram-web Author: craziks Author-email:
 chandrashekharpanday07@gmail.com License: MIT Description:
                             ****** [Telegram-news]
                                  Telegram-news
                                      ******
   Python package for automatically fetching and pushing news by Telegram. [!
```

