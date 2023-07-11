# Comparing `tmp/oarepo-model-builder-ui-4.0.6.tar.gz` & `tmp/oarepo-model-builder-ui-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-ui-4.0.6.tar", last modified: Sun Jul  2 16:29:54 2023, max compression
+gzip compressed data, was "oarepo-model-builder-ui-4.0.7.tar", last modified: Tue Jul 11 07:40:10 2023, max compression
```

## Comparing `oarepo-model-builder-ui-4.0.6.tar` & `oarepo-model-builder-ui-4.0.7.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.791012 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/layout_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/components/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/outputs/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/outputs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.791012 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:40:10.436294 oarepo-model-builder-ui-4.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-11 07:40:10.440294 oarepo-model-builder-ui-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:40:10.436294 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:40:10.436294 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/builders/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/builders/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/builders/layout_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:40:10.436294 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:40:10.436294 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/datatypes/components/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/datatypes/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:40:10.436294 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/outputs/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/outputs/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:40:10.436294 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:40:10.436294 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-11 07:40:10.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-11 07:40:10.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 07:40:10.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-11 07:40:10.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 07:40:10.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 07:40:10.000000 oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 07:40:10.440294 oarepo-model-builder-ui-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 07:36:29.000000 oarepo-model-builder-ui-4.0.7/setup.py
```

### Comparing `oarepo-model-builder-ui-4.0.6/PKG-INFO` & `oarepo-model-builder-ui-4.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 4.0.6
+Version: 4.0.7
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-4.0.6/README.md` & `oarepo-model-builder-ui-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/i18n.py` & `oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/builders/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/i18n_setup_cfg.py` & `oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/builders/i18n_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/layout.py` & `oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/builders/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/layout_setup_cfg.py` & `oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/builders/layout_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/components/model.py` & `oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/datatypes/components/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 class TranslationsSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
     module = ma.fields.Str()
     alias = ma.fields.Str()
 
+
 class UISchema(ma.Schema):
     """
     registered in entry points to the ui.model group
     """
     class Meta:
         unknown = ma.RAISE
 
     module = ma.fields.Str()
     file = ma.fields.Str()
     alias = ma.fields.Str()
 
+
 class UIModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
     depends_on=[SavedModelComponent]
 
     class ModelSchema(ma.Schema):
         translations = ma.fields.Nested(TranslationsSchema)
```

### Comparing `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/outputs/i18n.py` & `oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/outputs/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/outputs/layout.py` & `oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui/outputs/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/PKG-INFO` & `oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 4.0.6
+Version: 4.0.7
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/SOURCES.txt` & `oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 oarepo_model_builder_ui.egg-info/top_level.txt
 oarepo_model_builder_ui/builders/__init__.py
 oarepo_model_builder_ui/builders/i18n.py
 oarepo_model_builder_ui/builders/i18n_setup_cfg.py
 oarepo_model_builder_ui/builders/layout.py
 oarepo_model_builder_ui/builders/layout_setup_cfg.py
 oarepo_model_builder_ui/datatypes/__init__.py
+oarepo_model_builder_ui/datatypes/validation.py
 oarepo_model_builder_ui/datatypes/components/__init__.py
 oarepo_model_builder_ui/datatypes/components/model.py
 oarepo_model_builder_ui/outputs/i18n.py
 oarepo_model_builder_ui/outputs/layout.py
 oarepo_model_builder_ui/validation/__init__.py
```

### Comparing `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/entry_points.txt` & `oarepo-model-builder-ui-4.0.7/oarepo_model_builder_ui.egg-info/entry_points.txt`

 * *Files 17% similar despite different names*

```diff
@@ -14,7 +14,13 @@
 po = oarepo_model_builder_ui.outputs.i18n:POOutput
 
 [oarepo_model_builder.validation.settings]
 ui-settings = oarepo_model_builder_ui.validation:UISettingsSchema
 
 [oarepo_model_builder.validation.ui.model]
 ui-model = oarepo_model_builder_ui.datatypes.components.model:UISchema
+
+[oarepo_model_builder.validation.ui.object]
+ui-object = oarepo_model_builder_ui.datatypes.validation:UIObjectSchema
+
+[oarepo_model_builder.validation.ui.property]
+ui-property = oarepo_model_builder_ui.datatypes.validation:UIPropertySchema
```

### Comparing `oarepo-model-builder-ui-4.0.6/setup.cfg` & `oarepo-model-builder-ui-4.0.7/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-ui
-version = 4.0.6
+version = 4.0.7
 description = Model builder plugin for oarepo-ui
 authors = 
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -29,14 +29,18 @@
 * = *.json, *.rst, *.md, *.json5, *.jinja2
 
 [options.entry_points]
 oarepo_model_builder.validation.settings = 
 	ui-settings = oarepo_model_builder_ui.validation:UISettingsSchema
 oarepo_model_builder.validation.ui.model = 
 	ui-model = oarepo_model_builder_ui.datatypes.components.model:UISchema
+oarepo_model_builder.validation.ui.property = 
+	ui-property = oarepo_model_builder_ui.datatypes.validation:UIPropertySchema
+oarepo_model_builder.validation.ui.object = 
+	ui-object = oarepo_model_builder_ui.datatypes.validation:UIObjectSchema
 oarepo_model_builder.datatypes.components = 
 	ui-components = oarepo_model_builder_ui.datatypes.components:components
 oarepo_model_builder.builders.record = 
 	4000-oarepo-i18n = oarepo_model_builder_ui.builders.i18n:InvenioI18nBuilder
 	4010-oarepo-i18n-setup = oarepo_model_builder_ui.builders.i18n_setup_cfg:InvenioI18NSetupCfgBuilder
 	4020-oarepo-ui-layout = oarepo_model_builder_ui.builders.layout:InvenioLayoutBuilder
 	4030-oarepo-ui-layout-setup = oarepo_model_builder_ui.builders.layout_setup_cfg:InvenioLayoutSetupCfgBuilder
```

