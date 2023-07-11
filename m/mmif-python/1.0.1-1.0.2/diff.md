# Comparing `tmp/mmif-python-1.0.1.tar.gz` & `tmp/mmif-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmif-python-1.0.1.tar", last modified: Fri May 26 13:34:57 2023, max compression
+gzip compressed data, was "mmif-python-1.0.2.tar", last modified: Tue Jul 11 01:07:32 2023, max compression
```

## Comparing `mmif-python-1.0.1.tar` & `mmif-python-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.949401 mmif-python-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-26 13:34:05.000000 mmif-python-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 13:34:05.000000 mmif-python-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 13:34:57.949401 mmif-python-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-26 13:34:05.000000 mmif-python-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 13:34:05.000000 mmif-python-1.0.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.945401 mmif-python-1.0.1/mmif/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.945401 mmif-python-1.0.1/mmif/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/res/clams.vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/res/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/res/mmif.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.945401 mmif-python-1.0.1/mmif/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/serialize/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/serialize/mmif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/serialize/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/serialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.945401 mmif-python-1.0.1/mmif/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/ver/do-not-edit.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.949401 mmif-python-1.0.1/mmif/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/vocabulary/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/vocabulary/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/vocabulary/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/vocabulary/document_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.949401 mmif-python-1.0.1/mmif_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 13:34:05.000000 mmif-python-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:34:57.949401 mmif-python-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-05-26 13:34:05.000000 mmif-python-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.870120 mmif-python-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-11 01:06:51.000000 mmif-python-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 01:06:51.000000 mmif-python-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-11 01:07:32.870120 mmif-python-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-11 01:06:51.000000 mmif-python-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 01:06:51.000000 mmif-python-1.0.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.862120 mmif-python-1.0.2/mmif/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.862120 mmif-python-1.0.2/mmif/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/res/clams.vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/res/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/res/mmif.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.862120 mmif-python-1.0.2/mmif/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19491 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/serialize/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/serialize/mmif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/serialize/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-07-11 01:06:51.000000 mmif-python-1.0.2/mmif/serialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.866120 mmif-python-1.0.2/mmif/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/ver/do-not-edit.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.866120 mmif-python-1.0.2/mmif/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/vocabulary/annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/vocabulary/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/vocabulary/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif/vocabulary/document_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:07:32.870120 mmif-python-1.0.2/mmif_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 01:07:32.000000 mmif-python-1.0.2/mmif_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 01:06:51.000000 mmif-python-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 01:07:32.870120 mmif-python-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-11 01:06:51.000000 mmif-python-1.0.2/setup.py
```

### Comparing `mmif-python-1.0.1/LICENSE` & `mmif-python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.1/PKG-INFO` & `mmif-python-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-1.0.1/mmif/res/clams.vocabulary.yaml` & `mmif-python-1.0.2/mmif/res/clams.vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.1/mmif/res/mmif.json` & `mmif-python-1.0.2/mmif/res/mmif.json`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.1/mmif/serialize/annotation.py` & `mmif-python-1.0.2/mmif/serialize/annotation.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,38 +2,48 @@
 The :mod:`annotation` module contains the classes used to represent a
 MMIF annotation as a live Python object.
 
 In MMIF, annotations are created by apps in a pipeline as a part
 of a view. For documentation on how views are represented, see
 :mod:`mmif.serialize.view`.
 """
+import importlib
 import itertools
 import pathlib
-from typing import Union, Dict, List, Type, Optional, Iterator, MutableMapping, TypeVar
+import pkgutil
+import re
+import typing
+import warnings
+from typing import Union, Dict, List, Optional, Iterator, MutableMapping, TypeVar
 from urllib.parse import urlparse
 
 from mmif.vocabulary import ThingTypesBase, DocumentTypesBase
-from .model import MmifObject
+from .model import MmifObject, JSON_PRMTV_TYPES
 
 __all__ = ['Annotation', 'AnnotationProperties', 'Document', 'DocumentProperties', 'Text']
 
 T = TypeVar('T')
 
-from .. import DocumentTypes
+from .. import DocumentTypes, AnnotationTypes
 
-JSON_COMPATIBLE_PRIMITIVES: Type = Union[str, int, float, bool, None]
+discovered_docloc_plugins = {
+    name[len('mmif_docloc_'):]: importlib.import_module(name) for _, name, _ in pkgutil.iter_modules() if re.match(r'mmif[-_]docloc[-_]', name)
+}
 
 
 class Annotation(MmifObject):
     """
     MmifObject that represents an annotation in a MMIF view.
     """
 
     def __init__(self, anno_obj: Optional[Union[bytes, str, dict]] = None) -> None:
         self._type: ThingTypesBase = ThingTypesBase('')
+        # to store the parent view ID
+        self._parent_view_id = ''
+        self.reserved_names.add('_parent_view_id')
         if not hasattr(self, 'properties'):  # don't overwrite DocumentProperties on super() call
             self.properties: AnnotationProperties = AnnotationProperties()
             self._attribute_classes = {'properties': AnnotationProperties}
         self.disallow_additional_properties()
         self._required_attributes = ["_type", "properties"]
         super().__init__(anno_obj)
     
@@ -59,46 +69,76 @@
     def at_type(self, at_type: Union[str, ThingTypesBase]) -> None:
         if isinstance(at_type, str):
             self._type = ThingTypesBase.from_str(at_type)
         else:
             self._type = at_type
 
     @property
+    def parent(self) -> str:
+        return self._parent_view_id
+
+    @parent.setter
+    def parent(self, parent_view_id: str) -> None:
+        # I want to make this to accept `View` object as an input too,
+        # but import `View` will break the code due to circular imports
+        self._parent_view_id = parent_view_id
+
+    @property
     def id(self) -> str:
         return self.properties.id
 
     @id.setter
     def id(self, aid: str) -> None:
         self.properties.id = aid
+        
+    @staticmethod
+    def check_prop_value_is_simple_enough(
+            value: Union[JSON_PRMTV_TYPES, List[JSON_PRMTV_TYPES], List[List[JSON_PRMTV_TYPES]]]):
+        def json_primitives(x): 
+            return isinstance(x, typing.get_args(JSON_PRMTV_TYPES))
+        return json_primitives(value) \
+            or (isinstance(value, list) and all(map(json_primitives, value))) \
+            or (all(map(lambda elem: isinstance(elem, list), value)) and map(json_primitives, [subelem for elem in value for subelem in elem]))
 
     def add_property(self, name: str,
-                     value: Union[JSON_COMPATIBLE_PRIMITIVES,
-                                  List[JSON_COMPATIBLE_PRIMITIVES],
-                                  List[List[JSON_COMPATIBLE_PRIMITIVES]]
-                    ]) -> None:
+                     value: Union[JSON_PRMTV_TYPES, List[JSON_PRMTV_TYPES], List[List[JSON_PRMTV_TYPES]]]
+                     ) -> None:
         """
         Adds a property to the annotation's properties.
         :param name: the name of the property
         :param value: the property's desired value
         :return: None
         """
-        json_primitives = lambda x:isinstance(x, JSON_COMPATIBLE_PRIMITIVES.__args__)
-        if json_primitives(value) or (
-                isinstance(value,list)
-                and all(map(json_primitives, value)) or (
-                        all(map(lambda elem: isinstance(elem, list), value))
-                        and map(json_primitives, [subelem for elem in value for subelem in elem])
-                )
-        ):
+        if self.check_prop_value_is_simple_enough(value):
             self.properties[name] = value
         else:
             raise ValueError("Property values cannot be a complex object. It must be "
                              "either string, number, boolean, None, or a list of them."
                              f"(\"{name}\": \"{str(value)}\"")
 
+    def get(self, prop_name: str) -> Union['AnnotationProperties', JSON_PRMTV_TYPES, List[JSON_PRMTV_TYPES], List[List[JSON_PRMTV_TYPES]]]:
+        """
+        A special getter for Annotation properties. This is to allow for
+        directly accessing properties without having to go through the
+        properties object.
+        """
+        if prop_name in {'at_type', '@type'}:
+            return str(self._type)
+        elif prop_name == 'properties':
+            return self.properties
+        elif prop_name in self.properties:
+            return self.properties[prop_name]
+        else:
+            raise KeyError(f"Property {prop_name} does not exist in this annotation.")
+
+    get_property = get
+
+    def __getitem__(self, prop_name: str):
+        return self.get(prop_name)
+    
     def is_document(self):
         return isinstance(self.at_type, DocumentTypesBase)
 
 
 class Document(Annotation):
     """
     Document object that represents a single document in a MMIF file.
@@ -109,44 +149,89 @@
     subdocuments grouped together logically.
 
     If ``document_obj`` is not provided, an empty Document will be generated.
 
     :param document_obj: the JSON data that defines the document
     """
     def __init__(self, doc_obj: Optional[Union[bytes, str, dict]] = None) -> None:
-        # to store the parent view ID
-        self._parent_view_id = ''
-        self.reserved_names.add('_parent_view_id')
+        # see https://github.com/clamsproject/mmif-python/issues/226 for discussion
+        # around the use of these three dictionaries
+        self._props_original: DocumentProperties = DocumentProperties()
+        self._props_existing: AnnotationProperties = AnnotationProperties()
+        self._props_temporary: AnnotationProperties = AnnotationProperties()
+        self.reserved_names.update(('_props_original', '_props_existing', '_props_temporary'))
         
         self._type: Union[ThingTypesBase, DocumentTypesBase] = ThingTypesBase('')
-        self.properties: DocumentProperties = DocumentProperties()
+        self.properties = self._props_original
         self.disallow_additional_properties()
         self._attribute_classes = {'properties': DocumentProperties}
         super().__init__(doc_obj)
-
-    @property
-    def parent(self) -> str:
-        return self._parent_view_id
-
-    @parent.setter
-    def parent(self, parent_view_id: str) -> None:
-        # I want to make this to accept `View` object as an input too,
-        # but import `View` will break the code due to circular imports
-        self._parent_view_id = parent_view_id
+    
+    def _add_property_from_annotation(self, annotation: Annotation):
+        if annotation.at_type != AnnotationTypes.Annotation:
+            raise ValueError("Only `Annotation` type can be added as a property to a `Document` object.")
+        for prop_name, prop_value in annotation.properties.items():
+            self._props_existing[prop_name] = prop_value
 
     def add_property(self, name: str,
-                     value: Union[JSON_COMPATIBLE_PRIMITIVES,
-                                  List[JSON_COMPATIBLE_PRIMITIVES]]) -> None:
+                     value: Union[JSON_PRMTV_TYPES, List[JSON_PRMTV_TYPES]]
+                     ) -> None:
+        """
+        Adds a property to the document's properties.
+        
+        Unlike the parent :class:`Annotation` class, added properties of a 
+        ``Document`` object can be lost during serialization unless it belongs 
+        to somewhere in a ``Mmif`` object. This is because we want to keep 
+        ``Document`` object as "read-only" as possible. Thus, if you want to add 
+        a property to a ``Document`` object, 
+        
+        * add the document to a ``Mmif`` object (either in the documents list or 
+          in a view from the views list), or
+        * directly write to ``Document.properties`` instead of using this method
+          (which is not recommended). 
+        
+        With the former method, the SDK will record the added property as a 
+        `Annotation` annotation object, separate from the original `Document` 
+        object. See :meth:`.Mmif.generate_capital_annotations()` for more.
+        
+        A few notes to keep in mind:
+        
+        #. You can't overwrite an existing property of a ``Document`` object. 
+        #. A MMIF can have multiple ``Annotation`` objects with the same 
+           property name but different values. When this happens, the SDK will
+           only keep the latest value (in order of appearances in views list) of 
+           the property, effectively overwriting the previous values.
+        """
         if name == "text":
             self.properties.text = Text(value)
+        elif name == "mime":
+            self.properties.mime = str(value)
         elif name == "location":
             self.location = value
+        elif name not in self._props_original:
+            if self.check_prop_value_is_simple_enough(value):
+                self._props_temporary[name] = value
+            else:
+                super().add_property(name, value)
+
+    def get(self, prop_name):
+        """
+        A special getter for Document properties. This is to allow for reading 
+        the three properties in a specific order so that the latest value is 
+        returned, in case there are multiple values for the same key.
+        """
+        if prop_name in self._props_temporary:
+            return self._props_temporary[prop_name]
+        elif prop_name in self._props_existing:
+            return self._props_existing[prop_name]
         else:
-            super().add_property(name, value)
+            return super().get(prop_name)
 
+    get_property = get
+    
     @property
     def text_language(self) -> str:
         if self.at_type == DocumentTypes.TextDocument:
             return self.properties.text_language
         else:
             raise ValueError("Only TextDocument can have `text` field.")
 
@@ -206,19 +291,20 @@
         Retrieves the full address from the document location URI.
         Returns None when no location is set.
         """
         return self.properties.location_address()
 
     def location_path(self) -> Optional[str]:
         """
-        Retrieves only path name of the document location (hostname is ignored). 
-        Useful to get a path of a local file.
+        Retrieves a path that's resolved to a pathname in the local file system.
+        To obtain the original value of the "path" part in the location string
+        (before resolving), use ``properties.location_path_literal`` method.
         Returns None when no location is set.
         """
-        return self.properties.location_path()
+        return self.properties.location_path_resolved()
 
 
 class AnnotationProperties(MmifObject, MutableMapping[str, T]):
     """
     AnnotationProperties object that represents the
     ``properties`` object within a MMIF annotation.
 
@@ -237,15 +323,15 @@
     def __iter__(self) -> Iterator[str]:
         """
         ``__iter__`` on Mapping should basically work as ``keys()`` method of vanilla dict
         however, when MMIF objects are serialized, all optional (not in ``_req_atts``),
         empty props are ignored (note that emtpy but required props are serialized 
         with the *emtpy* value). 
         Hence, this ``__iter__`` method should also work in the same way and 
-        ignored empty but optional props. 
+        ignore empty optional props. 
         """
         for key in itertools.chain(self._named_attributes(), self._unnamed_attributes):
             if key in self._required_attributes:
                 yield key
             else:
                 try:
                     self.__getitem__(key)
@@ -345,17 +431,40 @@
         parsed_location = urlparse(self.location)
         if len(parsed_location.netloc) == 0:
             return parsed_location.path
         else:
             return "".join((parsed_location.netloc, parsed_location.path))
 
     def location_path(self) -> Optional[str]:
+        warnings.warn('location_path() is deprecated. Use location_path_resolved() instead.', DeprecationWarning)
+        return self.location_path_resolved()
+    
+    def location_path_resolved(self) -> Optional[str]:
+        """
+        Retrieves only path name of the document location (hostname is ignored), 
+        and then try to resolve the path name in the local file system.
+        This method should be used when the document scheme is ``file`` or empty.
+        For other schemes, users should install ``mmif-locdoc-<scheme>`` plugin.
+        
+        Returns None when no location is set.
+        Raise ValueError when no code found to resolve the given location scheme.
+        """
+        if self.location is None:
+            return None
+        scheme = self.location_scheme()
+        if scheme in ('', 'file'):
+            return urlparse(self.location).path
+        elif scheme in discovered_docloc_plugins:
+            return discovered_docloc_plugins[scheme].resolve(self.location)
+        else:
+            raise ValueError(f'Cannot resolve location of scheme "{scheme}". Interested in developing mmif-locdoc-{scheme} plugin? See https://clams.ai/mmif-python/plugins')
+
+    def location_path_literal(self) -> Optional[str]:
         """
         Retrieves only path name of the document location (hostname is ignored). 
-        Useful to get a path of a local file.
         Returns None when no location is set.
         """
         if self.location is None:
             return None
         return urlparse(self.location).path
```

