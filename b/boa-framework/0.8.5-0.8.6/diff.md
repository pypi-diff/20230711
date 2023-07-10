# Comparing `tmp/boa-framework-0.8.5.tar.gz` & `tmp/boa-framework-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boa-framework-0.8.5.tar", last modified: Mon Jul 10 18:14:45 2023, max compression
+gzip compressed data, was "boa-framework-0.8.6.tar", last modified: Mon Jul 10 22:44:04 2023, max compression
```

## Comparing `boa-framework-0.8.5.tar` & `boa-framework-0.8.6.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.338438 boa-framework-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-10 18:11:52.000000 boa-framework-0.8.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.238436 boa-framework-0.8.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.246436 boa-framework-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-10 18:11:52.000000 boa-framework-0.8.5/.github/workflows/CI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-10 18:11:52.000000 boa-framework-0.8.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-10 18:11:52.000000 boa-framework-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-10 18:11:52.000000 boa-framework-0.8.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 18:11:52.000000 boa-framework-0.8.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 18:11:52.000000 boa-framework-0.8.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-10 18:11:52.000000 boa-framework-0.8.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-10 18:11:52.000000 boa-framework-0.8.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-10 18:11:52.000000 boa-framework-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 18:11:52.000000 boa-framework-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-10 18:14:45.338438 boa-framework-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-10 18:11:52.000000 boa-framework-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.250436 boa-framework-0.8.5/boa/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/_doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 18:14:44.000000 boa-framework-0.8.5/boa/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/ax_instantiation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/instantiation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/metaclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.254436 boa-framework-0.8.5/boa/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/metrics/metric_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/metrics/modular_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/metrics/synthetic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.254436 boa-framework-0.8.5/boa/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/scripts/moo.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/scripts/moo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/scripts/run_branin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/scripts/script_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/scripts/synth_func_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/scripts/synth_func_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.258436 boa-framework-0.8.5/boa/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/wrappers/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/wrappers/script_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-07-10 18:11:52.000000 boa-framework-0.8.5/boa/wrappers/wrapper_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.258436 boa-framework-0.8.5/boa_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-10 18:14:45.000000 boa-framework-0.8.5/boa_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-10 18:14:45.000000 boa-framework-0.8.5/boa_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:14:45.000000 boa-framework-0.8.5/boa_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-10 18:14:45.000000 boa-framework-0.8.5/boa_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 18:14:45.000000 boa-framework-0.8.5/boa_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 18:11:52.000000 boa-framework-0.8.5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.262436 boa-framework-0.8.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.262436 boa-framework-0.8.5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/_templates/custom_module_template_short.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/code_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.286437 boa-framework-0.8.5/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.286437 boa-framework-0.8.5/docs/examples/cached_notebooks/
--rw-r--r--   0 runner    (1001) docker     (123) 14829280 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/examples/cached_notebooks/example_optimization_results.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/examples/example_py_run.rst
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)  4003040 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/examples/load_moo_scheduler.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  3999980 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/examples/load_scheduler.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   145361 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/examples/moo_optimization_run.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   120176 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/examples/optimization_run.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/examples/single_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/examples/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/gallery.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.326438 boa-framework-0.8.5/docs/references/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/references/rst_references.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/troubleshooting.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.326438 boa-framework-0.8.5/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/user_guide/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/user_guide/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/user_guide/package_overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-10 18:11:52.000000 boa-framework-0.8.5/docs/user_guide/run_script.rst
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-10 18:11:52.000000 boa-framework-0.8.5/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-10 18:11:52.000000 boa-framework-0.8.5/environment_dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-10 18:11:52.000000 boa-framework-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:14:45.338438 boa-framework-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-10 18:11:52.000000 boa-framework-0.8.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.326438 boa-framework-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.326438 boa-framework-0.8.5/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/integration_tests/test_dunder_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/integration_tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/integration_tests/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.242436 boa-framework-0.8.5/tests/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.242436 boa-framework-0.8.5/tests/scripts/other_langs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.330438 boa-framework-0.8.5/tests/scripts/other_langs/r_package_full/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_package_full/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_package_full/fetch_trial_data.R
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_package_full/run_model.R
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_package_full/set_trial_status.R
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_package_full/write_configs.R
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.330438 boa-framework-0.8.5/tests/scripts/other_langs/r_package_light/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_package_light/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_package_light/run_model.R
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.330438 boa-framework-0.8.5/tests/scripts/other_langs/r_package_streamlined/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_package_streamlined/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_package_streamlined/config_fail.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_package_streamlined/run_model.R
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.330438 boa-framework-0.8.5/tests/scripts/other_langs/r_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/other_langs/r_utils/hartman6.R
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.334438 boa-framework-0.8.5/tests/scripts/stand_alone_opt_package/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/stand_alone_opt_package/stand_alone_model_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/stand_alone_opt_package/stand_alone_pkg_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/scripts/stand_alone_opt_package/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.334438 boa-framework-0.8.5/tests/test_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/test_configs/test_config_gen_strat1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/test_configs/test_config_metric.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/test_configs/test_config_moo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/test_configs/test_config_param_parse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/test_configs/test_config_pass_through_metric.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/test_configs/test_config_soo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/test_configs/test_config_synth.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:45.338438 boa-framework-0.8.5/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/unit_tests/test_config_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/unit_tests/test_generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/unit_tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/unit_tests/test_objective_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-10 18:11:52.000000 boa-framework-0.8.5/tests/unit_tests/test_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.454373 boa-framework-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-10 22:41:10.000000 boa-framework-0.8.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.366373 boa-framework-0.8.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.382373 boa-framework-0.8.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-10 22:41:10.000000 boa-framework-0.8.6/.github/workflows/CI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-10 22:41:10.000000 boa-framework-0.8.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-10 22:41:10.000000 boa-framework-0.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-10 22:41:10.000000 boa-framework-0.8.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 22:41:10.000000 boa-framework-0.8.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 22:41:10.000000 boa-framework-0.8.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-10 22:41:10.000000 boa-framework-0.8.6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-10 22:41:10.000000 boa-framework-0.8.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-10 22:41:10.000000 boa-framework-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 22:41:10.000000 boa-framework-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-10 22:44:04.454373 boa-framework-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-10 22:41:10.000000 boa-framework-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.390373 boa-framework-0.8.6/boa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/_doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 22:44:04.000000 boa-framework-0.8.6/boa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/ax_instantiation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/instantiation_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/metaclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.390373 boa-framework-0.8.6/boa/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/metrics/metric_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/metrics/modular_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/metrics/synthetic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.390373 boa-framework-0.8.6/boa/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/scripts/moo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/scripts/moo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/scripts/run_branin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/scripts/script_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/scripts/synth_func_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/scripts/synth_func_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.394373 boa-framework-0.8.6/boa/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/wrappers/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/wrappers/script_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-07-10 22:41:10.000000 boa-framework-0.8.6/boa/wrappers/wrapper_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.394373 boa-framework-0.8.6/boa_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-10 22:44:04.000000 boa-framework-0.8.6/boa_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-10 22:44:04.000000 boa-framework-0.8.6/boa_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:44:04.000000 boa-framework-0.8.6/boa_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-10 22:44:04.000000 boa-framework-0.8.6/boa_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 22:44:04.000000 boa-framework-0.8.6/boa_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 22:41:10.000000 boa-framework-0.8.6/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.398373 boa-framework-0.8.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.398373 boa-framework-0.8.6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/_templates/custom_module_template_short.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/code_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.418373 boa-framework-0.8.6/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.418373 boa-framework-0.8.6/docs/examples/cached_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123) 14829280 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/examples/cached_notebooks/example_optimization_results.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/examples/example_py_run.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)  4003040 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/examples/load_moo_scheduler.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3999980 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/examples/load_scheduler.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   145361 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/examples/moo_optimization_run.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   120176 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/examples/optimization_run.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/examples/single_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/examples/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/gallery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.442373 boa-framework-0.8.6/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/references/rst_references.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/troubleshooting.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.446373 boa-framework-0.8.6/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/user_guide/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/user_guide/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/user_guide/package_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-10 22:41:10.000000 boa-framework-0.8.6/docs/user_guide/run_script.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-10 22:41:10.000000 boa-framework-0.8.6/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-10 22:41:10.000000 boa-framework-0.8.6/environment_dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-10 22:41:10.000000 boa-framework-0.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 22:44:04.454373 boa-framework-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-10 22:41:10.000000 boa-framework-0.8.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.446373 boa-framework-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.446373 boa-framework-0.8.6/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/integration_tests/test_dunder_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/integration_tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/integration_tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.370373 boa-framework-0.8.6/tests/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.370373 boa-framework-0.8.6/tests/scripts/other_langs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.446373 boa-framework-0.8.6/tests/scripts/other_langs/r_package_full/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_package_full/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_package_full/fetch_trial_data.R
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_package_full/run_model.R
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_package_full/set_trial_status.R
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_package_full/write_configs.R
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.446373 boa-framework-0.8.6/tests/scripts/other_langs/r_package_light/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_package_light/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_package_light/run_model.R
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.450374 boa-framework-0.8.6/tests/scripts/other_langs/r_package_streamlined/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_package_streamlined/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_package_streamlined/config_fail.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_package_streamlined/run_model.R
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.450374 boa-framework-0.8.6/tests/scripts/other_langs/r_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/other_langs/r_utils/hartman6.R
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.450374 boa-framework-0.8.6/tests/scripts/stand_alone_opt_package/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/stand_alone_opt_package/stand_alone_model_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/stand_alone_opt_package/stand_alone_pkg_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/scripts/stand_alone_opt_package/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.450374 boa-framework-0.8.6/tests/test_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/test_configs/test_config_gen_strat1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/test_configs/test_config_metric.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/test_configs/test_config_moo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/test_configs/test_config_param_parse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/test_configs/test_config_pass_through_metric.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/test_configs/test_config_soo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/test_configs/test_config_synth.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:44:04.454373 boa-framework-0.8.6/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/unit_tests/test_config_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/unit_tests/test_generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/unit_tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/unit_tests/test_objective_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-10 22:41:10.000000 boa-framework-0.8.6/tests/unit_tests/test_plots.py
```

### Comparing `boa-framework-0.8.5/.github/workflows/CI.yaml` & `boa-framework-0.8.6/.github/workflows/CI.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -62,21 +62,29 @@
 
       - name: Set cache date
         run: echo "DATE=$(date +'%Y%m%d')" >> $GITHUB_ENV
 
       - uses: actions/cache@v3
         with:
           path: ${{ matrix.prefix }}
