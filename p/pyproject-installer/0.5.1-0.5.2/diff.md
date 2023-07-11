# Comparing `tmp/pyproject_installer-0.5.1.tar.gz` & `tmp/pyproject_installer-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_installer-0.5.1.tar", last modified: Thu Jun  1 14:08:57 2023, max compression
+gzip compressed data, was "pyproject_installer-0.5.2.tar", last modified: Tue Jul 11 08:42:22 2023, max compression
```

## Comparing `pyproject_installer-0.5.1.tar` & `pyproject_installer-0.5.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0       78 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/__init__.py
--rw-r--r--   0        0        0    16053 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/__main__.py
--rw-r--r--   0        0        0      317 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/codes.py
--rw-r--r--   0        0        0      391 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/errors.py
--rw-r--r--   0        0        0       18 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/version.py
--rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/__init__.py
--rw-r--r--   0        0        0      501 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8926 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0    10194 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/markers.py
--rw-r--r--   0        0        0    16397 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/metadata.py
--rw-r--r--   0        0        0     3287 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18106 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16326 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/version.py
--rw-r--r--   0        0        0      396 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      172 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/build_cmd/__init__.py
--rw-r--r--   0        0        0     4477 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/build_cmd/_build.py
--rw-r--r--   0        0        0      206 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/__init__.py
--rw-r--r--   0        0        0      181 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/_deps_command.py
--rw-r--r--   0        0        0     9067 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/deps_config.py
--rw-r--r--   0        0        0      728 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/__init__.py
--rw-r--r--   0        0        0      190 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/collector.py
--rw-r--r--   0        0        0     2358 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/hatch.py
--rw-r--r--   0        0        0     1306 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/metadata.py
--rw-r--r--   0        0        0     1361 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pdm.py
--rw-r--r--   0        0        0      825 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pep517.py
--rw-r--r--   0        0        0      679 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pep518.py
--rw-r--r--   0        0        0     1062 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py
--rw-r--r--   0        0        0     2481 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/poetry.py
--rw-r--r--   0        0        0     2239 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/tox.py
--rw-r--r--   0        0        0       73 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/install_cmd/__init__.py
--rw-r--r--   0        0        0     6215 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/install_cmd/_install.py
--rw-r--r--   0        0        0      270 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/__init__.py
--rw-r--r--   0        0        0     9335 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/build_backend.py
--rw-r--r--   0        0        0      913 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/entry_points.py
--rw-r--r--   0        0        0      193 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/normalization.py
--rw-r--r--   0        0        0     1811 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/scripts.py
--rw-r--r--   0        0        0    10893 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/wheel.py
--rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/backend_helper/__init__.py
--rw-r--r--   0        0        0     5872 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/backend_helper/backend_caller.py
--rw-r--r--   0        0        0       65 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/run_cmd/__init__.py
--rw-r--r--   0        0        0      430 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/run_cmd/_run_command.py
--rw-r--r--   0        0        0     7104 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/run_cmd/_run_env.py
--rw-r--r--   0        0        0      172 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/__init__.py
--rw-r--r--   0        0        0      367 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/common.py
--rw-r--r--   0        0        0     2092 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/config.py
--rw-r--r--   0        0        0     8581 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/metadata.py
--rw-r--r--   0        0        0     5559 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/sdist.py
--rw-r--r--   0        0        0     6922 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/wheel.py
--rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      396 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0     7856 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     5082 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     4144 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/integration/test_backends.py
--rw-r--r--   0        0        0     1719 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/integration/test_buildable.py
--rw-r--r--   0        0        0     2238 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/integration/test_config_settings.py
--rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/__init__.py
--rw-r--r--   0        0        0    31635 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_main.py
--rw-r--r--   0        0        0       92 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_version.py
--rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_build/__init__.py
--rw-r--r--   0        0        0      509 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_build/conftest.py
--rw-r--r--   0        0        0    15784 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_build/test_backend_caller.py
--rw-r--r--   0        0        0    12189 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_build/test_builder.py
--rw-r--r--   0        0        0     8179 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_build/test_pyproject_parser.py
--rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_deps/__init__.py
--rw-r--r--   0        0        0      495 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_deps/conftest.py
--rw-r--r--   0        0        0    30305 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_deps/test_collectors.py
--rw-r--r--   0        0        0    23966 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_deps/test_deps_config.py
--rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_install/__init__.py
--rw-r--r--   0        0        0    17931 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_install/test_installer.py
--rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_run/__init__.py
--rw-r--r--   0        0        0    18875 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_run/test_env.py
--rw-r--r--   0        0        0    17234 2023-06-01 14:08:57.000000 pyproject_installer-0.5.1/PKG-INFO
--rw-r--r--   0        0        0    16282 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/README.md
--rw-r--r--   0        0        0     3464 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1024 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/LICENSE
+-rw-r--r--   0        0        0       78 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/__init__.py
+-rw-r--r--   0        0        0    16053 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/__main__.py
+-rw-r--r--   0        0        0      317 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/codes.py
+-rw-r--r--   0        0        0      391 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/errors.py
+-rw-r--r--   0        0        0       18 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/version.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/__init__.py
+-rw-r--r--   0        0        0      501 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0     3287 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      396 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0      172 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/build_cmd/__init__.py
+-rw-r--r--   0        0        0     4477 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/build_cmd/_build.py
+-rw-r--r--   0        0        0      206 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/_deps_command.py
+-rw-r--r--   0        0        0     9272 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/deps_config.py
+-rw-r--r--   0        0        0      728 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/collector.py
+-rw-r--r--   0        0        0     2358 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/hatch.py
+-rw-r--r--   0        0        0     1306 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/metadata.py
+-rw-r--r--   0        0        0     1361 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pdm.py
+-rw-r--r--   0        0        0      825 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pep517.py
+-rw-r--r--   0        0        0      679 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pep518.py
+-rw-r--r--   0        0        0     1062 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py
+-rw-r--r--   0        0        0     2481 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/poetry.py
+-rw-r--r--   0        0        0     2239 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/tox.py
+-rw-r--r--   0        0        0       73 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/install_cmd/__init__.py
+-rw-r--r--   0        0        0     6215 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/install_cmd/_install.py
+-rw-r--r--   0        0        0      270 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/__init__.py
+-rw-r--r--   0        0        0     9335 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/build_backend.py
+-rw-r--r--   0        0        0      913 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/entry_points.py
+-rw-r--r--   0        0        0      193 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/normalization.py
+-rw-r--r--   0        0        0     1811 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/scripts.py
+-rw-r--r--   0        0        0    10893 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/wheel.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/backend_helper/__init__.py
+-rw-r--r--   0        0        0     5872 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/backend_helper/backend_caller.py
+-rw-r--r--   0        0        0       65 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/run_cmd/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/run_cmd/_run_command.py
+-rw-r--r--   0        0        0     7104 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/run_cmd/_run_env.py
+-rw-r--r--   0        0        0      172 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/__init__.py
+-rw-r--r--   0        0        0      367 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/common.py
+-rw-r--r--   0        0        0     2092 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/config.py
+-rw-r--r--   0        0        0     8581 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/metadata.py
+-rw-r--r--   0        0        0     5559 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/sdist.py
+-rw-r--r--   0        0        0     6922 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/wheel.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0     7856 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0     5082 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/integration/conftest.py
+-rw-r--r--   0        0        0     4144 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/integration/test_backends.py
+-rw-r--r--   0        0        0     1719 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/integration/test_buildable.py
+-rw-r--r--   0        0        0     2238 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/integration/test_config_settings.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0    31635 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_main.py
+-rw-r--r--   0        0        0       92 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_version.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_build/__init__.py
+-rw-r--r--   0        0        0      509 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_build/conftest.py
+-rw-r--r--   0        0        0    15784 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_build/test_backend_caller.py
+-rw-r--r--   0        0        0    12189 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_build/test_builder.py
+-rw-r--r--   0        0        0     8179 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_build/test_pyproject_parser.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_deps/__init__.py
+-rw-r--r--   0        0        0      495 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_deps/conftest.py
+-rw-r--r--   0        0        0    30288 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_deps/test_collectors.py
+-rw-r--r--   0        0        0    25247 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_deps/test_deps_config.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_install/__init__.py
+-rw-r--r--   0        0        0    17931 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_install/test_installer.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_run/__init__.py
+-rw-r--r--   0        0        0    18875 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_run/test_env.py
+-rw-r--r--   0        0        0    17234 2023-07-11 08:42:22.000000 pyproject_installer-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     3464 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    16282 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/README.md
+-rw-r--r--   0        0        0     1024 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/LICENSE
```

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/__main__.py` & `pyproject_installer-0.5.2/src/pyproject_installer/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_elffile.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_manylinux.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_musllinux.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_parser.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_structures.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_tokenizer.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/markers.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/metadata.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/requirements.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/specifiers.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/tags.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/utils.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/version.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/_parser.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/_re.py` & `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/build_cmd/_build.py` & `pyproject_installer-0.5.2/src/pyproject_installer/build_cmd/_build.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/deps_config.py` & `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/deps_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,38 +174,43 @@
 
         verify: do sync of selected sources, but print the diff on
         stdout and raise DepsUnsyncedError if sources were unsynced before
         """
         diff = {}
         for srcname, source in self.iter_sources(srcnames):
             synced_deps = set(
-                self.collect(
-                    source["srctype"],
-                    srcargs=source.get("srcargs", ()),
+                map(
+                    requirements.Requirement,
+                    self.collect(
+                        source["srctype"],
+                        srcargs=source.get("srcargs", ()),
+                    ),
                 )
             )
 
-            stored_deps = set(source.get("deps", ()))
+            stored_deps = set(
+                map(requirements.Requirement, source.get("deps", ()))
+            )
 
             if stored_deps == synced_deps:
                 continue
 
             new_deps = synced_deps - stored_deps
             if new_deps:
                 if srcname not in diff:
                     diff[srcname] = {}
-                diff[srcname]["new_deps"] = sorted(new_deps)
+                diff[srcname]["new_deps"] = sorted(map(str, new_deps))
 
             extra_deps = stored_deps - synced_deps
             if extra_deps:
                 if srcname not in diff:
                     diff[srcname] = {}
-                diff[srcname]["extra_deps"] = sorted(extra_deps)
+                diff[srcname]["extra_deps"] = sorted(map(str, extra_deps))
 
-            source["deps"] = sorted(synced_deps)
+            source["deps"] = sorted(map(str, synced_deps))
 
         self.save()
 
         if verify and diff:
             self._show(diff)
             raise DepsUnsyncedError
 
@@ -271,11 +276,11 @@
                         set(
                             self.depformat(
                                 parsed_req, depformat, depformatextra
                             )
                         )
                     )
                 else:
-                    deps.add(req)
+                    deps.add(str(parsed_req))
 
         for dep in sorted(deps):
             sys.stdout.write(dep + "\n")
```

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/__init__.py` & `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/hatch.py` & `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/hatch.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/metadata.py` & `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pdm.py` & `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pdm.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pep517.py` & `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pep517.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pep518.py` & `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pep518.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py` & `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/poetry.py` & `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/poetry.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/tox.py` & `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/tox.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/install_cmd/_install.py` & `pyproject_installer-0.5.2/src/pyproject_installer/install_cmd/_install.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/lib/build_backend.py` & `pyproject_installer-0.5.2/src/pyproject_installer/lib/build_backend.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/lib/entry_points.py` & `pyproject_installer-0.5.2/src/pyproject_installer/lib/entry_points.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/lib/scripts.py` & `pyproject_installer-0.5.2/src/pyproject_installer/lib/scripts.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/lib/wheel.py` & `pyproject_installer-0.5.2/src/pyproject_installer/lib/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/lib/backend_helper/backend_caller.py` & `pyproject_installer-0.5.2/src/pyproject_installer/lib/backend_helper/backend_caller.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/src/pyproject_installer/run_cmd/_run_env.py` & `pyproject_installer-0.5.2/src/pyproject_installer/run_cmd/_run_env.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/backend/config.py` & `pyproject_installer-0.5.2/backend/config.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/backend/metadata.py` & `pyproject_installer-0.5.2/backend/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/backend/sdist.py` & `pyproject_installer-0.5.2/backend/sdist.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/backend/wheel.py` & `pyproject_installer-0.5.2/backend/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/backend/_vendor/tomli/_parser.py` & `pyproject_installer-0.5.2/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/backend/_vendor/tomli/_re.py` & `pyproject_installer-0.5.2/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/conftest.py` & `pyproject_installer-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/integration/conftest.py` & `pyproject_installer-0.5.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/integration/test_backends.py` & `pyproject_installer-0.5.2/tests/integration/test_backends.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/integration/test_buildable.py` & `pyproject_installer-0.5.2/tests/integration/test_buildable.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/integration/test_config_settings.py` & `pyproject_installer-0.5.2/tests/integration/test_config_settings.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/unit/test_main.py` & `pyproject_installer-0.5.2/tests/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/unit/test_build/test_backend_caller.py` & `pyproject_installer-0.5.2/tests/unit/test_build/test_backend_caller.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/unit/test_build/test_builder.py` & `pyproject_installer-0.5.2/tests/unit/test_build/test_builder.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/unit/test_build/test_pyproject_parser.py` & `pyproject_installer-0.5.2/tests/unit/test_build/test_pyproject_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/unit/test_deps/test_collectors.py` & `pyproject_installer-0.5.2/tests/unit/test_deps/test_collectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,33 +164,33 @@
 
     return _pdm_deps
 
 
 PEP508_DEPS_DATA = (
     ([], []),
     (["foo"], ["foo"]),
-    (["foo == 1.0"], ["foo == 1.0"]),
+    (["foo == 1.0"], ["foo==1.0"]),
     (
         ["foo @ https://example.com/foo.zip"],
-        ["foo @ https://example.com/foo.zip"],
+        ["foo@ https://example.com/foo.zip"],
     ),
-    (["foo [test]"], ["foo [test]"]),
-    (["foo [test] > 1.0"], ["foo [test] > 1.0"]),
-    (["foo [test] > 1.0", "bar"], ["bar", "foo [test] > 1.0"]),
+    (["foo [test]"], ["foo[test]"]),
+    (["foo [test] > 1.0"], ["foo[test]>1.0"]),
+    (["foo [test] > 1.0", "bar"], ["bar", "foo[test]>1.0"]),
     (["Fo_.--o"], ["Fo_.--o"]),
     (["bar", "foo"], ["bar", "foo"]),
     (["foo", "bar"], ["bar", "foo"]),
-    (["foo", "bar > 1.0"], ["bar > 1.0", "foo"]),
+    (["foo", "bar > 1.0"], ["bar>1.0", "foo"]),
     (
-        ["foo", "bar > 1.0; python_version == '1.0'"],
-        ["bar > 1.0; python_version == '1.0'", "foo"],
+        ["foo", "bar > 1.0; python_version=='1.0'"],
+        ['bar>1.0; python_version == "1.0"', "foo"],
     ),
     (["_foo"], []),
     (["foo", "bar !> 1.0"], ["foo"]),
-    (["foo", "bar > 1.0; invalid_marker == '1.0'"], ["foo"]),
+    (["foo", "bar > 1.0; invalid_marker=='1.0'"], ["foo"]),
 )
 
 
 @pytest.mark.parametrize("deps_data", PEP508_DEPS_DATA)
 def test_metadata_collector_metadata(deps_data, pyproject_metadata, depsconfig):
     """Collection of core metadata via prepare_metadata_for_build_wheel"""
     # prepare source config
