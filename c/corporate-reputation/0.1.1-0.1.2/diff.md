# Comparing `tmp/corporate_reputation-0.1.1.tar.gz` & `tmp/corporate_reputation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corporate_reputation-0.1.1.tar", max compression
+gzip compressed data, was "corporate_reputation-0.1.2.tar", max compression
```

## Comparing `corporate_reputation-0.1.1.tar` & `corporate_reputation-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,51 @@
--rw-r--r--   0        0        0     1071 2023-06-28 04:25:54.597139 corporate_reputation-0.1.1/LICENSE
--rw-r--r--   0        0        0     3914 2023-06-28 04:25:54.597139 corporate_reputation-0.1.1/README.md
--rw-r--r--   0        0        0     3031 2023-06-28 04:26:19.373581 corporate_reputation-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      288 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/__cli__.py
--rw-r--r--   0        0        0      379 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/__init__.py
--rw-r--r--   0        0        0       22 2023-06-28 04:26:19.317580 corporate_reputation-0.1.1/src/corprep/_version.py
--rw-r--r--   0        0        0        0 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/__init__.py
--rw-r--r--   0        0        0      338 2023-06-28 04:26:19.321580 corporate_reputation-0.1.1/src/corprep/conf/about/__init__.yaml
--rw-r--r--   0        0        0      435 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/module/__init__.yaml
--rw-r--r--   0        0        0       96 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/path/__batch__.yaml
--rw-r--r--   0        0        0     1719 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/path/__init__.yaml
--rw-r--r--   0        0        0      412 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/path/__task__.yaml
--rw-r--r--   0        0        0       76 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       72 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       74 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0      119 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      237 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      242 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       92 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       19 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/pipeline/__test__.yaml
--rw-r--r--   0        0        0      742 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/project/__init__.yaml
--rw-r--r--   0        0        0      168 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/project/__test__.yaml
--rw-r--r--   0        0        0       36 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/running/__init__.yaml
--rw-r--r--   0        0        0      176 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      319 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/task/__init__.yaml
--rw-r--r--   0        0        0      311 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/task/__test__.yaml
--rw-r--r--   0        0        0       97 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       97 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0        0 2023-06-28 04:25:54.601139 corporate_reputation-0.1.1/src/corprep/py.typed
--rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 corporate_reputation-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-11 02:40:48.250285 corporate_reputation-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3912 2023-07-11 02:40:48.250285 corporate_reputation-0.1.2/README.md
+-rw-r--r--   0        0        0     3030 2023-07-11 02:41:12.890581 corporate_reputation-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/__cli__.py
+-rw-r--r--   0        0        0      379 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-11 02:41:12.834580 corporate_reputation-0.1.2/src/corprep/_version.py
+-rw-r--r--   0        0        0        0 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/__init__.py
+-rw-r--r--   0        0        0      338 2023-07-11 02:41:12.834580 corporate_reputation-0.1.2/src/corprep/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      553 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      901 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      880 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      291 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipeline/__test__.yaml
+-rw-r--r--   0        0        0      388 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      185 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      161 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      305 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      208 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/task/__test__.yaml
+-rw-r--r--   0        0        0      114 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0      113 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0        0 2023-07-11 02:40:48.254285 corporate_reputation-0.1.2/src/corprep/py.typed
+-rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 corporate_reputation-0.1.2/PKG-INFO
```

### Comparing `corporate_reputation-0.1.1/LICENSE` & `corporate_reputation-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.1.1/README.md` & `corporate_reputation-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
 [![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
-[codecov-image]: https://codecov.io/gh/entelecheia/corporate-reputation/branch/main/graph/badge.svg?token=[REPLACE_ME]
+[codecov-image]: https://codecov.io/gh/entelecheia/corporate-reputation/branch/main/graph/badge.svg?token=5QP39SFTGR
 [codecov-url]: https://codecov.io/gh/entelecheia/corporate-reputation
 [pypi-image]: https://img.shields.io/pypi/v/corporate-reputation
 [license-image]: https://img.shields.io/github/license/entelecheia/corporate-reputation
 [license-url]: https://github.com/entelecheia/corporate-reputation/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/corporate-reputation?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/corporate-reputation
 [release-url]: https://github.com/entelecheia/corporate-reputation/releases
```

### Comparing `corporate_reputation-0.1.1/pyproject.toml` & `corporate_reputation-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "corporate-reputation"
-version = "0.1.1"
+version = "0.1.2"
 description = "Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/corporate-reputation"
 repository = "https://github.com/entelecheia/corporate-reputation"
 readme = "README.md"
 packages = [{ include = "corprep", from = "src" }]
 
 [tool.poetry.scripts]
 corprep = 'corprep.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.15.0"
+hyfi = "^1.2.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `corporate_reputation-0.1.1/src/corprep/conf/copier/conf.yaml` & `corporate_reputation-0.1.2/src/corprep/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.1.1/src/corprep/conf/dotenv/__init__.yaml` & `corporate_reputation-0.1.2/src/corprep/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.1.1/src/corprep/conf/hydra/help/help.yaml` & `corporate_reputation-0.1.2/src/corprep/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.1.1/src/corprep/conf/mode/__init__.yaml` & `corporate_reputation-0.1.2/src/corprep/conf/mode/__init__.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # @package _global_
 debug_mode: false
-print_config: false
 resolve: true
 verbose: false
 ignore_warnings: true
 logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
 hydra_log_dir: ${oc.select:project.path.project_logs, ${oc.select:task.path.task_logs, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}/logs}}/hydra
 
 hydra:
```

### Comparing `corporate_reputation-0.1.1/src/corprep/conf/project/__init__.yaml` & `corporate_reputation-0.1.2/src/corprep/conf/project/__init__.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 defaults:
   - /dotenv: __init__
   - /joblib: __init__
   - /path: __init__
 
-config_name: __init__
+_config_name_: __init__
 project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}
 project_description: ${oc.env:HYFI_PROJECT_DESC,""}
 project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${.global_hyfi_root}/${.global_workspace_name}/projects/${.project_name}}
 project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}
 global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}
 global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}
 num_workers: ${oc.env:HYFI_NUM_WORKERS,1}
```

### Comparing `corporate_reputation-0.1.1/PKG-INFO` & `corporate_reputation-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: corporate-reputation
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling
 Home-page: https://entelecheia.github.io/corporate-reputation
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.15.0,<0.16.0)
+Requires-Dist: hyfi (>=1.2.2,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/corporate-reputation
 Description-Content-Type: text/markdown
 
 # Reputation Analysis of Companies and CEOs
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
 [![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
-[codecov-image]: https://codecov.io/gh/entelecheia/corporate-reputation/branch/main/graph/badge.svg?token=[REPLACE_ME]
+[codecov-image]: https://codecov.io/gh/entelecheia/corporate-reputation/branch/main/graph/badge.svg?token=5QP39SFTGR
 [codecov-url]: https://codecov.io/gh/entelecheia/corporate-reputation
 [pypi-image]: https://img.shields.io/pypi/v/corporate-reputation
 [license-image]: https://img.shields.io/github/license/entelecheia/corporate-reputation
 [license-url]: https://github.com/entelecheia/corporate-reputation/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/corporate-reputation?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/corporate-reputation
 [release-url]: https://github.com/entelecheia/corporate-reputation/releases
```