-          key: ${{ matrix.label }}-conda-${{ hashFiles('environment.yml') }}-${{ env.DATE }}-${{ env.CACHE_NUMBER }}
+          key: ${{ matrix.label }}-conda-${{ hashFiles('environment_dev.yml') }}-${{ env.DATE }}-${{ env.CACHE_NUMBER }}
         id: cache
 
       - name: Update base environment
         run: mamba env update -n boa -f environment_dev.yml --prune
         if: steps.cache.outputs.cache-hit != 'true'
 
+      - name: export env to artifact
+        run: mamba env export -n boa > environment_ci_${{ matrix.os }}.yml
+
+      - uses: actions/upload-artifact@v3
+        with:
+          name: environment_ci_${{ matrix.os }}.yml
+          path: environment_ci_${{ matrix.os }}.yml
+
       - name: Lint
         shell: bash -l {0}
         run: |
           invoke style --checkonly
 
       - name: Run tests
         shell: bash -l {0}
```

### Comparing `boa-framework-0.8.5/.github/workflows/release.yaml` & `boa-framework-0.8.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/.gitignore` & `boa-framework-0.8.6/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 docs/jupyter_execute
 docs/code_reference/api
 *.log
 
 # outputted opt runs (for testing usually)
 boa_runs*
 moo_runs*
