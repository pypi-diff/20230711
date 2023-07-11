# Comparing `tmp/flask-siwadoc-0.2.1.tar.gz` & `tmp/flask-siwadoc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-siwadoc-0.2.1.tar", last modified: Fri Mar 17 15:54:49 2023, max compression
+gzip compressed data, was "flask-siwadoc-0.2.2.tar", last modified: Tue Jul 11 14:08:31 2023, max compression
```

## Comparing `flask-siwadoc-0.2.1.tar` & `flask-siwadoc-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 15:54:49.197990 flask-siwadoc-0.2.1/
--rw-rw-rw-   0        0        0     1087 2022-06-04 15:34:19.000000 flask-siwadoc-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    11063 2023-03-17 15:54:49.196992 flask-siwadoc-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    10336 2023-03-12 12:56:33.000000 flask-siwadoc-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-17 15:54:49.171426 flask-siwadoc-0.2.1/flask_siwadoc/
--rw-rw-rw-   0        0        0     8621 2023-03-17 15:30:19.000000 flask-siwadoc-0.2.1/flask_siwadoc/__init__.py
--rw-rw-rw-   0        0        0      271 2022-07-20 14:27:37.000000 flask-siwadoc-0.2.1/flask_siwadoc/error.py
--rw-rw-rw-   0        0        0      655 2022-07-20 15:01:39.000000 flask-siwadoc-0.2.1/flask_siwadoc/models.py
--rw-rw-rw-   0        0        0     5666 2023-03-12 12:56:33.000000 flask-siwadoc-0.2.1/flask_siwadoc/openapi.py
--rw-rw-rw-   0        0        0     4625 2022-06-04 17:56:06.000000 flask-siwadoc-0.2.1/flask_siwadoc/schema.py
-drwxrwxrwx   0        0        0        0 2023-03-17 15:54:49.194995 flask-siwadoc-0.2.1/flask_siwadoc/templates/
--rw-rw-rw-   0        0        0      351 2022-06-05 03:47:17.000000 flask-siwadoc-0.2.1/flask_siwadoc/templates/rapidoc.html
--rw-rw-rw-   0        0        0      654 2022-06-04 14:12:15.000000 flask-siwadoc-0.2.1/flask_siwadoc/templates/redoc.html
--rw-rw-rw-   0        0        0     1638 2023-03-17 15:53:42.000000 flask-siwadoc-0.2.1/flask_siwadoc/templates/swagger.html
--rw-rw-rw-   0        0        0     6271 2022-08-08 15:43:32.000000 flask-siwadoc-0.2.1/flask_siwadoc/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-17 15:54:49.189378 flask-siwadoc-0.2.1/flask_siwadoc.egg-info/
--rw-rw-rw-   0        0        0    11063 2023-03-17 15:54:47.000000 flask-siwadoc-0.2.1/flask_siwadoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-03-17 15:54:48.000000 flask-siwadoc-0.2.1/flask_siwadoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 15:54:47.000000 flask-siwadoc-0.2.1/flask_siwadoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-03-17 15:54:48.000000 flask-siwadoc-0.2.1/flask_siwadoc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-17 15:54:48.000000 flask-siwadoc-0.2.1/flask_siwadoc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 15:54:49.197990 flask-siwadoc-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2108 2022-07-31 15:25:47.000000 flask-siwadoc-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:08:31.820537 flask-siwadoc-0.2.2/
+-rw-rw-rw-   0        0        0     1087 2022-06-04 15:34:19.000000 flask-siwadoc-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    11479 2023-07-11 14:08:31.820537 flask-siwadoc-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10752 2023-07-11 14:05:57.000000 flask-siwadoc-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 14:08:31.431275 flask-siwadoc-0.2.2/flask_siwadoc/
+-rw-rw-rw-   0        0        0    10077 2023-07-11 14:08:02.000000 flask-siwadoc-0.2.2/flask_siwadoc/__init__.py
+-rw-rw-rw-   0        0        0      271 2022-07-20 14:27:37.000000 flask-siwadoc-0.2.2/flask_siwadoc/error.py
+-rw-rw-rw-   0        0        0      655 2022-07-20 15:01:39.000000 flask-siwadoc-0.2.2/flask_siwadoc/models.py
+-rw-rw-rw-   0        0        0     5666 2023-03-12 12:56:33.000000 flask-siwadoc-0.2.2/flask_siwadoc/openapi.py
+-rw-rw-rw-   0        0        0     4625 2022-06-04 17:56:06.000000 flask-siwadoc-0.2.2/flask_siwadoc/schema.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:08:31.818547 flask-siwadoc-0.2.2/flask_siwadoc/templates/
+-rw-rw-rw-   0        0        0      351 2022-06-05 03:47:17.000000 flask-siwadoc-0.2.2/flask_siwadoc/templates/rapidoc.html
+-rw-rw-rw-   0        0        0      654 2022-06-04 14:12:15.000000 flask-siwadoc-0.2.2/flask_siwadoc/templates/redoc.html
+-rw-rw-rw-   0        0        0     1638 2023-03-17 15:53:42.000000 flask-siwadoc-0.2.2/flask_siwadoc/templates/swagger.html
+-rw-rw-rw-   0        0        0     6271 2022-08-08 15:43:32.000000 flask-siwadoc-0.2.2/flask_siwadoc/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:08:31.546132 flask-siwadoc-0.2.2/flask_siwadoc.egg-info/
+-rw-rw-rw-   0        0        0    11479 2023-07-11 14:08:27.000000 flask-siwadoc-0.2.2/flask_siwadoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-07-11 14:08:30.000000 flask-siwadoc-0.2.2/flask_siwadoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:08:27.000000 flask-siwadoc-0.2.2/flask_siwadoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-11 14:08:28.000000 flask-siwadoc-0.2.2/flask_siwadoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-11 14:08:29.000000 flask-siwadoc-0.2.2/flask_siwadoc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 14:08:31.821536 flask-siwadoc-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2108 2022-07-31 15:25:47.000000 flask-siwadoc-0.2.2/setup.py
```

### Comparing `flask-siwadoc-0.2.1/LICENSE` & `flask-siwadoc-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-siwadoc-0.2.1/PKG-INFO` & `flask-siwadoc-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-siwadoc
-Version: 0.2.1
+Version: 0.2.2
 Summary: flask openapi(swagger) doc generator
 Home-page: https://github.com/lzjun567/flask-siwadoc
 Author: liuzhijun
 Author-email: lzjun567@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
