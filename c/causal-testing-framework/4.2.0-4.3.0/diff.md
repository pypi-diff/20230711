# Comparing `tmp/causal_testing_framework-4.2.0.tar.gz` & `tmp/causal_testing_framework-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal_testing_framework-4.2.0.tar", last modified: Mon Jun 26 10:51:37 2023, max compression
+gzip compressed data, was "causal_testing_framework-4.3.0.tar", last modified: Tue Jul 11 10:18:34 2023, max compression
```

## Comparing `causal_testing_framework-4.2.0.tar` & `causal_testing_framework-4.3.0.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:37.001812 causal_testing_framework-4.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/workflows/lint-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.mega-linter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-26 10:51:37.001812 causal_testing_framework-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/causal_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/causal_testing/data_collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/data_collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/data_collection/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/causal_testing/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/generation/abstract_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/generation/enum_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/causal_testing/json_front/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/json_front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/json_front/json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/causal_testing/specification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26803 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/causal_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/metamorphic_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/causal_testing/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/causal_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    29468 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/intervention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/causal_testing/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-26 10:51:36.000000 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-26 10:51:36.000000 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:51:36.000000 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 10:51:36.000000 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 10:51:36.000000 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/dev/actions_and_webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/dev/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/dev/version_release.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/source/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/frontends/json_front_end.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/frontends/test_suite.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/glossary.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/modules/causal_specification.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/modules/causal_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/modules/data_collector.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.981812 causal_testing_framework-4.2.0/examples/covasim_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/example_beta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/dag.png
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/lr91/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/lr91/data/
--rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/data/normalised_results.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/data/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/example_max_conductances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/example_max_conductances_test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/poisson/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson/causal_tests.json
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson/example_run_causal_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/examples/poisson-line-process/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.981812 causal_testing_framework-4.2.0/examples/poisson-line-process/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/examples/poisson-line-process/data/random/
--rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/random/data_random_1000.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/example_poisson_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:51:37.001812 causal_testing_framework-4.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/data/nhefs.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/data_collection_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/data_collection_tests/test_observational_data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/generation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/generation_tests/test_abstract_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/json_front_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/json_front_tests/test_json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/resources/data/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/resources/data/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/resources/data/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/resources/data/data_with_meta.csv
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/resources/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:37.001812 causal_testing_framework-4.2.0/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/specification_tests/test_causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/specification_tests/test_metamorphic_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/specification_tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:37.001812 causal_testing_framework-4.2.0/tests/testing_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/testing_tests/test_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/workflows/lint-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.mega-linter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/causal_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/causal_testing/data_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/data_collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/data_collection/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/causal_testing/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/generation/abstract_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/generation/enum_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/causal_testing/json_front/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/json_front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/json_front/json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/causal_testing/specification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26885 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/causal_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/metamorphic_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/causal_testing/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/causal_test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/causal_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29865 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/intervention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/causal_testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 10:18:34.000000 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-11 10:18:34.000000 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:18:34.000000 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-11 10:18:34.000000 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 10:18:34.000000 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/dev/actions_and_webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/dev/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/dev/version_release.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/docs/source/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/frontends/json_front_end.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/frontends/test_suite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/glossary.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/docs/source/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/modules/causal_specification.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/modules/causal_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/modules/data_collector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.860614 causal_testing_framework-4.3.0/examples/covasim_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/example_beta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/dag.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/lr91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/lr91/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/data/normalised_results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/data/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/example_max_conductances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/example_max_conductances_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/examples/poisson/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson/causal_tests.json
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson/example_run_causal_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/examples/poisson-line-process/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.860614 causal_testing_framework-4.3.0/examples/poisson-line-process/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/examples/poisson-line-process/data/random/
+-rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/random/data_random_1000.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/example_poisson_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/data/nhefs.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/tests/data_collection_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/data_collection_tests/test_observational_data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/tests/generation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/generation_tests/test_abstract_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/tests/json_front_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/json_front_tests/test_json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/tests/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/resources/data/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/resources/data/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/resources/data/data_with_meta.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/resources/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/specification_tests/test_causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/specification_tests/test_metamorphic_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/specification_tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/tests/testing_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/testing_tests/test_estimators.py
```

### Comparing `causal_testing_framework-4.2.0/.github/CONTRIBUTING.md` & `causal_testing_framework-4.3.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `causal_testing_framework-4.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `causal_testing_framework-4.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/.github/workflows/ci-tests.yaml` & `causal_testing_framework-4.3.0/.github/workflows/ci-tests.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/.github/workflows/lint-format.yaml` & `causal_testing_framework-4.3.0/.github/workflows/lint-format.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/.github/workflows/publish-to-pypi.yaml` & `causal_testing_framework-4.3.0/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/.gitignore` & `causal_testing_framework-4.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/.pylintrc` & `causal_testing_framework-4.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/.readthedocs.yaml` & `causal_testing_framework-4.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/LICENSE` & `causal_testing_framework-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/PKG-INFO` & `causal_testing_framework-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal_testing_framework
-Version: 4.2.0
+Version: 4.3.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-4.2.0/README.md` & `causal_testing_framework-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/data_collection/data_collector.py` & `causal_testing_framework-4.3.0/causal_testing/data_collection/data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/generation/abstract_causal_test_case.py` & `causal_testing_framework-4.3.0/causal_testing/generation/abstract_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/generation/enum_gen.py` & `causal_testing_framework-4.3.0/causal_testing/generation/enum_gen.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/json_front/json_class.py` & `causal_testing_framework-4.3.0/causal_testing/json_front/json_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,62 +119,23 @@
         """Runs and evaluates each test case specified in the JSON input
 
         :param effects: Dictionary mapping effect class instances to string representations.
         :param mutates: Dictionary mapping mutation functions to string representations.
         :param estimators: Dictionary mapping estimator classes to string representations.
         :param f_flag: Failure flag that if True the script will stop executing when a test fails.
         """