@@ -420,15 +420,15 @@
         ([], []),
         (['_foo = "*"'], []),
         (['foo = { git = "https://example.com/bar.git" }'], ["foo"]),
         (['foo = { url = "https://example.com/foo-1.0.tar.gz" }'], ["foo"]),
         (['foo = { version = "^2.0.1", python = "<3.11" }'], ["foo"]),
         (
             ['foo = {version = "^2.2", markers = "python_version <= \'3.4\'"}'],
-            ["foo;python_version <= '3.4'"],
+            ['foo; python_version <= "3.4"'],
         ),
         (
             ['foo = {version = "^2.2", markers = "invalid_marker == \'3.4\'"}'],
             ["foo"],
         ),
         (
             [
```

### Comparing `pyproject_installer-0.5.1/tests/unit/test_deps/test_deps_config.py` & `pyproject_installer-0.5.2/tests/unit/test_deps/test_deps_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,14 +473,53 @@
     assert actual_conf == deepcopy(input_conf)
 
     captured = capsys.readouterr()
     assert not captured.err
     assert not captured.out
 
 
+@pytest.mark.parametrize(
+    "old_reqs,new_reqs",
+    (
+        (["foo"], ["foo "]),
+        (["foo[a,b]"], ["foo [ a, b ]"]),
+        (["foo>1"], ["foo > 1"]),
+        (["foo;python_version=='3'"], ["foo ; python_version == '3'"]),
+    ),
+)
+def test_config_sync_verify_normalized_dep(
+    old_reqs, new_reqs, depsconfig, mock_collector, capsys
+):
+    """Sync unchanged source with verify and dependency normalization"""
+
+    action = "sync"
+
+    # prepare source config
+    input_conf = {
+        "sources": {
+            "foo": {
+                "srctype": "mock_collector",
+                "deps": old_reqs,
+            },
+        },
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    mock_collector(new_reqs)
+
+    deps_command(action, depsconfig_path, srcnames=[], verify=True)
+
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == input_conf
+
+    captured = capsys.readouterr()
+    assert not captured.err
+    assert not captured.out
+
+
 @pytest.mark.parametrize("select_data", NONEXISTENT_SOURCE_DATA)
 def test_config_sync_nonexistent_source(select_data, depsconfig, capsys):
     """Sync nonexistent source"""
 
     action = "sync"
     select, error = select_data
 
@@ -673,69 +712,77 @@
 
     captured = capsys.readouterr()
     assert not captured.err
     assert not captured.out
 
 
 @pytest.mark.parametrize(
-    "deps",
+    "data",
     (
-        ["foo [bar]"],
-        ["foo == 1.0.0"],
-        ["foo [bar,foobar] >= 2.8.1, == 2.8.*"],
-        ["foo [bar,foobar] >= 2.8.1, == 2.8.* ; python_version > '2.7'"],
+        (["foo"], ["foo"]),
+        (["foo [bar]"], ["foo[bar]"]),
+        (["foo == 1.0.0"], ["foo==1.0.0"]),
+        (
+            ["foo [bar,foobar] >= 2.8.1, == 2.8.*"],
+            ["foo[bar,foobar]==2.8.*,>=2.8.1"],
+        ),
+        (
+            ["foo [bar,foobar] >= 2.8.1, == 2.8.* ; python_version > '2.7'"],
+            ['foo[bar,foobar]==2.8.*,>=2.8.1; python_version > "2.7"'],
+        ),
     ),
 )
-def test_config_eval_default(deps, depsconfig, capsys):
-    """Eval source and print in PEP508 format"""
+def test_config_eval_default(data, depsconfig, capsys):
+    """Eval source and print in normalized(packaging) PEP508 format"""
 
     action = "eval"
+    deps, out = data
 
     # prepare source config
     input_conf = {"sources": {"foo": {"srctype": "metadata", "deps": deps}}}
     depsconfig_path = depsconfig(json.dumps(input_conf))
 
     deps_command(action, depsconfig_path, srcnames=[])
 
-    expected_out = "\n".join(deps) + "\n"
+    expected_out = "\n".join(out) + "\n"
 
     captured = capsys.readouterr()
     assert not captured.err
     assert captured.out == expected_out
 
 
 @pytest.mark.parametrize(
     "data",
     (
-        (["foo ; python_version>'2.7'"], ["foo ; python_version>'2.7'"]),
+        (["foo ; python_version>'2.7'"], ['foo; python_version > "2.7"']),
         (["foo ; python_version<'2.7'"], ""),
         (
             ["foo ; python_version>'2.7'", "bar ; python_version<'2.7'"],
-            ["foo ; python_version>'2.7'"],
+            ['foo; python_version > "2.7"'],
         ),
         (
             [
                 "foo ; python_version>'2.7'",
                 "bar ; python_version<'2.7'",
                 "foo1 ; extra == 'test'",
             ],
-            ["foo ; python_version>'2.7'"],
+            ['foo; python_version > "2.7"'],
         ),
         (
             ["foobar", "foo ; python_version>'2.7'"],
-            ["foo ; python_version>'2.7'", "foobar"],
+            ['foo; python_version > "2.7"', "foobar"],
         ),
         (
             [
                 "foo ; python_version>'2.7'",
                 "bar ; python_version<'2.7'",
                 'foo1 ; extra == "test"',
                 "foobar",
             ],
-            ["foo ; python_version>'2.7'", "foobar"],
+            ['foo; python_version > "2.7"', "foobar"],
         ),
     ),
 )
 def test_config_eval_markers(data, depsconfig, capsys):
     """Eval source with markers"""
 
     action = "eval"
@@ -757,31 +804,31 @@
 @pytest.mark.parametrize(
     "data",
     (
         (["foo"], ["foo"]),
         (["foo", 'bar ; extra == "doc"'], ["foo"]),
         (
             ['foo ; extra == "test"', 'bar ; extra == "doc"'],
-            ['foo ; extra == "test"'],
+            ['foo; extra == "test"'],
         ),
         (
             ['foo ; extra == "test"', 'bar ; extra == "doc"', "foobar"],
-            ['foo ; extra == "test"', "foobar"],
+            ['foo; extra == "test"', "foobar"],
         ),
         (
             [
                 'foo ; extra == "test"',
                 'bar ; extra == "doc"',
                 "foobar",
                 'foo1 ; extra == "test"',
                 "foobar1",
             ],
             [
-                'foo ; extra == "test"',
-                'foo1 ; extra == "test"',
+                'foo1; extra == "test"',
+                'foo; extra == "test"',
                 "foobar",
                 "foobar1",
             ],
         ),
         (['foo ; extra == "doc"'], ""),
     ),
 )
```

### Comparing `pyproject_installer-0.5.1/tests/unit/test_install/test_installer.py` & `pyproject_installer-0.5.2/tests/unit/test_install/test_installer.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/tests/unit/test_run/test_env.py` & `pyproject_installer-0.5.2/tests/unit/test_run/test_env.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/PKG-INFO` & `pyproject_installer-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-installer
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pyproject installer
 Author-email: Stanislav Levin <slev@altlinux.org>
 License: MIT
 Project-URL: source,https://github.com/stanislavlevin/pyproject_installer
 Project-URL: tracker,https://github.com/stanislavlevin/pyproject_installer/issues
 Keywords: packaging,PEP517,build,install
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyproject_installer-0.5.1/README.md` & `pyproject_installer-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/pyproject.toml` & `pyproject_installer-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.1/LICENSE` & `pyproject_installer-0.5.2/LICENSE`

 * *Files identical despite different names*

