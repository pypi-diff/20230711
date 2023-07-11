# Comparing `tmp/power-grid-model-1.5.0rc9209002596082.tar.gz` & `tmp/power-grid-model-1.5.0rc9210200991489.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9209002596082.tar", last modified: Tue Jul 11 10:26:02 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9210200991489.tar", last modified: Tue Jul 11 13:32:15 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9209002596082.tar` & `power-grid-model-1.5.0rc9210200991489.tar`

### file list

```diff
@@ -1,622 +1,622 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.351322 power-grid-model-1.5.0rc9209002596082/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-11 10:26:02.351322 power-grid-model-1.5.0rc9209002596082/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 10:25:17.000000 power-grid-model-1.5.0rc9209002596082/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.275320 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.275320 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.267320 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.275320 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.279320 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28564 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.279320 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    68649 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.283320 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.283320 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.283320 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model_c/include/
--rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
--rw-r--r--   0 runner    (1001) docker     (123)    15757 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:26:02.351322 power-grid-model-1.5.0rc9209002596082/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.267320 power-grid-model-1.5.0rc9209002596082/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.283320 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.283320 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.287320 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    34661 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29948 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.283320 power-grid-model-1.5.0rc9209002596082/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-11 10:26:02.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-07-11 10:26:02.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:26:02.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 10:26:02.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 10:26:02.000000 power-grid-model-1.5.0rc9209002596082/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.275320 power-grid-model-1.5.0rc9209002596082/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.275320 power-grid-model-1.5.0rc9209002596082/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.271320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.287320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.287320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.287320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.291320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.291320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.291320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.295321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.295321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.295321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.299321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.299321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.299321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.271320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.271320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.271320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.299321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.303321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.303321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.303321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.303321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.307321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.307321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.307321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.307321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.271320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.311321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.311321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.311321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.311321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.315321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.315321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.315321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.315321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.319321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.271320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.271320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.319321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.319321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.271320 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.323321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.323321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.323321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.323321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.327321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.327321 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.275320 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.327321 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.331321 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.331321 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.331321 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58916 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.331321 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.335321 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.335321 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.335321 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.339321 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.339321 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.275320 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.339321 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.339321 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.343321 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.343321 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.343321 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.343321 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.343321 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.347321 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.347321 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.347321 power-grid-model-1.5.0rc9209002596082/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:26:02.347321 power-grid-model-1.5.0rc9209002596082/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-11 10:25:12.000000 power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.548237 power-grid-model-1.5.0rc9210200991489/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-11 13:32:15.548237 power-grid-model-1.5.0rc9210200991489/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 13:31:31.000000 power-grid-model-1.5.0rc9210200991489/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.484236 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.484236 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.480236 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.484236 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.488236 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28564 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.488236 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    68826 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.488236 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.488236 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.488236 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model_c/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15757 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:32:15.548237 power-grid-model-1.5.0rc9210200991489/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.480236 power-grid-model-1.5.0rc9210200991489/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.492236 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.492236 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.492236 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34661 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29948 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.492236 power-grid-model-1.5.0rc9210200991489/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-11 13:32:15.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-07-11 13:32:15.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:32:15.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 13:32:15.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 13:32:15.000000 power-grid-model-1.5.0rc9210200991489/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.484236 power-grid-model-1.5.0rc9210200991489/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.484236 power-grid-model-1.5.0rc9210200991489/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.480236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.492236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.492236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.496236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.496236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.496236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.500236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.500236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.500236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.500236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.504236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.504236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.504236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.480236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.480236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.480236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.504236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.504236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.508236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.508236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.508236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.508236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.508236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.512236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.512236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.480236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.512236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.516236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.516236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.516236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.520236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.520236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.520236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.520236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.524237 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.480236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.480236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.524237 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.524237 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.480236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.524237 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.524237 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.528236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.528236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.528236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.528236 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.484236 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.532236 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.532236 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.532236 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.532236 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58916 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.536237 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.536237 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.536237 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.536237 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.540237 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.540237 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.484236 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.540237 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.540237 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.540237 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.544237 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.544237 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.544237 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.544237 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.544237 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.548237 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.548237 power-grid-model-1.5.0rc9210200991489/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:32:15.548237 power-grid-model-1.5.0rc9210200991489/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-11 13:31:28.000000 power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9209002596082/LICENSE` & `power-grid-model-1.5.0rc9210200991489/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/PKG-INFO` & `power-grid-model-1.5.0rc9210200991489/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9209002596082
+Version: 1.5.0rc9210200991489
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9209002596082/README.md` & `power-grid-model-1.5.0rc9210200991489/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     explicit Base(BaseInput const& base_input) : id_{base_input.id} {
     }
     virtual ~Base() = default;
     ID id() const noexcept {
         return id_;
     }
     BaseOutput base_output(bool is_energized) const {
-        return BaseOutput{id_, is_energized};
+        return BaseOutput{id_, static_cast<IntS>(is_energized)};
     }
     virtual bool energized(bool is_connected_to_source) const = 0;
 
    private:
     ID id_;
 };
```

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,16 @@
             ((clock_13_ % 2) == 0 && (is_1_wye != is_3_wye)) ||
             // odd number is not possible, if both sides are wye winding or both sides are not wye winding.
             ((clock_13_ % 2) == 1 && (is_1_wye == is_3_wye))) {
             throw InvalidTransformerClock{id(), clock_13_};
         }
 
         // set clock to zero if it is 12