### Comparing `mmif-python-1.0.1/mmif/serialize/mmif.py` & `mmif-python-1.0.2/mmif/serialize/mmif.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 The :mod:`mmif` module contains the classes used to represent a full MMIF
 file as a live Python object.
 
 See the specification docs and the JSON Schema file for more information.
 """
 
 import json
+import warnings
+from collections import defaultdict
 from datetime import datetime
 from typing import List, Union, Optional, Dict, ClassVar, cast
 
 import jsonschema.validators
 
 import mmif
 from mmif import ThingTypesBase
@@ -64,19 +66,121 @@
         if isinstance(json_str, bytes):
             json_str = json_str.decode('utf8')
         schema = json.loads(mmif.get_mmif_json_schema())
         if isinstance(json_str, str):
             json_str = json.loads(json_str)
         jsonschema.validators.validate(json_str, schema)
 
-    def serialize(self, pretty: bool = False, sanitize: bool = False) -> str:
+    def serialize(self, pretty: bool = False, sanitize: bool = False, autogenerate_capital_annotations=True) -> str:
+        """
+        Serializes the MMIF object to a JSON string.
+
+        :param sanitize: If True, performs some sanitization of before returning 
+            the JSON string. See :meth:`sanitize` for details.
+        :param autogenerate_capital_annotations: If True, automatically convert 
+            any "pending" temporary properties from `Document` objects to 
+            `Annotation` objects. See :meth:`generate_capital_annotations` for 
+            details.
+        :param pretty: If True, returns string representation with indentation.
+        :return: JSON string of the MMIF object.
+        """
+        if autogenerate_capital_annotations:
+            self.generate_capital_annotations()
+        # sanitization should be done after `Annotation` annotations are generated
         if sanitize:
             self.sanitize()
         return super().serialize(pretty)
 
+    def _deserialize(self, input_dict: dict) -> None:
+        """
+        Deserializes the MMIF JSON string into a Mmif object.
+        This will read in existing ``Annotation`` typed annotations and 
+        attach the document-level properties to the ``Document`` objects, 
+        using a volatile property dict. This will allow apps to access the
+        document-level properties without having too much hassle to iterate
+        views and manually collect the properties.
+        """
+        super()._deserialize(input_dict)
+        for view in self.views:
+            doc_id = None
+            if AnnotationTypes.Annotation in view.metadata.contains:
+                if 'document' in view.metadata.contains[AnnotationTypes.Annotation]:
+                    doc_id = view.metadata.contains[AnnotationTypes.Annotation]['document']
+                # in a view, it is guaranteed that all Annotation objects are not duplicates
+                for ann in view.get_annotations(AnnotationTypes.Annotation):
+                    if doc_id is None:
+                        doc_id = ann.get_property('document')
+                    try:
+                        self.get_document_by_id(doc_id)._add_property_from_annotation(ann)
+                    except KeyError:
+                        warnings.warn(f"Annotation {ann.id} has a document ID {doc_id} that does not exist in the MMIF object. Skipping.", RuntimeWarning)
+
+    def generate_capital_annotations(self):
+        """
+        Automatically convert any "pending" temporary properties from 
+        `Document` objects to `Annotation` objects . The generated `Annotation` 
+        objects are then added to the last `View` in the views lists. 
+        
+        See https://github.com/clamsproject/mmif-python/issues/226 for rationale
+        behind this behavior and discussion.
+        """
+        # this view will be the default kitchen sink for all generated annotations
+        last_view = self.views.get_last()
+        # proceed only when there's at least one view
+        if last_view:
+            # to avoid duplicate property recording, this will be populated with
+            # existing Annotation objects from all existing views
+            existing_anns = defaultdict(lambda: defaultdict(dict))
+            
+            # new properties to record in the current serialization call
+            anns_to_write = defaultdict(dict)
+            for view in self.views:
+                doc_id = None
+                if AnnotationTypes.Annotation in view.metadata.contains:
+                    if 'document' in view.metadata.contains[AnnotationTypes.Annotation]:
+                        doc_id = view.metadata.contains[AnnotationTypes.Annotation]['document']
+                    for ann in view.get_annotations(AnnotationTypes.Annotation):
+                        if doc_id is None:
+                            doc_id = ann.get_property('document')
+                        existing_anns[doc_id].update(ann.properties)
+                for doc in view.get_documents():
+                    anns_to_write[doc.id].update(doc._props_temporary)
+            for doc in self.documents:
+                anns_to_write[doc.id].update(doc._props_temporary)
+            # additional iteration of views, to find a proper view to add the 
+            # generated annotations. If none found, use the last view as the kitchen sink
+            last_view_for_docs = defaultdict(lambda: last_view)
+            doc_ids = set(anns_to_write.keys())
+            for doc_id in doc_ids:
+                for view in reversed(self.views):
+                    # first try to find out if this view "contains" any annotation to the doc
+                    # then, check for individual annotations
+                    if [cont for cont in view.metadata.contains.values() if cont.get('document', None) == doc_id] \
+                            or list(view.get_annotations(document=doc_id)):
+                        last_view_for_docs[doc_id] = view
+                        break
+            for doc_id, found_props in anns_to_write.items():
+                # ignore the "empty" id property from temporary dict 
+                # `id` is "required" attribute for `AnnotationProperty` class 
+                # thus will always be present in `props` dict as a key with emtpy value
+                # also ignore duplicate k-v pairs
+                props = {}
+                for k, v in found_props.items():
+                    if k != 'id' and existing_anns[doc_id][k] != v:
+                        props[k] = v
+                if props:
+                    if len(anns_to_write) == 1:
+                        # if there's only one document, we can record the doc_id in the contains metadata
+                        last_view_for_docs[doc_id].metadata.new_contain(AnnotationTypes.Annotation, document=doc_id)
+                        props.pop('document', None)
+                    else:
+                        # otherwise, doc_id needs to be recorded in the annotation property
+                        props['document'] = doc_id
+                    last_view_for_docs[doc_id].new_annotation(AnnotationTypes.Annotation, **props)
+
     def sanitize(self):
         """
         Sanitizes a Mmif object by running some safeguards.
         Concretely, it performs the following before returning the JSON string.
         
         #. validating output using built-in MMIF jsonschema
         #. remove non-existing annotation types from ``contains`` metadata