+*20*T*
 
 # autogenerated version file from setuptools-scm
 _version.py
 
 # scratch work
 scratch
 
@@ -46,14 +47,17 @@
 .ipynb_checkpoints
 
 # General
 .DS_Store
 .AppleDouble
 .LSOverride
 
+# Linting
+.flakeheaven_cache
+
 #vscode
 .vscode
 
 ### JetBrains template
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio and Webstorm
 # Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
```

### Comparing `boa-framework-0.8.5/.pre-commit-config.yaml` & `boa-framework-0.8.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/CITATION.cff` & `boa-framework-0.8.6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/CODE_OF_CONDUCT.md` & `boa-framework-0.8.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/LICENSE` & `boa-framework-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/PKG-INFO` & `boa-framework-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boa-framework
-Version: 0.8.5
+Version: 0.8.6
 Summary: Bayesian Optimization for Anything: A high-level Bayesian optimization framework and model wrapping tool. It provides an easy-to-use interface between models and the python libraries Ax and BoTorch.
 Author-email: Madeline Scyphers <madelinescyphers@gmail.com>, Justine Missik <jemissik@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/madeline-scyphers/boa
 Project-URL: Bug Tracker, https://github.com/madeline-scyphers/boa/issues
 Project-URL: Documentation, http://boa-framework.readthedocs.io
 Classifier: Development Status :: 4 - Beta
