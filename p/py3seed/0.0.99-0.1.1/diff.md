# Comparing `tmp/py3seed-0.0.99.tar.gz` & `tmp/py3seed-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.0.99.tar", last modified: Wed May 11 04:06:54 2022, max compression
+gzip compressed data, was "py3seed-0.1.1.tar", last modified: Tue Jul 11 02:54:02 2023, max compression
```

## Comparing `py3seed-0.0.99.tar` & `py3seed-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 04:06:54.551836 py3seed-0.0.99/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.0.99/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      860 2022-05-11 04:06:54.551971 py3seed-0.0.99/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.0.99/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.0.99/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      932 2022-05-11 04:06:54.552575 py3seed-0.0.99/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      257 2021-12-04 07:21:56.000000 py3seed-0.0.99/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 04:06:54.536575 py3seed-0.0.99/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 04:06:54.547448 py3seed-0.0.99/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      609 2022-05-06 09:20:10.000000 py3seed-0.0.99/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1646 2022-05-06 09:20:10.000000 py3seed-0.0.99/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.0.99/src/py3seed/admin.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 04:06:54.551156 py3seed-0.0.99/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.0.99/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    12399 2022-05-11 03:45:53.000000 py3seed-0.0.99/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      665 2021-09-15 09:23:34.000000 py3seed-0.0.99/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.0.99/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    39377 2022-05-10 01:49:39.000000 py3seed-0.0.99/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    23006 2022-01-14 03:15:02.000000 py3seed-0.0.99/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6008 2022-05-06 14:11:36.000000 py3seed-0.0.99/src/py3seed/utils.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2022-05-11 04:06:54.550168 py3seed-0.0.99/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      860 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      503 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       66 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2022-05-11 04:06:54.000000 py3seed-0.0.99/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.523413 py3seed-0.1.1/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.1/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-11 02:54:02.523547 py3seed-0.1.1/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.1/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.1/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-11 02:54:02.524201 py3seed-0.1.1/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.1/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.499305 py3seed-0.1.1/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.514749 py3seed-0.1.1/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.1/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.1/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.1/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.1/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.518930 py3seed-0.1.1/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.1/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    20310 2023-07-11 02:45:05.000000 py3seed-0.1.1/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.1/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.1/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.1/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.1/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57499 2023-07-10 03:52:03.000000 py3seed-0.1.1/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.1/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14529 2023-07-11 02:00:45.000000 py3seed-0.1.1/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.1/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.517989 py3seed-0.1.1/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.522873 py3seed-0.1.1/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.1/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6093 2023-07-11 01:48:21.000000 py3seed-0.1.1/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.1/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.1/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.1/tests/test_mongosupport.py
```

### Comparing `py3seed-0.0.99/LICENSE` & `py3seed-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.99/PKG-INFO` & `py3seed-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.0.99
+Version: 0.1.1
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.0.99/setup.cfg` & `py3seed-0.1.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.0.99
+version = 0.1.1
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls = 
@@ -18,17 +18,15 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	importlib_metadata >= 4.4
 	pymongo >= 3.8
-	flask >= 1.1
-	inflection
-	pyyaml
+	Flask >= 2.1
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 pyseed.registered_commands = 
 	gen = py3seed.commands.gen:main
```

### Comparing `py3seed-0.0.99/src/py3seed/__main__.py` & `py3seed-0.1.1/src/py3seed/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 
 def list_dependencies_and_versions() -> List[Tuple[str, str]]:
     deps = (
         "flask",
         "pymongo",
         "importlib_metadata",
-        "inflection",
     )
     return [(dep, version(dep)) for dep in deps]
 
 
 def dep_versions() -> str:
     return ", ".join(
         "{}: {}".format(*dependency) for dependency in list_dependencies_and_versions()
```

### Comparing `py3seed-0.0.99/src/py3seed/admin.py` & `py3seed-0.1.1/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.99/src/py3seed/error.py` & `py3seed-0.1.1/src/py3seed/error.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,7 +39,12 @@
     """ Database error. """
     pass
 
 
 class TemplateError(SeedError):
     """ Template error. """
     pass
+
+
+class LayoutError(SeedError):
+    """ Layout error. """
+    pass
```

### Comparing `py3seed-0.0.99/src/py3seed/log.py` & `py3seed-0.1.1/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.0.99/src/py3seed/model.py` & `py3seed-0.1.1/src/py3seed/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,25 @@
     ~~~~~~~~~~~~~~
 
     Model related.
 
     :copyright: (c) 2021 by weiminfeng.
     :date: 2021/6/5
 """
-import functools
 import json
 import sys
 from abc import ABCMeta
 from copy import deepcopy
 from datetime import datetime
-from typing import no_type_check, Dict, Type, Callable, get_origin, get_args, Set, Any, ForwardRef, List
+from typing import no_type_check, Dict, Type, Callable, get_origin, get_args, Set, Any, ForwardRef, List, Tuple
 
 from bson import ObjectId
 
 from .error import SchemaError, DataError, PathError
-from .utils import parse_layout
+
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Custom Types
 #
 
 class SimpleEnumMeta(type):
     """ Metaclass for SimpleEnum. """
@@ -135,22 +134,25 @@
     IP = 'ip'
     OBJECTID = 'objectid'  # Default format for ObjectId
     CHECKBOX = 'checkbox'  # Default format for bool
     SWITCH = 'switch'
     HIDDEN = 'hidden'  # Hidden input
     LINK = 'link'  # Text input with an extenral link
     TIME = 'time'  # Time picker
+    METRIC = 'metric'  # Statistic card for simple or object
+    RANGE = 'range'  # Range picker
     # Below values are used for inner model/dict or list of model/dict
     TAB = 'tab'  # Objects with tabs nav, i.e, [{}]
     TABLE = 'table'  # Objects in table, i.e, [{}]
     MODAL = 'modal'  # Objects with some fields in table and all fields in modal, i.e, [{}]
     GRID = 'grid'  # Objects in grid, i.e, [{}]
-    TIMELINE = 'timeline'  # Objects in timeline
+    TIMELINE = 'timeline'  # Objects in timeline, i.e, [{}]
+    CALENDAR = 'calendar'  # Objects in calendar, i.e, [{}]
+    MEDIA = 'media'  # Objects in media components like blog comments, tweets and the like, i.e, [{}]
     CHART = 'chart'  # Charting with series, i.e, {title, names, values}
-    STATISTIC = 'statistic'  # Statistic card, i.e, {title, value, chart, children, extras}
     CASCADER = 'cascader'  # Cascade selection, i.e, List[str]
     LATLNG = 'latlng'  # LatLng chooser, i.e, List[float]
 
 
 class Comparator(SimpleEnum):
     """ Predefined compartors, which should be used to control search conditions.
 
@@ -164,14 +166,25 @@
     LT = 'lt'  # <
     LTE = 'lte'  # <=
     IN = 'in'
     NIN = 'nin'
     LIKE = 'like'  # Need to convert this to regex
 
 
+class Ownership(SimpleEnum):
+    """ Dependencies between two model, mainly used in many to one relation.
+
+    e.g,
+    task.project -> project.tasks, one project owns many tasks, means we can create task directly in a project detail page.
+    task.user -> user.tasks, one user has many tasks, but not owns them, means tasks should be created in other way and then you can assign them to different user.
+    """
+    HAVE = 'have'
+    OWN = 'own'
+
+
 # ----------------------------------------------------------------------------------------------------------------------
 # Constants
 #
 
 # Date format
 DATETIME_FORMAT = '%Y-%m-%d %H:%M:%S.%f'
 DATETIME_FORMAT_SHORT = '%Y-%m-%d %H:%M:%S'
@@ -210,14 +223,16 @@
 
     def default(self, o):
         """ Returns a serializable object for o. """
         if isinstance(o, ObjectId):
             return str(o)
         elif isinstance(o, datetime):
             return o.strftime(DATETIME_FORMAT)
+        elif isinstance(o, BaseModel):
+            return o.dict()
 
         return json.JSONEncoder.default(self, o)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Validator
 #
@@ -232,41 +247,42 @@
             skip_on_failure: bool = False,
     ):
         self.func = func
         self.skip_on_failure = skip_on_failure
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-# Model field
+# Field
 #
 
 class ModelField:
-    """ Field definition for model. """
+    """ Field definition. """
     __slots__ = (
         'name',
         'type',
         'default',
         'required',
-        'readonly',
+        'editable',
         'searchable',
         'sortable',
         'format',
         'icon',
         'title',
         'description',
         'unit',
-        'alias',
+        'source_field_name',
+        'depends'
     )
 
     def __init__(self,
                  name: str = None, type_: Type = None,
-                 default: Any = Undefined, required: bool = Undefined,
-                 readonly: bool = Undefined, searchable: Comparator = Undefined, sortable: bool = Undefined,
+                 default: Any = Undefined, required: bool = Undefined, editable: bool = Undefined,
+                 searchable: Comparator = Undefined, sortable: bool = Undefined,
                  format_: Format = None, icon: str = None, title: str = None, description: str = None, unit: str = None,
-                 alias: str = None) -> None:
+                 source_field_name: str = None, depends: Any = None):
         """ Init method.
 
         :param type_: annotaion for field, e.g, str or Dict[str, str] or List[Object]
         """
         self.name = name
         self.type = type_
         # default is none if undefined
@@ -275,19 +291,19 @@
         else:
             self.default = default
         # required is true if undefined
         if required is Undefined:
             self.required = True
         else:
             self.required = required
-        # readonly is false if undefined
-        if readonly is Undefined:
-            self.readonly = False
+        # editable is true if undefined
+        if editable is Undefined:
+            self.editable = True
         else:
-            self.readonly = readonly
+            self.editable = editable
         # searchable is none if undefined
         if searchable is Undefined:
             self.searchable = None
         else:
             self.searchable = searchable
         # sortable is false if undefined
         if sortable is Undefined:
@@ -296,57 +312,76 @@
             self.sortable = sortable
         #
         self.format = format_
         self.icon = icon
         self.title = title
         self.description = description
         self.unit = unit
-        self.alias = alias
+        #
+        self.source_field_name = source_field_name
+        # depends is mainly used to return dynamic data for page rendering and biz logic
+        # e.g,
+        # A tag field defiend in User model, tag: str = ModelField(format_=Format.SELECT, depends=lamdab self: self.team.tags)
+        # In page rendering, you can use user.tag_depends to draw select options
+        self.depends = depends
 
     def __str__(self):
         return f'{self.name}/{self.type}/{self.default}/{self.required}/{self.format}'
 
 
-# ----------------------------------------------------------------------------------------------------------------------
-# Relation
-#
-
-class relation(object):
-    """ Decorator on a method to tell that it is used to fetch related models.
+class RelationField(ModelField):
+    """ Relation field definition. """
 
-    class Post(BaseModel):
-        creator_id: ObjectId
-        tag_ids: List[ObjectId]
-
-        @relation
-        def creator(self):
-            return User.find_one(self.creator_id)
-
-        @relation
-        def tags(self):
-            return list(Tag.find({'_id':{'$in':self.tag_ids}})
-
-    p = Post()
-    p.creator
-    p.tags
-
-    Reference:
-    https://docs.python.org/3/howto/descriptor.html#properties
-    https://realpython.com/primer-on-python-decorators/#classes-as-decorators
-    https://docs.python.org/3/reference/datamodel.html#object.__get__
-    """
+    __slots__ = ModelField.__slots__ + (
+        'save_field_name',
+        'save_field_order',
+        'back_field_name',
+        'back_field_is_list',
+        'back_field_order',
+        'back_field_format',
+        'back_field_icon',
+        'back_field_title',
+        'back_field_description',
+        'back_field_unit',
+        'ownership',
+        'is_back_field',
+    )
 
