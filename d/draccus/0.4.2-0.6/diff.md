# Comparing `tmp/draccus-0.4.2.tar.gz` & `tmp/draccus-0.6.tar.gz`

## Comparing `draccus-0.4.2.tar` & `draccus-0.6.tar`

### file list

```diff
@@ -1,70 +1,73 @@
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 draccus-0.4.2/.all-contributorsrc
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 draccus-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 draccus-0.4.2/mkdocs.yml
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 draccus-0.4.2/python-package.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 draccus-0.4.2/setup.cfg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 draccus-0.4.2/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 draccus-0.4.2/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 draccus-0.4.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/draccus.iml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/vcs.xml
--rw-r--r--   0        0        0    39068 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/workspace.xml
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 draccus-0.4.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    17123 2020-02-02 00:00:00.000000 draccus-0.4.2/docs/api.md
--rw-r--r--   0        0        0  5114979 2020-02-02 00:00:00.000000 draccus-0.4.2/docs/argparse2pyrallis.gif
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 draccus-0.4.2/docs/index.md
--rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 draccus-0.4.2/docs/step_by_step.md
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/__init__.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/argparsing.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/cfgparsing.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/choice_types.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/fields.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/help_formatter.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/py.typed
--rw-r--r--   0        0        0     9252 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/parsers/__init__.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/parsers/config_parsers.py
--rw-r--r--   0        0        0    12653 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/parsers/decoding.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/parsers/encoding.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/parsers/registry_utils.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/__init__.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/choice_wrapper.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/dataclass_wrapper.py
--rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/docstring.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/field_metavar.py
--rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/field_wrapper.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/suppressing_argparse.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 draccus-0.4.2/draccus/wrappers/wrapper.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 draccus-0.4.2/examples/choice_class_demo.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 draccus-0.4.2/examples/demo.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/conftest.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_argparse_choice_types.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_argparse_choice_types_plugin.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_base.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_bools.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_choice_types.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_decoding.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_default_args.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_docstrings.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_enums.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_inheritance.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_lists.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_optional.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_optional_union.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_tuples.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_union.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/test_utils.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/testutils.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/draccus_choice_plugins/gpt.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 draccus-0.4.2/tests/draccus_choice_plugins/model_config.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.4.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 draccus-0.4.2/LICENSE
--rw-r--r--   0        0        0    20257 2020-02-02 00:00:00.000000 draccus-0.4.2/README.md
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 draccus-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    20931 2020-02-02 00:00:00.000000 draccus-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 draccus-0.6/.DS_Store
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 draccus-0.6/.all-contributorsrc
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 draccus-0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 draccus-0.6/mkdocs.yml
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 draccus-0.6/python-package.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 draccus-0.6/setup.cfg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 draccus-0.6/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 draccus-0.6/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 draccus-0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 draccus-0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 draccus-0.6/.idea/draccus.iml
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 draccus-0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 draccus-0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 draccus-0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0    41989 2020-02-02 00:00:00.000000 draccus-0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 draccus-0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 draccus-0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    17123 2020-02-02 00:00:00.000000 draccus-0.6/docs/api.md
+-rw-r--r--   0        0        0  5114979 2020-02-02 00:00:00.000000 draccus-0.6/docs/argparse2pyrallis.gif
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 draccus-0.6/docs/index.md
+-rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 draccus-0.6/docs/step_by_step.md
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 draccus-0.6/draccus/__init__.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 draccus-0.6/draccus/argparsing.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 draccus-0.6/draccus/cfgparsing.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 draccus-0.6/draccus/choice_types.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 draccus-0.6/draccus/fields.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 draccus-0.6/draccus/help_formatter.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 draccus-0.6/draccus/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.6/draccus/py.typed
+-rw-r--r--   0        0        0     9252 2020-02-02 00:00:00.000000 draccus-0.6/draccus/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 draccus-0.6/draccus/parsers/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 draccus-0.6/draccus/parsers/config_parsers.py
+-rw-r--r--   0        0        0    12653 2020-02-02 00:00:00.000000 draccus-0.6/draccus/parsers/decoding.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 draccus-0.6/draccus/parsers/encoding.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 draccus-0.6/draccus/parsers/registry_utils.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 draccus-0.6/draccus/parsers/yaml_loader.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 draccus-0.6/draccus/wrappers/__init__.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 draccus-0.6/draccus/wrappers/choice_wrapper.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 draccus-0.6/draccus/wrappers/dataclass_wrapper.py
+-rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 draccus-0.6/draccus/wrappers/docstring.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 draccus-0.6/draccus/wrappers/field_metavar.py
+-rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 draccus-0.6/draccus/wrappers/field_wrapper.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 draccus-0.6/draccus/wrappers/suppressing_argparse.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 draccus-0.6/draccus/wrappers/wrapper.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 draccus-0.6/examples/choice_class_demo.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 draccus-0.6/examples/demo.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 draccus-0.6/tests/__init__.py
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 draccus-0.6/tests/conftest.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_argparse_choice_types.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_argparse_choice_types_plugin.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_base.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_bools.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_choice_types.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_decoding.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_default_args.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_docstrings.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_enums.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_inheritance.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_lists.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_optional.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_optional_union.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_tuples.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_union.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_utils.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 draccus-0.6/tests/test_yaml_inclusion.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 draccus-0.6/tests/testutils.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 draccus-0.6/tests/draccus_choice_plugins/gpt.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 draccus-0.6/tests/draccus_choice_plugins/model_config.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 draccus-0.6/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 draccus-0.6/LICENSE
+-rw-r--r--   0        0        0    21248 2020-02-02 00:00:00.000000 draccus-0.6/README.md
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 draccus-0.6/pyproject.toml
+-rw-r--r--   0        0        0    21955 2020-02-02 00:00:00.000000 draccus-0.6/PKG-INFO
```

