# Comparing `tmp/dkist-processing-core-2.0.2.tar.gz` & `tmp/dkist-processing-core-2.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-core-2.0.2.tar", last modified: Tue Jul 11 17:34:58 2023, max compression
+gzip compressed data, was "dkist-processing-core-2.0.2rc1.tar", last modified: Tue Jul 11 15:38:11 2023, max compression
```

## Comparing `dkist-processing-core-2.0.2.tar` & `dkist-processing-core-2.0.2rc1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 17:34:58.331119 dkist-processing-core-2.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     2448 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     3935 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     7533 2023-07-11 17:34:58.331119 dkist-processing-core-2.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6922 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 17:34:58.327119 dkist-processing-core-2.0.2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      436 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 17:34:58.327119 dkist-processing-core-2.0.2/dkist_processing_core/
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3272 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/_failure_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2992 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/build_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9936 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/task.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 17:34:58.327119 dkist-processing-core-2.0.2/dkist_processing_core/tests/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 17:34:58.331119 dkist-processing-core-2.0.2/dkist_processing_core/tests/invalid_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/invalid_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/invalid_workflow_package/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/task_example.py
--rw-rw-rw-   0 root         (0) root         (0)     1637 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/test_build_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/test_export.py
--rw-rw-rw-   0 root         (0) root         (0)     4041 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/test_failure_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     3983 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/test_workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 17:34:58.331119 dkist-processing-core-2.0.2/dkist_processing_core/tests/valid_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/valid_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/valid_workflow_package/workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 17:34:58.331119 dkist-processing-core-2.0.2/dkist_processing_core/tests/zero_node_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/zero_node_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/tests/zero_node_workflow_package/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     8723 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/dkist_processing_core/workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 17:34:58.327119 dkist-processing-core-2.0.2/dkist_processing_core.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7533 2023-07-11 17:34:58.000000 dkist-processing-core-2.0.2/dkist_processing_core.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-07-11 17:34:58.000000 dkist-processing-core-2.0.2/dkist_processing_core.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-11 17:34:58.000000 dkist-processing-core-2.0.2/dkist_processing_core.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-11 17:34:58.000000 dkist-processing-core-2.0.2/dkist_processing_core.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-11 17:34:58.000000 dkist-processing-core-2.0.2/dkist_processing_core.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 17:34:58.331119 dkist-processing-core-2.0.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    85295 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/docs/auto-proc-concept-model.png
--rw-rw-rw-   0 root         (0) root         (0)    26060 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/docs/auto_proc_brick.png
--rw-rw-rw-   0 root         (0) root         (0)   267222 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/docs/automated-processing-deployed.png
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1854 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 17:34:58.331119 dkist-processing-core-2.0.2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1294 2023-07-11 17:34:58.331119 dkist-processing-core-2.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-11 17:34:52.000000 dkist-processing-core-2.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 15:38:11.547919 dkist-processing-core-2.0.2rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2448 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3763 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7536 2023-07-11 15:38:11.547919 dkist-processing-core-2.0.2rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6922 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 15:38:11.543919 dkist-processing-core-2.0.2rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/changelog/21.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      436 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 15:38:11.543919 dkist-processing-core-2.0.2rc1/dkist_processing_core/
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3272 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/_failure_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2992 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/build_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9936 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/task.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 15:38:11.543919 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 15:38:11.543919 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/invalid_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/invalid_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/invalid_workflow_package/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/task_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_build_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     4041 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_failure_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3983 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 15:38:11.547919 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/valid_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/valid_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/valid_workflow_package/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 15:38:11.547919 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/zero_node_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/zero_node_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/zero_node_workflow_package/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     8723 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 15:38:11.543919 dkist-processing-core-2.0.2rc1/dkist_processing_core.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     7536 2023-07-11 15:38:11.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2023-07-11 15:38:11.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-11 15:38:11.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-11 15:38:11.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-11 15:38:11.000000 dkist-processing-core-2.0.2rc1/dkist_processing_core.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 15:38:11.547919 dkist-processing-core-2.0.2rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    85295 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/docs/auto-proc-concept-model.png
+-rw-rw-rw-   0 root         (0) root         (0)    26060 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/docs/auto_proc_brick.png
+-rw-rw-rw-   0 root         (0) root         (0)   267222 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/docs/automated-processing-deployed.png
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 15:38:11.547919 dkist-processing-core-2.0.2rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1294 2023-07-11 15:38:11.547919 dkist-processing-core-2.0.2rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-11 15:38:06.000000 dkist-processing-core-2.0.2rc1/setup.py
```

### Comparing `dkist-processing-core-2.0.2/.gitignore` & `dkist-processing-core-2.0.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/.pre-commit-config.yaml` & `dkist-processing-core-2.0.2rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/CHANGELOG.rst` & `dkist-processing-core-2.0.2rc1/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-v2.0.2 (2023-07-11)
-===================
-
-Misc
-----
-
-- Update airflow dependency to 2.6.3 (`#21 <https://bitbucket.org/dkistdc/dkist-processing-core/pull-requests/21>`__)
-
-
 v2.0.1 (2023-06-28)
 ===================
 
 Bugfixes
 --------
 
 - Update MAXIMUM_ALLOWED_WORKFLOW_NAME_LENGTH to be consistent with database (100 characters). (`#19 <https://bitbucket.org/dkistdc/dkist-processing-core/pull-requests/19>`__)
