# Comparing `tmp/ptal_api-0.12.2.tar.gz` & `tmp/ptal_api-0.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.12.2.tar", max compression
+gzip compressed data, was "ptal_api-0.12.3.tar", max compression
```

## Comparing `ptal_api-0.12.2.tar` & `ptal_api-0.12.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      627 2023-06-27 08:38:38.936916 ptal_api-0.12.2/README.md
--rw-r--r--   0        0        0        0 2023-06-27 08:38:38.992917 ptal_api-0.12.2/ptal_api/__init__.py
--rw-r--r--   0        0        0   120656 2023-06-27 08:38:38.936916 ptal_api-0.12.2/ptal_api/adapter.py
--rw-r--r--   0        0        0      184 2023-06-27 08:38:38.936916 ptal_api-0.12.2/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-06-27 08:38:38.936916 ptal_api-0.12.2/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      484 2023-06-27 08:38:38.936916 ptal_api-0.12.2/ptal_api/core/query_factory.py
--rw-r--r--   0        0        0      435 2023-06-27 08:38:38.936916 ptal_api-0.12.2/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      737 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    14955 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      904 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3255 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2194 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1464 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4556 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    23314 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1800 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3571 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0      295 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/common.py
--rw-r--r--   0        0        0     1880 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/object_types.py
--rw-r--r--   0        0        0     2884 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/objects.py
--rw-r--r--   0        0        0     3716 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/pretty_adapter.py
--rw-r--r--   0        0        0      595 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/property_values.py
--rw-r--r--   0        0        0    16486 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/transformer.py
--rw-r--r--   0        0        0        0 2023-06-27 08:38:38.996917 ptal_api-0.12.2/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     4668 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1282 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-06-27 08:38:38.996917 ptal_api-0.12.2/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   290589 2023-06-27 08:38:38.944916 ptal_api-0.12.2/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    96961 2023-06-27 08:38:38.944916 ptal_api-0.12.2/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    74033 2023-06-27 08:38:38.944916 ptal_api-0.12.2/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   137221 2023-06-27 08:38:38.948916 ptal_api-0.12.2/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3662 2023-06-27 08:38:38.948916 ptal_api-0.12.2/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-06-27 08:38:38.996917 ptal_api-0.12.2/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-27 08:38:38.948916 ptal_api-0.12.2/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1871 2023-06-27 08:38:38.948916 ptal_api-0.12.2/pyproject.toml
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 ptal_api-0.12.2/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-07-11 09:36:41.189674 ptal_api-0.12.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 09:36:41.269676 ptal_api-0.12.3/ptal_api/__init__.py
+-rw-r--r--   0        0        0   119338 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/adapter.py
+-rw-r--r--   0        0        0      184 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      484 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/query_factory.py
+-rw-r--r--   0        0        0      435 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      737 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    14955 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      904 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3255 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2194 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1464 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4556 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    23314 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1800 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      192 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     3571 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0      295 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/common.py
+-rw-r--r--   0        0        0     1880 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/object_types.py
+-rw-r--r--   0        0        0     2884 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/objects.py
+-rw-r--r--   0        0        0     3716 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/pretty_adapter.py
+-rw-r--r--   0        0        0      595 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/property_values.py
+-rw-r--r--   0        0        0    16486 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/pretty_adapter/transformer.py
+-rw-r--r--   0        0        0        0 2023-07-11 09:36:41.273676 ptal_api-0.12.3/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1282 2023-07-11 09:36:41.193674 ptal_api-0.12.3/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 09:36:41.273676 ptal_api-0.12.3/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   289388 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    99292 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   135630 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3662 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-07-11 09:36:41.273676 ptal_api-0.12.3/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-11 09:36:41.197674 ptal_api-0.12.3/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1889 2023-07-11 09:36:41.197674 ptal_api-0.12.3/pyproject.toml
+-rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 ptal_api-0.12.3/PKG-INFO
```

### Comparing `ptal_api-0.12.2/README.md` & `ptal_api-0.12.3/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/adapter.py` & `ptal_api-0.12.3/ptal_api/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 from copy import copy
 from functools import wraps
 from time import time
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Union
 
+import graphql
 from deprecation import deprecated
 from sgqlc.operation import Fragment
 
 from .core.kb_sync.kb_iterator_config import KBIteratorConfig
 from .core.kb_sync.object_time_interval import ObjectTimeInterval
 from .core.query_factory import make_operation
 from .core.type_mapper.data_model.base_data_model import TypeMapping
@@ -481,14 +482,18 @@
         return value_input
 
     def _configure_pipeline_topic_fields(self, kafka_topic: tc.KafkaTopic):
         kafka_topic.__fields__(*self.pipeline_topic_fields)
         kafka_topic.metrics().__fields__(*self.pipeline_metrics_fields)
         kafka_topic.pipeline().pipeline_config().__fields__(*self.pipeline_config_fields)
 
