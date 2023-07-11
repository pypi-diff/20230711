# Comparing `tmp/nonebot_plugin_callapi-0.1.3.tar.gz` & `tmp/nonebot_plugin_callapi-0.1.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_callapi-0.1.3.tar", last modified: Fri Jun 23 17:38:12 2023, max compression
+gzip compressed data, was "nonebot_plugin_callapi-0.1.3.post1.tar", last modified: Tue Jul 11 00:41:26 2023, max compression
```

## Comparing `nonebot_plugin_callapi-0.1.3.tar` & `nonebot_plugin_callapi-0.1.3.post1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-06-23 17:38:00.305867 nonebot_plugin_callapi-0.1.3/LICENSE
--rw-r--r--   0        0        0     4723 2023-06-23 17:38:00.305867 nonebot_plugin_callapi-0.1.3/README.md
--rw-r--r--   0        0        0      530 2023-06-23 17:38:00.305867 nonebot_plugin_callapi-0.1.3/nonebot_plugin_callapi/__init__.py
--rw-r--r--   0        0        0     7567 2023-06-23 17:38:00.305867 nonebot_plugin_callapi-0.1.3/nonebot_plugin_callapi/__main__.py
--rw-r--r--   0        0        0      197 2023-06-23 17:38:00.305867 nonebot_plugin_callapi-0.1.3/nonebot_plugin_callapi/config.py
--rw-r--r--   0        0        0      661 2023-06-23 17:38:12.728107 nonebot_plugin_callapi-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 nonebot_plugin_callapi-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-11 00:41:09.797387 nonebot_plugin_callapi-0.1.3.post1/LICENSE
+-rw-r--r--   0        0        0     4723 2023-07-11 00:41:09.797387 nonebot_plugin_callapi-0.1.3.post1/README.md
+-rw-r--r--   0        0        0      530 2023-07-11 00:41:09.797387 nonebot_plugin_callapi-0.1.3.post1/nonebot_plugin_callapi/__init__.py
+-rw-r--r--   0        0        0     7574 2023-07-11 00:41:09.797387 nonebot_plugin_callapi-0.1.3.post1/nonebot_plugin_callapi/__main__.py
+-rw-r--r--   0        0        0      197 2023-07-11 00:41:09.797387 nonebot_plugin_callapi-0.1.3.post1/nonebot_plugin_callapi/config.py
+-rw-r--r--   0        0        0      667 2023-07-11 00:41:26.625510 nonebot_plugin_callapi-0.1.3.post1/pyproject.toml
+-rw-r--r--   0        0        0     5335 1970-01-01 00:00:00.000000 nonebot_plugin_callapi-0.1.3.post1/PKG-INFO
```

### Comparing `nonebot_plugin_callapi-0.1.3/LICENSE` & `nonebot_plugin_callapi-0.1.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_callapi-0.1.3/README.md` & `nonebot_plugin_callapi-0.1.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_callapi-0.1.3/nonebot_plugin_callapi/__init__.py` & `nonebot_plugin_callapi-0.1.3.post1/nonebot_plugin_callapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_callapi-0.1.3/nonebot_plugin_callapi/__main__.py` & `nonebot_plugin_callapi-0.1.3.post1/nonebot_plugin_callapi/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from nonebot_plugin_saa import Image as SAAImage
 from nonebot_plugin_saa import MessageFactory
 from PIL import Image
 from pil_utils import BuildImage, Text2Image
 from pil_utils.fonts import DEFAULT_FALLBACK_FONTS
 from pydantic import BaseModel
 from pygments import highlight
-from pygments.formatters import BBCodeFormatter
+from pygments.formatters.bbcode import BBCodeFormatter
 from pygments.lexers import get_lexer_by_name
 from pygments.style import Style
 
 from .config import config
 
 CODE_FONTS = [
     "JetBrains Mono",
```

### Comparing `nonebot_plugin_callapi-0.1.3/pyproject.toml` & `nonebot_plugin_callapi-0.1.3.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-callapi"
-version = "0.1.3"
+version = "0.1.3.post1"
 description = "Use bot command to call its API"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot_plugin_callapi-0.1.3/PKG-INFO` & `nonebot_plugin_callapi-0.1.3.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-callapi
-Version: 0.1.3
+Version: 0.1.3.post1
 Summary: Use bot command to call its API
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-callapi
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-callapi
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-callapi Version: 0.1.3 Summary: Use
-bot command to call its API Home-page: https://github.com/lgc-NB2Dev/nonebot-
-plugin-callapi Author-Email: student_2333
+Metadata-Version: 2.1 Name: nonebot-plugin-callapi Version: 0.1.3.post1
+Summary: Use bot command to call its API Home-page: https://github.com/lgc-
+NB2Dev/nonebot-plugin-callapi Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-callapi Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-Dist:
 pydantic>=1.10.4 Requires-Dist: Pygments>=2.15.1 Requires-Dist: pil-
 utils>=0.1.7 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.5
 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
```

