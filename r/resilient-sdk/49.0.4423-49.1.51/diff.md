# Comparing `tmp/resilient_sdk-49.0.4423.tar.gz` & `tmp/resilient_sdk-49.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_sdk-49.0.4423.tar", last modified: Thu Jun  1 15:59:18 2023, max compression
+gzip compressed data, was "resilient_sdk-49.1.51.tar", last modified: Tue Jul 11 16:15:16 2023, max compression
```

## Comparing `resilient_sdk-49.0.4423.tar` & `resilient_sdk-49.1.51.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.217552 resilient_sdk-49.0.4423/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8830 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2023-06-01 15:59:18.217552 resilient_sdk-49.0.4423/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/assets/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    62353 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/assets/IBM_Security_lockup_pos_RGB.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6354 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)      507 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8183 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/base_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36429 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/clone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36585 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/codegen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10400 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21294 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/docgen.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/cmds/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8445 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/ext/ext_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7602 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/extract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5757 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/run_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48148 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/data/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.893552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.893552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2853 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      454 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1105 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/
--rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      743 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      145 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/components/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3082 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/lib/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     7886 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/__init__.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_close_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_update_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)    10768 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/__init__.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      913 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4885 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/data/export.res.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      975 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/payload_samples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2018 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/tests/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3132 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      750 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/data/docgen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/data/docgen/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15077 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/docgen/templates/README.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/data/ext/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/data/ext/icons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/ext/icons/app_logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/ext/icons/company_logo.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/data/run_init/
--rw-rw-r--   0 travis    (2000) travis    (2000)      773 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/run_init/sdk_settings.json.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/data/validate/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18106 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/validate/.pylintrc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/data/validate/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/validate/templates/validate_report.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8225 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3006 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/jinja2_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53165 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/package_file_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3080 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/resilient_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      817 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_genson_overwrites.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65385 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28321 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_configs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86171 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_issue.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    15768 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      108 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1171 2023-06-01 15:59:18.221552 resilient_sdk-49.0.4423/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16904 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/tests/integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/integration/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/integration/test_installation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.909552 resilient_sdk-49.0.4423/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      806 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/.mock_sdk_settings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        3 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)    24687 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_app.log
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   224427 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    58851 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export.resz
--rw-rw-r--   0 travis    (2000) travis    (2000)   223680 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export_corrupt.res
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.909552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/
--rw-rw-r--   0 travis    (2000) travis    (2000)      627 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    57247 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191223 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/customize_old.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.909552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/
--rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    41671 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    41951 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   539154 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.945552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5843 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.949552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      712 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.949552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/
--rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      566 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.949552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.949552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.949552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6889 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.997552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.997552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_close_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_update_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.997552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.045552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    49696 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.049552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.049552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.101552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.101552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.157552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.157552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2381 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      741 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)    53354 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup_callable_data.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup_py_lines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2795 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   413882 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_reload_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_xml_test_report.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.165552 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)  3278485 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)   594886 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/export.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/orgs.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/session.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_mock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.165552 resilient_sdk-49.0.4423/tests/unit/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1830 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.165552 resilient_sdk-49.0.4423/tests/unit/test_cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.169552 resilient_sdk-49.0.4423/tests/unit/test_cmds/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6916 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/ext/test_ext_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_base_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20782 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_clone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34439 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_codegen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2736 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10659 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_docgen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1145 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_extract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5876 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_run_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23815 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.217552 resilient_sdk-49.0.4423/tests/unit/test_util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_jinja_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18754 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_package_file_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_resilient_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      470 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      947 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29770 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3988 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_configs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48045 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_issue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      991 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.525333 resilient_sdk-49.1.51/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8934 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3150 2023-07-11 16:15:16.525333 resilient_sdk-49.1.51/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.273332 resilient_sdk-49.1.51/assets/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    62353 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/assets/IBM_Security_lockup_pos_RGB.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.273332 resilient_sdk-49.1.51/resilient_sdk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6354 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/app.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.277332 resilient_sdk-49.1.51/resilient_sdk/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      507 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8183 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/base_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36429 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/clone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36585 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/codegen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10400 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21294 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/docgen.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.277332 resilient_sdk-49.1.51/resilient_sdk/cmds/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8445 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/ext/ext_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7602 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/extract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5757 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/run_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48148 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/cmds/validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.273332 resilient_sdk-49.1.51/resilient_sdk/data/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.269333 resilient_sdk-49.1.51/resilient_sdk/data/codegen/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.269333 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.277332 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2853 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      454 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.277332 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1105 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      534 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.269333 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.277332 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      743 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.277332 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      145 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.277332 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/components/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3082 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.277332 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/lib/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7886 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.277332 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/poller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/poller/__init__.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.281333 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/poller/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_close_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_update_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10768 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.281333 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/util/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/util/__init__.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      913 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4885 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.281333 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/util/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/util/data/export.res.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      975 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.269333 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/payload_samples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.281333 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2018 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.281333 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/tests/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3132 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      750 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.269333 resilient_sdk-49.1.51/resilient_sdk/data/docgen/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.281333 resilient_sdk-49.1.51/resilient_sdk/data/docgen/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15077 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/docgen/templates/README.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.273332 resilient_sdk-49.1.51/resilient_sdk/data/ext/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.281333 resilient_sdk-49.1.51/resilient_sdk/data/ext/icons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/ext/icons/app_logo.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/ext/icons/company_logo.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.281333 resilient_sdk-49.1.51/resilient_sdk/data/run_init/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      773 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/run_init/sdk_settings.json.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.281333 resilient_sdk-49.1.51/resilient_sdk/data/validate/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18106 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/validate/.pylintrc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.281333 resilient_sdk-49.1.51/resilient_sdk/data/validate/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/data/validate/templates/validate_report.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.285333 resilient_sdk-49.1.51/resilient_sdk/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8225 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3006 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/jinja2_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53165 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/package_file_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3080 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/resilient_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/sdk_argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      817 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/sdk_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/sdk_genson_overwrites.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65385 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/sdk_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28321 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/sdk_validate_configs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86171 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/sdk_validate_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/resilient_sdk/util/sdk_validate_issue.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.277332 resilient_sdk-49.1.51/resilient_sdk.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3150 2023-07-11 16:15:16.000000 resilient_sdk-49.1.51/resilient_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15768 2023-07-11 16:15:16.000000 resilient_sdk-49.1.51/resilient_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:15:16.000000 resilient_sdk-49.1.51/resilient_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2023-07-11 16:15:16.000000 resilient_sdk-49.1.51/resilient_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      108 2023-07-11 16:15:16.000000 resilient_sdk-49.1.51/resilient_sdk.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-07-11 16:15:16.000000 resilient_sdk-49.1.51/resilient_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1171 2023-07-11 16:15:16.529332 resilient_sdk-49.1.51/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.285333 resilient_sdk-49.1.51/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16904 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.285333 resilient_sdk-49.1.51/tests/integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/integration/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/integration/test_installation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.285333 resilient_sdk-49.1.51/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/.mock_sdk_settings.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        3 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24687 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_app.log
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   224427 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58851 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_export.resz
+-rw-rw-r--   0 travis    (2000) travis    (2000)   223680 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_export_corrupt.res
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.289332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      627 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    57247 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   191223 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/customize_old.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.289332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_app_zip_files/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41671 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41951 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   539154 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.273332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.289332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
+-rw-rw-r--   0 travis    (2000) travis    (2000)      214 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5843 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.289332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      712 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.273332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.289332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      566 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.289332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.293332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.313332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6889 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.317333 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.317333 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_close_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_update_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.353333 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      591 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.357333 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49696 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.361333 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.273332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.405332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.405332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.409333 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.457332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.457332 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2381 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      741 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53354 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/setup_callable_data.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/setup_py_lines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2795 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   413882 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_reload_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/mock_xml_test_report.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.465333 resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  3278485 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)   594886 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_data/export.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_data/orgs.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_data/session.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_mock.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.465333 resilient_sdk-49.1.51/tests/unit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1830 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_app.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.465333 resilient_sdk-49.1.51/tests/unit/test_cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.513332 resilient_sdk-49.1.51/tests/unit/test_cmds/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6916 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/ext/test_ext_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/test_base_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20782 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/test_clone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34439 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/test_codegen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2736 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/test_dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10659 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/test_docgen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1145 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/test_extract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5876 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/test_run_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23815 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_cmds/test_validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-11 16:15:16.525333 resilient_sdk-49.1.51/tests/unit/test_util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_util/test_jinja_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18754 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_util/test_package_file_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_util/test_resilient_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      470 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      947 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29770 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3988 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_validate_configs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48045 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_validate_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_validate_issue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      991 2023-07-11 16:13:50.000000 resilient_sdk-49.1.51/tox.ini
```

### Comparing `resilient_sdk-49.0.4423/CHANGES` & `resilient_sdk-49.1.51/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2023-07: version 49.1**
+
+* No major changes. Just bumping build number to coincide with other builds
+
 **2023-05: version 49.0**
 
 * Added support to create markdown files for Playbooks as they would have been created with Workflows.
   Includes automatic detection of global scripts in ``codegen`` when exporting playbooks. Expanded support for
   playbooks with ``docgen`` will be included in a future release
 
 **2023-04: version 48.1**