@@ -38,14 +38,22 @@
 
 ### 4、ui切换
 
 flask-siwadoc内置了`swagger`（默认）、`redoc`、`rapidoc`等多种UI界面
 
 ### 5、支持标签与分组
 
+### 6、可设置访问权限
+
+配置参数：
+* SIWA_USER：登录用户名
+* SIWA_PASSWORD: 登录密码
+
+只有同时设置了用户名和密码访问文档才需要登录权限，该场景用在正式环境中，防止接口文档被匿名访问
+
 ## 安装
 
 ```
 pip install flask-siwadoc
 ```
 
 ## 快速开始
@@ -346,8 +354,10 @@
 reference
 
 1. https://pydantic-docs.helpmanual.io/
 2. https://github.com/tiangolo/fastapi
 3. https://github.com/bauerji/flask-pydantic
 4. https://github.com/kemingy/flaskerk
 
-任何问题欢迎发issue或者加我微信 lzjun567 交流，欢迎PR
+任何问题欢迎发issue或者加我微信 lzjun567 交流，欢迎PR， 如果对你有帮助或者给你的工作带来了极大的便利，可考虑赞赏作者
+
+![赞赏](./screnshots/6802366f4419fd9db9fb3c730f873d2.jpg)
```

### Comparing `flask-siwadoc-0.2.1/README.md` & `flask-siwadoc-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 
 ### 4、ui切换
 
 flask-siwadoc内置了`swagger`（默认）、`redoc`、`rapidoc`等多种UI界面
 
 ### 5、支持标签与分组
 
+### 6、可设置访问权限
+
+配置参数：
+* SIWA_USER：登录用户名
+* SIWA_PASSWORD: 登录密码
+
+只有同时设置了用户名和密码访问文档才需要登录权限，该场景用在正式环境中，防止接口文档被匿名访问
+
 ## 安装
 
 ```
 pip install flask-siwadoc
 ```
 
 ## 快速开始
