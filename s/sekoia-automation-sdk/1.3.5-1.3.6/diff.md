# Comparing `tmp/sekoia_automation_sdk-1.3.5.tar.gz` & `tmp/sekoia_automation_sdk-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekoia_automation_sdk-1.3.5.tar", max compression
+gzip compressed data, was "sekoia_automation_sdk-1.3.6.tar", max compression
```

## Comparing `sekoia_automation_sdk-1.3.5.tar` & `sekoia_automation_sdk-1.3.6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-06-23 16:44:27.531147 sekoia_automation_sdk-1.3.5/LICENSE
--rw-r--r--   0        0        0     8422 2023-06-23 16:44:27.531147 sekoia_automation_sdk-1.3.5/README.md
--rw-r--r--   0        0        0     2114 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/__init__.py
--rw-r--r--   0        0        0    11420 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/action.py
--rw-r--r--   0        0        0     5193 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/cli.py
--rw-r--r--   0        0        0      548 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/config.py
--rw-r--r--   0        0        0     6955 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/connector/__init__.py
--rw-r--r--   0        0        0     2313 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/connector/workers.py
--rw-r--r--   0        0        0      426 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/constants.py
--rw-r--r--   0        0        0      869 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/exceptions.py
--rw-r--r--   0        0        0      399 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/metrics/__init__.py
--rw-r--r--   0        0        0      383 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/metrics/base.py
--rw-r--r--   0        0        0     1185 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/metrics/prometheus.py
--rw-r--r--   0        0        0    15640 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/module.py
--rw-r--r--   0        0        0        0 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/__init__.py
--rw-r--r--   0        0        0     6605 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/documentation/generate.py
--rw-r--r--   0        0        0     2669 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/documentation/templates/module.md
--rw-r--r--   0        0        0     7581 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/files_generator.py
--rw-r--r--   0        0        0      144 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/cookiecutter.json
--rw-r--r--   0        0        0      301 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
--rw-r--r--   0        0        0      225 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
--rw-r--r--   0        0        0      417 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
--rw-r--r--   0        0        0      596 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
--rw-r--r--   0        0        0      358 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
--rw-r--r--   0        0        0      140 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
--rw-r--r--   0        0        0    10011 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/openapi.py
--rwxr-xr-x   0        0        0    13709 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/sync_library.py
--rw-r--r--   0        0        0     6094 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/storage.py
--rw-r--r--   0        0        0    14583 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/trigger.py
--rw-r--r--   0        0        0     1294 2023-06-23 16:44:27.535147 sekoia_automation_sdk-1.3.5/sekoia_automation/utils.py
--rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/LICENSE
+-rw-r--r--   0        0        0     8422 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/README.md
+-rw-r--r--   0        0        0     2114 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/__init__.py
+-rw-r--r--   0        0        0    11420 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/action.py
+-rw-r--r--   0        0        0     5477 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/cli.py
+-rw-r--r--   0        0        0      548 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/config.py
+-rw-r--r--   0        0        0     6998 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/connector/__init__.py
+-rw-r--r--   0        0        0     2313 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/connector/workers.py
+-rw-r--r--   0        0        0      426 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/constants.py
+-rw-r--r--   0        0        0      869 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/exceptions.py
+-rw-r--r--   0        0        0      399 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/metrics/__init__.py
+-rw-r--r--   0        0        0      383 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/metrics/base.py
+-rw-r--r--   0        0        0     1185 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/metrics/prometheus.py
+-rw-r--r--   0        0        0    15640 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/module.py
+-rw-r--r--   0        0        0        0 2023-07-11 11:06:19.013614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/__init__.py
+-rw-r--r--   0        0        0     6605 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/documentation/generate.py
+-rw-r--r--   0        0        0     2669 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/documentation/templates/module.md
+-rw-r--r--   0        0        0     7581 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/files_generator.py
+-rw-r--r--   0        0        0      144 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/cookiecutter.json
+-rw-r--r--   0        0        0      301 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
+-rw-r--r--   0        0        0      225 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
+-rw-r--r--   0        0        0      417 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
+-rw-r--r--   0        0        0      596 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
+-rw-r--r--   0        0        0      358 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
+-rw-r--r--   0        0        0      140 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
+-rw-r--r--   0        0        0    10011 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/openapi.py
+-rwxr-xr-x   0        0        0    13709 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/sync_library.py
+-rw-r--r--   0        0        0     2089 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/update_sdk_version.py
+-rw-r--r--   0        0        0     6094 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/storage.py
+-rw-r--r--   0        0        0    14583 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/trigger.py
+-rw-r--r--   0        0        0     1294 2023-07-11 11:06:19.017614 sekoia_automation_sdk-1.3.6/sekoia_automation/utils.py
+-rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.6/PKG-INFO
```

### Comparing `sekoia_automation_sdk-1.3.5/LICENSE` & `sekoia_automation_sdk-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/README.md` & `sekoia_automation_sdk-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/pyproject.toml` & `sekoia_automation_sdk-1.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sekoia-automation-sdk"
 