```

### Comparing `resilient_sdk-49.0.4423/PKG-INFO` & `resilient_sdk-49.1.51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient_sdk
-Version: 49.0.4423
+Version: 49.1.51
 Summary: Python SDK for developing Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-sdk
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-sdk-changes
```

### Comparing `resilient_sdk-49.0.4423/README.md` & `resilient_sdk-49.1.51/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/assets/IBM_Security_lockup_pos_RGB.png` & `resilient_sdk-49.1.51/assets/IBM_Security_lockup_pos_RGB.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/LICENSE` & `resilient_sdk-49.1.51/resilient_sdk/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/app.py` & `resilient_sdk-49.1.51/resilient_sdk/app.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/cmds/base_cmd.py` & `resilient_sdk-49.1.51/resilient_sdk/cmds/base_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/cmds/clone.py` & `resilient_sdk-49.1.51/resilient_sdk/cmds/clone.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/cmds/codegen.py` & `resilient_sdk-49.1.51/resilient_sdk/cmds/codegen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/cmds/dev.py` & `resilient_sdk-49.1.51/resilient_sdk/cmds/dev.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/cmds/docgen.py` & `resilient_sdk-49.1.51/resilient_sdk/cmds/docgen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/cmds/ext/ext_package.py` & `resilient_sdk-49.1.51/resilient_sdk/cmds/ext/ext_package.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/cmds/extract.py` & `resilient_sdk-49.1.51/resilient_sdk/cmds/extract.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/cmds/run_init.py` & `resilient_sdk-49.1.51/resilient_sdk/cmds/run_init.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/cmds/validate.py` & `resilient_sdk-49.1.51/resilient_sdk/cmds/validate.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/docgen/templates/README.md.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/docgen/templates/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/ext/icons/app_logo.png` & `resilient_sdk-49.1.51/resilient_sdk/data/ext/icons/app_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/ext/icons/company_logo.png` & `resilient_sdk-49.1.51/resilient_sdk/data/ext/icons/company_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/run_init/sdk_settings.json.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/run_init/sdk_settings.json.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/validate/.pylintrc` & `resilient_sdk-49.1.51/resilient_sdk/data/validate/.pylintrc`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/data/validate/templates/validate_report.md.jinja2` & `resilient_sdk-49.1.51/resilient_sdk/data/validate/templates/validate_report.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/constants.py` & `resilient_sdk-49.1.51/resilient_sdk/util/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 PATH_RES_DEFAULT_LOG_FILE = os.path.join(PATH_RES_DEFAULT_LOG_DIR, "app.log")
 
 LOGGER_NAME = "resilient_sdk_log"
 LOG_DIVIDER = "\n------------------------\n"
 ENV_VAR_DEV = "RES_SDK_DEV"
 ENV_VAR_APP_CONFIG_FILE = "APP_CONFIG_FILE"
 
-RESILIENT_LIBRARIES_VERSION = "49.0.0"
-RESILIENT_LIBRARIES_VERSION_DEV = "49.0.0"
+RESILIENT_LIBRARIES_VERSION = "49.1.0"
+RESILIENT_LIBRARIES_VERSION_DEV = "49.1.0"
 RESILIENT_VERSION_WITH_PROXY_SUPPORT = (42, 0, 0)
 CURRENT_SOAR_SERVER_VERSION = None
 MIN_SOAR_SERVER_VERSION_PLAYBOOKS = 44.0
 
 MIN_SUPPORTED_PY_VERSION = (3, 6)
 SDK_PACKAGE_NAME = "resilient-sdk"
 SDK_RESOURCE_NAME = "resilient_sdk"
```

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/jinja2_filters.py` & `resilient_sdk-49.1.51/resilient_sdk/util/jinja2_filters.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/package_file_helpers.py` & `resilient_sdk-49.1.51/resilient_sdk/util/package_file_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/resilient_objects.py` & `resilient_sdk-49.1.51/resilient_sdk/util/resilient_objects.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_argparse.py` & `resilient_sdk-49.1.51/resilient_sdk/util/sdk_argparse.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_exception.py` & `resilient_sdk-49.1.51/resilient_sdk/util/sdk_exception.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_genson_overwrites.py` & `resilient_sdk-49.1.51/resilient_sdk/util/sdk_genson_overwrites.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_helpers.py` & `resilient_sdk-49.1.51/resilient_sdk/util/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_configs.py` & `resilient_sdk-49.1.51/resilient_sdk/util/sdk_validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_helpers.py` & `resilient_sdk-49.1.51/resilient_sdk/util/sdk_validate_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_issue.py` & `resilient_sdk-49.1.51/resilient_sdk/util/sdk_validate_issue.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/resilient_sdk.egg-info/PKG-INFO` & `resilient_sdk-49.1.51/resilient_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient-sdk
-Version: 49.0.4423
+Version: 49.1.51
 Summary: Python SDK for developing Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-sdk
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-sdk-changes
```

### Comparing `resilient_sdk-49.0.4423/resilient_sdk.egg-info/SOURCES.txt` & `resilient_sdk-49.1.51/resilient_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/setup.cfg` & `resilient_sdk-49.1.51/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient >= 49.0
+	resilient >= 49.1
 	
 	genson    ~= 1.2
 	
 	jinja2    ~= 3.0; python_version >= "3.6"
 	
 	jinja2    ~= 2.0; python_version == "2.7"
