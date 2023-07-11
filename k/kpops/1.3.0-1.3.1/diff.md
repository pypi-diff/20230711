# Comparing `tmp/kpops-1.3.0.tar.gz` & `tmp/kpops-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-1.3.0.tar", max compression
+gzip compressed data, was "kpops-1.3.1.tar", max compression
```

## Comparing `kpops-1.3.0.tar` & `kpops-1.3.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1064 2023-07-07 14:41:41.908185 kpops-1.3.0/LICENSE
--rw-r--r--   0        0        0     2350 2023-07-07 14:41:41.908185 kpops-1.3.0/README.md
--rw-r--r--   0        0        0       22 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      122 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/cli/exception.py
--rw-r--r--   0        0        0    11727 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/cli/main.py
--rw-r--r--   0        0        0     4283 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/cli/pipeline_config.py
--rw-r--r--   0        0        0     1969 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/cli/registry.py
--rw-r--r--   0        0        0      688 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0     1167 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py
--rw-r--r--   0        0        0       52 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0    10517 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2152 2023-07-07 14:41:41.912185 kpops-1.3.0/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     4341 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      667 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     8142 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      235 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5832 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     1825 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      999 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6272 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      361 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      231 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9358 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2503 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     6917 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      630 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      492 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/__init__.py
--rw-r--r--   0        0        0      466 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0     7711 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     6658 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0    15918 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     6941 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0       66 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     2471 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0     3340 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0     8915 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0      211 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2831 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0     9067 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     3463 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0        0 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/pipeline_generator/__init__.py
--rw-r--r--   0        0        0    13148 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/pipeline_generator/pipeline.py
--rw-r--r--   0        0        0        0 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/utils/__init__.py
--rw-r--r--   0        0        0      289 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3043 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     3878 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/utils/dict_ops.py
--rw-r--r--   0        0        0     2597 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/utils/docstring.py
--rw-r--r--   0        0        0     1032 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/utils/environment.py
--rw-r--r--   0        0        0     5620 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      552 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/utils/pydantic.py
--rw-r--r--   0        0        0     2563 2023-07-07 14:41:41.916185 kpops-1.3.0/kpops/utils/yaml_loading.py
--rw-r--r--   0        0        0     1900 2023-07-07 14:41:41.916185 kpops-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 kpops-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-11 14:40:57.030523 kpops-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2350 2023-07-11 14:40:57.030523 kpops-1.3.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      122 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/cli/exception.py
+-rw-r--r--   0        0        0    11641 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/cli/main.py
+-rw-r--r--   0        0        0     4283 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/cli/pipeline_config.py
+-rw-r--r--   0        0        0     1969 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/cli/registry.py
+-rw-r--r--   0        0        0      688 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0     1167 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/helm_wrapper/dry_run_handler.py
+-rw-r--r--   0        0        0       52 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0    10517 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2152 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     4341 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      667 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     8142 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      235 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     5832 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     1825 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      999 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6272 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      361 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      231 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9358 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2503 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     6917 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      630 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      492 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/__init__.py
+-rw-r--r--   0        0        0      466 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0     7711 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     6658 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0    15918 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     6941 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0       66 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     2471 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0     3340 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0     8915 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0      211 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2831 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0     9067 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     3463 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/pipeline_generator/__init__.py
+-rw-r--r--   0        0        0    13179 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/pipeline_generator/pipeline.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/utils/__init__.py
+-rw-r--r--   0        0        0      289 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3043 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     3878 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/utils/dict_ops.py
+-rw-r--r--   0        0        0     2597 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/utils/docstring.py
+-rw-r--r--   0        0        0     1032 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/utils/environment.py
+-rw-r--r--   0        0        0     5620 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      552 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0     2563 2023-07-11 14:40:57.038523 kpops-1.3.1/kpops/utils/yaml_loading.py
+-rw-r--r--   0        0        0     1933 2023-07-11 14:40:57.042523 kpops-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 kpops-1.3.1/PKG-INFO
```

### Comparing `kpops-1.3.0/LICENSE` & `kpops-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/README.md` & `kpops-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/cli/custom_formatter.py` & `kpops-1.3.1/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/cli/main.py` & `kpops-1.3.1/kpops/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,19 +150,17 @@
     )
     return steps_to_apply
 
 
 def get_steps_to_apply(
     pipeline: Pipeline, steps: str | None
 ) -> list[PipelineComponent]:
-    return (
-        list(pipeline)
-        if not steps or steps == '""'  # workaround to allow "" as empty value for CI
-        else filter_steps_to_apply(pipeline, steps=parse_steps(steps))
-    )
+    if steps:
+        return filter_steps_to_apply(pipeline, steps=parse_steps(steps))
+    return list(pipeline)
 
 
 def reverse_pipeline_steps(pipeline, steps) -> Iterator[PipelineComponent]:
     return reversed(get_steps_to_apply(pipeline, steps))
 
 
 def log_action(action: str, pipeline_component: PipelineComponent):
```

### Comparing `kpops-1.3.0/kpops/cli/pipeline_config.py` & `kpops-1.3.1/kpops/cli/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/cli/registry.py` & `kpops-1.3.1/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/__init__.py` & `kpops-1.3.1/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py` & `kpops-1.3.1/kpops/component_handlers/helm_wrapper/dry_run_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-1.3.1/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-1.3.1/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/helm_wrapper/model.py` & `kpops-1.3.1/kpops/component_handlers/helm_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-1.3.1/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-1.3.1/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-1.3.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/kafka_connect/model.py` & `kpops-1.3.1/kpops/component_handlers/kafka_connect/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-1.3.1/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-1.3.1/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/topic/handler.py` & `kpops-1.3.1/kpops/component_handlers/topic/handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/topic/model.py` & `kpops-1.3.1/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-1.3.1/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/topic/utils.py` & `kpops-1.3.1/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/component_handlers/utils/exception.py` & `kpops-1.3.1/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/base_components/base_defaults_component.py` & `kpops-1.3.1/kpops/components/base_components/base_defaults_component.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/base_components/kafka_app.py` & `kpops-1.3.1/kpops/components/base_components/kafka_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/base_components/kafka_connector.py` & `kpops-1.3.1/kpops/components/base_components/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/base_components/kubernetes_app.py` & `kpops-1.3.1/kpops/components/base_components/kubernetes_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/base_components/models/from_section.py` & `kpops-1.3.1/kpops/components/base_components/models/from_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/base_components/models/to_section.py` & `kpops-1.3.1/kpops/components/base_components/models/to_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/base_components/pipeline_component.py` & `kpops-1.3.1/kpops/components/base_components/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/streams_bootstrap/producer/model.py` & `kpops-1.3.1/kpops/components/streams_bootstrap/producer/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-1.3.1/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/streams_bootstrap/streams/model.py` & `kpops-1.3.1/kpops/components/streams_bootstrap/streams/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-1.3.1/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/pipeline_generator/pipeline.py` & `kpops-1.3.1/kpops/pipeline_generator/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,14 +253,15 @@
         :param substitution: Substitution dictionary, defaults to None
         :type substitution: dict | None, optional
         """
         syntax = Syntax(
             substitute(str(self), substitution),
             "yaml",
             background_color="default",
+            theme="ansi_dark",
         )
         Console(
             width=1000  # HACK: overwrite console width to avoid truncating output
         ).print(syntax)
 
     def __iter__(self) -> Iterator[PipelineComponent]:
         return iter(self.components)
```

### Comparing `kpops-1.3.0/kpops/utils/dict_differ.py` & `kpops-1.3.1/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/utils/dict_ops.py` & `kpops-1.3.1/kpops/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/utils/docstring.py` & `kpops-1.3.1/kpops/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/utils/environment.py` & `kpops-1.3.1/kpops/utils/environment.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/utils/gen_schema.py` & `kpops-1.3.1/kpops/utils/gen_schema.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/utils/pydantic.py` & `kpops-1.3.1/kpops/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/kpops/utils/yaml_loading.py` & `kpops-1.3.1/kpops/utils/yaml_loading.py`

 * *Files identical despite different names*

### Comparing `kpops-1.3.0/pyproject.toml` & `kpops-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "1.3.0"
+version = "1.3.1"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
@@ -46,14 +46,15 @@
 responses = "^0.22.0"
 pre-commit = "^2.19.0"
 flake8 = "^4.0.1"
 black = "^22.3.0"
 isort = "^5.12.0"
 typer-cli = "^0.0.13"
 pyright = "^1.1.314"
+pytest-rerunfailures = "^11.1.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-macros-plugin = "^0.7.0"
 mkdocs-material = "^9.0.0"
```

### Comparing `kpops-1.3.0/PKG-INFO` & `kpops-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 1.3.0
+Version: 1.3.1
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<4.0
```