+    def raw_execute(self, query: str, variables: Optional[dict] = None):
+        graphql.parse(query)
+        return self._gql_client.execute(query=query, variables=variables)
+
     # @prettify
     def get_all_documents(
         self,
         grouping: DocumentGrouping = "none",
         filter_settings: Optional[DocumentFilterSettings] = None,
         direction: SortDirection = "descending",
         sort_field: DocumentSorting = "score",
@@ -1401,110 +1406,65 @@
         ucpvt.__fields__(*self.cpvt_fields_truncated)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_property_value_type
 
     @prettify
+    @deprecated(details="Use update_concept_property method instead")
     def update_concept_string_property(self, cp: ConceptProperty) -> Union[ConceptProperty, objects.Property]:
-        op = make_operation(Mutation, "update_concept_string_property")
-        ucp: ConceptProperty = op.update_concept_property(
-            form=ConceptPropertyUpdateInput(
-                property_id=cp.id,
-                is_main=cp.is_main,
-                access_level_id=cp.access_level.id,
-                value_input=[
-                    ComponentValueInput(value=ValueInput(string_value_input=StringValueInput(value=cp.value.value)))
-                ],
-            )
-        )
-        self._configure_output_properties_fields(ucp)
-        res = self._gql_client.execute(op)
-        res = op + res
-
-        return res.update_concept_property
+        return self.update_concept_property(cp)
 
     @prettify
+    @deprecated(details="Use update_concept_property method instead")
     def update_concept_int_property(self, cp: ConceptProperty) -> Union[ConceptProperty, objects.Property]:
-        op = make_operation(Mutation, "update_concept_int_property")
-        ucp: ConceptProperty = op.update_concept_property(
-            form=ConceptPropertyUpdateInput(
-                property_id=cp.id,
-                is_main=cp.is_main,
-                access_level_id=cp.access_level.id,
-                value_input=[
-                    ComponentValueInput(value=ValueInput(int_value_input=IntValueInput(value=cp.value.number)))
-                ],
+        return self.update_concept_property(cp)
+
+    def _get_value_input_by_value(self, value: Any, named_value_id: Optional[str] = None) -> ComponentValueInput:
+        if isinstance(value, (StringValue, uas.StringValue)):
+            value_input = ComponentValueInput(value=ValueInput(string_value_input=StringValueInput(value=value.value)))
+        elif isinstance(value, (IntValue, uas.IntValue)):
+            value_input = ComponentValueInput(value=ValueInput(int_value_input=IntValueInput(value=value.number)))
+        elif isinstance(value, (DateTimeValue, uas.DateTimeValue)):
+            value_input = ComponentValueInput(
+                value=ValueInput(date_time_value_input=DateTimeValueInput(date=value.date, time=value.time))
             )
-        )
-        self._configure_output_properties_fields(ucp)
-        res = self._gql_client.execute(op)
-        res = op + res
+        elif isinstance(value, (StringLocaleValue, uas.StringLocaleValue)):
+            value_input = ComponentValueInput(
+                value=ValueInput(
+                    string_locale_value_input=StringLocaleValueInput(value=value.value, locale=value.locale)
+                )
+            )
+        elif isinstance(value, (LinkValue, uas.LinkValue)):
+            value_input = ComponentValueInput(value=ValueInput(link_value_input=LinkValueInput(link=value.link)))
+        elif isinstance(value, (DoubleValue, uas.DoubleValue)):
+            value_input = ComponentValueInput(
+                value=ValueInput(double_value_input=DoubleValueInput(double=value.double))
+            )
+        else:
+            raise NotImplementedError(f"{type(value)} type is not supported")
 
-        return res.update_concept_property
+        if named_value_id:
+            value_input.id = named_value_id
+        return value_input
 
     @prettify
-    def update_concept_composite_property(self, cp: ConceptProperty) -> Union[ConceptProperty, objects.Property]:
-        op = make_operation(Mutation, "update_concept_composite_property")
+    def update_concept_property(self, cp: ConceptProperty) -> Union[ConceptProperty, objects.Property]:
         value_input = []
-        for value in cp.value.list_value:
-            if isinstance(value.value, (StringValue, uas.StringValue)):
-                value_input.append(
-                    ComponentValueInput(
-                        id=value.id, value=ValueInput(string_value_input=StringValueInput(value=value.value.value))
-                    )
-                )
-            elif isinstance(value.value, (IntValue, uas.IntValue)):
-                value_input.append(
-                    ComponentValueInput(
-                        id=value.id, value=ValueInput(int_value_input=IntValueInput(value=value.value.number))
-                    )
-                )
-            elif isinstance(value.value, (DateTimeValue, uas.DateTimeValue)):
-                value_input.append(
-                    ComponentValueInput(
-                        id=value.id,
-                        value=ValueInput(
-                            date_time_value_input=DateTimeValueInput(date=value.value.date, time=value.value.time)
-                        ),
-                    )
-                )
-            elif isinstance(value.value, (StringLocaleValue, uas.StringLocaleValue)):
-                value_input.append(
-                    ComponentValueInput(
-                        id=value.id,
-                        value=ValueInput(
-                            string_locale_value_input=StringLocaleValueInput(
-                                value=value.value.value, locale=value.value.locale
-                            )
-                        ),
-                    )
-                )
-            elif isinstance(value.value, (LinkValue, uas.LinkValue)):
-                value_input.append(
-                    ComponentValueInput(
-                        id=value.id, value=ValueInput(link_value_input=LinkValueInput(link=value.value.link))
-                    )
-                )
-            elif isinstance(value.value, (DoubleValue, uas.DoubleValue)):
-                value_input.append(
-                    ComponentValueInput(
-                        id=value.id, value=ValueInput(double_value_input=DoubleValueInput(double=value.value.double))
-                    )
-                )
-        ucp: ConceptProperty = op.update_concept_property(
-            form=ConceptPropertyUpdateInput(
-                property_id=cp.id, is_main=cp.is_main, access_level_id=cp.access_level.id, value_input=value_input
-            )
-        )
-        self._configure_output_properties_fields(ucp)
-        res = self._gql_client.execute(op)
-        res = op + res
+        if hasattr(cp.value, "list_value"):
+            for value in cp.value.list_value:
+                value_input.append(self._get_value_input_by_value(value.value, value.id))
+        else:
+            value_input.append(self._get_value_input_by_value(cp.value))
+        return self._update_concept_property_with_input(cp.id, cp.is_main, value_input, cp.access_level.id)
 
-        return res.update_concept_property
+    @prettify
+    @deprecated(details="Use update_concept_property method instead")
+    def update_concept_composite_property(self, cp: ConceptProperty) -> Union[ConceptProperty, objects.Property]:
+        return self.update_concept_property(cp)
 
     def _update_concept_property_with_input(
         self,
         property_id: str,
         is_main: bool,
         value_input: List[ComponentValueInput],
         access_level_id: str,
```

### Comparing `ptal_api-0.12.2/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.12.3/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.12.3/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.12.3/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.12.3/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.12.3/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.12.3/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.12.3/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.12.3/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/core/values/value_mapping.py` & `ptal_api-0.12.3/ptal_api/core/values/value_mapping.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/pretty_adapter/object_types.py` & `ptal_api-0.12.3/ptal_api/pretty_adapter/object_types.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/pretty_adapter/objects.py` & `ptal_api-0.12.3/ptal_api/pretty_adapter/objects.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/pretty_adapter/pretty_adapter.py` & `ptal_api-0.12.3/ptal_api/pretty_adapter/pretty_adapter.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/pretty_adapter/property_values.py` & `ptal_api-0.12.3/ptal_api/pretty_adapter/property_values.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/pretty_adapter/transformer.py` & `ptal_api-0.12.3/ptal_api/pretty_adapter/transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/providers/gql_providers.py` & `ptal_api-0.12.3/ptal_api/providers/gql_providers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 import time
 from contextlib import AbstractContextManager
 from typing import Optional
 
+from jwt import decode
 from keycloak import KeycloakOpenID
 from sgqlc.endpoint.http import BaseEndpoint, HTTPEndpoint
 
 logger = logging.getLogger(__name__)
 
 
 def _configure_gql_client(
-    uri: str, timeout: float = None, _retries: int = 0, auth_token: Optional[str] = None
+    uri: str, timeout: Optional[float] = None, _retries: int = 0, auth_token: Optional[str] = None
 ) -> HTTPEndpoint:
     headers = {"X-Auth-Token": auth_token, "Authorization": f"Bearer {auth_token}"} if auth_token is not None else None
     return HTTPEndpoint(uri, headers, timeout=timeout)
 
 
 class AbstractGQLClient(AbstractContextManager):
     def __init__(self, gql_uri: str, timeout: float, retries: int, retry_timeout: float) -> None:
@@ -61,48 +62,125 @@
         gql_uri: str,
         timeout: float,
         retries: int,
         auth_url: str,
         realm: str,
         client_id: str,
         client_secret: str,
-        user: str,
-        pwd: str,
+        user: Optional[str] = None,
+        pwd: Optional[str] = None,
         retry_timeout: float = 1,
+        access_token: Optional[str] = None,
+        refresh_token: Optional[str] = None,
     ) -> None:
+        """
+        Do not use basic constructor. Use create_with_user_pwd and create_with_token instead.
+
+        Must be provided at least one of user and password or refresh token
+        """
+
+        if not (user and pwd or refresh_token):
+            raise ValueError(
+                "Authorization variables values are not set. "
+                "Must be provided at least one of login and password or refresh token"
+            )
+        if any(env is None for env in (auth_url, realm, client_id, client_secret)):
+            raise ValueError("Authorization variables values are not set")
+
         super().__init__(gql_uri, timeout, retries, retry_timeout)
 
         self._auth_url = auth_url
         self._realm = realm
         self._client_id = client_id
         self._client_secret = client_secret
-        self._user = user
-        self._pwd = pwd
-
-        if any(
-            env is None
-            for env in [self._auth_url, self._realm, self._client_id, self._client_secret, self._user, self._pwd]
-        ):
-            raise ValueError("Authorization variables values are not set")
 
         self._keycloak_openid: Optional[KeycloakOpenID] = None
-        self._access_token: Optional[str] = None
-        self._refresh_token: Optional[str] = None
+
+        self._user: Optional[str] = user
+        self._pwd: Optional[str] = pwd
+        self._access_token: Optional[str] = access_token
+        self._refresh_token: Optional[str] = refresh_token
         self._access_expiration_timestamp: Optional[float] = None
         self._refresh_expiration_timestamp: Optional[float] = None
 
+        if access_token:
+            self._access_expiration_timestamp = decode(access_token, options={"verify_signature": False})["exp"]
+            self._gql_client = _configure_gql_client(self._gql_uri, self._timeout, self._retries, self._access_token)
+        if refresh_token:
+            self._refresh_expiration_timestamp = decode(refresh_token, options={"verify_signature": False})["exp"]
+        elif not user:
+            raise ValueError("Authorization variables values are not set")
+
+    @classmethod
+    def create_with_user_pwd(
+        cls,
+        gql_uri: str,
+        timeout: float,
+        retries: int,
+        auth_url: str,
+        realm: str,
+        client_id: str,
+        client_secret: str,
+        user: str,
+        pwd: str,
+        retry_timeout: float = 1,
+    ) -> "KeycloakAwareGQLClient":
+        return KeycloakAwareGQLClient(
+            gql_uri=gql_uri,
+            timeout=timeout,
+            retries=retries,
+            auth_url=auth_url,
+            realm=realm,
+            client_id=client_id,
+            client_secret=client_secret,
+            user=user,
+            pwd=pwd,
+            retry_timeout=retry_timeout,
+        )
+
+    @classmethod
+    def create_with_token(
+        cls,
+        gql_uri: str,
+        timeout: float,
+        retries: int,
+        auth_url: str,
+        realm: str,
+        client_id: str,
+        client_secret: str,
+        refresh_token: str,
+        access_token: Optional[str] = None,
+        retry_timeout: float = 1,
+    ) -> "KeycloakAwareGQLClient":
+        return KeycloakAwareGQLClient(
+            gql_uri=gql_uri,
+            timeout=timeout,
+            retries=retries,
+            auth_url=auth_url,
+            realm=realm,
+            client_id=client_id,
+            client_secret=client_secret,
+            refresh_token=refresh_token,
+            access_token=access_token,
+            retry_timeout=retry_timeout,
+        )
+
     def _ensure_session_liveness(self):
         offsetted_time = time.time() + self._TIME_OFFSET
         if self._access_expiration_timestamp is not None and offsetted_time < self._access_expiration_timestamp:
             return
 
         time_before_req = time.time()
-        # if self._refresh_expiration_timestamp is not None and offsetted_time < self._refresh_expiration_timestamp:
-        logger.info("refreshing access token with credentials")
-        token_info = self._keycloak_openid.token(self._user, self._pwd)
+
+        if self._refresh_expiration_timestamp is not None and offsetted_time < self._refresh_expiration_timestamp:
+            logger.info("refreshing access token with refresh token")
+            token_info = self._keycloak_openid.refresh_token(self._refresh_token)
+        else:
+            logger.info("refreshing access token with credentials")
+            token_info = self._keycloak_openid.token(self._user, self._pwd)
 
         self._access_token = token_info["access_token"]
         self._access_expiration_timestamp = time_before_req + token_info["expires_in"]
         self._refresh_token = token_info["refresh_token"]
         self._refresh_expiration_timestamp = time_before_req + token_info["refresh_expires_in"]
 
         self._gql_client = _configure_gql_client(self._gql_uri, self._timeout, self._retries, self._access_token)
```

### Comparing `ptal_api-0.12.2/ptal_api/schema/README.md` & `ptal_api-0.12.3/ptal_api/schema/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/schema/api_schema.py` & `ptal_api-0.12.3/ptal_api/schema/api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,19 +156,14 @@
 
 
 class DocumentGrouping(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('none', 'story')
 
 
-class DocumentRecall(sgqlc.types.Enum):
-    __schema__ = api_schema
-    __choices__ = ('high', 'low', 'medium', 'none')
-
-
 class DocumentSorting(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('countChildDocs', 'countConcepts', 'countDisambiguatedEntities', 'countEntities', 'countEvents', 'countLinks', 'countNamedEntities', 'countObjects', 'countPropertyCandidates', 'countResearchMaps', 'countTasks', 'id', 'publicationDate', 'registrationDate', 'relevance', 'score', 'secretLevel', 'text', 'title', 'trustLevel', 'updateDate')
 
 
 class DocumentSourceType(sgqlc.types.Enum):
     __schema__ = api_schema
@@ -1824,22 +1819,16 @@
     list_account = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Account'))), graphql_name='listAccount')
     total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='total')
     total_platforms = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='totalPlatforms')
 
 
 class AccountStatistics(sgqlc.types.Type):
     __schema__ = api_schema
-    __field_names__ = ('count_doc', 'count_doc_today', 'count_doc_week', 'count_doc_month', 'recall_doc_today', 'recall_doc_week', 'recall_doc_month')
+    __field_names__ = ('count_doc',)
     count_doc = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDoc')
-    count_doc_today = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocToday')
-    count_doc_week = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocWeek')
-    count_doc_month = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocMonth')
-    recall_doc_today = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocToday')
-    recall_doc_week = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocWeek')
-    recall_doc_month = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocMonth')
 
 
 class Annotation(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('start', 'end', 'value')
     start = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='start')
     end = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='end')
@@ -3256,28 +3245,22 @@
     __field_names__ = ('list_platform', 'total')
     list_platform = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Platform'))), graphql_name='listPlatform')
     total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='total')
 
 
 class PlatformStatistics(sgqlc.types.Type):
     __schema__ = api_schema