@@ -191,17 +295,17 @@
         :param prop_key: the metadata key to search for
         :param prop_value: the metadata value to match
         :return: a list of documents matching the requested metadata key-value pair
         """
         docs = []
         for view in self.views:
             for doc in view.get_documents():
-                if prop_key in doc and doc.properties[prop_key] == prop_value:
+                if prop_key in doc and doc.get(prop_key) == prop_value:
                     docs.append(doc)
-        docs.extend([document for document in self.documents if document.properties[prop_key] == prop_value])
+        docs.extend([document for document in self.documents if document[prop_key] == prop_value])
         return docs
 
     def get_documents_locations(self, m_type: Union[DocumentTypes, str], path_only=False) -> List[Union[str, None]]:
         """
         This method returns the file paths of documents of given type.
         Only top-level documents have locations, so we only check them.
 
@@ -227,15 +331,15 @@
 
     def get_document_by_id(self, doc_id: str) -> Document:
         """
         Finds a Document object with the given ID.
 
         :param doc_id: the ID to search for
         :return: a reference to the corresponding document, if it exists
-        :raises Exception: if there is no corresponding document
+        :raises KeyError: if there is no corresponding document
         """
         if Mmif.id_delimiter in doc_id:
             vid, did = doc_id.split(Mmif.id_delimiter)
             view = self[vid]
             if isinstance(view, View):
                 return view.get_document_by_id(did) 
             else:
@@ -275,33 +379,33 @@
                 aligned_types = [ThingTypesBase.from_str(x) 
                                  for x in {contains_meta['sourceType'], contains_meta['targetType']}]
                 if len(aligned_types) == 2 and at_type1 in aligned_types and at_type2 in aligned_types:
                     alignments.extend(alignment_view.annotations)
             else:
                 for alignment in alignment_view.get_annotations(AnnotationTypes.Alignment):
                     aligned_types = set()
-                    for ann_id in [alignment.properties['target'], alignment.properties['source']]:
+                    for ann_id in [alignment['target'], alignment['source']]:
                         ann_id = cast(str, ann_id)
                         if Mmif.id_delimiter in ann_id:
                             view_id, ann_id = ann_id.split(Mmif.id_delimiter)
                             aligned_type = cast(Annotation, self[view_id][ann_id]).at_type
                         else:
                             aligned_type = cast(Annotation, alignment_view[ann_id]).at_type
                         aligned_types.add(aligned_type)
                     aligned_types = list(aligned_types)  # because membership check for sets also checks hash() values
                     if len(aligned_types) == 2 and at_type1 in aligned_types and at_type2 in aligned_types:
                         alignments.append(alignment)
             if len(alignments) > 0:
                 v_and_a[alignment_view.id] = alignments
         return v_and_a
 