@@ -326,8 +334,10 @@
 reference
 
 1. https://pydantic-docs.helpmanual.io/
 2. https://github.com/tiangolo/fastapi
 3. https://github.com/bauerji/flask-pydantic
 4. https://github.com/kemingy/flaskerk
 
-任何问题欢迎发issue或者加我微信 lzjun567 交流，欢迎PR
+任何问题欢迎发issue或者加我微信 lzjun567 交流，欢迎PR， 如果对你有帮助或者给你的工作带来了极大的便利，可考虑赞赏作者
+
+![赞赏](./screnshots/6802366f4419fd9db9fb3c730f873d2.jpg)
```

### Comparing `flask-siwadoc-0.2.1/flask_siwadoc/__init__.py` & `flask-siwadoc-0.2.2/flask_siwadoc/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,28 +3,39 @@
 from typing import Optional, Type, Dict
 
 import pydantic
 from flask import Blueprint, request, Flask, render_template
 from flask import jsonify
 from pydantic import BaseModel
 from pydantic.typing import Literal
-
+from werkzeug.security import generate_password_hash, check_password_hash
+from flask_httpauth import HTTPBasicAuth
 from . import utils, openapi, error
 from .error import ValidationError
 from pydantic import ValidationError as PydanticError
 from pydantic.errors import MissingError, ListMaxLengthError
 from pydantic.error_wrappers import ErrorWrapper
 import uuid
 
 __all__ = ["SiwaDoc", "ValidationError"]
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 SUPPORTED_UI = ('redoc', 'swagger', 'rapidoc')
 