-    __field_names__ = ('count_account', 'count_doc', 'count_doc_today', 'count_doc_week', 'count_doc_month', 'recall_doc_today', 'recall_doc_week', 'recall_doc_month')
+    __field_names__ = ('count_account', 'count_doc')
     count_account = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countAccount')
     count_doc = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDoc')
-    count_doc_today = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocToday')
-    count_doc_week = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocWeek')
-    count_doc_month = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocMonth')
-    recall_doc_today = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocToday')
-    recall_doc_week = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocWeek')
-    recall_doc_month = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocMonth')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = api_schema
-    __field_names__ = ('document', 'story', 'pagination_story', 'pagination_document_markers', 'concept_type', 'composite_concept_type', 'pagination_composite_concept_type', 'concept_property_type', 'concept_link_type', 'concept_property_value_type', 'list_concept_type', 'list_user_menu_type', 'list_concept_property_type', 'list_concept_property_type_by_id', 'list_concept_link_type', 'list_concept_property_value_type', 'pagination_concept_type', 'pagination_concept_property_type', 'pagination_concept_link_property_type', 'pagination_concept_link_type', 'pagination_concept_property_value_type', 'composite_concept_property_type', 'composite_link_property_type', 'list_composite_concept_property_type', 'list_composite_link_property_type', 'pagination_composite_concept_property_type', 'pagination_composite_link_property_type', 'composite_property_value_template', 'list_composite_property_value_template', 'pagination_composite_property_value_template', 'concept_type_view', 'domain_map', 'concept', 'list_concept_by_id', 'pagination_concept', 'composite_concept', 'pagination_composite_concept', 'list_concept_link_between_fixed_concepts', 'concept_property', 'concept_link', 'pagination_concept_link', 'pagination_kbrelated_document', 'issue', 'pagination_issue', 'pagination_issue_change', 'research_map', 'pagination_research_map', 'active_research_map', 'list_top_neighbors_on_map', 'list_last_research_map', 'document_autocomplete', 'concept_autocomplete', 'get_osm_place_name', 'get_osm_coordinates', 'get_redmine_issue_creation_default_parameters', 'get_redmine_issue_update_default_description', 'search_similar_redmine_issues', 'access_level', 'pagination_access_level', 'story_fs2_query', 'concept_fs2_query', 'markers_bulk', 'platform', 'list_platform_by_id', 'pagination_platform', 'account', 'list_account_by_id', 'pagination_account', 'pagination_country', 'pagination_language', 'document_feed', 'pagination_document_feed', 'concept_registry_view', 'document_registry_view', 'document_card_view', 'chart', 'preview_chart')
+    __field_names__ = ('document', 'story', 'pagination_story', 'pagination_document_markers', 'concept_type', 'composite_concept_type', 'pagination_composite_concept_type', 'concept_property_type', 'concept_link_type', 'concept_property_value_type', 'list_concept_type', 'list_user_menu_type', 'list_concept_property_type', 'list_concept_property_type_by_id', 'list_concept_link_type', 'list_concept_property_value_type', 'pagination_concept_type', 'pagination_concept_property_type', 'pagination_concept_link_property_type', 'pagination_concept_link_type', 'pagination_concept_property_value_type', 'composite_concept_property_type', 'composite_link_property_type', 'list_composite_concept_property_type', 'list_composite_link_property_type', 'pagination_composite_concept_property_type', 'pagination_composite_link_property_type', 'composite_property_value_template', 'list_composite_property_value_template', 'pagination_composite_property_value_template', 'concept_type_view', 'domain_map', 'concept', 'list_concept_by_id', 'pagination_concept', 'composite_concept', 'pagination_composite_concept', 'list_concept_link_between_fixed_concepts', 'concept_property', 'concept_link', 'pagination_concept_link', 'pagination_kbrelated_document', 'issue', 'pagination_issue', 'pagination_issue_change', 'research_map', 'pagination_research_map', 'active_research_map', 'list_top_neighbors_on_map', 'list_last_research_map', 'document_autocomplete', 'concept_autocomplete', 'get_osm_place_name', 'get_osm_coordinates', 'get_redmine_issue_creation_default_parameters', 'get_redmine_issue_update_default_description', 'search_similar_redmine_issues', 'access_level', 'pagination_access_level', 'story_fs2_query', 'concept_fs2_query', 'markers_bulk', 'platform', 'list_platform_by_id', 'pagination_platform', 'account', 'list_account_by_id', 'pagination_account', 'pagination_country', 'pagination_language', 'document_feed', 'pagination_document_feed', 'concept_registry_view', 'document_registry_view', 'document_card_view', 'chart', 'preview_chart', 'zklast_sync')
     document = sgqlc.types.Field('Document', graphql_name='document', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     story = sgqlc.types.Field('Story', graphql_name='story', args=sgqlc.types.ArgDict((
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
 ))
@@ -3633,14 +3616,15 @@
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     preview_chart = sgqlc.types.Field(sgqlc.types.non_null(Chart), graphql_name='previewChart', args=sgqlc.types.ArgDict((
         ('form', sgqlc.types.Arg(sgqlc.types.non_null(ChartDescriptionInput), graphql_name='form', default=None)),
 ))
     )
+    zklast_sync = sgqlc.types.Field('ZKLastSync', graphql_name='ZKLastSync')
 
 
 class RedmineIssue(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('id', 'subject', 'tracker', 'status', 'priority', 'author', 'assignee', 'creation_date')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     subject = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='subject')
@@ -3853,14 +3837,21 @@
 
 class User(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('id',)
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
 
 
+class ZKLastSync(sgqlc.types.Type):
+    __schema__ = api_schema
+    __field_names__ = ('zip_name', 'sync_date')
+    zip_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='zipName')
+    sync_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='syncDate')
+
+
 class Account(sgqlc.types.Type, RecordInterface):
     __schema__ = api_schema
     __field_names__ = ('id', 'name', 'url', 'country', 'markers', 'params', 'platform', 'image', 'metric', 'period')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     url = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='url')
     country = sgqlc.types.Field(String, graphql_name='country')
