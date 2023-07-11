# Comparing `tmp/pythogen-0.2.1.tar.gz` & `tmp/pythogen-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.2.1.tar", max compression
+gzip compressed data, was "pythogen-0.2.2.tar", max compression
```

## Comparing `pythogen-0.2.1.tar` & `pythogen-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-07-10 08:06:02.351284 pythogen-0.2.1/LICENSE
--rw-r--r--   0        0        0     2097 2023-07-10 08:06:02.351284 pythogen-0.2.1/README.md
--rw-r--r--   0        0        0     1567 2023-07-10 08:06:02.355284 pythogen-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1585 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/entrypoint.py
--rw-r--r--   0        0        0     7059 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/models.py
--rw-r--r--   0        0        0     2329 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3307 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/document.py
--rw-r--r--   0        0        0      576 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3239 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2132 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2437 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1074 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3512 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1810 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/response.py
--rw-r--r--   0        0        0    16508 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0     9844 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/renderer.py
--rw-r--r--   0        0        0      172 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/settings.py
--rw-r--r--   0        0        0     5149 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/templates/client/httpx-method.j2
--rw-r--r--   0        0        0     1668 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/templates/client/httpx-request-metrics.j2
--rw-r--r--   0        0        0    10825 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/templates/httpx.j2
--rw-r--r--   0        0        0       33 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/templates/init-py.j2
--rw-r--r--   0        0        0      312 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-11 12:27:36.792956 pythogen-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2097 2023-07-11 12:27:36.792956 pythogen-0.2.2/README.md
+-rw-r--r--   0        0        0     1567 2023-07-11 12:27:36.796956 pythogen-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1585 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/entrypoint.py
+-rw-r--r--   0        0        0     7474 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/models.py
+-rw-r--r--   0        0        0     2329 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3307 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      576 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3239 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2132 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2437 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1074 2023-07-11 12:27:36.796956 pythogen-0.2.2/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3512 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1810 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    16508 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0     9987 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/renderer.py
+-rw-r--r--   0        0        0      172 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/settings.py
+-rw-r--r--   0        0        0     5149 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/templates/client/httpx-method.j2
+-rw-r--r--   0        0        0     1668 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/templates/client/httpx-request-metrics.j2
+-rw-r--r--   0        0        0    11404 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/templates/httpx.j2
+-rw-r--r--   0        0        0       33 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/templates/init-py.j2
+-rw-r--r--   0        0        0      312 2023-07-11 12:27:36.800956 pythogen-0.2.2/pythogen/templates/pyproject-toml.j2
+-rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.2/PKG-INFO
```

### Comparing `pythogen-0.2.1/LICENSE` & `pythogen-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/README.md` & `pythogen-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pyproject.toml` & `pythogen-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.2.1"
+version = "0.2.2"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
```

### Comparing `pythogen-0.2.1/pythogen/entrypoint.py` & `pythogen-0.2.2/pythogen/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/models.py` & `pythogen-0.2.2/pythogen/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -256,29 +256,28 @@
     info: InfoObject
     paths: dict[str, PathItemObject]
     parameters: dict[str, ParameterObject]
     schemas: dict[str, SchemaObject]
 
     discriminator_base_class_schemas: list[DiscriminatorBaseClassSchema]
 
-    @property
-    def sorted_schemas(self) -> list[SchemaObject]:
+    def _build_sorted_schemas(self, keys):
         sorted: list[str] = []
-        keys = list(self.schemas.keys())
+        key_for_processing = set(keys)
         while keys:
             key = keys.pop()
             if key in sorted:
                 index = sorted.index(key)
             else:
                 sorted.append(key)
                 index = len(sorted) - 1
 
             schema = self.schemas[key]
             for property in schema.properties:
-                if property.schema.id in self.schemas and property.schema.id not in sorted:
+                if property.schema.id in key_for_processing and property.schema.id not in sorted:
                     sorted.insert(index, property.schema.id)
                 if property.schema.items:
                     if isinstance(property.schema.items, list):
                         for items in property.schema.items:
                             if items.id in self.schemas:
                                 sorted.insert(index, items.id)
                     elif property.schema.items.id in self.schemas:
@@ -286,12 +285,22 @@
 
         sorted_schemas = []
         for key in sorted:
             if self.schemas[key] not in sorted_schemas:
                 sorted_schemas.append(self.schemas[key])
         return sorted_schemas
 
