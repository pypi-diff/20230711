# Comparing `tmp/flask_restx_marshmallow-0.1.0.tar.gz` & `tmp/flask_restx_marshmallow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_restx_marshmallow-0.1.0.tar", max compression
+gzip compressed data, was "flask_restx_marshmallow-0.1.1.tar", max compression
```

## Comparing `flask_restx_marshmallow-0.1.0.tar` & `flask_restx_marshmallow-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3740 2023-06-16 10:04:55.731643 flask_restx_marshmallow-0.1.0/README.md
--rw-r--r--   0        0        0      726 2023-06-16 08:32:17.549159 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/__init__.py
--rw-r--r--   0        0        0     5946 2023-06-16 08:32:07.051658 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/api.py
--rw-r--r--   0        0        0     9701 2023-06-16 09:43:59.552465 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/namespace.py
--rw-r--r--   0        0        0     2881 2023-06-16 08:32:11.254992 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/parameter.py
--rw-r--r--   0        0        0     8281 2023-06-16 08:32:08.405825 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/schema.py
--rw-r--r--   0        0        0     5375 2023-06-16 08:32:11.254992 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/sqlalchemy.py
--rw-r--r--   0        0        0  1024792 2023-04-26 15:13:34.000000 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/static/swagger-ui-bundle.min.js
--rw-r--r--   0        0        0   316731 2023-04-26 15:13:34.000000 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/static/swagger-ui-standalone-preset.min.js
--rw-r--r--   0        0        0   144893 2023-04-26 15:13:34.000000 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/static/swagger-ui.min.css
--rw-r--r--   0        0        0     1643 2023-06-02 04:56:56.372088 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/static/swagger_fav.png
--rw-r--r--   0        0        0     5861 2023-06-16 08:32:11.254992 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/swagger.py
--rw-r--r--   0        0        0     1708 2023-06-16 08:32:02.111658 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/templates/index.html
--rw-r--r--   0        0        0     1702 2023-06-16 08:32:02.111658 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/templates/local.html
--rw-r--r--   0        0        0    19064 2023-06-16 08:32:08.113325 flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/util.py
--rw-r--r--   0        0        0     1632 2023-06-16 08:33:00.113328 flask_restx_marshmallow-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5231 2023-06-16 10:16:44.976690 flask_restx_marshmallow-0.1.0/setup.py
--rw-r--r--   0        0        0     5453 2023-06-16 10:16:44.977446 flask_restx_marshmallow-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3740 2023-07-11 05:18:52.422889 flask_restx_marshmallow-0.1.1/README.md
+-rw-r--r--   0        0        0      726 2023-07-11 05:19:54.162889 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/__init__.py
+-rw-r--r--   0        0        0     5946 2023-07-11 05:19:54.132889 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/api.py
+-rw-r--r--   0        0        0    10079 2023-07-11 05:19:54.132889 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/namespace.py
+-rw-r--r--   0        0        0     2881 2023-07-11 05:19:54.162889 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/parameter.py
+-rw-r--r--   0        0        0     8281 2023-07-11 05:19:54.132889 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/schema.py
+-rw-r--r--   0        0        0     5375 2023-07-11 05:19:54.162889 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/sqlalchemy.py
+-rw-r--r--   0        0        0  1024792 2023-07-11 04:36:04.602890 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/static/swagger-ui-bundle.min.js
+-rw-r--r--   0        0        0   316731 2023-07-11 04:36:04.602890 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/static/swagger-ui-standalone-preset.min.js
+-rw-r--r--   0        0        0   144893 2023-07-11 04:36:04.602890 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/static/swagger-ui.min.css
+-rw-r--r--   0        0        0     1643 2023-07-11 04:36:04.602890 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/static/swagger_fav.png
+-rw-r--r--   0        0        0     5861 2023-07-11 05:19:54.132889 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/swagger.py
+-rw-r--r--   0        0        0     1708 2023-07-11 05:18:52.502889 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/templates/index.html
+-rw-r--r--   0        0        0     1702 2023-07-11 05:18:52.502889 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/templates/local.html
+-rw-r--r--   0        0        0    18986 2023-07-11 05:32:58.802890 flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/util.py
+-rw-r--r--   0        0        0    22803 2023-07-11 05:24:40.362889 flask_restx_marshmallow-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5440 2023-07-11 05:36:26.285622 flask_restx_marshmallow-0.1.1/setup.py
+-rw-r--r--   0        0        0     5757 2023-07-11 05:36:26.287047 flask_restx_marshmallow-0.1.1/PKG-INFO
```

### Comparing `flask_restx_marshmallow-0.1.0/README.md` & `flask_restx_marshmallow-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!--
  * @Description: README for flask_restx_marshmallow