```

### Comparing `ptal_api-0.12.2/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.12.3/ptal_api/schema/crawlers_api_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 class JobRunningSort(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('args', 'crawlerName', 'creator', 'id', 'jobPriority', 'periodicJobId', 'projectName', 'settings', 'startTime', 'systemRegistrationDate')
 
 
 class JobStatus(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
-    __choices__ = ('Finished', 'Pending', 'Running')
+    __choices__ = ('Finished', 'Paused', 'Pending', 'Running')
 
 
 class LogLevel(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('Critical', 'Debug', 'Error', 'Info', 'Trace', 'Warning')
 
 
@@ -122,15 +122,15 @@
 class MonitoringStatus(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('Critical', 'Ok', 'Pending', 'SameItemsJob', 'SameItemsPeriodic', 'ZeroItemsZeroDuplicates')
 
 
 class PeriodicJobSorting(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
-    __choices__ = ('crawlerId', 'crawlerName', 'creator', 'id', 'lastUpdater', 'name', 'nextScheduleTime', 'priority', 'projectId', 'projectName', 'status', 'systemRegistrationDate', 'systemUpdateDate')
+    __choices__ = ('crawlerId', 'crawlerName', 'creator', 'credentialId', 'id', 'lastUpdater', 'name', 'nextScheduleTime', 'priority', 'projectId', 'projectName', 'status', 'systemRegistrationDate', 'systemUpdateDate')
 
 
 class PeriodicJobStatus(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('Disabled', 'Enabled')
 
 
@@ -318,17 +318,18 @@
     is_retrospective = sgqlc.types.Field(Boolean, graphql_name='isRetrospective')
     retrospective_interval = sgqlc.types.Field('TimestampInterval', graphql_name='retrospectiveInterval')
     actual_status = sgqlc.types.Field(InformationSourceLoaderActualStatus, graphql_name='actualStatus')
 
 
 class JobInput(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('crawler_id', 'version_id', 'priority', 'message_priority', 'is_noise', 'research_map_id', 'settings', 'args')
+    __field_names__ = ('crawler_id', 'version_id', 'credential_id', 'priority', 'message_priority', 'is_noise', 'research_map_id', 'settings', 'args')
     crawler_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='crawlerId')
     version_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='versionId')
+    credential_id = sgqlc.types.Field(ID, graphql_name='credentialId')
     priority = sgqlc.types.Field(sgqlc.types.non_null(JobPriorityType), graphql_name='priority')
     message_priority = sgqlc.types.Field(MessagePriority, graphql_name='messagePriority')
     is_noise = sgqlc.types.Field(Boolean, graphql_name='isNoise')
     research_map_id = sgqlc.types.Field(ID, graphql_name='researchMapId')
     settings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('KeyValueInputType'))), graphql_name='settings')
     args = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('KeyValueInputType'))), graphql_name='args')
 