```

### Comparing `resilient_sdk-49.0.4423/tests/conftest.py` & `resilient_sdk-49.1.51/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/helpers.py` & `resilient_sdk-49.1.51/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/integration/test_installation.py` & `resilient_sdk-49.1.51/tests/integration/test_installation.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/.mock_sdk_settings.json` & `resilient_sdk-49.1.51/tests/shared_mock_data/.mock_sdk_settings.json`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_app.log` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_app.log`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export.res` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export.resz` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_export.resz`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export_corrupt.res` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_export_corrupt.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/config.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/config.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/customize.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/customize.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/customize_old.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/customize_old.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/setup.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup_callable_data.txt` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/setup_callable_data.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup_py_lines.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_package_files/setup_py_lines.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_paths.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_reload_export.res` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_reload_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_xml_test_report.xml` & `resilient_sdk-49.1.51/tests/shared_mock_data/mock_xml_test_report.xml`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON` & `resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/export.JSON` & `resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_data/export.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/orgs.JSON` & `resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_data/orgs.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/session.JSON` & `resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_data/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_mock.py` & `resilient_sdk-49.1.51/tests/shared_mock_data/resilient_api_mock.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_app.py` & `resilient_sdk-49.1.51/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_cmds/ext/test_ext_package.py` & `resilient_sdk-49.1.51/tests/unit/test_cmds/ext/test_ext_package.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_base_cmd.py` & `resilient_sdk-49.1.51/tests/unit/test_cmds/test_base_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_clone.py` & `resilient_sdk-49.1.51/tests/unit/test_cmds/test_clone.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_codegen.py` & `resilient_sdk-49.1.51/tests/unit/test_cmds/test_codegen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_dev.py` & `resilient_sdk-49.1.51/tests/unit/test_cmds/test_dev.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_docgen.py` & `resilient_sdk-49.1.51/tests/unit/test_cmds/test_docgen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_extract.py` & `resilient_sdk-49.1.51/tests/unit/test_cmds/test_extract.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_run_init.py` & `resilient_sdk-49.1.51/tests/unit/test_cmds/test_run_init.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_validate.py` & `resilient_sdk-49.1.51/tests/unit/test_cmds/test_validate.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_util/test_jinja_filters.py` & `resilient_sdk-49.1.51/tests/unit/test_util/test_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_util/test_package_file_helpers.py` & `resilient_sdk-49.1.51/tests/unit/test_util/test_package_file_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_util/test_resilient_objects.py` & `resilient_sdk-49.1.51/tests/unit/test_util/test_resilient_objects.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_exception.py` & `resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_helpers.py` & `resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_configs.py` & `resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_helpers.py` & `resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_validate_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_issue.py` & `resilient_sdk-49.1.51/tests/unit/test_util/test_sdk_validate_issue.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-49.0.4423/tox.ini` & `resilient_sdk-49.1.51/tox.ini`

 * *Files identical despite different names*