- * @version: 0.1.0
+ * @version: 0.1.1
  * @Author: 1746104160
  * @Date: 2023-06-02 13:05:58
  * @LastEditors: 1746104160 shaojiahong2001@outlook.com
  * @LastEditTime: 2023-06-16 18:04:55
  * @FilePath: /flask_restx_marshmallow/README.md
 -->
 # Flask-RESTX-marshmallow
@@ -49,15 +49,15 @@
     StandardSchema,
 )
 
 app = Flask(__name__)
 app.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:///test.db"
 api = Api(
     app,
-    version="0.1.0",
+    version="0.1.1",
     title="example API",
     description="api interface for example app",
 )
 db = SQLAlchemy(app)
 ns = api.namespace("example", description="example operations")
```

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/__init__.py` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Description: flask-restx-marshmallow
-version: 0.1.0
+version: 0.1.1
 Author: 1746104160
 Date: 2023-06-02 12:56:56
 LastEditors: 1746104160 shaojiahong2001@outlook.com
 LastEditTime: 2023-06-16 16:32:05
 FilePath: /flask_restx_marshmallow/flask-restx-marshmallow/__init__.py
 """
 from flask_restx import Resource
```

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/api.py` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Description: patched api of flask_restx_marshmallow
-version: 0.1.0
+version: 0.1.1
 Author: 1746104160
 Date: 2023-06-02 12:56:56
 LastEditors: 1746104160 shaojiahong2001@outlook.com
 LastEditTime: 2023-06-04 21:38:24
 FilePath: /flask_restx_marshmallow/flask_restx_marshmallow/api.py
 """
 import importlib
```

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/namespace.py` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Description: patched namespace of flask_restx_marshmallow
-version: 0.1.0
+version: 0.1.1
 Author: 1746104160
 Date: 2023-06-02 12:56:56
 LastEditors: 1746104160 shaojiahong2001@outlook.com
 LastEditTime: 2023-06-04 21:38:50
 FilePath: /flask_restx_marshmallow/flask_restx_marshmallow/namespace.py
 """
 from functools import wraps
@@ -128,15 +128,22 @@
                                         request.get_json(
                                             force=True, silent=True
                                         )
                                     )
                                 except TypeError:
                                     pass
                             case "formData":
-                                new_data.update(request.form.to_dict())
+                                new_data.update(
+                                    {
+                                        key: value
+                                        if len(value) > 1
+                                        else value[0]
+                                        for key, value in request.form.lists()
+                                    }
+                                )
                                 new_data.update(
                                     {
                                         key: value
                                         if len(value) > 1
                                         else value[0]
                                         for key, value in request.files.lists()
                                     }
@@ -172,15 +179,17 @@
                 "formData": "form",
                 "body": "json",
                 "cookie": "cookies",
             }
             return self.doc(params=params)(
                 self.response(code=HTTPStatus.UNPROCESSABLE_ENTITY)(
                     parser.use_args(
-                        params, location=location2webargs_location[location], as_kwargs=as_kwargs
+                        params,
+                        location=location2webargs_location[location],
+                        as_kwargs=as_kwargs,
                     )(func)
                 )
             )
 
         return decorator
 
     @override
```

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/parameter.py` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Description: parameters of flask_restx_marshmallow
-version: 0.1.0
+version: 0.1.1
 Author: 1746104160
 Date: 2023-06-02 12:56:56
 LastEditors: 1746104160 shaojiahong2001@outlook.com
 LastEditTime: 2023-06-16 14:15:27
 FilePath: /flask_restx_marshmallow/flask_restx_marshmallow/parameter.py
 """
 import importlib