@@ -422,19 +423,20 @@
     system_registration_date = sgqlc.types.Field('TimestampInterval', graphql_name='systemRegistrationDate')
     system_update_date = sgqlc.types.Field('TimestampInterval', graphql_name='systemUpdateDate')
     next_schedule_time = sgqlc.types.Field('TimestampInterval', graphql_name='nextScheduleTime')
 
 
 class PeriodicJobInput(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('title', 'description', 'crawler_id', 'version_id', 'status', 'priority', 'message_priority', 'cron_expression', 'cron_utcoffset_minutes', 'settings', 'args', 'update_on_reload')
+    __field_names__ = ('title', 'description', 'crawler_id', 'version_id', 'credential_id', 'status', 'priority', 'message_priority', 'cron_expression', 'cron_utcoffset_minutes', 'settings', 'args', 'update_on_reload')
     title = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='title')
     description = sgqlc.types.Field(String, graphql_name='description')
     crawler_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='crawlerId')
     version_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='versionId')
+    credential_id = sgqlc.types.Field(ID, graphql_name='credentialId')
     status = sgqlc.types.Field(PeriodicJobStatus, graphql_name='status')
     priority = sgqlc.types.Field(JobPriorityType, graphql_name='priority')
     message_priority = sgqlc.types.Field(MessagePriority, graphql_name='messagePriority')
     cron_expression = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='cronExpression')
     cron_utcoffset_minutes = sgqlc.types.Field(Int, graphql_name='cronUTCOffsetMinutes')
     settings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValueInputType))), graphql_name='settings')
     args = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValueInputType))), graphql_name='args')
@@ -583,14 +585,22 @@
     next_schedule_time = sgqlc.types.Field(UnixTime, graphql_name='nextScheduleTime')
     total_time = sgqlc.types.Field(Long, graphql_name='totalTime')
     items_scraped_count_last = sgqlc.types.Field(Long, graphql_name='itemsScrapedCountLast')
     avg_performance_time = sgqlc.types.Field(Long, graphql_name='avgPerformanceTime')
     last_collection_date = sgqlc.types.Field(UnixTime, graphql_name='lastCollectionDate')
 
 
+class CredentialData(sgqlc.types.Type):
+    __schema__ = crawlers_api_schema
+    __field_names__ = ('id', 'data_type', 'status')
+    id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
+    data_type = sgqlc.types.Field(sgqlc.types.non_null(CredentialType), graphql_name='dataType')
+    status = sgqlc.types.Field(sgqlc.types.non_null(CredentialStatus), graphql_name='status')
+
+
 class CredentialPagination(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('total', 'list_credential')
     total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='total')
     list_credential = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Credential'))), graphql_name='listCredential')
 
 