-        failures = 0
-        msg = ""
         for test in self.test_plan["tests"]:
             if "skip" in test and test["skip"]:
                 continue
             test["estimator"] = estimators[test["estimator"]]
             if "mutations" in test:
                 if test["estimate_type"] == "coefficient":
-                    base_test_case = BaseTestCase(
-                        treatment_variable=next(self.scenario.variables[v] for v in test["mutations"]),
-                        outcome_variable=next(self.scenario.variables[v] for v in test["expected_effect"]),
-                        effect=test.get("effect", "direct"),
-                    )
-                    assert len(test["expected_effect"]) == 1, "Can only have one expected effect."
-                    causal_test_case = CausalTestCase(
-                        base_test_case=base_test_case,
-                        expected_causal_effect=next(
-                            effects[effect] for variable, effect in test["expected_effect"].items()
-                        ),
-                        estimate_type="coefficient",
-                        effect_modifier_configuration={
-                            self.scenario.variables[v] for v in test.get("effect_modifiers", [])
-                        },
-                    )
-                    result = self._execute_test_case(causal_test_case=causal_test_case, test=test, f_flag=f_flag)
-                    msg = (
-                        f"Executing test: {test['name']} \n"
-                        + f"  {causal_test_case} \n"
-                        + "  "
-                        + ("\n  ").join(str(result[1]).split("\n"))
-                        + "==============\n"
-                        + f"  Result: {'FAILED' if result[0] else 'Passed'}"
-                    )
-                    print(msg)
+                    msg = self._run_coefficient_test(test=test, f_flag=f_flag, effects=effects)
                 else:
-                    abstract_test = self._create_abstract_test_case(test, mutates, effects)
-                    concrete_tests, _ = abstract_test.generate_concrete_tests(5, 0.05)
-                    failures, _ = self._execute_tests(concrete_tests, test, f_flag)
-
-                    msg = (
-                        f"Executing test: {test['name']} \n"
-                        + "  abstract_test \n"
-                        + f"  {abstract_test} \n"
-                        + f"  {abstract_test.treatment_variable.name},"
-                        + f"  {abstract_test.treatment_variable.distribution} \n"
-                        + f"  Number of concrete tests for test case: {str(len(concrete_tests))} \n"
-                        + f"  {failures}/{len(concrete_tests)} failed for {test['name']}"
-                    )
+                    msg = self._run_ate_test(test=test, f_flag=f_flag, effects=effects, mutates=mutates)
                 self._append_to_file(msg, logging.INFO)
             else:
                 outcome_variable = next(
                     iter(test["expected_effect"])
                 )  # Take first key from dictionary of expected effect
                 base_test_case = BaseTestCase(
                     treatment_variable=self.variables["inputs"][test["treatment_variable"]],
@@ -193,16 +154,82 @@
                 msg = (
                     f"Executing concrete test: {test['name']} \n"
                     + f"treatment variable: {test['treatment_variable']} \n"
                     + f"outcome_variable = {outcome_variable} \n"
                     + f"control value = {test['control_value']}, treatment value = {test['treatment_value']} \n"
                     + f"Result: {'FAILED' if failed else 'Passed'}"
                 )
+                print(msg)
                 self._append_to_file(msg, logging.INFO)
 
+    def _run_coefficient_test(self, test: dict, f_flag: bool, effects: dict):
+        """Builds structures and runs test case for tests with an estimate_type of 'coefficient'.
+
+        :param test: Single JSON test definition stored in a mapping (dict)
+        :param f_flag: Failure flag that if True the script will stop executing when a test fails.
+        :param effects: Dictionary mapping effect class instances to string representations.
+        :return: String containing the message to be outputted
+        """
+        base_test_case = BaseTestCase(
+            treatment_variable=next(self.scenario.variables[v] for v in test["mutations"]),
+            outcome_variable=next(self.scenario.variables[v] for v in test["expected_effect"]),
+            effect=test.get("effect", "direct"),
+        )
+        assert len(test["expected_effect"]) == 1, "Can only have one expected effect."
+        causal_test_case = CausalTestCase(
+            base_test_case=base_test_case,
+            expected_causal_effect=next(effects[effect] for variable, effect in test["expected_effect"].items()),
+            estimate_type="coefficient",
+            effect_modifier_configuration={self.scenario.variables[v] for v in test.get("effect_modifiers", [])},
+        )
+        result = self._execute_test_case(causal_test_case=causal_test_case, test=test, f_flag=f_flag)
+        msg = (
+            f"Executing test: {test['name']} \n"
+            + f"  {causal_test_case} \n"
+            + "  "
+            + ("\n  ").join(str(result[1]).split("\n"))
+            + "==============\n"
+            + f"  Result: {'FAILED' if result[0] else 'Passed'}"
+        )
+        return msg
+
+    def _run_ate_test(self, test: dict, f_flag: bool, effects: dict, mutates: dict):
+        """Builds structures and runs test case for tests with an estimate_type of 'ate'.
+
+        :param test: Single JSON test definition stored in a mapping (dict)
+        :param f_flag: Failure flag that if True the script will stop executing when a test fails.
+        :param effects: Dictionary mapping effect class instances to string representations.
+        :param mutates: Dictionary mapping mutation functions to string representations.
+        :return: String containing the message to be outputted
+        """
+        if "sample_size" in test:
+            sample_size = test["sample_size"]
+        else:
+            sample_size = 5
+        if "target_ks_score" in test:
+            target_ks_score = test["target_ks_score"]
+        else:
+            target_ks_score = 0.05
+        abstract_test = self._create_abstract_test_case(test, mutates, effects)
+        concrete_tests, _ = abstract_test.generate_concrete_tests(
+            sample_size=sample_size, target_ks_score=target_ks_score
+        )
+        failures, _ = self._execute_tests(concrete_tests, test, f_flag)
+
+        msg = (
+            f"Executing test: {test['name']} \n"
+            + "  abstract_test \n"
+            + f"  {abstract_test} \n"
+            + f"  {abstract_test.treatment_variable.name},"
+            + f"  {abstract_test.treatment_variable.distribution} \n"
+            + f"  Number of concrete tests for test case: {str(len(concrete_tests))} \n"
+            + f"  {failures}/{len(concrete_tests)} failed for {test['name']}"
+        )
+        return msg
+
     def _execute_tests(self, concrete_tests, test, f_flag):
         failures = 0
         details = []
         if "formula" in test:
             self._append_to_file(f"Estimator formula used for test: {test['formula']}")
         for concrete_test in concrete_tests:
             failed, result = self._execute_test_case(concrete_test, test, f_flag)
```

### Comparing `causal_testing_framework-4.2.0/causal_testing/specification/causal_dag.py` & `causal_testing_framework-4.3.0/causal_testing/specification/causal_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import logging
 from itertools import combinations
 from random import sample
 from typing import Union
 
 import networkx as nx
+import pydot
 
 from causal_testing.testing.base_test_case import BaseTestCase
 
 from .scenario import Scenario
 from .variable import Output
 
 Node = Union[str, int]  # Node type hint: A node is a string or an int
@@ -129,15 +130,16 @@
     between a pair of random variables. We implement a CausalDAG as a networkx DiGraph with an additional check that
     ensures it is acyclic. A CausalDAG must be specified as a dot file.
     """
 
     def __init__(self, dot_path: str = None, **attr):
         super().__init__(**attr)
         if dot_path:
-            self.graph = nx.DiGraph(nx.drawing.nx_agraph.read_dot(dot_path))
+            pydot_graph = pydot.graph_from_dot_file(dot_path)
+            self.graph = nx.DiGraph(nx.drawing.nx_pydot.from_pydot(pydot_graph[0]))
         else:
             self.graph = nx.DiGraph()
 
         if not self.is_acyclic():
             raise nx.HasACycle("Invalid Causal DAG: contains a cycle.")
 
     def check_iv_assumptions(self, treatment, outcome, instrument) -> bool:
```

### Comparing `causal_testing_framework-4.2.0/causal_testing/specification/causal_specification.py` & `causal_testing_framework-4.3.0/causal_testing/specification/causal_specification.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/specification/metamorphic_relation.py` & `causal_testing_framework-4.3.0/causal_testing/specification/metamorphic_relation.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/specification/scenario.py` & `causal_testing_framework-4.3.0/causal_testing/specification/scenario.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/specification/variable.py` & `causal_testing_framework-4.3.0/causal_testing/specification/variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/testing/base_test_case.py` & `causal_testing_framework-4.3.0/causal_testing/testing/base_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/testing/causal_test_case.py` & `causal_testing_framework-4.3.0/causal_testing/testing/causal_test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         # pylint: disable=too-many-arguments
         self,
         base_test_case: BaseTestCase,
         expected_causal_effect: CausalTestOutcome,
         control_value: Any = None,
         treatment_value: Any = None,
         estimate_type: str = "ate",
+        estimate_params: dict = None,
         effect_modifier_configuration: dict[Variable:Any] = None,
     ):
         """
         :param base_test_case: A BaseTestCase object consisting of a treatment variable, outcome variable and effect
         :param expected_causal_effect: The expected causal effect (Positive, Negative, No Effect).
         :param control_value: The control value for the treatment variable (before intervention).
         :param treatment_value: The treatment value for the treatment variable (after intervention).
@@ -43,14 +44,16 @@
         self.base_test_case = base_test_case
         self.control_value = control_value
         self.expected_causal_effect = expected_causal_effect
         self.outcome_variable = base_test_case.outcome_variable
         self.treatment_variable = base_test_case.treatment_variable
         self.treatment_value = treatment_value
         self.estimate_type = estimate_type
+        if estimate_params is None:
+            self.estimate_params = {}
         self.effect = base_test_case.effect
 
         if effect_modifier_configuration:
             self.effect_modifier_configuration = effect_modifier_configuration
         else:
             self.effect_modifier_configuration = {}
```

### Comparing `causal_testing_framework-4.2.0/causal_testing/testing/causal_test_engine.py` & `causal_testing_framework-4.3.0/causal_testing/testing/causal_test_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,16 @@
                 estimator=estimator,
                 test_value=TestValue("ate", cates_df),
                 effect_modifier_configuration=causal_test_case.effect_modifier_configuration,
                 confidence_intervals=confidence_intervals,
             )
         elif causal_test_case.estimate_type == "risk_ratio":
             logger.debug("calculating risk_ratio")