```

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/schema.py` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Description: schemas of flask_restx_marshmallow
-version: 0.1.0
+version: 0.1.1
 Author: 1746104160
 Date: 2023-06-02 12:56:56
 LastEditors: 1746104160 shaojiahong2001@outlook.com
 LastEditTime: 2023-06-16 14:16:11
 FilePath: /flask_restx_marshmallow/flask_restx_marshmallow/schema.py
 """
 import importlib
```

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/sqlalchemy.py` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/sqlalchemy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Description: patched salalchemy of flask_restx_marshmallow
-version: 0.1.0
+version: 0.1.1
 Author: 1746104160
 Date: 2023-06-02 12:56:56
 LastEditors: 1746104160 shaojiahong2001@outlook.com
 LastEditTime: 2023-06-16 14:16:40
 FilePath: /flask_restx_marshmallow/flask_restx_marshmallow/sqlalchemy.py
 """
 from typing import Optional
```

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/static/swagger-ui-bundle.min.js` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/static/swagger-ui-bundle.min.js`

 * *Files identical despite different names*

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/static/swagger-ui-standalone-preset.min.js` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/static/swagger-ui-standalone-preset.min.js`

 * *Files identical despite different names*

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/static/swagger-ui.min.css` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/static/swagger-ui.min.css`

 * *Files identical despite different names*

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/static/swagger_fav.png` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/static/swagger_fav.png`

 * *Files identical despite different names*

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/swagger.py` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/swagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Description: patched swagger of flask_restx_marshmallow
-version: 0.1.0
+version: 0.1.1
 Author: 1746104160
 Date: 2023-06-02 12:56:56
 LastEditors: 1746104160 shaojiahong2001@outlook.com
 LastEditTime: 2023-06-04 21:45:14
 FilePath: /flask_restx_marshmallow/flask_restx_marshmallow/swagger.py
 """
 from apispec.ext.marshmallow.common import get_fields
```

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/templates/index.html` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!--
  * @Description: html template for swagger ui when the server can access the internet
- * @version: 0.1.0
+ * @version: 0.1.1
  * @Author: 1746104160
  * @Date: 2023-06-02 12:56:56
  * @LastEditors: 1746104160 shaojiahong2001@outlook.com
  * @LastEditTime: 2023-06-16 14:14:14
  * @FilePath: /flask_restx_marshmallow/flask_restx_marshmallow/templates/index.html
 -->
 <!DOCTYPE html>
```

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/templates/local.html` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/templates/local.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!--
  * @Description: html template for swagger ui when the server is not able to access the internet
- * @version: 0.1.0
+ * @version: 0.1.1
  * @Author: 1746104160
  * @Date: 2023-06-02 12:56:56
  * @LastEditors: 1746104160 shaojiahong2001@outlook.com
  * @LastEditTime: 2023-06-16 14:14:22
  * @FilePath: /flask_restx_marshmallow/flask_restx_marshmallow/templates/local.html
 -->
 <!DOCTYPE html>
```

### Comparing `flask_restx_marshmallow-0.1.0/flask_restx_marshmallow/util.py` & `flask_restx_marshmallow-0.1.1/flask_restx_marshmallow/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Description: utils of flask_restx_marshmallow
-version: 0.1.0
+version: 0.1.1
 Author: 1746104160
 Date: 2023-06-02 12:56:56
 LastEditors: 1746104160 shaojiahong2001@outlook.com
 LastEditTime: 2023-06-02 13:25:40
 FilePath: /flask_restx_marshmallow/flask_restx_marshmallow/util.py
 """
 import importlib