+    @property
+    def sorted_schemas(self) -> list[SchemaObject]:
+        schema_keys = list(filter(lambda x: self.schemas[x].enum is None, self.schemas.keys()))
+        return self._build_sorted_schemas(schema_keys)
+
+    @property
+    def sorted_enums(self) -> list[SchemaObject]:
+        enum_keys = list(filter(lambda x: self.schemas[x].enum is not None, self.schemas.keys()))
+        return self._build_sorted_schemas(enum_keys)
+
 
 @dataclass
 class DiscriminatorBaseClassSchema:
     name: str
     attr: str
```

### Comparing `pythogen-0.2.1/pythogen/packager.py` & `pythogen-0.2.2/pythogen/packager.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/parsers/document.py` & `pythogen-0.2.2/pythogen/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.2.2/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/parsers/operations.py` & `pythogen-0.2.2/pythogen/parsers/operations.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/parsers/parameters.py` & `pythogen-0.2.2/pythogen/parsers/parameters.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/parsers/paths.py` & `pythogen-0.2.2/pythogen/parsers/paths.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/parsers/references.py` & `pythogen-0.2.2/pythogen/parsers/references.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/parsers/request_body.py` & `pythogen-0.2.2/pythogen/parsers/request_body.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/parsers/response.py` & `pythogen-0.2.2/pythogen/parsers/response.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/parsers/schemas.py` & `pythogen-0.2.2/pythogen/parsers/schemas.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/renderer.py` & `pythogen-0.2.2/pythogen/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
     prepared_operations = prepare_operations(document)
 
     rendered_client = template.render(
         document=document,
         name=name,
         version=document.info.version,
+        enums=document.sorted_enums,
         models=document.sorted_schemas,
         get=prepared_operations.get,
         post=prepared_operations.post,
         patch=prepared_operations.patch,
         post_no_body=prepared_operations.post_no_body,
         put=prepared_operations.put,
         delete_no_body=prepared_operations.delete_no_body,
@@ -233,16 +234,18 @@
     # TODO: всегда передавать document в функцию
     if document:
         schema = document.schemas.get(schema.id, schema)
 
     representation = 'dict'
 
     if schema.type in primitive_type_mapping:
-        if schema.enum:
+        if schema.enum and schema.id == '<inline+SchemaObject>':
             representation = f'Literal{schema.enum}'
+        elif schema.enum:
+            representation = schema.id
         elif schema.format in format_mapping:
             representation = format_mapping[schema.format]  # type: ignore
         else:
             representation = primitive_type_mapping[schema.type]
 
     elif schema.type == models.Type.object and schema.id != '<inline+SchemaObject>':
         representation = classname(schema.id)
```

### Comparing `pythogen-0.2.1/pythogen/templates/client/httpx-method.j2` & `pythogen-0.2.2/pythogen/templates/client/httpx-method.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/templates/client/httpx-request-metrics.j2` & `pythogen-0.2.2/pythogen/templates/client/httpx-request-metrics.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.1/pythogen/templates/httpx.j2` & `pythogen-0.2.2/pythogen/templates/httpx.j2`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 from __future__ import annotations
 
 import abc
 from dataclasses import dataclass
 
 import datetime
 
+from enum import Enum
+from enum import IntEnum
+
 from httpx import Timeout
 from typing import Literal
 
 from typing import Any
 
 from typing import Union
 from typing import Callable
@@ -167,14 +170,37 @@
 ]
 
 
 class RequiredHeaders(Exception):
     ...
 
 
+{%- for enum_class in enums %}
+{%- if enum_class.type.value == "integer"  %}
+class {{ classname(enum_class.id) }}(IntEnum):
+    """
+    {{ enum_class.title }}
+    """
+    {%- for val in enum_class.enum %}
+    _{{ val }} = {{ val }}
+    {%- endfor %}
+{%- else %}
+class {{ classname(enum_class.id) }}(str, Enum):
+    """
+    {{ enum_class.title }}
+    """
+    {%- for val in enum_class.enum %}
+    {{ val.upper() }} = "{{ val }}"
+    {%- endfor %}
+
+    def __str__(self) -> Any:
+        return self.value
+{%- endif %}
+{%- endfor %}
+
 class EmptyBody(BaseModel):
     status_code: int
     text: str
 
 {% for schema in discriminator_base_class_schemas %}
 class {{ schema.name }}(BaseModel):
     {{ schema.attr }}: str
```

### Comparing `pythogen-0.2.1/PKG-INFO` & `pythogen-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythogen
-Version: 0.2.1
+Version: 0.2.2
 Summary: Generator of python HTTP-clients from OpenApi specification.
 Home-page: https://github.com/artsmolin/pythogen
 License: MIT
 Keywords: openapi,openapi-generator,swagger,http-client,generator
 Author: Artur Smolin
 Author-email: artursmolin@outlook.com
 Requires-Python: >=3.10,<4.0
```