-    def get_views_for_document(self, doc_id: str):
+    def get_views_for_document(self, doc_id: str) -> List[View]:
         """
         Returns the list of all views that have annotations anchored on a particular document.
-        Note that when the document is insids a view (generated during the pipeline's running),
+        Note that when the document is inside a view (generated during the pipeline's running),
         doc_id must be prefixed with the view_id.
         """
         views = []
         for view in self.views:
             annotations = view.get_annotations(document=doc_id)
             try:
                 next(annotations)
@@ -443,24 +547,28 @@
 
 class ViewsList(DataList[View]):
     """
     ViewsList object that implements :class:`mmif.serialize.model.DataList`
     for :class:`mmif.serialize.view.View`.
     """
     _items: Dict[str, View]
+    
+    def __init__(self, mmif_obj: Optional[Union[bytes, str, list]] = None):
+        super().__init__(mmif_obj)
 
     def _deserialize(self, input_list: list) -> None:  # pytype: disable=signature-mismatch
         """
         Extends base ``_deserialize`` method to initialize ``items`` as a dict from
         view IDs to :class:`mmif.serialize.view.View` objects.
 
         :param input_list: the JSON data that defines the list of views
         :return: None
         """
-        self._items = {item['id']: View(item) for item in input_list}
+        if input_list:
+            self._items = {item['id']: View(item) for item in input_list}
 
     def append(self, value: View, overwrite=False) -> None:
         """
         Appends a view to the list.
 
         Fails if there is already a view with the same ID
         in the list, unless ``overwrite`` is set to True.
@@ -471,7 +579,15 @@
                           existing view with the same ID
         :raises KeyError: if ``overwrite`` is set to False and
                           a view with the same ID exists
                           in the list
         :return: None
         """
         super()._append_with_key(value.id, value, overwrite)