```

### Comparing `dkist-processing-core-2.0.2/PKG-INFO` & `dkist-processing-core-2.0.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-core
-Version: 2.0.2
+Version: 2.0.2rc1
 Summary: Abstraction layer that is used by the DKIST Science Data Processing pipelines to process DKIST data using Apache Airflow.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-core/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/core
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-core-2.0.2/README.rst` & `dkist-processing-core-2.0.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/bitbucket-pipelines.yml` & `dkist-processing-core-2.0.2rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/_failure_callback.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/_failure_callback.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/_node.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/_node.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/build_utils.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/build_utils.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/task.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/tests/conftest.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/tests/task_example.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/task_example.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/tests/test_build_utils.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_build_utils.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/tests/test_export.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/tests/test_failure_callback.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_failure_callback.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/tests/test_node.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/tests/test_task.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/tests/test_workflow.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/tests/valid_workflow_package/workflow.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/tests/valid_workflow_package/workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core/workflow.py` & `dkist-processing-core-2.0.2rc1/dkist_processing_core/workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core.egg-info/PKG-INFO` & `dkist-processing-core-2.0.2rc1/dkist_processing_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-core
-Version: 2.0.2
+Version: 2.0.2rc1
 Summary: Abstraction layer that is used by the DKIST Science Data Processing pipelines to process DKIST data using Apache Airflow.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-core/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/core
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-core-2.0.2/dkist_processing_core.egg-info/SOURCES.txt` & `dkist-processing-core-2.0.2rc1/dkist_processing_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
+changelog/21.misc.rst
 dkist_processing_core/__init__.py
 dkist_processing_core/_failure_callback.py
 dkist_processing_core/_node.py
 dkist_processing_core/build_utils.py
 dkist_processing_core/task.py
 dkist_processing_core/workflow.py
 dkist_processing_core.egg-info/PKG-INFO
```

### Comparing `dkist-processing-core-2.0.2/docs/Makefile` & `dkist-processing-core-2.0.2rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/docs/auto-proc-concept-model.png` & `dkist-processing-core-2.0.2rc1/docs/auto-proc-concept-model.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/docs/auto_proc_brick.png` & `dkist-processing-core-2.0.2rc1/docs/auto_proc_brick.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/docs/automated-processing-deployed.png` & `dkist-processing-core-2.0.2rc1/docs/automated-processing-deployed.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/docs/conf.py` & `dkist-processing-core-2.0.2rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/docs/make.bat` & `dkist-processing-core-2.0.2rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/licenses/LICENSE.rst` & `dkist-processing-core-2.0.2rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/pyproject.toml` & `dkist-processing-core-2.0.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-2.0.2/setup.cfg` & `dkist-processing-core-2.0.2rc1/setup.cfg`

 * *Files identical despite different names*