-            risk_ratio, confidence_intervals = estimator.estimate_risk_ratio()
+            risk_ratio, confidence_intervals = estimator.estimate_risk_ratio(**causal_test_case.estimate_params)
+
             causal_test_result = CausalTestResult(
                 estimator=estimator,
                 test_value=TestValue("risk_ratio", risk_ratio),
                 effect_modifier_configuration=causal_test_case.effect_modifier_configuration,
                 confidence_intervals=confidence_intervals,
             )
         elif causal_test_case.estimate_type == "coefficient":
```

### Comparing `causal_testing_framework-4.2.0/causal_testing/testing/causal_test_outcome.py` & `causal_testing_framework-4.3.0/causal_testing/testing/causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/testing/causal_test_result.py` & `causal_testing_framework-4.3.0/causal_testing/testing/causal_test_result.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/testing/causal_test_suite.py` & `causal_testing_framework-4.3.0/causal_testing/testing/causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/testing/estimators.py` & `causal_testing_framework-4.3.0/causal_testing/testing/estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         x = dmatrix(self.formula.split("~")[1], x, return_type="dataframe")
         for col in x:
             if str(x.dtypes[col]) == "object":
                 x = pd.get_dummies(x, columns=[col], drop_first=True)
         # x = x[model.params.index]
         return model.predict(x)
 