```

### Comparing `boa-framework-0.8.5/README.md` & `boa-framework-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/__init__.py` & `boa-framework-0.8.6/boa/__init__.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/__main__.py` & `boa-framework-0.8.6/boa/__main__.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/_doc_utils.py` & `boa-framework-0.8.6/boa/_doc_utils.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/ax_instantiation_utils.py` & `boa-framework-0.8.6/boa/ax_instantiation_utils.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/controller.py` & `boa-framework-0.8.6/boa/controller.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/instantiation_base.py` & `boa-framework-0.8.6/boa/instantiation_base.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/logger.py` & `boa-framework-0.8.6/boa/logger.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/metaclasses.py` & `boa-framework-0.8.6/boa/metaclasses.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/metrics/metric_funcs.py` & `boa-framework-0.8.6/boa/metrics/metric_funcs.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/metrics/metrics.py` & `boa-framework-0.8.6/boa/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/metrics/modular_metric.py` & `boa-framework-0.8.6/boa/metrics/modular_metric.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/metrics/synthetic_funcs.py` & `boa-framework-0.8.6/boa/metrics/synthetic_funcs.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/plotting.py` & `boa-framework-0.8.6/boa/plotting.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/registry.py` & `boa-framework-0.8.6/boa/registry.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/runner.py` & `boa-framework-0.8.6/boa/runner.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/scheduler.py` & `boa-framework-0.8.6/boa/scheduler.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/scripts/moo.py` & `boa-framework-0.8.6/boa/scripts/moo.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/scripts/moo.yaml` & `boa-framework-0.8.6/boa/scripts/moo.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/scripts/run_branin.py` & `boa-framework-0.8.6/boa/scripts/run_branin.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/scripts/script_wrappers.py` & `boa-framework-0.8.6/boa/scripts/script_wrappers.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/scripts/synth_func_cli.py` & `boa-framework-0.8.6/boa/scripts/synth_func_cli.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/scripts/synth_func_config.yaml` & `boa-framework-0.8.6/boa/scripts/synth_func_config.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/storage.py` & `boa-framework-0.8.6/boa/storage.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/utils.py` & `boa-framework-0.8.6/boa/utils.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/wrappers/__init__.py` & `boa-framework-0.8.6/boa/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/wrappers/base_wrapper.py` & `boa-framework-0.8.6/boa/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/wrappers/script_wrapper.py` & `boa-framework-0.8.6/boa/wrappers/script_wrapper.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa/wrappers/wrapper_utils.py` & `boa-framework-0.8.6/boa/wrappers/wrapper_utils.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/boa_framework.egg-info/PKG-INFO` & `boa-framework-0.8.6/boa_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boa-framework
-Version: 0.8.5
+Version: 0.8.6
 Summary: Bayesian Optimization for Anything: A high-level Bayesian optimization framework and model wrapping tool. It provides an easy-to-use interface between models and the python libraries Ax and BoTorch.
 Author-email: Madeline Scyphers <madelinescyphers@gmail.com>, Justine Missik <jemissik@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/madeline-scyphers/boa
 Project-URL: Bug Tracker, https://github.com/madeline-scyphers/boa/issues
 Project-URL: Documentation, http://boa-framework.readthedocs.io
 Classifier: Development Status :: 4 - Beta