+
+    def get_last(self) -> Optional[View]:
+        """
+        Returns the last view appended to the list.
+        """
+        for view in reversed(self._items.values()):
+            if 'error' not in view.metadata and 'warning' not in view.metadata:
+                return view
```

### Comparing `mmif-python-1.0.1/mmif/serialize/model.py` & `mmif-python-1.0.2/mmif/serialize/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,33 @@
 
 These objects are generally instantiated from JSON, either as a string
 or as an already-loaded Python dictionary. This base class provides the
 core functionality for deserializing MMIF JSON data into live objects
 and serializing live objects into MMIF JSON data. Specialized behavior
 for the different components of MMIF is added in the subclasses.
 """
-
 import json
 from datetime import datetime
+from types import MethodType
 from typing import Union, Any, Dict, Optional, TypeVar, Generic, Generator, Iterator, Type, Set
 
 from deepdiff import DeepDiff
 
+import mmif
+
 T = TypeVar('T')
 S = TypeVar('S')
+JSON_PRMTV_TYPES: Type = Union[str, int, float, bool, None]
 
 __all__ = [
     'MmifObject',
     'MmifObjectEncoder',
     'DataList',
-    'DataDict'
+    'DataDict',
+    'JSON_PRMTV_TYPES'
 ]
 
 
 class MmifObject(object):
     """
     Abstract superclass for MMIF related key-value pair objects.
 