-    def estimate_control_treatment(self, bootstrap_size=100, adjustment_config=None) -> tuple[pd.Series, pd.Series]:
+    def estimate_control_treatment(self, bootstrap_size, adjustment_config) -> tuple[pd.Series, pd.Series]:
         """Estimate the outcomes under control and treatment.
 
         :return: The estimated control and treatment values and their confidence
         intervals in the form ((ci_low, control, ci_high), (ci_low, treatment, ci_high)).
         """
 
         y = self.estimate(self.df, adjustment_config=adjustment_config)
@@ -211,22 +211,26 @@
         # std_errors = np.array([np.sqrt(np.dot(np.dot(g, cov), g)) for g in gradient.to_numpy()])
         # c = 1.96  # multiplier for confidence interval
         # upper = np.maximum(0, np.minimum(1, y + std_errors * c))
         # lower = np.maximum(0, np.minimum(1, y - std_errors * c))
 
         return (y.iloc[1], np.array(control)), (y.iloc[0], np.array(treatment))
 
-    def estimate_ate(self, bootstrap_size=100, adjustment_config=None) -> float:
+    def estimate_ate(self, estimator_params: dict = None) -> float:
         """Estimate the ate effect of the treatment on the outcome. That is, the change in outcome caused
         by changing the treatment variable from the control value to the treatment value. Here, we actually
         calculate the expected outcomes under control and treatment and take one away from the other. This
         allows for custom terms to be put in such as squares, inverses, products, etc.
 
         :return: The estimated average treatment effect and 95% confidence intervals
         """
+        if estimator_params is None:
+            estimator_params = {}
+        bootstrap_size = estimator_params.get("bootstrap_size", 100)
+        adjustment_config = estimator_params.get("adjustment_config", None)
         (control_outcome, control_bootstraps), (
             treatment_outcome,
             treatment_bootstraps,
         ) = self.estimate_control_treatment(bootstrap_size=bootstrap_size, adjustment_config=adjustment_config)
         estimate = treatment_outcome - control_outcome
 
         if control_bootstraps is None or treatment_bootstraps is None:
@@ -241,22 +245,26 @@
             f"Changing {self.treatment} from {self.control_value} to {self.treatment_value} gives an estimated "
             f"ATE of {ci_low} < {estimate} < {ci_high}"
         )
         assert ci_low < estimate < ci_high, f"Expecting {ci_low} < {estimate} < {ci_high}"
 
         return estimate, (ci_low, ci_high)
 
-    def estimate_risk_ratio(self, bootstrap_size=100, adjustment_config=None) -> float:
+    def estimate_risk_ratio(self, estimator_params: dict = None) -> float:
         """Estimate the ate effect of the treatment on the outcome. That is, the change in outcome caused
         by changing the treatment variable from the control value to the treatment value. Here, we actually
         calculate the expected outcomes under control and treatment and divide one by the other. This
         allows for custom terms to be put in such as squares, inverses, products, etc.
 
         :return: The estimated risk ratio and 95% confidence intervals.
         """
+        if estimator_params is None:
+            estimator_params = {}
+        bootstrap_size = estimator_params.get("bootstrap_size", 100)
+        adjustment_config = estimator_params.get("adjustment_config", None)
         (control_outcome, control_bootstraps), (
             treatment_outcome,
             treatment_bootstraps,
         ) = self.estimate_control_treatment(bootstrap_size=bootstrap_size, adjustment_config=adjustment_config)
         estimate = treatment_outcome / control_outcome
 
         if control_bootstraps is None or treatment_bootstraps is None:
```

### Comparing `causal_testing_framework-4.2.0/causal_testing/testing/intervention.py` & `causal_testing_framework-4.3.0/causal_testing/testing/intervention.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing/utils/validation.py` & `causal_testing_framework-4.3.0/causal_testing/utils/validation.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/causal_testing_framework.egg-info/PKG-INFO` & `causal_testing_framework-4.3.0/causal_testing_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-testing-framework
-Version: 4.2.0
+Version: 4.3.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-4.2.0/causal_testing_framework.egg-info/SOURCES.txt` & `causal_testing_framework-4.3.0/causal_testing_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/Makefile` & `causal_testing_framework-4.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/README.md` & `causal_testing_framework-4.3.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/make.bat` & `causal_testing_framework-4.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/conf.py` & `causal_testing_framework-4.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/description.rst` & `causal_testing_framework-4.3.0/docs/source/description.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/dev/actions_and_webhooks.rst` & `causal_testing_framework-4.3.0/docs/source/dev/actions_and_webhooks.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/dev/documentation.rst` & `causal_testing_framework-4.3.0/docs/source/dev/documentation.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/dev/version_release.rst` & `causal_testing_framework-4.3.0/docs/source/dev/version_release.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/frontends/json_front_end.rst` & `causal_testing_framework-4.3.0/docs/source/frontends/json_front_end.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/frontends/test_suite.rst` & `causal_testing_framework-4.3.0/docs/source/frontends/test_suite.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/images/workflow.png` & `causal_testing_framework-4.3.0/docs/source/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/index.rst` & `causal_testing_framework-4.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/modules/causal_specification.rst` & `causal_testing_framework-4.3.0/docs/source/modules/causal_specification.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/modules/causal_tests.rst` & `causal_testing_framework-4.3.0/docs/source/modules/causal_tests.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/modules/data_collector.rst` & `causal_testing_framework-4.3.0/docs/source/modules/data_collector.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/docs/source/usage.rst` & `causal_testing_framework-4.3.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/README.md` & `causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/dag.png` & `causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv` & `causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/example_beta.py` & `causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/example_beta.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/README.md` & `causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/dag.png` & `causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/example_vaccine.py` & `causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/example_vaccine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/lr91/README.md` & `causal_testing_framework-4.3.0/examples/lr91/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/lr91/dag.dot` & `causal_testing_framework-4.3.0/examples/lr91/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/lr91/dag.png` & `causal_testing_framework-4.3.0/examples/lr91/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/lr91/data/normalised_results.csv` & `causal_testing_framework-4.3.0/examples/lr91/data/normalised_results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/lr91/data/results.csv` & `causal_testing_framework-4.3.0/examples/lr91/data/results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/lr91/example_max_conductances.py` & `causal_testing_framework-4.3.0/examples/lr91/example_max_conductances.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/lr91/example_max_conductances_test_suite.py` & `causal_testing_framework-4.3.0/examples/lr91/example_max_conductances_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson/README.md` & `causal_testing_framework-4.3.0/examples/poisson/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson/causal_tests.json` & `causal_testing_framework-4.3.0/examples/poisson/causal_tests.json`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson/dag.dot` & `causal_testing_framework-4.3.0/examples/poisson/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson/data.csv` & `causal_testing_framework-4.3.0/examples/poisson/data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson/example_run_causal_tests.py` & `causal_testing_framework-4.3.0/examples/poisson/example_run_causal_tests.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/README.md` & `causal_testing_framework-4.3.0/examples/poisson-line-process/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/dag.png` & `causal_testing_framework-4.3.0/examples/poisson-line-process/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/random/data_random_1000.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/random/data_random_1000.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv` & `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/examples/poisson-line-process/example_poisson_process.py` & `causal_testing_framework-4.3.0/examples/poisson-line-process/example_poisson_process.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/images/workflow.png` & `causal_testing_framework-4.3.0/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/pyproject.toml` & `causal_testing_framework-4.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     "lhsmdu~=1.1",
     "networkx~=2.6",
     "numpy~=1.22.0",
     "pandas~=1.3",
     "scikit_learn~=1.1",
     "scipy~=1.7",
     "statsmodels~=0.13",
-    "tabulate~=0.8"
+    "tabulate~=0.8",
+    "pydot~=1.4"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "autopep8",
     "isort",
```