### Comparing `draccus-0.4.2/.all-contributorsrc` & `draccus-0.6/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/.pre-commit-config.yaml` & `draccus-0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/mkdocs.yml` & `draccus-0.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/python-package.yml` & `draccus-0.6/python-package.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/.github/workflows/pytest.yml` & `draccus-0.6/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/.github/workflows/python-publish.yml` & `draccus-0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/.idea/draccus.iml` & `draccus-0.6/.idea/draccus.iml`

 * *Files 3% similar despite different names*

#### Comparing `draccus-0.4.2/.idea/draccus.iml` & `draccus-0.6/.idea/draccus.iml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <module type="PYTHON_MODULE" version="4">
   <component name="NewModuleRootManager">
     <content url="file://$MODULE_DIR$"/>
-    <orderEntry type="jdk" jdkName="levanter" jdkType="Python SDK"/>
+    <orderEntry type="jdk" jdkName="draccus-3.8" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
   <component name="PyDocumentationSettings">
     <option name="format" value="PLAIN"/>
     <option name="myDocStringFormat" value="Plain"/>
   </component>
   <component name="TestRunnerService">
```

### Comparing `draccus-0.4.2/.idea/workspace.xml` & `draccus-0.6/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `draccus-0.4.2/.idea/workspace.xml` & `draccus-0.6/.idea/workspace.xml`