@@ -750,15 +760,15 @@
     __field_names__ = ('total', 'list_metric')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_metric = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Metric))), graphql_name='listMetric')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('update_crawler', 'update_crawler_settings_arguments', 'delete_crawler_versions', 'delete_crawlers', 'update_site_map_crawler_body', 'add_crawl_state', 'update_crawl_state', 'delete_crawl_state', 'add_credential', 'update_credential', 'delete_credential', 'single_upload', 'add_job', 'delete_job', 'cancel_job', 'suspend_job', 'resume_job', 'download_pending_jobs', 'schedule_uploaded_jobs', 'add_periodic_job', 'run_periodic_jobs', 'update_enable_jobs_scheduling', 'update_disable_jobs_scheduling', 'delete_periodic_job', 'update_periodic_job', 'update_periodic_job_settings_and_arguments', 'import_periodic_jobs', 'delete_project', 'delete_project_versions', 'add_project', 'update_project', 'update_project_settings_and_arguments', 'add_information_source_loader', 'delete_information_source_loader', 'add_recovery_job', 'cancel_recovery_job')
+    __field_names__ = ('update_crawler', 'update_crawler_settings_arguments', 'delete_crawler_versions', 'delete_crawlers', 'update_site_map_crawler_body', 'add_crawl_state', 'update_crawl_state', 'delete_crawl_state', 'add_credential', 'update_credential', 'delete_credential', 'single_upload', 'add_job', 'delete_job', 'cancel_job', 'suspend_job', 'resume_job', 'download_pending_jobs', 'schedule_uploaded_jobs', 'restart_job', 'add_periodic_job', 'run_periodic_jobs', 'update_enable_jobs_scheduling', 'update_disable_jobs_scheduling', 'delete_periodic_job', 'update_periodic_job', 'update_periodic_job_settings_and_arguments', 'import_periodic_jobs', 'delete_project', 'delete_project_versions', 'add_project', 'update_project', 'update_project_settings_and_arguments', 'add_information_source_loader', 'delete_information_source_loader', 'add_recovery_job', 'cancel_recovery_job')
     update_crawler = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='updateCrawler', args=sgqlc.types.ArgDict((
         ('crawler_update_input', sgqlc.types.Arg(sgqlc.types.non_null(CrawlerUpdateInput), graphql_name='crawlerUpdateInput', default=None)),
         ('crawler_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='crawlerId', default=None)),
         ('project_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='projectId', default=None)),
 ))
     )
     update_crawler_settings_arguments = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='updateCrawlerSettingsArguments', args=sgqlc.types.ArgDict((
@@ -834,14 +844,18 @@
 ))
     )
     download_pending_jobs = sgqlc.types.Field(sgqlc.types.non_null(JSON), graphql_name='downloadPendingJobs')
     schedule_uploaded_jobs = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Job'))), graphql_name='scheduleUploadedJobs', args=sgqlc.types.ArgDict((
         ('file_uuid', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='fileUUID', default=None)),
 ))
     )
+    restart_job = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Job'))), graphql_name='restartJob', args=sgqlc.types.ArgDict((
+        ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
+))
+    )
     add_periodic_job = sgqlc.types.Field(sgqlc.types.non_null('PeriodicJob'), graphql_name='addPeriodicJob', args=sgqlc.types.ArgDict((
         ('periodic_job_input', sgqlc.types.Arg(sgqlc.types.non_null(PeriodicJobInput), graphql_name='periodicJobInput', default=None)),
 ))
     )
     run_periodic_jobs = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Job'))), graphql_name='runPeriodicJobs', args=sgqlc.types.ArgDict((
         ('periodic_job_ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='periodicJobIds', default=None)),
 ))
@@ -865,15 +879,15 @@
     )
     update_periodic_job_settings_and_arguments = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='updatePeriodicJobSettingsAndArguments', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
         ('settings', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValueInputType))), graphql_name='settings', default=None)),
         ('args', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValueInputType))), graphql_name='args', default=None)),
 ))
     )
-    import_periodic_jobs = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('PeriodicJob'))), graphql_name='importPeriodicJobs', args=sgqlc.types.ArgDict((
+    import_periodic_jobs = sgqlc.types.Field(sgqlc.types.non_null('PeriodicJobImport'), graphql_name='importPeriodicJobs', args=sgqlc.types.ArgDict((
         ('file_uuid', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='fileUUID', default=None)),
 ))
     )
     delete_project = sgqlc.types.Field(sgqlc.types.non_null('State'), graphql_name='deleteProject', args=sgqlc.types.ArgDict((
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
 ))
     )
@@ -918,14 +932,22 @@
 class PeriodicJobData(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('id', 'name')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(String, graphql_name='name')
 
 
+class PeriodicJobImport(sgqlc.types.Type):
+    __schema__ = crawlers_api_schema
+    __field_names__ = ('list_added_periodic_job', 'list_existing_periodic_job', 'list_failed_periodic_job_name')
+    list_added_periodic_job = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('PeriodicJob'))), graphql_name='listAddedPeriodicJob')
+    list_existing_periodic_job = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('PeriodicJob'))), graphql_name='listExistingPeriodicJob')
+    list_failed_periodic_job_name = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='listFailedPeriodicJobName')
+
+
 class PeriodicJobMetrics(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('periodic_job_id',)
     periodic_job_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='periodicJobId')
 
 
 class PeriodicJobPagination(sgqlc.types.Type):
@@ -973,15 +995,15 @@
     jobs_with_errors_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithErrorsLogsCount')
     job_ids_with_error_logs = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Long))), graphql_name='jobIdsWithErrorLogs')
     jobs_with_critical_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithCriticalLogsCount')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('analytics', 'crawler', 'list_crawler', 'pagination_crawler', 'crawler_args_and_settings_description', 'crawler_site_map', 'crawl_state', 'crawl_state_by_parameters', 'pagination_crawl_state', 'credential', 'pagination_credential', 'job', 'list_job', 'pagination_job_logs', 'pagination_job_requests', 'pagination_job_metrics', 'pagination_job', 'pagination_job_new', 'periodic_job', 'pagination_periodic_job', 'pagination_periodic_job_logs', 'pagination_periodic_job_requests', 'pagination_periodic_job_metrics', 'check_periodic_job_by_input', 'export_periodic_jobs', 'project', 'pagination_project', 'project_args_and_settings_description', 'project_default_args_and_settings_description', 'information_source_loader', 'pagination_information_source_loader', 'information_source', 'pagination_information_source', 'recovery_job', 'pagination_recovery_job', 'version', 'list_version', 'pagination_versions_crawler', 'pagination_egg_file_versions_project', 'web_scraper_version_is_compatible')