+auth = HTTPBasicAuth()
+users = dict()
+
+
+@auth.verify_password
+def verify_password(username, password):
+    if username in users and \
+            check_password_hash(users.get(username), password):
+        return username
+
 
 class SiwaDoc:
     def __init__(self,
                  app: Flask = None,
                  title: str = "SiwaDocAPI",
                  description: str = "",
                  version="latest",
@@ -56,14 +67,34 @@
         siwa_bp = Blueprint("siwadoc",
                             __name__,
                             template_folder=template_folder,
                             )
 
         @siwa_bp.route(self.doc_url)
         def doc_html():
+            siwa_user = self.app.config.get("SIWA_USER")
+            siwa_pass = self.app.config.get("SIWA_PASSWORD")
+            if siwa_user and siwa_pass:
+                global users
+                users = {
+                    siwa_user: generate_password_hash(siwa_pass),
+                }
+                login_info = auth.get_auth()
+                password = auth.get_auth_password(login_info)
+                status = None
+                user = auth.authenticate(login_info, password)
+                if user in (False, None):
+                    status = 401
+                elif not auth.authorize(None, user, auth):
+                    status = 403
+                if status:
+                    try:
+                        return auth.auth_error_callback(status)
+                    except TypeError:
+                        return auth.auth_error_callback()
             ui = request.args.get("ui") or self.ui
             assert ui in SUPPORTED_UI, f"ui only support with {SUPPORTED_UI}"
             ui_file = f'{ui}.html'
             return render_template(ui_file, spec_url=self.openapi_url)
 
         @siwa_bp.route(f'{self.openapi_url}')
         def doc_json():
@@ -140,18 +171,22 @@
                         request_files = request.files
                         files_data = {}
                         for file_field, file_conf in files.items():
                             is_required_ = file_conf.get('required', False)
                             is_single_file_ = file_conf.get('single', True)
                             file_list = request_files.getlist(file_field)
                             if is_required_ and not file_list:
-                                raise ValidationError(PydanticError(errors=[ErrorWrapper(exc=MissingError(), loc=(file_field,))], model=form_model))
+                                raise ValidationError(
+                                    PydanticError(errors=[ErrorWrapper(exc=MissingError(), loc=(file_field,))],
+                                                  model=form_model))
 
                             if file_list and is_single_file_ and len(file_list) > 1:
-                                raise ValidationError(PydanticError(errors=[ErrorWrapper(exc=ListMaxLengthError(limit_value=1), loc=(file_field,))], model=form_model))
+                                raise ValidationError(PydanticError(
+                                    errors=[ErrorWrapper(exc=ListMaxLengthError(limit_value=1), loc=(file_field,))],
+                                    model=form_model))
 
                             if file_list:
                                 files_data[file_field] = file_list[0] if is_single_file_ else file_list
 
                 if query_in_kwargs:
                     kwargs["query"] = query_data
                 if body_in_kwargs:
@@ -174,15 +209,16 @@
                         # 将files中定义的字段填充到form的schema中
                         assert isinstance(files, dict)
                         for field, conf in files.items():
                             is_single_file = conf.get('single', True)
                             if is_single_file:
                                 file_schema = {'title': field, 'type': 'string', 'format': 'binary'}
                             else:
-                                file_schema = {'title': field, 'type': 'array', 'items': {'type': 'string', 'format': 'binary'}}
+                                file_schema = {'title': field, 'type': 'array',
+                                               'items': {'type': 'string', 'format': 'binary'}}
                             schema['properties'][field] = file_schema
 
                             is_required = conf.get('required', False)
                             if is_required:
                                 required_fields = schema.get('required', [])
                                 required_fields.append(field)
                                 schema['required'] = required_fields
```

### Comparing `flask-siwadoc-0.2.1/flask_siwadoc/models.py` & `flask-siwadoc-0.2.2/flask_siwadoc/models.py`

 * *Files identical despite different names*

### Comparing `flask-siwadoc-0.2.1/flask_siwadoc/openapi.py` & `flask-siwadoc-0.2.2/flask_siwadoc/openapi.py`

 * *Files identical despite different names*

### Comparing `flask-siwadoc-0.2.1/flask_siwadoc/schema.py` & `flask-siwadoc-0.2.2/flask_siwadoc/schema.py`

 * *Files identical despite different names*

### Comparing `flask-siwadoc-0.2.1/flask_siwadoc/templates/redoc.html` & `flask-siwadoc-0.2.2/flask_siwadoc/templates/redoc.html`

 * *Files identical despite different names*

### Comparing `flask-siwadoc-0.2.1/flask_siwadoc/templates/swagger.html` & `flask-siwadoc-0.2.2/flask_siwadoc/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `flask-siwadoc-0.2.1/flask_siwadoc/utils.py` & `flask-siwadoc-0.2.2/flask_siwadoc/utils.py`

 * *Files identical despite different names*

### Comparing `flask-siwadoc-0.2.1/flask_siwadoc.egg-info/PKG-INFO` & `flask-siwadoc-0.2.2/flask_siwadoc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-siwadoc
-Version: 0.2.1
+Version: 0.2.2
 Summary: flask openapi(swagger) doc generator
 Home-page: https://github.com/lzjun567/flask-siwadoc
 Author: liuzhijun
 Author-email: lzjun567@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
@@ -38,14 +38,22 @@
 
 ### 4、ui切换
 
 flask-siwadoc内置了`swagger`（默认）、`redoc`、`rapidoc`等多种UI界面
 
 ### 5、支持标签与分组
 
+### 6、可设置访问权限
+
+配置参数：
+* SIWA_USER：登录用户名
+* SIWA_PASSWORD: 登录密码
+
+只有同时设置了用户名和密码访问文档才需要登录权限，该场景用在正式环境中，防止接口文档被匿名访问
+
 ## 安装
 
 ```
 pip install flask-siwadoc
 ```
 
 ## 快速开始
@@ -346,8 +354,10 @@
 reference
 
 1. https://pydantic-docs.helpmanual.io/
 2. https://github.com/tiangolo/fastapi
 3. https://github.com/bauerji/flask-pydantic
 4. https://github.com/kemingy/flaskerk
 
-任何问题欢迎发issue或者加我微信 lzjun567 交流，欢迎PR
+任何问题欢迎发issue或者加我微信 lzjun567 交流，欢迎PR， 如果对你有帮助或者给你的工作带来了极大的便利，可考虑赞赏作者
+
+![赞赏](./screnshots/6802366f4419fd9db9fb3c730f873d2.jpg)
```

### Comparing `flask-siwadoc-0.2.1/setup.py` & `flask-siwadoc-0.2.2/setup.py`

 * *Files identical despite different names*