```diff
@@ -1,34 +1,40 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="5b933ae7-cc65-4dc5-9717-968698524fae" name="Changes" comment="improve exceptions when something goes wrong">
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+    <list default="true" id="5b933ae7-cc65-4dc5-9717-968698524fae" name="Changes" comment="support &lt;&lt;: inclusion">
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
       <list>
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
+    <option name="RECENT_BRANCH_BY_REPOSITORY">
+      <map>
+        <entry key="$PROJECT_DIR$" value="main"/>
+      </map>
+    </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="HighlightingSettingsPerFile">
     <setting file="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/typeshed/stdlib/argparse.pyi" root0="SKIP_INSPECTION"/>
     <setting file="file://$PROJECT_DIR$/draccus/choice_types.py" root0="SKIP_INSPECTION"/>
+    <setting file="file://$PROJECT_DIR$/draccus/parsers/decoding.py" root0="SKIP_INSPECTION"/>
     <setting file="file://$PROJECT_DIR$/draccus/wrappers/choice_wrapper.py" root0="SKIP_INSPECTION"/>
     <setting file="file://$PROJECT_DIR$/draccus/wrappers/dataclass_wrapper.py" root0="SKIP_INSPECTION"/>
     <setting file="file://$PROJECT_DIR$/draccus/wrappers/field_wrapper.py" root0="SKIP_INSPECTION"/>
     <setting file="file://$PROJECT_DIR$/tests/test_enums.py" root0="SKIP_INSPECTION"/>
     <setting file="file:///opt/homebrew/Caskroom/miniforge/base/envs/levanter/lib/python3.10/argparse.py" root0="SKIP_INSPECTION"/>
     <setting file="file:///opt/homebrew/Caskroom/miniforge/base/envs/levanter/lib/python3.10/dataclasses.py" root0="SKIP_INSPECTION"/>
     <setting file="file:///opt/homebrew/Caskroom/miniforge/base/envs/levanter/lib/python3.10/importlib/__init__.py" root0="SKIP_INSPECTION"/>
@@ -60,172 +66,138 @@
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "TODO_SCOPE": "All Places",
     "WebServerToolWindowFactoryState": "false",
-    "git-widget-placeholder": "main",
+    "git-widget-placeholder": "include",
     "last.edited.regexp": "usage: draccus [-h] [--config_path str] [--person.type {adult,child}]\n               [--person.age int] [--person.name str]\n               [--person.favorite_toy str]\n\noptions:\n  -h, --help            show this help message and exit\n  --config_path str     Path for a config file to parse with draccus (default:\n                        None)\n\nSomething:\n\nPerson ['person']:\n\n  --person.type {adult,child}\n                        Which type of Person ['person'] to use (default: None)\n\nAdult ['person']:\n\n  --person.name str     Person's name (default: None)\n  --person.age int\n\nChild ['person']:\n\n  --person.name str     Person's name (default: None)\n  --person.favorite_toy str\n                        Child's favorite toy (default: None)",
     "last_opened_file_path": "/Users/dlwh/src/draccus/tests",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
+    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/tests"/>
       <recent name="$PROJECT_DIR$/examples"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python tests.pytest for tests.test_lists.test_list_of_dataclasses">
-    <configuration name="pytest for test_optional.test_optional_parameter_group" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+  <component name="RunManager" selected="Python tests.pytest for test_yaml_inclusion.test_merge_include_hyperparameters">
+    <configuration name="pytest for test_yaml_inclusion.test_merge_include_hyperparameters" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_keywords" value="&quot;&quot;"/>
       <option name="_new_parameters" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_optional.test_optional_parameter_group&quot;"/>
+      <option name="_new_target" value="&quot;test_yaml_inclusion.test_merge_include_hyperparameters&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="pytest for tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+    <configuration name="pytest for tests.test_lists.test_collection_no_type (1)" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_keywords" value="&quot;&quot;"/>
-      <option name="_new_parameters" value="&quot;&quot;"/>
+      <option name="_new_parameters" value="&quot;dict-Dict-value4-{1: 2}&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_lists.test_collection_no_type&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="pytest for tests.test_lists.test_collection_no_type (1)" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+    <configuration name="pytest for tests.test_lists.test_collection_no_type" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_keywords" value="&quot;&quot;"/>
-      <option name="_new_parameters" value="&quot;dict-Dict-value4-{1: 2}&quot;"/>
+      <option name="_new_parameters" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;tests.test_lists.test_collection_no_type&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="pytest for tests.test_lists.test_collection_no_type" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+    <configuration name="pytest for tests.test_lists.test_list_of_dataclasses" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_keywords" value="&quot;&quot;"/>
       <option name="_new_parameters" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.test_lists.test_collection_no_type&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_lists.test_list_of_dataclasses&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="pytest for tests.test_lists.test_list_of_dataclasses" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
+    <configuration name="pytest for tests.test_yaml_inclusion.test_load_hyperparameters_with_include" type="tests" factoryName="py.test" temporary="true" nameIsGenerated="true">
       <module name="draccus"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_keywords" value="&quot;&quot;"/>
       <option name="_new_parameters" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.test_lists.test_list_of_dataclasses&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_yaml_inclusion.test_load_hyperparameters_with_include&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <recent_temporary>
       <list>
+        <item itemvalue="Python tests.pytest for test_yaml_inclusion.test_merge_include_hyperparameters"/>
+        <item itemvalue="Python tests.pytest for tests.test_yaml_inclusion.test_load_hyperparameters_with_include"/>
         <item itemvalue="Python tests.pytest for tests.test_lists.test_list_of_dataclasses"/>
         <item itemvalue="Python tests.pytest for tests.test_lists.test_collection_no_type (1)"/>
         <item itemvalue="Python tests.pytest for tests.test_lists.test_collection_no_type"/>
-        <item itemvalue="Python tests.pytest for test_optional.test_optional_parameter_group"/>
-        <item itemvalue="Python tests.pytest for tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="5b933ae7-cc65-4dc5-9717-968698524fae" name="Changes" comment=""/>
       <created>1687456901125</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1687456901125</updated>
       <workItem from="1687456902334" duration="32485000"/>
-      <workItem from="1687548821702" duration="33145000"/>
-    </task>
-    <task id="LOCAL-00011" summary="wtf">
-      <created>1687463618770</created>
-      <option name="number" value="00011"/>
-      <option name="presentableId" value="LOCAL-00011"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687463618770</updated>
-    </task>
-    <task id="LOCAL-00012" summary="refactoring towardss registries">
-      <created>1687464412290</created>
-      <option name="number" value="00012"/>
-      <option name="presentableId" value="LOCAL-00012"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687464412290</updated>
-    </task>
-    <task id="LOCAL-00013" summary="refactoring towardss registries">
-      <created>1687464450788</created>
-      <option name="number" value="00013"/>
-      <option name="presentableId" value="LOCAL-00013"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687464450788</updated>
-    </task>
-    <task id="LOCAL-00014" summary="refactoring towards registries">
-      <created>1687464453332</created>
-      <option name="number" value="00014"/>
-      <option name="presentableId" value="LOCAL-00014"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687464453332</updated>
-    </task>
-    <task id="LOCAL-00015" summary="refactor methods around a bit so that Fields are responsible for registering themselves">
-      <created>1687476683353</created>
-      <option name="number" value="00015"/>
-      <option name="presentableId" value="LOCAL-00015"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1687476683353</updated>
+      <workItem from="1687548821702" duration="55783000"/>
     </task>
     <task id="LOCAL-00016" summary="composition over inheritance">
       <created>1687477252681</created>
       <option name="number" value="00016"/>
       <option name="presentableId" value="LOCAL-00016"/>
       <option name="project" value="LOCAL"/>
       <updated>1687477252681</updated>
@@ -527,15 +499,50 @@
     <task id="LOCAL-00059" summary="improve exceptions when something goes wrong">
       <created>1688064033785</created>
       <option name="number" value="00059"/>
       <option name="presentableId" value="LOCAL-00059"/>
       <option name="project" value="LOCAL"/>
       <updated>1688064033785</updated>
     </task>
-    <option name="localTasksCounter" value="60"/>
+    <task id="LOCAL-00060" summary="missed a dep">
+      <created>1688065186816</created>
+      <option name="number" value="00060"/>
+      <option name="presentableId" value="LOCAL-00060"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688065186816</updated>
+    </task>
+    <task id="LOCAL-00061" summary="add !include for yaml">
+      <created>1688625802990</created>
+      <option name="number" value="00061"/>
+      <option name="presentableId" value="LOCAL-00061"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688625802990</updated>
+    </task>
+    <task id="LOCAL-00062" summary="add basic docs for inclusion">
+      <created>1688714606842</created>
+      <option name="number" value="00062"/>
+      <option name="presentableId" value="LOCAL-00062"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688714606842</updated>
+    </task>
+    <task id="LOCAL-00063" summary="add support for inclusion of configs">
+      <created>1688714885616</created>
+      <option name="number" value="00063"/>
+      <option name="presentableId" value="LOCAL-00063"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1688714885617</updated>
+    </task>
+    <task id="LOCAL-00064" summary="support &lt;&lt;: inclusion">
+      <created>1689089769805</created>
+      <option name="number" value="00064"/>
+      <option name="presentableId" value="LOCAL-00064"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1689089769805</updated>
+    </task>
+    <option name="localTasksCounter" value="65"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -545,19 +552,14 @@
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="strawman choice type"/>
-    <MESSAGE value="add decorator"/>
-    <MESSAGE value="encode/decode choice types, add tests"/>
-    <MESSAGE value="add docs, expose __init__"/>
-    <MESSAGE value="rename, add demo"/>
     <MESSAGE value="stupid"/>
     <MESSAGE value="wip choice wrappers"/>
     <MESSAGE value="test_enums.py"/>
     <MESSAGE value="argparsing for simple closed choice types seems to work"/>
     <MESSAGE value="wip fixing help"/>
     <MESSAGE value="fix help for choice_types (and unbreak for everything else)"/>
     <MESSAGE value="older python didn't have exit_on_error"/>
@@ -570,15 +572,20 @@
     <MESSAGE value="make pytest ignore the test plugins dir to not confuse the registration"/>
     <MESSAGE value="sigh"/>
     <MESSAGE value="add project urls for draccus"/>
     <MESSAGE value="ultimately unnecessary, but it works"/>
     <MESSAGE value="add preliminary support for dataclass lists"/>
     <MESSAGE value="fix merging of int keys"/>
     <MESSAGE value="improve exceptions when something goes wrong"/>
-    <option name="LAST_COMMIT_MESSAGE" value="improve exceptions when something goes wrong"/>
+    <MESSAGE value="missed a dep"/>
+    <MESSAGE value="add !include for yaml"/>
+    <MESSAGE value="add basic docs for inclusion"/>
+    <MESSAGE value="add support for inclusion of configs"/>
+    <MESSAGE value="support &lt;&lt;: inclusion"/>
+    <option name="LAST_COMMIT_MESSAGE" value="support &lt;&lt;: inclusion"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/draccus/parsers/decoding.py</url>
           <line>101</line>
@@ -591,43 +598,77 @@
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/draccus/choice_types.py</url>
           <line>104</line>
           <option name="timeStamp" value="29"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/draccus/parsers/config_parsers.py</url>
-          <line>33</line>
-          <option name="timeStamp" value="31"/>
-        </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_lists.py</url>
           <line>103</line>
           <option name="timeStamp" value="32"/>
         </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file:///opt/homebrew/Caskroom/miniforge/base/envs/levanter/lib/python3.10/site-packages/yaml/scanner.py</url>
+          <line>576</line>
+          <option name="timeStamp" value="36"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file:///opt/homebrew/Caskroom/miniforge/base/envs/levanter/lib/python3.10/site-packages/yaml/parser.py</url>
+          <line>170</line>
+          <option name="timeStamp" value="40"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file:///opt/homebrew/Caskroom/miniforge/base/envs/levanter/lib/python3.10/site-packages/yaml/constructor.py</url>
+          <line>205</line>
+          <option name="timeStamp" value="41"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file:///opt/homebrew/Caskroom/miniforge/base/envs/levanter/lib/python3.10/site-packages/yaml/resolver.py</url>
+          <line>100</line>
+          <option name="timeStamp" value="44"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/draccus/parsers/yaml_loader.py</url>
+          <line>52</line>
+          <option name="timeStamp" value="49"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/draccus/parsers/yaml_loader.py</url>
+          <line>22</line>
+          <option name="timeStamp" value="55"/>
+        </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
+    <watches-manager>
+      <configuration name="tests">
+        <watch expression="self.buffer" language="Python"/>
+        <watch expression="self.buffer[self.pointer]" language="Python"/>
+        <watch expression="self.tokens" language="Python"/>
+      </configuration>
+    </watches-manager>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_base_test_basic_required_argument.coverage" NAME="pytest for tests.test_base.test_basic_required_argument Coverage Results" MODIFIED="1687463263242" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_types_test_class_registry.coverage" NAME="pytest for test_choice_types.test_class_registry Coverage Results" MODIFIED="1687504378733" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_collection_no_type.coverage" NAME="pytest for tests.test_lists.test_collection_no_type Coverage Results" MODIFIED="1688060693847" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_bools_test_bool_doesnt_parse_non_bools.coverage" NAME="pytest for tests.test_bools.test_bool_doesnt_parse_non_bools Coverage Results" MODIFIED="1687457197879" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_tuples_test_each_type_is_used_correctly.coverage" NAME="pytest for tests.test_tuples.test_each_type_is_used_correctly Coverage Results" MODIFIED="1687460314264" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_yaml_inclusion_test_load_hyperparameters_with_include.coverage" NAME="pytest for tests.test_yaml_inclusion.test_load_hyperparameters_with_include Coverage Results" MODIFIED="1688625535749" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_types_test_class_registry_decode.coverage" NAME="pytest for test_choice_types.test_class_registry_decode Coverage Results" MODIFIED="1687504658088" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_inheritance_test_subclasses_with_same_base_class_with_args.coverage" NAME="pytest for tests.test_inheritance.test_subclasses_with_same_base_class_with_args Coverage Results" MODIFIED="1687554125735" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_test_choice_registry_argparse.coverage" NAME="pytest for tests.test_argparse_choice_types.test_choice_registry_argparse Coverage Results" MODIFIED="1687566492053" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_plugin_test_plugin_registry_argparse.coverage" NAME="pytest for tests.test_argparse_choice_types_plugin.test_plugin_registry_argparse Coverage Results" MODIFIED="1687760916671" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_test_passing_enum_to_choice.coverage" NAME="pytest for tests.test_enums.test_passing_enum_to_choice Coverage Results" MODIFIED="1687554307878" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_list_one_element.coverage" NAME="pytest for tests.test_lists.test_list_one_element Coverage Results" MODIFIED="1687554263882" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_plugin_test_choice_registry_examine_help.coverage" NAME="pytest for tests.test_argparse_choice_types_plugin.test_choice_registry_examine_help Coverage Results" MODIFIED="1687760920532" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$choice_class_demo.coverage" NAME="choice_class_demo Coverage Results" MODIFIED="1687505257500" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/examples"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_optional_test_optional_parameter_group.coverage" NAME="pytest for test_optional.test_optional_parameter_group Coverage Results" MODIFIED="1688020223360" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_collection_no_type__1_.coverage" NAME="pytest for tests.test_lists.test_collection_no_type (1) Coverage Results" MODIFIED="1688062023358" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_lists_test_list_of_dataclasses.coverage" NAME="pytest for tests.test_lists.test_list_of_dataclasses Coverage Results" MODIFIED="1688063356342" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_argparse_choice_types_test_choice_registry_examine_help.coverage" NAME="pytest for tests.test_argparse_choice_types.test_choice_registry_examine_help Coverage Results" MODIFIED="1687594973111" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/draccus$pytest_for_test_yaml_inclusion_test_merge_include_hyperparameters.coverage" NAME="pytest for test_yaml_inclusion.test_merge_include_hyperparameters Coverage Results" MODIFIED="1689089538819" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_optional_test_optional_seed.coverage" NAME="pytest for test_optional.test_optional_seed Coverage Results" MODIFIED="1687463071605" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_tests_test_bools_test_bool_attributes_work.coverage" NAME="pytest for tests.test_bools.test_bool_attributes_work Coverage Results" MODIFIED="1687457200730" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_in_test_argparse_choice_types_plugin_py.coverage" NAME="pytest in test_argparse_choice_types_plugin.py Coverage Results" MODIFIED="1687670438197" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/draccus$pytest_for_test_choice_types_test_choice_registry_encode.coverage" NAME="pytest for test_choice_types.test_choice_registry_encode Coverage Results" MODIFIED="1687504823786" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
   </component>
 </project>
```