-        clock_12_ = clock_12_ % 12;
-        clock_13_ = clock_13_ % 12;
+        clock_12_ = static_cast<IntS>(clock_12_ % 12);
+        clock_13_ = static_cast<IntS>(clock_13_ % 12);
         // check tap bounds
         tap_pos_ = tap_limit(tap_pos_);
     }
 
     // override getter
     double base_i_1() const final {
         return base_i_1_;
@@ -275,93 +275,93 @@
             return std::make_tuple(u1, u2, u3);
         }();
 
         auto const [uk_T1, uk_T2, uk_T3] = calculate_uk();
         auto const [pk_T1, pk_T2, pk_T3] = calculate_pk();
 
         TransformerInput const transformer_input_T1{
-            {{2}, 0, 1, status_1(), true},  // {{id}, from_node, to_node, from_status, to_status}
-            u1,                             // u1
-            u1,                             // u2
-            sn_1_,                          // sn
-            uk_T1,                          // uk
-            pk_T1,                          // pk
-            i0_,                            // i0
-            p0_,                            // p0
-            WindingType::wye_n,             // winding_from
-            WindingType::wye_n,             // winding_to
-            0,                              // clock
-            BranchSide::from,               // tap_side
-            0,                              // tap_pos
-            0,                              // tap_min
-            0,                              // tap_max
-            0,                              // tap_nom
-            0.0,                            // tap_size
-            nan,                            // uk_min
-            nan,                            // uk_max
-            nan,                            // pk_min
-            nan,                            // pk_max
-            z_grounding_1_.real(),          // r_grounding_from
-            z_grounding_1_.imag(),          // x_grounding_from
-            0,                              // r_grounding_to
-            0                               // x_grounding_to
+            {{2}, 0, 1, static_cast<IntS>(status_1()), true},  // {{id}, from_node, to_node, from_status, to_status}
+            u1,                                                // u1
+            u1,                                                // u2
+            sn_1_,                                             // sn
+            uk_T1,                                             // uk
+            pk_T1,                                             // pk
+            i0_,                                               // i0
+            p0_,                                               // p0
+            WindingType::wye_n,                                // winding_from
+            WindingType::wye_n,                                // winding_to
+            0,                                                 // clock
+            BranchSide::from,                                  // tap_side
+            0,                                                 // tap_pos
+            0,                                                 // tap_min
+            0,                                                 // tap_max
+            0,                                                 // tap_nom
+            0.0,                                               // tap_size
+            nan,                                               // uk_min
+            nan,                                               // uk_max
+            nan,                                               // pk_min
+            nan,                                               // pk_max
+            z_grounding_1_.real(),                             // r_grounding_from
+            z_grounding_1_.imag(),                             // x_grounding_from
+            0,                                                 // r_grounding_to
+            0                                                  // x_grounding_to
         };
         TransformerInput const transformer_input_T2{
-            {{2}, 0, 1, status_2(), true},      // {{id}, from_node, to_node, from_status, to_status}
-            u2,                                 // u1
-            u1,                                 // u2
-            sn_2_,                              // sn
-            uk_T2,                              // uk
-            pk_T2,                              // pk
-            0.0,                                // i0
-            0.0,                                // p0
-            winding_2_,                         // winding_from
-            winding_1_,                         // winding_to
-            static_cast<IntS>(12 - clock_12_),  // clock, reversed
-            BranchSide::from,                   // tap_side
-            0,                                  // tap_pos
-            0,                                  // tap_min
-            0,                                  // tap_max
-            0,                                  // tap_nom
-            0.0,                                // tap_size
-            nan,                                // uk_min
-            nan,                                // uk_max
-            nan,                                // pk_min
-            nan,                                // pk_max
-            z_grounding_2_.real(),              // r_grounding_from
-            z_grounding_2_.imag(),              // x_grounding_from
-            0,                                  // r_grounding_to
-            0                                   // x_grounding_to
+            {{2}, 0, 1, static_cast<IntS>(status_2()), true},  // {{id}, from_node, to_node, from_status, to_status}
+            u2,                                                // u1
+            u1,                                                // u2
+            sn_2_,                                             // sn
+            uk_T2,                                             // uk
+            pk_T2,                                             // pk
+            0.0,                                               // i0
+            0.0,                                               // p0
+            winding_2_,                                        // winding_from
+            winding_1_,                                        // winding_to
+            static_cast<IntS>(12 - clock_12_),                 // clock, reversed
+            BranchSide::from,                                  // tap_side
+            0,                                                 // tap_pos
+            0,                                                 // tap_min
+            0,                                                 // tap_max
+            0,                                                 // tap_nom
+            0.0,                                               // tap_size
+            nan,                                               // uk_min
+            nan,                                               // uk_max
+            nan,                                               // pk_min
+            nan,                                               // pk_max
+            z_grounding_2_.real(),                             // r_grounding_from
+            z_grounding_2_.imag(),                             // x_grounding_from
+            0,                                                 // r_grounding_to
+            0                                                  // x_grounding_to
         };
         TransformerInput const transformer_input_T3{
-            {{2}, 0, 1, status_3(), true},      // {{id}, from_node, to_node, from_status, to_status}
-            u3,                                 // u1
-            u1,                                 // u2
-            sn_3_,                              // sn
-            uk_T3,                              // uk
-            pk_T3,                              // pk
-            0.0,                                // i0
-            0.0,                                // p0
-            winding_3_,                         // winding_from
-            winding_1_,                         // winding_to
-            static_cast<IntS>(12 - clock_13_),  // clock, reversed
-            BranchSide::from,                   // tap_side
-            0,                                  // tap_pos
-            0,                                  // tap_min
-            0,                                  // tap_max
-            0,                                  // tap_nom
-            0.0,                                // tap_size
-            nan,                                // uk_min
-            nan,                                // uk_max
-            nan,                                // pk_min
-            nan,                                // pk_max
-            z_grounding_3_.real(),              // r_grounding_from
-            z_grounding_3_.imag(),              // x_grounding_from
-            0,                                  // r_grounding_to
-            0                                   // x_grounding_to
+            {{2}, 0, 1, static_cast<IntS>(status_3()), true},  // {{id}, from_node, to_node, from_status, to_status}
+            u3,                                                // u1
+            u1,                                                // u2
+            sn_3_,                                             // sn
+            uk_T3,                                             // uk
+            pk_T3,                                             // pk
+            0.0,                                               // i0
+            0.0,                                               // p0
+            winding_3_,                                        // winding_from
+            winding_1_,                                        // winding_to
+            static_cast<IntS>(12 - clock_13_),                 // clock, reversed
+            BranchSide::from,                                  // tap_side
+            0,                                                 // tap_pos
+            0,                                                 // tap_min
+            0,                                                 // tap_max
+            0,                                                 // tap_nom
+            0.0,                                               // tap_size
+            nan,                                               // uk_min
+            nan,                                               // uk_max
+            nan,                                               // pk_min
+            nan,                                               // pk_max
+            z_grounding_3_.real(),                             // r_grounding_from
+            z_grounding_3_.imag(),                             // x_grounding_from
+            0,                                                 // r_grounding_to
+            0                                                  // x_grounding_to
         };
 
         Transformer const T1{transformer_input_T1, u1_rated_, u1_rated_};
         Transformer const T2{transformer_input_T2, u2_rated_, u1_rated_};
         Transformer const T3{transformer_input_T3, u3_rated_, u1_rated_};
 
         return {T1, T2, T3};