@@ -71,17 +71,21 @@
 try:
     json: ModuleType = importlib.import_module("orjson")
 except ModuleNotFoundError:
     json = importlib.import_module("json")
 
 
 class File(Field):
-    """
-    Author: 1746104160
-    msg: check file upload type
+    """parameter validation for file
+
+    Args:
+        mimetypes (Iterable[str], optional): accept mimetype or iterable mimetypes
+        like `image/png|image|image/*`. Defaults to None.
+        size (Union[int, float], optional): maximum size to upload. Defaults to None.
+        size_unit (str, optional): size unit like m|mb|M|MB|. Defaults to "MB".
     """
 
     default_error_messages: dict[str, str] = {
         "invalid": "Not a valid file.",
         "invalid_mimetype": "{mimetype} is not a valid mimetype.",
         "invalid_size": "File size is too large for {text}.",
     }
@@ -107,22 +111,14 @@
         self,
         *,
         mimetypes: Optional[str | Iterable[str]] = None,
         size: Optional[int | float] = None,
         size_unit: str = "MB",
         **kwargs,
     ) -> None:
-        """initialize file type
-
-        Args:
-            mimetypes (Iterable[str], optional): accept mimetype or iterable mimetypes
-            like `image/png|image|image/*`. Defaults to None.
-            size (Union[int, float], optional): maximum size to upload. Defaults to None.
-            size_unit (str, optional): size unit like m|mb|M|MB|. Defaults to "MB".
-        """
         super().__init__(**kwargs)
         if mimetypes is not None:
             if isinstance(mimetypes, str):
                 self.mimetypes = {mimetypes}
                 mimetype_begin: str = mimetypes.split("/")[0].lower()
                 assert mimetype_begin in self.mimes
                 self.mimetypes: set[str] = {mimetypes}
@@ -162,25 +158,25 @@
             raise self.make_error("invalid file")
         byte_value: bytes = value.stream.read()
         file_mime = (
             res.mime
             if (res := filetype.guess(byte_value)) is not None
             else value.mimetype
         )
-        if getattr(self, "mimetypes") is not None and not any(
+        if getattr(self, "mimetypes", None) is not None and not any(
             re.match(
                 re.compile(mimetype, re.IGNORECASE),
                 file_mime,
             )
             for mimetype in self.mimetypes
         ):
             raise self.make_error("invalid_mimetype", mimetype=value.mimetype)
 
         if (
-            getattr(self, "size") is not None
+            getattr(self, "size", None) is not None
             and len(value.stream.read()) > self.size
         ):
             raise self.make_error("invalid_size", text=self.size_text)
         value.stream = BytesIO(byte_value)
         return value
 
 
@@ -550,15 +546,15 @@
         title=api.title,
         specs_url=api.specs_url,
     )
 
 
 spec: APISpec = APISpec(
     title="flask_restx_marshmallow",
-    version="0.1.0",
+    version="0.1.1",
     openapi_version="3.0.2",
     plugins=[MarshmallowPlugin(schema_name_resolver=resolver)],
     info={"description": "flask_restx_marshmallow backend api"},
 )
 converter: MarshmallowPlugin.Converter = spec.plugins[0].converter
 apidoc: Apidoc = Apidoc(
     "swagger_doc",
```

### Comparing `flask_restx_marshmallow-0.1.0/setup.py` & `flask_restx_marshmallow-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,33 +16,39 @@
  'SQLAlchemy>=2.0.15,<3.0.0',
  'apispec>=6.3.0,<7.0.0',
  'beautifulsoup4>=4.12.2,<5.0.0',
  'filetype>=1.2.0,<2.0.0',
  'flask-restx>=1.1.0,<2.0.0',
  'marshmallow-sqlalchemy>=0.29.0,<0.30.0',
  'marshmallow>=3.19.0,<4.0.0',
- 'mysqlclient>=2.1.1,<3.0.0',
  'orjson>=3.9.0,<4.0.0',
  'passlib>=1.7.4,<2.0.0',
  'redis>=4.5.5,<5.0.0',
  'requests>=2.31.0,<3.0.0',
  'sortedcontainers>=2.4.0,<3.0.0',
+ 'toml>=0.10.2,<0.11.0',
  'webargs>=8.2.0,<9.0.0']
 
+extras_require = \
+{'databases': ['psycopg2-binary>=2.9.6,<3.0.0', 'pymysql>=1.0.3,<2.0.0'],
+ 'mysql': ['pymysql>=1.0.3,<2.0.0'],
+ 'pgsql': ['psycopg2-binary>=2.9.6,<3.0.0']}
+
 setup_kwargs = {
     'name': 'flask-restx-marshmallow',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A successful practice combining flask_restx with marshmallow',
-    'long_description': '<!--\n * @Description: README for flask_restx_marshmallow\n * @version: 0.1.0\n * @Author: 1746104160\n * @Date: 2023-06-02 13:05:58\n * @LastEditors: 1746104160 shaojiahong2001@outlook.com\n * @LastEditTime: 2023-06-16 18:04:55\n * @FilePath: /flask_restx_marshmallow/README.md\n-->\n# Flask-RESTX-marshmallow\n\nFlask-RESTX-marshmallow is an extension for [Flask](https://flask.palletsprojects.com/en/latest/) and [Flask-RESTX](https://flask-restx.readthedocs.io/en/latest/), which is a successful practice combining flask_restx with marshmallow.\n\n## Compatibility\n\nFlask-RESTX-marshmallow requires Python 3.10+.\n\n## Installation\n\nInstall the extension with pip:\n\n```bash\npip install flask-restx-marshmallow\n```\n\nor with poetry:\n\n```bash\npoetry add flask-restx-marshmallow\n```\n\n## Quickstart\n\nWith Flask-RESTX-marshmallow, you only import the api instance to route and document your endpoints.\n\n```python\nimport uuid\n\nimport sqlalchemy as sa\nfrom flask import Flask\nfrom marshmallow import fields, post_load\n\nfrom flask_restx_marshmallow import (\n    Api,\n    JSONParameters,\n    QueryParameters,\n    Resource,\n    SQLAlchemy,\n    StandardSchema,\n)\n\napp = Flask(__name__)\napp.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:///test.db"\napi = Api(\n    app,\n    version="0.1.0",\n    title="example API",\n    description="api interface for example app",\n)\ndb = SQLAlchemy(app)\nns = api.namespace("example", description="example operations")\n\n\nclass Task(db.Model):\n    id = db.Column(db.String(32), primary_key=True)\n    task = db.Column(db.String(80))\n\n    def __init__(self, id, task):\n        self.id = id.hex\n        self.task = task\n\n    def __repr__(self):\n        return "<Task %r>" % self.task\n\n\nclass QueryTaskParameters(QueryParameters):\n    id = fields.UUID(metadata={"description": "The task unique identifier"})\n\n    @post_load\n    def process(self, data, **_kwargs):\n        if "id" in data:\n            return {"data": Task.query.filter_by(id=data["id"].hex).first()}\n        return {"code": 1, "message": "id is required", "success": False}\n\n\nclass CreateTaskParameters(JSONParameters):\n    task = fields.String(\n        required=True, metadata={"description": "The task details"}\n    )\n\n    @post_load\n    def process(self, data, **_kwargs):\n        try:\n            task = Task(id=uuid.uuid4(), task=data["task"])\n            db.session.add(task)\n        except sa.exc.IntegrityError as e:\n            db.session.rollback()\n            return {"code": 1, "message": str(e), "success": False}\n        else:\n            db.session.commit()\n            return {\n                "message": f"create task success with id {uuid.UUID(task.id)}"\n            }\n\n\nclass TaskSchema(StandardSchema):\n    data = fields.Nested(\n        {\n            "id": fields.UUID(\n                metadata={"description": "The task unique identifier"},\n            ),\n            "task": fields.String(metadata={"description": "The task details"}),\n        }\n    )\n\n\n@ns.route("/")\nclass TaskManage(Resource):\n    """task manage"""\n\n    @ns.parameters(params=QueryTaskParameters(), location="query")\n    @ns.response(\n        code=200,\n        description="query task by id",\n        model=TaskSchema(message="query task success"),\n    )\n    def get(self, task):\n        """query task by id"""\n        return task\n\n    @ns.parameters(params=CreateTaskParameters(), location="body")\n    @ns.response(\n        code=200,\n        description="create a new task",\n        model=None,\n        name="CreateSchema",\n        message="create successfully",\n    )\n    def post(self, res):\n        """create a new task"""\n        return res\n\n\nif __name__ == "__main__":\n    with app.app_context():\n        db.create_all()\n    api.register_doc(app)\n    app.run(debug=True)\n```\n',
+    'long_description': '<!--\n * @Description: README for flask_restx_marshmallow\n * @version: 0.1.1\n * @Author: 1746104160\n * @Date: 2023-06-02 13:05:58\n * @LastEditors: 1746104160 shaojiahong2001@outlook.com\n * @LastEditTime: 2023-06-16 18:04:55\n * @FilePath: /flask_restx_marshmallow/README.md\n-->\n# Flask-RESTX-marshmallow\n\nFlask-RESTX-marshmallow is an extension for [Flask](https://flask.palletsprojects.com/en/latest/) and [Flask-RESTX](https://flask-restx.readthedocs.io/en/latest/), which is a successful practice combining flask_restx with marshmallow.\n\n## Compatibility\n\nFlask-RESTX-marshmallow requires Python 3.10+.\n\n## Installation\n\nInstall the extension with pip:\n\n```bash\npip install flask-restx-marshmallow\n```\n\nor with poetry:\n\n```bash\npoetry add flask-restx-marshmallow\n```\n\n## Quickstart\n\nWith Flask-RESTX-marshmallow, you only import the api instance to route and document your endpoints.\n\n```python\nimport uuid\n\nimport sqlalchemy as sa\nfrom flask import Flask\nfrom marshmallow import fields, post_load\n\nfrom flask_restx_marshmallow import (\n    Api,\n    JSONParameters,\n    QueryParameters,\n    Resource,\n    SQLAlchemy,\n    StandardSchema,\n)\n\napp = Flask(__name__)\napp.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:///test.db"\napi = Api(\n    app,\n    version="0.1.1",\n    title="example API",\n    description="api interface for example app",\n)\ndb = SQLAlchemy(app)\nns = api.namespace("example", description="example operations")\n\n\nclass Task(db.Model):\n    id = db.Column(db.String(32), primary_key=True)\n    task = db.Column(db.String(80))\n\n    def __init__(self, id, task):\n        self.id = id.hex\n        self.task = task\n\n    def __repr__(self):\n        return "<Task %r>" % self.task\n\n\nclass QueryTaskParameters(QueryParameters):\n    id = fields.UUID(metadata={"description": "The task unique identifier"})\n\n    @post_load\n    def process(self, data, **_kwargs):\n        if "id" in data:\n            return {"data": Task.query.filter_by(id=data["id"].hex).first()}\n        return {"code": 1, "message": "id is required", "success": False}\n\n\nclass CreateTaskParameters(JSONParameters):\n    task = fields.String(\n        required=True, metadata={"description": "The task details"}\n    )\n\n    @post_load\n    def process(self, data, **_kwargs):\n        try:\n            task = Task(id=uuid.uuid4(), task=data["task"])\n            db.session.add(task)\n        except sa.exc.IntegrityError as e:\n            db.session.rollback()\n            return {"code": 1, "message": str(e), "success": False}\n        else:\n            db.session.commit()\n            return {\n                "message": f"create task success with id {uuid.UUID(task.id)}"\n            }\n\n\nclass TaskSchema(StandardSchema):\n    data = fields.Nested(\n        {\n            "id": fields.UUID(\n                metadata={"description": "The task unique identifier"},\n            ),\n            "task": fields.String(metadata={"description": "The task details"}),\n        }\n    )\n\n\n@ns.route("/")\nclass TaskManage(Resource):\n    """task manage"""\n\n    @ns.parameters(params=QueryTaskParameters(), location="query")\n    @ns.response(\n        code=200,\n        description="query task by id",\n        model=TaskSchema(message="query task success"),\n    )\n    def get(self, task):\n        """query task by id"""\n        return task\n\n    @ns.parameters(params=CreateTaskParameters(), location="body")\n    @ns.response(\n        code=200,\n        description="create a new task",\n        model=None,\n        name="CreateSchema",\n        message="create successfully",\n    )\n    def post(self, res):\n        """create a new task"""\n        return res\n\n\nif __name__ == "__main__":\n    with app.app_context():\n        db.create_all()\n    api.register_doc(app)\n    app.run(debug=True)\n```\n',
     'author': '1746104160',
     'author_email': 'shaojiahong2001@outlook.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/1746104160/flask-restx-marshmallow',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `flask_restx_marshmallow-0.1.0/PKG-INFO` & `flask_restx_marshmallow-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-restx-marshmallow
-Version: 0.1.0
+Version: 0.1.1
 Summary: A successful practice combining flask_restx with marshmallow
 Home-page: https://github.com/1746104160/flask-restx-marshmallow
 License: MIT
 Keywords: flask,flask_restx,sqlalchemy,marshmallow
 Author: 1746104160
 Author-email: shaojiahong2001@outlook.com
 Requires-Python: >=3.10,<4.0
@@ -12,14 +12,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: databases
+Provides-Extra: mysql
+Provides-Extra: pandas
+Provides-Extra: pgsql
 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: Flask-Caching (>=2.0.2,<3.0.0)
 Requires-Dist: Flask-JWT-Extended (>=4.5.2,<5.0.0)
 Requires-Dist: Flask-SQLAlchemy (>=3.0.3,<4.0.0)
 Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0)
 Requires-Dist: SQLAlchemy-Utils (>=0.41.1,<0.42.0)
 Requires-Dist: apispec (>=6.3.0,<7.0.0)
@@ -27,24 +31,27 @@
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: flask-restx (>=1.1.0,<2.0.0)
 Requires-Dist: marshmallow (>=3.19.0,<4.0.0)
 Requires-Dist: marshmallow-sqlalchemy (>=0.29.0,<0.30.0)
 Requires-Dist: mysqlclient (>=2.1.1,<3.0.0)
 Requires-Dist: orjson (>=3.9.0,<4.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0); extra == "pgsql" or extra == "databases"
+Requires-Dist: pymysql (>=1.0.3,<2.0.0); extra == "mysql" or extra == "databases"
 Requires-Dist: redis (>=4.5.5,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: webargs (>=8.2.0,<9.0.0)
 Project-URL: Repository, https://github.com/1746104160/flask-restx-marshmallow
 Description-Content-Type: text/markdown
 
 <!--
  * @Description: README for flask_restx_marshmallow
- * @version: 0.1.0
+ * @version: 0.1.1
  * @Author: 1746104160
  * @Date: 2023-06-02 13:05:58
  * @LastEditors: 1746104160 shaojiahong2001@outlook.com
  * @LastEditTime: 2023-06-16 18:04:55
  * @FilePath: /flask_restx_marshmallow/README.md
 -->
 # Flask-RESTX-marshmallow
@@ -89,15 +96,15 @@
     StandardSchema,
 )
 
 app = Flask(__name__)
 app.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:///test.db"
 api = Api(
     app,
-    version="0.1.0",
+    version="0.1.1",
     title="example API",
     description="api interface for example app",
 )
 db = SQLAlchemy(app)
 ns = api.namespace("example", description="example operations")
```