### Comparing `draccus-0.4.2/.idea/inspectionProfiles/Project_Default.xml` & `draccus-0.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/docs/api.md` & `draccus-0.6/docs/api.md`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/docs/argparse2pyrallis.gif` & `draccus-0.6/docs/argparse2pyrallis.gif`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/docs/index.md` & `draccus-0.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/docs/step_by_step.md` & `draccus-0.6/docs/step_by_step.md`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/argparsing.py` & `draccus-0.6/draccus/argparsing.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/cfgparsing.py` & `draccus-0.6/draccus/cfgparsing.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/choice_types.py` & `draccus-0.6/draccus/choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/fields.py` & `draccus-0.6/draccus/fields.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/help_formatter.py` & `draccus-0.6/draccus/help_formatter.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/options.py` & `draccus-0.6/draccus/options.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/utils.py` & `draccus-0.6/draccus/utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/parsers/config_parsers.py` & `draccus-0.6/draccus/parsers/config_parsers.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,21 +27,25 @@
 
 
 class YAMLParser(Parser):
     @staticmethod
     def parse_string(s):
         import yaml  # type: ignore
 
-        return yaml.safe_load(s)
+        from .yaml_loader import SafeLoaderWithInclusion
+
+        return yaml.load(s, SafeLoaderWithInclusion)
 
     @staticmethod
     def load_config(stream):
         import yaml  # type: ignore
 