@@ -73,14 +77,16 @@
     implementation.
 
     :param mmif_obj: JSON string or `dict` to initialize an object.
      If not given, an empty object will be initialized, sometimes with
      an ID value automatically generated, based on its parent object.
     """
     
+    # these are the reserved names that cannot be used as attribute names, and 
+    # they won't be serialized
     reserved_names: Set[str] = {
         'reserved_names',
         '_unnamed_attributes',
         '_attribute_classes',
         '_required_attributes',
         '_exclude_from_diff'
     }
@@ -95,14 +101,16 @@
             self._required_attributes = []
         if not hasattr(self, '_exclude_from_diff'):
             self._exclude_from_diff = set()
         if not hasattr(self, '_unnamed_attributes'):
             self._unnamed_attributes = {}
         if mmif_obj is not None:
             self.deserialize(mmif_obj)
+        for method in mmif.patches[self.__class__]:
+            setattr(self, method.__name__, MethodType(method, self))
 
     def disallow_additional_properties(self) -> None:
         """
         Call this method in :func:`__init__` to prevent the insertion
         of unnamed attributes after initialization.
         """
         self._unnamed_attributes = None
@@ -415,15 +423,15 @@
     def __iter__(self) -> Iterator[T]:
         return self._items.values().__iter__()
 
     def __len__(self) -> int:
         return self._items.__len__()
 
     def __reversed__(self) -> Iterator[T]:
-        return reversed(list(self._items.values()))
+        return reversed(self._items.values())
 
     def __contains__(self, item) -> bool:
         return item in self._items
 
     def empty(self):
         self._items = {}
 
@@ -436,17 +444,14 @@
         if mmif_obj is None:
             mmif_obj = {}
         super().__init__(mmif_obj)
 
     def _serialize(self, *args, **kwargs) -> dict:
         return super()._serialize(self._items)
 
-    def _deserialize(self, input_dict: dict) -> None:
-        raise NotImplementedError()
-
     def get(self, key: T, default=None) -> Optional[S]:
         return self._items.get(key, default)
 
     def _append_with_key(self, key: T, value: S, overwrite=False) -> None:
         if not overwrite and key in self._items:
             raise KeyError(f"Key {key} already exists")
         else:
```

### Comparing `mmif-python-1.0.1/mmif/serialize/view.py` & `mmif-python-1.0.2/mmif/serialize/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,15 @@
         self._attribute_classes = {
             'metadata': ViewMetadata,
             'annotations': AnnotationsList
         }
         self._required_attributes = ["id", "metadata", "annotations"]
         super().__init__(view_obj)
         for item in self.annotations:
-            if isinstance(item, Document):
-                item.parent = self.id
+            item.parent = self.id
 
     def new_contain(self, at_type: Union[str, ThingTypesBase], **contains_metadata) -> Optional['Contain']:
         """
         Adds a new element to the ``contains`` metadata.
 
         :param at_type: the ``@type`` of the annotation type being added
         :param contains_metadata: any metadata associated with the annotation type