### Comparing `causal_testing_framework-4.2.0/tests/data/nhefs.csv` & `causal_testing_framework-4.3.0/tests/data/nhefs.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/tests/data_collection_tests/test_observational_data_collector.py` & `causal_testing_framework-4.3.0/tests/data_collection_tests/test_observational_data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/tests/generation_tests/test_abstract_test_case.py` & `causal_testing_framework-4.3.0/tests/generation_tests/test_abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/tests/json_front_tests/test_json_class.py` & `causal_testing_framework-4.3.0/tests/json_front_tests/test_json_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,45 @@
         effects = {"NoEffect": NoEffect()}
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, estimators=estimators, f_flag=False)
         with open("temp_out.txt", "r") as reader:
             temp_out = reader.readlines()
         self.assertIn("FAILED", temp_out[-1])
+    def test_concrete_generate_params(self):
+        example_test = {
+            "tests": [
+                {
+                    "name": "test1",
+                    "mutations": {"test_input": "Increase"},
+                    "estimator": "LinearRegressionEstimator",
+                    "estimate_type": "ate",
+                    "effect_modifiers": [],
+                    "expected_effect": {"test_output": "NoEffect"},
+                    "sample_size": 5,
+                    "target_ks_score": 0.05,
+                    "skip": False,
+                }
+            ]
+        }
+        self.json_class.test_plan = example_test
+        effects = {"NoEffect": NoEffect()}
+        mutates = {
+            "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
+                                  > self.json_class.scenario.variables[x].z3
+        }
+        estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
+
+        self.json_class.run_json_tests(effects=effects, estimators=estimators, f_flag=False, mutates=mutates)
+
+        # Test that the final log message prints that failed tests are printed, which is expected behaviour for this
+        # scenario
+        with open("temp_out.txt", "r") as reader:
+            temp_out = reader.readlines()
+        self.assertIn("failed", temp_out[-1])
 
     def test_no_data_provided(self):
         example_test = {
             "tests": [
                 {
                     "name": "test1",
                     "mutations": {"test_input": "Increase"},
```

### Comparing `causal_testing_framework-4.2.0/tests/specification_tests/test_causal_dag.py` & `causal_testing_framework-4.3.0/tests/specification_tests/test_causal_dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import networkx as nx
 from causal_testing.specification.causal_dag import CausalDAG, close_separator, list_all_min_sep
 from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
 
 
 class TestCausalDAGIssue90(unittest.TestCase):
-
     """
     Test the CausalDAG class for the resolution of Issue 90.
     """
 
     def setUp(self) -> None:
         temp_dir_path = create_temp_dir_if_non_existent()
         self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
@@ -58,15 +57,14 @@
         causal_dag = CausalDAG(self.dag_dot_path)
         causal_dag.graph.add_edge("U", "I")
         with self.assertRaises(ValueError):
             causal_dag.check_iv_assumptions("X", "Y", "I")
 
 
 class TestCausalDAG(unittest.TestCase):
-
     """
     Test the CausalDAG class for creation of Causal Directed Acyclic Graphs (DAGs).
 
     In particular, confirm whether the Causal DAG class creates valid causal directed acyclic graphs (empty and directed
     graphs without cycles) and refuses to create invalid (cycle-containing) graphs.
     """
 
@@ -172,46 +170,45 @@
         self.assertEqual(list(indirect_graph.graph.edges), original_edges)
         self.assertEqual(indirect_graph.graph.nodes, causal_dag.graph.nodes)
 
     def test_proper_backdoor_graph(self):
         """Test whether converting a Causal DAG to a proper back-door graph works correctly."""
         causal_dag = CausalDAG(self.dag_dot_path)
         proper_backdoor_graph = causal_dag.get_proper_backdoor_graph(["X1", "X2"], ["Y"])
-        self.assertEqual(
-            list(proper_backdoor_graph.graph.edges),
-            [
-                ("X1", "X2"),
-                ("X2", "V"),
-                ("X2", "D2"),
-                ("D1", "D2"),
-                ("D1", "Y"),
-                ("Y", "D3"),
-                ("Z", "X2"),
-                ("Z", "Y"),
-            ],
-        )
+        edges = set([
+                    ("X1", "X2"),
+                    ("X2", "V"),
+                    ("X2", "D2"),
+                    ("D1", "D2"),
+                    ("D1", "Y"),
+                    ("Y", "D3"),
+                    ("Z", "X2"),
+                    ("Z", "Y"),
+                ])
+        self.assertTrue(
+            set(proper_backdoor_graph.graph.edges).issubset(edges))
 
     def test_constructive_backdoor_criterion_should_hold(self):
         """Test whether the constructive criterion holds when it should."""
         causal_dag = CausalDAG(self.dag_dot_path)
         xs, ys, zs = ["X1", "X2"], ["Y"], ["Z"]
         proper_backdoor_graph = causal_dag.get_proper_backdoor_graph(xs, ys)
         self.assertTrue(causal_dag.constructive_backdoor_criterion(proper_backdoor_graph, xs, ys, zs))
 
     def test_constructive_backdoor_criterion_should_not_hold_not_d_separator_in_proper_backdoor_graph(
-        self,
+            self,
     ):
         """Test whether the constructive criterion fails when the adjustment set is not a d-separator."""
         causal_dag = CausalDAG(self.dag_dot_path)
         xs, ys, zs = ["X1", "X2"], ["Y"], ["V"]
         proper_backdoor_graph = causal_dag.get_proper_backdoor_graph(xs, ys)
         self.assertFalse(causal_dag.constructive_backdoor_criterion(proper_backdoor_graph, xs, ys, zs))
 
     def test_constructive_backdoor_criterion_should_not_hold_descendent_of_proper_causal_path(
-        self,
+            self,
     ):
         """Test whether the constructive criterion holds when the adjustment set Z contains a descendent of a variable
         on a proper causal path between X and Y."""
         causal_dag = CausalDAG(self.dag_dot_path)
         xs, ys, zs = ["X1", "X2"], ["Y"], ["D1"]
         proper_backdoor_graph = causal_dag.get_proper_backdoor_graph(xs, ys)
         self.assertFalse(causal_dag.constructive_backdoor_criterion(proper_backdoor_graph, xs, ys, zs))
@@ -388,15 +385,14 @@
         self.assertFalse(causal_dag.depends_on_outputs("D", self.scenario))
 
     def tearDown(self) -> None:
         remove_temp_dir_if_existent()
 
 
 class TestUndirectedGraphAlgorithms(unittest.TestCase):
-
     """
     Test the graph algorithms designed for the undirected graph variants of a Causal DAG.
     During the identification process, a Causal DAG is converted into several forms of undirected graph which allow for
     more efficient computation of minimal separators. This suite of tests covers the two main algorithms applied to
     these forms of undirected graphs (ancestor and moral graphs): close_separator and list_all_min_sep."""
 
     def setUp(self) -> None:
```

### Comparing `causal_testing_framework-4.2.0/tests/specification_tests/test_metamorphic_relations.py` & `causal_testing_framework-4.3.0/tests/specification_tests/test_metamorphic_relations.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/tests/specification_tests/test_variable.py` & `causal_testing_framework-4.3.0/tests/specification_tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/tests/test_helpers.py` & `causal_testing_framework-4.3.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_case.py` & `causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_engine.py` & `causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_engine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_outcome.py` & `causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_suite.py` & `causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.2.0/tests/testing_tests/test_estimators.py` & `causal_testing_framework-4.3.0/tests/testing_tests/test_estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,22 +120,22 @@
         self.assertEqual(round(odds, 4), 0.8948)
 
     def test_ate_adjustment(self):
         df = self.scarf_df.copy()
         logistic_regression_estimator = LogisticRegressionEstimator(
             "length_in", 65, 55, {"large_gauge"}, "completed", df
         )
-        ate, _ = logistic_regression_estimator.estimate_ate(adjustment_config={"large_gauge": 0})
+        ate, _ = logistic_regression_estimator.estimate_ate(estimator_params={"adjustment_config": {"large_gauge": 0}})
         self.assertEqual(round(ate, 4), -0.3388)
 
     def test_ate_invalid_adjustment(self):
         df = self.scarf_df.copy()
         logistic_regression_estimator = LogisticRegressionEstimator("length_in", 65, 55, {}, "completed", df)
         with self.assertRaises(ValueError):
-            ate, _ = logistic_regression_estimator.estimate_ate(adjustment_config={"large_gauge": 0})
+            ate, _ = logistic_regression_estimator.estimate_ate(estimator_params={"adjustment_config": {"large_gauge": 0}})
 
     def test_ate_effect_modifiers(self):
         df = self.scarf_df.copy()
         logistic_regression_estimator = LogisticRegressionEstimator(
             "length_in", 65, 55, set(), "completed", df, effect_modifiers={"large_gauge": 0}
         )
         ate, _ = logistic_regression_estimator.estimate_ate()
```