```

### Comparing `boa-framework-0.8.5/boa_framework.egg-info/SOURCES.txt` & `boa-framework-0.8.6/boa_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/Makefile` & `boa-framework-0.8.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/_templates/custom-class-template.rst` & `boa-framework-0.8.6/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/_templates/custom-module-template.rst` & `boa-framework-0.8.6/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/code_reference.rst` & `boa-framework-0.8.6/docs/code_reference.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/conf.py` & `boa-framework-0.8.6/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 sys.path.insert(0, os.path.abspath("../boa/"))
 
 
 from boa._doc_utils import add_ref_to_all_submodules_inits
 
 # -- Project information -----------------------------------------------------
 
-project = "boa"
+project = "BOA"
 copyright = "2022, Madeline Scyphers, Justine Missik"
 author = "Madeline Scyphers, Justine Missik"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named "sphinx.ext.*") or your custom
```

### Comparing `boa-framework-0.8.5/docs/contributing.rst` & `boa-framework-0.8.6/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/examples/cached_notebooks/example_optimization_results.ipynb` & `boa-framework-0.8.6/docs/examples/cached_notebooks/example_optimization_results.ipynb`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/examples/example_py_run.rst` & `boa-framework-0.8.6/docs/examples/example_py_run.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/examples/load_moo_scheduler.ipynb` & `boa-framework-0.8.6/docs/examples/load_moo_scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/examples/load_scheduler.ipynb` & `boa-framework-0.8.6/docs/examples/load_scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/examples/moo_optimization_run.ipynb` & `boa-framework-0.8.6/docs/examples/moo_optimization_run.ipynb`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/examples/optimization_run.ipynb` & `boa-framework-0.8.6/docs/examples/optimization_run.ipynb`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/examples/single_config.yaml` & `boa-framework-0.8.6/docs/examples/single_config.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/examples/wrapper.py` & `boa-framework-0.8.6/docs/examples/wrapper.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/index.rst` & `boa-framework-0.8.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/make.bat` & `boa-framework-0.8.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/references/rst_references.rst` & `boa-framework-0.8.6/docs/references/rst_references.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/user_guide/configuration.rst` & `boa-framework-0.8.6/docs/user_guide/configuration.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/user_guide/getting_started.rst` & `boa-framework-0.8.6/docs/user_guide/getting_started.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/user_guide/package_overview.rst` & `boa-framework-0.8.6/docs/user_guide/package_overview.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/docs/user_guide/run_script.rst` & `boa-framework-0.8.6/docs/user_guide/run_script.rst`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/environment_dev.yml` & `boa-framework-0.8.6/environment_dev.yml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - scipy
 - scikit-learn
 - click
 - panel
 - plotly>=5.10.0
 - notebook>=5.3
 - ipywidgets>=7.5
-- ax-platform==0.3.1
+- ax-platform==0.3.3
 - PyYAML
 
   ## Jupyter and sphinx jupyter
 - myst-nb
 - jupyter
 
   ## Aux Languages for testing
@@ -49,8 +49,8 @@
 
   ## Docs
   # we use external role, which is from v4.4. in conda this causes conflicts
   - sphinx>=4.4,<6  # <6 b/c pydata (<=0.12) doesn't work with sphinx 6, 4.4 is when certain sphinx options were introduced that we use
   - pydata-sphinx-theme>=0.13.0  # pydata 0.12 has a flyout menu bug
   - sphinxext-remoteliteralinclude
 