+    __field_names__ = ('analytics', 'crawler', 'list_crawler', 'pagination_crawler', 'crawler_args_and_settings_description', 'crawler_site_map', 'crawler_by_information_source', 'crawl_state', 'crawl_state_by_parameters', 'pagination_crawl_state', 'credential', 'pagination_credential', 'job', 'list_job', 'pagination_job_logs', 'pagination_job_requests', 'pagination_job_metrics', 'pagination_job', 'pagination_job_new', 'periodic_job', 'pagination_periodic_job', 'pagination_periodic_job_logs', 'pagination_periodic_job_requests', 'pagination_periodic_job_metrics', 'check_periodic_job_by_input', 'export_periodic_jobs', 'project', 'pagination_project', 'project_args_and_settings_description', 'project_default_args_and_settings_description', 'information_source_loader', 'pagination_information_source_loader', 'information_source', 'pagination_information_source', 'recovery_job', 'pagination_recovery_job', 'version', 'list_version', 'pagination_versions_crawler', 'pagination_egg_file_versions_project', 'web_scraper_version_is_compatible')
     analytics = sgqlc.types.Field(sgqlc.types.non_null('Stats'), graphql_name='analytics')
     crawler = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='crawler', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     list_crawler = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of('Crawler')), graphql_name='listCrawler', args=sgqlc.types.ArgDict((
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
@@ -1001,14 +1023,19 @@
 ))
     )
     crawler_site_map = sgqlc.types.Field(sgqlc.types.non_null(JSON), graphql_name='crawlerSiteMap', args=sgqlc.types.ArgDict((
         ('crawler_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='crawlerId', default=None)),
         ('version_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='versionId', default=None)),
 ))
     )
+    crawler_by_information_source = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='crawlerByInformationSource', args=sgqlc.types.ArgDict((
+        ('source', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='source', default=None)),
+        ('is_search_crawler', sgqlc.types.Arg(sgqlc.types.non_null(Boolean), graphql_name='isSearchCrawler', default=None)),
+))
+    )
     crawl_state = sgqlc.types.Field(sgqlc.types.non_null(CrawlState), graphql_name='crawlState', args=sgqlc.types.ArgDict((
         ('crawl_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='crawlId', default=None)),
 ))
     )
     crawl_state_by_parameters = sgqlc.types.Field(sgqlc.types.non_null(CrawlState), graphql_name='crawlStateByParameters', args=sgqlc.types.ArgDict((
         ('crawl_state_parameters', sgqlc.types.Arg(sgqlc.types.non_null(CrawlStateParameters), graphql_name='crawlStateParameters', default=None)),
 ))
@@ -1122,14 +1149,15 @@
 ))
     )
     check_periodic_job_by_input = sgqlc.types.Field('PeriodicJob', graphql_name='checkPeriodicJobByInput', args=sgqlc.types.ArgDict((
         ('periodic_job_input', sgqlc.types.Arg(sgqlc.types.non_null(PeriodicJobInput), graphql_name='periodicJobInput', default=None)),
 ))
     )
     export_periodic_jobs = sgqlc.types.Field(sgqlc.types.non_null(JSON), graphql_name='exportPeriodicJobs', args=sgqlc.types.ArgDict((
+        ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
         ('filter_settings', sgqlc.types.Arg(PeriodicJobFilterSettings, graphql_name='filterSettings', default={})),
 ))
     )
     project = sgqlc.types.Field(sgqlc.types.non_null('Project'), graphql_name='project', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
@@ -1409,46 +1437,48 @@
     actual_status = sgqlc.types.Field(sgqlc.types.non_null(InformationSourceLoaderActualStatus), graphql_name='actualStatus')
     status = sgqlc.types.Field(sgqlc.types.non_null(CollectionStatus), graphql_name='status')
     metrics = sgqlc.types.Field(sgqlc.types.non_null(InformationSourceLoaderStats), graphql_name='metrics')
 
 
 class Job(sgqlc.types.Type, RecordInterface):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('id', 'status', 'priority', 'message_priority', 'start_time', 'end_time', 'collection_status', 'monitoring_status', 'is_noise', 'crawler', 'project', 'version', 'periodic', 'settings', 'args', 'metrics', 'job_stats', 'histogram_requests', 'histogram_items', 'schema')
+    __field_names__ = ('id', 'status', 'priority', 'message_priority', 'start_time', 'end_time', 'collection_status', 'monitoring_status', 'is_noise', 'crawler', 'project', 'version', 'credential', 'periodic', 'settings', 'args', 'metrics', 'job_stats', 'histogram_requests', 'histogram_items', 'schema')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     status = sgqlc.types.Field(sgqlc.types.non_null(JobStatus), graphql_name='status')
     priority = sgqlc.types.Field(sgqlc.types.non_null(JobPriorityType), graphql_name='priority')
     message_priority = sgqlc.types.Field(sgqlc.types.non_null(MessagePriority), graphql_name='messagePriority')
     start_time = sgqlc.types.Field(UnixTime, graphql_name='startTime')
     end_time = sgqlc.types.Field(UnixTime, graphql_name='endTime')
     collection_status = sgqlc.types.Field(sgqlc.types.non_null(CollectionStatus), graphql_name='collectionStatus')
     monitoring_status = sgqlc.types.Field(sgqlc.types.non_null(MonitoringStatus), graphql_name='monitoringStatus')
     is_noise = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isNoise')
     crawler = sgqlc.types.Field(sgqlc.types.non_null(CrawlerData), graphql_name='crawler')
     project = sgqlc.types.Field(sgqlc.types.non_null(ProjectData), graphql_name='project')
     version = sgqlc.types.Field(sgqlc.types.non_null(VersionData), graphql_name='version')
+    credential = sgqlc.types.Field(CredentialData, graphql_name='credential')
     periodic = sgqlc.types.Field(PeriodicJobData, graphql_name='periodic')
     settings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='settings')
     args = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='args')
     metrics = sgqlc.types.Field(sgqlc.types.non_null(JobMetrics), graphql_name='metrics')
     job_stats = sgqlc.types.Field(JobStats, graphql_name='jobStats')
     histogram_requests = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(DateHistogramBucket))), graphql_name='histogramRequests')
     histogram_items = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(DateHistogramBucket))), graphql_name='histogramItems')
     schema = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='schema')
 
 
 class PeriodicJob(sgqlc.types.Type, RecordInterface):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('id', 'name', 'description', 'project', 'crawler', 'version', 'priority', 'message_priority', 'status', 'monitoring_status', 'cron', 'cron_utcoffset_minutes', 'next_schedule_time', 'update_on_reload', 'settings', 'args', 'metrics', 'histogram_requests', 'histogram_items', 'job_stats', 'job_failed_monitoring_statuses')