-        return yaml.full_load(stream)
+        from .yaml_loader import FullLoaderWithInclusion
+
+        return yaml.load(stream, FullLoaderWithInclusion)
 
     @staticmethod
     def save_config(d, stream=None, **kwargs):
         import yaml
 
         return yaml.dump(d, stream, **kwargs)
```

### Comparing `draccus-0.4.2/draccus/parsers/decoding.py` & `draccus-0.6/draccus/parsers/decoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/parsers/encoding.py` & `draccus-0.6/draccus/parsers/encoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/parsers/registry_utils.py` & `draccus-0.6/draccus/parsers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/wrappers/choice_wrapper.py` & `draccus-0.6/draccus/wrappers/choice_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/wrappers/dataclass_wrapper.py` & `draccus-0.6/draccus/wrappers/dataclass_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/wrappers/docstring.py` & `draccus-0.6/draccus/wrappers/docstring.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/wrappers/field_metavar.py` & `draccus-0.6/draccus/wrappers/field_metavar.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/wrappers/field_wrapper.py` & `draccus-0.6/draccus/wrappers/field_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/wrappers/suppressing_argparse.py` & `draccus-0.6/draccus/wrappers/suppressing_argparse.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/draccus/wrappers/wrapper.py` & `draccus-0.6/draccus/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/examples/choice_class_demo.py` & `draccus-0.6/examples/choice_class_demo.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/examples/demo.py` & `draccus-0.6/examples/demo.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/conftest.py` & `draccus-0.6/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import logging
 from dataclasses import dataclass, field