@@ -112,14 +111,15 @@
         :param overwrite: if set to True, will overwrite an
                           existing annotation with the same ID
         :raises KeyError: if ``overwrite`` is set to False and
                           an annotation with the same ID exists
                           in the view
         :return: the same Annotation object passed in as ``annotation``
         """
+        annotation.parent = self.id
         self.annotations.append(annotation, overwrite)
         self.new_contain(annotation.at_type)
         return annotation
 
     def new_textdocument(self, text: str, lang: str = "en", did: Optional[str] = None, 
                          overwrite=False, **properties) -> 'Document':
         """
@@ -158,15 +158,14 @@
         Fails if there is already a document with the same ID in the annotations list.
 
         :param document: the Document object to add
         :param overwrite: if set to True, will overwrite
                           an existing view with the same ID
         :return: None
         """
-        document.parent = self.id
         return self.add_annotation(document, overwrite)
 
     def get_annotations(self, at_type: Optional[Union[str, ThingTypesBase]] = None, 
                         **properties) -> Generator[Annotation, None, None]:
         """
         Look for certain annotations in this view, specified by parameters
 
@@ -274,16 +273,19 @@
         :return: the generated :class:`Contain` object
         """
         if isinstance(at_type, str):
             at_type = ThingTypesBase.from_str(at_type)
             
         if at_type not in self.contains:
             new_contain = Contain(contains_metadata)
-            self.contains[at_type] = new_contain
+            self.add_contain(new_contain, at_type)
             return new_contain
+    
+    def add_contain(self, contain: 'Contain', at_type: Union[str, ThingTypesBase]):
+        self.contains[at_type] = contain
 
     def add_parameters(self, **runtime_params):
         self.parameters.update(dict(runtime_params))
 
     def add_parameter(self, param_key, param_value):
         self.parameters[param_key] = param_value
 
@@ -311,15 +313,15 @@
     """
     def __init__(self, error_obj: Optional[Union[bytes, str, dict]] = None) -> None:
         self.message: str = ''
         self.stackTrace: str = ''
         super().__init__(error_obj)
         
 
-class Contain(MmifObject):
+class Contain(DataDict[str, str]):
     """
     Contain object that represents the metadata of a single
     annotation type in the ``contains`` metadata of a MMIF view.
     """
 
 
 class AnnotationsList(DataList[Union[Annotation, Document]]):
```

### Comparing `mmif-python-1.0.1/mmif/vocabulary/annotation_types.py` & `mmif-python-1.0.2/mmif/vocabulary/annotation_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.1/mmif/vocabulary/base_types.py` & `mmif-python-1.0.2/mmif/vocabulary/base_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.1/mmif/vocabulary/document_types.py` & `mmif-python-1.0.2/mmif/vocabulary/document_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.1/mmif_python.egg-info/PKG-INFO` & `mmif-python-1.0.2/mmif_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-1.0.1/mmif_python.egg-info/SOURCES.txt` & `mmif-python-1.0.2/mmif_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.1/setup.py` & `mmif-python-1.0.2/setup.py`

 * *Files identical despite different names*