-    def __init__(self, func):
-        functools.update_wrapper(self, func)
-        self.func = func
+    def __init__(self,
+                 name: str = None, type_: Type = None,
+                 save_field_name: str = Undefined, save_field_order: List[Tuple[str, int]] = [],
+                 back_field_name: str = None, back_field_is_list: bool = False, back_field_order: List[Tuple[str, int]] = [],
+                 back_field_format: Format = None, back_field_icon: str = None, back_field_title: str = None,
+                 back_field_description: str = None, back_field_unit: str = None,
+                 ownership: Ownership = None, is_back_field: bool = False,
+                 **kwargs):
+        """ Init method.
 
-    def __get__(self, obj, objtype=None):
-        if obj is None:
-            return self
-        return self.func(obj)
+        :param save_field_name: The name to use for saving current relation, if it is none, will use xxx_id/xxx_ids by default. The back field in related model have same value, used for searching the original model
+        :param save_field_order: If the field is List, use this order when loading and saving
+        :param back_field_name: The name to use for the relation from the related model back to this one, if it is none, do not create back field in related model
+        :param back_field_is_list: If back field is list
+        :param back_field_order: If back field is list, use this order when loading and saving
+        :param is_back_field: If is a back field defined in related object
+        """
+        super().__init__(name, type_, **kwargs)
+        # x12
+        self.save_field_name = save_field_name
+        self.save_field_order = save_field_order
+        self.back_field_name = back_field_name
+        self.back_field_is_list = back_field_is_list
+        self.back_field_order = back_field_order
+        self.back_field_format = back_field_format
+        self.back_field_icon = back_field_icon
+        self.back_field_title = back_field_title
+        self.back_field_description = back_field_description
+        self.back_field_unit = back_field_unit
+        #
+        self.ownership = ownership
+        self.is_back_field = is_back_field
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Meta class
 #
 
 def evaluate_forward_ref(type_, globalns_):
@@ -358,26 +393,39 @@
 
 
 class ModelMeta(ABCMeta):
     """ Metaclass for model. """
 
     @no_type_check
     def __new__(mcs, name, bases, namespace, **kwargs):
-        """ Create and return a new object. """
+        """ Create and return a new object.
+
+        :param bases: Only contains current class' direct parents
+        :param namespace: Only contains the fields of current object
+        """
         fields: Dict[str, ModelField] = {}
-        relations: Dict[str, relation] = {}
+        relations: Dict[str, RelationField] = {}
         properties: Dict[str, property] = {}
         # TODO: Support callable validators
         slots: Set[str] = namespace.get('__slots__', ())
         slots = {slots} if isinstance(slots, str) else set(slots)
+        # Using for self-referencing, so we that we can remove all ForwardRef just after the class is created
+        # If use ForwardRef('other_class_name'), we do not have appropriate timing to replace it to its real class
+        # as we do not know if it is created or not
         has_forward_refs = False
         #
         for base in reversed(bases):
-            if issubclass(base, BaseModel) and base is not BaseModel:
-                fields.update(deepcopy(base.__fields__))
+            if issubclass(base, BaseModel):  # True if base is BaseModel or its subclass
+                # BaseModel do not have __fields__
+                if base is not BaseModel:
+                    fields.update(deepcopy(base.__fields__))
+                # Id field's type should be defined in MongoModel/CacheModel, so we need to fetch them from bases
+                if '__id_type__' not in namespace:
+                    namespace['__id_type__'] = base.__id_type__
+                    namespace['__id_name__'] = base.__id_name__
 
         def _validate_annotation(field_name, field_type):
             """ Validate field definition.
 
             Do not need to validate recrusively as referencing models has done their own validation.
             """
             nonlocal has_forward_refs
@@ -419,112 +467,156 @@
                     raise SchemaError(f'{field_name}: {check_type} has not defined any enum values')
                 if len(enum_types) > 1:
                     raise SchemaError(f'{field_name}: {check_type} can not have more than one type')
             elif issubclass(check_type, BaseModel):
                 pass
             elif check_type not in AUTHORIZED_TYPES:
                 raise SchemaError(f'{field_name}: {check_type} is not an authorized type')
+            #
+            return check_type, origin
 
         # Validation
         skips = set()
         if namespace.get('__qualname__') != 'BaseModel':
             #
-            # Annotations(Fields), similar to typing.get_type_hints
+            # Iterate each annotation(field)
+            # Similar to typing.get_type_hints, https://docs.python.org/3/library/typing.html
+            # But we can not use get_type_hints() here as it tries to create class from ForwardRef
             #
             annotations = namespace.get('__annotations__', {})
             for ann_name, ann_type in annotations.items():
                 # Skip
                 if ann_name.startswith('__'):
                     skips.add(ann_name)
                     continue
                 # Validate
-                _validate_annotation(ann_name, ann_type)
-                # Create model field
-                field = ModelField(name=ann_name, type_=ann_type)
+                f_type, f_origin = _validate_annotation(ann_name, ann_type)
+                # Create another field for RelationField
+                save_field = None
+                #
                 value = namespace.get(ann_name, Undefined)
                 # Field is required if undefined
                 if value is Undefined:
-                    field.default = None
-                    field.required = True
+                    field = ModelField(name=ann_name, type_=ann_type, default=None, required=True)
                 # Field is NOT required
                 elif value is None:
-                    field.default = None
-                    field.required = False
-                # Define a ModelField directly
+                    field = ModelField(name=ann_name, type_=ann_type, default=None, required=False)
+                # Define a RelationField
+                elif isinstance(value, RelationField):
+                    field = value
+                    field.name = ann_name
+                    field.type = ann_type
+                    # When save_field is underfined in this object, it will go to its default setting logic
+                    if field.save_field_name is Undefined:
+                        if f_origin is list:
+                            field.save_field_name = ann_name + '_ids'
+                        else:
+                            field.save_field_name = ann_name + '_id'
+                    # Create the save field
+                    id_type = f_type.__id_type__  # related model's is a basemodel
+                    if id_type is None:
+                        raise SchemaError(f'{field.save_field_name}: id type can not be blank')
+                    #
+                    save_field = ModelField(
+                        name=field.save_field_name,
+                        type_=List[id_type] if f_origin is list else id_type,
+                        required=field.required,
+                        editable=False,  # save field value will be updated by its source field, so no need to render in form
+                        source_field_name=ann_name,  # Mark the source field
+                    )
+                    # back_field_name should always has a meaningful value, if it is none, do not create back field in related object
+                    # e.g,
+                    # project.activities.user -> user, no need to create back_field in user model as it is hard to search all the activities for user
+                    # in such case, we need to create activity model, activity.project -> project.activities, activity.user -> user.activities
+                    if field.back_field_name is None:
+                        pass
+                    #
+                    relations[ann_name] = value
+                # Define a ModelField
                 elif isinstance(value, ModelField):
-                    # x11
-                    field.default = value.default
-                    field.required = value.required
-                    field.readonly = value.readonly
-                    field.searchable = value.searchable
-                    field.sortable = value.sortable
-                    field.format = value.format
-                    field.icon = value.icon
-                    field.title = value.title
-                    field.description = value.description
-                    field.unit = value.unit
-                    field.alias = value.alias
+                    # Supplement field's name and type, as we use annotation to define a model field
+                    # e.g, name: str = Field(title='User Name'), so need to mannaully set name/str here
+                    field = value
+                    field.name = ann_name
+                    field.type = ann_type
                 # Set default value
                 else:
-                    field.default = value
-                    field.required = True
+                    field = ModelField(name=ann_name, type_=ann_type, default=value, required=True)
                 # check default value type
                 if field.default is not None:
                     if isinstance(ann_type, SimpleEnumMeta):
                         if not ann_type.validate(field.default):
                             raise SchemaError(f'{ann_name}: {ann_type} default value is invalid')
                     else:
                         # Skip if default is callable, e.g, datetime.now
                         if callable(field.default):
                             pass
                         elif isinstance(field.default, list):
                             pass
                         elif not isinstance(field.default, ann_type):
                             raise SchemaError(f'{ann_name}: {ann_type} default value is invalid')
+                # check depends
+                if field.depends is not None:
+                    if callable(field.depends):
+                        pass
+                    elif not isinstance(field.depends, list):
+                        raise SchemaError(f'{ann_name}: {ann_type} depdends value should be list')
                 #
                 fields[ann_name] = field
+                if save_field is not None:
+                    fields[save_field.name] = save_field
             #
-            # Relations & Properties
+            # Properties
             #
             for attr in namespace:
-                if isinstance(namespace.get(attr), relation):
-                    relations[attr] = namespace.get(attr)
                 if isinstance(namespace.get(attr), property):
                     properties[attr] = namespace.get(attr)
         #
         # Check depth
         #
         max_list_depth = 0
 
         def _iter(field_name, field_type, level):
             """ Check all the fields recrusively. """
             nonlocal max_list_depth
             max_list_depth = max(max_list_depth, level)
-            origin = get_origin(field_type)
+            #
+            origin_ = get_origin(field_type)
             is_in_list = False
-            if origin is dict:
+            if origin_ is dict:
                 _, check_type = get_args(field_type)
-            elif origin is list:
+            elif origin_ is list:
                 check_type = get_args(field_type)[0]
                 is_in_list = True
             else:
                 check_type = field_type
             #
             if isinstance(check_type, ForwardRef):  # Skip forwardref, always using for self-referencing
                 pass
             elif isinstance(check_type, SimpleEnumMeta):
                 pass
             elif issubclass(check_type, BaseModel):
-                # We do not use typing.get_type_hints() here
-                # As the method converts str to ForwardRef, but we are now using ForwardRef() directly
-                for a_n, a_t in check_type.__dict__.get('__annotations__', {}).items():
-                    _iter(a_n, a_t, level + (1 if is_in_list else 0))
+                # do not iterate check_type.__fields__ but iterate __annotations__ instead
+                # e.g,
+                # if use check_type.__fields__, when checking project.members, will fall into user.team and team.members recursion
+                # because the import mechanism, it is not possible to make explicit reference between user and team, so using annotations can prevent the recursion
+                for c_n, c_t in check_type.__dict__.get('__annotations__', {}).items():
+                    c_f = check_type.__fields__[c_n]
+                    # Skip relation field
+                    if isinstance(c_f, RelationField):
+                        continue
+                    #
+                    _iter(c_n, c_t, level + (1 if is_in_list else 0))
 
         #
         for f in fields.values():
+            # Skip relation field
+            if isinstance(f, RelationField):
+                continue
+            #
             _iter(f.name, f.type, 0)
         #
         if max_list_depth >= 3:
             raise SchemaError(f'Model {name} is too deep: {max_list_depth}')
         #
         # Create class
         #
@@ -542,47 +634,87 @@
         #
         if has_forward_refs:
             globalns = sys.modules[cls.__module__].__dict__.copy()
             globalns.setdefault(cls.__name__, cls)
             for f in cls.__fields__.values():
                 f_origin = get_origin(f.type)
                 if f_origin is dict:
-                    _, typ = get_args(f.type)
-                    if typ.__class__ == ForwardRef:
-                        f.type = Dict[evaluate_forward_ref(typ, globalns)]
+                    _, f_type = get_args(f.type)
+                    if f_type.__class__ == ForwardRef:
+                        f.type = Dict[evaluate_forward_ref(f_type, globalns)]
                 elif f_origin is list:
-                    typ = get_args(f.type)[0]
-                    if typ.__class__ == ForwardRef:
-                        f.type = List[evaluate_forward_ref(typ, globalns)]
+                    f_type = get_args(f.type)[0]
+                    if f_type.__class__ == ForwardRef:
+                        f.type = List[evaluate_forward_ref(f_type, globalns)]
                 else:
-                    typ = f.type
-                    if typ.__class__ == ForwardRef:
-                        f.type = evaluate_forward_ref(typ, globalns)
+                    f_type = f.type
+                    if f_type.__class__ == ForwardRef:
+                        f.type = evaluate_forward_ref(f_type, globalns)
+        #
+        # Try to create back field of relation fields after this class is created
+        #
+        for f in cls.__fields__.values():
+            if isinstance(f, RelationField) and f.back_field_name:  # Do not create back field in related model if back_field_name is None
+                back_field = RelationField(
+                    name=f.back_field_name, type_=List[cls] if f.back_field_is_list else cls,
+                    save_field_name=f.save_field_name, save_field_order=f.back_field_order,
+                    required=False,  # back field is used for display only, so it is not required
+                    editable=False,  # ditto
+                    format_=f.back_field_format, icon=f.back_field_icon, title=f.back_field_title, description=f.back_field_description,
+                    unit=f.back_field_unit,
+                    ownership=f.ownership,
+                    is_back_field=True,  # Mark this field to be a back field created by a relation field
+                )
+                f_origin = get_origin(f.type)
+                if f_origin is dict:
+                    _, f_type = get_args(f.type)
+                elif f_origin is list:
+                    f_type = get_args(f.type)[0]
+                else:
+                    f_type = f.type
+                # Update related model
+                f_type.__fields__[f.back_field_name] = back_field
+                f_type.__slots__ = tuple(f_type.__slots__) + (f.back_field_name,)
+                f_type.__relations__[f.back_field_name] = back_field
+
         #
         return cls
 
 
 class BaseModel(metaclass=ModelMeta):
     """ Base Model. """
 
     __slots__ = ('__dict__', '__errors__')
     __doc__ = ''
     #
-    # Fields sould be overwrited
+    # Fields may be overwrited
+    #
+    # The id field name
+    __id_name__ = None
+    __id_type__ = None
     #
     __icon__ = None
     __title__ = None
     __description__ = None
-    # TODO: Validate all fields in layout are defined
-    # Define fields can be show in query result table or card
-    __columns__ = []
-    # Define layouts to render form or detail page
-    __layout__ = None
-    __read__ = None
-    __form__ = None
+    # Views for this model, should be a dict
+    # i.e,
+    # {
+    #   view_name: {                    # View name should be unique, in blueprint/view format, if blueprint is not specified, use default public by default
+    #     domains: ['www'],             # Domains that this view can be generated, should always be application's name
+    #     layout: '''action?param=1     # Layout of this view, we use this layout to generate corresponding view and template source code
+    #       field_string, field_select
+    #       field_image
+    #       field_object
+    #         field_string
+    #       field_textarea
+    #     ''',
+    #   },
+    #   ...
+    # }
+    __views__ = {}
 
     def __init__(self, *d: Dict[str, Any], **data: Any) -> None:
         """ Init.
 
         :param d: create model from dict
         :param **data: create model from kwargs
         """