-version = "1.3.5"
+version = "1.3.6"
 description = "SDK to create SEKOIA.IO playbook modules"
 license = "MIT"
 readme = "README.md"
 authors = ["SEKOIA.IO"]
 packages = [
     { include = "sekoia_automation" },
 ]
```

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/action.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/action.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/cli.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from sekoia_automation.scripts.documentation.generate import (
     DocumentationGenerator,
 )
 from sekoia_automation.scripts.files_generator import FilesGenerator
 from sekoia_automation.scripts.openapi import OpenApiToModule
 from sekoia_automation.scripts.sync_library import SyncLibrary
+from sekoia_automation.scripts.update_sdk_version import SDKUpdater
 
 app = typer.Typer(
     help="SEKOIA.IO's automation helper to generate playbook modules",
     rich_markup_mode="markdown",
 )
 OptionalPath = Optional[Path]  # noqa: UP007
 OptionalStr = Optional[str]  # noqa: UP007
@@ -171,9 +172,16 @@
         registry_check=check_image_on_registry,
         registry=registry,
         namespace=namespace,
         registry_pat=registry_pat,
     ).execute()
 
 
+@app.command(name="update-sdk-version")
+def update_sekoia_library(
+    modules_path: Path = typer.Option(".", help="Path to the playbook modules"),
+):
+    SDKUpdater(modules_path=modules_path).update_sdk_version()
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/config.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/connector/__init__.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/connector/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
                 with attempt:
                     res: Response = requests.post(
                         batch_api,
                         json=request_body,
                         headers={"User-Agent": self.__connector_user_agent},
                         timeout=30,
                     )
+                    res.raise_for_status()
             if res.status_code > 299:
                 self.log(f"Intake rejected events: {res.text}", level="error")
                 res.raise_for_status()
             collect_ids[chunk_index] = res.json().get("event_ids", [])
         except Exception as ex:
             self.log_exception(ex, message=f"Failed to forward {len(chunk)} events")
```

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/connector/workers.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/connector/workers.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/exceptions.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/exceptions.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/metrics/prometheus.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/module.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/module.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/documentation/generate.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/documentation/generate.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/documentation/templates/module.md` & `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/documentation/templates/module.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/files_generator.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/files_generator.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml` & `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "SEKOIA's automation module for {{cookiecutter.module_name.capitalize()}}"
 version = "0.0"
 description = ""
 authors = []
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.11"
+python = ">=3.10,<3.12"
 sekoia-automation-sdk = "^1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-cov = "*"
 requests = "*"
 requests-mock = "*"
```

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/openapi.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/openapi.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/scripts/sync_library.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/scripts/sync_library.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/storage.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/storage.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/trigger.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/trigger.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/sekoia_automation/utils.py` & `sekoia_automation_sdk-1.3.6/sekoia_automation/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.5/PKG-INFO` & `sekoia_automation_sdk-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekoia-automation-sdk
-Version: 1.3.5
+Version: 1.3.6
 Summary: SDK to create SEKOIA.IO playbook modules
 Home-page: https://sekoia.io/
 License: MIT
 Keywords: SDK,SEKOIA.IO,automation,playbook
 Author: SEKOIA.IO
 Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
```