-from typing import *
+from enum import Enum
+from typing import Any, ClassVar, List, Optional, Tuple, Type
 
 import pytest
 
 from .testutils import TestSetup
 
 
-# from draccus import choice
-# from draccus.helpers import Serializable
-
 # List of simple attributes to use in tests:
 simple_arguments: List[Tuple[Type, Any, Any]] = [
     # type, passed value, expected (parsed) value
     (int, "123", 123),
     (int, 123, 123),
     (int, "-1", -1),
     (float, "123.0", 123.0),
@@ -42,15 +40,15 @@
 
 
 @pytest.fixture
 def assert_equals_stdout(capsys):
     def strip(string):
         return "".join(string.split())
 
-    def should_equal(expected: str, file_path: str = None):
+    def should_equal(expected: str, file_path: Optional[str] = None):
         out = capsys.readouterr().out
         assert strip(out) == strip(expected), file_path
 
     return should_equal
 
 
 @pytest.fixture
@@ -129,22 +127,21 @@
         # Whether or not a task-specific Embedding layer should be used on the 'likes' features.
         # When set to 'True', it is expected that there no shared embedding is used.
         embed_likes: bool = False
 
     return TaskHyperParameters
 
 
-@pytest.fixture
-def HyperParameters(TaskHyperParameters):
-    from enum import Enum
+class Optimizers(Enum):
+    ADAM = "ADAM"
+    SGD = "SGD"
 
-    class Optimizers(Enum):
-        ADAM = "ADAM"
-        SGD = "SGD"
 
+@pytest.fixture
+def HyperParameters(TaskHyperParameters):
     @dataclass
     class HyperParameters(TestSetup):
         """Hyperparameters of a multi-headed model."""
 
         batch_size: int = 128  # the batch size
         learning_rate: float = 0.001  # Learning Rate
         optimizer: Optimizers = Optimizers.SGD  # Which optimizer to use during training.
```

### Comparing `draccus-0.4.2/tests/test_argparse_choice_types.py` & `draccus-0.6/tests/test_argparse_choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_argparse_choice_types_plugin.py` & `draccus-0.6/tests/test_argparse_choice_types_plugin.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_base.py` & `draccus-0.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_bools.py` & `draccus-0.6/tests/test_bools.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_choice_types.py` & `draccus-0.6/tests/test_choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_decoding.py` & `draccus-0.6/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_default_args.py` & `draccus-0.6/tests/test_default_args.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_docstrings.py` & `draccus-0.6/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_enums.py` & `draccus-0.6/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_inheritance.py` & `draccus-0.6/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_lists.py` & `draccus-0.6/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_optional.py` & `draccus-0.6/tests/test_optional.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_tuples.py` & `draccus-0.6/tests/test_tuples.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/test_utils.py` & `draccus-0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/tests/testutils.py` & `draccus-0.6/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/.gitignore` & `draccus-0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/LICENSE` & `draccus-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `draccus-0.4.2/README.md` & `draccus-0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 
 > Draccus: “a large herbivorous reptilian creature, known for their ability to breathe fire.”
 
 Draccus is a fork of the excellent [Pyrallis](https://github.com/eladrich/pyrallis) library, but with
 a few changes to make it more suitable for my use cases. The main changes are:
 
 * Support for subtyping configs (that is, choosing between different configs based on a parameter)
-* WIP: Support for including config files in config files
+* Support for including config files in config files
 * Better support for containers of configs (e.g. a list of configs)
 * Couple of bug fixes
 
 I swear I didn't want to fork it, but the Pyrallis devs (understandably) didn't want to merge some of
 these.
 
 
 <p align="center"><img src="https://github.com/eladrich/pyrallis/raw/master/docs/argparse2pyrallis.gif" alt="GIF" width="100%" /></p>
 
 ## Why `draccus`?
 
 We support everything in Pyrallis (see their examples), but also support subtyping and including config files in config files.
-We still try to maintain their simple, clean
+We still try to maintain their simple, clean YAML-focused approach.
 
 With `draccus` your configuration is linked directly to your pre-defined `dataclass`, allowing you to easily create different configuration structures, including nested ones, using an object-oriented design. The parsed arguments are used to initialize your `dataclass`, giving you the typing hints and automatic code completion of a full `dataclass` object.
 
 
 ## My First Draccus Example
 
 (This example is the same as in Pyrallis. Draccus differs mainly in advanced features like subtyping.)
@@ -77,16 +77,59 @@
   type: bert
   num_layers: 24
   num_heads: 24
   hidden_size: 1024
   dropout: 0.2
 ```
 
+## Inclusion of Config Files
+
+(This is a difference from Pyrallis.)
+
+We support including config files from other config files via [pyyaml-include](https://github.com/tanbro/pyyaml-include).
+This is useful for splitting up your config into multiple files, or for including a base config file in your config.
+
+It works like this:
+
+```yaml
+# model_config.yaml
+type: bert
+num_layers: 24
+num_heads: 24
+hidden_size: 1024
+dropout: 0.2
+```
+
+```yaml
+# train_config.yaml
+exp_name: my_yaml_exp
+workers: 42
+model: !include model_config.yaml
+```
+
+### Including Configs at Top Level
+
+PyYAML, upon which draccus is based, supports a common YAML extension `<<` for merging keys from multiple maps. We can combine this with `!include` to include a config file:
+
+```yaml
+# base_config.yaml
+type: bert
+lr: 0.001
+
+# train_config.yaml
+<<: !include base_config.yaml
+exp_name: my_yaml_exp
+```
+
+(I don't love this syntax, but it's consistent with PyYAML.)
+
 ## More Flexible Configuration with Choice Types
 
+(This is a difference from Pyrallis.)
+
 Choice Types, aka "Sum Types" or "Tagged Unions", are a powerful way to define a choice of types that can be selected at
 runtime. For instance, you might want to choose what kind of model to train, or what kind of optimizer to use.
 
 Draccus provides a `ChoiceRegistry` class that lets you define a choice of types that can be selected at runtime. You
 can then use the `register_subclass` decorator to register a subclass of your choice type. The `type` field of the
 choice type is used to select the subclass.
```

### Comparing `draccus-0.4.2/pyproject.toml` & `draccus-0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "draccus"
-version = "0.4.2"
+version = "0.6"
 authors = [
   { name="David Hall", email="dlwh@cs.stanford.edu" },
     { name="Sidd Karamcheti"},
 ]
 description = "A framework for simple dataclass-based configurations."
 readme = "README.md"
 requires-python = ">=3.6"
@@ -18,15 +18,16 @@
 "License :: OSI Approved :: MIT License",
 "Operating System :: OS Independent",
 ]
 dependencies = [
   "typing-inspect>=0.9.0",
   "dataclasses; python_version < '3.7'",
   "pyyaml",
-  "mergedeep"
+  "mergedeep",
+  "pyyaml-include>=1.3"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dlwh/draccus"
 "Bug Tracker" = "https://github.com/dlwh/draccus/issues"
 
 [tool.hatch.extras]
```

### Comparing `draccus-0.4.2/PKG-INFO` & `draccus-0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: draccus
-Version: 0.4.2
+Version: 0.6
 Summary: A framework for simple dataclass-based configurations.
 Project-URL: Homepage, https://github.com/dlwh/draccus
 Project-URL: Bug Tracker, https://github.com/dlwh/draccus/issues
 Author: Sidd Karamcheti
 Author-email: David Hall <dlwh@cs.stanford.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: dataclasses; python_version < '3.7'
 Requires-Dist: mergedeep
 Requires-Dist: pyyaml
+Requires-Dist: pyyaml-include>=1.3
 Requires-Dist: typing-inspect>=0.9.0
 Description-Content-Type: text/markdown
 
 <!--
 <p align="center"><img src="https://raw.githubusercontent.com/eladrich/pyrallis/master/docs/pyrallis_logo.png" alt="logo" width="70%" /></p>
 
 <p align="center">
@@ -34,28 +35,28 @@
 
 > Draccus: “a large herbivorous reptilian creature, known for their ability to breathe fire.”
 
 Draccus is a fork of the excellent [Pyrallis](https://github.com/eladrich/pyrallis) library, but with
 a few changes to make it more suitable for my use cases. The main changes are:
 
 * Support for subtyping configs (that is, choosing between different configs based on a parameter)
-* WIP: Support for including config files in config files
+* Support for including config files in config files
 * Better support for containers of configs (e.g. a list of configs)
 * Couple of bug fixes
 
 I swear I didn't want to fork it, but the Pyrallis devs (understandably) didn't want to merge some of
 these.
 
 
 <p align="center"><img src="https://github.com/eladrich/pyrallis/raw/master/docs/argparse2pyrallis.gif" alt="GIF" width="100%" /></p>
 
 ## Why `draccus`?
 
 We support everything in Pyrallis (see their examples), but also support subtyping and including config files in config files.
-We still try to maintain their simple, clean
+We still try to maintain their simple, clean YAML-focused approach.
 
 With `draccus` your configuration is linked directly to your pre-defined `dataclass`, allowing you to easily create different configuration structures, including nested ones, using an object-oriented design. The parsed arguments are used to initialize your `dataclass`, giving you the typing hints and automatic code completion of a full `dataclass` object.
 
 
 ## My First Draccus Example
 
 (This example is the same as in Pyrallis. Draccus differs mainly in advanced features like subtyping.)
@@ -96,16 +97,59 @@
   type: bert
   num_layers: 24
   num_heads: 24
   hidden_size: 1024
   dropout: 0.2
 ```
 
+## Inclusion of Config Files
+
+(This is a difference from Pyrallis.)
+
+We support including config files from other config files via [pyyaml-include](https://github.com/tanbro/pyyaml-include).
+This is useful for splitting up your config into multiple files, or for including a base config file in your config.
+
+It works like this:
+
+```yaml
+# model_config.yaml
+type: bert
+num_layers: 24
+num_heads: 24
+hidden_size: 1024
+dropout: 0.2
+```
+
+```yaml
+# train_config.yaml
+exp_name: my_yaml_exp
+workers: 42
+model: !include model_config.yaml
+```
+
+### Including Configs at Top Level
+
+PyYAML, upon which draccus is based, supports a common YAML extension `<<` for merging keys from multiple maps. We can combine this with `!include` to include a config file:
+
+```yaml
+# base_config.yaml
+type: bert
+lr: 0.001
+
+# train_config.yaml
+<<: !include base_config.yaml
+exp_name: my_yaml_exp
+```
+
+(I don't love this syntax, but it's consistent with PyYAML.)
+
 ## More Flexible Configuration with Choice Types
 
+(This is a difference from Pyrallis.)
+
 Choice Types, aka "Sum Types" or "Tagged Unions", are a powerful way to define a choice of types that can be selected at
 runtime. For instance, you might want to choose what kind of model to train, or what kind of optimizer to use.
 
 Draccus provides a `ChoiceRegistry` class that lets you define a choice of types that can be selected at runtime. You
 can then use the `register_subclass` decorator to register a subclass of your choice type. The `type` field of the
 choice type is used to select the subclass.
```