+    __field_names__ = ('id', 'name', 'description', 'project', 'crawler', 'version', 'credential', 'priority', 'message_priority', 'status', 'monitoring_status', 'cron', 'cron_utcoffset_minutes', 'next_schedule_time', 'update_on_reload', 'settings', 'args', 'metrics', 'histogram_requests', 'histogram_items', 'job_stats', 'job_failed_monitoring_statuses')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(String, graphql_name='name')
     description = sgqlc.types.Field(String, graphql_name='description')
     project = sgqlc.types.Field(sgqlc.types.non_null(ProjectData), graphql_name='project')
     crawler = sgqlc.types.Field(sgqlc.types.non_null(CrawlerData), graphql_name='crawler')
     version = sgqlc.types.Field(sgqlc.types.non_null(VersionData), graphql_name='version')
+    credential = sgqlc.types.Field(CredentialData, graphql_name='credential')
     priority = sgqlc.types.Field(sgqlc.types.non_null(JobPriorityType), graphql_name='priority')
     message_priority = sgqlc.types.Field(sgqlc.types.non_null(MessagePriority), graphql_name='messagePriority')
     status = sgqlc.types.Field(sgqlc.types.non_null(PeriodicJobStatus), graphql_name='status')
     monitoring_status = sgqlc.types.Field(sgqlc.types.non_null(MonitoringStatus), graphql_name='monitoringStatus')
     cron = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='cron')
     cron_utcoffset_minutes = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='cronUTCOffsetMinutes')
     next_schedule_time = sgqlc.types.Field(UnixTime, graphql_name='nextScheduleTime')
```

### Comparing `ptal_api-0.12.2/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.12.3/ptal_api/schema/tcontroller_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.12.3/ptal_api/schema/utils_api_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,19 +76,14 @@
 
 
 class DocumentGrouping(sgqlc.types.Enum):
     __schema__ = utils_api_schema
     __choices__ = ('none', 'story')
 
 
-class DocumentRecall(sgqlc.types.Enum):
-    __schema__ = utils_api_schema
-    __choices__ = ('high', 'low', 'medium', 'none')
-
-
 class DocumentSorting(sgqlc.types.Enum):
     __schema__ = utils_api_schema
     __choices__ = ('countChildDocs', 'countConcepts', 'countDisambiguatedEntities', 'countEntities', 'countEvents', 'countLinks', 'countNamedEntities', 'countObjects', 'countPropertyCandidates', 'countResearchMaps', 'countTasks', 'id', 'publicationDate', 'registrationDate', 'relevance', 'score', 'secretLevel', 'text', 'title', 'trustLevel', 'updateDate')
 
 
 class DocumentSourceType(sgqlc.types.Enum):
     __schema__ = utils_api_schema
@@ -686,22 +681,16 @@
     list_account = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Account'))), graphql_name='listAccount')
     total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='total')
     total_platforms = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='totalPlatforms')
 
 
 class AccountStatistics(sgqlc.types.Type):
     __schema__ = utils_api_schema
-    __field_names__ = ('count_doc', 'count_doc_today', 'count_doc_week', 'count_doc_month', 'recall_doc_today', 'recall_doc_week', 'recall_doc_month')
+    __field_names__ = ('count_doc',)
     count_doc = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDoc')
-    count_doc_today = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocToday')
-    count_doc_week = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocWeek')
-    count_doc_month = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocMonth')
-    recall_doc_today = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocToday')
-    recall_doc_week = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocWeek')
-    recall_doc_month = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocMonth')
 
 
 class Annotation(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('start', 'end', 'value')
     start = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='start')
     end = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='end')
@@ -1299,23 +1288,17 @@
     __field_names__ = ('value', 'count')
     value = sgqlc.types.Field(sgqlc.types.non_null('Platform'), graphql_name='value')
     count = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='count')
 
 
 class PlatformStatistics(sgqlc.types.Type):
     __schema__ = utils_api_schema
-    __field_names__ = ('count_account', 'count_doc', 'count_doc_today', 'count_doc_week', 'count_doc_month', 'recall_doc_today', 'recall_doc_week', 'recall_doc_month')
+    __field_names__ = ('count_account', 'count_doc')
     count_account = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countAccount')
     count_doc = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDoc')
-    count_doc_today = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocToday')
-    count_doc_week = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocWeek')
-    count_doc_month = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDocMonth')
-    recall_doc_today = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocToday')
-    recall_doc_week = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocWeek')
-    recall_doc_month = sgqlc.types.Field(sgqlc.types.non_null(DocumentRecall), graphql_name='recallDocMonth')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('mention_search', 'batch_mention_search', 'list_document_for_time_period', 'list_text_from_document_with_marker', 'pagination_concept_without_elastic', 'tdm', 'pagination_concept', 'pagination_concept_property_type')
     mention_search = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ConceptMentionCount))), graphql_name='mentionSearch', args=sgqlc.types.ArgDict((
         ('form', sgqlc.types.Arg(sgqlc.types.non_null(ConceptMentionCountInput), graphql_name='form', default=None)),
```

### Comparing `ptal_api-0.12.2/ptal_api/scripts/type_mapper.py` & `ptal_api-0.12.3/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.12.3/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.2/pyproject.toml` & `ptal_api-0.12.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "0.12.2"
+version = "0.12.3"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
@@ -24,14 +24,15 @@
 sgqlc = ">=16.0"
 python-keycloak = ">=2.6.0"
 graphql-core = ">=3.2.3"
 transliterate = ">=1.10.2"
 marshmallow-dataclass = ">=8.5.11"
 "ruamel.yaml" = ">=0.17.21"
 click = ">=8.1.3"
+pyjwt = ">=2.7.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
 ruff = "^0.0.261"
 black = "^23.3.0"
 
 [tool.black]
```

### Comparing `ptal_api-0.12.2/PKG-INFO` & `ptal_api-0.12.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.12.2
+Version: 0.12.3
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: graphql-core (>=3.2.3)
 Requires-Dist: marshmallow-dataclass (>=8.5.11)
+Requires-Dist: pyjwt (>=2.7.0)
 Requires-Dist: python-keycloak (>=2.6.0)
 Requires-Dist: ruamel.yaml (>=0.17.21)
 Requires-Dist: sgqlc (>=16.0)
 Requires-Dist: transliterate (>=1.10.2)
 Description-Content-Type: text/markdown
 
 # ptal-api
```