@@ -604,23 +736,78 @@
         :param data: Inner sub models can be dict or model instance
         """
         values = {}
         errors = []
         # Validate against schema
         # print(f'Validate {cls.__name__} with {data}')
         for field_name, field_type in cls.__fields__.items():
+            # Skip recursive validation in relation value, just keep the relation value
+            # please note: in save logic, we need to skip relation field, e.g, in mongosupport, we use self.dict(include_relations=False)
+            if isinstance(field_type, RelationField):
+                relation_value = data.get(field_name, Undefined)
+                if relation_value is not Undefined:
+                    data[field_name] = relation_value
+                #
+                continue
+            #
+            # Update id/ids field created by relation field
+            # But can NOT do update in back relation field
+            # e.g,
+            # user.team -> team.members, team_id is saved in user model, we can use user.team = another team to update it
+            # However, it is not supported to update by team.members.append(user), because it is complex to implement below:
+            #   - Need to implement some logic to remember which users are removed and appended from team, especially there are huge amount of members
+            #   - Add transaction support to update these users before updating team object
+            #
+            if field_type.source_field_name is not None:  # e.g, team_id is created by team relation, so source field name of team_id is team
+                source_field = cls.__fields__[field_type.source_field_name]
+                relation_value = data.get(source_field.name, Undefined)  # e.g, get team value
+                # RelationField's value is lazy loaded, undefined means it is not load, so trust the value in current field
+                if relation_value is Undefined:
+                    pass
+                # If it is not Undefined, means it is already loaded and may be updated programmtically, so overwrite current field
+                else:
+                    update_value = None
+                    if isinstance(relation_value, list):
+                        relation_type = get_args(source_field.type)[0]
+                        update_value = []
+                        for v in relation_value:
+                            if isinstance(v, dict):  # Value can be raw dict against related model
+                                id_ = v.get(relation_type.__id_name__)
+                            else:  # Value should be instance of relatited model
+                                id_ = getattr(v, relation_type.__id_name__)
+                            #
+                            if id_:
+                                if not isinstance(id_, relation_type.__id_type__):
+                                    id_ = relation_type.__id_type__(id_)
+                                #
+                                update_value.append(id_)
+                    elif relation_value is not None:
+                        relation_type = source_field.type
+                        if isinstance(relation_value, dict):
+                            id_ = relation_value.get(relation_type.__id_name__)
+                        else:
+                            id_ = getattr(relation_value, relation_type.__id_name__)
+                        #
+                        if id_:
+                            if not isinstance(id_, relation_type.__id_type__):
+                                id_ = relation_type.__id_type__(id_)
+                            #
+                            update_value = id_
+                    # update_value can be none or [], meaning clear the field
+                    data[field_name] = update_value
+            #
             field_value, field_errors = cls._validate_field(field_type, data.get(field_name, Undefined))
             if field_value is not Undefined:
                 values[field_name] = field_value
             if field_errors:
                 errors.extend(field_errors)
         # Check if any non-defined fields
         undefined_fields = set(data.keys()) - set(cls.__fields__.keys())
         if len(undefined_fields) > 0:
-            # Do not raise error for non-defined fields
+            # Do not raise error for non-defined fields, because we are using __dict__ to store data and other dynamic attributes also use __dict__ to store
             # errors.append(f'{cls.__name__}: Found undefined data fields, {undefined_fields}')
             pass
         #
         return values, errors
 
     @classmethod
     def _validate_field(cls, field: ModelField, value: Any):
@@ -720,36 +907,97 @@
         """ Del a field. """
         if name not in self.__dict__:
             raise AttributeError(name)
         #
         del self.__dict__[name]
 
     def __getattr__(self, name):
-        """ Try to init a field if it is not in self.__dict__. """
+        """ Try to init a field if it is not in self.__dict__.
+
+        Note: When an attribute is accessed, __getattribute__ is invoked firstly
+        and then if the attribute wasn't found, __getattr__ should be invoked.
+        """
+        # Return _depends data defined in a field, which can be function to return dynamic data
+        if name.endswith('_depends'):
+            name = name.split('_depends')[0]
+            field = self.__class__.__fields__.get(name)
+            if field and field.depends:
+                depends = field.depends
+                if callable(depends):
+                    # check if _depends function has arguments
+                    if depends.__code__.co_argcount == 0:
+                        return depends()
+                    else:
+                        return depends(self)  # Can only have one argument at most
+                else:
+                    return depends
+        #
         if name in self.__class__.__fields__:
-            type_ = self.__class__.__fields__[name].type
-            origin = get_origin(type_)
-            v = None
-            if origin is None:
-                if issubclass(type_, BaseModel):
-                    v = type_()
-            elif origin is list:
-                v = []
-            elif origin is dict:
-                v = {}
-            #
-            if v is not None:
-                self.__setattr__(name, v)
+            field = self.__class__.__fields__[name]
+            f_type = field.type
+            f_origin = get_origin(f_type)
+            # Try to init relation values lazy
+            if isinstance(field, RelationField):
+                # TODO: filter param is in mongodb's format, maybe more abstract approach is needed
+                if f_origin is None:
+                    # This is a back field created by relation field, means id is saved in one relation object
+                    if field.is_back_field:
+                        default = f_type.find_one({field.save_field_name: self.__dict__.get(self.__class__.__id_name__)})
+                    else:
+                        default = f_type.find_one({f_type.__id_name__: self.__dict__.get(field.save_field_name)})
+                elif f_origin is list:
+                    l_type = get_args(f_type)[0]
+                    # This is a back field created by relation field, means this object id is saved in many related objects
+                    if field.is_back_field:
+                        # TODO: support paging, e.g, team.members__2 to fetch page 2's records and defined a back_field_page_size to config paging size
+                        # Typical many-to-one definition way, i.e, using a foreign key to store related object's id
+                        # In such case, may return very big amount of object so we only fetch part of it, i.e, 100 records
+                        # e.g,
+                        # Relation field is defined in User using field name team, so the team id stores in a field name team_id, a back relation field with name members is auto-created in Team
+                        # user.team -> team.members, then team.members = User.find({team_id: self._id}, sort=[{team.join_time, 1}])
+                        default = list(
+                            l_type.find(
+                                {field.save_field_name: self.__dict__.get(self.__class__.__id_name__)},
+                                sort=field.save_field_order,
+                                limit=100)
+                        )
+                    else:
+                        # Please note: Databases like mongodb supports list format field
+                        # In such case, the ids field should not be very large, so we fetch all the objects and sort them by id's position
+                        # e.g,
+                        # Relation field is defined in Team using field name members, so the team ids store in a field name members_ids
+                        # team.members -> user.team, then team.members = User.find({_id: {$in: self.members_ids}})
+                        ids = self.__dict__.get(field.save_field_name)
+                        if ids is None:
+                            default = []
+                        else:
+                            default = list(l_type.find({l_type.__id_name__: {'$in': ids}}))
+                            default.sort(key=lambda i: ids.index(getattr(i, l_type.__id_name__)))
+                elif f_origin is dict:
+                    default = None
+                # If relation return None, we need to set the field to None
+                # So that in the second access on the field, we can return None directly
+                # This is a key step to implement the lazy loading for relation field
+                self.__setattr__(name, default)
+            else:
+                default = None
+                if f_origin is None:
+                    if issubclass(f_type, BaseModel):
+                        # Create inner model automatically
+                        default = f_type()
+                elif f_origin is list:
+                    default = []
+                elif f_origin is dict:
+                    default = {}
+                #
+                if default is not None:
+                    self.__setattr__(name, default)
             #
-            return v
-        # Because __dict__ is overwrited by values, so we need invoke relation mannaully
-        if name in self.__class__.__relations__:
-            rel = self.__class__.__relations__[name]
-            return rel.__get__(self)
-        # Invoke property mannaully
+            return default
+        # Because __dict__ is overwrited by values, so we need to invoke property mannaully
         if name in self.__class__.__properties__:
             prp = self.__class__.__properties__[name]
             return prp.__get__(self)
         #
         raise AttributeError(f'\'{self.__class__.__name__}\' object has no attribute \'{name}\'')
 
     def __str__(self):
@@ -829,203 +1077,237 @@
             encode: bool = False,
             include: dict = None,
             exclude: dict = None,
             include_relations: bool = False,
     ):
         """ Access model recrusively. """
         for field_name, field_value in self.__dict__.items():
-            #
-            yield field_name, self._get_value(field_value, to_dict,
-                                              encode, include, exclude, include_relations)
-        #
-        if include_relations:
-            for relation_name in self.__class__.__relations__:
-                relation_value = getattr(self, relation_name)
-                # Note: Prevent infinite recursion on calling relations
-                yield relation_name, self._get_value(relation_value, to_dict,
-                                                     encode, include, exclude, False)
+            field = self.__class__.__fields__[field_name]
+            if isinstance(field, RelationField):
+                if include_relations:
+                    yield field_name, getattr(self, field_name)
+            else:
+                yield field_name, self._get_value(field_value, to_dict, encode, include, exclude, include_relations)
 
     def _get_value(
             self, v,
             to_dict: bool,
             encode: bool,
             include: dict,
             exclude: dict,
             include_relations: bool,
     ):
         """ Access model field recrusively. """
         if isinstance(v, dict):
             return {
-                k_: self._get_value(v_, to_dict, encode,
-                                    include,
-                                    exclude,
-                                    include_relations)
+                k_: self._get_value(v_, to_dict, encode, include, exclude, include_relations)
                 for k_, v_ in v.items()
             }
         elif isinstance(v, list):
             return [
-                self._get_value(v_, to_dict, encode,
-                                include,
-                                exclude,
-                                include_relations)
+                self._get_value(v_, to_dict, encode, include, exclude, include_relations)
                 for i, v_ in enumerate(v)
             ]
         elif isinstance(v, BaseModel):
             if to_dict:
                 return v.dict(encode=encode, include=include, exclude=exclude, include_relations=include_relations)
             else:
                 return v.copy()
         else:
             if encode:
                 if isinstance(v, ObjectId):
                     return str(v)
                 elif isinstance(v, datetime):
                     return v.strftime(DATETIME_FORMAT_SHORT)
+            #
             return v
 
     def json(self, **kwargs) -> str:
         """ Convert to json str. """
         return json.dumps(self.dict(), cls=ModelJSONEncoder, **kwargs)
 
     @classmethod
-    def schema(cls):
+    def find_one(cls, filter_or_id, *args, **kwargs):
+        """ abstract method, use it to fetch one related model. """
+        return None
+
+    @classmethod
+    def find(cls, *args, **kwargs):
+        """ abstract method, use it to fetch many related models. """
+        return []
+
+    @classmethod
+    def schema(cls, layouts={}):
         """ To json schema dict.
 
         NOTE:
         Return json schema is a subset of Object Schema from OAS 3.0.
         In order to keep all the things simple, we do not use complex keywords such as oneOf, $ref, patternProperties, additionalProperties, etc.
         https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md#schemaObject
         https://swagger.io/docs/specification/data-models/
 