```

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             // even number is not possible if one side is wye winding and the other side is not wye winding.
             ((clock_ % 2) == 0 && (is_from_wye != is_to_wye)) ||
             // odd number is not possible, if both sides are wye winding or both sides are not wye winding.
             ((clock_ % 2) == 1 && (is_from_wye == is_to_wye))) {
             throw InvalidTransformerClock{id(), clock_};
         }
         // set clock to zero if it is 12
-        clock_ = clock_ % 12;
+        clock_ = static_cast<IntS>(clock_ % 12);
         // check tap bounds
         tap_pos_ = tap_limit(tap_pos_);
     }
 
     // override getter
     double base_i_from() const final {
         return base_i_from_;
```

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1008,25 +1008,28 @@
         // get connection info
         ComponentConnections comp_conn;
         comp_conn.branch_connected.resize(comp_topo_->branch_node_idx.size());
         comp_conn.branch_phase_shift.resize(comp_topo_->branch_node_idx.size());
         comp_conn.branch3_connected.resize(comp_topo_->branch3_node_idx.size());
         comp_conn.branch3_phase_shift.resize(comp_topo_->branch3_node_idx.size());
         comp_conn.source_connected.resize(comp_topo_->source_node_idx.size());
-        std::transform(components_.template citer<Branch>().begin(), components_.template citer<Branch>().end(),
-                       comp_conn.branch_connected.begin(), [](Branch const& branch) {
-                           return BranchConnected{branch.from_status(), branch.to_status()};
-                       });
+        std::transform(
+            components_.template citer<Branch>().begin(), components_.template citer<Branch>().end(),
+            comp_conn.branch_connected.begin(), [](Branch const& branch) {
+                return BranchConnected{static_cast<IntS>(branch.from_status()), static_cast<IntS>(branch.to_status())};
+            });
         std::transform(components_.template citer<Branch>().begin(), components_.template citer<Branch>().end(),
                        comp_conn.branch_phase_shift.begin(), [](Branch const& branch) {
                            return branch.phase_shift();
                        });
         std::transform(components_.template citer<Branch3>().begin(), components_.template citer<Branch3>().end(),
                        comp_conn.branch3_connected.begin(), [](Branch3 const& branch3) {
-                           return Branch3Connected{branch3.status_1(), branch3.status_2(), branch3.status_3()};
+                           return Branch3Connected{static_cast<IntS>(branch3.status_1()),
+                                                   static_cast<IntS>(branch3.status_2()),
+                                                   static_cast<IntS>(branch3.status_3())};
                        });
         std::transform(components_.template citer<Branch3>().begin(), components_.template citer<Branch3>().end(),
                        comp_conn.branch3_phase_shift.begin(), [](Branch3 const& branch3) {
                            return branch3.phase_shift();
                        });
         std::transform(components_.template citer<Source>().begin(), components_.template citer<Source>().end(),
                        comp_conn.source_connected.begin(), [](Source const& source) {
```

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp` & `power-grid-model-1.5.0rc9210200991489/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/pyproject.toml` & `power-grid-model-1.5.0rc9210200991489/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/setup.py` & `power-grid-model-1.5.0rc9210200991489/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/__init__.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/data_handling.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/data_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9209002596082
+Version: 1.5.0rc9210200991489
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9209002596082/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9210200991489/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9210200991489/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/sc_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/three_phase_abc/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/three_phase_abc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/sc_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ab/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/sc_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_ac/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/sc_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_bc/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9210200991489/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/utils.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9209002596082/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9210200991489/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