-  - -e .
+  - -e . --global-option="--no-deps"
```

### Comparing `boa-framework-0.8.5/pyproject.toml` & `boa-framework-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/setup.py` & `boa-framework-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tasks.py` & `boa-framework-0.8.6/tasks.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/conftest.py` & `boa-framework-0.8.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/integration_tests/test_dunder_main.py` & `boa-framework-0.8.6/tests/integration_tests/test_dunder_main.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/integration_tests/test_scripts.py` & `boa-framework-0.8.6/tests/integration_tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/integration_tests/test_storage.py` & `boa-framework-0.8.6/tests/integration_tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/other_langs/r_package_full/config.yaml` & `boa-framework-0.8.6/tests/scripts/other_langs/r_package_full/config.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/other_langs/r_package_full/run_model.R` & `boa-framework-0.8.6/tests/scripts/other_langs/r_package_full/run_model.R`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/other_langs/r_package_full/set_trial_status.R` & `boa-framework-0.8.6/tests/scripts/other_langs/r_package_full/set_trial_status.R`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/other_langs/r_package_full/write_configs.R` & `boa-framework-0.8.6/tests/scripts/other_langs/r_package_full/write_configs.R`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/other_langs/r_package_light/config.yaml` & `boa-framework-0.8.6/tests/scripts/other_langs/r_package_light/config.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/other_langs/r_package_light/run_model.R` & `boa-framework-0.8.6/tests/scripts/other_langs/r_package_light/run_model.R`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/other_langs/r_package_streamlined/config.yaml` & `boa-framework-0.8.6/tests/scripts/other_langs/r_package_streamlined/config.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/other_langs/r_package_streamlined/config_fail.yaml` & `boa-framework-0.8.6/tests/scripts/other_langs/r_package_streamlined/config_fail.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/other_langs/r_package_streamlined/run_model.R` & `boa-framework-0.8.6/tests/scripts/other_langs/r_package_streamlined/run_model.R`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/other_langs/r_utils/hartman6.R` & `boa-framework-0.8.6/tests/scripts/other_langs/r_utils/hartman6.R`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/stand_alone_opt_package/stand_alone_pkg_config.yaml` & `boa-framework-0.8.6/tests/scripts/stand_alone_opt_package/stand_alone_pkg_config.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/scripts/stand_alone_opt_package/wrapper.py` & `boa-framework-0.8.6/tests/scripts/stand_alone_opt_package/wrapper.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/test_configs/test_config_gen_strat1.yaml` & `boa-framework-0.8.6/tests/test_configs/test_config_gen_strat1.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/test_configs/test_config_metric.yaml` & `boa-framework-0.8.6/tests/test_configs/test_config_metric.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/test_configs/test_config_moo.yaml` & `boa-framework-0.8.6/tests/test_configs/test_config_moo.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/test_configs/test_config_param_parse.yaml` & `boa-framework-0.8.6/tests/test_configs/test_config_param_parse.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/test_configs/test_config_pass_through_metric.yaml` & `boa-framework-0.8.6/tests/test_configs/test_config_pass_through_metric.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/test_configs/test_config_soo.yaml` & `boa-framework-0.8.6/tests/test_configs/test_config_soo.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/test_configs/test_config_synth.yaml` & `boa-framework-0.8.6/tests/test_configs/test_config_synth.yaml`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/unit_tests/test_config_normalization.py` & `boa-framework-0.8.6/tests/unit_tests/test_config_normalization.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/unit_tests/test_generation_strategy.py` & `boa-framework-0.8.6/tests/unit_tests/test_generation_strategy.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/unit_tests/test_metrics.py` & `boa-framework-0.8.6/tests/unit_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/unit_tests/test_objective_loading.py` & `boa-framework-0.8.6/tests/unit_tests/test_objective_loading.py`

 * *Files identical despite different names*

### Comparing `boa-framework-0.8.5/tests/unit_tests/test_plots.py` & `boa-framework-0.8.6/tests/unit_tests/test_plots.py`

 * *Files identical despite different names*