-        However, we still have some grammars
+        However, we still have some grammars, e.g,
           - add type date
-          - add enum_titles, py_type, layout, form, read, icon, stat, readonly to help code generation
-          - Add format to array, so that we can gen a component for the whole array
-          - Add searchables to object, so that it can be used to generate search form
-          - Add sortables to object, so that it can be used to generate order drowpdown
-          - Add columns to object, so that it can be used to generate columns for table
+          - add enum_titles, py_type, icon, editable to help code generation
+          - add format to array, so that we can gen a component for the whole array
+          - add searchables to object, so that it can be used to generate search form
+          - add sortables to object, so that it can be used to generate order drowpdown
         """
 
-        def _gen_schema(type_: Type):
-
+        def _gen_schema(type_: Type, parents=[]):
             """ Generate schema for type. """
             if isinstance(type_, SimpleEnumMeta):
-                enum = _gen_schema(type_.type)
+                enum = _gen_schema(type_.type, parents)
                 enum.update({
                     'enum': list(type_),
                     'enum_titles': type_.titles,
                     'format': Format.SELECT,
                     'py_type': type_.__name__,
                 })
                 return enum
             elif issubclass(type_, BaseModel):
-                stat = None
-                properties = {}
-                required, searchables, sortables = [], [], []
+                # Need to prevent recursively access
+                # e.g,
+                #   User.friends:User == #User
+                #   User.team:Team -> Team.members:List[User] == List[#User]
+                check_parents = [type_.__name__] + parents
+                #
+                properties = {}  # {field_name:field_schema}
+                requires, searchables, sortables = [], [], []
+                relations = {}  # {model_name:[field_name]}, use dict to keep the order
                 for f_n, f_t in type_.__fields__.items():
                     field_schema = {}
-                    origin = get_origin(f_t.type)
+                    f_origin = get_origin(f_t.type)
+                    inner_type = None
                     # Dict
-                    if origin is dict:
+                    if f_origin is dict:
+                        f_type = get_args(f_t.type)[1]
                         # TODO: SUPPORT DICT
-                        pass
                     # List
-                    elif origin is list:
-                        l_type = get_args(f_t.type)[0]
-                        # https://json-schema.org/understanding-json-schema/structuring.html#recursion
-                        # Self-referencing
-                        if l_type == type_:
+                    elif f_origin is list:
+                        f_type = get_args(f_t.type)[0]
+                        if f_type.__name__ in check_parents:
                             field_schema.update({
                                 'type': 'array',
-                                'items': {'$ref': '#'},
-                                'py_type': f'List[{type_.__name__}]',
+                                # Your program should use the reference object's schema to replace `items` value
+                                'items': {'ref': f_type.__name__},
+                                'py_type': f'List[{f_type.__name__}]',
                             })
                         else:
-                            inner_type = _gen_schema(l_type)
+                            inner_type = _gen_schema(f_type, check_parents)
                             field_schema.update({
                                 'type': 'array',
                                 'items': inner_type,
                                 'py_type': f'List[{inner_type["py_type"]}]',
                             })
                     # built-in type, SimpleEnum or sub model
                     else:
-                        if f_t.type == type_:  # Self-referencing
-                            field_schema.update({'$ref': '#'})
+                        f_type = f_t.type
+                        if f_type.__name__ in check_parents:
+                            field_schema.update({
+                                'type': 'object',
+                                # Your program should use the reference object's schema to replace `properties` under current schema
+                                # But should NOT overwrite the icon/title/description/... as these fields may use different values
+                                'ref': f_type.__name__,
+                                'py_type': f_type.__name__,
+                            })
                         else:
-                            inner_type = _gen_schema(f_t.type)
+                            inner_type = _gen_schema(f_type, check_parents)
                             field_schema.update(inner_type)
                     # default
                     if f_t.default:
                         # Skip if default is callable, e.g, datetime.now
                         if callable(f_t.default):
                             pass
                         else:
                             default = f_t.default
                             field_schema.update({'default': default})
                     # icon
                     if f_t.icon:
                         field_schema.update({'icon': f_t.icon})
+                    else:
+                        if inner_type and 'icon' in inner_type:
+                            field_schema.update({'icon': inner_type['icon']})
                     # title
                     field_schema.update({'title': f_t.title if f_t.title else f_n.upper()})
                     # description
                     if f_t.description:
                         field_schema.update({'description': f_t.description})
                     # unit
                     if f_t.unit:
                         field_schema.update({'unit': f_t.unit})
                     # format, overwrite default format
                     if f_t.format:
                         field_schema.update({'format': f_t.format})
                         #
                         if f_t.format in [Format.DATE, Format.DATETIME]:
                             field_schema.update({'type': 'date'})
-                        elif f_t.format == Format.STATISTIC:
-                            stat = f_n
                     # required
                     if f_t.required:
                         field_schema.update({'required': True})
-                        required.append(f_n)
-                    # readonly
-                    if f_t.readonly:
-                        field_schema.update({'readonly': True})
+                        requires.append(f_n)
+                    # editable
+                    field_schema.update({'editable': f_t.editable})
                     # searchable
                     if f_t.searchable is not None:
                         searchables.append((f_n, f_t.searchable))
                     # sortable
                     if f_t.sortable is True:
                         sortables.append(f_n)
+                    # depends, only update it to true, then you can access it by {field_name}_depends in page rendering or biz logic
+                    if f_t.depends:
+                        field_schema.update({'depends': True})
+                    # relation
+                    if isinstance(f_t, RelationField):
+                        field_schema.update({'is_relation': True})
+                        #
+                        if f_t.ownership:
+                            field_schema.update({'ownership': f_t.ownership})
+                        #
+                        field_schema.update({'is_out_relation': not f_t.is_back_field})
+                        field_schema.update({'is_back_relation': f_t.is_back_field})
+                        #
+                        field_schema.update({'save_field_name': f_t.save_field_name})
+                        #
+                        relations.setdefault(f_type.__name__, [])
+                        relations[f_type.__name__] += [f_n]
                     #
                     properties[f_n] = field_schema
                 #
                 obj = {
                     'type': 'object',
                     'properties': properties,
-                    'required': required,
-                    'columns': type_.__columns__ if type_.__columns__ else required,  # Using required fields as columns as the default
+                    'requires': requires,
+                    'editable': True,
                     'py_type': type_.__name__,
                     'icon': type_.__icon__ if type_.__icon__ else None,
                     'title': type_.__title__ if type_.__title__ else type_.__name__.upper(),
                     'description': type_.__description__ if type_.__description__ else None,
+                    # searchables, [field__comparator|field]
+                    'searchables': [('{}__{}'.format(*s) if s[1] != Comparator.EQ else s[0]) for s in searchables],
+                    'searchable_fields': [s[0] for s in searchables],
+                    # sortables, [(field_name, 1/-1)]
+                    'sortables': sortables,
+                    'relations': [k for k in relations.keys() if k != type_.__name__],  # skip self
+                    # id_name & id_type, used for relation inputs
+                    'id_name': type_.__id_name__,
+                    'id_type': type_.__id_type__.__name__ if type_.__id_type__ else None,
                 }
-                # layout
-                if type_.__layout__:
-                    layout = parse_layout(type_.__layout__)[0]
-                else:
-                    layout = [[f] for f in properties.keys()]  # Each field has one row
-                #
-                obj['layout'] = layout
-                obj['read'] = parse_layout(type_.__read__)[0] if type_.__read__ else layout
-                obj['form'] = parse_layout(type_.__form__)[0] if type_.__form__ else layout
-                # searchables
-                obj['searchables'] = [('{}__{}'.format(*s) if s[1] != Comparator.EQ else s[0]) for s in searchables]
-                # sortables
-                obj['sortables'] = sortables
-                #
-                if stat:
-                    obj['stat'] = stat
+                # Inject layouts into schema
+                if layouts:
+                    layout = layouts.get(type_.__name__, {})
+                    if not layout.get('columns'):
+                        layout['columns'] = obj['requires']
+                    if not layout.get('read'):
+                        # Each field is a row
+                        layout['read'] = [[{'name': f, 'params': {}}] for f in obj['properties'].keys()]
+                    if not layout.get('form'):
+                        layout['form'] = layout['read']
+                    #
+                    obj.update(layout)
                 #
                 return obj
             elif type_ is str:
                 return {'type': 'string', 'format': Format.TEXT, 'py_type': 'str'}
             elif type_ is int:
                 return {'type': 'integer', 'format': Format.INT, 'py_type': 'int'}
             elif type_ is float:
@@ -1036,9 +1318,8 @@
                 return {'type': 'string', 'format': Format.OBJECTID, 'py_type': 'ObjectId'}
             elif type_ is datetime:
                 return {'type': 'date', 'format': Format.DATETIME, 'py_type': 'datetime'}
 
         #
         ret = _gen_schema(cls)
         # print(json.dumps(ret))
-        #
         return ret
```

### Comparing `py3seed-0.0.99/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.1.1/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.0.99
+Version: 0.1.1
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

