# Comparing `tmp/libensemble-0.9.2.tar.gz` & `tmp/libensemble-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libensemble-0.9.2.tar", last modified: Wed Jul  6 22:37:56 2022, max compression
+gzip compressed data, was "libensemble-0.9.3.tar", last modified: Thu Oct 13 21:10:03 2022, max compression
```

## Comparing `libensemble-0.9.2.tar` & `libensemble-0.9.3.tar`

### file list

```diff
@@ -1,678 +1,694 @@
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.779381 libensemble-0.9.2/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2100 2022-07-06 22:32:09.000000 libensemble-0.9.2/.flake8
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    21992 2022-07-06 22:32:09.000000 libensemble-0.9.2/CHANGELOG.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3115 2022-07-06 22:32:09.000000 libensemble-0.9.2/CONTRIBUTING.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1759 2022-07-06 22:32:09.000000 libensemble-0.9.2/LICENSE
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      401 2022-07-06 22:32:09.000000 libensemble-0.9.2/MANIFEST.in
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1553 2022-07-06 22:37:56.779381 libensemble-0.9.2/PKG-INFO
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    14592 2022-07-06 22:32:09.000000 libensemble-0.9.2/README.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      269 2022-07-06 22:32:09.000000 libensemble-0.9.2/SUPPORT.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.723379 libensemble-0.9.2/docs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11639 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/FAQ.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      613 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/Makefile
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.723379 libensemble-0.9.2/docs/_static/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      501 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/_static/my_theme.css
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.723379 libensemble-0.9.2/docs/_templates/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      415 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/_templates/page.html
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6070 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/advanced_installation.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      159 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/bibliography.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9254 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/conf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       33 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/contributing.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.723379 libensemble-0.9.2/docs/data_structures/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1735 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/alloc_specs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4861 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/calc_status.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1321 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/data_structures.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1054 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/exit_criteria.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3220 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/gen_specs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6055 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/history_array.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10963 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/libE_specs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      882 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/persis_info.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2222 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/sim_specs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1688 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/work_dict.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1985 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/data_structures/worker_array.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.715379 libensemble-0.9.2/docs/dev_guide/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.723379 libensemble-0.9.2/docs/dev_guide/dev_API/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      390 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/developer_API.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      211 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/env_resources_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      300 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/history_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      187 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/manager_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       85 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/mpi_resources_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       87 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/node_resources_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      285 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/resources_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      171 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/rset_resources_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      166 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/scheduler_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      164 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/worker_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      354 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/dev_API/worker_resources_module.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.723379 libensemble-0.9.2/docs/dev_guide/release_management/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      277 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/release_management/release_index.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.727380 libensemble-0.9.2/docs/dev_guide/release_management/release_platforms/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      194 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/release_management/release_platforms/index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1809 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/release_management/release_platforms/rel_conda.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      918 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/release_management/release_platforms/rel_github.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1162 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/release_management/release_platforms/rel_pypi.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4291 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/release_management/release_platforms/rel_spack.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2911 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/dev_guide/release_management/release_process.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.727380 libensemble-0.9.2/docs/examples/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1507 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/alloc_funcs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1395 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/aposmm.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2751 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/calling_scripts.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      628 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/examples_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      129 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/fd_param_finder.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      462 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/gen_funcs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      624 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/sampling.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1591 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/sim_funcs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      531 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/surmise.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      757 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/tasmanian.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      183 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/examples/uniform_or_localopt.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.727380 libensemble-0.9.2/docs/executor/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      350 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/executor/balsam_2_executor.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      354 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/executor/ex_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3124 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/executor/executor.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      497 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/executor/legacy_balsam_executor.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1185 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/executor/mpi_executor.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6979 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/executor/overview.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.727380 libensemble-0.9.2/docs/function_guides/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6349 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/function_guides/allocator.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1328 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/function_guides/function_guide_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7766 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/function_guides/generator.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2846 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/function_guides/simulator.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7729 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/history_output_logging.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.735380 libensemble-0.9.2/docs/images/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    12163 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/ANL_CMYK.png
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13786 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/ECP_logo.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)  1001535 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/balsam2.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   295622 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/basic_6hc.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   192276 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/basic_6hc_simple.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   269938 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/central_balsam.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   429889 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/centralized_new.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   189953 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/centralized_new_detailed.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   256348 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/centralized_new_detailed_balsam.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   139065 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/diagram_with_persis.png
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.739380 libensemble-0.9.2/docs/images/diagram_xml/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   707087 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/diagram_xml/balsam2.xml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    73648 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/diagram_xml/centralized_new.xml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    73704 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/diagram_xml/distributed_new.xml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   638359 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/diagram_xml/funcx.xml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    74050 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/diagram_xml/persis_add_worker.xml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    73798 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/diagram_xml/persis_wasted_node.xml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   388503 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/distributed_new.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   171140 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/distributed_new_detailed.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   886431 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/funcx.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   367100 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/funcxmodel.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   337602 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/gen_v_fail_or_cancel.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   244843 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/history_gen1.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   244574 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/history_gen2.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    26836 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/history_init.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   205538 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/history_sim1.png
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    54153 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/libE_logo.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    44157 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/libE_logo_smaller.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    32035 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/libE_logo_white.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6292 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/libEnsemble_Logo.svg
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    26268 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/libe_opal_complete_v_killed_511w_2044sims_1030nodes.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    31284 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/libe_opal_util_v_time_511w_2044sims_1030nodes.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   372562 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/localopt_6hc.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   155087 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/logo_manager_worker.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   250428 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/persis_add_worker.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   233756 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/persis_wasted_node.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   373798 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/sampling_6hc.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    34960 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/sinex.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   354301 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/using_new.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    45757 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/variable_resources1.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    48241 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/variable_resources2.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    41003 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/variable_resources3.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    43963 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/variable_resources_larger_rsets1.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    46233 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/variable_resources_more_rsets1.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    52608 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/variable_resources_persis_gen1.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    37856 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/variable_resources_sched_opts.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1221 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/images/white.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1167 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       66 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/introduction.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3918 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/introduction_latex.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1125 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/known_issues.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      794 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/latex_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      125 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/libe_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7433 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/overview_usecases.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.739380 libensemble-0.9.2/docs/platforms/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4933 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/platforms/bebop.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6841 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/platforms/cori.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2421 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/platforms/example_scripts.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6728 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/platforms/perlmutter.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9849 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/platforms/platforms_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2790 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/platforms/spock_crusher.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4447 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/platforms/srun.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7440 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/platforms/summit.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    13063 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/platforms/theta.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      580 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/posters.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      426 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/programming_libE.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      435 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/references.bib
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       30 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/release_notes.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       45 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/requirements.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.739380 libensemble-0.9.2/docs/resource_manager/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10510 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/resource_manager/overview.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1661 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/resource_manager/resource_detection.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      415 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/resource_manager/resources_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      783 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/resource_manager/scheduler_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      413 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/resource_manager/worker_resources.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1439 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/resource_manager/zero_resource_workers.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      464 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/rst_formatting_guidelines
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6526 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/running_libE.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    13061 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/scipy2020.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3869 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/sim_gen_alloc_funcs.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.739380 libensemble-0.9.2/docs/tutorials/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    12439 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/tutorials/aposmm_tutorial.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    16084 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/tutorials/calib_cancel_tutorial.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    17748 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/tutorials/executor_forces_tutorial.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8594 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/tutorials/forces_gpu_tutorial.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    18543 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/tutorials/local_sine_tutorial.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      153 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/tutorials/tutorials.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      978 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/utilities.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1551 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/welcome.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10302 2022-07-06 22:32:09.000000 libensemble-0.9.2/docs/xSDK_policy_compatibility.md
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.739380 libensemble-0.9.2/examples/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      856 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/README.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.739380 libensemble-0.9.2/examples/alloc_funcs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2473 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/alloc_funcs/fast_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3178 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/alloc_funcs/fast_alloc_to_aposmm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3494 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/alloc_funcs/give_sim_work_first.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11635 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/alloc_funcs/start_only_persistent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4889 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/alloc_funcs/start_persistent_local_opt_gens.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.739380 libensemble-0.9.2/examples/calling_scripts/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.747380 libensemble-0.9.2/examples/calling_scripts/regression_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      461 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/.bal_coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      456 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      431 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/1d_sampling.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2232 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/check_libE_stats.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5374 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/common.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4132 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/dont_run_test_persistent_aposmm_pounders.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3537 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/dont_run_test_persistent_aposmm_tao_blmvm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2819 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/dont_run_test_persistent_aposmm_tao_nm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5147 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/dont_run_test_persistent_gp.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3321 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/script_test_balsam_hworld.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.747380 libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2496 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ECnoise.m
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      694 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       37 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/cleanup-balsam-test.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      787 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/configure-balsam-test.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4327 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/test_balsam_hworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      500 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/wrapper_obj_fun.m
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3646 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1882 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_1d_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1254 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_1d_sampling_from_yaml.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2517 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_1d_sampling_with_profile.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2021 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_evaluate_existing_sample.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2154 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_evaluate_mixed_sample.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3000 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_fast_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2217 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_heffte.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2849 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_inverse_bayes_example.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4564 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_dfols.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3210 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_exception.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4269 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_external_localopt.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3505 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_nlopt.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3695 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_periodic.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4810 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_scipy.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3080 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_timeout.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4770 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_with_grad.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2876 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_fd_param_finder.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4118 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_gp_multitask_ax.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4611 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_independent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9099 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_n_agent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9012 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_pds.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6891 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_prox_slide.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2921 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_sampling_CUDA_variable_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2873 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_sim_uniform_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4843 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_surmise_calib.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5433 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_surmise_killsims.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5928 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_tasmanian.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3940 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_tasmanian_async.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3384 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_uniform_gen_decides_stop.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2696 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_uniform_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2791 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_uniform_sampling_adv.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2772 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_uniform_sampling_async.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2428 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_uniform_sampling_nonblocking.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4227 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_stats_output.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2424 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_uniform_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5557 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_uniform_sampling_cancel.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4178 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_uniform_sampling_one_residual_at_a_time.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3043 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_uniform_sampling_then_persistent_localopt_runs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4162 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/regression_tests/test_uniform_sampling_with_variable_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4279 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/run_libe_forces.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      902 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/run_libe_forces_from_yaml.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7558 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/run_libensemble_on_warpx.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1721 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/calling_scripts/tutorial_calling.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.747380 libensemble-0.9.2/examples/gen_funcs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8058 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/gen_funcs/persistent_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6628 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/gen_funcs/sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4819 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/gen_funcs/uniform_or_localopt.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.747380 libensemble-0.9.2/examples/libE_submission_scripts/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      833 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/libE_submission_scripts/bebop_submit_slurm_central.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2803 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/libE_submission_scripts/bebop_submit_slurm_distrib.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1669 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/libE_submission_scripts/blues_script.pbs
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      705 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/libE_submission_scripts/bridges_submit_slurm_central.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1157 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/libE_submission_scripts/cori_submit.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      939 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/libE_submission_scripts/edtb_submit_pbspro_central.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      367 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/libE_submission_scripts/submit_slurm_simple.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1278 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/libE_submission_scripts/summit_submit_mproc.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3701 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/libE_submission_scripts/theta_submit_balsam.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1541 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/libE_submission_scripts/theta_submit_mproc.sh
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.747380 libensemble-0.9.2/examples/misc/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      586 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/misc/ps_nodes.sh
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.747380 libensemble-0.9.2/examples/sim_funcs/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.747380 libensemble-0.9.2/examples/sim_funcs/branin/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/sim_funcs/branin/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      599 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/sim_funcs/branin/branin.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1042 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/sim_funcs/branin/branin_obj.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       71 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/sim_funcs/branin/known_minima_and_func_values
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11278 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/sim_funcs/chwirut1.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6242 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/sim_funcs/executor_hworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      324 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/sim_funcs/helloworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8202 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/sim_funcs/six_hump_camel.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.719380 libensemble-0.9.2/examples/tutorials/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.747380 libensemble-0.9.2/examples/tutorials/aposmm/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    13701 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/aposmm/aposmm_tutorial_notebook.ipynb
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1816 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/aposmm/tutorial_aposmm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      633 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/aposmm/tutorial_six_hump_camel.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.747380 libensemble-0.9.2/examples/tutorials/forces_with_executor/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1178 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/forces_with_executor/build_forces.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13024 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/forces_with_executor/forces.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1424 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/forces_with_executor/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    22332 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/forces_with_executor/forces_tutorial_notebook.ipynb
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1832 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/forces_with_executor/run_libe_forces.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.751380 libensemble-0.9.2/examples/tutorials/images/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   295622 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/images/basic_6hc.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   372562 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/images/localopt_6hc.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   373798 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/images/sampling_6hc.png
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.751380 libensemble-0.9.2/examples/tutorials/simple_sine/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11697 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/simple_sine/sine_tutorial_notebook.ipynb
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1721 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/simple_sine/tutorial_calling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2016 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/simple_sine/tutorial_calling_mpi.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      751 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/simple_sine/tutorial_gen.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      376 2022-07-06 22:32:09.000000 libensemble-0.9.2/examples/tutorials/simple_sine/tutorial_sim.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.751380 libensemble-0.9.2/install/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1444 2022-07-06 22:32:09.000000 libensemble-0.9.2/install/configure_balsam_install.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       93 2022-07-06 22:32:09.000000 libensemble-0.9.2/install/environment.yml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      539 2022-07-06 22:32:09.000000 libensemble-0.9.2/install/find_mpi.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      105 2022-07-06 22:32:09.000000 libensemble-0.9.2/install/testing_requirements.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.751380 libensemble-0.9.2/libensemble/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      427 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/__init__.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.751380 libensemble-0.9.2/libensemble/alloc_funcs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      193 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/defaults.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2473 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/fast_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7462 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/fast_alloc_and_pausing.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3178 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/fast_alloc_to_aposmm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1593 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/give_pregenerated_work.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3494 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/give_sim_work_first.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3160 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/inverse_bayes_allocf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1939 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/only_one_gen_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3858 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/persistent_aposmm_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3231 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/start_fd_persistent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11635 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/start_only_persistent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    14138 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/start_persistent_consensus.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4889 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/alloc_funcs/start_persistent_local_opt_gens.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8677 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/api.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.755380 libensemble-0.9.2/libensemble/comms/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/comms/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    17754 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/comms/comms.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6400 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/comms/logs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3764 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/comms/mpi.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3607 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/comms/tcp_mgr.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.755380 libensemble-0.9.2/libensemble/executors/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      150 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/executors/__init__.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.755380 libensemble-0.9.2/libensemble/executors/balsam_executors/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      947 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/executors/balsam_executors/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    19156 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/executors/balsam_executors/balsam_executor.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    12463 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/executors/balsam_executors/legacy_balsam_executor.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    23426 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/executors/executor.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10074 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/executors/mpi_executor.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10051 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/executors/mpi_runner.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.755380 libensemble-0.9.2/libensemble/gen_funcs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      497 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    21944 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/aposmm_localopt_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    40148 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/old_aposmm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    32925 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_aposmm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10174 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_ax_multitask.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4950 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_fd_param_finder.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10437 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_gp.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2061 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_independent_optimize.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1486 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_inverse_bayes.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3485 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_n_agent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5334 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_pds.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4142 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_prox_slide.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8058 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8758 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_surmise_calib.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    14507 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/persistent_tasmanian.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6628 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2242 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/surmise_calib_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4819 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/gen_funcs/uniform_or_localopt.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9089 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/history.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      995 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/information_about_W
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    22304 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/libE.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1365 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/logger.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    24294 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/manager.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2131 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/message_numbers.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9841 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/output_directory.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.755380 libensemble-0.9.2/libensemble/resources/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/resources/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8786 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/resources/env_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8372 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/resources/mpi_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3732 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/resources/node_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    12253 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/resources/resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5263 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/resources/rset_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    14808 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/resources/scheduler.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    12317 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/resources/worker_resources.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.759380 libensemble-0.9.2/libensemble/sim_funcs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1119 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/alt_rosenbrock.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2544 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/borehole.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1875 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/borehole_kills.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.759380 libensemble-0.9.2/libensemble/sim_funcs/branin/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/branin/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      599 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/branin/branin.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1042 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/branin/branin_obj.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       71 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/branin/known_minima_and_func_values
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11278 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/chwirut1.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      353 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/comms_testing.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6242 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/executor_hworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1105 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/geomedian.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      720 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/heffte.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      324 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/helloworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      606 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/inverse_bayes.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1773 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/linear_regression.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1794 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/logistic_regression.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1286 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/nesterov_quadratic.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1338 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/noisy_vector_mapping.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      512 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/one_d_func.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      486 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/periodic_func.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2441 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/rosenbrock.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4206 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/run_line_check.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8202 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/six_hump_camel.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2766 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/surmise_test_function.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1767 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/sim_funcs/svm.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.759380 libensemble-0.9.2/libensemble/tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      732 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/__init__.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.759380 libensemble-0.9.2/libensemble/tests/deprecated_tests/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.759380 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.759380 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/bash_scripts/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1898 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/bash_scripts/setup_balsam_tests.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      291 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/env_setup_theta.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      732 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/readme.balsam_tests.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7837 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/readme.rst
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      259 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/reset_balsam_tests.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     3175 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/setup_balsam_tests.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2010 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_1__runjobs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2127 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_2__workerkill.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2986 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_3__managerkill.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.759380 libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2070 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/create_balsam_job.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1447 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/readme.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      641 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/set.balsam.database.sh
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.759380 libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      957 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/my_simtask.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1247 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/my_simtask.f90
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3280 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3663 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor_manager_poll.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4971 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor_multi.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1944 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/test_nan_func_old_aposmm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4092 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_logic.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2752 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_one_residual_at_a_time.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2487 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_pounders.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2857 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_pounders_splitcomm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2856 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_pounders_subcomm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3406 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_sim_dirs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4877 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_with_gradients.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.763380 libensemble-0.9.2/libensemble/tests/functionality_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      457 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2754 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_1d_uniform_sampling_with_comm_dup.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2786 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1791 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_calc_exception.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2502 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_cancel_in_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2396 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_comms.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2230 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_elapsed_time_abort.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3808 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_executor_hworld_pass_fail.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3596 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_executor_hworld_timeout.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3184 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_comms.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    13123 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4251 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners_subnode.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5050 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners_subnode_uneven.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4626 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners_supernode_uneven.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5254 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners_zrw_subnode_uneven.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5004 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners_zrw_supernode_uneven.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3341 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3514 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3748 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent_oversubscribe_rsets.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3243 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_sim_dirs_per_calc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3508 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_sim_dirs_per_worker.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2183 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_sim_dirs_with_exception.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4069 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_sim_dirs_with_gen_dirs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2600 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_sim_input_dir_option.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1982 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_worker_exceptions.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4385 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_zero_resource_workers.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4640 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/functionality_tests/test_zero_resource_workers_subnode.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.767380 libensemble-0.9.2/libensemble/tests/regression_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      461 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/.bal_coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      456 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      431 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/1d_sampling.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2232 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/check_libE_stats.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5374 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/common.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4132 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/dont_run_test_persistent_aposmm_pounders.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3537 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/dont_run_test_persistent_aposmm_tao_blmvm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2819 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/dont_run_test_persistent_aposmm_tao_nm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5147 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/dont_run_test_persistent_gp.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3321 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/script_test_balsam_hworld.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.767380 libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2496 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ECnoise.m
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      694 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       37 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/cleanup-balsam-test.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      787 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/configure-balsam-test.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4327 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/test_balsam_hworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      500 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/wrapper_obj_fun.m
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3646 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1882 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_1d_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1254 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_1d_sampling_from_yaml.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2517 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_1d_sampling_with_profile.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2021 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_evaluate_existing_sample.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2154 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_evaluate_mixed_sample.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3000 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_fast_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2217 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_heffte.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2849 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_inverse_bayes_example.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4564 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_dfols.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3210 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_exception.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4269 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_external_localopt.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3505 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_nlopt.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3695 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_periodic.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4810 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_scipy.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3080 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_timeout.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4770 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_with_grad.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2876 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_fd_param_finder.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4118 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_gp_multitask_ax.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4611 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_independent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9099 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_n_agent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9012 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_pds.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6891 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_prox_slide.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2921 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_sampling_CUDA_variable_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2873 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_sim_uniform_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4843 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_surmise_calib.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5433 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_surmise_killsims.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5928 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_tasmanian.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3940 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_tasmanian_async.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3384 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_uniform_gen_decides_stop.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2696 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_uniform_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2791 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_uniform_sampling_adv.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2772 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_uniform_sampling_async.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2428 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_uniform_sampling_nonblocking.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4227 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_stats_output.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2424 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_uniform_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5557 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_uniform_sampling_cancel.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4178 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_uniform_sampling_one_residual_at_a_time.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3043 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_uniform_sampling_then_persistent_localopt_runs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4162 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/regression_tests/test_uniform_sampling_with_variable_resources.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    26146 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/run-tests.sh
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.767380 libensemble-0.9.2/libensemble/tests/scaling_tests/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.719380 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.767380 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       60 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2056 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/define_apps.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2008 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7612 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2531 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/run_libe_forces_balsam.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2366 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/submit_libe_forces_remotely.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.767380 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1527 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/balsam_local.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      290 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/clone.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      899 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/forces.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4901 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2590 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/forces_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4548 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4279 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      902 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces_from_yaml.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.767380 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1178 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/build_forces.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13024 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/forces.c
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      885 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/build_forces.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5148 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4845 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces_AoS.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      916 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/readme.md
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_gpu/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_gpu/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1891 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_gpu/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2076 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_gpu/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2266 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_gpu/run_libe_forces.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      254 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_gpu/submit_perlmutter.sh
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_simple/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_simple/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1424 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_simple/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1413 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_simple/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1832 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_simple/run_libe_forces.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/funcx_forces/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       54 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/funcx_forces/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4739 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/funcx_forces/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1141 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/funcx_forces/funcx_forces.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1447 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/funcx_forces/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      394 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/funcx_forces/run_libe_forces_funcx.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/submission_scripts/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      363 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/submission_scripts/submit_slurm_simple.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1370 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/submission_scripts/summit_submit_mproc.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     3641 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/submission_scripts/theta_submit_balsam.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1563 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/forces/submission_scripts/theta_submit_mproc.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      148 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/note_moved_examples.md
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/scaling_tests/persistent_gp/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2975 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/persistent_gp/run_example.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      853 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/all_machine_specs.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     4470 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/plot_results.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2502 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/read_sim_output.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1925 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/readme.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       44 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/requirements.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7558 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/run_libensemble_on_warpx.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/sim/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8355 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/sim/inputs
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1413 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/summit_submit_mproc.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4023 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/warpx_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3284 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/write_sim_input.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.719380 libensemble-0.9.2/libensemble/tests/standalone_tests/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/standalone_tests/comms_test/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1839 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/comms_test/commtest.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      973 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/comms_test/readme.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       84 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/build.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      663 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/burn_time.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4772 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/killtest.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2587 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/log.autotest.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2411 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/log.burn_time_test_with_top.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1822 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/readme.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1011 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/sleep_and_print.c
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.771381 libensemble-0.9.2/libensemble/tests/standalone_tests/mpi_launch_test/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      679 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/mpi_launch_test/create_mpi_jobs.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      310 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/mpi_launch_test/helloworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      747 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/standalone_tests/mpi_launch_test/readme.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.775380 libensemble-0.9.2/libensemble/tests/unit_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      378 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      712 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/conftest.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      456 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/launch_busy.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3167 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/mpich-only_test_api.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2910 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/setup.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.775380 libensemble-0.9.2/libensemble/tests/unit_tests/simdir/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1359 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/simdir/borehole.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      210 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/simdir/c_startup.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      806 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/simdir/my_serialtask.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1166 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/simdir/my_simtask.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1247 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/simdir/my_simtask.f90
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       32 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/simdir/py_startup.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      560 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/simdir/test_example.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      560 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/simdir/test_example_badfuncs_attribute.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      544 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/simdir/test_example_badfuncs_notfound.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    16181 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_allocation_funcs_and_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10825 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_comms.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    12580 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_env_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    31017 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_executor.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    16832 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_history.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2568 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_launcher.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11661 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_libE_main.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4224 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_loc_stack.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1765 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_manager_main.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      221 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_mpi4py.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4061 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_node_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6017 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_persistent_aposmm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    24268 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_resource_scheduler.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    31212 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1501 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_scipy.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5557 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_sim_dir_properties.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4341 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_task_funcs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1556 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/test_timer.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1200 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests/tofix__test_worker.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.775380 libensemble-0.9.2/libensemble/tests/unit_tests_logger/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      404 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests_logger/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4404 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests_logger/test_logger.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.775380 libensemble-0.9.2/libensemble/tests/unit_tests_nompi/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      404 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests_nompi/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2634 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tests/unit_tests_nompi/test_aaa_comms.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.775380 libensemble-0.9.2/libensemble/tools/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      326 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tools/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    13870 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tools/alloc_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10648 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tools/check_inputs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    13550 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tools/consensus_subroutines.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2927 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tools/fields_keys.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1367 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tools/forkable_pdb.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8464 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tools/parse_args.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3680 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tools/persistent_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5633 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/tools/tools.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.775380 libensemble-0.9.2/libensemble/utils/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/utils/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3226 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/utils/launcher.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4221 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/utils/loc_stack.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2813 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/utils/timer.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       22 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/version.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    15099 2022-07-06 22:32:09.000000 libensemble-0.9.2/libensemble/worker.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.751380 libensemble-0.9.2/libensemble.egg-info/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1553 2022-07-06 22:37:56.000000 libensemble-0.9.2/libensemble.egg-info/PKG-INFO
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    30158 2022-07-06 22:37:56.000000 libensemble-0.9.2/libensemble.egg-info/SOURCES.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        1 2022-07-06 22:37:56.000000 libensemble-0.9.2/libensemble.egg-info/dependency_links.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      168 2022-07-06 22:37:56.000000 libensemble-0.9.2/libensemble.egg-info/requires.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       12 2022-07-06 22:37:56.000000 libensemble-0.9.2/libensemble.egg-info/top_level.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.779381 libensemble-0.9.2/scripts/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/__init__.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-07-06 22:37:56.779381 libensemble-0.9.2/scripts/balsam/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      517 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/balsam/plot_tasks_v_time.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      523 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/balsam/plot_util_v_time.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      514 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/balsam/plot_waiting_v_time.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      409 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/balsam/readme.rst
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     2474 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/compare_npy.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1630 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/plot_contours_and_history_points.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     3131 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/plot_libe_calcs_util_v_time.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     4186 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/plot_libe_histogram.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3709 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/plot_libe_tasks_util_v_time.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1772 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/plot_pareto_2d.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     2051 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/plot_pareto_3d.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1566 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/print_fields.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      838 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/print_npy.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      496 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/print_pickle.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1744 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/process_history_to_make_chart.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2306 2022-07-06 22:32:09.000000 libensemble-0.9.2/scripts/readme.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       38 2022-07-06 22:37:56.779381 libensemble-0.9.2/setup.cfg
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3749 2022-07-06 22:32:09.000000 libensemble-0.9.2/setup.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.385823 libensemble-0.9.3/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2105 2022-10-13 21:09:01.000000 libensemble-0.9.3/.flake8
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    23557 2022-10-13 21:09:01.000000 libensemble-0.9.3/CHANGELOG.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3115 2022-10-13 17:42:55.000000 libensemble-0.9.3/CONTRIBUTING.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1759 2022-10-13 17:42:55.000000 libensemble-0.9.3/LICENSE
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      401 2022-10-13 17:42:55.000000 libensemble-0.9.3/MANIFEST.in
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1533 2022-10-13 21:10:03.385823 libensemble-0.9.3/PKG-INFO
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    15191 2022-10-13 21:09:01.000000 libensemble-0.9.3/README.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      269 2022-10-13 17:42:55.000000 libensemble-0.9.3/SUPPORT.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.321823 libensemble-0.9.3/docs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14406 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/FAQ.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      613 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/Makefile
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.321823 libensemble-0.9.3/docs/_static/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      501 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/_static/my_theme.css
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.321823 libensemble-0.9.3/docs/_templates/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      415 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/_templates/page.html
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6070 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/advanced_installation.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      159 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/bibliography.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9332 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/conf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       33 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/contributing.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.325823 libensemble-0.9.3/docs/data_structures/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1735 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/data_structures/alloc_specs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4861 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/data_structures/calc_status.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1321 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/data_structures/data_structures.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1054 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/data_structures/exit_criteria.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3220 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/data_structures/gen_specs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6055 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/data_structures/history_array.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11131 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/data_structures/libE_specs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      882 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/data_structures/persis_info.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2222 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/data_structures/sim_specs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2125 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/data_structures/work_dict.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1985 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/data_structures/worker_array.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.313823 libensemble-0.9.3/docs/dev_guide/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.325823 libensemble-0.9.3/docs/dev_guide/dev_API/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      390 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/developer_API.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      211 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/env_resources_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      300 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/history_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      187 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/manager_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       85 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/mpi_resources_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       87 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/node_resources_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      285 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/resources_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      171 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/rset_resources_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      166 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/scheduler_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      164 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/worker_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      354 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/dev_API/worker_resources_module.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.325823 libensemble-0.9.3/docs/dev_guide/release_management/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      277 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/release_management/release_index.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.325823 libensemble-0.9.3/docs/dev_guide/release_management/release_platforms/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      194 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/release_management/release_platforms/index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1809 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/release_management/release_platforms/rel_conda.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      918 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/release_management/release_platforms/rel_github.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1162 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/release_management/release_platforms/rel_pypi.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4291 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/release_management/release_platforms/rel_spack.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2911 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/dev_guide/release_management/release_process.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.325823 libensemble-0.9.3/docs/examples/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1507 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/alloc_funcs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1395 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/aposmm.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2751 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/calling_scripts.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      628 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/examples_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      129 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/fd_param_finder.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      462 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/gen_funcs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      624 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/sampling.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1591 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/sim_funcs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      531 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/surmise.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      757 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/tasmanian.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      183 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/examples/uniform_or_localopt.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.325823 libensemble-0.9.3/docs/executor/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      350 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/executor/balsam_2_executor.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      354 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/executor/ex_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3284 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/executor/executor.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      497 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/executor/legacy_balsam_executor.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1348 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/executor/mpi_executor.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7007 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/executor/overview.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.325823 libensemble-0.9.3/docs/function_guides/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6349 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/function_guides/allocator.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1328 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/function_guides/function_guide_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8767 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/function_guides/generator.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2846 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/function_guides/simulator.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7729 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/history_output_logging.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.333823 libensemble-0.9.3/docs/images/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12163 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/ANL_CMYK.png
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13786 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/ECP_logo.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)  1001535 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/balsam2.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   295622 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/basic_6hc.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   192276 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/basic_6hc_simple.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   189953 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/centralized_new_detailed.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   256348 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/centralized_new_detailed_balsam.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   139065 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/diagram_with_persis.png
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.337823 libensemble-0.9.3/docs/images/diagram_xml/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   707087 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/diagram_xml/balsam2.xml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    74050 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/diagram_xml/persis_add_worker.xml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    73798 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/diagram_xml/persis_wasted_node.xml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   171140 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/distributed_new_detailed.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   367100 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/funcxmodel.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   337602 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/gen_v_fail_or_cancel.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   244843 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/history_gen1.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   244574 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/history_gen2.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    26836 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/history_init.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   205538 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/history_sim1.png
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    54153 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/libE_logo.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    32035 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/libE_logo_white.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6292 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/libEnsemble_Logo.svg
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    26268 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/libe_opal_complete_v_killed_511w_2044sims_1030nodes.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    31284 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/libe_opal_util_v_time_511w_2044sims_1030nodes.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   372562 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/localopt_6hc.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   250428 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/persis_add_worker.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   233756 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/persis_wasted_node.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   373798 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/sampling_6hc.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    34960 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/sinex.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    45757 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/variable_resources1.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    48241 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/variable_resources2.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    41003 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/variable_resources3.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    43963 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/variable_resources_larger_rsets1.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    46233 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/variable_resources_more_rsets1.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    52608 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/variable_resources_persis_gen1.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    37856 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/images/variable_resources_sched_opts.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1167 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       66 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/introduction.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4137 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/introduction_latex.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1338 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/known_issues.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      794 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/latex_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      125 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/libe_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7433 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/overview_usecases.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.337823 libensemble-0.9.3/docs/platforms/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4933 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/platforms/bebop.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6841 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/platforms/cori.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2652 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/platforms/example_scripts.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6722 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/platforms/perlmutter.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9878 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/platforms/platforms_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2790 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/platforms/spock_crusher.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4447 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/platforms/srun.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7440 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/platforms/summit.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    13063 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/platforms/theta.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      580 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/posters.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      426 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/programming_libE.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      435 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/references.bib
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       30 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/release_notes.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       45 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/requirements.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.337823 libensemble-0.9.3/docs/resource_manager/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10294 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/resource_manager/overview.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1661 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/resource_manager/resource_detection.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      728 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/resource_manager/resources_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      783 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/resource_manager/scheduler_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      413 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/resource_manager/worker_resources.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3236 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/resource_manager/zero_resource_workers.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      464 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/rst_formatting_guidelines
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12317 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/running_libE.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12828 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/scipy2020.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3869 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/sim_gen_alloc_funcs.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.337823 libensemble-0.9.3/docs/tutorials/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12439 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/tutorials/aposmm_tutorial.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    15542 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/tutorials/calib_cancel_tutorial.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    17748 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/tutorials/executor_forces_tutorial.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9534 2022-10-13 21:09:01.000000 libensemble-0.9.3/docs/tutorials/forces_gpu_tutorial.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    18543 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/tutorials/local_sine_tutorial.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      153 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/tutorials/tutorials.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      978 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/utilities.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1551 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/welcome.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10302 2022-10-13 17:42:55.000000 libensemble-0.9.3/docs/xSDK_policy_compatibility.md
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.337823 libensemble-0.9.3/examples/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      856 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/README.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.337823 libensemble-0.9.3/examples/alloc_funcs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2473 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/alloc_funcs/fast_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3178 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/alloc_funcs/fast_alloc_to_aposmm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3494 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/alloc_funcs/give_sim_work_first.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11635 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/alloc_funcs/start_only_persistent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4889 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/alloc_funcs/start_persistent_local_opt_gens.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.337823 libensemble-0.9.3/examples/calling_scripts/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.341823 libensemble-0.9.3/examples/calling_scripts/regression_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      461 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/.bal_coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      456 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5366 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/common.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3305 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/script_test_balsam_hworld.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.345823 libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2496 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ECnoise.m
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      694 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       37 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/cleanup-balsam-test.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      787 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/configure-balsam-test.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4271 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/test_balsam_hworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      500 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/wrapper_obj_fun.m
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3614 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1882 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_1d_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2021 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_evaluate_existing_sample.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2154 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_evaluate_mixed_sample.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2217 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_heffte.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2849 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_inverse_bayes_example.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4473 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_dfols.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3119 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_exception.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4182 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_external_localopt.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3309 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_nlopt.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3604 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_periodic.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4041 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_pounders.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4711 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_scipy.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3446 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_blmvm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2728 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_nm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2989 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_timeout.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4679 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_with_grad.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2876 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_fd_param_finder.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5147 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_gp.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4045 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_gp_multitask_ax.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4611 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_independent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9079 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_n_agent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8994 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_pds.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6871 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_prox_slide.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4833 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_surmise_calib.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5637 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_surmise_killsims.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5919 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_tasmanian.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3922 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_tasmanian_async.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4271 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/run_libe_forces.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      894 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/run_libe_forces_from_yaml.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7558 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/calling_scripts/run_libensemble_on_warpx.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1713 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/calling_scripts/tutorial_calling.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.345823 libensemble-0.9.3/examples/gen_funcs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9120 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/gen_funcs/persistent_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6628 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/gen_funcs/sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4819 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/gen_funcs/uniform_or_localopt.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.345823 libensemble-0.9.3/examples/libE_submission_scripts/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      833 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/libE_submission_scripts/bebop_submit_slurm_central.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2803 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/libE_submission_scripts/bebop_submit_slurm_distrib.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1669 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/libE_submission_scripts/blues_script.pbs
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      705 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/libE_submission_scripts/bridges_submit_slurm_central.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1157 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/libE_submission_scripts/cori_submit.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      939 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/libE_submission_scripts/edtb_submit_pbspro_central.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      367 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/libE_submission_scripts/submit_slurm_simple.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1278 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/libE_submission_scripts/summit_submit_mproc.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3701 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/libE_submission_scripts/theta_submit_balsam.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1541 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/libE_submission_scripts/theta_submit_mproc.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.345823 libensemble-0.9.3/examples/misc/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      586 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/misc/ps_nodes.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.345823 libensemble-0.9.3/examples/sim_funcs/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.345823 libensemble-0.9.3/examples/sim_funcs/branin/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/sim_funcs/branin/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      599 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/sim_funcs/branin/branin.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1041 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/sim_funcs/branin/branin_obj.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       71 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/sim_funcs/branin/known_minima_and_func_values
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11278 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/sim_funcs/chwirut1.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6498 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/sim_funcs/executor_hworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      324 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/sim_funcs/helloworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8152 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/sim_funcs/six_hump_camel.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.317823 libensemble-0.9.3/examples/tutorials/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.345823 libensemble-0.9.3/examples/tutorials/aposmm/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    13701 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/aposmm/aposmm_tutorial_notebook.ipynb
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1816 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/aposmm/tutorial_aposmm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      632 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/tutorials/aposmm/tutorial_six_hump_camel.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.345823 libensemble-0.9.3/examples/tutorials/forces_with_executor/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1170 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/tutorials/forces_with_executor/build_forces.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13024 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/forces_with_executor/forces.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1424 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/forces_with_executor/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    22332 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/forces_with_executor/forces_tutorial_notebook.ipynb
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1996 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/tutorials/forces_with_executor/run_libe_forces.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.349823 libensemble-0.9.3/examples/tutorials/images/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   295622 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/images/basic_6hc.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   372562 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/images/localopt_6hc.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   373798 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/images/sampling_6hc.png
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.349823 libensemble-0.9.3/examples/tutorials/simple_sine/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11697 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/simple_sine/sine_tutorial_notebook.ipynb
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1713 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/tutorials/simple_sine/tutorial_calling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2008 2022-10-13 21:09:01.000000 libensemble-0.9.3/examples/tutorials/simple_sine/tutorial_calling_mpi.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      751 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/simple_sine/tutorial_gen.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      376 2022-10-13 17:42:55.000000 libensemble-0.9.3/examples/tutorials/simple_sine/tutorial_sim.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.349823 libensemble-0.9.3/install/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1444 2022-10-13 17:42:55.000000 libensemble-0.9.3/install/configure_balsam_install.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       93 2022-10-13 17:42:55.000000 libensemble-0.9.3/install/environment.yml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      539 2022-10-13 17:42:55.000000 libensemble-0.9.3/install/find_mpi.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      120 2022-10-13 21:09:01.000000 libensemble-0.9.3/install/testing_requirements.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.349823 libensemble-0.9.3/libensemble/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      427 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/__init__.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.353823 libensemble-0.9.3/libensemble/alloc_funcs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      193 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/defaults.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2473 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/fast_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7462 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/fast_alloc_and_pausing.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3178 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/fast_alloc_to_aposmm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1593 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/give_pregenerated_work.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3494 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/give_sim_work_first.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3160 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/inverse_bayes_allocf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1939 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/only_one_gen_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3858 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/persistent_aposmm_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3231 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/start_fd_persistent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11635 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/start_only_persistent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14024 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/alloc_funcs/start_persistent_consensus.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4889 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/alloc_funcs/start_persistent_local_opt_gens.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8659 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/api.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.353823 libensemble-0.9.3/libensemble/comms/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/comms/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    17734 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/comms/comms.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6372 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/comms/logs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3764 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/comms/mpi.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3575 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/comms/tcp_mgr.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.353823 libensemble-0.9.3/libensemble/executors/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      150 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/executors/__init__.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.353823 libensemble-0.9.3/libensemble/executors/balsam_executors/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      947 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/executors/balsam_executors/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    18969 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/executors/balsam_executors/balsam_executor.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12284 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/executors/balsam_executors/legacy_balsam_executor.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    23147 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/executors/executor.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10183 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/executors/mpi_executor.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10573 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/executors/mpi_runner.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.353823 libensemble-0.9.3/libensemble/gen_funcs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1337 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    21925 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/aposmm_localopt_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    40127 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/old_aposmm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    32541 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_aposmm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10158 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_ax_multitask.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4942 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_fd_param_finder.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10437 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_gp.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2049 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_independent_optimize.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1486 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_inverse_bayes.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3469 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_n_agent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5318 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_pds.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4126 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_prox_slide.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9120 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8524 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_surmise_calib.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14491 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/persistent_tasmanian.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6628 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/gen_funcs/sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2241 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/gen_funcs/surmise_calib_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4819 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/gen_funcs/uniform_or_localopt.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9090 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/history.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      995 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/information_about_W
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    22256 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/libE.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1365 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/logger.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    24315 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/manager.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2188 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/message_numbers.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9114 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/output_directory.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.353823 libensemble-0.9.3/libensemble/resources/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/resources/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8776 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/resources/env_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8556 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/resources/mpi_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3723 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/resources/node_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11886 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/resources/resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5215 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/resources/rset_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14716 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/resources/scheduler.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12274 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/resources/worker_resources.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.357823 libensemble-0.9.3/libensemble/sim_funcs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1119 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/alt_rosenbrock.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2544 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/borehole.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2050 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/sim_funcs/borehole_kills.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.357823 libensemble-0.9.3/libensemble/sim_funcs/branin/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/branin/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      599 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/branin/branin.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1041 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/sim_funcs/branin/branin_obj.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       71 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/branin/known_minima_and_func_values
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11278 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/chwirut1.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      353 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/comms_testing.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6498 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/sim_funcs/executor_hworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1105 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/geomedian.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      720 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/heffte.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      324 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/helloworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      606 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/inverse_bayes.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1765 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/sim_funcs/linear_regression.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1786 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/sim_funcs/logistic_regression.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1286 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/nesterov_quadratic.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1337 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/sim_funcs/noisy_vector_mapping.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      512 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/one_d_func.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      486 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/periodic_func.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2441 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/rosenbrock.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4184 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/sim_funcs/run_line_check.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8152 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/sim_funcs/six_hump_camel.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2766 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/sim_funcs/surmise_test_function.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1759 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/sim_funcs/svm.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.357823 libensemble-0.9.3/libensemble/tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      707 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/__init__.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.357823 libensemble-0.9.3/libensemble/tests/deprecated_tests/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.361823 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.361823 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/bash_scripts/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1898 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/bash_scripts/setup_balsam_tests.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      291 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/env_setup_theta.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      732 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/readme.balsam_tests.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7837 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/readme.rst
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      259 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/reset_balsam_tests.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     3170 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/setup_balsam_tests.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2002 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_1__runjobs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2119 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_2__workerkill.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2978 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_3__managerkill.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.361823 libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2070 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/create_balsam_job.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1447 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/readme.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      641 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/set.balsam.database.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.361823 libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      957 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/my_simtask.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1247 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/my_simtask.f90
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3280 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3732 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor_manager_poll.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4846 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor_multi.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1944 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/test_nan_func_old_aposmm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4092 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_logic.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2752 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_one_residual_at_a_time.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2487 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_pounders.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2857 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_pounders_splitcomm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2856 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_pounders_subcomm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3406 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_sim_dirs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4869 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_with_gradients.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.365823 libensemble-0.9.3/libensemble/tests/functionality_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      457 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      431 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/1d_sampling.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2206 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/check_libE_stats.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1254 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_1d_sampling_from_yaml.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2498 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_1d_sampling_with_profile.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2779 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_1d_uniform_sampling_with_comm_dup.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2786 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1783 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_calc_exception.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2502 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_cancel_in_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2396 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_comms.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2230 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_elapsed_time_abort.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3807 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_executor_hworld_pass_fail.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3822 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_executor_hworld_timeout.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2659 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_executor_simple.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3000 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_fast_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3164 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_comms.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    13123 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4243 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners_subnode.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5020 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners_subnode_uneven.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4626 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners_supernode_uneven.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6276 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners_zrw_subnode_uneven.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5004 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners_zrw_supernode_uneven.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3104 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_sampling_CUDA_variable_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2898 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_sim_uniform_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3401 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_gen_decides_stop.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2696 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2791 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_adv.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2772 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_async.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2560 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_cancel.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2428 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_nonblocking.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3341 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_runlines_adaptive_workers.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3517 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3736 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent_oversubscribe_rsets.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3225 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_sim_dirs_per_calc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3514 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_sim_dirs_per_worker.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2175 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_sim_dirs_with_exception.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4043 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_sim_dirs_with_gen_dirs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2592 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_sim_input_dir_option.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4227 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_stats_output.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2424 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_uniform_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5556 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_uniform_sampling_cancel.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4178 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_uniform_sampling_one_residual_at_a_time.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3043 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_uniform_sampling_then_persistent_localopt_runs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4186 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1974 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_worker_exceptions.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4385 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_zero_resource_workers.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4632 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/functionality_tests/test_zero_resource_workers_subnode.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.369823 libensemble-0.9.3/libensemble/tests/regression_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      461 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/.bal_coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      456 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5366 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/common.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3305 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/script_test_balsam_hworld.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.369823 libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2496 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ECnoise.m
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      694 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       37 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/cleanup-balsam-test.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      787 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/configure-balsam-test.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4271 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/test_balsam_hworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      500 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/wrapper_obj_fun.m
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3614 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1882 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_1d_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2021 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_evaluate_existing_sample.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2154 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_evaluate_mixed_sample.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2217 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_heffte.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2849 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_inverse_bayes_example.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4473 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_dfols.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3119 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_exception.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4182 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_external_localopt.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3309 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_nlopt.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3604 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_periodic.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4041 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_pounders.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4711 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_scipy.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3446 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_tao_blmvm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2728 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_tao_nm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2989 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_timeout.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4679 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_with_grad.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2876 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_fd_param_finder.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5147 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_gp.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4045 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_gp_multitask_ax.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4611 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_independent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9079 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_n_agent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8994 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_pds.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6871 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_prox_slide.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4833 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_surmise_calib.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5637 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_surmise_killsims.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5919 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_tasmanian.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3922 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_tasmanian_async.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    26341 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/run-tests.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.369823 libensemble-0.9.3/libensemble/tests/scaling_tests/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.317823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       60 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2056 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/define_apps.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1990 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7612 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2531 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/run_libe_forces_balsam.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2366 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/submit_libe_forces_remotely.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1527 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/balsam_local.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      290 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/clone.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      899 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/forces.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4853 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2554 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/forces_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4548 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4271 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      894 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces_from_yaml.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1170 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/build_forces.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13024 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/forces.c
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    21992 2022-10-13 17:46:32.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/forces.x
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      885 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/build_forces.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5148 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4845 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces_AoS.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      916 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/readme.md
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/cleanup.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.317823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim0_worker1/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      120 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim0_worker1/forces.stat
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:46:36.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim0_worker1/libe_task_forces_worker1_0.err
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1345 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim0_worker1/libe_task_forces_worker1_0.out
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim1_worker2/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      120 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim1_worker2/forces.stat
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:46:36.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim1_worker2/libe_task_forces_worker2_0.err
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1345 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim1_worker2/libe_task_forces_worker2_0.out
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim2_worker3/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      120 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim2_worker3/forces.stat
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:46:36.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim2_worker3/libe_task_forces_worker3_0.err
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1345 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim2_worker3/libe_task_forces_worker3_0.out
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim3_worker4/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      120 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim3_worker4/forces.stat
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:46:36.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim3_worker4/libe_task_forces_worker4_0.err
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1345 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim3_worker4/libe_task_forces_worker4_0.out
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim4_worker3/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      120 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim4_worker3/forces.stat
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim4_worker3/libe_task_forces_worker3_1.err
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1345 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim4_worker3/libe_task_forces_worker3_1.out
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim5_worker1/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      120 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim5_worker1/forces.stat
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim5_worker1/libe_task_forces_worker1_1.err
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1345 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim5_worker1/libe_task_forces_worker1_1.out
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.373823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim6_worker3/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      130 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim6_worker3/forces.stat
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim6_worker3/libe_task_forces_worker3_2.err
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1357 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim6_worker3/libe_task_forces_worker3_2.out
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.377823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim7_worker1/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      130 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim7_worker1/forces.stat
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim7_worker1/libe_task_forces_worker1_2.err
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1356 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim7_worker1/libe_task_forces_worker1_2.out
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4386 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/ensemble.log
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1891 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1232 2022-10-13 17:46:37.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/libE_stats.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2076 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2354 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/run_libe_forces.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      254 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/submit_perlmutter.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.377823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_simple/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_simple/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1424 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_simple/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1413 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_simple/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1996 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_simple/run_libe_forces.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.377823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/funcx_forces/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       54 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/funcx_forces/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4691 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/funcx_forces/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1141 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/funcx_forces/funcx_forces.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1447 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/funcx_forces/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      394 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/funcx_forces/run_libe_forces_funcx.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.377823 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/submission_scripts/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      363 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/submission_scripts/submit_slurm_simple.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1370 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/submission_scripts/summit_submit_mproc.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     3641 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/submission_scripts/theta_submit_balsam.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1563 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/forces/submission_scripts/theta_submit_mproc.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      148 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/note_moved_examples.md
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.377823 libensemble-0.9.3/libensemble/tests/scaling_tests/persistent_gp/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2975 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/persistent_gp/run_example.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.377823 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      853 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/all_machine_specs.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     4470 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/plot_results.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2502 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/read_sim_output.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1925 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/readme.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       44 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/requirements.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7558 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/run_libensemble_on_warpx.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.377823 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/sim/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8355 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/sim/inputs
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1413 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/summit_submit_mproc.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3993 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/warpx_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3284 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/write_sim_input.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.317823 libensemble-0.9.3/libensemble/tests/standalone_tests/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.377823 libensemble-0.9.3/libensemble/tests/standalone_tests/comms_test/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1821 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/comms_test/commtest.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      973 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/comms_test/readme.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.377823 libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       84 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/build.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      663 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/burn_time.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4716 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/killtest.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2587 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/log.autotest.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2411 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/log.burn_time_test_with_top.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1822 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/readme.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1011 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/sleep_and_print.c
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.377823 libensemble-0.9.3/libensemble/tests/standalone_tests/mpi_launch_test/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      663 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/mpi_launch_test/create_mpi_jobs.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      310 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/mpi_launch_test/helloworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      747 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/standalone_tests/mpi_launch_test/readme.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.381823 libensemble-0.9.3/libensemble/tests/unit_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      378 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      712 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/conftest.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      446 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/launch_busy.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3167 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/mpich-only_test_api.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2910 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/setup.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.381823 libensemble-0.9.3/libensemble/tests/unit_tests/simdir/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1359 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/simdir/borehole.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      210 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/simdir/c_startup.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      806 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/simdir/my_serialtask.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1166 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/simdir/my_simtask.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1247 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/simdir/my_simtask.f90
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       32 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/simdir/py_startup.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      560 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/simdir/test_example.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      560 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/simdir/test_example_badfuncs_attribute.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      544 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/simdir/test_example_badfuncs_notfound.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    16181 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_allocation_funcs_and_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10825 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_comms.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12576 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_env_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    31403 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_executor.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9143 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_executor_balsam.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    16832 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_history.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2620 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_launcher.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11678 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_libE_main.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4134 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_loc_stack.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3804 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_make_runners.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1896 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_manager_main.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      256 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_mpi4py.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4057 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_node_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6078 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_persistent_aposmm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    23918 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_resource_scheduler.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    31196 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1499 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_scipy.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5550 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_sim_dir_properties.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4335 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_task_funcs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1533 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests/test_timer.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1200 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests/tofix__test_worker.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.381823 libensemble-0.9.3/libensemble/tests/unit_tests_logger/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      404 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests_logger/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4474 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests_logger/test_logger.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.381823 libensemble-0.9.3/libensemble/tests/unit_tests_nompi/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      404 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tests/unit_tests_nompi/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      712 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests_nompi/conftest.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2667 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tests/unit_tests_nompi/test_aaa_comms.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.385823 libensemble-0.9.3/libensemble/tools/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      326 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tools/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    13687 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tools/alloc_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10492 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tools/check_inputs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    13532 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tools/consensus_subroutines.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2927 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tools/fields_keys.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1367 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/tools/forkable_pdb.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8909 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tools/parse_args.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4544 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tools/persistent_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5623 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/tools/tools.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.385823 libensemble-0.9.3/libensemble/utils/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/utils/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3226 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/utils/launcher.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4221 2022-10-13 17:42:55.000000 libensemble-0.9.3/libensemble/utils/loc_stack.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      715 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/utils/misc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2975 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/utils/runners.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2774 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/utils/timer.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       22 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/version.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12573 2022-10-13 21:09:01.000000 libensemble-0.9.3/libensemble/worker.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.349823 libensemble-0.9.3/libensemble.egg-info/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1533 2022-10-13 21:10:02.000000 libensemble-0.9.3/libensemble.egg-info/PKG-INFO
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    31271 2022-10-13 21:10:03.000000 libensemble-0.9.3/libensemble.egg-info/SOURCES.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        1 2022-10-13 21:10:02.000000 libensemble-0.9.3/libensemble.egg-info/dependency_links.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      174 2022-10-13 21:10:03.000000 libensemble-0.9.3/libensemble.egg-info/requires.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       12 2022-10-13 21:10:03.000000 libensemble-0.9.3/libensemble.egg-info/top_level.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.385823 libensemble-0.9.3/scripts/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/__init__.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2022-10-13 21:10:03.385823 libensemble-0.9.3/scripts/balsam/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      517 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/balsam/plot_tasks_v_time.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      523 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/balsam/plot_util_v_time.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      514 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/balsam/plot_waiting_v_time.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      409 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/balsam/readme.rst
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     2466 2022-10-13 21:09:01.000000 libensemble-0.9.3/scripts/compare_npy.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4505 2022-10-13 21:09:01.000000 libensemble-0.9.3/scripts/liberegister
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7194 2022-10-13 21:09:01.000000 libensemble-0.9.3/scripts/libesubmit
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1630 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/plot_contours_and_history_points.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     3131 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/plot_libe_calcs_util_v_time.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     4168 2022-10-13 21:09:01.000000 libensemble-0.9.3/scripts/plot_libe_histogram.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3709 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/plot_libe_tasks_util_v_time.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1772 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/plot_pareto_2d.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     2051 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/plot_pareto_3d.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1566 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/print_fields.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      838 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/print_npy.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      496 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/print_pickle.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1744 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/process_history_to_make_chart.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2306 2022-10-13 17:42:55.000000 libensemble-0.9.3/scripts/readme.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       38 2022-10-13 21:10:03.385823 libensemble-0.9.3/setup.cfg
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3853 2022-10-13 21:09:01.000000 libensemble-0.9.3/setup.py
```

### Comparing `libensemble-0.9.2/.flake8` & `libensemble-0.9.3/.flake8`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         examples/gen_funcs/*aposmm.py:E501
 
         # Need to set something before the APOSMM import
         libensemble/tests/scaling_tests/warpx/run_libensemble_on_warpx.py:E402
         examples/calling_scripts/run_libensemble_on_warpx.py:E402
         libensemble/gen_funcs/persistent_aposmm.py:E402, E501
         libensemble/tests/regression_tests/test_persistent_aposmm*:E402
-        libensemble/tests/regression_tests/dont_run_test_persistent_aposmm*:E402
-        libensemble/tests/regression_tests/test_uniform_sampling_then_persistent_localopt_runs.py:E402
+        libensemble/tests/regression_tests/test_persistent_gp_multitask_ax.py:E402
+        libensemble/tests/functionality_tests/test_uniform_sampling_then_persistent_localopt_runs.py:E402
         libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py:E402
         libensemble/tests/deprecated_tests/test_old_aposmm*:E402
         libensemble/tests/unit_tests/test_persistent_aposmm.py:E402
 
         # Allow undefined name '__version__'
         setup.py:F821
```

### Comparing `libensemble-0.9.2/CHANGELOG.rst` & `libensemble-0.9.3/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,56 @@
 
 Below are the notes from all libEnsemble releases.
 
 GitHub issues are referenced, and can be viewed with hyperlinks on the `github releases page`_.
 
 .. _`github releases page`: https://github.com/Libensemble/libensemble/releases
 
+Release 0.9.3
+-------------
+
+:Date: October 13, 2022
+
+New capabilities:
+
+* New pair of utilities, `liberegister` and `libesubmit` (based on *PSI/J*), for easily preparing and launching libEnsemble workflows with local comms onto most machines and schedulers. #807
+* New persistent support function to cancel sim_ids (`request_cancel_sim_ids`). #880
+* `keep_state` option for persistent workers: this lets the manager know that the information being sent is intermediate. #880 
+
+Other enhancements:
+
+* The Executor `manager_poll()` interface now sets consistent flags instead of literal strings. #877
+* Some internal modules and the test suite now work on Windows. #869 #888
+* Specifying the `num_resource_sets` *libE_specs* option instead of `zero_resource_workers` is now recommended except when using a fixed worker/resource mapping. Use ``persis_info["gen_resources"]`` to assign persistent generator resources (default is zero). #905
+* An extraneous warning removed. #903
+
+:Note:
+
+* Tested platforms include Linux, MacOS, Windows, Theta (Cray XC40/Cobalt), Summit (IBM Power9/LSF), Bebop (Cray CS400/Slurm), Swing (A100 GPU system), Perlmutter (HPE Cray EX with A100 NVIDIA GPUs). For Perlmutter, see "Known issues" below.
+* Tested Python versions: (Cpython) 3.7, 3.8, 3.9, 3.10.
+
+:Known issues:
+
+* At time of testing on Perlmutter there was an issue running concurrent applications on a node, following a recent system update. This also affects previous versions of libEnsemble, and is being investigated.
+* See known issues section in the documentation.
+
 Release 0.9.2
 -------------
 
 :Date: July 06, 2022
 
 New capabilities:
 
 * Support auto-detection of PBS node lists. #602
 * Added configuration options for `libE_stats.txt` file. #743
 * Support for `spawn` and `forkserver` multiprocessing start methods. #797
 
- * Note that macOS no longer switches to using `fork`. macOS (since Python 3.8) and Windows
- default to using `spawn`. When using `spawn`, we recommend placing calling script code in
- an ``if __name__ == "__main__":`` block. The multiprocessing interface can be used to switch methods (https://docs.python.org/3/library/multiprocessing.html#multiprocessing.set_start_method).
+ * Note that macOS no longer switches to using `fork`. macOS (since Python 3.8) and Windows default to
+   using `spawn`. When using `spawn`, we recommend placing calling script code in an ``if __name__ == "__main__":`` block.
+   The multiprocessing interface can be used to switch methods (https://docs.python.org/3/library/multiprocessing.html#multiprocessing.set_start_method).
 
 Updates to example functions:
 
 Added simple dynamic sampling example. #833
 Added heFFTe example. #844
 Regression tests separated into problem examples and functionality tests. #839
```

### Comparing `libensemble-0.9.2/CONTRIBUTING.rst` & `libensemble-0.9.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/LICENSE` & `libensemble-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/PKG-INFO` & `libensemble-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: libensemble
-Version: 0.9.2
+Version: 0.9.3
 Summary: Library to coordinate the concurrent evaluation of dynamic ensembles of calculations
 Home-page: https://github.com/Libensemble/libensemble
 Author: Jeffrey Larson, Stephen Hudson, Stefan M. Wild, David Bindel and John-Luke Navarro
 Author-email: libensemble@lists.mcs.anl.gov
 License: BSD 3-clause
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
@@ -30,9 +29,7 @@
 libEnsemble is a Python toolkit for coordinating workflows of asynchronous
 and dynamic ensembles of calculations.
 
 libEnsemble can help users take advantage of massively parallel resources to
 solve design, decision, and inference problems and expand the class of
 problems that can benefit from increased parallelism.
 
-
-
```

### Comparing `libensemble-0.9.2/README.rst` & `libensemble-0.9.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
 ===========================
 Introduction to libEnsemble
 ===========================
 
 libEnsemble is a Python_ toolkit for coordinating workflows of asynchronous and dynamic ensembles of calculations.
 
-libEnsemble can help users take advantage of massively parallel resources to solve design,
-decision, and inference problems and expand the class of problems that can benefit from
+libEnsemble helps users take advantage of massively parallel resources to solve design,
+decision, and inference problems and expands the class of problems that can benefit from
 increased parallelism.
 
 libEnsemble aims for:
 
 • **Extreme scaling**: Run on or across_ laptops, clusters, and leadership-class machines.
 • **Dynamic Ensembles**: Generate new tasks on-the-fly based on previous computations.
 • **Dynamic Resource Management**: Reassign resource partitions of any size for tasks.
@@ -54,59 +54,67 @@
 Simulator functions can themselves use parallel resources and involve libraries
 or executables that are not written in Python.
 
 With a basic familiarity of Python and NumPy_, users can easily incorporate
 any other mathematics, machine-learning, or resource-management libraries into libEnsemble
 workflows.
 
-libEnsemble employs a manager/worker scheme that runs on MPI, multiprocessing,
+libEnsemble employs a manager/worker scheme that communicates via MPI, multiprocessing,
 or TCP. Workers control and monitor any level of work using the aforementioned
 generator and simulator functions, from small subnode tasks to huge many-node computations.
 
 libEnsemble includes an Executor interface so application-launching functions are
 portable, resilient, and flexible; it also automatically detects available nodes
 and cores, and can dynamically assign resources to workers.
 
+libEnsemble performs best on Unix-like systems like Linux and macOS. See the
+:ref:`FAQ<faqwindows>` for more information.
+
 .. before_dependencies_rst_tag
 
 Dependencies
 ~~~~~~~~~~~~
 
-Required dependencies:
+**Required dependencies**:
 
 * Python_ 3.7 or above
 * NumPy_
 * psutil_
 * setuptools_
 
 When using  ``mpi4py`` for libEnsemble communications:
 
 * A functional MPI 1.x/2.x/3.x implementation, such as MPICH_, built with shared/dynamic libraries
 * mpi4py_ v2.0.0 or above
 
-Optional dependencies:
+**Optional dependencies**:
 
 * Balsam_
 
 As of v0.9.0, libEnsemble features an updated `Balsam Executor`_
 for workers to schedule and launch applications to *anywhere* with a running
 Balsam site, including to remote machines.
 
 * pyyaml_
 
-libEnsemble is typically configured and parameterized via Python dictionaries.
-As of v0.8.0, libEnsemble can also be parameterized via yaml.
+libEnsemble is typically configured and parameterized via Python dictionaries. libEnsemble can also be parameterized via yaml.
 
 * funcX_
 
 As of v0.9.0, libEnsemble features a cross-system capability powered by funcX_,
 a function-as-a-service platform to which workers can submit remote generator or
 simulator function instances. This feature can help distribute an ensemble
 across systems and heterogeneous resources.
 
+* `psi-j-python`_
+
+As of v0.9.3, libEnsemble features a set of command-line utilities for submitting
+libEnsemble jobs to almost any system or scheduler via a `PSI/J`_ Python interface. tqdm_
+is also required.
+
 The example simulation and generation functions and tests require the following:
 
 * SciPy_
 * mpmath_
 * petsc4py_
 * DEAP_
 * DFO-LS_
@@ -225,29 +233,30 @@
 - Email questions or request `libEnsemble Slack page`_ access from ``libEnsemble@lists.mcs.anl.gov``.
 - Open issues on GitHub_.
 - Join the `libEnsemble mailing list`_ for updates about new releases.
 
 **Further Information:**
 
 - Documentation is provided by ReadtheDocs_.
-- An overview of libEnsemble's structure and capabilities is given in this manuscript_ and poster_
+- Contributions_ to libEnsemble are welcome.
+- An overview of libEnsemble's structure and capabilities is given in this manuscript_ and poster_.
 - Examples of production user functions and complete workflows can be viewed, downloaded, and contributed to in the libEnsemble `Community Examples repository`_.
 
 **Citation:**
 
 - Please use the following to cite libEnsemble:
 
 .. code-block:: bibtex
 
   @techreport{libEnsemble,
     title   = {{libEnsemble} Users Manual},
     author  = {Stephen Hudson and Jeffrey Larson and Stefan M. Wild and
                David Bindel and John-Luke Navarro},
     institution = {Argonne National Laboratory},
-    number  = {Revision 0.9.2},
+    number  = {Revision 0.9.3},
     year    = {2022},
     url     = {https://buildmedia.readthedocs.org/media/pdf/libensemble/latest/libensemble.pdf}
   }
 
   @article{Hudson2022,
     title   = {{libEnsemble}: A Library to Coordinate the Concurrent
                Evaluation of Dynamic Ensembles of Calculations},
@@ -301,14 +310,15 @@
 .. _APOSMM: https://link.springer.com/article/10.1007/s12532-017-0131-4
 .. _AWA: https://link.springer.com/article/10.1007/s12532-017-0131-4
 .. _Balsam: https://balsam.readthedocs.io/en/latest/
 .. _Balsam Executor: https://libensemble.readthedocs.io/en/develop/executor/balsam_2_executor.html
 .. _Community Examples repository: https://github.com/Libensemble/libe-community-examples
 .. _Conda: https://docs.conda.io/en/latest/
 .. _conda-forge: https://conda-forge.org/
+.. _Contributions: https://github.com/Libensemble/libensemble/blob/main/CONTRIBUTING.rst
 .. _Coveralls: https://coveralls.io/github/Libensemble/libensemble?branch=main
 .. _DEAP: https://deap.readthedocs.io/en/master/overview.html
 .. _DFO-LS: https://github.com/numericalalgorithmsgroup/dfols
 .. _ECNoise: https://www.mcs.anl.gov/~wild/cnoise/
 .. _example user scripts: https://libensemble.readthedocs.io/en/main/examples/examples_index.html
 .. _funcX: https://funcx.org/
 .. _GitHub: https://github.com/Libensemble/libensemble
@@ -326,14 +336,16 @@
 .. _NLopt documentation: http://ab-initio.mit.edu/wiki/index.php/NLopt_Installation#Shared_libraries
 .. _nlopt: http://ab-initio.mit.edu/wiki/index.php/NLopt
 .. _NumPy: http://www.numpy.org
 .. _OPAL: http://amas.web.psi.ch/docs/opal/opal_user_guide-1.6.0.pdf
 .. _petsc4py: https://bitbucket.org/petsc/petsc4py
 .. _PETSc/TAO: http://www.mcs.anl.gov/petsc
 .. _poster: https://figshare.com/articles/libEnsemble_A_Python_Library_for_Dynamic_Ensemble-Based_Computations/12559520
+.. _PSI/J: https://exaworks.org/psij
+.. _psi-j-python: https://github.com/ExaWorks/psi-j-python
 .. _psutil: https://pypi.org/project/psutil/
 .. _PyPI: https://pypi.org
 .. _pytest-cov: https://pypi.org/project/pytest-cov/
 .. _pytest-timeout: https://pypi.org/project/pytest-timeout/
 .. _pytest: https://pypi.org/project/pytest/
 .. _Python: http://www.python.org
 .. _pyyaml: https://pyyaml.org/
@@ -344,12 +356,13 @@
 .. _Spack: https://spack.readthedocs.io/en/latest
 .. _Summit: https://www.olcf.ornl.gov/olcf-resources/compute-systems/summit/
 .. _Surmise: https://surmise.readthedocs.io/en/latest/index.html
 .. _SWIG: http://swig.org/
 .. _tarball: https://github.com/Libensemble/libensemble/releases/latest
 .. _Tasmanian: https://tasmanian.ornl.gov/
 .. _Theta: https://www.alcf.anl.gov/alcf-resources/theta
+.. _tqdm: https://tqdm.github.io/
 .. _user guide: https://libensemble.readthedocs.io/en/latest/programming_libE.html
 .. _VTMOP: https://github.com/Libensemble/libe-community-examples#vtmop
 .. _WarpX: https://warpx.readthedocs.io/en/latest/
 .. _WarpX + libE scripts: https://warpx.readthedocs.io/en/latest/usage/workflows/libensemble.html
 .. _xSDK Extreme-scale Scientific Software Development Kit: https://xsdk.info
```

### Comparing `libensemble-0.9.2/docs/FAQ.rst` & `libensemble-0.9.3/docs/FAQ.rst`

 * *Files 13% similar despite different names*

```diff
@@ -217,24 +217,80 @@
     from libensemble import logger
     logger.set_stderr_level('CRITICAL')
 
 This effectively puts libEnsemble in silent mode.
 
 See the :ref:`Logger Configuration<logger_config>` docs for more information.
 
-macOS-Specific Errors
----------------------
+macOS and Windows Errors
+------------------------
 
-**"Fatal error in MPI_Init_thread: Other MPI error, error stack: ... gethostbyname failed"**
+.. _faqwindows:
+
+**Can I run libEnsemble on Windows**
+
+Although we have run many libEnsemble workflows successfully on Windows using
+both MPI and local comms, Windows is not rigorously supported. We highly
+recommend Unix-like systems. Windows tends to produce more platform-specific
+issues that are difficult to reproduce and troubleshoot.
+
+Feel free to check our `Github Actions`_ page to see what tests we run regularly on Windows.
+
+.. _`Github Actions`: https://github.com/Libensemble/libensemble/actions
+
+**Windows - How can I run libEnsemble with MPI comms?**
+
+We have run Windows workflows with MPI comms. However, as most MPI
+distributions have either dropped Windows support (MPICH and Open MPI) or are
+no longer being maintained (``msmpi``), we cannot guarantee success.
+
+If users wish to try, we recommend experimenting with the many Unix-like
+emulators, containers, virtual machines, and other such systems. The
+`Installing PETSc On Microsoft Windows`_ documentation contains valuable
+information.
+
+Otherwise, install ``msmpi`` and ``mpi4py`` from conda and experiment, or use ``local`` comms.
+
+.. _`Installing PETSc On Microsoft Windows`: https://petsc.org/release/install/windows/#recommended-installation-methods
+
+**Windows - 'A required privilege is not held by the client'**
+
+Assuming you were trying to use the ``sim_dir_symlink_files`` or ``gen_dir_symlink_files`` options, this indicates that to
+allow libEnsemble to create symlinks, you need to run your current ``cmd`` shell as administrator.
+
+**"RuntimeError: An attempt has been made to start a new process... this probably means that you are not using fork...
+" if __name__ == '__main__': freeze_support() ...**
+
+You need to place your main calling script code underneath an ``if __name__ == "__main__":`` block.
+
+Explanation: Python chooses one of three methods to start new processes when using multiprocessing
+(``--comms local`` with libEnsemble). These are ``'fork'``, ``'spawn'``, and ``'forkserver'``. ``'fork'``
+is the default on Unix, and in our experience is quicker and more reliable, but ``'spawn'`` is the default
+on Windows and macOS (See the `Python multiprocessing docs`_).
+
+Prior to libEnsemble v0.9.2, if libEnsemble detected macOS, it would automatically switch the multiprocessing
+method to ``'fork'``. We decided to stop doing this to avoid overriding defaults and compatibility issues with
+some libraries.
+
+If you'd prefer to use ``'fork'`` or not reformat your code, you can set the
+multiprocessing start method by placing 
+the following near the top of your calling script::
+
+  import multiprocessing
+  multiprocessing.set_start_method('fork', force=True)
+
+.. _`Python multiprocessing docs`: https://docs.python.org/3/library/multiprocessing.html
+
+**"macOS - Fatal error in MPI_Init_thread: Other MPI error, error stack: ... gethostbyname failed"**
 
 Resolve this by appending ``127.0.0.1   [your hostname]`` to /etc/hosts.
 Unfortunately, ``127.0.0.1   localhost`` isn't satisfactory for preventing this
 error.
 
-**How do I stop the Firewall Security popups when running with the Executor?**
+**macOS - How do I stop the Firewall Security popups when running with the Executor?**
 
 There are several ways to address this nuisance, but all involve trial and error.
 An easy (but insecure) solution is temporarily disabling the firewall through
 System Preferences -> Security & Privacy -> Firewall -> Turn Off Firewall.
 Alternatively, adding a firewall "Allow incoming connections" rule can be
 attempted for the offending executable. We've had limited success running
 ``sudo codesign --force --deep --sign - /path/to/application.app``
```

### Comparing `libensemble-0.9.2/docs/Makefile` & `libensemble-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/advanced_installation.rst` & `libensemble-0.9.3/docs/advanced_installation.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/conf.py` & `libensemble-0.9.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 sys.path.append(os.path.abspath("../libensemble/alloc_funcs"))
 sys.path.append(os.path.abspath("../libensemble/gen_funcs"))
 sys.path.append(os.path.abspath("../libensemble/sim_funcs"))
 sys.path.append(os.path.abspath("../libensemble/comms"))
 sys.path.append(os.path.abspath("../libensemble/utils"))
 sys.path.append(os.path.abspath("../libensemble/tools"))
 sys.path.append(os.path.abspath("../libensemble/executors"))
+sys.path.append(os.path.abspath("../libensemble/executors/balsam_executors"))
 sys.path.append(os.path.abspath("../libensemble/resources"))
 # print(sys.path)
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
```

### Comparing `libensemble-0.9.2/docs/data_structures/alloc_specs.rst` & `libensemble-0.9.3/docs/data_structures/alloc_specs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/data_structures/calc_status.rst` & `libensemble-0.9.3/docs/data_structures/calc_status.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/data_structures/data_structures.rst` & `libensemble-0.9.3/docs/data_structures/data_structures.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/data_structures/exit_criteria.rst` & `libensemble-0.9.3/docs/data_structures/exit_criteria.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/data_structures/gen_specs.rst` & `libensemble-0.9.3/docs/data_structures/gen_specs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/data_structures/history_array.rst` & `libensemble-0.9.3/docs/data_structures/history_array.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/data_structures/libE_specs.rst` & `libensemble-0.9.3/docs/data_structures/libE_specs.rst`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             Default: True
         'worker_timeout' [int]:
             When libEnsemble concludes and attempts to close down worker processes,
             the number of seconds after which workers are considered timed out. Worker
             processes are then terminated. multiprocessing default: 1
         'kill_canceled_sims' [bool]:
             Will libE try to kill sims that user functions mark 'cancel_requested' as True.
-            If False, the manager avoid this moderate overhead.
+            If False, the manager avoids this moderate overhead.
             Default: True
 
         Directory management options:
         -----------------------------
         'ensemble_dir_path' [str]:
             Path to main ensemble directory containing calculation directories. Can serve
             as single working directory for workers, or contain calculation directories.
@@ -143,15 +143,17 @@
         'dedicated_mode' [bool]:
             If True, then running in dedicated mode, otherwise in distributed
             mode. Dedicated mode means libE processes (manager and workers) are
             grouped together and do not share nodes with applications.
             Distributed mode means workers share nodes with applications.
             Default: False
         'zero_resource_workers' [list of ints]:
-            List of workers that require no resources.
+            List of workers that require no resources. For when a fixed mapping of workers
+            to resources is required. Otherwise, use "num_resource_sets".
+            For use with supported allocation functions.
         'resource_info' [dict]:
             Provide resource information that will override automatically detected resources.
             The allowable fields are given below in 'Overriding Auto-detection'
             Note that if "disable_resource_manager" is set then
             this option is ignored.
         'scheduler_opts' [dict]:
             A dictionary of options for the resource scheduler.
```

### Comparing `libensemble-0.9.2/docs/data_structures/persis_info.rst` & `libensemble-0.9.3/docs/data_structures/persis_info.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/data_structures/sim_specs.rst` & `libensemble-0.9.3/docs/data_structures/sim_specs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/data_structures/work_dict.rst` & `libensemble-0.9.3/docs/data_structures/work_dict.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 .. _datastruct-work-dict:
 
 work dictionary
 ===============
 
-The work dictionary contains integer keys ``i`` and dictionary values to be
-given to worker ``i``. ``Work[i]`` has the following form::
+The work dictionary contains metadata that is used by the manager to send a packet
+of work to a worker. The dictionary uses integer keys ``i`` and values that determine
+the data given to worker ``i``. ``Work[i]`` has the following form::
 
     Work[i]: [dict]:
 
         Required keys:
-        'persis_info' [dict]: Any persistent info to be sent to worker 'i'
         'H_fields' [list]: The field names of the history 'H' to be sent to worker 'i'
+        'persis_info' [dict]: Any persistent info to be sent to worker 'i'
         'tag' [int]: 'EVAL_SIM_TAG'/'EVAL_GEN_TAG' if worker 'i' is to call sim/gen_func
-        'libE_info' [dict]: Info sent to/from worker to help manager update the 'H'
+        'libE_info' [dict]: Info sent to/from worker to help manager update the 'H' array
 
-        Optional keys are:
+        libE_info contains the following:
         'H_rows' [list of ints]: History rows to send to worker 'i'
-        'blocking' [list of ints]: Workers to be blocked by this calculation
-        'persistent' [bool]: True if worker 'i' will enter persistent mode
+        'rset_team' [list of ints]: The resource sets to be assigned (if dynamic scheduling is used)
+        'persistent' [bool]: True if worker 'i' will enter persistent mode (Default: False)
+
+The work dictionary is typically set using the ``gen_work`` or ``sim_work``
+:doc:`helper functions<../function_guides/allocator>` in the allocation function.
+``H_fields``, for example, is usually packed from either ``sim_specs["in"]``, ``gen_specs["in"]``
+or the equivalent "persis_in" variants.
 
 .. seealso::
   For allocation functions giving work dictionaries using persistent workers,
   see `start_only_persistent.py`_ or `start_persistent_local_opt_gens.py`_.
   For a use case where the allocation and generator functions combine to do
-  simulation evaluations with different resources (blocking some workers), see
+  simulation evaluations with different resources, see
   `test_uniform_sampling_with_variable_resources.py`_.
 
 .. _start_only_persistent.py: https://github.com/Libensemble/libensemble/blob/develop/libensemble/alloc_funcs/start_only_persistent.py
 .. _start_persistent_local_opt_gens.py: https://github.com/Libensemble/libensemble/blob/develop/libensemble/alloc_funcs/start_persistent_local_opt_gens.py
 .. _test_uniform_sampling_with_variable_resources.py: https://github.com/Libensemble/libensemble/blob/develop/libensemble/tests/regression_tests/test_uniform_sampling_with_variable_resources.py
```

### Comparing `libensemble-0.9.2/docs/data_structures/worker_array.rst` & `libensemble-0.9.3/docs/data_structures/worker_array.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/dev_guide/release_management/release_platforms/rel_conda.rst` & `libensemble-0.9.3/docs/dev_guide/release_management/release_platforms/rel_conda.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/dev_guide/release_management/release_platforms/rel_github.rst` & `libensemble-0.9.3/docs/dev_guide/release_management/release_platforms/rel_github.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/dev_guide/release_management/release_platforms/rel_pypi.rst` & `libensemble-0.9.3/docs/dev_guide/release_management/release_platforms/rel_pypi.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/dev_guide/release_management/release_platforms/rel_spack.rst` & `libensemble-0.9.3/docs/dev_guide/release_management/release_platforms/rel_spack.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/dev_guide/release_management/release_process.rst` & `libensemble-0.9.3/docs/dev_guide/release_management/release_process.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/examples/alloc_funcs.rst` & `libensemble-0.9.3/docs/examples/alloc_funcs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/examples/aposmm.rst` & `libensemble-0.9.3/docs/examples/aposmm.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/examples/calling_scripts.rst` & `libensemble-0.9.3/docs/examples/calling_scripts.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/examples/examples_index.rst` & `libensemble-0.9.3/docs/examples/examples_index.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/examples/sampling.rst` & `libensemble-0.9.3/docs/examples/sampling.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/examples/sim_funcs.rst` & `libensemble-0.9.3/docs/examples/sim_funcs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/examples/surmise.rst` & `libensemble-0.9.3/docs/examples/surmise.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/examples/tasmanian.rst` & `libensemble-0.9.3/docs/examples/tasmanian.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/executor/executor.rst` & `libensemble-0.9.3/docs/executor/executor.rst`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 ---------------
 
 Only create an object of this class for running local serial-launched applications.
 To run MPI applications and use detected resources, use an alternative Executor
 class, as shown above.
 
 .. autoclass:: Executor
-  :members: __init__, register_app, submit
+  :members:
+  :exclude-members: serial_setup, sim_default_app, gen_default_app, get_app, default_app, set_resources, get_task, set_workerID, set_worker_info, new_tasks_timing
+
+  .. automethod:: __init__
 
 .. _task_tag:
 
 Task Class
 ----------
 
 Tasks are created and returned through the Executor ``submit()`` function. Tasks
```

### Comparing `libensemble-0.9.2/docs/executor/mpi_executor.rst` & `libensemble-0.9.3/docs/executor/mpi_executor.rst`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 .. automodule:: mpi_executor
   :no-undoc-members:
 
 .. autoclass:: MPIExecutor
   :show-inheritance:
   :inherited-members:
+  :exclude-members: serial_setup, sim_default_app, gen_default_app, get_app, default_app, set_resources, get_task, set_workerID, set_worker_info, new_tasks_timing
 
   .. automethod:: __init__
 
 ..  :member-order: bysource
 ..  :members: __init__, register_app, submit, manager_poll
 
 Class-specific Attributes
```

### Comparing `libensemble-0.9.2/docs/executor/overview.rst` & `libensemble-0.9.3/docs/executor/overview.rst`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     timeout_sec = 600
     poll_delay_sec = 1
 
     while(not task.finished):
 
         # Has manager sent a finish signal
         exctr.manager_poll()
-        if exctr.manager_signal == 'finish':
+        if exctr.manager_signal in [MAN_SIGNAL_KILL, MAN_SIGNAL_FINISH]:
             task.kill()
             my_cleanup()
 
         # Check output file for error and kill task
         elif task.stdout_exists():
             if 'Error' in task.read_stdout():
                 task.kill()
```

### Comparing `libensemble-0.9.2/docs/function_guides/allocator.rst` & `libensemble-0.9.3/docs/function_guides/allocator.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/function_guides/function_guide_index.rst` & `libensemble-0.9.3/docs/function_guides/function_guide_index.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/function_guides/generator.rst` & `libensemble-0.9.3/docs/function_guides/generator.rst`

 * *Files 9% similar despite different names*

```diff
@@ -48,21 +48,25 @@
     appended to ``persis_info``.
 
 .. _persistent-gens:
 
 Persistent Generators
 ---------------------
 
-While normal generators return after completing their calculation, persistent
-generators receive Work units, perform computations, and communicate results
-directly to the manager in a loop, not returning until explicitly instructed by
-the manager. The calling worker becomes a dedicated :ref:`persistent worker<persis_worker>`.
+While non-persistent generators return after completing their calculation, persistent
+generators receive work units, perform computations, and communicate results
+directly to the manager in a loop. A persistent generator returns either when
+explicitly instructed by the manager, or by exiting its main loop based on some
+condition. The allocation function can determine what to do once a persistent
+generator finishes, such as ending the ensemble.
+
+The calling worker becomes a dedicated :ref:`persistent worker<persis_worker>`.
 A ``gen_f`` is initiated as persistent by the ``alloc_f``.
 
-Most users prefer persistent generators since they do not need to be
+Many users prefer persistent generators since they do not need to be
 re-initialized every time their past work is completed and evaluated by a
 simulation, and can evaluate returned simulation results over the course of
 an entire libEnsemble routine as a single function instance. The :doc:`APOSMM<../examples/aposmm>`
 optimization generator function included with libEnsemble is persistent so it can
 maintain multiple local optimization subprocesses based on results from complete simulations.
 
 Functions for a persistent generator to communicate directly with the manager
@@ -125,56 +129,71 @@
 Active receive mode
 -------------------
 
 By default, a persistent worker (generator in this case) models the manager/worker
 communications of a regular worker (i.e., the generator is expected to alternately
 receive and send data in a *ping pong* fashion). To have an irregular communication
 pattern, a worker can be initiated in *active receive* mode by the allocation
-function (see :ref:`start_only_persistent<start_only_persistent_label>`).
+function (see :ref:`start_only_persistent<start_only_persistent_label>`). In this mode,
+the persistent worker will always be considered ready to receive more data
+(e.g.,~ evaluation results). It can also send to the manager at any time.
 
 The user is responsible for ensuring there are no communication deadlocks
 in this mode. Note that in manager/worker message exchanges, only the worker-side
-receive is blocking.
+receive is blocking by default (a non-blocking option is available).
 
 Cancelling Simulations
 ----------------------
 
 Previously submitted simulations can be cancelled by sending a message to the manager.
-To do this as a separate communication, a persistent generator should be
-in *active receive* mode to prevent a deadlock.
-
-To send out cancellations of previously submitted simulations, the generator
-can initiate a history array with just the ``sim_id`` and ``cancel_requested`` fields.
-Then fill in the ``sim_id``'s to cancel and set the ``cancel_requested`` field to ``True``.
-In the following example, ``sim_ids_to_cancel`` is a list of integers.
 
-.. code-block:: python
+To do this a PersistentSupport helper function is provided.
 
-    # Send only these fields to existing H rows and libEnsemble will slot in the change.
-    H_o = np.zeros(len(sim_ids_to_cancel), dtype=[('sim_id', int), ('cancel_requested', bool)])
-    H_o['sim_id'] = sim_ids_to_cancel
-    H_o['cancel_requested'] = True
-    my_support.send(H_o)
+.. currentmodule:: libensemble.tools.persistent_support.PersistentSupport
+.. autofunction:: request_cancel_sim_ids
 
 If a generated point is cancelled by the generator before it has been given to a
 worker for evaluation, then it will never be given. If it has already returned from the
 simulation, then results can be returned, but the ``cancel_requested`` field remains
 as ``True``. However, if the simulation is running when the manager receives the cancellation
 request, a kill signal will be sent to the worker. This can be caught and acted upon
 by a user function, otherwise it will be ignored.
 
 The :doc:`Borehole Calibration tutorial<../tutorials/calib_cancel_tutorial>` gives an example
 of the capability to cancel pending simulations.
 
+Modification of existing points
+-------------------------------
+
+To change existing fields of the history array, the generator can initialize an output
+array where the *dtype* contains the ``sim_id`` and the fields to be modified (in
+place of ``gen_specs["out"]``), and then send this output array to the manager (as with regular
+communications). Any such array received by the manager will overwrite the specific fields
+for the given *sim_ids*. If the changes do not correspond with newly generated points,
+then the generator needs to communicate to the manager that it is not ready
+to receive completed evaluations. Send to the manager with the ``keep_state`` argument
+set to *True*.
+
+For example, the cancellation function ``request_cancel_sim_ids`` could be replicated by
+the following (where ``sim_ids_to_cancel`` is a list of integers):
+
+.. code-block:: python
+
+    # Send only these fields to existing H rows and libEnsemble will slot in the change.
+    H_o = np.zeros(len(sim_ids_to_cancel), dtype=[('sim_id', int), ('cancel_requested', bool)])
+    H_o['sim_id'] = sim_ids_to_cancel
+    H_o['cancel_requested'] = True
+    ps.send(H_o, keep_state=True)
+
 Generator initiated shutdown
 ----------------------------
 
 If using a supporting allocation function, the generator can prompt the ensemble to shutdown
 by simply exiting the function (e.g., on a test for a converged value). For example, the
 allocation function :ref:`start_only_persistent<start_only_persistent_label>` closes down
 the ensemble as soon a persistent generator returns. The usual return values should be given.
 
 Examples
 --------
 
-Examples of normal and persistent generator functions
+Examples of non-persistent and persistent generator functions
 can be found :doc:`here<../examples/gen_funcs>`.
```

### Comparing `libensemble-0.9.2/docs/function_guides/simulator.rst` & `libensemble-0.9.3/docs/function_guides/simulator.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/history_output_logging.rst` & `libensemble-0.9.3/docs/history_output_logging.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/ANL_CMYK.png` & `libensemble-0.9.3/docs/images/ANL_CMYK.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/ECP_logo.png` & `libensemble-0.9.3/docs/images/ECP_logo.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/balsam2.png` & `libensemble-0.9.3/docs/images/balsam2.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/basic_6hc.png` & `libensemble-0.9.3/docs/images/basic_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/basic_6hc_simple.png` & `libensemble-0.9.3/docs/images/basic_6hc_simple.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/centralized_new_detailed.png` & `libensemble-0.9.3/docs/images/centralized_new_detailed.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/centralized_new_detailed_balsam.png` & `libensemble-0.9.3/docs/images/centralized_new_detailed_balsam.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/diagram_with_persis.png` & `libensemble-0.9.3/docs/images/diagram_with_persis.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/diagram_xml/balsam2.xml` & `libensemble-0.9.3/docs/images/diagram_xml/balsam2.xml`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/diagram_xml/persis_add_worker.xml` & `libensemble-0.9.3/docs/images/diagram_xml/persis_add_worker.xml`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/diagram_xml/persis_wasted_node.xml` & `libensemble-0.9.3/docs/images/diagram_xml/persis_wasted_node.xml`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/distributed_new_detailed.png` & `libensemble-0.9.3/docs/images/distributed_new_detailed.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/funcxmodel.png` & `libensemble-0.9.3/docs/images/funcxmodel.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/gen_v_fail_or_cancel.png` & `libensemble-0.9.3/docs/images/gen_v_fail_or_cancel.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/history_gen1.png` & `libensemble-0.9.3/docs/images/history_gen1.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/history_gen2.png` & `libensemble-0.9.3/docs/images/history_gen2.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/history_init.png` & `libensemble-0.9.3/docs/images/history_init.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/history_sim1.png` & `libensemble-0.9.3/docs/images/history_sim1.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/libE_logo.png` & `libensemble-0.9.3/docs/images/libE_logo.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/libE_logo_white.png` & `libensemble-0.9.3/docs/images/libE_logo_white.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/libEnsemble_Logo.svg` & `libensemble-0.9.3/docs/images/libEnsemble_Logo.svg`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/libe_opal_complete_v_killed_511w_2044sims_1030nodes.png` & `libensemble-0.9.3/docs/images/libe_opal_complete_v_killed_511w_2044sims_1030nodes.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/libe_opal_util_v_time_511w_2044sims_1030nodes.png` & `libensemble-0.9.3/docs/images/libe_opal_util_v_time_511w_2044sims_1030nodes.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/localopt_6hc.png` & `libensemble-0.9.3/docs/images/localopt_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/persis_add_worker.png` & `libensemble-0.9.3/docs/images/persis_add_worker.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/persis_wasted_node.png` & `libensemble-0.9.3/docs/images/persis_wasted_node.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/sampling_6hc.png` & `libensemble-0.9.3/docs/images/sampling_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/sinex.png` & `libensemble-0.9.3/docs/images/sinex.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/variable_resources1.png` & `libensemble-0.9.3/docs/images/variable_resources1.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/variable_resources2.png` & `libensemble-0.9.3/docs/images/variable_resources2.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/variable_resources3.png` & `libensemble-0.9.3/docs/images/variable_resources3.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/variable_resources_larger_rsets1.png` & `libensemble-0.9.3/docs/images/variable_resources_larger_rsets1.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/variable_resources_more_rsets1.png` & `libensemble-0.9.3/docs/images/variable_resources_more_rsets1.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/variable_resources_persis_gen1.png` & `libensemble-0.9.3/docs/images/variable_resources_persis_gen1.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/images/variable_resources_sched_opts.png` & `libensemble-0.9.3/docs/images/variable_resources_sched_opts.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/index.rst` & `libensemble-0.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/introduction_latex.rst` & `libensemble-0.9.3/docs/introduction_latex.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 .. _APOSMM: https://link.springer.com/article/10.1007/s12532-017-0131-4
 .. _AWA: https://link.springer.com/article/10.1007/s12532-017-0131-4
 .. _Balsam: https://balsam.readthedocs.io/en/latest/
 .. _Balsam Executor: https://libensemble.readthedocs.io/en/develop/executor/balsam_2_executor.html
 .. _Community Examples repository: https://github.com/Libensemble/libe-community-examples
 .. _Conda: https://docs.conda.io/en/latest/
 .. _conda-forge: https://conda-forge.org/
+.. _Contributions: https://github.com/Libensemble/libensemble/blob/main/CONTRIBUTING.rst
 .. _Coveralls: https://coveralls.io/github/Libensemble/libensemble?branch=main
 .. _DEAP: https://deap.readthedocs.io/en/master/overview.html
 .. _DFO-LS: https://github.com/numericalalgorithmsgroup/dfols
 .. _ECNoise: https://www.mcs.anl.gov/~wild/cnoise/
 .. _example user scripts: https://libensemble.readthedocs.io/en/main/examples/examples_index.html
 .. _funcX: https://funcx.org/
 .. _GitHub: https://github.com/Libensemble/libensemble
@@ -50,14 +51,16 @@
 .. _NLopt documentation: http://ab-initio.mit.edu/wiki/index.php/NLopt_Installation#Shared_libraries
 .. _nlopt: http://ab-initio.mit.edu/wiki/index.php/NLopt
 .. _NumPy: http://www.numpy.org
 .. _OPAL: http://amas.web.psi.ch/docs/opal/opal_user_guide-1.6.0.pdf
 .. _petsc4py: https://bitbucket.org/petsc/petsc4py
 .. _PETSc/TAO: http://www.mcs.anl.gov/petsc
 .. _poster: https://figshare.com/articles/libEnsemble_A_Python_Library_for_Dynamic_Ensemble-Based_Computations/12559520
+.. _PSI/J: https://exaworks.org/psij
+.. _psi-j-python: https://github.com/ExaWorks/psi-j-python
 .. _psutil: https://pypi.org/project/psutil/
 .. _PyPI: https://pypi.org
 .. _pytest-cov: https://pypi.org/project/pytest-cov/
 .. _pytest-timeout: https://pypi.org/project/pytest-timeout/
 .. _pytest: https://pypi.org/project/pytest/
 .. _Python: http://www.python.org
 .. _pyyaml: https://pyyaml.org/
@@ -68,12 +71,13 @@
 .. _Spack: https://spack.readthedocs.io/en/latest
 .. _Summit: https://www.olcf.ornl.gov/olcf-resources/compute-systems/summit/
 .. _Surmise: https://surmise.readthedocs.io/en/latest/index.html
 .. _SWIG: http://swig.org/
 .. _tarball: https://github.com/Libensemble/libensemble/releases/latest
 .. _Tasmanian: https://tasmanian.ornl.gov/
 .. _Theta: https://www.alcf.anl.gov/alcf-resources/theta
+.. _tqdm: https://tqdm.github.io/
 .. _user guide: https://libensemble.readthedocs.io/en/latest/programming_libE.html
 .. _VTMOP: https://informs-sim.org/wsc20papers/311.pdf
 .. _WarpX: https://warpx.readthedocs.io/en/latest/
 .. _WarpX + libE scripts: https://warpx.readthedocs.io/en/latest/usage/workflows/libensemble.html
 .. _xSDK Extreme-scale Scientific Software Development Kit: https://xsdk.info
```

### Comparing `libensemble-0.9.2/docs/latex_index.rst` & `libensemble-0.9.3/docs/latex_index.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/overview_usecases.rst` & `libensemble-0.9.3/docs/overview_usecases.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/platforms/bebop.rst` & `libensemble-0.9.3/docs/platforms/bebop.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/platforms/cori.rst` & `libensemble-0.9.3/docs/platforms/cori.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/platforms/example_scripts.rst` & `libensemble-0.9.3/docs/platforms/example_scripts.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Example libEnsemble Submission Scripts
 ======================================
 
 Below are example submission scripts used to configure and launch libEnsemble
 on a variety of high-powered systems. See :doc:`here<platforms_index>` for more
 information about the respective systems and configuration.
 
+Alternatively to interacting with the scheduler or configuring submission scripts,
+libEnsemble now features a portable set of :ref:`command-line utilities<liberegister>`
+for submitting workflows to almost any system or scheduler.
+
 Slurm - Basic
 -------------
 
 ..  literalinclude:: ../../examples/libE_submission_scripts/submit_slurm_simple.sh
     :caption: /examples/libE_submission_scripts/submit_slurm_simple.sh
     :language: bash
```

### Comparing `libensemble-0.9.2/docs/platforms/perlmutter.rst` & `libensemble-0.9.3/docs/platforms/perlmutter.rst`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     inherited by the job on Perlmutter.
 
 This example calling script has the following line so the node is divided into
 four resource sets (the example generator does not need dedicated resources):
 
 .. code-block:: python
 
-    libE_specs['zero_resource_workers'] = [1]
+    libE_specs['num_resource_sets'] = 4
 
 The MPIExecutor is also initiated in the calling script, ensuring that ``srun`` is picked up::
 
     from libensemble.executors.mpi_executor import MPIExecutor
     exctr = MPIExecutor(custom_info={'mpi_runner':'srun'})
 
 Each worker runs a simulator function that uses the :doc:`MPIExecutor<../executor/mpi_executor>`
```

### Comparing `libensemble-0.9.2/docs/platforms/platforms_index.rst` & `libensemble-0.9.3/docs/platforms/platforms_index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -135,39 +135,41 @@
 accesses the resources available to the current worker when launching tasks.
 
 Zero-resource workers
 ~~~~~~~~~~~~~~~~~~~~~
 
 Users with persistent ``gen_f`` functions may notice that the persistent workers
 are still automatically assigned system resources. This can be resolved by
-using :ref:`zero resource workers<zero_resource_workers>`.
+:ref:`fixing the number of resource sets<zero_resource_workers>`.
 
 Overriding Auto-detection
 -------------------------
 
 libEnsemble can automatically detect system information. This includes resource information, such as
 available nodes and the number of cores on the node, and information about available MPI runners.
 
 System detection for resources can be overridden using the :ref:`resource_info<resource_info>`
 libE_specs option.
 
 When using the MPI Executor, it is possible to override the detected information using the
 `custom_info` argument. See the :doc:`MPI Executor<../executor/mpi_executor>` for more.
 
+ .. _funcx_ref:
+
 funcX - Remote User functions
 -----------------------------
 
 *Alternatively to much of the above*, if libEnsemble is running on some resource with
 internet access (laptops, login nodes, other servers, etc.), workers can be instructed to
 launch generator or simulator user function instances to separate resources from
 themselves via funcX_, a distributed, high-performance function-as-a-service platform:
 
-    .. image:: ../images/funcx.png
+    .. image:: ../images/funcxmodel.png
         :alt: running_with_funcx
-        :scale: 40
+        :scale: 50
         :align: center
 
 This is useful for running ensembles across machines and heterogeneous resources, but
 comes with several caveats:
 
     1. User functions registered with funcX must be *non-persistent*, since
        manager-worker communicators can't be serialized or used by a remote resource.
```

### Comparing `libensemble-0.9.2/docs/platforms/spock_crusher.rst` & `libensemble-0.9.3/docs/platforms/spock_crusher.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/platforms/srun.rst` & `libensemble-0.9.3/docs/platforms/srun.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/platforms/summit.rst` & `libensemble-0.9.3/docs/platforms/summit.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/platforms/theta.rst` & `libensemble-0.9.3/docs/platforms/theta.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/posters.rst` & `libensemble-0.9.3/docs/posters.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/resource_manager/overview.rst` & `libensemble-0.9.3/docs/resource_manager/overview.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,48 +4,47 @@
 Overview
 --------
 
 libEnsemble comes with built-in resource management. This entails the
 :ref:`detection of available resources<resource_detection>` (e.g., nodelists and
 core counts), and the allocation of resources to workers.
 
-By default, the provisioned resources are divided by the number of workers (excluding
-any workers given in the ``zero_resource_workers`` libE_specs option). libEnsemble's
-:doc:`MPI Executor<../executor/mpi_executor>` is aware of these supplied resources,
-and if not given any of ``num_nodes``, ``num_procs``, or ``procs_per_node`` in the submit
-function, it will try to use all nodes and CPU cores available to the worker.
+By default, the provisioned resources are divided by the number of workers.
+libEnsemble's :doc:`MPI Executor<../executor/mpi_executor>` is aware of
+these supplied resources, and if not given any of ``num_nodes``, ``num_procs``,
+or ``procs_per_node`` in the submit function, it will try to use all nodes and
+CPU cores available to the worker.
 
 Detected resources can be overridden using the libE_specs option :ref:`resource_info<resource_info>`.
 
-Resource management can be disabled by setting
-``libE_specs['disable_resource_manager'] = True``. This will prevent libEnsemble
-from doing any resource detection or management.
-
 Variable resource assignment
 ----------------------------
 
 In slightly more detail, the resource manager divides resources into **resource sets**.
 One resource set is the smallest unit of resources that can be assigned (and
 dynamically reassigned) to workers. By default, the provisioned resources are
-divided by the number of workers (excluding any workers given in the ``zero_resource_workers``
-``libE_specs`` option). However, it can also be set directly by the ``num_resource_sets``
-``libE_specs`` option. If the latter is set, the dynamic resource assignment algorithm
-will always be used.
+divided by the number of workers (excluding any workers given in the
+``zero_resource_workers`` ``libE_specs`` option). However, it can also be set
+directly by the ``num_resource_sets`` ``libE_specs`` option. If the latter is set,
+the dynamic resource assignment algorithm will always be used.
 
 If there are more resource sets than nodes, then the resource sets on each node
-will be given a slot number, enumerated from zero. For example, if there are three slots
-on a node, they will have slot numbers 0, 1, and 2.
+will be given a slot number, enumerated from zero. For example, if there are three
+slots on a node, they will have slot numbers 0, 1, and 2.
 
 The resource manager will not split a resource set over nodes, rather the resource
 sets on each node will be the integer division of resource sets over nodes, with
 the remainder dealt out from the first node. Even breakdowns are generally
 preferable, however.
 
 For example, say a given system has four GPUs per node, and the user has run
-libEnsemble on two nodes, with eight workers. The default division of resources would be:
+libEnsemble on two nodes, with eight workers. The default division of resources
+would be:
+
+.. _rsets-diagram:
 
 .. image:: ../images/variable_resources1.png
 
 Variable Size simulations
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 A dynamic assignment of resources to simulation workers can be achieved by the
@@ -62,15 +61,15 @@
     gen_specs = {'gen_f': gen_f,
                  'in': ['sim_id'],
                  'out': [('priority', float),
                          ('resource_sets', int),
                          ('x', float, n)]
                 }
 
-For an example calling script, see The libEnsemble regression test
+For an example calling script, see the regression test
 `test_persistent_sampling_CUDA_variable_resources.py`_
 
 In the generator, the ``resource_sets`` field must be set to a value for each point
 (simulation) generated (if it is not set, it will have the initialized value of zero,
 and supply zero resources).
 
 .. code-block:: python
@@ -118,18 +117,17 @@
 For example, in *six_hump_camel_CUDA_variable_resources*, the environment variable
 ``CUDA_VISIBLE_DEVICES`` is set to slots:
 
 .. code-block:: python
     :emphasize-lines: 3
 
     resources = Resources.resources.worker_resources
-    if resources.even_slots:  # Need same slots on each node
-        resources.set_env_to_slots("CUDA_VISIBLE_DEVICES")  # Use convenience function.
-        num_nodes = resources.local_node_count
-        cores_per_node = resources.slot_count  # One CPU per GPU
+    resources.set_env_to_slots("CUDA_VISIBLE_DEVICES")  # Use convenience function.
+    num_nodes = resources.local_node_count
+    cores_per_node = resources.slot_count  # One CPU per GPU
 
 In the figure above, this would result in worker one setting::
 
     export CUDA_VISIBLE_DEVICES=0,1
 
 while worker five would set::
 
@@ -192,25 +190,27 @@
 
 Persistent generator
 ^^^^^^^^^^^^^^^^^^^^
 
 You have *one* persistent generator and want *eight* workers for running concurrent
 simulations. In this case you can run with *nine* workers.
 
-Either use one zero resource worker, if the generator should always be the same worker:
+Either explicitly set eight resource sets (recommended):
 
 .. code-block:: python
 
-    libE_specs['zero_resource_workers'] = [1]
+    libE_specs['num_resource_sets'] = 8
 
-Or explicitly set eight resource sets:
+Or if the generator should always be the same worker, use one zero resource worker:
 
 .. code-block:: python
 
-    libE_specs['num_resource_sets'] = 8
+    libE_specs['zero_resource_workers'] = [1]
+
+For the second option, an allocation function supporting zero resource workers must be used.
 
 Using the two-node example above, the initial worker mapping in this example will be:
 
 .. image:: ../images/variable_resources_persis_gen1.png
     :width: 98%
 
 Using large resource sets
```

### Comparing `libensemble-0.9.2/docs/resource_manager/resource_detection.rst` & `libensemble-0.9.3/docs/resource_manager/resource_detection.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/resource_manager/scheduler_module.rst` & `libensemble-0.9.3/docs/resource_manager/scheduler_module.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/scipy2020.rst` & `libensemble-0.9.3/docs/scipy2020.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,14 @@
  :align: left
 
 .. image:: images/ANL_CMYK.png
  :alt: ANL
  :width: 33 %
  :align: right
 
-.. image:: images/white.png
-  :align: center
-  :width: 33 %
-  :height: 1.2 in
-
 =========================================================================
 **libEnsemble**: A Python Library for Dynamic Ensemble-Based Computations
 =========================================================================
 
 *David Bindel, Stephen Hudson, Jeffrey Larson, John-Luke Navarro and Stefan Wild*
 
 A PDF poster version of this content is available on figshare_.
@@ -47,19 +42,14 @@
 -----------------
 
 The user selects or supplies a ``gen_f`` function  that generates simulation
 input and a ``sim_f`` function that performs and monitors simulations. The user
 parameterizes these functions and initiates libEnsemble in a *calling script*.
 Examples and templates of such scripts and functions are included in the library.
 
-.. image:: images/using_new.png
- :alt: Using libEnsemble
- :scale: 30 %
- :align: center
-
 For example, the ``gen_f`` may contain an optimization routine to generate new
 simulation parameters on-the-fly based on results from previous ``sim_f``
 simulations.
 
 Other potential use-cases include:
 
 ====================             =====================
@@ -78,37 +68,32 @@
 libEnsemble employs a manager/worker scheme that can communicate through **MPI**,
 Python's **multiprocessing**, or **TCP**. Each *worker*
 can control and monitor any level of work, from small sub-node tasks to huge
 many-node simulations. The *manager* allocates workers to asynchronously execute
 ``gen_f`` generation functions and ``sim_f`` simulation functions based on
 produced output, directed by a provided ``alloc_f`` allocation function.
 
-.. image:: images/logo_manager_worker.png
- :alt: Managers and Workers
- :align: center
- :scale: 40 %
-
 Flexible Run Mechanisms
 -----------------------
 
 libEnsemble has been developed, supported, and tested on systems of highly
 varying scales, from laptops to machines with thousands of compute nodes.
 On multi-node systems, there are two basic modes of configuring libEnsemble to
 run and launch tasks (user applications) on available nodes.
 
 * **Distributed**: Workers are distributed across allocated nodes and launch tasks in-place. Workers share nodes with their applications.
 
-.. image:: images/distributed_new.png
+.. image:: images/distributed_new_detailed.png
  :alt: Distributed
  :align: center
  :scale: 30 %
 
 * **Centralized**: Workers run on one or more dedicated nodes and launch tasks to the remaining allocated nodes.
 
-.. image:: images/centralized_new.png
+.. image:: images/centralized_new_detailed.png
  :alt: Centralized
  :align: center
  :scale: 30 %
 
 .. note::
     Dividing up workers and tasks to allocated nodes is highly configurable.
     Multiple workers (and thus multiple tasks or user function instances) can be
@@ -128,15 +113,15 @@
 ``submit()``, ``poll()``, and ``kill()``.
 
 On machines that do not support launches from compute nodes, libEnsemble's
 Executor can interface with the **Balsam** library, which functions as a proxy
 job launcher that maintains and submits jobs from a database on front end launch
 nodes.
 
-.. image:: images/central_balsam.png
+.. image:: images/centralized_new_detailed_balsam.png
  :alt: Central Balsam
  :align: center
  :scale: 40 %
 
 Supported Research Machines
 ---------------------------
```

### Comparing `libensemble-0.9.2/docs/sim_gen_alloc_funcs.rst` & `libensemble-0.9.3/docs/sim_gen_alloc_funcs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/tutorials/aposmm_tutorial.rst` & `libensemble-0.9.3/docs/tutorials/aposmm_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/tutorials/calib_cancel_tutorial.rst` & `libensemble-0.9.3/docs/tutorials/calib_cancel_tutorial.rst`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,16 @@
 have been marked as cancelled.
 
 Overview of the Calibration Problem
 -----------------------------------
 
 The generator function featured in this tutorial can be found in
 ``gen_funcs/persistent_surmise_calib.py`` and uses the `surmise`_ library for its
-calibration surrogate model interface.
-
-.. note::
-    Note that this repository is a fork of
-    the main surmise repository, but it retains support for the "PCGPwM" emulation
-    method used in the generator. surmise is under active development.
+calibration surrogate model interface. The surmise library uses the  "PCGPwM"
+emulation method in this example.
 
 Say there is a computer model :math:`f(\theta, x)` to be calibrated.  To calibrate
 is to find some parameter :math:`\theta_0` such that :math:`f(\theta_0, x)` closely
 resembles data collected from a physical experiment.  For example, a (simple)
 physical experiment may involve dropping a ball at different heights to study the
 gravitational constant, and the corresponding computer model could be the set of
 differential equations that governs the drop. In a case where the computation of
@@ -101,51 +97,45 @@
 cancelled ("obviated"). If so, the generator then calls ``cancel_columns()``::
 
     if select_condition(pending):
         new_theta, info = select_next_theta(step_add_theta, cal, emu, pending, n_explore_theta)
         ...
         c_obviate = info['obviatesugg']  # suggested
         if len(c_obviate) > 0:
-            cancel_columns(obs_offset, c_obviate, n_x, pending, comm)
+            cancel_columns(obs_offset, c_obviate, n_x, pending, ps)
 
 ``obs_offset`` is an offset that excludes the observations when mapping points in surmise
 data structures to ``sim_id``'s, ``c_obviate`` is a selection
 of columns to cancel, ``n_x`` is the number of ``x`` values, and ``pending`` is used
-to check that points marked for cancellation have not already returned. ``comm`` is a
-communicator object from :doc:`libE_info<../data_structures/work_dict>` used to send
-and receive messages from the Manager.
+to check that points marked for cancellation have not already returned. ``ps`` is the
+instantiation of the *PersistentSupport* class that is set up for persistent generators, and
+provides an interface for communication with the manager.
 
 Within ``cancel_columns()``, each column in ``c_obviate`` is iterated over, and if a
 point is ``pending`` and thus has not yet been evaluated by a simulation,
 its ``sim_id`` is appended to a list to be sent to the Manager for cancellation.
-A new, separate local :doc:`History array<../history_output_logging>` is defined with the
-selected ``'sim_id'`` s and the ``'cancel_requested'`` field set to ``True``. This array is
-then sent to the Manager using the ``send_mgr_worker_msg`` persistent generator
-helper function. Each of these helper functions is described :ref:`here<p_gen_routines>`.
-The entire ``cancel_columns()`` routine is listed below:
+Cancellation is requested using the helper function ``request_cancel_sim_ids`` provided
+by the *PersistentSupport* class.  Each of these helper functions is described
+:ref:`here<p_gen_routines>`. The entire ``cancel_columns()`` routine is listed below:
 
 .. code-block:: python
 
-    def cancel_columns(obs_offset, c, n_x, pending, comm):
+    def cancel_columns(obs_offset, c, n_x, pending, ps):
         """Cancel columns"""
         sim_ids_to_cancel = []
         columns = np.unique(c)
         for c in columns:
             col_offset = c*n_x
             for i in range(n_x):
                 sim_id_cancel = obs_offset + col_offset + i
                 if pending[i, c]:
                     sim_ids_to_cancel.append(sim_id_cancel)
                     pending[i, c] = 0
 
-        # Send only these fields to existing H rows and libEnsemble will slot in the change.
-        H_o = np.zeros(len(sim_ids_to_cancel), dtype=[('sim_id', int), ('cancel_requested', bool)])
-        H_o['sim_id'] = sim_ids_to_cancel
-        H_o['cancel_requested'] = True
-        send_mgr_worker_msg(comm, H_o)
+        ps.request_cancel_sim_ids(sim_ids_to_cancel)
 
 In future calls to the allocation function by the manager, points that would have
 been distributed for simulation work but are now marked with "cancel_requested" will not
 be processed. The manager will send kill signals to workers that are already processing
 cancelled points. These signals can be caught and acted on by the user ``sim_f``; otherwise
 they will be ignored.
 
@@ -170,19 +160,18 @@
 **init_sample_size** gives the size of the initial sample that is batch returned to the gen.
 This is calculated from other parameters in the calling script.
 
 **active_recv_gen** allows the persistent generator to handle irregular communications (see below).
 
 By default, workers (including persistent workers), are only
 allocated work when they're in an :doc:`idle or non-active state<../data_structures/worker_array>`.
-However, since this generator must asynchronously update its model and
-cancel pending evaluations, the worker running this generator remains
-in an *active receive* state, until it becomes non-persistent. This means
-both the manager and persistent worker (generator in this case) must be
-prepared for irregular sending /receiving of data.
+However, since this generator must asynchronously update its model, the worker
+running this generator remains in an *active receive* state, until it becomes
+non-persistent. This means both the manager and persistent worker (generator in
+this case) must be prepared for irregular sending/receiving of data.
 
 .. Manager - Cancellation, History Updates, and Allocation
 .. -------------------------------------------------------
 ..
 .. Between routines to call the allocation function and distribute allocated work
 .. to each Worker, the Manager selects points from the History array that are:
 ..
@@ -236,15 +225,15 @@
 ..     def polling_loop(exctr, task, sim_id):
 ..         calc_status = UNSET_TAG
 ..         poll_interval = 0.01
 ..
 ..         # Poll task for finish and poll manager for kill signals
 ..         while(not task.finished):
 ..             exctr.manager_poll()
-..             if exctr.manager_signal == 'kill':
+..             if exctr.manager_signal == MAN_SIGNAL_KILL:
 ..                 task.kill()
 ..                 calc_status = MAN_SIGNAL_KILL
 ..                 break
 ..             else:
 ..                 task.poll()
 ..                 time.sleep(poll_interval)
 ..
@@ -252,15 +241,15 @@
 ..             calc_status = TASK_FAILED
 ..
 ..         return calc_status
 ..
 .. While the launched task isn't finished, the simulator function periodically polls
 .. both the task's statuses and for signals from the manager via
 .. the :ref:`executor.manager_poll()<manager_poll_label>` function.
-.. Immediately after ``exctr.manager_signal`` is confirmed as ``'kill'``, the current
+.. Immediately after ``exctr.manager_signal`` is confirmed as ``MAN_SIGNAL_KILL``, the current
 .. task is killed and the function returns with the
 .. ``MAN_SIGNAL_KILL`` :doc:`calc_status<../data_structures/calc_status>`.
 .. This status will be logged in ``libE_stats.txt``.
 
 Calling Script - Reading Results
 --------------------------------
```

### Comparing `libensemble-0.9.2/docs/tutorials/executor_forces_tutorial.rst` & `libensemble-0.9.3/docs/tutorials/executor_forces_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/tutorials/forces_gpu_tutorial.rst` & `libensemble-0.9.3/docs/tutorials/forces_gpu_tutorial.rst`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,20 @@
 ``#pragma omp target`` line uncommented and comment out the equivalent
 ``#pragma omp parallel`` line. Then compile **forces.x** using one of the
 GPU build lines in build_forces.sh_ or similar for your platform.
 
 The libEnsemble scripts in this example are available under forces_gpu_ in
 the libEnsemble repository.
 
-Note that at time of writing the calling script ``run_libe_forces.py`` is identical
-to that in ``forces_simple``. The ``forces_simf`` file has slight modifications to
-assign GPUs.
+Note that at the time of writing, the calling script **run_libe_forces.py** is functionally
+the same as that in *forces_simple*, but contains some commented out lines that can
+be used for a variable resources example. The *forces_simf.py* file has slight modifications
+to assign GPUs.
+
+Videos demonstrate running this example on Perlmutter_ and Spock_.
 
 Simulation function
 -------------------
 
 The ``sim_f`` (``forces_simf.py``) becomes as follows. The new lines are highlighted:
 
 .. code-block:: python
@@ -102,14 +105,19 @@
 and the line::
 
     resources.set_env_to_slots("CUDA_VISIBLE_DEVICES")
 
 will set the environment variable ``CUDA_VISIBLE_DEVICES`` to match the assigned
 slots (partitions on the node).
 
+.. note::
+    **slots** refers to the ``resource sets`` enumerated on a node (starting with
+    zero). If a resource set has more than one node, then each node is considered to
+    have slot zero. [:ref:`diagram<rsets-diagram>`]
+
 Note that if you are on a system that automatically assigns free GPUs on the node,
 then setting ``CUDA_VISIBLE_DEVICES`` is not necessary unless you want to ensure
 workers are strictly bound to GPUs. For example, on many **SLURM** systems, you
 can use ``--gpus-per-task=1`` (e.g., :doc:`Perlmutter<../platforms/perlmutter>`).
 Such options can be added to the `exctr.submit` call as ``extra_args``::
 
     task = exctr.submit(
@@ -128,47 +136,50 @@
 -------------------
 
 As an example, if you have been allocated two nodes, each with four GPUs, then assign
 eight workers. For example::
 
     python run_libe_forces.py --comms local --nworkers 8
 
-If you are running one persistent generator which does not require
-resources, then assign nine workers, and set the following in your
-calling script::
-
-    libE_specs['zero_resource_workers'] = [1]
-
-Or - if you do not care which worker runs the generator, you could fix the
-*resource_sets*::
+Note that if you are running one persistent generator that does not require
+resources, then assign nine workers, and fix the number of *resource_sets* in
+you calling script::
 
     libE_specs['num_resource_sets'] = 8
 
+See :ref:`zero resource workers<zero_resource_workers>` for more ways to express this.
+
 Changing number of GPUs per worker
 ----------------------------------
 
 If you want to have two GPUs per worker on the same system (four GPUs per node),
 you could assign only four workers, and change line 24 to::
 
     resources.set_env_to_slots("CUDA_VISIBLE_DEVICES", multiplier=2)
 
 In this case there are two GPUs per worker (and per slot).
 
 Varying resources
 -----------------
 
 The same code can be used when varying worker resources. In this case, you may
-choose to set one worker per GPU (as we did originally). Then add ``resource_sets``
-as a ``gen_specs['out']`` in your calling script. Simply assign the
-``resource_sets`` field of :doc:`H<../data_structures/history_array>` for each point
-generated.
-
-In this case the above code would still work, assigning one CPU processor and
-one GPU to each rank. If you want to have one rank with multiple GPUs, then
-change source lines 29/30 accordingly.
+add an integer field called ``resource_sets`` as a ``gen_specs['out']`` in your
+calling script.
+
+In the generator function, assign the ``resource_sets`` field of
+:doc:`H<../data_structures/history_array>` for each point generated. For example
+if a larger simulation requires two MPI tasks (and two GPUs), set ``resource_sets``
+field to *2* for that sim_id in the generator function.
+
+The calling script run_libe_forces.py_ contains alternative commented out lines for
+a variable resource example. Search for "Uncomment for var resources"
+
+In this case, the simulator function will still work, assigning one CPU processor
+and one GPU to each MPI rank. If you want to have one rank with multiple GPUs,
+then change source lines 29/30 accordingly.
 
 Further guidance on varying resource to workers can be found under the
 :doc:`resource manager<../resource_manager/resources_index>`.
 
 Checking GPU usage
 ------------------
 
@@ -225,7 +236,10 @@
 
 where ``SLURM_EXACT`` and ``SLURM_MEM_PER_NODE`` are set to prevent
 resource conflicts on each node.
 
 .. _forces_gpu: https://github.com/Libensemble/libensemble/blob/develop/libensemble/tests/scaling_tests/forces/forces_gpu
 .. _forces.c: https://github.com/Libensemble/libensemble/blob/develop/libensemble/tests/scaling_tests/forces/forces_app/forces.c
 .. _build_forces.sh: https://github.com/Libensemble/libensemble/blob/develop/libensemble/tests/scaling_tests/forces/forces_app/build_forces.sh
+.. _Perlmutter: https://www.youtube.com/watch?v=Av8ctYph7-Y
+.. _Spock: https://www.youtube.com/watch?v=XHXcslDORjU
+.. _run_libe_forces.py: https://github.com/Libensemble/libensemble/blob/develop/libensemble/tests/scaling_tests/forces/forces_gpu/run_libe_forces.py
```

### Comparing `libensemble-0.9.2/docs/tutorials/local_sine_tutorial.rst` & `libensemble-0.9.3/docs/tutorials/local_sine_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/utilities.rst` & `libensemble-0.9.3/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/welcome.rst` & `libensemble-0.9.3/docs/welcome.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/docs/xSDK_policy_compatibility.md` & `libensemble-0.9.3/docs/xSDK_policy_compatibility.md`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/README.rst` & `libensemble-0.9.3/examples/README.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/alloc_funcs/fast_alloc.py` & `libensemble-0.9.3/examples/alloc_funcs/fast_alloc.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/alloc_funcs/fast_alloc_to_aposmm.py` & `libensemble-0.9.3/examples/alloc_funcs/fast_alloc_to_aposmm.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/alloc_funcs/give_sim_work_first.py` & `libensemble-0.9.3/examples/alloc_funcs/give_sim_work_first.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/alloc_funcs/start_only_persistent.py` & `libensemble-0.9.3/examples/alloc_funcs/start_only_persistent.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/alloc_funcs/start_persistent_local_opt_gens.py` & `libensemble-0.9.3/examples/alloc_funcs/start_persistent_local_opt_gens.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/check_libE_stats.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/check_libE_stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     If just time, then t2 will be non-datetime.
     If second is datetime (time), then merger should be a datetime
     """
     if is_date(t2):
         dt = t1 + " " + t2
     else:
         dt = t1
-    assert is_date(dt), "Expected a datetime, found {}".format(dt)
+    assert is_date(dt), f"Expected a datetime, found {dt}"
 
 
 def check_start_end_times(start="Start:", end="End:", everyline=True):
     """Iterate over rows in infile and check delimiters and datetime formats"""
     with open(infile) as f:
         total_cnt = 0
         for line in f:
@@ -54,17 +54,17 @@
                 if val == end:
                     e1 = lst[i + 1]
                     e2 = lst[i + 2]
                     check_datetime(e1, e2)
                     e_cnt += 1
             if everyline:
                 assert s_cnt > 0, "Expected timings not found"
-            assert s_cnt == e_cnt, "Start/end count different {} {}".format(s_cnt, e_cnt)
+            assert s_cnt == e_cnt, f"Start/end count different {s_cnt} {e_cnt}"
             total_cnt += s_cnt
-        assert total_cnt > 0, "No timings found starting {}".format(start)
+        assert total_cnt > 0, f"No timings found starting {start}"
 
 
 def check_libE_stats(task_datetime=False):
     """Determine and run checks"""
     check_start_end_times()
     if task_datetime:
         check_start_end_times(start="Tstart:", end="Tend:", everyline=False)
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/common.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     import balsam
 
     rcfile = os.path.abspath("./libensemble/tests/regression_tests/.bal_coveragerc")
 
     old_line = "            path = ' '.join((exe, script_path, args))\n"
     new_line = (
         "            path = ' '.join((exe, '-m coverage run "
-        + "--parallel-mode --rcfile={}', script_path, args))\n".format(rcfile)
+        + f"--parallel-mode --rcfile={rcfile}', script_path, args))\n"
     )
 
     commandfile = "cli_commands.py"
     balsam_path = os.path.dirname(balsam.__file__) + "/scripts"
     balsam_commands_path = os.path.join(balsam_path, commandfile)
 
     with open(balsam_commands_path, "r") as f:
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/dont_run_test_persistent_aposmm_pounders.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_pounders.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 def combine_component(x):
     return np.sum(np.power(x, 2))
 
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/dont_run_test_persistent_aposmm_tao_blmvm.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_blmvm.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
 from libensemble.tests.regression_tests.support import six_hump_camel_minima as minima
 from time import time
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if is_manager:
         start_time = time()
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/dont_run_test_persistent_aposmm_tao_nm.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_nm.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 from libensemble.alloc_funcs.persistent_aposmm_alloc import persistent_aposmm_alloc as alloc_f
 from libensemble.tools import parse_args, add_unique_random_streams
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/dont_run_test_persistent_gp.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_gp.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/script_test_balsam_hworld.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/script_test_balsam_hworld.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     if is_manager:
         print("\nChecking expected task status against Workers ...\n")
         calc_status_list_in = np.asarray(
             [WORKER_DONE, WORKER_KILL_ON_ERR, WORKER_DONE, WORKER_KILL_ON_TIMEOUT, TASK_FAILED]
         )
         calc_status_list = np.repeat(calc_status_list_in, nworkers)
 
-        print("Expecting: {}".format(calc_status_list))
-        print("Received:  {}\n".format(H["cstat"]))
+        print(f"Expecting: {calc_status_list}")
+        print(f"Received:  {H['cstat']}\n")
 
         assert np.array_equal(H["cstat"], calc_status_list), "Error - unexpected calc status. Received: " + str(
             H["cstat"]
         )
 
         # Check dry_run submissions inside ensemble.log
         with open("ensemble.log", "r") as f:
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ECnoise.m` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ECnoise.m`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/configure-balsam-test.sh` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/configure-balsam-test.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/test_balsam_hworld.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/test_balsam_hworld.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # This test is NOT submitted as a job to Balsam. script_test_balsam_hworld.py is
 #   the executable submitted to Balsam as a job. This test executes that job
 #   through the 'runstr' line in run_Balsam_job()
 
 
 def run_Balsam_job():
     runstr = "balsam launcher --consume-all --job-mode=mpi --num-transition-threads=1"
-    print("Executing Balsam job with command: {}".format(runstr))
+    print(f"Executing Balsam job with command: {runstr}")
     subprocess.Popen(runstr.split())
 
 
 def build_simfunc():
     buildstring = "mpicc -o my_simtask.x ../unit_tests/simdir/my_simtask.c"
     subprocess.check_call(buildstring.split())
 
@@ -32,48 +32,48 @@
     print("Waiting for Balsam Database directory.")
     while sleeptime < limit:
         if os.path.isdir(basedb):
             break
         time.sleep(1)
         sleeptime += 1
 
-    assert sleeptime < limit, "Balsam Database directory not created within {} seconds.".format(limit)
+    assert sleeptime < limit, f"Balsam Database directory not created within {limit} seconds."
 
     # Stop sleeping once job directory detected within database directory
-    print("Waiting for Job Directory {}".format(sleeptime))
+    print(f"Waiting for Job Directory {sleeptime}")
     while sleeptime < limit:
         if len(os.listdir(basedb)) > 0:
             break
         print(sleeptime, end=" ", flush=True)
         time.sleep(1)
         sleeptime += 1
 
-    assert sleeptime < limit, "Balsam Job directory not created within {} seconds.".format(limit)
+    assert sleeptime < limit, f"Balsam Job directory not created within {limit} seconds."
 
     # Assumes database dir was empty, now contains single job dir
     jobdir = os.path.join(basedb, os.listdir(basedb)[0])
     return jobdir
 
 
 def wait_for_job_output(jobdir):
     sleeptime = 0
     limit = 60
 
     output = os.path.join(jobdir, "job_script_test_balsam_hworld.out")
-    print("Checking for Balsam output file: {}".format(output))
+    print(f"Checking for Balsam output file: {output}")
 
     while sleeptime < limit:
         if os.path.isfile(output):
             break
         print(sleeptime, end=" ", flush=True)
         print(os.listdir(jobdir), flush=True)
         time.sleep(1)
         sleeptime += 1
 
-    assert sleeptime < limit, "Balsam output file not created within {} seconds.".format(limit)
+    assert sleeptime < limit, f"Balsam output file not created within {limit} seconds."
 
     return output
 
 
 def print_job_output(outscript):
     sleeptime = 0
     limit = 90
@@ -90,15 +90,15 @@
         if succeed_line in lines:
             print("Success. Received task statuses match expected.")
             break
 
         time.sleep(1)
         sleeptime += 1
 
-    assert sleeptime < limit, "Expected Balsam Job output-file contents not detected after {} seconds.".format(limit)
+    assert sleeptime < limit, f"Expected Balsam Job output-file contents not detected after {limit} seconds."
 
 
 def move_job_coverage(jobdir):
     # Move coverage files from Balsam DB to ./regression_tests (for concatenation)
     print("Moving job coverage results.")
     here = os.getcwd()
     covname = ".cov_reg_out."
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/support.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/support.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,50 +28,50 @@
     return (H, persis_info)
 
 
 def write_sim_func(calc_in, persis_info, sim_specs, libE_info):
     out = np.zeros(1, dtype=sim_specs["out"])
     out["f"] = calc_in["x"]
     with open("test_sim_out.txt", "a") as f:
-        f.write("sim_f received: {}\n".format(out["f"]))
+        f.write(f"sim_f received: {out['f']}\n")
     return out, persis_info
 
 
 def remote_write_sim_func(calc_in, persis_info, sim_specs, libE_info):
     import numpy as np
 
     out = np.zeros(1, dtype=sim_specs["out"])
     calc_dir = sim_specs["user"]["calc_dir"]
     out["f"] = calc_in["x"]
     with open(calc_dir + "/test_sim_out.txt", "a") as f:
-        f.write("sim_f received: {}\n".format(out["f"]))
+        f.write(f"sim_f received: {out['f']}\n")
     return out, persis_info
 
 
 def remote_write_gen_func(calc_in, persis_info, gen_specs, libE_info):
     import socket
     import secrets
     import numpy as np
 
     H_o = np.zeros(1, dtype=gen_specs["out"])
     H_o["x"] = socket.gethostname() + "_" + secrets.token_hex(nbytes=3)
     with open("test_gen_out.txt", "a") as f:
-        f.write("gen_f produced: {}\n".format(H_o["x"]))
+        f.write(f"gen_f produced: {H_o['x']}\n")
     return H_o, persis_info
 
 
 def write_uniform_gen_func(H, persis_info, gen_specs, _):
     ub = gen_specs["user"]["ub"]
     lb = gen_specs["user"]["lb"]
     n = len(lb)
     b = gen_specs["user"]["gen_batch_size"]
     H_o = np.zeros(b, dtype=gen_specs["out"])
     H_o["x"] = persis_info["rand_stream"].uniform(lb, ub, (b, n))
     with open("test_gen_out.txt", "a") as f:
-        f.write("gen_f produced: {}\n".format(H_o["x"]))
+        f.write(f"gen_f produced: {H_o['x']}\n")
     return H_o, persis_info
 
 
 uniform_or_localopt_gen_out = [
     ("priority", float),
     ("local_pt", bool),
     ("known_to_aposmm", bool),
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_1d_sampling.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_1d_sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_1d_sampling_from_yaml.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_1d_sampling_from_yaml.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_1d_sampling_with_profile.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_1d_sampling_with_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,21 +56,21 @@
     if is_manager:
         assert len(H) >= 501
         print("\nlibEnsemble with random sampling has generated enough points")
 
         assert "manager.prof" in os.listdir(), "Expected manager profile not found after run"
         os.remove("manager.prof")
 
-        prof_files = ["worker_{}.prof".format(i + 1) for i in range(nworkers)]
+        prof_files = [f"worker_{i+1}.prof" for i in range(nworkers)]
 
         # Ensure profile writes complete before checking
         time.sleep(0.5)
 
         for file in prof_files:
-            assert file in os.listdir(), "Expected profile {} not found after run".format(file)
+            assert file in os.listdir(), "Expected profile {file} not found after run"
             with open(file, "r") as f:
                 data = f.read().split()
                 num_worker_funcs_profiled = sum(["worker" in i for i in data])
             assert num_worker_funcs_profiled >= 8, (
                 "Insufficient number of " + "worker functions profiled: " + str(num_worker_funcs_profiled)
             )
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_evaluate_existing_sample.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_evaluate_existing_sample.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_evaluate_mixed_sample.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_evaluate_mixed_sample.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_fast_alloc.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_fast_alloc.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_heffte.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_heffte.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_inverse_bayes_example.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_inverse_bayes_example.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_dfols.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_dfols.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 def combine_component(x):
     return np.sum(np.power(x, 2))
 
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_exception.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         assert passed
         print("\n\nException received as expected")
 
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_external_localopt.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_external_localopt.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 persistent generator.
 
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: local mpi tcp
 # TESTSUITE_NPROCS: 4
-# TESTSUITE_OS_SKIP: OSX
+# TESTSUITE_OS_SKIP: OSX WIN
 # TESTSUITE_EXTRA: true
 
 import sys
 import multiprocessing
 import numpy as np
 import shutil  # For copying the external_localopt script
 
@@ -42,15 +42,14 @@
 from time import time
 
 np.set_printoptions(precision=16)
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if is_manager:
         start_time = time()
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_nlopt.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_nlopt.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 the objective function will be 2, as one of the three workers will be the
 persistent generator.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: local mpi tcp
 # TESTSUITE_NPROCS: 3
-# TESTSUITE_EXTRA: true
 
 import sys
-import multiprocessing
 import numpy as np
 
 # Import libEnsemble items for this test
 from libensemble.libE import libE
 from math import gamma, pi, sqrt
 from libensemble.sim_funcs.six_hump_camel import six_hump_camel as sim_f
 
@@ -34,17 +32,14 @@
 from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
 from libensemble.tests.regression_tests.support import six_hump_camel_minima as minima
 from time import time
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
-    multiprocessing.set_start_method("fork", force=True)
-
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if is_manager:
         start_time = time()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_periodic.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_periodic.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from libensemble.sim_funcs.periodic_func import func_wrapper as sim_f
 from libensemble.alloc_funcs.persistent_aposmm_alloc import persistent_aposmm_alloc as alloc_f
 from libensemble.tools import parse_args, add_unique_random_streams
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_scipy.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_scipy.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
 from libensemble.tests.regression_tests.support import six_hump_camel_minima as minima
 from time import time
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if is_manager:
         start_time = time()
 
@@ -105,15 +104,15 @@
             min_found = 0
             for m in minima:
                 # The minima are known on this test problem.
                 # We use their values to test APOSMM has identified all minima
                 print(np.min(np.sum((H[H["local_min"]]["x"] - m) ** 2, 1)), flush=True)
                 if np.min(np.sum((H[H["local_min"]]["x"] - m) ** 2, 1)) < tol:
                     min_found += 1
-            assert min_found >= 4, "Found {} minima".format(min_found)
+            assert min_found >= 4, f"Found {min_found} minima"
 
             save_libE_output(H, persis_info, __file__, nworkers)
 
     # Now let's run on the same problem with a really large n (but we won't test
     # convergence to all local min). Note that sim_f uses only entries x[0:2]
     n = 400
     persis_info = add_unique_random_streams({}, nworkers + 1)
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_timeout.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_timeout.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 from libensemble.gen_funcs.persistent_aposmm import aposmm as gen_f
 from libensemble.alloc_funcs.persistent_aposmm_alloc import persistent_aposmm_alloc as alloc_f
 from libensemble.tools import parse_args, add_unique_random_streams, save_libE_output
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_with_grad.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_aposmm_with_grad.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
 from libensemble.tests.regression_tests.support import six_hump_camel_minima as minima
 from time import time
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if is_manager:
         start_time = time()
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_fd_param_finder.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_fd_param_finder.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_gp_multitask_ax.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_gp_multitask_ax.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,56 +22,59 @@
 import numpy as np
 from libensemble.libE import libE
 from libensemble import logger
 from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens
 from libensemble.tools import save_libE_output, add_unique_random_streams
 from libensemble.tools import parse_args
 from libensemble.message_numbers import WORKER_DONE
-from libensemble.gen_funcs.persistent_ax_multitask import persistent_gp_mt_ax_gen_f
 
 import warnings
 
+# Ax uses a deprecated warn command.
+warnings.filterwarnings("ignore", category=UserWarning)
+warnings.filterwarnings("ignore", category=DeprecationWarning)
+
+from libensemble.gen_funcs.persistent_ax_multitask import persistent_gp_mt_ax_gen_f
+
+
+def run_simulation(H, persis_info, sim_specs, libE_info):
+    # Extract input parameters
+    values = list(H["x"][0])
+    x0 = values[0]
+    x1 = values[1]
+    # Extract fidelity parameter
+    task = H["task"][0]
+    if task == "expensive_model":
+        z = 8
+    elif task == "cheap_model":
+        z = 1
+
+    libE_output = np.zeros(1, dtype=sim_specs["out"])
+    calc_status = WORKER_DONE
+
+    # Function that depends on the resolution parameter
+    libE_output["f"] = -(x0 + 10 * np.cos(x0 + 0.1 * z)) * (x1 + 5 * np.cos(x1 - 0.2 * z))
+
+    return libE_output, persis_info, calc_status
+
+
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Ax uses a deprecated warn command.
-    warnings.filterwarnings("ignore", category=UserWarning)
-    warnings.filterwarnings("ignore", category=DeprecationWarning)
-
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     mt_params = {
         "name_hifi": "expensive_model",
         "name_lofi": "cheap_model",
         "n_init_hifi": 4,
         "n_init_lofi": 4,
         "n_opt_hifi": 2,
         "n_opt_lofi": 4,
     }
 
-    def run_simulation(H, persis_info, sim_specs, libE_info):
-        # Extract input parameters
-        values = list(H["x"][0])
-        x0 = values[0]
-        x1 = values[1]
-        # Extract fidelity parameter
-        task = H["task"][0]
-        if task == "expensive_model":
-            z = 8
-        elif task == "cheap_model":
-            z = 1
-
-        libE_output = np.zeros(1, dtype=sim_specs["out"])
-        calc_status = WORKER_DONE
-
-        # Function that depends on the resolution parameter
-        libE_output["f"] = -(x0 + 10 * np.cos(x0 + 0.1 * z)) * (x1 + 5 * np.cos(x1 - 0.2 * z))
-
-        return libE_output, persis_info, calc_status
-
     sim_specs = {
         "sim_f": run_simulation,
         "in": ["x", "task"],
         "out": [("f", float)],
     }
 
     gen_specs = {
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_independent.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_independent.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_n_agent.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_n_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                 "rho": rho,
                 "N_const": N_const,  # multiplicative constant on numiters
                 "step_const": 1,
             }
         )
 
         if is_manager:
-            print("=== Optimizing {} ===".format(prob_name), flush=True)
+            print(f"=== Optimizing {prob_name} ===", flush=True)
 
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
         if is_manager:
             print("=== End algorithm ===", flush=True)
 
             # check we completed
@@ -232,8 +232,8 @@
 
             A_kron_I = spp.kron(A, spp.eye(n))
             consensus_val = np.dot(x, A_kron_I.dot(x))
 
             assert F - fstar < err_const * eps, "Error of {:.4e}, expected {:.4e} (assuming f*={:.4e})".format(
                 F - fstar, err_const * eps, fstar
             )
-            assert consensus_val < eps, "Consensus score of {:.4e}, expected {:.4e}\nx={}".format(consensus_val, eps, x)
+            assert consensus_val < eps, f"Consensus score of {consensus_val:.4e}, expected {eps:.4e}\nx={x}"
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_pds.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_pds.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                 "Vx_0x": n**0.5,  # Bregman divergence of x_0 and x_*
                 "eps": eps,  # error / tolerance
                 "A_norm": lam_max,  # ||A \otimes I||_2 = ||A||_2
             }
         )
 
         if is_manager:
-            print("=== Optimizing {} ===".format(prob_name), flush=True)
+            print(f"=== Optimizing {prob_name} ===", flush=True)
 
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
         if is_manager:
             print("=== End algorithm ===", flush=True)
 
             # check we completed
@@ -230,8 +230,8 @@
 
             A_kron_I = spp.kron(A, spp.eye(n))
             consensus_val = np.dot(x, A_kron_I.dot(x))
 
             assert F - fstar < err_const * eps, "Error of {:.4e}, expected {:.4e} (assuming f*={:.4e})".format(
                 F - fstar, err_const * eps, fstar
             )
-            assert consensus_val < eps, "Consensus score of {:.4e}, expected {:.4e}".format(consensus_val, eps)
+            assert consensus_val < eps, f"Consensus score of {consensus_val:.4e}, expected {eps:.4e}"
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_prox_slide.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_prox_slide.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
         # Include @f_i_eval and @df_i_eval if we want to compute gradient in gen
         persis_info["gen_params"].update(
             {"M": M, "R": 10**2, "nu": 1, "eps": eps, "D": 2 * n, "N_const": N_const, "lam_max": lam_max}
         )
 
         if is_manager:
-            print("=== Optimizing {} ===".format(prob_name), flush=True)
+            print(f"=== Optimizing {prob_name} ===", flush=True)
 
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
         if is_manager:
             print("=== End algorithm ===", flush=True)
 
             # check we completed
@@ -187,8 +187,8 @@
 
             A_kron_I = spp.kron(A, spp.eye(n))
             consensus_val = np.dot(x, A_kron_I.dot(x))
 
             assert F - fstar < err_const * eps, "Error of {:.4e}, expected {:.4e} (assuming f*={:.4e})".format(
                 F - fstar, err_const * eps, fstar
             )
-            assert consensus_val < eps, "Consensus score of {:.4e}, expected {:.4e}\nx={}".format(consensus_val, eps, x)
+            assert consensus_val < eps, f"Consensus score of {consensus_val:.4e}, expected {eps:.4e}\nx={x}"
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_sampling_CUDA_variable_resources.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_sampling_CUDA_variable_resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,20 @@
 from libensemble.executors.mpi_executor import MPIExecutor
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
-    libE_specs["zero_resource_workers"] = [1]
+    # The persistent gen does not need resources
+
+    libE_specs["num_resource_sets"] = nworkers - 1  # Any worker can be the gen
+
+    # libE_specs["zero_resource_workers"] = [1]  # If first worker must be gen, use this instead
+
     libE_specs["sim_dirs_make"] = True
     libE_specs["ensemble_dir_path"] = "./ensemble_CUDA_variable_w" + str(nworkers)
 
     if libE_specs["comms"] == "tcp":
         sys.exit("This test only runs with MPI or local -- aborting...")
 
     # Get paths for applications to run
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_sim_uniform_sampling.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_sim_uniform_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 the objective function will be 2, as one of the three workers will be the
 persistent generator.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: mpi local tcp
 # TESTSUITE_NPROCS: 3 4
+# TESTSUITE_OS_SKIP: WIN
 
 import sys
 import numpy as np
 
 # Import libEnsemble items for this test
 from libensemble.libE import libE
 from libensemble.sim_funcs.six_hump_camel import persistent_six_hump_camel as sim_f
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_surmise_calib.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_surmise_calib.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,11 +113,11 @@
         sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs=alloc_specs, libE_specs=libE_specs
     )
 
     if is_manager:
         print("Cancelled sims", H["sim_id"][H["cancel_requested"]])
         sims_done = np.count_nonzero(H["sim_ended"])
         save_libE_output(H, persis_info, __file__, nworkers)
-        assert sims_done == max_evals, "Num of completed simulations should be {}. Is {}".format(max_evals, sims_done)
+        assert sims_done == max_evals, f"Num of completed simulations should be {max_evals}. Is {sims_done}"
 
         # The following line is only to cover parts of tstd2theta
         tstd2theta(H[0]["thetas"].squeeze(), hard=False)
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_surmise_killsims.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_surmise_killsims.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,18 @@
 
     # Rename ensemble dir for non-inteference with other regression tests
     libE_specs["ensemble_dir_path"] = "ensemble_calib_kills"
 
     sim_specs = {
         "sim_f": sim_f,
         "in": ["x", "thetas"],
-        "out": [("f", float)],
+        "out": [
+            ("f", float),
+            ("sim_killed", bool),  # "sim_killed" is used only for display at the end of this test
+        ],
         "user": {
             "num_obs": n_x,
             "init_sample_size": init_sample_size,
         },
     }
 
     gen_out = [
@@ -126,11 +129,12 @@
     # Perform the run
     H, persis_info, flag = libE(
         sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs=alloc_specs, libE_specs=libE_specs
     )
 
     if is_manager:
         print("Cancelled sims", H["sim_id"][H["cancel_requested"]])
-        print("Killed sims", H["sim_id"][H["kill_sent"]])
+        print("Kills sent by manager to running simulations", H["sim_id"][H["kill_sent"]])
+        print("Killed sims", H["sim_id"][H["sim_killed"]])
         sims_done = np.count_nonzero(H["sim_ended"])
         save_libE_output(H, persis_info, __file__, nworkers)
-        assert sims_done == max_evals, "Num of completed simulations should be {}. Is {}".format(max_evals, sims_done)
+        assert sims_done == max_evals, f"Num of completed simulations should be {max_evals}. Is {sims_done}"
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_tasmanian.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_tasmanian.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             exit_criteria = {"gen_max": 100}  # This will test persistent_tasmanian stopping early.
 
         # tasmanian_init has to be a method that returns an initialized TasmanianSparseGrid object
         # tasmanian_checkpoint_file will be overwritten between each step of the iterative refinement
         #   the final grid will also be stored in the file
         gen_specs["user"] = {
             "tasmanian_init": tasmanian_init_global if run < 2 else tasmanian_init_localp,
-            "tasmanian_checkpoint_file": "tasmanian{0}.grid".format(run),
+            "tasmanian_checkpoint_file": f"tasmanian{run}.grid",
         }
 
         # setup the refinement criteria
         if run == 0:
             gen_specs["user"]["refinement"] = "none"
 
         if run == 1:
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_tasmanian_async.py` & `libensemble-0.9.3/examples/calling_scripts/regression_tests/test_persistent_tasmanian_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,13 +95,13 @@
         sim_specs, gen_specs, alloc_specs, persis_info = get_sparse_grid_specs(user_specs, sim_f, 2, mode="async")
 
         if run_num == 0:
             gen_specs["user"]["tasmanian_checkpoint_file"] = "tasmanian.grid"
             run_num += 1
 
         if is_manager:
-            print("[Manager]: user_specs = {0}".format(user_specs))
-            print("[Manager]: exit_criteria = {0}".format(exit_criteria))
+            print(f"[Manager]: user_specs = {user_specs}")
+            print(f"[Manager]: exit_criteria = {exit_criteria}")
             start_time = time()
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
         if is_manager:
             print("[Manager]: Time taken = ", time() - start_time, "\n", flush=True)
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_uniform_gen_decides_stop.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_gen_decides_stop.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 The number of concurrent evaluations of the objective function with 2 gens will be 2:
 5 - 1 manager - 2 persistent gens = 2.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: mpi local tcp
 # TESTSUITE_NPROCS: 5
+# TESTSUITE_OS_SKIP: WIN
 
 import sys
 import numpy as np
 
 # Import libEnsemble items for this test
 from libensemble.libE import libE
 from libensemble.sim_funcs.branin.branin_obj import call_branin as sim_f
@@ -84,12 +85,12 @@
         ), "The second gen_ended_time should be common among initial_batch_size number of points"
         assert (
             len(np.unique(counts)) > 1
         ), "All gen_ended_times are the same; they should be different for the async case"
 
         gen_workers = np.unique(H["gen_worker"])
         print("Generators that issued points", gen_workers)
-        assert len(gen_workers) == ngens, "The number of gens used {} does not match num_active_gens {}".format(
-            len(gen_workers), ngens
-        )
+        assert (
+            len(gen_workers) == ngens
+        ), f"The number of gens used {len(gen_workers)} does not match num_active_gens {ngens}"
 
         save_libE_output(H, persis_info, __file__, nworkers)
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_uniform_sampling.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_uniform_sampling_adv.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_adv.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_uniform_sampling_async.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_async.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_persistent_uniform_sampling_nonblocking.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_nonblocking.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_stats_output.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_stats_output.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_uniform_sampling.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_uniform_sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_uniform_sampling_cancel.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_uniform_sampling_cancel.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from libensemble.alloc_funcs.fast_alloc import give_sim_work_first as fast_gswf
 from libensemble.alloc_funcs.only_one_gen_alloc import ensure_one_active_gen
 from libensemble.alloc_funcs.give_pregenerated_work import give_pregenerated_sim_work
 
 
 def create_H0(persis_info, gen_specs, sim_max):
     """Create an H0 for give_pregenerated_sim_work"""
-
     # Manually creating H0
     ub = gen_specs["user"]["ub"]
     lb = gen_specs["user"]["lb"]
     n = len(lb)
     b = sim_max
 
     H0 = np.zeros(b, dtype=[("x", float, 2), ("sim_id", int), ("sim_started", bool), ("cancel_requested", bool)])
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_uniform_sampling_one_residual_at_a_time.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_uniform_sampling_one_residual_at_a_time.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_uniform_sampling_then_persistent_localopt_runs.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_uniform_sampling_then_persistent_localopt_runs.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/regression_tests/test_uniform_sampling_with_variable_resources.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 Note: This test contains multiple iterations to test different configurations.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: mpi local
 # TESTSUITE_NPROCS: 2 4
+# TESTSUITE_EXTRA: true
 
 import sys
 import numpy as np
 
 # Import libEnsemble items for this test
 from libensemble.libE import libE
 from libensemble.sim_funcs import helloworld, six_hump_camel
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/run_libe_forces.py` & `libensemble-0.9.3/examples/calling_scripts/run_libe_forces.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 sim_app = os.path.join(os.getcwd(), "../forces_app/forces.x")
 
 if not os.path.isfile(sim_app):
     sys.exit("forces.x not found - please build first in ../forces_app dir")
 
 if is_manager:
-    print("\nRunning with {} workers\n".format(nworkers))
+    print(f"\nRunning with {nworkers} workers\n")
 
 
 # Create executor and register sim to it.
 if USE_BALSAM:
     from libensemble.executors.legacy_balsam_executor import LegacyBalsamMPIExecutor
 
     exctr = LegacyBalsamMPIExecutor()
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/run_libe_forces_from_yaml.py` & `libensemble-0.9.3/examples/calling_scripts/run_libe_forces_from_yaml.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 forces = Ensemble()
 forces.from_yaml("forces.yaml")
 
 forces.logger.set_level("INFO")
 
 if forces.is_manager:
-    print("\nRunning with {} workers\n".format(forces.nworkers))
+    print(f"\nRunning with {forces.nworkers} workers\n")
 
 exctr = MPIExecutor()
 exctr.register_app(full_path=sim_app, app_name="forces")
 
 forces.libE_specs["ensemble_dir_path"] = "./ensemble"
 forces.gen_specs["user"].update(
     {
```

### Comparing `libensemble-0.9.2/examples/calling_scripts/run_libensemble_on_warpx.py` & `libensemble-0.9.3/examples/calling_scripts/run_libensemble_on_warpx.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/calling_scripts/tutorial_calling.py` & `libensemble-0.9.3/examples/calling_scripts/tutorial_calling.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,14 @@
 
 colors = ["b", "g", "r", "y", "m", "c", "k", "w"]
 
 for i in range(1, nworkers + 1):
     worker_xy = np.extract(H["sim_worker"] == i, H)
     x = [entry.tolist()[0] for entry in worker_xy["x"]]
     y = [entry for entry in worker_xy["y"]]
-    plt.scatter(x, y, label="Worker {}".format(i), c=colors[i - 1])
+    plt.scatter(x, y, label=f"Worker {i}", c=colors[i - 1])
 
 plt.title("Sine calculations for a uniformly sampled random distribution")
 plt.xlabel("x")
 plt.ylabel("sine(x)")
 plt.legend(loc="lower right")
 plt.savefig("tutorial_sines.png")
```

### Comparing `libensemble-0.9.2/examples/gen_funcs/persistent_sampling.py` & `libensemble-0.9.3/examples/gen_funcs/persistent_sampling.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from libensemble.message_numbers import STOP_TAG, PERSIS_STOP, FINISHED_PERSISTENT_GEN_TAG, EVAL_GEN_TAG
 from libensemble.tools.persistent_support import PersistentSupport
 
 __all__ = [
     "persistent_uniform",
     "uniform_random_sample_with_variable_resources",
     "persistent_request_shutdown",
+    "uniform_nonblocking",
     "batched_history_matching",
+    "persistent_uniform_with_cancellations",
 ]
 
 
 def persistent_uniform(H, persis_info, gen_specs, libE_info):
     """
     This generation function always enters into persistent mode and returns
     ``gen_specs['initial_batch_size']`` uniformly sampled points the first time it
@@ -75,15 +77,15 @@
     tag, Work, calc_in = ps.send_recv(H_o)
     while tag not in [STOP_TAG, PERSIS_STOP]:
         H_o = np.zeros(b, dtype=gen_specs["out"])
         # H_o['x'] = len(H)*np.ones(n)
         H_o["x"] = persis_info["rand_stream"].uniform(lb, ub, (b, n))
         H_o["resource_sets"] = persis_info["rand_stream"].integers(1, gen_specs["user"]["max_resource_sets"] + 1, b)
         H_o["priority"] = 10 * H_o["resource_sets"]
-        print("Created {} sims, with worker_teams req. of size(s) {}".format(b, H_o["resource_sets"]), flush=True)
+        print(f"Created {b} sims, with worker_teams req. of size(s) {H_o['resource_sets']}", flush=True)
         tag, Work, calc_in = ps.send_recv(H_o)
 
         if calc_in is not None:
             b = len(calc_in)
 
     return H_o, persis_info, FINISHED_PERSISTENT_GEN_TAG
 
@@ -200,7 +202,38 @@
         if calc_in is not None:
             all_inds = np.argsort(calc_in["f"])
             best_inds = all_inds[:q]
             mu = np.mean(H_o["x"][best_inds], axis=0)
             Sigma = np.cov(H_o["x"][best_inds].T)
 
     return H_o, persis_info, FINISHED_PERSISTENT_GEN_TAG
+
+
+def persistent_uniform_with_cancellations(H, persis_info, gen_specs, libE_info):
+
+    ub = gen_specs["user"]["ub"]
+    lb = gen_specs["user"]["lb"]
+    n = len(lb)
+    b = gen_specs["user"]["initial_batch_size"]
+
+    # Start cancelling points from half initial batch onward
+    cancel_from = b // 2  # Should get at least this many points back
+
+    ps = PersistentSupport(libE_info, EVAL_GEN_TAG)
+
+    # Send batches until manager sends stop tag
+    tag = None
+    while tag not in [STOP_TAG, PERSIS_STOP]:
+
+        H_o = np.zeros(b, dtype=gen_specs["out"])
+        H_o["x"] = persis_info["rand_stream"].uniform(lb, ub, (b, n))
+        tag, Work, calc_in = ps.send_recv(H_o)
+
+        if hasattr(calc_in, "__len__"):
+            b = len(calc_in)
+
+            # Cancel as many points as got back
+            cancel_ids = list(range(cancel_from, cancel_from + b))
+            cancel_from += b
+            ps.request_cancel_sim_ids(cancel_ids)
+
+    return H_o, persis_info, FINISHED_PERSISTENT_GEN_TAG
```

### Comparing `libensemble-0.9.2/examples/gen_funcs/sampling.py` & `libensemble-0.9.3/examples/gen_funcs/sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/gen_funcs/uniform_or_localopt.py` & `libensemble-0.9.3/examples/gen_funcs/uniform_or_localopt.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/libE_submission_scripts/bebop_submit_slurm_central.sh` & `libensemble-0.9.3/examples/libE_submission_scripts/bebop_submit_slurm_central.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/libE_submission_scripts/bebop_submit_slurm_distrib.sh` & `libensemble-0.9.3/examples/libE_submission_scripts/bebop_submit_slurm_distrib.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/libE_submission_scripts/blues_script.pbs` & `libensemble-0.9.3/examples/libE_submission_scripts/blues_script.pbs`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/libE_submission_scripts/bridges_submit_slurm_central.sh` & `libensemble-0.9.3/examples/libE_submission_scripts/bridges_submit_slurm_central.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/libE_submission_scripts/cori_submit.sh` & `libensemble-0.9.3/examples/libE_submission_scripts/cori_submit.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/libE_submission_scripts/edtb_submit_pbspro_central.sh` & `libensemble-0.9.3/examples/libE_submission_scripts/edtb_submit_pbspro_central.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/libE_submission_scripts/summit_submit_mproc.sh` & `libensemble-0.9.3/examples/libE_submission_scripts/summit_submit_mproc.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/libE_submission_scripts/theta_submit_balsam.sh` & `libensemble-0.9.3/examples/libE_submission_scripts/theta_submit_balsam.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/libE_submission_scripts/theta_submit_mproc.sh` & `libensemble-0.9.3/examples/libE_submission_scripts/theta_submit_mproc.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/misc/ps_nodes.sh` & `libensemble-0.9.3/examples/misc/ps_nodes.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/sim_funcs/branin/branin.py` & `libensemble-0.9.3/examples/sim_funcs/branin/branin.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/sim_funcs/branin/branin_obj.py` & `libensemble-0.9.3/examples/sim_funcs/branin/branin_obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import numpy as np
 import time
 from libensemble.sim_funcs.branin.branin import branin
 
 
 def call_branin(H, persis_info, sim_specs, _):
     """Evaluates the Branin function"""
-
     batch = len(H["x"])
 
     H_o = np.zeros(batch, dtype=sim_specs["out"])
 
     for i, x in enumerate(H["x"]):
         # Uncomment the following if you want to use the file system to do evaluations
         # devnull = open(os.devnull, 'w')
```

### Comparing `libensemble-0.9.2/examples/sim_funcs/chwirut1.py` & `libensemble-0.9.3/examples/sim_funcs/chwirut1.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/sim_funcs/executor_hworld.py` & `libensemble-0.9.3/examples/sim_funcs/executor_hworld.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,162 +20,165 @@
     import time
 
     calc_status = UNSET_TAG  # Sim func determines status of libensemble calc - returned to worker
 
     while task.runtime < timeout_sec:
         time.sleep(delay)
 
-        exctr.manager_poll()
-        if exctr.manager_signal == "finish":
+        if exctr.manager_kill_received():
             exctr.kill(task)
             calc_status = MAN_SIGNAL_FINISH  # Worker will pick this up and close down
-            print("Task {} killed by manager on worker {}".format(task.id, exctr.workerID))
+            print(f"Task {task.id} killed by manager on worker {exctr.workerID}")
             break
 
         task.poll()
         if task.finished:
             break
         elif task.state == "RUNNING":
-            print("Task {} still running on worker {} ....".format(task.id, exctr.workerID))
+            print(f"Task {task.id} still running on worker {exctr.workerID} ....")
 
         if task.stdout_exists():
             if "Error" in task.read_stdout():
                 print(
-                    "Found (deliberate) Error in output file - cancelling "
-                    "task {} on worker {}".format(task.id, exctr.workerID)
+                    "Found (deliberate) Error in output file - cancelling " f"task {task.id} on worker {exctr.workerID}"
                 )
                 exctr.kill(task)
                 calc_status = WORKER_KILL_ON_ERR
                 break
 
     # After exiting loop
     if task.finished:
-        print("Task {} done on worker {}".format(task.id, exctr.workerID))
+        print(f"Task {task.id} done on worker {exctr.workerID}")
         # Fill in calc_status if not already
         if calc_status == UNSET_TAG:
             if task.state == "FINISHED":  # Means finished successfully
                 calc_status = WORKER_DONE
             elif task.state == "FAILED":
                 calc_status = TASK_FAILED
 
     else:
         # assert task.state == 'RUNNING', "task.state expected to be RUNNING. Returned: " + str(task.state)
-        print("Task {} timed out - killing on worker {}".format(task.id, exctr.workerID))
+        print(f"Task {task.id} timed out - killing on worker {exctr.workerID}")
         exctr.kill(task)
         if task.finished:
-            print("Task {} done on worker {}".format(task.id, exctr.workerID))
+            print(f"Task {task.id} done on worker {exctr.workerID}")
         calc_status = WORKER_KILL_ON_TIMEOUT
 
     return task, calc_status
 
 
 def executor_hworld(H, persis_info, sim_specs, libE_info):
     """Tests launching and polling task and exiting on task finish"""
     exctr = MPIExecutor.executor
     cores = sim_specs["user"]["cores"]
     USE_BALSAM = "balsam_test" in sim_specs["user"]
     ELAPSED_TIMEOUT = "elapsed_timeout" in sim_specs["user"]
 
     wait = False
     args_for_sim = "sleep 1"
+    calc_status = UNSET_TAG
 
-    if ELAPSED_TIMEOUT:
-        args_for_sim = "sleep 60"  # Manager kill - if signal received else completes
-        timeout = 65.0
+    batch = len(H["x"])
+    H_o = np.zeros(batch, dtype=sim_specs["out"])
+
+    if "six_hump_camel" not in exctr.default_app("sim").full_path:
 
-    else:
         global sim_ended_count
         sim_ended_count += 1
-        timeout = 6.0
-        launch_shc = False
-        print(sim_ended_count)
-
-        if sim_ended_count == 1:
-            args_for_sim = "sleep 1"  # Should finish
-        elif sim_ended_count == 2:
-            args_for_sim = "sleep 1 Error"  # Worker kill on error
-        elif sim_ended_count == 3:
-            wait = True
-            args_for_sim = "sleep 1"  # Should finish
-            launch_shc = True
-        elif sim_ended_count == 4:
-            args_for_sim = "sleep 8"  # Worker kill on timeout
-            timeout = 1.0
-        elif sim_ended_count == 5:
-            args_for_sim = "sleep 2 Fail"  # Manager kill - if signal received else completes
-
-    if USE_BALSAM:
-        task = exctr.submit(
-            calc_type="sim",
-            num_procs=cores,
-            app_args=args_for_sim,
-            hyperthreads=True,
-            machinefile="notused",
-            stdout="notused",
-            wait_on_start=True,
-        )
-    else:
-        task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim, hyperthreads=True)
+        print("sim_ended_count", sim_ended_count, flush=True)
 
-    if wait:
-        task.wait()
-        if not task.finished:
-            calc_status = UNSET_TAG
-        if task.state == "FINISHED":
-            calc_status = WORKER_DONE
-        elif task.state == "FAILED":
-            calc_status = TASK_FAILED
+        if ELAPSED_TIMEOUT:
+            args_for_sim = "sleep 60"  # Manager kill - if signal received else completes
+            timeout = 65.0
 
-    else:
-        if not ELAPSED_TIMEOUT:
+        else:
+            timeout = 6.0
+            launch_shc = False
+
+            if sim_ended_count == 1:
+                args_for_sim = "sleep 1"  # Should finish
+            elif sim_ended_count == 2:
+                args_for_sim = "sleep 1 Error"  # Worker kill on error
+            elif sim_ended_count == 3:
+                wait = True
+                args_for_sim = "sleep 1"  # Should finish
+                launch_shc = True
+            elif sim_ended_count == 4:
+                args_for_sim = "sleep 8"  # Worker kill on timeout
+                timeout = 1.0
+            elif sim_ended_count == 5:
+                args_for_sim = "sleep 2 Fail"  # Manager kill - if signal received else completes
+
+        if USE_BALSAM:
+            task = exctr.submit(
+                calc_type="sim",
+                num_procs=cores,
+                app_args=args_for_sim,
+                hyperthreads=True,
+                machinefile="notused",
+                stdout="notused",
+                wait_on_start=True,
+            )
+        else:
+            task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim, hyperthreads=True)
+
+        if wait:
+            task.wait()
+            if not task.finished:
+                calc_status = UNSET_TAG
+            if task.state == "FINISHED":
+                calc_status = WORKER_DONE
+            elif task.state == "FAILED":
+                calc_status = TASK_FAILED
+
+        else:
             if sim_ended_count >= 2 and not USE_BALSAM:
                 calc_status = exctr.polling_loop(task, timeout=timeout, delay=0.3, poll_manager=True)
                 if sim_ended_count == 2 and task.stdout_exists() and "Error" in task.read_stdout():
                     calc_status = WORKER_KILL_ON_ERR
-
             else:
                 task, calc_status = custom_polling_loop(exctr, task, timeout)
 
-        else:
-            calc_status = exctr.polling_loop(task, timeout=timeout, delay=0.3, poll_manager=True)
+        if USE_BALSAM:
+            task.read_file_in_workdir("ensemble.log")
+            try:
+                task.read_stderr()
+            except ValueError:
+                pass
+
+            task = exctr.submit(
+                app_name="sim_hump_camel_dry_run",
+                num_procs=cores,
+                app_args=args_for_sim,
+                hyperthreads=True,
+                machinefile="notused",
+                stdout="notused",
+                wait_on_start=True,
+                dry_run=True,
+                stage_inout=os.getcwd(),
+            )
 
-    if USE_BALSAM:
-        task.read_file_in_workdir("ensemble.log")
-        try:
-            task.read_stderr()
-        except ValueError:
-            pass
-
-        task = exctr.submit(
-            app_name="sim_hump_camel_dry_run",
-            num_procs=cores,
-            app_args=args_for_sim,
-            hyperthreads=True,
-            machinefile="notused",
-            stdout="notused",
-            wait_on_start=True,
-            dry_run=True,
-            stage_inout=os.getcwd(),
-        )
+            task.poll()
+            task.wait()
 
-        task.poll()
-        task.wait()
+    else:
+        launch_shc = True
+        calc_status = UNSET_TAG
 
-    # This is temp - return something - so doing six_hump_camel_func again...
-    batch = len(H["x"])
-    H_o = np.zeros(batch, dtype=sim_specs["out"])
-    for i, x in enumerate(H["x"]):
-        H_o["f"][i] = six_hump_camel_func(x)
-        if launch_shc:
-            # Test launching a named app.
-            app_args = " ".join(str(val) for val in list(x[:]))
-            task = exctr.submit(app_name="six_hump_camel", num_procs=1, app_args=app_args)
-            task.wait()
-            output = np.float64(task.read_stdout())
-            assert np.isclose(H_o["f"][i], output)
+        # Comparing six_hump_camel output, directly called vs. submitted as app
+        for i, x in enumerate(H["x"]):
+            H_o["f"][i] = six_hump_camel_func(x)
+            if launch_shc:
+                # Test launching a named app.
+                app_args = " ".join(str(val) for val in list(x[:]))
+                task = exctr.submit(app_name="six_hump_camel", num_procs=1, app_args=app_args)
+                task.wait()
+                output = np.float64(task.read_stdout())
+                assert np.isclose(H_o["f"][i], output)
+                calc_status = WORKER_DONE
 
     # This is just for testing at calling script level - status of each task
     H_o["cstat"] = calc_status
 
     return H_o, persis_info, calc_status
```

### Comparing `libensemble-0.9.2/examples/sim_funcs/six_hump_camel.py` & `libensemble-0.9.3/examples/sim_funcs/six_hump_camel.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,26 +138,23 @@
     x = H["x"][0]
     H_o = np.zeros(1, dtype=sim_specs["out"])
 
     # Interrogate resources available to this worker
     resources = Resources.resources.worker_resources
     slots = resources.slots
 
-    assert resources.matching_slots, "Error: Cannot set CUDA_VISIBLE_DEVICES when unmatching slots on nodes {}".format(
-        slots
-    )
+    assert resources.matching_slots, f"Error: Cannot set CUDA_VISIBLE_DEVICES when unmatching slots on nodes {slots}"
 
     resources.set_env_to_slots("CUDA_VISIBLE_DEVICES")
     num_nodes = resources.local_node_count
     cores_per_node = resources.slot_count  # One CPU per GPU
 
     print(
-        "Worker {}: CUDA_VISIBLE_DEVICES={}  \tnodes {} ppn {}  slots {}".format(
-            libE_info["workerID"], os.environ["CUDA_VISIBLE_DEVICES"], num_nodes, cores_per_node, slots
-        )
+        f"Worker {libE_info['workerID']}: CUDA_VISIBLE_DEVICES={os.environ['CUDA_VISIBLE_DEVICES']}"
+        f"\tnodes {num_nodes} ppn {cores_per_node}  slots {slots}"
     )
 
     # Create application input file
     inpt = " ".join(map(str, x))
     exctr = Executor.executor  # Get Executor
 
     # Launch application via system MPI runner, using assigned resources.
```

### Comparing `libensemble-0.9.2/examples/tutorials/aposmm/aposmm_tutorial_notebook.ipynb` & `libensemble-0.9.3/examples/tutorials/aposmm/aposmm_tutorial_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/tutorials/aposmm/tutorial_aposmm.py` & `libensemble-0.9.3/examples/tutorials/aposmm/tutorial_aposmm.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/tutorials/aposmm/tutorial_six_hump_camel.py` & `libensemble-0.9.3/examples/tutorials/aposmm/tutorial_six_hump_camel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 
 
 def six_hump_camel(H, persis_info, sim_specs, _):
     """Six-Hump Camel sim_f."""
-
     batch = len(H["x"])  # Num evaluations each sim_f call.
     H_o = np.zeros(batch, dtype=sim_specs["out"])  # Define output array H
 
     for i, x in enumerate(H["x"]):
         H_o["f"][i] = six_hump_camel_func(x)  # Function evaluations placed into H
 
     return H_o, persis_info
```

### Comparing `libensemble-0.9.2/examples/tutorials/forces_with_executor/build_forces.sh` & `libensemble-0.9.3/examples/tutorials/forces_with_executor/build_forces.sh`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 # Building with OpenMP for target device (e.g. GPU)
 # Need to toggle to OpenMP target directive in forces.c.
 
 # xl
 # xlc_r -O3 -qsmp=omp -qoffload -o forces.x forces.c
 
 # Nvidia (nvc) compiler with mpicc and on Cray system with target (Perlmutter)
-# mpicc -O3 -fopenmp -mp=gpu -o forces_gpu.x forces_gpu.c
+# mpicc -O3 -fopenmp -mp=gpu -o forces.x forces.c
 # cc -O3 -fopenmp -mp=gpu -target-accel=nvidia80 -o forces.x forces.c
 
 # Spock/Crusher (AMD ROCm compiler)
 # cc -I${ROCM_PATH}/include -L${ROCM_PATH}/lib -lamdhip64 -fopenmp -O3 -o forces.x forces.c
 
 # Intel oneAPI (Clang based) Compiler (JIT compiled for device)
 # mpiicx -O3 -fiopenmp -fopenmp-targets=spir64 -o forces.x forces.c
```

### Comparing `libensemble-0.9.2/examples/tutorials/forces_with_executor/forces.c` & `libensemble-0.9.3/examples/tutorials/forces_with_executor/forces.c`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/tutorials/forces_with_executor/forces_simf.py` & `libensemble-0.9.3/examples/tutorials/forces_with_executor/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/tutorials/forces_with_executor/forces_tutorial_notebook.ipynb` & `libensemble-0.9.3/examples/tutorials/forces_with_executor/forces_tutorial_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/tutorials/forces_with_executor/run_libe_forces.py` & `libensemble-0.9.3/examples/tutorials/forces_with_executor/run_libe_forces.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,51 +5,53 @@
 from forces_simf import run_forces  # Sim func from current dir
 
 from libensemble.libE import libE
 from libensemble.gen_funcs.sampling import uniform_random_sample
 from libensemble.tools import parse_args, add_unique_random_streams
 from libensemble.executors import MPIExecutor
 
-# Parse number of workers, comms type, etc. from arguments
-nworkers, is_manager, libE_specs, _ = parse_args()
+if __name__ == "__main__":
 
-# Initialize MPI Executor instance
-exctr = MPIExecutor()
+    # Parse number of workers, comms type, etc. from arguments
+    nworkers, is_manager, libE_specs, _ = parse_args()
 
-# Register simulation executable with executor
-sim_app = os.path.join(os.getcwd(), "../forces_app/forces.x")
+    # Initialize MPI Executor instance
+    exctr = MPIExecutor()
 
-if not os.path.isfile(sim_app):
-    sys.exit("forces.x not found - please build first in ../forces_app dir")
-
-exctr.register_app(full_path=sim_app, app_name="forces")
-
-# State the sim_f, inputs, outputs
-sim_specs = {
-    "sim_f": run_forces,  # sim_f, imported above
-    "in": ["x"],  # Name of input for sim_f
-    "out": [("energy", float)],  # Name, type of output from sim_f
-}
-
-# State the gen_f, inputs, outputs, additional parameters
-gen_specs = {
-    "gen_f": uniform_random_sample,  # Generator function
-    "in": [],  # Generator input
-    "out": [("x", float, (1,))],  # Name, type and size of data from gen_f
-    "user": {
-        "lb": np.array([1000]),  # User parameters for the gen_f
-        "ub": np.array([3000]),
-        "gen_batch_size": 8,
-    },
-}
-
-# Create and work inside separate per-simulation directories
-libE_specs["sim_dirs_make"] = True
+    # Register simulation executable with executor
+    sim_app = os.path.join(os.getcwd(), "../forces_app/forces.x")
+
+    if not os.path.isfile(sim_app):
+        sys.exit("forces.x not found - please build first in ../forces_app dir")
+
+    exctr.register_app(full_path=sim_app, app_name="forces")
+
+    # State the sim_f, inputs, outputs
+    sim_specs = {
+        "sim_f": run_forces,  # sim_f, imported above
+        "in": ["x"],  # Name of input for sim_f
+        "out": [("energy", float)],  # Name, type of output from sim_f
+    }
+
+    # State the gen_f, inputs, outputs, additional parameters
+    gen_specs = {
+        "gen_f": uniform_random_sample,  # Generator function
+        "in": [],  # Generator input
+        "out": [("x", float, (1,))],  # Name, type and size of data from gen_f
+        "user": {
+            "lb": np.array([1000]),  # User parameters for the gen_f
+            "ub": np.array([3000]),
+            "gen_batch_size": 8,
+        },
+    }
+
+    # Create and work inside separate per-simulation directories
+    libE_specs["sim_dirs_make"] = True
 
-# Instruct libEnsemble to exit after this many simulations
-exit_criteria = {"sim_max": 8}
+    # Instruct libEnsemble to exit after this many simulations
+    exit_criteria = {"sim_max": 8}
 
-# Seed random streams for each worker, particularly for gen_f
-persis_info = add_unique_random_streams({}, nworkers + 1)
+    # Seed random streams for each worker, particularly for gen_f
+    persis_info = add_unique_random_streams({}, nworkers + 1)
 
-# Launch libEnsemble
-H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info=persis_info, libE_specs=libE_specs)
+    # Launch libEnsemble
+    H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info=persis_info, libE_specs=libE_specs)
```

### Comparing `libensemble-0.9.2/examples/tutorials/images/basic_6hc.png` & `libensemble-0.9.3/examples/tutorials/images/basic_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/tutorials/images/localopt_6hc.png` & `libensemble-0.9.3/examples/tutorials/images/localopt_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/tutorials/images/sampling_6hc.png` & `libensemble-0.9.3/examples/tutorials/images/sampling_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/tutorials/simple_sine/sine_tutorial_notebook.ipynb` & `libensemble-0.9.3/examples/tutorials/simple_sine/sine_tutorial_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/examples/tutorials/simple_sine/tutorial_calling.py` & `libensemble-0.9.3/examples/tutorials/simple_sine/tutorial_calling.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,14 @@
 
 colors = ["b", "g", "r", "y", "m", "c", "k", "w"]
 
 for i in range(1, nworkers + 1):
     worker_xy = np.extract(H["sim_worker"] == i, H)
     x = [entry.tolist()[0] for entry in worker_xy["x"]]
     y = [entry for entry in worker_xy["y"]]
-    plt.scatter(x, y, label="Worker {}".format(i), c=colors[i - 1])
+    plt.scatter(x, y, label=f"Worker {i}", c=colors[i - 1])
 
 plt.title("Sine calculations for a uniformly sampled random distribution")
 plt.xlabel("x")
 plt.ylabel("sine(x)")
 plt.legend(loc="lower right")
 plt.savefig("tutorial_sines.png")
```

### Comparing `libensemble-0.9.2/examples/tutorials/simple_sine/tutorial_calling_mpi.py` & `libensemble-0.9.3/examples/tutorials/simple_sine/tutorial_calling_mpi.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,14 @@
 
     colors = ["b", "g", "r", "y", "m", "c", "k", "w"]
 
     for i in range(1, nworkers + 1):
         worker_xy = np.extract(H["sim_worker"] == i, H)
         x = [entry.tolist()[0] for entry in worker_xy["x"]]
         y = [entry for entry in worker_xy["y"]]
-        plt.scatter(x, y, label="Worker {}".format(i), c=colors[i - 1])
+        plt.scatter(x, y, label=f"Worker {i}", c=colors[i - 1])
 
     plt.title("Sine calculations for a uniformly sampled random distribution")
     plt.xlabel("x")
     plt.ylabel("sine(x)")
     plt.legend(loc="lower right")
     plt.savefig("tutorial_sines.png")
```

### Comparing `libensemble-0.9.2/examples/tutorials/simple_sine/tutorial_gen.py` & `libensemble-0.9.3/examples/tutorials/simple_sine/tutorial_gen.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/install/configure_balsam_install.py` & `libensemble-0.9.3/install/configure_balsam_install.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/install/find_mpi.py` & `libensemble-0.9.3/install/find_mpi.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/fast_alloc.py` & `libensemble-0.9.3/libensemble/alloc_funcs/fast_alloc.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/fast_alloc_and_pausing.py` & `libensemble-0.9.3/libensemble/alloc_funcs/fast_alloc_and_pausing.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/fast_alloc_to_aposmm.py` & `libensemble-0.9.3/libensemble/alloc_funcs/fast_alloc_to_aposmm.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/give_pregenerated_work.py` & `libensemble-0.9.3/libensemble/alloc_funcs/give_pregenerated_work.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/give_sim_work_first.py` & `libensemble-0.9.3/libensemble/alloc_funcs/give_sim_work_first.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/inverse_bayes_allocf.py` & `libensemble-0.9.3/libensemble/alloc_funcs/inverse_bayes_allocf.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/only_one_gen_alloc.py` & `libensemble-0.9.3/libensemble/alloc_funcs/only_one_gen_alloc.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/persistent_aposmm_alloc.py` & `libensemble-0.9.3/libensemble/alloc_funcs/persistent_aposmm_alloc.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/start_fd_persistent.py` & `libensemble-0.9.3/libensemble/alloc_funcs/start_fd_persistent.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/start_only_persistent.py` & `libensemble-0.9.3/libensemble/alloc_funcs/start_only_persistent.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/start_persistent_consensus.py` & `libensemble-0.9.3/libensemble/alloc_funcs/start_persistent_consensus.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,17 +129,17 @@
 
             # did gen sent consensus? (start @last_H_len to avoid old work)
             consensus_sim_ids = np.where(
                 np.logical_and(H[last_H_len:]["consensus_pt"], H[last_H_len:]["gen_worker"] == wid)
             )[0]
 
             if len(consensus_sim_ids) > 0:
-                assert (
-                    len(consensus_sim_ids) == 1
-                ), "Gen should only send one " + "point for consensus step, received {}".format(len(consensus_sim_ids))
+                assert len(consensus_sim_ids) == 1, (
+                    "Gen should only send one " + f"point for consensus step, received {len(consensus_sim_ids)}"
+                )
 
                 # re-center (since the last_H_len has relative index 0)
                 sim_id = consensus_sim_ids[0] + last_H_len
 
                 persis_info[wid].update({"curr_H_ids": [sim_id, sim_id + 1]})
                 persis_info[wid].update({"at_consensus": True})
 
@@ -164,17 +164,15 @@
                 persis_info[wid].update({"curr_H_ids": [l_H_id, r_H_id]})
 
     # If all gens at consensus, distribute data to all gens
     if num_gens_at_consensus == user["num_gens"]:
 
         assert num_gens_at_consensus == len(
             avail_persis_worker_ids
-        ), "All gens must be available, only {}/{} are though...".format(
-            len(avail_persis_worker_ids), len(num_gens_at_consensus)
-        )
+        ), f"All gens must be available, only {len(avail_persis_worker_ids)}/{len(num_gens_at_consensus)} are though..."
 
         # get index in history array @H where each gen's consensus point lies
         consensus_ids_in_H = np.array([persis_info[i]["curr_H_ids"][0] for i in avail_persis_worker_ids], dtype=int)
 
         # Setup for printing progress
         print_progress = persis_info.get("print_progress", False)
         print_obj = H[consensus_ids_in_H[0]]["eval_pt"]
@@ -222,20 +220,20 @@
                 persistent=True,
             )
 
             persis_info[wid].update({"curr_H_ids": []})
             persis_info[wid].update({"at_consensus": False})
 
         if print_obj and print_progress:
-            msg = "F(x)={:.8f}\n".format(fsum)
-            print("{}con={:.4e}".format(msg, np.dot(x, Ax)), flush=True)
+            msg = f"F(x)={fsum:.8f}\n"
+            print(f"{msg}con={np.dot(x, Ax):.4e}", flush=True)
         elif print_obj:
-            print("F(x)={:.8f}".format(fsum), flush=True)
+            print(f"F(x)={fsum:.8f}", flush=True)
         elif print_progress:
-            print("con={:.4e}".format(np.dot(x, Ax)), flush=True)
+            print(f"con={np.dot(x, Ax):.4e}", flush=True)
 
     # partition sum of convex functions evenly (only do at beginning)
     if is_first_iter and len(support.avail_worker_ids(persistent=False)):
         num_funcs = user["m"]
         num_gens = user["num_gens"]
         num_funcs_arr = partition_funcs_arr(num_funcs, num_gens)
 
@@ -304,17 +302,15 @@
                     break
 
             gen_id = H[persis_info["next_to_give"]]["gen_worker"]
             [l_H_ids, r_H_ids] = persis_info[gen_id]["curr_H_ids"]
 
             assert (
                 l_H_ids == persis_info["next_to_give"]
-            ), "@next_to_give={} does not match gen's requested work H id of {}".format(
-                persis_info["next_to_give"], l_H_ids
-            )
+            ), f"@next_to_give={persis_info['next_to_give']} does not match gen's requested work H id of {l_H_ids}"
 
             persis_info[wid].update({"params": persis_info.get("sim_params", {})})
 
             Work[wid] = support.sim_work(
                 wid, H, sim_specs["in"], np.arange(l_H_ids, r_H_ids), persis_info.get(wid), rset_team=rset_team
             )
```

### Comparing `libensemble-0.9.2/libensemble/alloc_funcs/start_persistent_local_opt_gens.py` & `libensemble-0.9.3/libensemble/alloc_funcs/start_persistent_local_opt_gens.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/api.py` & `libensemble-0.9.3/libensemble/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,28 +89,28 @@
         self._filename = inspect.stack()[1].filename
 
     def __str__(self):
         """
         Returns pretty-printed representation of Ensemble object. Depicts libEnsemble
         version, plus representations of major specification dicts.
         """
-        info = "\nlibEnsemble {}\n".format(__version__) + 79 * "*" + "\n"
+        info = f"\nlibEnsemble {__version__}\n" + 79 * "*" + "\n"
         info += "\nCalling Script: " + self._filename.split("/")[-1] + "\n"
 
         dicts = {
             "libE_specs": self.libE_specs,
             "sim_specs": self.sim_specs,
             "gen_specs": self.gen_specs,
             "alloc_specs": self.alloc_specs,
             "persis_info": self.persis_info.persis_info,
             "exit_criteria": self.exit_criteria,
         }
 
         for i in dicts:
-            info += "{}:\n {} \n\n".format(i, pprint.pformat(dicts[i]))
+            info += f"{i}:\n {pprint.pformat(dicts[i])} \n\n"
 
         info += 79 * "*"
         return info
 
     def run(self):
         """
         Initializes libEnsemble, passes in all specification dictionaries.
```

### Comparing `libensemble-0.9.2/libensemble/comms/comms.py` & `libensemble-0.9.3/libensemble/comms/comms.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,23 +340,23 @@
 
     def process_message(self, timeout=None):
         """Receive and process a message via the comm."""
         msg = self.comm.recv(timeout)
         msg_type = msg[0]
         args = msg[1:]
         try:
-            method = "on_{}".format(msg_type)
+            method = f"on_{msg_type}"
             handler = getattr(self, method)
         except AttributeError:
             return self.on_unhandled_message(msg)
         return handler(*args)
 
     def on_unhandled_message(self, msg):
         """Handle any messages for which there are no named handlers."""
-        raise ValueError("No handler available for message {0}{1}".format(msg[0], msg[1:]))
+        raise ValueError(f"No handler available for message {msg[0]}{msg[1:]}")
 
 
 class GenCommHandler(CommHandler):
     """Wrapper for handling messages at a persistent gen."""
 
     def send_request(self, recs):
         """Request new evaluations."""
```

### Comparing `libensemble-0.9.2/libensemble/comms/logs.py` & `libensemble-0.9.3/libensemble/comms/logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         self.worker_id = worker_id
 
         # Prefix used by stats logger
         if worker_id == 0:
             self.prefix = "Manager" + " " * (WorkerIDFilter.margin_align)
         else:
             worker_str = str(self.worker_id).rjust(WorkerIDFilter.margin_align, " ")
-            self.prefix = "Worker {}".format(worker_str)
+            self.prefix = f"Worker {worker_str}"
 
     def filter(self, record):
         """Add worker ID to a LogRecord"""
         record.worker = getattr(record, "worker", self.worker_id)
         record.prefix = getattr(record, "prefix", self.prefix)
         return True
 
@@ -116,15 +116,14 @@
     """Initialize a worker logger attributes"""
     logr.propagate = False
     logr.setLevel(lev)
 
 
 def worker_logging_config(comm, worker_id=None):
     """Add a comm handler with worker ID filter to the indicated logger."""
-
     logconfig = LogConfig.config
     logger = logging.getLogger(logconfig.name)
     slogger = logging.getLogger(logconfig.stats_name)
 
     ch = CommLogHandler(comm, pack=lambda rec: (0, rec))
     ch.addFilter(WorkerIDFilter(worker_id or comm.rank))
 
@@ -138,15 +137,14 @@
 
     logger.addHandler(ch)
     slogger.addHandler(ch)
 
 
 def manager_logging_config():
     """Add file-based logging at manager."""
-
     stat_timer = Timer()
     stat_timer.start()
 
     # Regular logging
     logconfig = LogConfig.config
 
     if not logconfig.logger_set:
@@ -177,18 +175,18 @@
         efilter = ErrorFilter(logconfig.stderr_level)
         fhe.addFilter(efilter)
         fhe.setFormatter(formatter)
         logger.addHandler(fhe)
     else:
         stat_logger = logging.getLogger(logconfig.stats_name)
 
-    stat_logger.info("Starting ensemble at: {}".format(stat_timer.date_start))
+    stat_logger.info(f"Starting ensemble at: {stat_timer.date_start}")
 
     def exit_logger():
         stat_timer.stop()
-        stat_logger.info("Exiting ensemble at: {} Time Taken: {}".format(stat_timer.date_end, stat_timer.elapsed))
+        stat_logger.info(f"Exiting ensemble at: {stat_timer.date_end} Time Taken: {stat_timer.elapsed}")
 
         # If closing logs - each libE() call will log to a new file.
         # fh.close()
         # fhs.close()
 
     return exit_logger
```

### Comparing `libensemble-0.9.2/libensemble/comms/mpi.py` & `libensemble-0.9.3/libensemble/comms/mpi.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/comms/tcp_mgr.py` & `libensemble-0.9.3/libensemble/comms/tcp_mgr.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,19 +43,19 @@
 
     def get_queue(self, name):
         """Get a queue from the shared manager"""
         return self.manager.get_queue(name)
 
     def get_inbox(self, workerID):
         """Get a worker inbox queue."""
-        return self.get_queue("inbox{}".format(workerID))
+        return self.get_queue(f"inbox{workerID}")
 
     def get_outbox(self, workerID):
         """Get a worker outbox queue."""
-        return self.get_queue("outbox{}".format(workerID))
+        return self.get_queue(f"outbox{workerID}")
 
     def get_shared(self):
         """Get a shared queue for worker subscription."""
         return self.get_queue("shared")
 
     def await_workers(self, nworkers):
         """Wait for a pool of workers to join."""
@@ -99,19 +99,19 @@
 
     def get_queue(self, name):
         """Get a queue from the server."""
         return self.manager.get_queue(name)
 
     def get_inbox(self):
         """Get this worker's inbox."""
-        return self.get_queue("inbox{}".format(self.workerID))
+        return self.get_queue(f"inbox{self.workerID}")
 
     def get_outbox(self):
         """Get this worker's outbox."""
-        return self.get_queue("outbox{}".format(self.workerID))
+        return self.get_queue(f"outbox{self.workerID}")
 
     def get_shared(self):
         """Get the shared queue for worker sign-up."""
         return self.get_queue("shared")
 
     def __enter__(self):
         """Enter the context."""
```

### Comparing `libensemble-0.9.2/libensemble/executors/balsam_executors/__init__.py` & `libensemble-0.9.3/libensemble/executors/balsam_executors/__init__.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/executors/balsam_executors/balsam_executor.py` & `libensemble-0.9.3/libensemble/executors/balsam_executors/balsam_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     :align: center
 
 At this time, access to Balsam is limited to those with valid organizational logins
 authenticated through Globus_.
 
 In order to initiate a Balsam executor, the calling script should contain ::
 
-    from libensemble.executors import BalsamExecutor
+    from libensemble.executors.balsam_executors import BalsamExecutor
     exctr = BalsamExecutor()
 
 Key differences to consider between this executor and libEnsemble's others is
 Balsam ``ApplicationDefinition`` instances are registered instead of paths and task
 submissions will not run until Balsam reserves compute resources at a site.
 
 This process may resemble::
 
-    from libensemble.executors import BalsamExecutor
+    from libensemble.executors.balsam_executors import BalsamExecutor
     from balsam.api import ApplicationDefinition
 
     class HelloApp(ApplicationDefinition):
         site = "my-balsam-site"
         command_template = "/path/to/hello.app {{ my_name }}"
 
     exctr = BalsamExecutor()
@@ -75,15 +75,14 @@
 
 from libensemble.executors.executor import (
     Application,
     Task,
     ExecutorException,
     TimeoutExpired,
     jassert,
-    STATES,
 )
 from libensemble.executors import Executor
 
 from balsam.api import Job, BatchJob, EventLog
 
 logger = logging.getLogger(__name__)
 # To change logging level for just this module
@@ -116,28 +115,26 @@
         executor on a submission.
         """
         # May want to override workdir with Balsam value when it exists
         Task.__init__(self, app, app_args, workdir, stdout, stderr, workerid)
 
     def _get_time_since_balsam_submit(self):
         """Return time since balsam task entered ``RUNNING`` state"""
-
         event_query = EventLog.objects.filter(job_id=self.process.id, to_state="RUNNING")
         if not len(event_query):
             return 0
         balsam_launch_datetime = event_query[0].timestamp
         current_datetime = datetime.datetime.now()
         if balsam_launch_datetime:
             return (current_datetime - balsam_launch_datetime).total_seconds()
         else:
             return 0
 
     def calc_task_timing(self):
         """Calculate timing information for this task"""
-
         # Get runtime from Balsam
         self.runtime = self._get_time_since_balsam_submit()
 
         if self.submit_time is None:
             logger.warning("Cannot calc task total_time - submit time not set")
             return
 
@@ -158,21 +155,18 @@
                 "RUN_DONE",
                 "POSTPROCESSED",
                 "STAGED_OUT",
                 "JOB_FINISHED",
             ]:
                 self.success = True
                 self.state = "FINISHED"
-            elif balsam_state in STATES:  # In my states
-                self.state = balsam_state
             else:
-                logger.warning("Task finished, but in unrecognized " "Balsam state {}".format(balsam_state))
-                self.state = "UNKNOWN"
+                self.state = balsam_state
 
-            logger.info("Task {} ended with state {}".format(self.name, self.state))
+        logger.info(f"Task {self.name} ended with state {self.state}")
 
     def poll(self):
         """Polls and updates the status attributes of the supplied task. Requests
         Job information from Balsam service."""
         if self.dry_run:
             return
 
@@ -198,35 +192,28 @@
             "STAGED_IN",
             "PREPROCESSED",
         ]:
             self.state = "WAITING"
 
         elif balsam_state in ["RUN_ERROR", "RUN_TIMEOUT", "FAILED"]:
             self.state = "FAILED"
-
-        else:
-            raise ExecutorException(
-                "Task state returned from Balsam is not in known list of "
-                "Balsam states. Task state is {}".format(balsam_state)
-            )
+            self._set_complete()
 
     def wait(self, timeout=None):
         """Waits on completion of the task or raises ``TimeoutExpired``.
 
         Status attributes of task are updated on completion.
 
         Parameters
         ----------
 
         timeout: int or float,  optional
             Time in seconds after which a TimeoutExpired exception is raised.
             If not set, then simply waits until completion.
-            Note that the task is not automatically killed if libEnsemble
-            timeouts from reaching exit_criteria["wallclock_max"].
-
+            Note that the task is not automatically killed on timeout.
         """
 
         if self.dry_run:
             return
 
         if not self._check_poll():
             return
@@ -235,30 +222,32 @@
         start = time.time()
         self.process.refresh_from_db()
         while self.process.state not in [
             "RUN_DONE",
             "POSTPROCESSED",
             "STAGED_OUT",
             "JOB_FINISHED",
+            "RUN_ERROR",
+            "RUN_TIMEOUT",
+            "FAILED",
         ]:
             time.sleep(0.2)
             self.process.refresh_from_db()
             if timeout and time.time() - start > timeout:
                 self.runtime = self._get_time_since_balsam_submit()
                 raise TimeoutExpired(self.name, timeout)
 
         self.runtime = self._get_time_since_balsam_submit()
         self._set_complete()
 
     def kill(self):
         """Cancels the supplied task. Killing is unsupported at this time."""
-
         self.process.delete()
 
-        logger.info("Killing task {}".format(self.name))
+        logger.info(f"Killing task {self.name}")
         self.state = "USER_KILLED"
         self.finished = True
         self.calc_task_timing()
 
 
 class BalsamExecutor(Executor):
     """Inherits from ``Executor`` and wraps the Balsam service. Via this Executor,
@@ -266,29 +255,28 @@
 
     .. note::  Task kills are not configurable in the Balsam executor.
 
     """
 
     def __init__(self):
         """Instantiate a new ``BalsamExecutor`` instance."""
-
         super().__init__()
 
         self.workflow_name = "libe_workflow"
         self.allocations = []
 
     def serial_setup(self):
         """Balsam serial setup includes emptying database and adding applications"""
         pass
 
-    def add_app(self, name, site, exepath, desc):
+    def add_app(self, *args):
         """Sync application with Balsam service"""
         pass
 
-    def register_app(self, BalsamApp, app_name, calc_type=None, desc=None, precedent=None):
+    def register_app(self, BalsamApp, app_name=None, calc_type=None, desc=None, precedent=None):
         """Registers a Balsam ``ApplicationDefinition`` to libEnsemble. This class
         instance *must* have a ``site`` and ``command_template`` specified. See
         the Balsam docs for information on other optional fields.
 
         Parameters
         ----------
 
@@ -388,41 +376,51 @@
             filter_tags=filter_tags,
             partitions=partitions,
         )
 
         self.allocations.append(allocation)
 
         logger.info(
-            "Submitted Batch allocation to site {}: "
-            "nodes {} queue {} project {}".format(site_id, num_nodes, queue, project)
+            f"Submitted Batch allocation to site {site_id}: " f"nodes {num_nodes} queue {queue} project {project}"
         )
 
         return allocation
 
-    def revoke_allocation(self, allocation):
+    def revoke_allocation(self, allocation, timeout=60):
         """
         Terminates a Balsam ``BatchJob`` machine allocation remotely. Balsam apps should
         no longer be submitted to this allocation. Best to run after libEnsemble
         completes, or after this ``BatchJob`` is no longer needed. Helps save machine time.
 
         Parameters
         ----------
 
         allocation: ``BatchJob`` object
             a ``BatchJob`` with a corresponding machine allocation that should be cancelled.
+
+        timeout: int, optional
+            Timeout and warn user after this many seconds of attempting to revoke an allocation.
         """
         allocation.refresh_from_db()
 
+        start = time.time()
+
         while not allocation.scheduler_id:
             time.sleep(1)
             allocation.refresh_from_db()
+            if time.time() - start > timeout:
+                logger.warning(
+                    "Unable to terminate Balsam BatchJob. You may need to login to the machine and manually remove it."
+                )
+                return False
 
         batchjob = BatchJob.objects.get(scheduler_id=allocation.scheduler_id)
         batchjob.state = "pending_deletion"
         batchjob.save()
+        return True
 
     def set_resources(self, resources):
         self.resources = resources
 
     def submit(
         self,
         calc_type=None,
@@ -519,24 +517,20 @@
         if len(workdir):
             workdir = os.path.join(self.workflow_name, workdir)
         else:
             workdir = self.workflow_name
 
         if machinefile is not None:
             logger.warning("machinefile arg ignored - not supported in Balsam")
-            jassert(
-                num_procs or num_nodes or procs_per_node,
-                "No procs/nodes provided - aborting",
-            )
 
         task = BalsamTask(app, app_args, workdir, None, None, self.workerID)
 
         if dry_run:
             task.dry_run = True
-            logger.info("Test (No submit) Balsam app {}".format(app_name))
+            logger.info(f"Test (No submit) Balsam app {app_name}")
             task._set_complete(dry_run=True)
         else:
             App = app.pyobj
 
             try:
                 App.sync()  # if App source-code available, send to Balsam service
             except OSError:
@@ -559,13 +553,11 @@
             if wait_on_start:
                 self._wait_on_start(task)
 
             if not task.timer.timing and not task.finished:
                 task.timer.start()
                 task.submit_time = task.timer.tstart  # Time not date - may not need if using timer.
 
-            logger.info(
-                "Submitted Balsam App to site {}: " "nodes {} ppn {}".format(App.site, num_nodes, procs_per_node)
-            )
+            logger.info(f"Submitted Balsam App to site {App.site}: " "nodes {num_nodes} ppn {procs_per_node}")
 
         self.list_of_tasks.append(task)
         return task
```

### Comparing `libensemble-0.9.2/libensemble/executors/balsam_executors/legacy_balsam_executor.py` & `libensemble-0.9.3/libensemble/executors/balsam_executors/legacy_balsam_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,29 +61,27 @@
         return self.process.read_file_in_workdir(self.stdout)
 
     def read_stderr(self):
         return self.process.read_file_in_workdir(self.stderr)
 
     def _get_time_since_balsam_submit(self):
         """Return time since balsam task entered RUNNING state"""
-
         # If wait_on_start then can could calculate runtime same a base executor
         # but otherwise that will return time from task submission. Get from Balsam.
 
         # self.runtime = self.process.runtime_seconds # Only reports at end of run currently
         balsam_launch_datetime = self.process.get_state_times().get("RUNNING", None)
         current_datetime = datetime.datetime.now()
         if balsam_launch_datetime:
             return (current_datetime - balsam_launch_datetime).total_seconds()
         else:
             return 0
 
     def calc_task_timing(self):
         """Calculate timing information for this task"""
-
         # Get runtime from Balsam
         self.runtime = self._get_time_since_balsam_submit()
 
         if self.submit_time is None:
             logger.warning("Cannot calc task total_time - submit time not set")
             return
 
@@ -104,18 +102,18 @@
             if balsam_state == "JOB_FINISHED":
                 self.state = "FINISHED"
             elif balsam_state == "PARENT_KILLED":  # Not currently used
                 self.state = "USER_KILLED"
             elif balsam_state in STATES:  # In my states
                 self.state = balsam_state
             else:
-                logger.warning("Task finished, but in unrecognized " "Balsam state {}".format(balsam_state))
+                logger.warning(f"Task finished, but in unrecognized Balsam state {balsam_state}")
                 self.state = "UNKNOWN"
 
-            logger.info("Task {} ended with state {}".format(self.name, self.state))
+            logger.info(f"Task {self.name} ended with state {self.state}")
 
     def poll(self):
         """Polls and updates the status attributes of the supplied task"""
         if self.dry_run:
             return
 
         if not self._check_poll():
@@ -148,16 +146,15 @@
         Status attributes of task are updated on completion.
 
         Parameters
         ----------
         timeout: int or float,  optional
             Time in seconds after which a TimeoutExpired exception is raised.
             If not set, then simply waits until completion.
-            Note that the task is not automatically killed if libEnsemble
-            timeouts from reaching exit_criteria["wallclock_max"].
+            Note that the task is not automatically killed on timeout.
         """
 
         if self.dry_run:
             return
 
         if not self._check_poll():
             return
@@ -173,21 +170,20 @@
                 raise TimeoutExpired(self.name, timeout)
 
         self.runtime = self._get_time_since_balsam_submit()
         self._set_complete()
 
     def kill(self, wait_time=None):
         """Kills or cancels the supplied task"""
-
         dag.kill(self.process)
 
         # Could have Wait here and check with Balsam its killed -
         # but not implemented yet.
 
-        logger.info("Killing task {}".format(self.name))
+        logger.info(f"Killing task {self.name}")
         self.state = "USER_KILLED"
         self.finished = True
         self.calc_task_timing()
 
 
 class LegacyBalsamMPIExecutor(MPIExecutor):
     """Inherits from MPIExecutor and wraps the Balsam task management service
@@ -227,39 +223,39 @@
         AppDef = models.ApplicationDefinition
 
         # Some error handling on deletes.... is it internal
         for app_type in [Application.prefix]:
             deletion_objs = AppDef.objects.filter(name__contains=app_type)
             if deletion_objs:
                 for del_app in deletion_objs.iterator():
-                    logger.debug("Deleting app {}".format(del_app.name))
+                    logger.debug(f"Deleting app {del_app.name}")
                 deletion_objs.delete()
 
     @staticmethod
     def del_tasks():
         """Deletes all Balsam tasks"""
         for app_type in [Task.prefix]:
             deletion_objs = models.BalsamJob.objects.filter(name__contains=app_type)
             if deletion_objs:
                 for del_task in deletion_objs.iterator():
-                    logger.debug("Deleting task {}".format(del_task.name))
+                    logger.debug(f"Deleting task {del_task.name}")
                 deletion_objs.delete()
 
     @staticmethod
     def add_app(name, exepath, desc):
         """Add application to Balsam database"""
         AppDef = models.ApplicationDefinition
         app = AppDef()
         app.name = name
         app.executable = exepath
         app.description = desc
         # app.default_preprocess = '' # optional
         # app.default_postprocess = '' # optional
         app.save()
-        logger.debug("Added App {}".format(app.name))
+        logger.debug(f"Added App {app.name}")
 
     def set_resources(self, resources):
         self.resources = resources
 
     def submit(
         self,
         calc_type=None,
@@ -322,26 +318,24 @@
             # For now hardcode staging - for testing
             add_task_args["stage_in_url"] = "local:" + stage_inout + "/*"
             add_task_args["stage_out_url"] = "local:" + stage_inout
             add_task_args["stage_out_files"] = "*.out"
 
         if dry_run:
             task.dry_run = True
-            logger.info("Test (No submit) Runline: {}".format(" ".join(add_task_args)))
+            logger.info(f"Test (No submit) Runline: {' '.join(add_task_args)}")
             task._set_complete(dry_run=True)
         else:
             task.process = dag.add_job(**add_task_args)
 
             if wait_on_start:
                 self._wait_on_start(task)
 
             if not task.timer.timing and not task.finished:
                 task.timer.start()
                 task.submit_time = task.timer.tstart  # Time not date - may not need if using timer.
 
-            logger.info(
-                "Added task to Balsam database {}: " "nodes {} ppn {}".format(task.name, num_nodes, procs_per_node)
-            )
+            logger.info(f"Added task to Balsam database {task.name}: nodes {num_nodes} ppn {procs_per_node}")
 
             # task.workdir = task.process.working_directory  # Might not be set yet!
         self.list_of_tasks.append(task)
         return task
```

### Comparing `libensemble-0.9.2/libensemble/executors/executor.py` & `libensemble-0.9.3/libensemble/executors/executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 import sys
 import logging
 import itertools
 import time
 
 from libensemble.message_numbers import (
     UNSET_TAG,
-    MAN_SIGNAL_FINISH,
-    MAN_SIGNAL_KILL,
+    MAN_KILL_SIGNALS,
     WORKER_DONE,
     TASK_FAILED,
     WORKER_KILL_ON_TIMEOUT,
     STOP_TAG,
 )
 
 import libensemble.utils.launcher as launcher
@@ -63,15 +62,15 @@
     """Timeout exception raised when Timeout expires"""
 
     def __init__(self, task, timeout):
         self.task = task
         self.timeout = timeout
 
     def __str__(self):
-        return "Task {} timed out after {} seconds".format(self.task, self.timeout)
+        return f"Task {self.task} timed out after {self.timeout} seconds"
 
 
 def jassert(test, *args):
     "Version of assert that raises a ExecutorException"
     if not test:
         raise ExecutorException(*args)
 
@@ -121,18 +120,18 @@
         self.timer = TaskTimer()
 
         # Run attributes
         self.app = app
         self.app_args = app_args
         self.workerID = workerid
 
-        jassert(app is not None, "Task must be created with an app - no app found for task {}".format(self.id))
+        jassert(app is not None, f"Task must be created with an app - no app found for task {self.id}")
 
-        worker_name = "_worker{}".format(self.workerID) if self.workerID else ""
-        self.name = Task.prefix + "_{}{}_{}".format(app.name, worker_name, self.id)
+        worker_name = f"_worker{self.workerID}" if self.workerID else ""
+        self.name = Task.prefix + f"_{app.name}{worker_name}_{self.id}"
         self.stdout = stdout or self.name + ".out"
         self.stderr = stderr or self.name + ".err"
         self.workdir = workdir
         self.dry_run = dry_run
         self.runline = None
         self.run_attempts = 0
 
@@ -155,15 +154,15 @@
         """Returns true if the named file exists in the task's workdir"""
         return self.workdir and os.path.exists(os.path.join(self.workdir, filename))
 
     def read_file_in_workdir(self, filename):
         """Opens and reads the named file in the task's workdir"""
         path = os.path.join(self.workdir, filename)
         if not os.path.exists(path):
-            raise ValueError("{} not found in working directory".format(filename))
+            raise ValueError(f"{filename} not found in working directory")
         with open(path) as f:
             return f.read()
 
     def stdout_exists(self):
         """Returns true if the task's stdout file exists in the workdir"""
         return self.file_exists_in_workdir(self.stdout)
 
@@ -189,36 +188,32 @@
         if self.total_time is None:
             self.timer.stop()
             self.runtime = self.timer.elapsed
             self.total_time = self.runtime  # For direct launched tasks
 
     def _check_poll(self):
         """Check whether polling this task makes sense."""
-        jassert(
-            self.process is not None, "Polled task {} has no process ID - check tasks been launched".format(self.name)
-        )
+        jassert(self.process is not None, f"Polled task {self.name} has no process ID - check tasks been launched")
         if self.finished:
-            logger.debug(
-                "Polled task {} has already finished. " "Not re-polling. Status is {}".format(self.name, self.state)
-            )
+            logger.debug(f"Polled task {self.name} has already finished. Not re-polling. Status is {self.state}")
             return False
         return True
 
     def _set_complete(self, dry_run=False):
         """Set task as complete"""
         self.finished = True
         if dry_run:
             self.success = True
             self.state = "FINISHED"
         else:
             self.calc_task_timing()
             self.errcode = self.process.returncode
             self.success = self.errcode == 0
             self.state = "FINISHED" if self.success else "FAILED"
-            logger.info("Task {} finished with errcode {} ({})".format(self.name, self.errcode, self.state))
+            logger.info(f"Task {self.name} finished with errcode {self.errcode} ({self.state})")
 
     def poll(self):
         """Polls and updates the status attributes of the task"""
         if self.dry_run:
             return
 
         if not self._check_poll():
@@ -240,16 +235,15 @@
 
         Parameters
         ----------
 
         timeout: int or float,  optional
             Time in seconds after which a TimeoutExpired exception is raised.
             If not set, then simply waits until completion.
-            Note that the task is not automatically killed if libEnsemble
-            timeouts from reaching exit_criteria["wallclock_max"].
+            Note that the task is not automatically killed on timeout.
         """
 
         if self.dry_run:
             return
 
         if not self._check_poll():
             return
@@ -266,32 +260,30 @@
 
         Parameters
         ----------
 
         timeout: int or float,  optional
             Time in seconds after which a TimeoutExpired exception is raised.
             If not set, then simply waits until completion.
-            Note that the task is not automatically killed if libEnsemble
-            timeouts from reaching exit_criteria["wallclock_max"].
+            Note that the task is not automatically killed on timeout.
         """
 
         self.wait(timeout=timeout)
         return self.state
 
     def exception(self, timeout=None):
         """Wrapper for task.wait() that instead returns the task's error code on completion.
 
         Parameters
         ----------
 
         timeout: int or float,  optional
             Time in seconds after which a TimeoutExpired exception is raised.
             If not set, then simply waits until completion.
-            Note that the task is not automatically killed if libEnsemble
-            timeouts from reaching exit_criteria["wallclock_max"].
+            Note that the task is not automatically killed on timeout.
         """
 
         self.wait(timeout=timeout)
         return self.errcode
 
     def running(self):
         """Return ```True`` if task is currently running."""
@@ -309,27 +301,25 @@
         is 0, we go immediately to SIGKILL; if <wait_time> is none, we
         never do a SIGKILL.
         """
         if self.dry_run:
             return
 
         if self.finished:
-            logger.warning(
-                "Trying to kill task that is no longer running. Task {}: Status is {}".format(self.name, self.state)
-            )
+            logger.warning(f"Trying to kill task that is no longer running. Task {self.name}: Status is {self.state}")
             return
 
         if self.process is None:
             time.sleep(0.2)
             jassert(
                 self.process is not None,
-                "Attempting to kill task {} that has no process ID - check tasks been launched".format(self.name),
+                f"Attempting to kill task {self.name} that has no process ID - check tasks been launched",
             )
 
-        logger.info("Killing task {}".format(self.name))
+        logger.info(f"Killing task {self.name}")
         launcher.cancel(self.process, wait_time)
         self.state = "USER_KILLED"
         self.finished = True
         self.calc_task_timing()
 
     def cancel(self):
         """Wrapper for task.kill() without waiting"""
@@ -346,14 +336,15 @@
     **Class Attributes:**
 
     :cvar Executor: executor: The executor object is stored here and can be retrieved in user functions.
 
     **Object Attributes:**
 
     :ivar list list_of_tasks: A list of tasks created in this executor
+    :ivar int manager_signal: The most recent manager signal received since manager_poll() was called.
     """
 
     executor = None
 
     def _wait_on_start(self, task, fail_time=None):
         """Called by submit when wait_on_start is True.
 
@@ -363,34 +354,34 @@
         """
         start = time.time()
         task.timer.start()  # To ensure a start time before poll - will be overwritten unless finished by poll.
         task.submit_time = task.timer.tstart
         while task.state in NOT_STARTED_STATES:
             time.sleep(0.001)
             task.poll()
-        logger.debug("Task {} polled as {} after {} seconds".format(task.name, task.state, time.time() - start))
+        logger.debug(f"Task {task.name} polled as {task.state} after {time.time() - start} seconds")
         if not task.finished:
             task.timer.start()
             task.submit_time = task.timer.tstart
             if fail_time:
                 remaining = fail_time - task.timer.elapsed
                 while task.state not in END_STATES and remaining > 0:
                     time.sleep(min(0.01, remaining))
                     task.poll()
                     remaining = fail_time - task.timer.elapsed
-                logger.debug("After {} seconds: task {} polled as {}".format(task.timer.elapsed, task.name, task.state))
+                logger.debug(f"After {task.timer.elapsed} seconds: task {task.name} polled as {task.state}")
 
     def __init__(self):
         """Instantiate a new Executor instance.
 
         A new Executor object is created.
         This is typically created in the user calling script.
         """
 
-        self.manager_signal = "none"
+        self.manager_signal = None
         self.default_apps = {"sim": None, "gen": None}
         self.apps = {}
 
         self.wait_time = 60
         self.list_of_tasks = []
         self.workerID = None
         self.comm = None
@@ -420,23 +411,23 @@
     def get_app(self, app_name):
         """Gets the app for a given app_name or raise exception"""
         try:
             app = self.apps[app_name]
         except KeyError:
             app_keys = list(self.apps.keys())
             raise ExecutorException(
-                "Application {} not found in registry".format(app_name), "Registered applications: {}".format(app_keys)
+                f"Application {app_name} not found in registry", f"Registered applications: {app_keys}"
             )
         return app
 
     def default_app(self, calc_type):
         """Gets the default app for a given calc type"""
         app = self.default_apps.get(calc_type)
         jassert(calc_type in ["sim", "gen"], "Unrecognized calculation type", calc_type)
-        jassert(app, "Default {} app is not set".format(calc_type))
+        jassert(app, f"Default {calc_type} app is not set")
         return app
 
     def set_resources(self, resources):
         # Does not use resources
         pass
 
     def register_app(self, full_path, app_name=None, calc_type=None, desc=None, precedent=""):
@@ -481,34 +472,41 @@
         .. _manager_poll_label:
 
         Polls for a manager signal
 
         The executor manager_signal attribute will be updated.
         """
 
-        self.manager_signal = "none"  # Reset
+        self.manager_signal = None  # Reset
 
         # Check for messages; disregard anything but a stop signal
         if not self.comm.mail_flag():
             return
         mtag, man_signal = self.comm.recv()
         if mtag != STOP_TAG:
             return
 
         # Process the signal and push back on comm (for now)
-        logger.info("Worker received kill signal {} from manager".format(man_signal))
-        if man_signal == MAN_SIGNAL_FINISH:
-            self.manager_signal = "finish"
-        elif man_signal == MAN_SIGNAL_KILL:
-            self.manager_signal = "kill"
+        self.manager_signal = man_signal
+
+        if man_signal in MAN_KILL_SIGNALS:
+            # Only kill signals exist currently
+            logger.info(f"Worker received kill signal {man_signal} from manager")
         else:
-            logger.warning("Received unrecognized manager signal {} - ignoring".format(man_signal))
+            logger.warning(f"Received unrecognized manager signal {man_signal} - ignoring")
         self.comm.push_to_buffer(mtag, man_signal)
         return man_signal
 
+    def manager_kill_received(self):
+        """Return True if received kill signal from the manager"""
+        man_signal = self.manager_poll()
+        if man_signal in MAN_KILL_SIGNALS:
+            return True
+        return False
+
     def polling_loop(self, task, timeout=None, delay=0.1, poll_manager=False):
         """Optional, blocking, generic task status polling loop. Operates until the task
         finishes, times out, or is optionally killed via a manager signal. On completion, returns a
         presumptive :ref:`calc_status<datastruct-calc-status>` integer. Potentially useful
         for running an application via the Executor until it stops without monitoring
         its intermediate output.
 
@@ -538,15 +536,15 @@
         calc_status = UNSET_TAG
 
         while not task.finished:
             task.poll()
 
             if poll_manager:
                 man_signal = self.manager_poll()
-                if self.manager_signal != "none":
+                if self.manager_signal in MAN_KILL_SIGNALS:
                     task.kill()
                     calc_status = man_signal
                     break
 
             if timeout is not None and task.runtime > timeout:
                 task.kill()
                 calc_status = WORKER_KILL_ON_TIMEOUT
@@ -556,25 +554,23 @@
 
         if calc_status == UNSET_TAG:
             if task.state == "FINISHED":
                 calc_status = WORKER_DONE
             elif task.state == "FAILED":
                 calc_status = TASK_FAILED
             else:
-                logger.warning(
-                    "Warning: Task {} in unknown state {}. Error code {}".format(self.name, self.state, self.errcode)
-                )
+                logger.warning(f"Warning: Task {self.name} in unknown state {self.state}. Error code {self.errcode}")
 
         return calc_status
 
     def get_task(self, taskid):
         """Returns the task object for the supplied task ID"""
         task = next((j for j in self.list_of_tasks if j.id == taskid), None)
         if task is None:
-            logger.warning("Task {} not found in tasklist".format(taskid))
+            logger.warning(f"Task {taskid} not found in tasklist")
         return task
 
     def new_tasks_timing(self, datetime=False):
         """Returns timing of new tasks as a string
 
         Parameters
         ----------
@@ -584,17 +580,17 @@
         """
 
         timing_msg = ""
         if self.list_of_tasks:
             start_task = self.last_task
             for i, task in enumerate(self.list_of_tasks[start_task:]):
                 if datetime:
-                    timing_msg += " Task {}: {}".format(i, task.timer)
+                    timing_msg += f" Task {i}: {task.timer}"
                 else:
-                    timing_msg += " Task {}: {}".format(i, task.timer.summary())
+                    timing_msg += f" Task {i}: {task.timer.summary()}"
                 self.last_task += 1
         return timing_msg
 
     def set_workerID(self, workerid):
         """Sets the worker ID for this executor"""
         self.workerID = workerid
 
@@ -602,15 +598,15 @@
         """Sets info for this executor"""
         self.workerID = workerid
         self.comm = comm
 
     def _check_app_exists(self, full_path):
         """Allows submit function to check if app exists and error if not"""
         if not os.path.isfile(full_path):
-            raise ExecutorException("Application does not exist {}".format(full_path))
+            raise ExecutorException(f"Application does not exist {full_path}")
 
     def submit(
         self, calc_type=None, app_name=None, app_args=None, stdout=None, stderr=None, dry_run=False, wait_on_start=False
     ):
         """Create a new task and run as a local serial subprocess.
 
         The created task object is returned.
@@ -664,18 +660,18 @@
             self._check_app_exists(task.app.full_path)
 
         runline = task.app.app_cmd.split()
         if task.app_args is not None:
             runline.extend(task.app_args.split())
 
         if dry_run:
-            logger.info("Test (No submit) Runline: {}".format(" ".join(runline)))
+            logger.info(f"Test (No submit) Runline: {' '.join(runline)}")
         else:
             # Launch Task
-            logger.info("Launching task {}: {}".format(task.name, " ".join(runline)))
+            logger.info(f"Launching task {task.name}: {' '.join(runline)}")
             with open(task.stdout, "w") as out, open(task.stderr, "w") as err:
                 task.process = launcher.launch(
                     runline,
                     cwd="./",
                     stdout=out,
                     stderr=err,
                     start_new_session=False,
```

### Comparing `libensemble-0.9.2/libensemble/executors/mpi_executor.py` & `libensemble-0.9.3/libensemble/executors/mpi_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 
 logger = logging.getLogger(__name__)
 # To change logging level for just this module
 # logger.setLevel(logging.DEBUG)
 
 
 class MPIExecutor(Executor):
-    """The MPI executor can create, poll and kill runnable MPI tasks"""
+    """The MPI executor can create, poll and kill runnable MPI tasks
+
+    **Object Attributes:**
+
+    :ivar list list_of_tasks: A list of tasks created in this executor
+    :ivar int manager_signal: The most recent manager signal received since manager_poll() was called.
+    """
 
     def __init__(self, custom_info={}):
         """Instantiate a new MPIExecutor instance.
 
         A new MPIExecutor is created with an application
         registry and configuration attributes.
 
@@ -98,45 +104,43 @@
 
     def _launch_with_retries(self, task, runline, subgroup_launch, wait_on_start):
         """Launch task with retry mechanism"""
         retry_count = 0
         while retry_count < self.max_launch_attempts:
             retry = False
             try:
-                retry_string = " (Retry {})".format(retry_count) if retry_count > 0 else ""
-                logger.info("Launching task {}{}: {}".format(task.name, retry_string, " ".join(runline)))
+                retry_string = f" (Retry {retry_count})" if retry_count > 0 else ""
+                logger.info(f"Launching task {task.name}{retry_string}: {' '.join(runline)}")
                 task.run_attempts += 1
                 with open(task.stdout, "w") as out, open(task.stderr, "w") as err:
                     task.process = launcher.launch(
                         runline,
                         cwd="./",
                         stdout=out,
                         stderr=err,
                         start_new_session=subgroup_launch,
                     )
             except Exception as e:
-                logger.warning(
-                    "task {} submit command failed on try {} with error {}".format(task.name, retry_count, e)
-                )
+                logger.warning(f"task {task.name} submit command failed on try {retry_count} with error {e}")
                 retry = True
                 retry_count += 1
             else:
                 if wait_on_start:
                     self._wait_on_start(task, self.fail_time)
 
                 if task.state == "FAILED":
                     logger.warning(
-                        "task {} failed within fail_time on "
-                        "try {} with err code {}".format(task.name, retry_count, task.errcode)
+                        f"task {task.name} failed within fail_time on "
+                        f"try {retry_count} with err code {task.errcode}"
                     )
                     retry = True
                     retry_count += 1
 
             if retry and retry_count < self.max_launch_attempts:
-                logger.debug("Retry number {} for task {}".format(retry_count, task.name))
+                logger.debug(f"Retry number {retry_count} for task {task.name}")
                 time.sleep(retry_count * self.retry_delay_incr)
                 task.reset()  # Some cases may require user cleanup
             else:
                 break
 
     def submit(
         self,
@@ -261,15 +265,15 @@
         runline.extend(task.app.app_cmd.split())
         if task.app_args is not None:
             runline.extend(task.app_args.split())
 
         task.runline = " ".join(runline)  # Allow to be queried
         if dry_run:
             task.dry_run = True
-            logger.info("Test (No submit) Runline: {}".format(" ".join(runline)))
+            logger.info(f"Test (No submit) Runline: {' '.join(runline)}")
             task._set_complete(dry_run=True)
         else:
             # Launch Task
             self._launch_with_retries(task, runline, sglaunch, wait_on_start)
 
             if not task.timer.timing and not task.finished:
                 task.timer.start()
```

### Comparing `libensemble-0.9.2/libensemble/executors/mpi_runner.py` & `libensemble-0.9.3/libensemble/executors/mpi_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
         mpi_runners = {
             "mpich": MPICH_MPIRunner,
             "openmpi": OPENMPI_MPIRunner,
             "aprun": APRUN_MPIRunner,
             "srun": SRUN_MPIRunner,
             "jsrun": JSRUN_MPIRunner,
+            "msmpi": MSMPI_MPIRunner,
             "custom": MPIRunner,
         }
         mpi_runner = mpi_runners[mpi_runner_type]
         if runner_name is not None:
             runner = mpi_runner(runner_name)
         else:
             runner = mpi_runner()
@@ -88,15 +89,15 @@
         if extra_args:
             num_procs, num_nodes, procs_per_node, p_args = self._parse_extra_args(
                 num_procs, num_nodes, procs_per_node, hyperthreads, extra_args=extra_args
             )
 
         hostlist = None
         if machinefile and not self.mfile_support:
-            logger.warning("User machinefile ignored - not supported by {}".format(self.run_command))
+            logger.warning(f"User machinefile ignored - not supported by {self.run_command}")
             machinefile = None
 
         if machinefile is None and resources is not None:
             num_procs, num_nodes, procs_per_node = mpi_resources.get_resources(
                 resources, num_procs, num_nodes, procs_per_node, hyperthreads
             )
             hostlist, machinefile = self.express_spec(
@@ -167,16 +168,16 @@
         hostlist = None
         machinefile = None
         # Use machine files for OpenMPI
         # as "-host" requires entry for every rank
 
         machinefile = "machinefile_autogen"
         if workerID is not None:
-            machinefile += "_for_worker_{}".format(workerID)
-        machinefile += "_task_{}".format(task.id)
+            machinefile += f"_for_worker_{workerID}"
+        machinefile += f"_task_{task.id}"
         mfile_created, num_procs, num_nodes, procs_per_node = mpi_resources.create_machinefile(
             resources, machinefile, num_procs, num_nodes, procs_per_node, hyperthreads
         )
         jassert(mfile_created, "Auto-creation of machinefile failed")
 
         return hostlist, machinefile
 
@@ -195,14 +196,31 @@
             "-L {hostlist}",
             "-n {num_procs}",
             "-N {procs_per_node}",
             "{extra_args}",
         ]
 
 
+class MSMPI_MPIRunner(MPIRunner):
+    def __init__(self, run_command="mpiexec"):
+        self.run_command = run_command
+        self.subgroup_launch = False
+        self.mfile_support = False
+        self.arg_nprocs = ("-n", "-np")
+        self.arg_nnodes = ("--LIBE_NNODES_ARG_EMPTY",)
+        self.arg_ppn = ("-cores",)
+        self.mpi_command = [
+            self.run_command,
+            "-env {env}",
+            "-n {num_procs}",
+            "-cores {procs_per_node}",
+            "{extra_args}",
+        ]
+
+
 class SRUN_MPIRunner(MPIRunner):
     def __init__(self, run_command="srun"):
         self.run_command = run_command
         self.subgroup_launch = False
         self.mfile_support = False
         self.arg_nprocs = ("-n", "--ntasks")
         self.arg_nnodes = ("-N", "--nodes")
@@ -239,15 +257,15 @@
                 num_procs, num_nodes, procs_per_node, hyperthreads, extra_args=extra_args
             )
 
         rm_rpn = True if procs_per_node is None and num_nodes is None else False
 
         hostlist = None
         if machinefile and not self.mfile_support:
-            logger.warning("User machinefile ignored - not supported by {}".format(self.run_command))
+            logger.warning(f"User machinefile ignored - not supported by {self.run_command}")
             machinefile = None
         if machinefile is None and resources is not None:
             num_procs, num_nodes, procs_per_node = mpi_resources.get_resources(
                 resources, num_procs, num_nodes, procs_per_node, hyperthreads
             )
 
             # TODO: Create ERF file if mapping worker to resources req.
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/aposmm_localopt_support.py` & `libensemble-0.9.3/libensemble/gen_funcs/aposmm_localopt_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     import dfols
     from scipy import optimize as sp_opt
 else:
     if not isinstance(optimizers, list):
         optimizers = [optimizers]
     unrec = set(optimizers) - set(optimizer_list)
     if unrec:
-        print('APOSMM Warning: unrecognized optimizers {}'.format(unrec))
+        print(f'APOSMM Warning: unrecognized optimizers {unrec}')
 
     if 'petsc' in optimizers:
         from petsc4py import PETSc
     if 'nlopt' in optimizers:
         import nlopt
     if 'dfols' in optimizers:
         import dfols
@@ -244,15 +244,14 @@
 
 
 def run_local_scipy_opt(user_specs, comm_queue, x0, f0, child_can_read, parent_can_read):
     """
     Runs a SciPy local optimization run starting at ``x0``, governed by the
     parameters in ``user_specs``.
     """
-
     # Construct the bounds in the form of constraints
     cons = []
     for factor in range(len(x0)):
         lo = {'type': 'ineq',
               'fun': lambda x, lb=user_specs['lb'][factor], i=factor: x[i]-lb}
         up = {'type': 'ineq',
               'fun': lambda x, ub=user_specs['ub'][factor], i=factor: ub-x[i]}
@@ -301,15 +300,15 @@
     y_file = 'y_' + run_id + '.txt'
     x_done_file = 'x_done_' + run_id + '.txt'
     y_done_file = 'y_done_' + run_id + '.txt'
     opt_file = 'opt_' + run_id + '.txt'
 
     # cmd = ["matlab", "-nodisplay", "-nodesktop", "-nojvm", "-nosplash", "-r",
     cmd = ["octave", "--no-window-system", "--eval",
-           "x0=[" + " ".join(["{:18.18f}".format(x) for x in x0]) + "];"
+           "x0=[" + " ".join([f"{x:18.18f}" for x in x0]) + "];"
            "opt_file='" + opt_file + "';"
            "x_file='" + x_file + "';"
            "y_file='" + y_file + "';"
            "x_done_file='" + x_done_file + "';"
            "y_done_file='" + y_done_file + "';"
            "call_matlab_octave_script"]
 
@@ -335,15 +334,14 @@
 
 
 def run_local_dfols(user_specs, comm_queue, x0, f0, child_can_read, parent_can_read):
     """
     Runs a DFOLS local optimization run starting at ``x0``, governed by the
     parameters in ``user_specs``.
     """
-
     # Define bound constraints (lower <= x <= upper)
     lb = np.zeros(len(x0))
     ub = np.ones(len(x0))
 
     # Set random seed (for reproducibility)
     np.random.seed(0)
 
@@ -373,15 +371,14 @@
 
 
 def run_local_tao(user_specs, comm_queue, x0, f0, child_can_read, parent_can_read):
     """
     Runs a PETSc/TAO local optimization run starting at ``x0``, governed by the
     parameters in ``user_specs``.
     """
-
     assert isinstance(x0, np.ndarray)
 
     tao_comm = PETSc.COMM_SELF
     n, = x0.shape
     if f0.shape == ():
         m = 1
     else:
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/old_aposmm.py` & `libensemble-0.9.3/libensemble/gen_funcs/old_aposmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     import nlopt
     from scipy import optimize as scipy_optimize
 else:
     if not isinstance(optimizers, list):
         optimizers = [optimizers]
     unrec = set(optimizers) - set(optimizer_list)
     if unrec:
-        print('APOSMM Warning: unrecognized optimizers {}'.format(unrec))
+        print(f'APOSMM Warning: unrecognized optimizers {unrec}')
 
     if 'petsc' in optimizers:
         from petsc4py import PETSc
     if 'nlopt' in optimizers:
         import nlopt
     if 'scipy' in optimizers:
         from scipy import optimize as scipy_optimize
@@ -880,15 +880,14 @@
     advance_local_run.pt_in_run += 1
 
     return f_out
 
 
 def calc_rk(n, n_s, rk_const, lhs_divisions=0):
     """ Calculate the critical distance r_k """
-
     if lhs_divisions == 0:
         r_k = rk_const*(log(n_s)/n_s)**(1/n)
     else:
         k = np.floor(n_s/lhs_divisions).astype(int)
         if k <= 1:  # to prevent r_k=0
             r_k = np.inf
         else:
@@ -957,15 +956,15 @@
 def display_exception(e):
     print(e.__doc__)
     print(e.args)
     _, _, tb = sys.exc_info()
     traceback.print_tb(tb)  # Fixed format
     tb_info = traceback.extract_tb(tb)
     filename, line, func, text = tb_info[-1]
-    print('An error occurred on line {} of function {} with statement {}'.format(line, func, text), flush=True)
+    print(f'An error occurred on line {line} of function {func} with statement {text}', flush=True)
 
     # PETSc/TAO errors are printed in the following manner:
     if hasattr(e, '_traceback_'):
         print('The error was:')
         for i in e._traceback_:
             print(i, flush=True)
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_aposmm.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_aposmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 from math import log, pi, sqrt
 from mpmath import gamma
 from libensemble.gen_funcs.aposmm_localopt_support import LocalOptInterfacer, ConvergedMsg, simulate_recv_from_manager
 
 from libensemble.message_numbers import STOP_TAG, PERSIS_STOP, FINISHED_PERSISTENT_GEN_TAG, EVAL_GEN_TAG
 from libensemble.tools.persistent_support import PersistentSupport
 
-import multiprocessing
-
 
 def aposmm(H, persis_info, gen_specs, libE_info):
     """
     APOSMM coordinates multiple local optimization runs, starting from points
     which do not have a better point nearby (within a distance ``r_k``). This
     generation function uses a ``local_H`` (serving a similar purpose as ``H``
     in libEnsemble) containing the fields:
@@ -139,19 +137,14 @@
     persis_info['total_runs']: Running count of started/completed localopt runs
     persis_info['run_order']: Sequence of indices of points in unfinished runs
     persis_info['old_runs']: Sequence of indices of points in finished runs
 
     """
 
     try:
-
-        if multiprocessing.get_start_method() != "fork":
-            print("[APOSMM]: Detected multiprocessing start method is currently known to cause slowdowns. This will be fixed in a future release.")
-            print("[APOSMM]: Set the multiprocessing start method to 'fork' in your calling script to resolve in the meantime.")
-
         user_specs = gen_specs['user']
         ps = PersistentSupport(libE_info, EVAL_GEN_TAG)
         n, n_s, rk_const, ld, mu, nu, comm, local_H = initialize_APOSMM(H, user_specs, libE_info)
         local_opters, sim_id_to_child_inds, run_order, run_pts, total_runs, fields_to_pass = initialize_children(user_specs)
         if user_specs['initial_sample_size'] != 0:
             # Send our initial sample. We don't need to check that n_s is large enough:
             # the alloc_func only returns when the initial sample has function values.
@@ -423,18 +416,18 @@
         print("[APOSMM] Dist from reported x_opt to closest evaluated point is: " + str(dists[ind]) + "\n" +
               "[APOSMM] Check that the local optimizer is working correctly\n", x_opt, run_inds, flush=True)
 
     tol_x2 = 1e-8
     failsafe = np.logical_and(H['f'][run_inds] < H['f'][opt_ind], dists < tol_x2)
     if opt_flag:
         if np.any(failsafe):
-            print("[APOSMM] This run has {} point(s) with smaller 'f' value within {} of "
+            print(f"[APOSMM] This run has {sum(failsafe)} point(s) with smaller 'f' value within {tol_x2} of "
                   "the point ruled to be the run minimum. \nMarking all as being "
                   "a 'local_min' to prevent APOSMM from starting another run "
-                  "immediately from these points.".format(sum(failsafe), tol_x2))
+                  "immediately from these points.")
             print("[APOSMM] Sim_ids to be marked optimal: ", opt_ind, run_inds[failsafe])
             print("[APOSMM] Check that the local optimizer is working correctly", flush=True)
             H['local_min'][run_inds[failsafe]] = 1
 
         H['local_min'][opt_ind] = 1
 
     H['num_active_runs'][run_inds] -= 1
@@ -563,15 +556,14 @@
     start_inds = np.array(start_inds)[inds].tolist()
 
     return start_inds
 
 
 def calc_rk(n, n_s, rk_const, lhs_divisions=0):
     """ Calculate the critical distance r_k """
-
     if lhs_divisions == 0:
         r_k = rk_const*(log(n_s)/n_s)**(1/n)
     else:
         k = np.floor(n_s/lhs_divisions).astype(int)
         if k <= 1:  # to prevent r_k=0
             r_k = np.inf
         else:
@@ -663,15 +655,15 @@
     elif user_specs['localopt_method'] in ['LN_SBPLX', 'LN_BOBYQA', 'LN_COBYLA', 'LN_NEWUOA',
                                            'LN_NELDERMEAD', 'scipy_Nelder-Mead', 'scipy_COBYLA',
                                            'external_localopt', 'nm']:
         fields_to_pass = ['x_on_cube', 'f']
     elif user_specs['localopt_method'] in ['pounders', 'dfols']:
         fields_to_pass = ['x_on_cube', 'fvec']
     else:
-        raise NotImplementedError("Unknown local optimization method " "'{}'.".format(user_specs['localopt_method']))
+        raise NotImplementedError(f"Unknown local optimization method {user_specs['localopt_method']}.")
 
     return local_opters, sim_id_to_child_inds, run_order, run_pts, total_runs, fields_to_pass
 
 
 def add_k_sample_points_to_local_H(k, user_specs, persis_info, n, comm, local_H, sim_id_to_child_inds):
 
     if 'sample_points' in user_specs:
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_ax_multitask.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_ax_multitask.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     n_opt_lofi = gen_specs["user"]["n_opt_lofi"]
 
     # Create search space.
     parameters = []
     for i, (ub, lb) in enumerate(zip(ub_list, lb_list)):
         parameters.append(
             RangeParameter(
-                name="x{}".format(i),
+                name=f"x{i}",
                 parameter_type=ParameterType.FLOAT,
                 lower=float(lb),
                 upper=float(ub),
             )
         )
     search_space = SearchSpace(parameters=parameters)
 
@@ -206,15 +206,15 @@
 
         for i, (arm_name, arm) in enumerate(trial.arms_by_name.items()):
             # fill H_o
             params = arm.parameters
             n_param = len(params)
             param_array = np.zeros(n_param)
             for j in range(n_param):
-                param_array[j] = params["x{}".format(j)]
+                param_array[j] = params[f"x{j}"]
             H_o["x"][i] = param_array
             H_o["resource_sets"][i] = 1
             H_o["task"][i] = task
 
         tag, Work, calc_in = self.ps.send_recv(H_o)
 
         trial_metadata["tag"] = tag
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_fd_param_finder.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_fd_param_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             # [Fnoise2(i, j), ~, inform2(i, j)] = ECnoise(nf-1, Fhist0(i, j, 2:nf));
 
             # cmd = ["/home/jlarson/software/MATLAB/R2019a/bin/matlab", "-batch",
             cmd = [
                 "octave",
                 "--no-window-system",
                 "--eval",
-                "F=[" + " ".join(["{:18.18f}".format(x) for x in Fhist0[i, j, : nf + 1]]) + "];"
+                "F=[" + " ".join([f"{x:18.18f}" for x in Fhist0[i, j, : nf + 1]]) + "];"
                 "nf=" + str(nf) + "';"
                 "[fnoise, ~, inform] = ECnoise(nf+1, F);"
                 "dlmwrite('fnoise.out', fnoise, 'delimiter', ' ', 'precision', 16);"
                 "dlmwrite('inform.out', inform, 'delimiter', ' ', 'precision', 16);"
                 "exit",
             ]
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_gp.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_gp.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_independent_optimize.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_independent_optimize.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 "norm": np.inf,
                 "maxiter": None,
             },
         )
         print_final_score(res.x, f_i_idxs, gen_specs, libE_info)
 
         start_pt, end_pt = f_i_idxs[0], f_i_idxs[-1]
-        print("[Worker {}]: x={}".format(persis_info["worker_num"], res.x[2 * start_pt : 2 * end_pt]), flush=True)
+        print(f"[Worker {persis_info['worker_num']}]: x={res.x[2 * start_pt:2 * end_pt]}", flush=True)
         """
         try:
            res = sciopt.minimize(_f, x0, jac=_df, method="BFGS", tol=eps,
                                   options={'gtol': eps, 'norm': np.inf, 'maxiter': None})
            print_final_score(res.x, f_i_idxs, gen_specs, libE_info)
 
         except:
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_inverse_bayes.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_inverse_bayes.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_n_agent.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_n_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     A_i_gen_ids = A_i_gen_ids[_perm_ids]
     A_i_gen_ids_no_local = np.delete(A_i_gen_ids, np.where(A_i_gen_ids == local_gen_id)[0][0])
 
     prev_s_is = np.zeros((len(A_i_data), n), dtype=float)
     prev_gradf_is = np.zeros((len(A_i_data), n), dtype=float)
 
     if local_gen_id == 1:
-        print("[{}%]: ".format(0), flush=True, end="")
+        print(f"[{0}%]: ", flush=True, end="")
     print_final_score(x_k, f_i_idxs, gen_specs, libE_info)
     percent = 0.1
 
     for k in range(N):
         tag, gradf = get_grad(x_k, f_i_idxs, gen_specs, libE_info)
         if tag in [STOP_TAG, PERSIS_STOP]:
             return None, persis_info, FINISHED_PERSISTENT_GEN_TAG
@@ -77,12 +77,12 @@
 
         # Save data to avoid more communication
         prev_s_is = neighbor_s_is
         prev_gradf_is = neighbor_gradf_is
 
         if (k + 1) / N >= percent:
             if local_gen_id == 1:
-                print("[{}%]: ".format(int(percent * 100)), flush=True, end="")
+                print(f"[{int(percent * 100)}%]: ", flush=True, end="")
             percent += 0.1
             print_final_score(x_k, f_i_idxs, gen_specs, libE_info)
 
     return None, persis_info, FINISHED_PERSISTENT_GEN_TAG
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_pds.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_pds.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     weighted_x_hk_sum = np.zeros(len(x_0), dtype=float)
     b_k_sum = 0
 
     prev_b_k = 0
     prev_T_k = 0
 
     if local_gen_id == 1:
-        print("[{}%]: ".format(0), flush=True, end="")
+        print(f"[{0}%]: ", flush=True, end="")
     print_final_score(prev_x_k, f_i_idxs, gen_specs, libE_info)
     percent = 0.1
 
     for k in range(1, N + 1):
         tau_k = (k - 1) / 2
         lam_k = (k - 1) / k
         b_k = k
@@ -114,15 +114,15 @@
 
         weighted_x_hk_sum += b_k * x_hk
         b_k_sum += b_k
 
         if k / N >= percent:
             curr_x_star = 1.0 / b_k_sum * weighted_x_hk_sum
             if local_gen_id == 1:
-                print("[{}%]: ".format(int(percent * 100)), flush=True, end="")
+                print(f"[{int(percent * 100)}%]: ", flush=True, end="")
             percent += 0.1
             print_final_score(curr_x_star, f_i_idxs, gen_specs, libE_info)
 
     return None, persis_info, FINISHED_PERSISTENT_GEN_TAG
 
 
 def primaldual_slide(y_k, x_curr, x_prev, z_t, settings, gen_specs, libE_info):
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_prox_slide.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_prox_slide.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     lam_max = persis_info["params"]["lam_max"]
     df_i_eval = persis_info["params"].get("df_i_eval", None)
 
     L = 2 * R * lam_max
     N = N_const * int(((L * D) / (nu * eps)) ** 0.5 + 1)
 
     if local_gen_id == 1:
-        print("[{}%]: ".format(0), flush=True, end="")
+        print(f"[{0}%]: ", flush=True, end="")
     print_final_score(x_k, f_i_idxs, gen_specs, libE_info)
     percent = 0.1
 
     for k in range(1, N + 1):
         b_k = 2.0 * L / (nu * k)
         g_k = 2.0 / (k + 1)
         T_k = int((N * ((M * k) ** 2)) / (D * (L**2)) + 1)
@@ -68,15 +68,15 @@
         if tag in [STOP_TAG, PERSIS_STOP]:
             return None, persis_info, FINISHED_PERSISTENT_GEN_TAG
 
         post_x_k = (1.0 - g_k) * post_x_k + (g_k * x2_k)
 
         if k / N >= percent:
             if local_gen_id == 1:
-                print("[{}%]: ".format(int(percent * 100)), flush=True, end="")
+                print(f"[{int(percent * 100)}%]: ", flush=True, end="")
             percent += 0.1
             print_final_score(post_x_k, f_i_idxs, gen_specs, libE_info)
 
     return None, persis_info, FINISHED_PERSISTENT_GEN_TAG
 
 
 def PS(x, gradg, beta, T, f_i_idxs, gen_specs, libE_info, pre_x_k, df_i_eval):
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_sampling.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_sampling.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from libensemble.message_numbers import STOP_TAG, PERSIS_STOP, FINISHED_PERSISTENT_GEN_TAG, EVAL_GEN_TAG
 from libensemble.tools.persistent_support import PersistentSupport
 
 __all__ = [
     "persistent_uniform",
     "uniform_random_sample_with_variable_resources",
     "persistent_request_shutdown",
+    "uniform_nonblocking",
     "batched_history_matching",
+    "persistent_uniform_with_cancellations",
 ]
 
 
 def persistent_uniform(H, persis_info, gen_specs, libE_info):
     """
     This generation function always enters into persistent mode and returns
     ``gen_specs['initial_batch_size']`` uniformly sampled points the first time it
@@ -75,15 +77,15 @@
     tag, Work, calc_in = ps.send_recv(H_o)
     while tag not in [STOP_TAG, PERSIS_STOP]:
         H_o = np.zeros(b, dtype=gen_specs["out"])
         # H_o['x'] = len(H)*np.ones(n)
         H_o["x"] = persis_info["rand_stream"].uniform(lb, ub, (b, n))
         H_o["resource_sets"] = persis_info["rand_stream"].integers(1, gen_specs["user"]["max_resource_sets"] + 1, b)
         H_o["priority"] = 10 * H_o["resource_sets"]
-        print("Created {} sims, with worker_teams req. of size(s) {}".format(b, H_o["resource_sets"]), flush=True)
+        print(f"Created {b} sims, with worker_teams req. of size(s) {H_o['resource_sets']}", flush=True)
         tag, Work, calc_in = ps.send_recv(H_o)
 
         if calc_in is not None:
             b = len(calc_in)
 
     return H_o, persis_info, FINISHED_PERSISTENT_GEN_TAG
 
@@ -200,7 +202,38 @@
         if calc_in is not None:
             all_inds = np.argsort(calc_in["f"])
             best_inds = all_inds[:q]
             mu = np.mean(H_o["x"][best_inds], axis=0)
             Sigma = np.cov(H_o["x"][best_inds].T)
 
     return H_o, persis_info, FINISHED_PERSISTENT_GEN_TAG
+
+
+def persistent_uniform_with_cancellations(H, persis_info, gen_specs, libE_info):
+
+    ub = gen_specs["user"]["ub"]
+    lb = gen_specs["user"]["lb"]
+    n = len(lb)
+    b = gen_specs["user"]["initial_batch_size"]
+
+    # Start cancelling points from half initial batch onward
+    cancel_from = b // 2  # Should get at least this many points back
+
+    ps = PersistentSupport(libE_info, EVAL_GEN_TAG)
+
+    # Send batches until manager sends stop tag
+    tag = None
+    while tag not in [STOP_TAG, PERSIS_STOP]:
+
+        H_o = np.zeros(b, dtype=gen_specs["out"])
+        H_o["x"] = persis_info["rand_stream"].uniform(lb, ub, (b, n))
+        tag, Work, calc_in = ps.send_recv(H_o)
+
+        if hasattr(calc_in, "__len__"):
+            b = len(calc_in)
+
+            # Cancel as many points as got back
+            cancel_ids = list(range(cancel_from, cancel_from + b))
+            cancel_from += b
+            ps.request_cancel_sim_ids(cancel_ids)
+
+    return H_o, persis_info, FINISHED_PERSISTENT_GEN_TAG
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_surmise_calib.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_surmise_calib.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,19 +93,15 @@
         col_offset = c * n_x
         for i in range(n_x):
             sim_id_cancel = obs_offset + col_offset + i
             if pending[i, c]:
                 sim_ids_to_cancel.append(sim_id_cancel)
                 pending[i, c] = 0
 
-    # Send only these fields to existing H rows and libEnsemble will slot in the change.
-    H_o = np.zeros(len(sim_ids_to_cancel), dtype=[("sim_id", int), ("cancel_requested", bool)])
-    H_o["sim_id"] = sim_ids_to_cancel
-    H_o["cancel_requested"] = True
-    ps.send(H_o)
+    ps.request_cancel_sim_ids(sim_ids_to_cancel)
 
 
 def assign_priority(n_x, n_thetas):
     """Assign priorities to points."""
     # Arbitrary priorities
     priority = np.arange(n_x * n_thetas)
     np.random.shuffle(priority)
@@ -238,12 +234,12 @@
             H_o = np.zeros(n_x * (len(new_theta)), dtype=gen_specs["out"])
             load_H(H_o, x, new_theta, set_priorities=True)
             tag, Work, calc_in = ps.send_recv(H_o)
 
             # Determine evaluations to cancel
             c_obviate = info["obviatesugg"]
             if len(c_obviate) > 0:
-                print("columns sent for cancel is:  {}".format(c_obviate), flush=True)
+                print(f"columns sent for cancel is:  {c_obviate}", flush=True)
                 cancel_columns(obs_offset, c_obviate, n_x, pending, ps)
             pending[:, c_obviate] = False
 
     return None, persis_info, FINISHED_PERSISTENT_GEN_TAG
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/persistent_tasmanian.py` & `libensemble-0.9.3/libensemble/gen_funcs/persistent_tasmanian.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         "getAnisotropicRefinement",
         "setSurplusRefinement",
         "getSurplusRefinement",
         "none",
     ]
     assert (
         "refinement" in U and U["refinement"] in allowed_refinements
-    ), "Must provide a gen_specs['user']['refinement'] in: {}".format(allowed_refinements)
+    ), f"Must provide a gen_specs['user']['refinement'] in: {allowed_refinements}"
 
     while grid.getNumNeeded() > 0:
         aPoints = grid.getNeededPoints()
 
         H0 = np.zeros(len(aPoints), dtype=gen_specs["out"])
         H0["x"] = aPoints
 
@@ -206,15 +206,15 @@
     """
     U = gen_specs["user"]
     ps = PersistentSupport(libE_info, EVAL_GEN_TAG)
     grid = U["tasmanian_init"]()  # initialize the grid
     allowed_refinements = ["getCandidateConstructionPoints", "getCandidateConstructionPointsSurplus"]
     assert (
         "refinement" in U and U["refinement"] in allowed_refinements
-    ), "Must provide a gen_specs['user']['refinement'] in: {}".format(allowed_refinements)
+    ), f"Must provide a gen_specs['user']['refinement'] in: {allowed_refinements}"
     tol = U["_match_tolerance"] if "_match_tolerance" in U else 1.0e-12
 
     # Choose the refinement function based on U['refinement'].
     if U["refinement"] == "getCandidateConstructionPoints":
         assert "sType" in U
         assert "liAnisotropicWeightsOrOutput" in U
     if U["refinement"] == "getCandidateConstructionPointsSurplus":
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/sampling.py` & `libensemble-0.9.3/libensemble/gen_funcs/sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/surmise_calib_support.py` & `libensemble-0.9.3/libensemble/gen_funcs/surmise_calib_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Contains supplemental methods for gen function in persistent_surmise_calib.py."""
-
 import numpy as np
 import scipy.stats as sps
 
 
 class thetaprior:
     """Define the class instance of priors provided to the methods."""
```

### Comparing `libensemble-0.9.2/libensemble/gen_funcs/uniform_or_localopt.py` & `libensemble-0.9.3/libensemble/gen_funcs/uniform_or_localopt.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/history.py` & `libensemble-0.9.3/libensemble/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             self.H["sim_id"][self.index : self.index + num_new] = range(self.index, self.index + num_new)
         else:
             # gen method is building sim_id or adjusting values in existing sim_id rows.
 
             # Ensure there aren't any gaps in the generated sim_id values:
             assert np.all(
                 np.in1d(np.arange(self.index, np.max(D["sim_id"]) + 1), D["sim_id"])
-            ), "The generator function has produced sim_id that are not in order."
+            ), "The generator function has produced sim_ids that are not in order."
 
             num_new = len(np.setdiff1d(D["sim_id"], self.H["sim_id"]))
 
             if num_new > rows_remaining:
                 self.grow_count = max(num_new - rows_remaining, 2 * self.grow_count)
                 self.grow_H(self.grow_count)
```

### Comparing `libensemble-0.9.2/libensemble/information_about_W` & `libensemble-0.9.3/libensemble/information_about_W`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/libE.py` & `libensemble-0.9.3/libensemble/libE.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             - x
         outputs:
             y:
                 type: float
 
 On macOS (since Python 3.8) and Windows, the default multiprocessing start method is ``'spawn'``
 and you must place most calling script code (or just ``libE()`` / ``Ensemble().run()`` at a minimum) in
-an ``if __name__ == "__main__:" block.
+an ``if __name__ == "__main__:"`` block.
 
 Therefore a calling script that is universal across
 all platforms and comms-types may resemble:
 
 .. code-block:: python
     :linenos:
 
@@ -138,15 +138,15 @@
         persis_info = add_unique_random_streams({}, nworkers+1)
 
         exit_criteria = {"sim_max": 80}
 
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info,
                                     libE_specs=libE_specs)
 
-Alternatively, you may set the multiprocesing start method to ``'fork'`` via the following:
+Alternatively, you may set the multiprocessing start method to ``'fork'`` via the following:
 
     from multiprocessing import set_start_method
     set_start_method("fork")
 
 But note that this is incompatible with some libraries.
 
 See below for the complete traditional ``libE()`` API.
@@ -266,15 +266,15 @@
     if "comms" not in libE_specs:
         libE_specs["comms"] = "mpi"
 
     libE_funcs = {"mpi": libE_mpi, "tcp": libE_tcp, "local": libE_local}
 
     comms_type = libE_specs.get("comms")
 
-    assert comms_type in libE_funcs, "Unknown comms type: {}".format(comms_type)
+    assert comms_type in libE_funcs, f"Unknown comms type: {comms_type}"
 
     # Resource management not supported with TCP
     if comms_type == "tcp":
         libE_specs["disable_resource_manager"] = True
 
     Resources.init_resources(libE_specs)
 
@@ -293,29 +293,29 @@
     alloc_specs,
     libE_specs,
     hist,
     on_abort=None,
     on_cleanup=None,
 ):
     """Generic manager routine run."""
-
     logger.info("Logger initializing: [workerID] precedes each line. [0] = Manager")
-    logger.info("libE version v{}".format(__version__))
+    logger.info(f"libE version v{__version__}")
 
     if "out" in gen_specs and ("sim_id", int) in gen_specs["out"]:
-        logger.manager_warning(_USER_SIM_ID_WARNING)
+        if "libensemble.gen_funcs" not in gen_specs["gen_f"].__module__:
+            logger.manager_warning(_USER_SIM_ID_WARNING)
 
     save_H = libE_specs.get("save_H_and_persis_on_abort", True)
 
     try:
         try:
             persis_info, exit_flag, elapsed_time = manager_main(
                 hist, libE_specs, alloc_specs, sim_specs, gen_specs, exit_criteria, persis_info, wcomms
             )
-            logger.info("Manager total time: {}".format(elapsed_time))
+            logger.info(f"Manager total time: {elapsed_time}")
         except LoggedException:
             # Exception already logged in manager
             raise
         except WorkerException as e:
             report_worker_exc(e)
             raise LoggedException(e.args[0], e.args[1]) from None
         except Exception as e:
@@ -326,16 +326,16 @@
         _dump_on_abort(hist, persis_info, save_H=save_H)
         if libE_specs.get("abort_on_exception", True) and on_abort is not None:
             on_cleanup()
             on_abort()
         raise LoggedException(*e.args, "See error details above and in ensemble.log") from None
     else:
         logger.debug("Manager exiting")
-        logger.debug("Exiting with {} workers.".format(len(wcomms)))
-        logger.debug("Exiting with exit criteria: {}".format(exit_criteria))
+        logger.debug(f"Exiting with {len(wcomms)} workers.")
+        logger.debug(f"Exiting with exit criteria: {exit_criteria}")
     finally:
         if on_cleanup is not None:
             on_cleanup()
 
     H = hist.trim_H()
     return H, persis_info, exit_flag
 
@@ -360,26 +360,24 @@
 def comms_abort(mpi_comm):
     """Abort all MPI ranks"""
     mpi_comm.Abort(1)  # Exit code 1 to represent an abort
 
 
 def libE_mpi_defaults(libE_specs):
     """Fill in default values for MPI-based communicators."""
-
     from mpi4py import MPI
 
     if "mpi_comm" not in libE_specs:
         libE_specs["mpi_comm"] = MPI.COMM_WORLD  # Will be duplicated immediately
 
     return libE_specs, MPI.COMM_NULL
 
 
 def libE_mpi(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs, H0):
     """MPI version of the libE main routine"""
-
     libE_specs, mpi_comm_null = libE_mpi_defaults(libE_specs)
 
     if libE_specs["mpi_comm"] == mpi_comm_null:
         return [], persis_info, 3  # Process not in mpi_comm
 
     check_inputs(libE_specs, alloc_specs, sim_specs, gen_specs, exit_criteria, H0)
 
@@ -411,15 +409,14 @@
         # Worker returns a subset of MPI output
         libE_mpi_worker(mpi_comm, sim_specs, gen_specs, libE_specs)
         return [], {}, []
 
 
 def libE_mpi_manager(mpi_comm, sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs, H0):
     """Manager routine runs on rank 0."""
-
     from libensemble.comms.mpi import MainMPIComm
 
     hist = History(alloc_specs, sim_specs, gen_specs, exit_criteria, H0)
 
     # Launch worker team
     wcomms = [MainMPIComm(mpi_comm, w) for w in range(1, mpi_comm.Get_size())]
 
@@ -451,28 +448,26 @@
         on_abort=on_abort,
         on_cleanup=cleanup,
     )
 
 
 def libE_mpi_worker(libE_comm, sim_specs, gen_specs, libE_specs):
     """Worker routines run on ranks > 0."""
-
     from libensemble.comms.mpi import MainMPIComm
 
     comm = MainMPIComm(libE_comm)
     worker_main(comm, sim_specs, gen_specs, libE_specs, log_comm=True)
-    logger.debug("Worker {} exiting".format(libE_comm.Get_rank()))
+    logger.debug(f"Worker {libE_comm.Get_rank()} exiting")
 
 
 # ==================== Local version ===============================
 
 
 def start_proc_team(nworkers, sim_specs, gen_specs, libE_specs, log_comm=True):
     """Launch a process worker team."""
-
     resources = Resources.resources
     executor = Executor.executor
 
     wcomms = [
         QCommProcess(worker_main, nworkers, sim_specs, gen_specs, libE_specs, w, log_comm, resources, executor)
         for w in range(1, nworkers + 1)
     ]
@@ -489,15 +484,14 @@
             wcomm.result(timeout=timeout)
         except Timeout:
             wcomm.terminate()
 
 
 def libE_local(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs, H0):
     """Main routine for thread/process launch of libE."""
-
     nworkers = libE_specs["nworkers"]
 
     check_inputs(libE_specs, alloc_specs, sim_specs, gen_specs, exit_criteria, H0)
 
     resources = Resources.resources
     if resources is not None:
         local_host = [socket.gethostname()]
@@ -545,25 +539,24 @@
     except socket.gaierror:
         return "localhost"
 
 
 def libE_tcp_authkey():
     """Generate an authkey if not assigned by manager."""
     nonce = random.randrange(99999)
-    return "libE_auth_{}".format(nonce)
+    return f"libE_auth_{nonce}"
 
 
 def libE_tcp_default_ID():
     """Assign a (we hope unique) worker ID if not assigned by manager."""
-    return "{}_pid{}".format(get_ip(), os.getpid())
+    return f"{get_ip()}_pid{os.getpid()}"
 
 
 def libE_tcp(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs, H0):
     """Main routine for TCP multiprocessing launch of libE."""
-
     check_inputs(libE_specs, alloc_specs, sim_specs, gen_specs, exit_criteria, H0)
 
     is_worker = True if "workerID" in libE_specs else False
 
     exctr = Executor.executor
     if exctr is not None:
         # TCP does not currently support resource_management but when does, assume
@@ -594,29 +587,28 @@
 
 def libE_tcp_start_team(manager, nworkers, workers, ip, port, authkey, launchf):
     """Launch nworkers workers that attach back to a managers server."""
     worker_procs = []
     specs = {"manager_ip": ip, "manager_port": port, "authkey": authkey}
     with Timer() as timer:
         for w in range(1, nworkers + 1):
-            logger.info("Manager is launching worker {}".format(w))
+            logger.info(f"Manager is launching worker {w}")
             if workers is not None:
                 specs["worker_ip"] = workers[w - 1]
                 specs["tunnel_port"] = 0x71BE
             specs["workerID"] = w
             worker_procs.append(launchf(specs))
-        logger.info("Manager is awaiting {} workers".format(nworkers))
+        logger.info(f"Manager is awaiting {nworkers} workers")
         wcomms = manager.await_workers(nworkers)
-        logger.info("Manager connected to {} workers ({} s)".format(nworkers, timer.elapsed))
+        logger.info(f"Manager connected to {nworkers} workers ({timer.elapsed} s)")
     return worker_procs, wcomms
 
 
 def libE_tcp_mgr(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs, H0):
     """Main routine for TCP multiprocessing launch of libE at manager."""
-
     hist = History(alloc_specs, sim_specs, gen_specs, exit_criteria, H0)
 
     # Set up a worker launcher
     launchf = libE_tcp_worker_launcher(libE_specs)
 
     # Get worker launch parameters and fill in defaults for TCP/IP conn
     if "nworkers" in libE_specs:
@@ -636,15 +628,15 @@
             _, port = tcp_manager.address
 
         if not libE_specs.get("disable_log_files", False):
             exit_logger = manager_logging_config()
         else:
             exit_logger = None
 
-        logger.info("Launched server at ({}, {})".format(ip, port))
+        logger.info(f"Launched server at ({ip}, {port})")
 
         # Launch worker team and set up logger
         worker_procs, wcomms = libE_tcp_start_team(tcp_manager, nworkers, workers, ip, port, authkey, launchf)
 
         def cleanup():
             """Handler to clean up launched team."""
             for wp in worker_procs:
@@ -656,30 +648,29 @@
         return manager(
             wcomms, sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs, hist, on_cleanup=cleanup
         )
 
 
 def libE_tcp_worker(sim_specs, gen_specs, libE_specs):
     """Main routine for TCP worker launched by libE."""
-
     ip = libE_specs["ip"]
     port = libE_specs["port"]
     authkey = libE_specs["authkey"]
     workerID = libE_specs["workerID"]
 
     with ClientQCommManager(ip, port, authkey, workerID) as comm:
         worker_main(comm, sim_specs, gen_specs, libE_specs, workerID=workerID, log_comm=True)
-        logger.debug("Worker {} exiting".format(workerID))
+        logger.debug(f"Worker {workerID} exiting")
 
 
 # ==================== Additional Internal Functions ===========================
 
 
 def _dump_on_abort(hist, persis_info, save_H=True):
     """Dump history and persis_info on abort"""
     logger.error("Manager exception raised .. aborting ensemble:")
-    logger.error("Dumping ensemble history with {} sims evaluated:".format(hist.sim_ended_count))
+    logger.error(f"Dumping ensemble history with {hist.sim_ended_count} sims evaluated:")
 
     if save_H:
         np.save("libE_history_at_abort_" + str(hist.sim_ended_count) + ".npy", hist.trim_H())
         with open("libE_persis_info_at_abort_" + str(hist.sim_ended_count) + ".pickle", "wb") as f:
             pickle.dump(persis_info, f)
```

### Comparing `libensemble-0.9.2/libensemble/logger.py` & `libensemble-0.9.3/libensemble/logger.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/manager.py` & `libensemble-0.9.3/libensemble/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 """
 
 import sys
 import os
 import glob
 import logging
 import socket
+import platform
 import traceback
 import numpy as np
 
 from libensemble.utils.timer import Timer
+from libensemble.utils.misc import extract_H_ranges
 
 from libensemble.message_numbers import (
     EVAL_SIM_TAG,
     EVAL_GEN_TAG,
     PERSIS_STOP,
     STOP_TAG,
     MAN_SIGNAL_FINISH,
@@ -58,16 +60,16 @@
     """Raise exception for handling without re-logging"""
 
 
 def report_worker_exc(wrk_exc=None):
     """Write worker exception to log"""
     if wrk_exc is not None:
         from_line, msg, exc = wrk_exc.args
-        logger.error("---- {} ----".format(from_line))
-        logger.error("Message: {}".format(msg))
+        logger.error(f"---- {from_line} ----")
+        logger.error(f"Message: {msg}")
         logger.error(exc)
 
 
 def manager_main(hist, libE_specs, alloc_specs, sim_specs, gen_specs, exit_criteria, persis_info, wcomms=[]):
     """Manager routine to coordinate the generation and simulation evaluations
 
     Parameters
@@ -230,15 +232,15 @@
 
     def term_test(self, logged=True):
         """Checks termination criteria"""
         for retval, key, testf in self.term_tests:
             if key in self.exit_criteria:
                 if testf(self.exit_criteria[key]):
                     if logged:
-                        logger.info("Term test tripped: {}".format(key))
+                        logger.info(f"Term test tripped: {key}")
                     return retval
         return 0
 
     # --- Low-level communication routines
 
     def _kill_workers(self):
         """Kills the workers"""
@@ -247,14 +249,16 @@
 
     # --- Checkpointing logic
 
     def _save_every_k(self, fname, count, k):
         """Saves history every kth step"""
         count = k * (count // k)
         filename = fname.format(self.date_start, count)
+        if platform.system() == "Windows":
+            filename = filename.replace(":", "-")  # ":" is invalid in windows filenames
         if not os.path.isfile(filename) and count > 0:
             for old_file in glob.glob(fname.format(self.date_start, "*")):
                 os.remove(old_file)
             np.save(filename, self.hist.H)
 
     def _save_every_k_sims(self):
         """Saves history every kth sim step"""
@@ -276,34 +280,32 @@
 
     def _check_work_order(self, Work, w):
         """Checks validity of an allocation function order"""
         assert w != 0, "Can't send to worker 0; this is the manager."
         if self.W[w - 1]["active_recv"]:
             assert "active_recv" in Work["libE_info"], (
                 "Messages to a worker in active_recv mode should have active_recv"
-                "set to True in libE_info. Work['libE_info'] is {}".format(Work["libE_info"])
+                f"set to True in libE_info. Work['libE_info'] is {Work['libE_info']}"
             )
         else:
             assert self.W[w - 1]["active"] == 0, (
                 "Allocation function requested work be sent to worker %d, an already active worker." % w
             )
         work_rows = Work["libE_info"]["H_rows"]
         if len(work_rows):
             work_fields = set(Work["H_fields"])
 
             assert len(work_fields), (
-                "Allocation function requested rows={} be sent to worker={}, "
-                "but requested no fields to be sent.".format(work_rows, w)
+                f"Allocation function requested rows={work_rows} be sent to worker={w}, "
+                "but requested no fields to be sent."
             )
             hist_fields = self.hist.H.dtype.names
             diff_fields = list(work_fields.difference(hist_fields))
 
-            assert not diff_fields, "Allocation function requested invalid fields {} be sent to worker={}.".format(
-                diff_fields, w
-            )
+            assert not diff_fields, f"Allocation function requested invalid fields {diff_fields} be sent to worker={w}."
 
     def _set_resources(self, Work, w):
         """Check rsets given in Work match rsets assigned in resources.
 
         If rsets are not assigned, then assign using default mapping
         """
         resource_manager = self.resources.resource_manager
@@ -316,52 +318,45 @@
                 rset_team.append(default_rset)
             Work["libE_info"]["rset_team"] = rset_team
 
         resource_manager.assign_rsets(Work["libE_info"]["rset_team"], w)
 
     def _freeup_resources(self, w):
         """Free up resources assigned to the worker"""
-
         if self.resources:
             self.resources.resource_manager.free_rsets(w)
 
     def _send_work_order(self, Work, w):
         """Sends an allocation function order to a worker"""
-
-        logger.debug("Manager sending work unit to worker {}".format(w))
+        logger.debug(f"Manager sending work unit to worker {w}")
 
         if self.resources:
             self._set_resources(Work, w)
 
         self.wcomms[w - 1].send(Work["tag"], Work)
 
         if Work["tag"] == EVAL_GEN_TAG:
             self.W[w - 1]["gen_started_time"] = time.time()
 
         work_rows = Work["libE_info"]["H_rows"]
         work_name = calc_type_strings[Work["tag"]]
-        logger.debug(
-            "Manager sending {} work to worker {}. Rows {}".format(
-                work_name, w, EnsembleDirectory.extract_H_ranges(Work) or None
-            )
-        )
+        logger.debug(f"Manager sending {work_name} work to worker {w}. Rows {extract_H_ranges(Work) or None}")
         if len(work_rows):
             if "repack_fields" in globals():
                 new_dtype = [(name, self.hist.H.dtype.fields[name][0]) for name in Work["H_fields"]]
                 H_to_be_sent = np.empty(len(work_rows), dtype=new_dtype)
                 for i, row in enumerate(work_rows):
                     H_to_be_sent[i] = repack_fields(self.hist.H[Work["H_fields"]][row])
                 # H_to_be_sent = repack_fields(self.hist.H[Work['H_fields']])[work_rows]
                 self.wcomms[w - 1].send(0, H_to_be_sent)
             else:
                 self.wcomms[w - 1].send(0, self.hist.H[Work["H_fields"]][work_rows])
 
     def _update_state_on_alloc(self, Work, w):
         """Updates a workers' active/idle status following an allocation order"""
-
         self.W[w - 1]["active"] = Work["tag"]
         if "libE_info" in Work:
             if "persistent" in Work["libE_info"]:
                 self.W[w - 1]["persis_state"] = Work["tag"]
                 if Work["libE_info"].get("active_recv", False):
                     self.W[w - 1]["active_recv"] = Work["tag"]
             else:
@@ -379,19 +374,19 @@
     def _check_received_calc(D_recv):
         """Checks the type and status fields on a receive calculation"""
         calc_type = D_recv["calc_type"]
         calc_status = D_recv["calc_status"]
         assert calc_type in [
             EVAL_SIM_TAG,
             EVAL_GEN_TAG,
-        ], "Aborting, Unknown calculation type received. Received type: {}".format(calc_type)
+        ], f"Aborting, Unknown calculation type received. Received type: {calc_type}"
 
         assert calc_status in list(calc_status_strings.keys()) + [PERSIS_STOP] or isinstance(
             calc_status, str
-        ), "Aborting: Unknown calculation status received. Received status: {}".format(calc_status)
+        ), f"Aborting: Unknown calculation status received. Received status: {calc_status}"
 
     def _receive_from_workers(self, persis_info):
         """Receives calculation output from workers. Loops over all
         active workers and probes to see if worker is ready to
         communticate. If any output is received, all other workers are
         looped back over.
         """
@@ -411,15 +406,16 @@
 
     def _update_state_on_worker_msg(self, persis_info, D_recv, w):
         """Updates history and worker info on worker message"""
         calc_type = D_recv["calc_type"]
         calc_status = D_recv["calc_status"]
         Manager._check_received_calc(D_recv)
 
-        if w not in self.persis_pending and not self.W[w - 1]["active_recv"]:
+        keep_state = D_recv["libE_info"].get("keep_state", False)
+        if w not in self.persis_pending and not self.W[w - 1]["active_recv"] and not keep_state:
             self.W[w - 1]["active"] = 0
 
         if calc_status in [FINISHED_PERSISTENT_SIM_TAG, FINISHED_PERSISTENT_GEN_TAG]:
             final_data = D_recv.get("calc_out", None)
             if isinstance(final_data, np.ndarray):
                 if calc_status is FINISHED_PERSISTENT_GEN_TAG and self.libE_specs.get("use_persis_return_gen", False):
                     self.hist.update_history_x_in(w, final_data, self.safe_mode, self.W[w - 1]["gen_started_time"])
@@ -454,43 +450,43 @@
 
     def _handle_msg_from_worker(self, persis_info, w):
         """Handles a message from worker w"""
         try:
             msg = self.wcomms[w - 1].recv()
             tag, D_recv = msg
         except CommFinishedException:
-            logger.debug("Finalizing message from Worker {}".format(w))
+            logger.debug(f"Finalizing message from Worker {w}")
             return
         if isinstance(D_recv, WorkerErrMsg):
             self.W[w - 1]["active"] = 0
-            logger.debug("Manager received exception from worker {}".format(w))
+            logger.debug(f"Manager received exception from worker {w}")
             if not self.WorkerExc:
                 self.WorkerExc = True
                 self._kill_workers()
-                raise WorkerException("Received error message from worker {}".format(w), D_recv.msg, D_recv.exc)
+                raise WorkerException(f"Received error message from worker {w}", D_recv.msg, D_recv.exc)
         elif isinstance(D_recv, logging.LogRecord):
-            logger.debug("Manager received a log message from worker {}".format(w))
+            logger.debug(f"Manager received a log message from worker {w}")
             logging.getLogger(D_recv.name).handle(D_recv)
         else:
-            logger.debug("Manager received data message from worker {}".format(w))
+            logger.debug(f"Manager received data message from worker {w}")
             self._update_state_on_worker_msg(persis_info, D_recv, w)
 
     def _kill_cancelled_sims(self):
         """Send kill signals to any sims marked as cancel_requested"""
         if self.kill_canceled_sims:
             kill_sim = (
                 self.hist.H["sim_started"]
                 & self.hist.H["cancel_requested"]
                 & ~self.hist.H["sim_ended"]
                 & ~self.hist.H["kill_sent"]
             )
 
             # Note that a return is still expected when running sims are killed
             if np.any(kill_sim):
-                logger.debug("Manager sending kill signals to H indices {}".format(np.where(kill_sim)))
+                logger.debug(f"Manager sending kill signals to H indices {np.where(kill_sim)}")
                 kill_ids = self.hist.H["sim_id"][kill_sim]
                 kill_on_workers = self.hist.H["sim_worker"][kill_sim]
                 for w in kill_on_workers:
                     self.wcomms[w - 1].send(STOP_TAG, MAN_SIGNAL_KILL)
                     self.hist.H["kill_sent"][kill_ids] = True
 
     # --- Handle termination
@@ -503,15 +499,15 @@
         nonblocking receive is posted (though the manager will not receive this
         data) and a kill signal is sent.
         """
 
         # Send a handshake signal to each persistent worker.
         if any(self.W["persis_state"]):
             for w in self.W["worker_id"][self.W["persis_state"] > 0]:
-                logger.debug("Manager sending PERSIS_STOP to worker {}".format(w))
+                logger.debug(f"Manager sending PERSIS_STOP to worker {w}")
                 if "final_fields" in self.libE_specs:
                     rows_to_send = self.hist.trim_H()["sim_ended"]
                     fields_to_send = self.libE_specs["final_fields"]
                     H_to_send = self.hist.trim_H()[rows_to_send][fields_to_send]
                     self.wcomms[w - 1].send(PERSIS_STOP, H_to_send)
                 else:
                     self.wcomms[w - 1].send(PERSIS_STOP, MAN_SIGNAL_KILL)
@@ -543,15 +539,14 @@
         if "sim_max" in self.exit_criteria:
             return self.hist.sim_started_count >= self.exit_criteria["sim_max"] + self.hist.sim_started_offset
         else:
             return False
 
     def _get_alloc_libE_info(self):
         """Selected statistics useful for alloc_f"""
-
         return {
             "any_idle_workers": any(self.W["active"] == 0),
             "exit_criteria": self.exit_criteria,
             "elapsed_time": self.elapsed(),
             "gen_informed_count": self.hist.gen_informed_count,
             "manager_kill_canceled_sims": self.kill_canceled_sims,
             "scheduler_opts": self.libE_specs.get("scheduler_opts", {}),
@@ -594,16 +589,16 @@
         assert isinstance(output[1], dict), "Second alloc_f output must be a dictionary"
         assert output[2] in [0, 1], "Third alloc_f output must be 0 or 1."
 
         return output
 
     def run(self, persis_info):
         """Runs the manager"""
-        logger.info("Manager initiated on node {}".format(socket.gethostname()))
-        logger.info("Manager exit_criteria: {}".format(self.exit_criteria))
+        logger.info(f"Manager initiated on node {socket.gethostname()}")
+        logger.info(f"Manager exit_criteria: {self.exit_criteria}")
 
         # Continue receiving and giving until termination test is satisfied
         try:
             while not self.term_test():
                 self._kill_cancelled_sims()
                 persis_info = self._receive_from_workers(persis_info)
                 Work, persis_info, flag = self._alloc_work(self.hist.trim_H(), persis_info)
```

### Comparing `libensemble-0.9.2/libensemble/message_numbers.py` & `libensemble-0.9.3/libensemble/message_numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 WORKER_KILL_ON_ERR = 31  # Worker killed due to an error in results
 WORKER_KILL_ON_TIMEOUT = 32  # Worker killed on timeout
 TASK_FAILED = 33  # Calc had tasks that failed
 WORKER_DONE = 34  # Calculation was successful
 # last_calc_status_rst_tag
 CALC_EXCEPTION = 35  # Reserved: Automatically used if user_f raised an exception
 
+MAN_KILL_SIGNALS = [MAN_SIGNAL_FINISH, MAN_SIGNAL_KILL]
+
 calc_status_strings = {
     UNSET_TAG: "Not set",
     FINISHED_PERSISTENT_SIM_TAG: "Persis sim finished",
     FINISHED_PERSISTENT_GEN_TAG: "Persis gen finished",
     MAN_SIGNAL_FINISH: "Manager killed on finish",
     MAN_SIGNAL_KILL: "Manager killed task",
     WORKER_KILL_ON_ERR: "Worker killed task on Error",
```

### Comparing `libensemble-0.9.2/libensemble/output_directory.py` & `libensemble-0.9.3/libensemble/output_directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import re
 import shutil
-from itertools import groupby
-from operator import itemgetter
 
 from libensemble.utils.loc_stack import LocationStack
+from libensemble.utils.misc import extract_H_ranges
 from libensemble.tools.fields_keys import libE_spec_sim_dir_keys, libE_spec_gen_dir_keys, libE_spec_calc_dir_misc
 from libensemble.message_numbers import EVAL_SIM_TAG, calc_type_strings
 
 
 class EnsembleDirectory:
     """
     The EnsembleDirectory class provides methods for workers to initialize and
@@ -74,40 +73,21 @@
         except Exception:
             raise
         if self.ensemble_copy_back:
             self._make_copyback_dir()
 
     def use_calc_dirs(self, type):
         """Determines calc_dirs enabling for each calc type"""
-
         if type == EVAL_SIM_TAG:
             return self.sim_use
         else:
             return self.gen_use
 
-    @staticmethod
-    def extract_H_ranges(Work):
-        """Convert received H_rows into ranges for labeling"""
-        work_H_rows = Work["libE_info"]["H_rows"]
-        if len(work_H_rows) == 1:
-            return str(work_H_rows[0])
-        else:
-            # From https://stackoverflow.com/a/30336492
-            ranges = []
-            for diff, group in groupby(enumerate(work_H_rows.tolist()), lambda x: x[0] - x[1]):
-                group = list(map(itemgetter(1), group))
-                if len(group) > 1:
-                    ranges.append(str(group[0]) + "-" + str(group[-1]))
-                else:
-                    ranges.append(str(group[0]))
-            return "_".join(ranges)
-
     def _make_calc_dir(self, workerID, H_rows, calc_str, locs):
         """Create calc dirs and intermediate dirs, copy inputs, based on libE_specs"""
-
         if calc_str == "sim":
             input_dir = self.sim_input_dir
             do_calc_dirs = self.sim_dirs_make
             copy_files = self.sim_dir_copy_files
             symlink_files = self.sim_dir_symlink_files
         else:  # calc_str is 'gen'
             input_dir = self.gen_input_dir
@@ -155,15 +135,15 @@
             worker_path = os.path.abspath(os.path.join(self.prefix, worker_dir))
             calc_dir = calc_str + str(H_rows)
             locs.register_loc(workerID, worker_dir, prefix=self.prefix)
             calc_prefix = worker_path
 
         # Otherwise, ensemble_dir set as parent dir for sim dirs
         else:
-            calc_dir = "{}{}_worker{}".format(calc_str, H_rows, workerID)
+            calc_dir = f"{calc_str}{H_rows}_worker{workerID}"
             if not os.path.isdir(self.prefix):
                 os.makedirs(self.prefix, exist_ok=True)
             calc_prefix = self.prefix
 
         # Register calc dir with adjusted parent dir and source-file location
         locs.register_loc(
             calc_dir,
@@ -173,20 +153,19 @@
             symlink_files=symlink_files,
         )
 
         return calc_dir
 
     def prep_calc_dir(self, Work, calc_iter, workerID, calc_type):
         """Determines choice for calc_dir structure, then performs calculation."""
-
         if not self.loc_stack:
             self.loc_stack = LocationStack()
 
         if calc_type == EVAL_SIM_TAG:
-            H_rows = self.extract_H_ranges(Work)
+            H_rows = extract_H_ranges(Work)
         else:
             H_rows = str(calc_iter[calc_type])
 
         calc_str = calc_type_strings[calc_type]
 
         calc_dir = self._make_calc_dir(workerID, H_rows, calc_str, self.loc_stack)
```

### Comparing `libensemble-0.9.2/libensemble/resources/env_resources.py` & `libensemble-0.9.3/libensemble/resources/env_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 break
 
     def get_nodelist(self):
         """Returns nodelist from environment or an empty list"""
         if self.scheduler:
             env = self.scheduler
             env_var = self.nodelists[env]
-            logger.debug("{} env found - getting nodelist from {}".format(env, env_var))
+            logger.debug(f"{env} env found - getting nodelist from {env_var}")
             get_list_func = self.ndlist_funcs[env]
             global_nodelist = get_list_func(env_var)
             return global_nodelist
         return []
 
     @staticmethod
     def abbrev_nodenames(node_list, prefix=None):
```

### Comparing `libensemble-0.9.2/libensemble/resources/mpi_resources.py` & `libensemble-0.9.3/libensemble/resources/mpi_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def get_MPI_variant():
     """Returns MPI base implementation
 
     Returns
     -------
     mpi_variant: string:
-        MPI variant 'aprun' or 'jsrun' or 'mpich' or 'openmpi' or 'srun'
+        MPI variant 'aprun' or 'jsrun' or 'msmpi' or 'mpich' or 'openmpi' or 'srun'
 
     """
 
     try:
         subprocess.check_call(["aprun", "--version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         return "aprun"
     except Exception:
@@ -49,14 +49,22 @@
     try:
         subprocess.check_call(["jsrun", "--version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         return "jsrun"
     except Exception:
         pass
 
     try:
+        try_msmpi = subprocess.Popen(["mpiexec"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        stdout, _ = try_msmpi.communicate()
+        if "Microsoft" in stdout.decode():
+            return "msmpi"
+    except Exception:
+        pass
+
+    try:
         # Explore mpi4py.MPI.get_vendor() and mpi4py.MPI.Get_library_version() for mpi4py
         try_mpich = subprocess.Popen(["mpirun", "-npernode"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         stdout, _ = try_mpich.communicate()
         if "unrecognized argument npernode" in stdout.decode():
             return "mpich"
         return "openmpi"
     except Exception:
@@ -136,15 +144,15 @@
     # Advantage of cores per rset first is they will always get same no. per rset (double rsets, double cores)
     # Advantage of multiply first is less wasted cores.
     cores_avail_per_node_per_worker = cores_avail_per_node // rsets_per_node * wresources.slot_count
     # cores_avail_per_node_per_worker = int(cores_avail_per_node/rsets_per_node * wresources.slot_count)
 
     rassert(
         wresources.even_slots,
-        "Uneven distribution of node resources not yet supported. Nodes and slots are: {}".format(wresources.slots),
+        f"Uneven distribution of node resources not yet supported. Nodes and slots are: {wresources.slots}",
     )
 
     if not num_procs and not procs_per_node:
         rassert(
             cores_avail_per_node_per_worker > 0,
             "There is less than one core per resource set. "
             "Provide num_procs or num_nodes/procs_per_node to oversubsribe",
@@ -152,55 +160,55 @@
         procs_per_node = cores_avail_per_node_per_worker
         if not num_nodes:
             # If no decomposition supplied - use all available cores/nodes
             num_nodes = local_node_count
             logger.debug(
                 "No decomposition supplied - "
                 "using all available resource. "
-                "Nodes: {}  procs_per_node {}".format(num_nodes, procs_per_node)
+                f"Nodes: {num_nodes}  procs_per_node {procs_per_node}"
             )
     elif not num_nodes and not procs_per_node:
         if num_procs <= cores_avail_per_node_per_worker:
             num_nodes = 1
         else:
             num_nodes = local_node_count
     elif not num_procs and not num_nodes:
         num_nodes = local_node_count
 
     # Checks config is consistent and sufficient to express
     num_procs, num_nodes, procs_per_node = task_partition(num_procs, num_nodes, procs_per_node)
 
     rassert(
         num_nodes <= local_node_count,
-        "Not enough nodes to honor arguments. " "Requested {}. Only {} available".format(num_nodes, local_node_count),
+        "Not enough nodes to honor arguments. " f"Requested {num_nodes}. Only {local_node_count} available",
     )
 
     if gresources.enforce_worker_core_bounds:
         rassert(
             procs_per_node <= cores_avail_per_node,
             "Not enough processors on a node to honor arguments. "
-            "Requested {}. Only {} available".format(procs_per_node, cores_avail_per_node),
+            f"Requested {procs_per_node}. Only {cores_avail_per_node} available",
         )
 
         rassert(
             procs_per_node <= cores_avail_per_node_per_worker,
             "Not enough processors per worker to honor arguments. "
-            "Requested {}. Only {} available".format(procs_per_node, cores_avail_per_node_per_worker),
+            f"Requested {procs_per_node}. Only {cores_avail_per_node_per_worker} available",
         )
 
         rassert(
             num_procs <= (cores_avail_per_node * local_node_count),
             "Not enough procs to honor arguments. "
-            "Requested {}. Only {} available".format(num_procs, cores_avail_per_node * local_node_count),
+            f"Requested {num_procs}. Only {cores_avail_per_node * local_node_count} available",
         )
 
     if num_nodes < local_node_count:
         logger.warning(
             "User constraints mean fewer nodes being used "
-            "than available. {} nodes used. {} nodes available".format(num_nodes, local_node_count)
+            f"than available. {num_nodes} nodes used. {local_node_count} nodes available"
         )
 
     return num_procs, num_nodes, procs_per_node
 
 
 def create_machinefile(
     resources, machinefile=None, num_procs=None, num_nodes=None, procs_per_node=None, hyperthreads=False
@@ -210,18 +218,18 @@
     """
 
     machinefile = machinefile or "machinefile"
     if os.path.isfile(machinefile):
         try:
             os.remove(machinefile)
         except Exception as e:
-            logger.warning("Could not remove existing machinefile: {}".format(e))
+            logger.warning(f"Could not remove existing machinefile: {e}")
 
     node_list = resources.worker_resources.local_nodelist
-    logger.debug("Creating machinefile with {} nodes and {} ranks per node".format(num_nodes, procs_per_node))
+    logger.debug(f"Creating machinefile with {num_nodes} nodes and {procs_per_node} ranks per node")
 
     with open(machinefile, "w") as f:
         for node in node_list[:num_nodes]:
             f.write((node + "\n") * procs_per_node)
 
     built_mfile = os.path.isfile(machinefile) and os.path.getsize(machinefile) > 0
     return built_mfile, num_procs, num_nodes, procs_per_node
```

### Comparing `libensemble-0.9.2/libensemble/resources/node_resources.py` & `libensemble-0.9.3/libensemble/resources/node_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
     output = subprocess.check_output([launcher, "python", __file__])
     return output.decode()
 
 
 def _get_cpu_resources_from_env(env_resources=None):
     """Returns logical and physical cores per node by querying environment or None"""
-
     if not env_resources:
         return None
 
     found_count = False
     if env_resources.nodelists["LSF"] in os.environ:
         full_list = os.environ.get(env_resources.nodelists["LSF"]).split()
         nodes = [n for n in full_list if "batch" not in n]
@@ -65,15 +64,15 @@
         nodes_with_count = [n for n in zipped_list if "batch" not in n[0]]
         counter = [int(n[1]) for n in nodes_with_count]
         found_count = True
 
     if found_count:
         # Check all nodes have equal cores -  Not doing for other methods currently.
         if len(set(counter)) != 1:
-            logger.warning("Detected compute nodes have different core counts: {}".format(set(counter)))
+            logger.warning(f"Detected compute nodes have different core counts: {set(counter)}")
 
         physical_cores_avail_per_node = counter[0]
         logical_cores_avail_per_node = counter[0]  # How to get SMT threads remotely
         logger.warning("SMT currently not detected, returning physical cores only. Specify procs_per_node to override")
         return (physical_cores_avail_per_node, logical_cores_avail_per_node)
     else:
         return None
```

### Comparing `libensemble-0.9.2/libensemble/resources/resources.py` & `libensemble-0.9.3/libensemble/resources/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,21 +48,19 @@
     resources = None
 
     DEFAULT_NODEFILE = "node_list"
 
     @classmethod
     def init_resources(cls, libE_specs):
         """Initiate resource management"""
-
         # If disable_resource_manager is True, then Resources.resources will remain None.
         disable_resource_manager = libE_specs.get("disable_resource_manager", False)
         if not disable_resource_manager:
             top_level_dir = os.getcwd()
-            if Resources.resources is None:
-                Resources.resources = Resources(libE_specs=libE_specs, top_level_dir=top_level_dir)
+            Resources.resources = Resources(libE_specs=libE_specs, top_level_dir=top_level_dir)
 
     def __init__(self, libE_specs, top_level_dir=None):
         """Initiate a new resources object"""
         self.top_level_dir = top_level_dir or os.getcwd()
         self.glob_resources = GlobalResources(libE_specs=libE_specs, top_level_dir=None)
         self.resource_manager = None  # For Manager
         self.worker_resources = None  # For Workers
@@ -160,17 +158,14 @@
         """
         self.top_level_dir = top_level_dir
         self.dedicated_mode = libE_specs.get("dedicated_mode", False)
         self.zero_resource_workers = libE_specs.get("zero_resource_workers", [])
         self.num_resource_sets = libE_specs.get("num_resource_sets", None)
         self.enforce_worker_core_bounds = libE_specs.get("enforce_worker_core_bounds", False)
 
-        if self.dedicated_mode:
-            logger.debug("Running in dedicated mode")
-
         resource_info = libE_specs.get("resource_info", {})
         cores_on_node = resource_info.get("cores_on_node", None)
         node_file = resource_info.get("node_file", None)
         nodelist_env_slurm = resource_info.get("nodelist_env_slurm", None)
         nodelist_env_cobalt = resource_info.get("nodelist_env_cobalt", None)
         nodelist_env_lsf = resource_info.get("nodelist_env_lsf", None)
         nodelist_env_lsf_shortform = resource_info.get("nodelist_env_lsf_shortform", None)
@@ -224,14 +219,15 @@
             self.libE_nodes = libE_nodes
         libE_nodes_in_list = list(filter(lambda x: x in self.libE_nodes, self.global_nodelist))
         if libE_nodes_in_list:
             if self.dedicated_mode and len(self.global_nodelist) > 1:
                 self.global_nodelist = GlobalResources.remove_nodes(self.global_nodelist, self.libE_nodes)
                 if not self.global_nodelist:
                     logger.warning("Warning. Node-list for tasks is empty. Remove dedicated_mode or add nodes")
+                    pass
 
     @staticmethod
     def is_nodelist_shortnames(nodelist):
         """Returns True if any entry contains a '.', else False"""
         for item in nodelist:
             if "." in item:
                 return False
@@ -255,25 +251,22 @@
 
         In dedicated mode, any node with a libE worker is removed from the list.
         """
         top_level_dir = rundir or os.getcwd()
         node_filepath = os.path.join(top_level_dir, node_file)
         global_nodelist = []
         if os.path.isfile(node_filepath):
-            logger.debug("node_file found - getting nodelist from node_file")
             with open(node_filepath, "r") as f:
                 for line in f:
                     global_nodelist.append(line.rstrip())
         else:
-            logger.debug("No node_file found - searching for nodelist in environment")
             if env_resources:
                 global_nodelist = env_resources.get_nodelist()
 
             if not global_nodelist:
                 # Assume a standalone machine
-                logger.info("Can not find nodelist from environment. Assuming standalone")
                 # global_nodelist.append(env_resources.shortnames([socket.gethostname()])[0])
                 global_nodelist.append(socket.gethostname())
 
         if global_nodelist:
             return global_nodelist
         raise ResourcesException("Error. global_nodelist is empty")
```

### Comparing `libensemble-0.9.2/libensemble/resources/rset_resources.py` & `libensemble-0.9.3/libensemble/resources/rset_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,28 +96,26 @@
 
         Assumes that self.global_nodelist has been calculated (in __init__).
         """
         global_nodelist = resources.global_nodelist
         num_nodes = len(global_nodelist)
 
         if not RSetResources.even_assignment(num_nodes, num_rsets):
-            logger.warning(
-                "Resource sets ({}) are not distributed evenly to available nodes ({})".format(num_rsets, num_nodes)
-            )
+            logger.warning(f"Resource sets ({num_rsets}) are not distributed evenly to available nodes ({num_nodes})")
 
         # If multiple workers per node - create global node_list with N duplicates (for N workers per node)
         sub_node_workers = num_rsets >= num_nodes
         if sub_node_workers:
             global_nodelist, local_rsets_list = RSetResources.expand_list(num_nodes, num_rsets, global_nodelist)
         else:
             local_rsets_list = [1] * num_rsets
 
         # Divide global list between workers
         split_list = list(RSetResources.best_split(global_nodelist, num_rsets))
-        logger.debug("split_list is {}".format(split_list))
+        logger.debug(f"split_list is {split_list}")
         return split_list, local_rsets_list
 
     @staticmethod
     def get_partitioned_nodelist(num_rsets, resources):
         """Returns lists of nodes available to all resource sets
 
         Assumes that self.global_nodelist has been calculated (in __init__).
```

### Comparing `libensemble-0.9.2/libensemble/resources/scheduler.py` & `libensemble-0.9.3/libensemble/resources/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         """
 
         if rsets_req == 0:
             return []
 
         if rsets_req > self.resources.total_num_rsets:
             raise InsufficientResourcesError(
-                "More resource sets requested {} than exist {}".format(rsets_req, self.resources.total_num_rsets)
+                f"More resource sets requested {rsets_req} than exist {self.resources.total_num_rsets}"
             )
 
         if rsets_req > self.rsets_free:
             raise InsufficientFreeResources
 
         self.log_msg = None  # Log resource messages only when find resources
         num_groups = self.resources.num_groups
@@ -152,24 +152,21 @@
                 avail_rsets_by_group, max_grpsize, rsets_req, num_groups_req, rsets_req_per_group
             )
 
         if self.log_msg is not None:
             logger.debug(self.log_msg)
 
         logger.debug(
-            "rset_team found: Req: {} rsets. Found: {} Avail sets {}".format(
-                rsets_req, rset_team, self.avail_rsets_by_group
-            )
+            f"rset_team found: Req: {rsets_req} rsets. Found: {rset_team} Avail sets {self.avail_rsets_by_group}"
         )
 
         return rset_team
 
     def find_rsets_any_slots(self, rsets_by_group, max_grpsize, rsets_req, ngroups, rsets_per_group):
         """Find optimal non-matching slots across groups"""
-
         tmp_rsets_by_group = copy.deepcopy(rsets_by_group)
         max_upper_bound = max_grpsize + 1
 
         # Now find slots on as many nodes as need
         accum_team = []
         group_list = []
 
@@ -281,17 +278,16 @@
             else:
                 if extend:
                     rsets_per_group = rsets_req // num_groups_req + (rsets_req % num_groups_req > 0)
                     orig_rsets_req = rsets_req
                     rsets_req = num_groups_req * rsets_per_group
                     self.log_msg = (
                         "Increasing resource requirement to obtain an even partition of resource sets\n"
-                        "to nodes. rsets_req orig: {} New: {}  num_groups_req {} rsets_per_group {}".format(
-                            orig_rsets_req, rsets_req, num_groups_req, rsets_per_group
-                        )
+                        f"to nodes. rsets_req orig: {orig_rsets_req} New: {rsets_req} "
+                        f"  num_groups_req {num_groups_req} rsets_per_group {rsets_per_group}"
                     )
                 else:
                     rsets_per_group = max_grpsize
         else:
             rsets_per_group = rsets_req
         return rsets_req, num_groups_req, rsets_per_group
```

### Comparing `libensemble-0.9.2/libensemble/resources/worker_resources.py` & `libensemble-0.9.3/libensemble/resources/worker_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,25 +61,23 @@
         unique, counts = np.unique(self.rsets["group"], return_counts=True)
         self.group_sizes = dict(zip(unique, counts))
         self.ngroups_by_size = Counter(counts)
         self.even_groups = True if len(self.ngroups_by_size) == 1 else False
 
     def assign_rsets(self, rset_team, worker_id):
         """Mark the resource sets given by rset_team as assigned to worker_id"""
-
         if rset_team:
             rteam = self.rsets["assigned"][rset_team]
             for i, wid in enumerate(rteam):
                 if wid == 0:
                     self.rsets["assigned"][rset_team[i]] = worker_id
                     self.rsets_free -= 1
                 elif wid != worker_id:
                     ResourceManagerException(
-                        "Error: Attempting to assign rsets {}"
-                        " already assigned to workers: {}".format(rset_team, rteam)
+                        f"Error: Attempting to assign rsets {rset_team}" f" already assigned to workers: {rteam}"
                     )
 
     def free_rsets(self, worker=None):
         """Free up assigned resource sets"""
         if worker is None:
             self.rsets["assigned"] = 0
             self.rsets_free = self.total_num_rsets
@@ -303,24 +301,23 @@
             self.matching_slots = True if all_match else False
             self.slots_on_node = first_node_slots if self.matching_slots else None
             self.slot_count = first_len if self.even_slots else None
 
     @staticmethod
     def get_local_nodelist(workerID, rset_team, split_list, rsets_per_node):
         """Returns the list of nodes available to the given worker and the slot dictionary"""
-
         if workerID is None:
             raise WorkerResourcesException("Worker has no workerID - aborting")
 
         team_list = []
         for index in rset_team:
             team_list += split_list[index]
 
         local_nodelist = list(OrderedDict.fromkeys(team_list))  # Maintain order of nodes
-        logger.debug("Worker's local_nodelist is {}".format(local_nodelist))
+        logger.debug(f"Worker's local_nodelist is {local_nodelist}")
 
         slots = {}
         for node in local_nodelist:
             slots[node] = []
 
         for index in rset_team:
             mynodes = split_list[index]
```

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/alt_rosenbrock.py` & `libensemble-0.9.3/libensemble/sim_funcs/alt_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/borehole.py` & `libensemble-0.9.3/libensemble/sim_funcs/borehole.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/borehole_kills.py` & `libensemble-0.9.3/libensemble/sim_funcs/borehole_kills.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from libensemble.executors.executor import Executor
 from libensemble.sim_funcs.surmise_test_function import borehole_true
-from libensemble.message_numbers import TASK_FAILED, MAN_SIGNAL_KILL, UNSET_TAG
+from libensemble.message_numbers import UNSET_TAG, TASK_FAILED, MAN_KILL_SIGNALS
 
 
 def subproc_borehole(H, delay):
     """This evaluates the Borehole function using a subprocess
     running compiled code.
 
     Note that the Executor base class submit runs a
@@ -19,15 +19,15 @@
 
     exctr = Executor.executor
     args = "input" + " " + str(delay)
 
     task = exctr.submit(app_name="borehole", app_args=args, stdout="out.txt", stderr="err.txt")
     calc_status = exctr.polling_loop(task, delay=0.01, poll_manager=True)
 
-    if calc_status in [MAN_SIGNAL_KILL, TASK_FAILED]:
+    if calc_status in MAN_KILL_SIGNALS + [TASK_FAILED]:
         f = np.inf
     else:
         f = float(task.read_stdout())
     return f, calc_status
 
 
 def borehole(H, persis_info, sim_specs, libE_info):
@@ -42,16 +42,19 @@
     sim_id = libE_info["H_rows"][0]
     delay = 0
     if sim_id > sim_specs["user"]["init_sample_size"]:
         delay = 2 + np.random.normal(scale=0.5)
 
     f, calc_status = subproc_borehole(H, delay)
 
-    # Failure model (excluding observations)
-    if sim_id > sim_specs["user"]["num_obs"]:
-        if (f / borehole_true(H["x"])) > 1.25:
-            f = np.inf
-            calc_status = TASK_FAILED
-            print("Failure of sim_id {}".format(sim_id), flush=True)
+    if calc_status in MAN_KILL_SIGNALS and "sim_killed" in H_o.dtype.names:
+        H_o["sim_killed"] = True  # For calling script to print only.
+    else:
+        # Failure model (excluding observations)
+        if sim_id > sim_specs["user"]["num_obs"]:
+            if (f / borehole_true(H["x"])) > 1.25:
+                f = np.inf
+                calc_status = TASK_FAILED
+                print(f"Failure of sim_id {sim_id}", flush=True)
 
     H_o["f"] = f
     return H_o, persis_info, calc_status
```

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/branin/branin.py` & `libensemble-0.9.3/libensemble/sim_funcs/branin/branin.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/branin/branin_obj.py` & `libensemble-0.9.3/libensemble/sim_funcs/branin/branin_obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import numpy as np
 import time
 from libensemble.sim_funcs.branin.branin import branin
 
 
 def call_branin(H, persis_info, sim_specs, _):
     """Evaluates the Branin function"""
-
     batch = len(H["x"])
 
     H_o = np.zeros(batch, dtype=sim_specs["out"])
 
     for i, x in enumerate(H["x"]):
         # Uncomment the following if you want to use the file system to do evaluations
         # devnull = open(os.devnull, 'w')
```

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/chwirut1.py` & `libensemble-0.9.3/libensemble/sim_funcs/chwirut1.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/executor_hworld.py` & `libensemble-0.9.3/libensemble/sim_funcs/executor_hworld.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,162 +20,165 @@
     import time
 
     calc_status = UNSET_TAG  # Sim func determines status of libensemble calc - returned to worker
 
     while task.runtime < timeout_sec:
         time.sleep(delay)
 
-        exctr.manager_poll()
-        if exctr.manager_signal == "finish":
+        if exctr.manager_kill_received():
             exctr.kill(task)
             calc_status = MAN_SIGNAL_FINISH  # Worker will pick this up and close down
-            print("Task {} killed by manager on worker {}".format(task.id, exctr.workerID))
+            print(f"Task {task.id} killed by manager on worker {exctr.workerID}")
             break
 
         task.poll()
         if task.finished:
             break
         elif task.state == "RUNNING":
-            print("Task {} still running on worker {} ....".format(task.id, exctr.workerID))
+            print(f"Task {task.id} still running on worker {exctr.workerID} ....")
 
         if task.stdout_exists():
             if "Error" in task.read_stdout():
                 print(
-                    "Found (deliberate) Error in output file - cancelling "
-                    "task {} on worker {}".format(task.id, exctr.workerID)
+                    "Found (deliberate) Error in output file - cancelling " f"task {task.id} on worker {exctr.workerID}"
                 )
                 exctr.kill(task)
                 calc_status = WORKER_KILL_ON_ERR
                 break
 
     # After exiting loop
     if task.finished:
-        print("Task {} done on worker {}".format(task.id, exctr.workerID))
+        print(f"Task {task.id} done on worker {exctr.workerID}")
         # Fill in calc_status if not already
         if calc_status == UNSET_TAG:
             if task.state == "FINISHED":  # Means finished successfully
                 calc_status = WORKER_DONE
             elif task.state == "FAILED":
                 calc_status = TASK_FAILED
 
     else:
         # assert task.state == 'RUNNING', "task.state expected to be RUNNING. Returned: " + str(task.state)
-        print("Task {} timed out - killing on worker {}".format(task.id, exctr.workerID))
+        print(f"Task {task.id} timed out - killing on worker {exctr.workerID}")
         exctr.kill(task)
         if task.finished:
-            print("Task {} done on worker {}".format(task.id, exctr.workerID))
+            print(f"Task {task.id} done on worker {exctr.workerID}")
         calc_status = WORKER_KILL_ON_TIMEOUT
 
     return task, calc_status
 
 
 def executor_hworld(H, persis_info, sim_specs, libE_info):
     """Tests launching and polling task and exiting on task finish"""
     exctr = MPIExecutor.executor
     cores = sim_specs["user"]["cores"]
     USE_BALSAM = "balsam_test" in sim_specs["user"]
     ELAPSED_TIMEOUT = "elapsed_timeout" in sim_specs["user"]
 
     wait = False
     args_for_sim = "sleep 1"
+    calc_status = UNSET_TAG
 
-    if ELAPSED_TIMEOUT:
-        args_for_sim = "sleep 60"  # Manager kill - if signal received else completes
-        timeout = 65.0
+    batch = len(H["x"])
+    H_o = np.zeros(batch, dtype=sim_specs["out"])
+
+    if "six_hump_camel" not in exctr.default_app("sim").full_path:
 
-    else:
         global sim_ended_count
         sim_ended_count += 1
-        timeout = 6.0
-        launch_shc = False
-        print(sim_ended_count)
-
-        if sim_ended_count == 1:
-            args_for_sim = "sleep 1"  # Should finish
-        elif sim_ended_count == 2:
-            args_for_sim = "sleep 1 Error"  # Worker kill on error
-        elif sim_ended_count == 3:
-            wait = True
-            args_for_sim = "sleep 1"  # Should finish
-            launch_shc = True
-        elif sim_ended_count == 4:
-            args_for_sim = "sleep 8"  # Worker kill on timeout
-            timeout = 1.0
-        elif sim_ended_count == 5:
-            args_for_sim = "sleep 2 Fail"  # Manager kill - if signal received else completes
-
-    if USE_BALSAM:
-        task = exctr.submit(
-            calc_type="sim",
-            num_procs=cores,
-            app_args=args_for_sim,
-            hyperthreads=True,
-            machinefile="notused",
-            stdout="notused",
-            wait_on_start=True,
-        )
-    else:
-        task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim, hyperthreads=True)
+        print("sim_ended_count", sim_ended_count, flush=True)
 
-    if wait:
-        task.wait()
-        if not task.finished:
-            calc_status = UNSET_TAG
-        if task.state == "FINISHED":
-            calc_status = WORKER_DONE
-        elif task.state == "FAILED":
-            calc_status = TASK_FAILED
+        if ELAPSED_TIMEOUT:
+            args_for_sim = "sleep 60"  # Manager kill - if signal received else completes
+            timeout = 65.0
 
-    else:
-        if not ELAPSED_TIMEOUT:
+        else:
+            timeout = 6.0
+            launch_shc = False
+
+            if sim_ended_count == 1:
+                args_for_sim = "sleep 1"  # Should finish
+            elif sim_ended_count == 2:
+                args_for_sim = "sleep 1 Error"  # Worker kill on error
+            elif sim_ended_count == 3:
+                wait = True
+                args_for_sim = "sleep 1"  # Should finish
+                launch_shc = True
+            elif sim_ended_count == 4:
+                args_for_sim = "sleep 8"  # Worker kill on timeout
+                timeout = 1.0
+            elif sim_ended_count == 5:
+                args_for_sim = "sleep 2 Fail"  # Manager kill - if signal received else completes
+
+        if USE_BALSAM:
+            task = exctr.submit(
+                calc_type="sim",
+                num_procs=cores,
+                app_args=args_for_sim,
+                hyperthreads=True,
+                machinefile="notused",
+                stdout="notused",
+                wait_on_start=True,
+            )
+        else:
+            task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim, hyperthreads=True)
+
+        if wait:
+            task.wait()
+            if not task.finished:
+                calc_status = UNSET_TAG
+            if task.state == "FINISHED":
+                calc_status = WORKER_DONE
+            elif task.state == "FAILED":
+                calc_status = TASK_FAILED
+
+        else:
             if sim_ended_count >= 2 and not USE_BALSAM:
                 calc_status = exctr.polling_loop(task, timeout=timeout, delay=0.3, poll_manager=True)
                 if sim_ended_count == 2 and task.stdout_exists() and "Error" in task.read_stdout():
                     calc_status = WORKER_KILL_ON_ERR
-
             else:
                 task, calc_status = custom_polling_loop(exctr, task, timeout)
 
-        else:
-            calc_status = exctr.polling_loop(task, timeout=timeout, delay=0.3, poll_manager=True)
+        if USE_BALSAM:
+            task.read_file_in_workdir("ensemble.log")
+            try:
+                task.read_stderr()
+            except ValueError:
+                pass
+
+            task = exctr.submit(
+                app_name="sim_hump_camel_dry_run",
+                num_procs=cores,
+                app_args=args_for_sim,
+                hyperthreads=True,
+                machinefile="notused",
+                stdout="notused",
+                wait_on_start=True,
+                dry_run=True,
+                stage_inout=os.getcwd(),
+            )
 
-    if USE_BALSAM:
-        task.read_file_in_workdir("ensemble.log")
-        try:
-            task.read_stderr()
-        except ValueError:
-            pass
-
-        task = exctr.submit(
-            app_name="sim_hump_camel_dry_run",
-            num_procs=cores,
-            app_args=args_for_sim,
-            hyperthreads=True,
-            machinefile="notused",
-            stdout="notused",
-            wait_on_start=True,
-            dry_run=True,
-            stage_inout=os.getcwd(),
-        )
+            task.poll()
+            task.wait()
 
-        task.poll()
-        task.wait()
+    else:
+        launch_shc = True
+        calc_status = UNSET_TAG
 
-    # This is temp - return something - so doing six_hump_camel_func again...
-    batch = len(H["x"])
-    H_o = np.zeros(batch, dtype=sim_specs["out"])
-    for i, x in enumerate(H["x"]):
-        H_o["f"][i] = six_hump_camel_func(x)
-        if launch_shc:
-            # Test launching a named app.
-            app_args = " ".join(str(val) for val in list(x[:]))
-            task = exctr.submit(app_name="six_hump_camel", num_procs=1, app_args=app_args)
-            task.wait()
-            output = np.float64(task.read_stdout())
-            assert np.isclose(H_o["f"][i], output)
+        # Comparing six_hump_camel output, directly called vs. submitted as app
+        for i, x in enumerate(H["x"]):
+            H_o["f"][i] = six_hump_camel_func(x)
+            if launch_shc:
+                # Test launching a named app.
+                app_args = " ".join(str(val) for val in list(x[:]))
+                task = exctr.submit(app_name="six_hump_camel", num_procs=1, app_args=app_args)
+                task.wait()
+                output = np.float64(task.read_stdout())
+                assert np.isclose(H_o["f"][i], output)
+                calc_status = WORKER_DONE
 
     # This is just for testing at calling script level - status of each task
     H_o["cstat"] = calc_status
 
     return H_o, persis_info, calc_status
```

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/geomedian.py` & `libensemble-0.9.3/libensemble/sim_funcs/geomedian.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/heffte.py` & `libensemble-0.9.3/libensemble/sim_funcs/heffte.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/inverse_bayes.py` & `libensemble-0.9.3/libensemble/sim_funcs/inverse_bayes.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/linear_regression.py` & `libensemble-0.9.3/libensemble/sim_funcs/linear_regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 def linear_regression_eval(H, persis_info, sim_specs, _):
 
     X = persis_info["params"]["X"]
     y = persis_info["params"]["y"]
     c = persis_info["params"]["c"]
     reg = persis_info["params"].get("reg", None)
 
-    assert (reg is None) or (reg == "l1") or (reg == "l2"), "Incompatible regularization {}".format(reg)
+    assert (reg is None) or (reg == "l1") or (reg == "l2"), f"Incompatible regularization {reg}"
 
     batch = len(H["x"])
     H_o = np.zeros(batch, dtype=sim_specs["out"])
 
     for i, x in enumerate(H["x"]):
         obj_component = H["obj_component"][i]  # which f_i
```

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/logistic_regression.py` & `libensemble-0.9.3/libensemble/sim_funcs/logistic_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 def logistic_regression_eval(H, persis_info, sim_specs, _):
 
     X = persis_info["params"]["X"]
     y = persis_info["params"]["y"]
     c = persis_info["params"]["c"]
     reg = persis_info["params"].get("reg", None)
 
-    assert (reg is None) or (reg == "l1") or (reg == "l2"), "Incompatible regularization {}".format(reg)
+    assert (reg is None) or (reg == "l1") or (reg == "l2"), f"Incompatible regularization {reg}"
 
     batch = len(H["x"])
     H_o = np.zeros(batch, dtype=sim_specs["out"])
 
     for i, x in enumerate(H["x"]):
         obj_component = H["obj_component"][i]  # which f_i
```

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/nesterov_quadratic.py` & `libensemble-0.9.3/libensemble/sim_funcs/nesterov_quadratic.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/noisy_vector_mapping.py` & `libensemble-0.9.3/libensemble/sim_funcs/noisy_vector_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         H0["f_val"][i] = noisy_function(x)[H["f_ind"][i]]
 
     return H0, persis_info
 
 
 def noisy_function(x):
     """ """
-
     x1 = x[0]
     x2 = x[1]
     term1 = (4 - 2.1 * x1**2 + (x1**4) / 3) * x1**2
     term2 = x1 * x2
     term3 = (-4 + 4 * x2**2) * x2**2
 
     phi1 = 0.9 * sin(100 * norm(x, 1)) * cos(100 * norm(x, np.inf)) + 0.1 * cos(norm(x, 2))
```

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/one_d_func.py` & `libensemble-0.9.3/libensemble/sim_funcs/one_d_func.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/rosenbrock.py` & `libensemble-0.9.3/libensemble/sim_funcs/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/run_line_check.py` & `libensemble-0.9.3/libensemble/sim_funcs/run_line_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             dry_run=True,
         )
 
         outline = task.runline
         new_exp_list = exp_nodelist_for_worker(exp_list[i], libE_info["workerID"], npw, p_gens)
 
         if outline != new_exp_list:
-            print("outline is: {}\nexp     is: {}".format(outline, new_exp_list), flush=True)
+            print(f"outline is: {outline}\nexp     is: {new_exp_list}", flush=True)
 
         assert outline == new_exp_list
 
     calc_status = WORKER_DONE
     output = np.zeros(1, dtype=sim_specs["out"])
     output["f"][0] = np.linalg.norm(x)
     return output, persis_info, calc_status
@@ -104,15 +104,15 @@
         wid_mod = circ_offset(wid, len(exp_list))
     else:
         wid_mod = wid
 
     new_exp_list = exp_list[wid_mod - 1 - p_gens]
 
     if outline != new_exp_list:
-        print("Worker {}:\n outline is: {}\n exp     is: {}".format(wid, outline, new_exp_list), flush=True)
+        print(f"Worker {wid}:\n outline is: {outline}\n exp     is: {new_exp_list}", flush=True)
 
     assert outline == new_exp_list
 
     calc_status = WORKER_DONE
     output = np.zeros(1, dtype=sim_specs["out"])
     output["f"][0] = np.linalg.norm(x)
     return output, persis_info, calc_status
```

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/six_hump_camel.py` & `libensemble-0.9.3/libensemble/sim_funcs/six_hump_camel.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,26 +138,23 @@
     x = H["x"][0]
     H_o = np.zeros(1, dtype=sim_specs["out"])
 
     # Interrogate resources available to this worker
     resources = Resources.resources.worker_resources
     slots = resources.slots
 
-    assert resources.matching_slots, "Error: Cannot set CUDA_VISIBLE_DEVICES when unmatching slots on nodes {}".format(
-        slots
-    )
+    assert resources.matching_slots, f"Error: Cannot set CUDA_VISIBLE_DEVICES when unmatching slots on nodes {slots}"
 
     resources.set_env_to_slots("CUDA_VISIBLE_DEVICES")
     num_nodes = resources.local_node_count
     cores_per_node = resources.slot_count  # One CPU per GPU
 
     print(
-        "Worker {}: CUDA_VISIBLE_DEVICES={}  \tnodes {} ppn {}  slots {}".format(
-            libE_info["workerID"], os.environ["CUDA_VISIBLE_DEVICES"], num_nodes, cores_per_node, slots
-        )
+        f"Worker {libE_info['workerID']}: CUDA_VISIBLE_DEVICES={os.environ['CUDA_VISIBLE_DEVICES']}"
+        f"\tnodes {num_nodes} ppn {cores_per_node}  slots {slots}"
     )
 
     # Create application input file
     inpt = " ".join(map(str, x))
     exctr = Executor.executor  # Get Executor
 
     # Launch application via system MPI runner, using assigned resources.
```

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/surmise_test_function.py` & `libensemble-0.9.3/libensemble/sim_funcs/surmise_test_function.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/sim_funcs/svm.py` & `libensemble-0.9.3/libensemble/sim_funcs/svm.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 def svm_eval(H, persis_info, sim_specs, _):
 
     X = persis_info["params"]["X"]
     b = persis_info["params"]["b"]
     c = persis_info["params"]["c"]
     reg = persis_info["params"].get("reg", None)
 
-    assert (reg is None) or (reg == "l1") or (reg == "l2"), "Incompatible regularization {}".format(reg)
+    assert (reg is None) or (reg == "l1") or (reg == "l2"), f"Incompatible regularization {reg}"
 
     batch = len(H["x"])
     H_o = np.zeros(batch, dtype=sim_specs["out"])
 
     for i, x in enumerate(H["x"]):
         obj_component = H["obj_component"][i]  # which f_i
```

### Comparing `libensemble-0.9.2/libensemble/tests/.coveragerc` & `libensemble-0.9.3/libensemble/tests/.coveragerc`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     */setup.py
     */unit_tests/*
     */unit_tests_nompi/*
     */unit_tests_logger/*
     */regression_tests/*
     */sim_funcs/helloworld.py
     */sim_funcs/executor_hworld.py
-    */balsam_executor.py
     */legacy_balsam_executor.py
     */forkable_pdb.py
     */parse_args.py
     */gen_funcs/old_aposmm.py
     */alloc_funcs/fast_alloc_to_aposmm.py
 exclude_lines =
     if __name__ == .__main__.:
```

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/bash_scripts/setup_balsam_tests.sh` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/bash_scripts/setup_balsam_tests.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/readme.balsam_tests.txt` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/readme.balsam_tests.txt`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/readme.rst` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/readme.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/setup_balsam_tests.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/setup_balsam_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 
 """ Script to set up apps and jobs for balsam tests """
-
 # Note: To see use of command line interface see bash_scripts/setup_balsam_tests.sh script.
 #       Currently that script does not create deps between jobs so may run simultaneously
 #       This script tests setup within python (could in theory be integrated with job!)
 
 import os
 import sys
 import subprocess
@@ -29,20 +28,20 @@
 
 
 # As balsam req python 3.6 lets use subprocess.run
 # For any stuff requiring CLI
 def run_cmd(cmd, echo=False):
     """Run a bash command"""
     if echo:
-        print("\nRunning %s ...\n" % cmd)
+        print(f"\nRunning {cmd} ...\n")
     try:
         subprocess.run(cmd.split(), check=True)
     except Exception as e:
         print(e)
-        raise ("Error: Command %s failed to run" % cmd)
+        raise (f"Error: Command {cmd} failed to run")
 
 
 # Use relative paths to balsam_tests dir
 work_dir = os.path.dirname(os.path.abspath(__file__))
 
 sim_input_dir = os.path.abspath("../../examples/sim_funcs")
 sim_app = "helloworld.py"
```

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_1__runjobs.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_2__workerkill.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import os  # for adding to path
 import time
 from mpi4py import MPI
 
 import balsam.launcher.dag as dag
 
 
-def poll_until_state(job, state, timeout_sec=60.0, delay=2.0):
+def poll_until_state(job, state, timeout_sec=120.0, delay=2.0):
     start = time.time()
     while time.time() - start < timeout_sec:
         time.sleep(delay)
         job.refresh_from_db()
         if job.state == state:
             return True
-    raise RuntimeError("Task %s failed to reach state %s in %.1f seconds" % (job.cute_id, state, timeout_sec))
+        elif job.state == "USER_KILLED":
+            return False
+    raise RuntimeError(f"Task {job.cute_id} failed to reach state {state} in {timeout_sec:.1f} seconds")
 
 
 myrank = MPI.COMM_WORLD.Get_rank()
 steps = 3
 sleep_time = 3  # + myrank
 
 # Create output dir
@@ -28,33 +30,35 @@
 
 if myrank == 0:
     if not os.path.isdir(sim_path):
         try:
             os.mkdir(sim_path)
         except Exception as e:
             print(e)
-            raise ("Cannot make simulation directory %s" % sim_path)
+            raise (f"Cannot make simulation directory {sim_path}")
 MPI.COMM_WORLD.Barrier()  # Ensure output dir created
 
 print("Host job rank is %d Output dir is %s" % (myrank, sim_input_dir))
 
 start = time.time()
 for sim_id in range(steps):
-    jobname = "outfile_t1_" + "for_sim_id_" + str(sim_id) + "_ranks_" + str(myrank) + ".txt"
+    jobname = "outfile_t2_" + "for_sim_id_" + str(sim_id) + "_ranks_" + str(myrank) + ".txt"
 
     current_job = dag.add_job(
         name=jobname,
         workflow="libe_workflow",
         application="helloworld",
         application_args=str(sleep_time),
         num_nodes=1,
         procs_per_node=8,
         stage_out_url="local:" + sim_path,
         stage_out_files=jobname + ".out",
     )
+    if sim_id == 1:
+        dag.kill(current_job)
 
     success = poll_until_state(current_job, "JOB_FINISHED")  # OR job killed
     if success:
         print("Completed job: %s rank=%d time=%f" % (jobname, myrank, time.time() - start))
     else:
         print(
             "Task not completed: %s rank=%d time=%f Status" % (jobname, myrank, time.time() - start), current_job.state
```

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_2__workerkill.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_1__runjobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 import os  # for adding to path
 import time
 from mpi4py import MPI
 
 import balsam.launcher.dag as dag
 
 
-def poll_until_state(job, state, timeout_sec=120.0, delay=2.0):
+def poll_until_state(job, state, timeout_sec=60.0, delay=2.0):
     start = time.time()
     while time.time() - start < timeout_sec:
         time.sleep(delay)
         job.refresh_from_db()
         if job.state == state:
             return True
-        elif job.state == "USER_KILLED":
-            return False
-    raise RuntimeError("Task %s failed to reach state %s in %.1f seconds" % (job.cute_id, state, timeout_sec))
+    raise RuntimeError(f"Task {job.cute_id} failed to reach state {state} in {timeout_sec:.1f} seconds")
 
 
 myrank = MPI.COMM_WORLD.Get_rank()
 steps = 3
 sleep_time = 3  # + myrank
 
 # Create output dir
@@ -30,35 +28,33 @@
 
 if myrank == 0:
     if not os.path.isdir(sim_path):
         try:
             os.mkdir(sim_path)
         except Exception as e:
             print(e)
-            raise ("Cannot make simulation directory %s" % sim_path)
+            raise (f"Cannot make simulation directory {sim_path}")
 MPI.COMM_WORLD.Barrier()  # Ensure output dir created
 
 print("Host job rank is %d Output dir is %s" % (myrank, sim_input_dir))
 
 start = time.time()
 for sim_id in range(steps):
-    jobname = "outfile_t2_" + "for_sim_id_" + str(sim_id) + "_ranks_" + str(myrank) + ".txt"
+    jobname = "outfile_t1_" + "for_sim_id_" + str(sim_id) + "_ranks_" + str(myrank) + ".txt"
 
     current_job = dag.add_job(
         name=jobname,
         workflow="libe_workflow",
         application="helloworld",
         application_args=str(sleep_time),
         num_nodes=1,
         procs_per_node=8,
         stage_out_url="local:" + sim_path,
         stage_out_files=jobname + ".out",
     )
-    if sim_id == 1:
-        dag.kill(current_job)
 
     success = poll_until_state(current_job, "JOB_FINISHED")  # OR job killed
     if success:
         print("Completed job: %s rank=%d time=%f" % (jobname, myrank, time.time() - start))
     else:
         print(
             "Task not completed: %s rank=%d time=%f Status" % (jobname, myrank, time.time() - start), current_job.state
```

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_3__managerkill.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/balsam_tests/test_balsam_3__managerkill.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     while time.time() - start < timeout_sec:
         time.sleep(delay)
         job.refresh_from_db()
         if job.state == state:
             return True
         elif job.state == "USER_KILLED":
             return False
-        raise RuntimeError("Task %s failed to reach state %s in %.1f seconds" % (job.cute_id, state, timeout_sec))
+        raise RuntimeError(f"Task {job.cute_id} failed to reach state {state} in {timeout_sec:.1f} seconds")
 
 
 myrank = MPI.COMM_WORLD.Get_rank()
 steps = 3
 sleep_time = 3  # + myrank
 
 # Create output dir
@@ -30,15 +30,15 @@
 
 if myrank == 0:
     if not os.path.isdir(sim_path):
         try:
             os.mkdir(sim_path)
         except Exception as e:
             print(e)
-            raise ("Cannot make simulation directory %s" % sim_path)
+            raise (f"Cannot make simulation directory {sim_path}")
 MPI.COMM_WORLD.Barrier()  # Ensure output dir created
 
 print("Host job rank is %d Output dir is %s" % (myrank, sim_input_dir))
 
 start = time.time()
 for sim_id in range(steps):
     jobname = "outfile_t3_" + "for_sim_id_" + str(sim_id) + "_ranks_" + str(myrank) + ".txt"
```

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/create_balsam_job.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/create_balsam_job.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/readme.txt` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/readme.txt`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/set.balsam.database.sh` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/set.balsam.database.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/my_simtask.c` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/my_simtask.c`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/my_simtask.f90` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/my_simtask.f90`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor_manager_poll.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor_manager_poll.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #  This keeps MPI out of user code and is portable across different
 #  worker concurrency schemes (MPI/threading/multiprocessing)
 
 # Test does not require running full libensemble
 
 import os
 from libensemble.executors.executor import Executor
+from libensemble.message_numbers import MAN_SIGNAL_KILL
 
 
 def build_simfunc():
     import subprocess
 
     # Build simfunc
     # buildstring='mpif90 -o my_simtask.x my_simtask.f90' # On cray need to use ftn
@@ -64,22 +65,22 @@
 
     start = time.time()
 
     while time.time() - start < timeout_sec:
 
         exctr.manager_poll(task)
 
-        if task.manager_signal == "kill":
+        if task.manager_signal == MAN_SIGNAL_KILL:
             print("Manager has sent kill signal - killing task")
             exctr.kill(task)
 
         # In future might support other manager signals eg:
-        elif task.manager_signal == "pause":
-            # checkpoint_task()
-            pass
+        # elif task.manager_signal == "pause":
+        #     checkpoint_task()
+        #     pass
 
         time.sleep(delay)
         print("Polling at time", time.time() - start)
         task.poll()
         if task.finished:
             break
         elif task.state == "WAITING":
```

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor_multi.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor_multi.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,28 +65,28 @@
         active_list = [task for task in task_list if not task.finished]
         if not active_list:
             break
 
         for task in task_list:
             if not task.finished:
                 time.sleep(delay)
-                print("Polling task {0} at time {1}".format(task.id, time.time() - start))
+                print(f"Polling task {task.id} at time {time.time() - start}")
                 task.poll()
 
                 if task.finished:
                     continue
                 elif task.state == "WAITING":
-                    print("Task {0} waiting to execute".format(task.id))
+                    print(f"Task {task.id} waiting to execute")
                 elif task.state == "RUNNING":
-                    print("Task {0} still running ....".format(task.id))
+                    print(f"Task {task.id} still running ....")
 
                 # Check output file for error
                 if task.stdout_exists():
                     if "Error" in task.read_stdout():
-                        print("Found (deliberate) Error in output file - " "cancelling task {}".format(task.id))
+                        print(f"Found (deliberate) Error in output file - cancelling task {task.id}")
                         exctr.kill(task)
                         time.sleep(delay)  # Give time for kill
                         continue
 
                 # But if I want to do something different -
                 #  I want to make a file - no function for THAT!
                 # But you can get all the task attributes!
@@ -95,29 +95,29 @@
                 # open(path, 'a')
 
     print("Loop time", time.time() - start)
 
     for task in task_list:
         if task.finished:
             if task.state == "FINISHED":
-                print("Task {0} finished successfully. Status: {1}".format(task.id, task.state))
+                print(f"Task {task.id} finished successfully. Status: {task.state}")
             elif task.state == "FAILED":
-                print("Task {0} failed. Status: {1}".format(task.id, task.state))
+                print(f"Task {task.id} failed. Status: {task.state}")
             elif task.state == "USER_KILLED":
-                print("Task {0} has been killed. Status: {1}".format(task.id, task.state))
+                print(f"Task {task.id} has been killed. Status: {task.state}")
             else:
-                print("Task {0} status: {1}".format(task.id, task.state))
+                print(f"Task {task.id} status: {task.state}")
         else:
-            print("Task {0} timed out. Status: {1}".format(task.id, task.state))
+            print(f"Task {task.id} timed out. Status: {task.state}")
             exctr.kill(task)
             if task.finished:
-                print("Task {0} Now killed. Status: {1}".format(task.id, task.state))
+                print(f"Task {task.id} Now killed. Status: {task.state}")
                 # double check
                 task.poll()
-                print("Task {0} state is {1}".format(task.id, task.state))
+                print(f"Task {task.id} state is {task.state}")
 
 
 # Tests
 
 # From worker call Executor by different name to ensure getting registered
 # app from Executor
 exctr = Executor.executor
```

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/test_nan_func_old_aposmm.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/test_nan_func_old_aposmm.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_logic.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_logic.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_one_residual_at_a_time.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_one_residual_at_a_time.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_pounders.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_pounders.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_pounders_splitcomm.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_pounders_splitcomm.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_pounders_subcomm.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_pounders_subcomm.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_sim_dirs.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_sim_dirs.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/deprecated_tests/test_old_aposmm_with_gradients.py` & `libensemble-0.9.3/libensemble/tests/deprecated_tests/test_old_aposmm_with_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
         persis_info = deepcopy(persis_info_safe)
 
     H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
     if is_manager:
         if flag != 0:
-            print("Exit was not on convergence (code {})".format(flag), flush=True)
+            print(f"Exit was not on convergence (code {flag})", flush=True)
             libE_abort()
 
         tol = 1e-5
         for m in minima:
             # The minima are known on this test problem.
             # 1) We use their values to test APOSMM has identified all minima
             # 2) We use their approximate values to ensure APOSMM evaluates a
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_1d_uniform_sampling_with_comm_dup.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_1d_uniform_sampling_with_comm_dup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 The number of concurrent evaluations of the objective function will be 4-1=3.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: mpi
 # TESTSUITE_NPROCS: 2 4
+# TESTSUITE_OS_SKIP: WIN
 
 import sys
 import numpy as np
 
 # Import libEnsemble items for this test
 from libensemble.libE import libE
 from libensemble.sim_funcs.one_d_func import one_d_example as sim_f
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_calc_exception.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_calc_exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,12 +53,12 @@
     libE_specs["abort_on_exception"] = False
 
     # Perform the run
     return_flag = 1
     try:
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs)
     except LoggedException as e:
-        print("Caught deliberate exception: {}".format(e))
+        print(f"Caught deliberate exception: {e}")
         return_flag = 0
 
     if is_manager:
         assert return_flag == 0
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_cancel_in_alloc.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_cancel_in_alloc.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_comms.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_comms.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_elapsed_time_abort.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_elapsed_time_abort.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_executor_hworld_pass_fail.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_executor_hworld_pass_fail.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 from libensemble.tools import parse_args, add_unique_random_streams
 from libensemble.tests.regression_tests.common import build_simfunc
 from libensemble.executors.mpi_executor import MPIExecutor
 
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: mpi local tcp
-# TESTSUITE_OS_SKIP: OSX
+# TESTSUITE_OS_SKIP: OSX WIN
 # TESTSUITE_NPROCS: 2 3 4
 # TESTSUITE_OMPI_SKIP: true
+# TESTSUITE_EXTRA: true
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     libE_specs["disable_resource_manager"] = True
@@ -48,15 +49,15 @@
         disable_resource_manager = True
         mess_resources = "TCP comms does not support resource management. Resource manager disabled"
     else:
         disable_resource_manager = False
         mess_resources = "Resource manager enabled"
 
     if is_manager:
-        print("\nCores req: {} Cores avail: {}\n  {}\n".format(cores_all_tasks, logical_cores, mess_resources))
+        print(f"\nCores req: {cores_all_tasks} Cores avail: {logical_cores}\n  {mess_resources}\n")
 
     sim_app = "./my_simtask.x"
     if not os.path.isfile(sim_app):
         build_simfunc()
     sim_app2 = six_hump_camel.__file__
 
     exctr = MPIExecutor()
@@ -95,15 +96,15 @@
 
         calc_status_list_in = np.asarray(
             [WORKER_DONE, WORKER_KILL_ON_ERR, WORKER_DONE, WORKER_KILL_ON_TIMEOUT, TASK_FAILED]
         )
         calc_status_list = np.repeat(calc_status_list_in, nworkers)
 
         # For debug
-        print("Expecting: {}".format(calc_status_list))
-        print("Received:  {}\n".format(H["cstat"]))
+        print(f"Expecting: {calc_status_list}")
+        print("Received:  {H['cstat']}\n")
 
         assert np.array_equal(H["cstat"], calc_status_list), "Error - unexpected calc status. Received: " + str(
             H["cstat"]
         )
 
         print("\n\n\nRun completed.")
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_executor_hworld_timeout.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_executor_hworld_timeout.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from libensemble.tests.regression_tests.common import build_simfunc
 from libensemble.executors.mpi_executor import MPIExecutor
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: mpi local tcp
 # TESTSUITE_NPROCS: 2 3 4
 # TESTSUITE_OMPI_SKIP: true
-# TESTSUITE_OS_SKIP: OSX
+# TESTSUITE_OS_SKIP: OSX WIN
+# TESTSUITE_EXTRA: true
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     libE_specs["disable_resource_manager"] = True
@@ -46,15 +47,15 @@
         disable_resource_manager = True
         mess_resources = "TCP comms does not support resource management. Resource manager disabled"
     else:
         disable_resource_manager = False
         mess_resources = "Resource manager enabled"
 
     if is_manager:
-        print("\nCores req: {} Cores avail: {}\n  {}\n".format(cores_all_tasks, logical_cores, mess_resources))
+        print(f"\nCores req: {cores_all_tasks} Cores avail: {logical_cores}\n  {mess_resources}\n")
 
     sim_app = "./my_simtask.x"
     if not os.path.isfile(sim_app):
         build_simfunc()
     sim_app2 = six_hump_camel.__file__
 
     exctr = MPIExecutor()
@@ -81,27 +82,35 @@
             "ub": np.array([3, 2]),
             "gen_batch_size": nworkers,
         },
     }
 
     persis_info = add_unique_random_streams({}, nworkers + 1)
 
-    exit_criteria = {"wallclock_max": 30}
+    exit_criteria = {"wallclock_max": 10}
 
-    # Perform the run
-    H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs)
+    # TCP does not support multiple libE calls
+    if libE_specs["comms"] == "tcp":
+        iterations = 1
+    else:
+        iterations = 2
 
-    if is_manager:
-        print("\nChecking expected task status against Workers ...\n")
+    for i in range(iterations):
+
+        # Perform the run
+        H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs)
+
+        if is_manager:
+            print("\nChecking expected task status against Workers ...\n")
 
-        calc_status_list_in = np.asarray([0])
-        calc_status_list = np.repeat(calc_status_list_in, nworkers)
+            calc_status_list_in = np.asarray([0])
+            calc_status_list = np.repeat(calc_status_list_in, nworkers)
 
-        # For debug
-        print("Expecting: {}".format(calc_status_list))
-        print("Received:  {}\n".format(H["cstat"]))
+            # For debug
+            print(f"Expecting: {calc_status_list}")
+            print(f"Received:  {H['cstat']}\n")
 
-        assert np.array_equal(H["cstat"], calc_status_list), "Error - unexpected calc status. Received: " + str(
-            H["cstat"]
-        )
+            assert np.array_equal(H["cstat"], calc_status_list), "Error - unexpected calc status. Received: " + str(
+                H["cstat"]
+            )
 
-        print("\n\n\nRun completed.")
+            print("\n\n\nRun completed.")
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_comms.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_comms.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     assert libE_specs["comms"] == "mpi", "This test can only be run with mpi comms -- aborting..."
 
     def check_recv(comm, expected_msg):
         msg = comm.recv()
-        assert msg == expected_msg, "Expected {}, received {}".format(expected_msg, msg)
+        assert msg == expected_msg, f"Expected {expected_msg}, received {msg}"
 
     def worker_main(mpi_comm):
         "Worker main routine"
         comm = MPIComm(mpi_comm)
         check_recv(comm, "Hello")
         check_recv(comm, "World")
         check_recv(comm, comm.rank)
@@ -62,15 +62,15 @@
 
     def check_ranks(mpi_comm, test_exp, test_num):
         try:
             rank = mpi_comm.Get_rank()
         except Exception:
             rank = -1
         comm_ranks_in_world = MPI.COMM_WORLD.allgather(rank)
-        print("got {},  exp {} ".format(comm_ranks_in_world, test_exp[test_num]), flush=True)
+        print(f"got {comm_ranks_in_world},  exp {test_exp[test_num]} ", flush=True)
         # This is really testing the test is testing what is it supposed to test
         assert comm_ranks_in_world == test_exp[test_num], (
             "comm_ranks_in_world are: " + str(comm_ranks_in_world) + " Expected: " + str(test_exp[test_num])
         )
         if rank == -1:
             return False
         return True
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners_subnode.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners_subnode.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     nodes_per_worker = 0.5
 
     # For varying size test - relate node count to nworkers
     nsim_workers = nworkers
 
     if not (nsim_workers * nodes_per_worker).is_integer():
-        sys.exit("Sim workers ({}) must divide evenly into nodes".format(nsim_workers))
+        sys.exit(f"Sim workers ({nsim_workers}) must divide evenly into nodes")
 
     comms = libE_specs["comms"]
     node_file = "nodelist_mpi_runners_subnode_comms_" + str(comms) + "_wrks_" + str(nworkers)
     nnodes = int(nsim_workers * nodes_per_worker)
 
     # Mock up system
     custom_resources = {
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners_subnode_uneven.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners_subnode_uneven.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,15 @@
     log_file = "ensemble_mpi_runners_subnode_uneven_comms_" + str(comms) + "_wrks_" + str(nworkers) + ".log"
     logger.set_filename(log_file)
 
     # For varying size test - relate node count to nworkers
     nsim_workers = nworkers
 
     if nsim_workers % 2 == 0:
-        sys.exit(
-            "This test must be run with an odd of workers >= 3 and <= 31. There are {} workers.".format(nsim_workers)
-        )
+        sys.exit(f"This test must be run with an odd of workers >= 3 and <= 31. There are {nsim_workers} workers.")
 
     comms = libE_specs["comms"]
     node_file = "nodelist_mpi_runners_subnode_uneven_comms_" + str(comms) + "_wrks_" + str(nworkers)
     nnodes = 2
 
     if is_manager:
         create_node_file(num_nodes=nnodes, name=node_file)
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners_supernode_uneven.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners_supernode_uneven.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners_zrw_subnode_uneven.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners_zrw_supernode_uneven.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """
-Runs libEnsemble testing the MPI Runners command creation with uneven workers per node.
+Runs libEnsemble testing the MPI Runners command creation with multiple and uneven nodes per worker.
 
-This test must be run on an even number of workers >= 4 and <= 32 (e.g. odd no. of procs when using mpi4py).
+This test must be run on a number of workers >= 3.
 
 Execute via one of the following commands (e.g. 6 workers - one is zero resource):
-   mpiexec -np 7 python test_mpi_runners_zrw_subnode_uneven.py
-   python test_mpi_runners_zrw_subnode_uneven.py --nworkers 6 --comms local
-   python test_mpi_runners_zrw_subnode_uneven.py --nworkers 6 --comms tcp
+   mpiexec -np 7 python test_mpi_runners_zrw_supernode_uneven.py
+   python test_mpi_runners_zrw_supernode_uneven.py --nworkers 6 --comms local
 """
 
-import sys
 import numpy as np
 
 from libensemble.libE import libE
 from libensemble.sim_funcs.run_line_check import runline_check_by_worker as sim_f
 from libensemble.gen_funcs.persistent_sampling import persistent_uniform as gen_f
 from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens as alloc_f
 from libensemble.tools import parse_args, add_unique_random_streams
@@ -22,53 +20,47 @@
 from libensemble import logger
 
 # logger.set_level('DEBUG')  # For testing the test
 logger.set_level("INFO")
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: mpi local
-# TESTSUITE_NPROCS: 5 7
+# TESTSUITE_NPROCS: 4 5 6
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     nworkers, is_manager, libE_specs, _ = parse_args()
     rounds = 1
     sim_app = "/path/to/fakeapp.x"
     comms = libE_specs["comms"]
 
     libE_specs["zero_resource_workers"] = [1]
     libE_specs["dedicated_mode"] = True
     libE_specs["enforce_worker_core_bounds"] = True
 
     # To allow visual checking - log file not used in test
-    log_file = "ensemble_mpi_runners_zrw_subnode_uneven_comms_" + str(comms) + "_wrks_" + str(nworkers) + ".log"
+    log_file = "ensemble_mpi_runners_zrw_supernode_uneven_comms_" + str(comms) + "_wrks_" + str(nworkers) + ".log"
     logger.set_filename(log_file)
 
+    nodes_per_worker = 2.5
+
     # For varying size test - relate node count to nworkers
     in_place = libE_specs["zero_resource_workers"]
     n_gens = len(in_place)
     nsim_workers = nworkers - n_gens
-
-    if nsim_workers % 2 == 0:
-        sys.exit(
-            "This test must be run with an odd number of sim workers >= 3 and <= 31. There are {} sim workers.".format(
-                nsim_workers
-            )
-        )
-
     comms = libE_specs["comms"]
-    node_file = "nodelist_mpi_runners_zrw_subnode_uneven_comms_" + str(comms) + "_wrks_" + str(nworkers)
-    nnodes = 2
+    node_file = "nodelist_mpi_runners_zrw_supernode_uneven_comms_" + str(comms) + "_wrks_" + str(nworkers)
+    nnodes = int(nsim_workers * nodes_per_worker)
 
     # Mock up system
     custom_resources = {
         "cores_on_node": (16, 64),  # Tuple (physical cores, logical cores)
-        "node_file": node_file,
-    }  # Name of file containing a node-list
+        "node_file": node_file,  # Name of file containing a node-list
+    }
     libE_specs["resource_info"] = custom_resources
 
     if is_manager:
         create_node_file(num_nodes=nnodes, name=node_file)
 
     if comms == "mpi":
         libE_specs["mpi_comm"].Barrier()
@@ -95,47 +87,53 @@
         },
     }
 
     alloc_specs = {"alloc_f": alloc_f, "out": []}
     persis_info = add_unique_random_streams({}, nworkers + 1)
     exit_criteria = {"sim_max": (nsim_workers) * rounds}
 
+    # Each worker has either 3 or 2 nodes. Basic test list for portable options
     test_list_base = [
         {"testid": "base1"},  # Give no config and no extra_args
     ]
 
-    # Example: On 5 workers, runlines should be ...
+    # Example: On 3 workers, runlines should be ...
+    # (one workers has 3 nodes, the other 2 - does not split 2.5 nodes each).
     # [w1]: Gen only
-    # [w2]: srun -w node-1 --ntasks 5 --nodes 1 --ntasks-per-node 5 /path/to/fakeapp.x --testid base1
-    # [w3]: srun -w node-1 --ntasks 5 --nodes 1 --ntasks-per-node 5 /path/to/fakeapp.x --testid base1
-    # [w4]: srun -w node-1 --ntasks 5 --nodes 1 --ntasks-per-node 5 /path/to/fakeapp.x --testid base1
-    # [w5]: srun -w node-2 --ntasks 8 --nodes 1 --ntasks-per-node 8 /path/to/fakeapp.x --testid base1
-    # [w6]: srun -w node-2 --ntasks 8 --nodes 1 --ntasks-per-node 8 /path/to/fakeapp.x --testid base1
+    # [w2]: srun -w node-1,node-2,node-3 --ntasks 48 --nodes 3 --ntasks-per-node 16 /path/to/fakeapp.x --testid base1
+    # [w3]: srun -w node-4,node-5 --ntasks 32 --nodes 2 --ntasks-per-node 16 /path/to/fakeapp.x --testid base1
 
     srun_p1 = "srun -w "
     srun_p2 = " --ntasks "
-    srun_p3 = " --nodes 1 --ntasks-per-node "
-    srun_p4 = " /path/to/fakeapp.x --testid base1"
+    srun_p3 = " --nodes "
+    srun_p4 = " --ntasks-per-node 16 /path/to/fakeapp.x --testid base1"
 
     exp_tasks = []
     exp_srun = []
 
     # Hard coding an example for 2 nodes to avoid replicating general logic in libEnsemble.
-    low_wpn = nsim_workers // nnodes
-    high_wpn = nsim_workers // nnodes + 1
+    low_npw = nnodes // nsim_workers
+    high_npw = nnodes // nsim_workers + 1
+
+    nodelist = []
+    for i in range(1, nnodes + 1):
+        nodelist.append("node-" + str(i))
 
+    inode = 0
     for i in range(nsim_workers):
-        if i < (nsim_workers // nnodes + 1):
-            nodename = "node-1"
-            ntasks = 16 // high_wpn
+        if i < (nsim_workers // 2):
+            npw = high_npw
         else:
-            nodename = "node-2"
-            ntasks = 16 // low_wpn
+            npw = low_npw
+        nodename = ",".join(nodelist[inode : inode + npw])
+        inode += npw
+        ntasks = 16 * npw
+        loc_nodes = npw
         exp_tasks.append(ntasks)
-        exp_srun.append(srun_p1 + str(nodename) + srun_p2 + str(ntasks) + srun_p3 + str(ntasks) + srun_p4)
+        exp_srun.append(srun_p1 + str(nodename) + srun_p2 + str(ntasks) + srun_p3 + str(loc_nodes) + srun_p4)
 
     test_list = test_list_base
     exp_list = exp_srun
     sim_specs["user"] = {
         "tests": test_list,
         "expect": exp_list,
         "persis_gens": n_gens,
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_mpi_runners_zrw_supernode_uneven.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_mpi_runners_zrw_subnode_uneven.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 """
-Runs libEnsemble testing the MPI Runners command creation with multiple and uneven nodes per worker.
+Runs libEnsemble testing the MPI Runners command creation with uneven workers per node.
 
-This test must be run on a number of workers >= 3.
+This test must be run on an even number of workers >= 4 and <= 32 (e.g. odd no. of procs when using mpi4py).
 
 Execute via one of the following commands (e.g. 6 workers - one is zero resource):
-   mpiexec -np 7 python test_mpi_runners_zrw_supernode_uneven.py
-   python test_mpi_runners_zrw_supernode_uneven.py --nworkers 6 --comms local
+   mpiexec -np 7 python test_mpi_runners_zrw_subnode_uneven.py
+   python test_mpi_runners_zrw_subnode_uneven.py --nworkers 6 --comms local
+   python test_mpi_runners_zrw_subnode_uneven.py --nworkers 6 --comms tcp
+
+The resource sets are split unevenly between the two nodes (e.g. 3 and 2).
+
+Two tests are run. In the first, num_resource_sets is used, and thus the dynamic scheduler.
+This will fill node two slots first as there are fewer resource sets on node two, and the
+scheduler will preference a smaller space for assigning the task. On the second test,
+zero_resource_workers are used, and the static scheduler will fill node one first.
 """
 
+import sys
 import numpy as np
 
 from libensemble.libE import libE
 from libensemble.sim_funcs.run_line_check import runline_check_by_worker as sim_f
 from libensemble.gen_funcs.persistent_sampling import persistent_uniform as gen_f
 from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens as alloc_f
 from libensemble.tools import parse_args, add_unique_random_streams
@@ -20,47 +29,51 @@
 from libensemble import logger
 
 # logger.set_level('DEBUG')  # For testing the test
 logger.set_level("INFO")
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: mpi local
-# TESTSUITE_NPROCS: 4 5 6
+# TESTSUITE_NPROCS: 5 7
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     nworkers, is_manager, libE_specs, _ = parse_args()
     rounds = 1
     sim_app = "/path/to/fakeapp.x"
     comms = libE_specs["comms"]
 
-    libE_specs["zero_resource_workers"] = [1]
     libE_specs["dedicated_mode"] = True
     libE_specs["enforce_worker_core_bounds"] = True
 
     # To allow visual checking - log file not used in test
-    log_file = "ensemble_mpi_runners_zrw_supernode_uneven_comms_" + str(comms) + "_wrks_" + str(nworkers) + ".log"
+    log_file = "ensemble_mpi_runners_zrw_subnode_uneven_comms_" + str(comms) + "_wrks_" + str(nworkers) + ".log"
     logger.set_filename(log_file)
 
-    nodes_per_worker = 2.5
-
     # For varying size test - relate node count to nworkers
-    in_place = libE_specs["zero_resource_workers"]
-    n_gens = len(in_place)
+    n_gens = 1
     nsim_workers = nworkers - n_gens
+
+    if nsim_workers % 2 == 0:
+        sys.exit(
+            "This test must be run with an odd number of sim workers >= 3 and <= 31. There are {} sim workers.".format(
+                nsim_workers
+            )
+        )
+
     comms = libE_specs["comms"]
-    node_file = "nodelist_mpi_runners_zrw_supernode_uneven_comms_" + str(comms) + "_wrks_" + str(nworkers)
-    nnodes = int(nsim_workers * nodes_per_worker)
+    node_file = "nodelist_mpi_runners_zrw_subnode_uneven_comms_" + str(comms) + "_wrks_" + str(nworkers)
+    nnodes = 2
 
     # Mock up system
     custom_resources = {
         "cores_on_node": (16, 64),  # Tuple (physical cores, logical cores)
-        "node_file": node_file,  # Name of file containing a node-list
-    }
+        "node_file": node_file,
+    }  # Name of file containing a node-list
     libE_specs["resource_info"] = custom_resources
 
     if is_manager:
         create_node_file(num_nodes=nnodes, name=node_file)
 
     if comms == "mpi":
         libE_specs["mpi_comm"].Barrier()
@@ -84,62 +97,70 @@
             "initial_batch_size": 20,
             "lb": np.array([-3, -2]),
             "ub": np.array([3, 2]),
         },
     }
 
     alloc_specs = {"alloc_f": alloc_f, "out": []}
-    persis_info = add_unique_random_streams({}, nworkers + 1)
     exit_criteria = {"sim_max": (nsim_workers) * rounds}
 
-    # Each worker has either 3 or 2 nodes. Basic test list for portable options
     test_list_base = [
         {"testid": "base1"},  # Give no config and no extra_args
     ]
 
-    # Example: On 3 workers, runlines should be ...
-    # (one workers has 3 nodes, the other 2 - does not split 2.5 nodes each).
+    # Example: On 5 workers, runlines should be ...
     # [w1]: Gen only
-    # [w2]: srun -w node-1,node-2,node-3 --ntasks 48 --nodes 3 --ntasks-per-node 16 /path/to/fakeapp.x --testid base1
-    # [w3]: srun -w node-4,node-5 --ntasks 32 --nodes 2 --ntasks-per-node 16 /path/to/fakeapp.x --testid base1
+    # [w2]: srun -w node-1 --ntasks 5 --nodes 1 --ntasks-per-node 5 /path/to/fakeapp.x --testid base1
+    # [w3]: srun -w node-1 --ntasks 5 --nodes 1 --ntasks-per-node 5 /path/to/fakeapp.x --testid base1
+    # [w4]: srun -w node-1 --ntasks 5 --nodes 1 --ntasks-per-node 5 /path/to/fakeapp.x --testid base1
+    # [w5]: srun -w node-2 --ntasks 8 --nodes 1 --ntasks-per-node 8 /path/to/fakeapp.x --testid base1
+    # [w6]: srun -w node-2 --ntasks 8 --nodes 1 --ntasks-per-node 8 /path/to/fakeapp.x --testid base1
 
     srun_p1 = "srun -w "
     srun_p2 = " --ntasks "
-    srun_p3 = " --nodes "
-    srun_p4 = " --ntasks-per-node 16 /path/to/fakeapp.x --testid base1"
+    srun_p3 = " --nodes 1 --ntasks-per-node "
+    srun_p4 = " /path/to/fakeapp.x --testid base1"
 
     exp_tasks = []
     exp_srun = []
 
     # Hard coding an example for 2 nodes to avoid replicating general logic in libEnsemble.
-    low_npw = nnodes // nsim_workers
-    high_npw = nnodes // nsim_workers + 1
+    low_wpn = nsim_workers // nnodes
+    high_wpn = nsim_workers // nnodes + 1
 
-    nodelist = []
-    for i in range(1, nnodes + 1):
-        nodelist.append("node-" + str(i))
-
-    inode = 0
     for i in range(nsim_workers):
-        if i < (nsim_workers // 2):
-            npw = high_npw
+        if i < (nsim_workers // nnodes + 1):
+            nodename = "node-1"
+            ntasks = 16 // high_wpn
         else:
-            npw = low_npw
-        nodename = ",".join(nodelist[inode : inode + npw])
-        inode += npw
-        ntasks = 16 * npw
-        loc_nodes = npw
+            nodename = "node-2"
+            ntasks = 16 // low_wpn
         exp_tasks.append(ntasks)
-        exp_srun.append(srun_p1 + str(nodename) + srun_p2 + str(ntasks) + srun_p3 + str(loc_nodes) + srun_p4)
+        exp_srun.append(srun_p1 + str(nodename) + srun_p2 + str(ntasks) + srun_p3 + str(ntasks) + srun_p4)
 
     test_list = test_list_base
     exp_list = exp_srun
     sim_specs["user"] = {
         "tests": test_list,
         "expect": exp_list,
         "persis_gens": n_gens,
     }
 
-    # Perform the run
-    H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
+    iterations = 2
+    for prob_id in range(iterations):
+
+        if prob_id == 0:
+            # Uses dynamic scheduler - will find node 2 slots first (as fewer)
+            libE_specs["num_resource_sets"] = nworkers - 1  # Any worker can be the gen
+            sim_specs["user"]["offset_for_scheduler"] = True  # Changes expected values
+            persis_info = add_unique_random_streams({}, nworkers + 1)
 
-    # All asserts are in sim func
+        else:
+            # Uses static scheduler - will find node 1 slots first
+            del libE_specs["num_resource_sets"]
+            libE_specs["zero_resource_workers"] = [1]  # Gen must be worker 1
+            sim_specs["user"]["offset_for_scheduler"] = False
+            persis_info = add_unique_random_streams({}, nworkers + 1)
+
+        # Perform the run
+        H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
+        # Run-line asserts are in sim func
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_runlines_adaptive_workers.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,17 @@
 from libensemble.tests.regression_tests.common import create_node_file
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
-    libE_specs["zero_resource_workers"] = [1]
-    num_gens = len(libE_specs["zero_resource_workers"])
+    num_gens = 1
+    libE_specs["num_resource_sets"] = nworkers - num_gens  # Any worker can be the gen
+
     total_nodes = (nworkers - num_gens) // 4  # 4 resourced workers per node.
 
     if total_nodes == 1:
         max_rsets = 4  # Up to one node
     else:
         max_rsets = 6  # Will expand to 2 full nodes
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent_oversubscribe_rsets.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent_oversubscribe_rsets.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     libE_specs["zero_resource_workers"] = [1]
     rsets = nsim_workers * 2
     libE_specs["num_resource_sets"] = rsets
 
     num_gens = len(libE_specs["zero_resource_workers"])
     total_nodes = (nworkers - num_gens) // 2  # 2 resourced workers per node.
 
-    print("sim_workers: {}.  rsets: {}.  Nodes: {}".format(nsim_workers, rsets, total_nodes), flush=True)
+    print(f"sim_workers: {nsim_workers}.  rsets: {rsets}.  Nodes: {total_nodes}", flush=True)
 
     if total_nodes == 1:
         max_rsets = 4  # Up to one node
     else:
         max_rsets = 6  # Will expand to 2 full nodes
 
     sim_app = helloworld.__file__
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_sim_dirs_per_calc.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_sim_dirs_per_worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
-Runs libEnsemble with uniform random sampling and writes results into sim
-dirs. This tests per-calculation sim_dir capabilities
+Runs libEnsemble with uniform random sampling and writes results into sim dirs.
+This tests per-worker or per-calculation sim_input_dir copying capabilities
 
 Execute via one of the following commands (e.g. 3 workers):
-   mpiexec -np 4 python test_sim_dirs_per_calc.py
-   python test_sim_dirs_per_calc.py --nworkers 3 --comms local
-   python test_sim_dirs_per_calc.py --nworkers 3 --comms tcp
+   mpiexec -np 4 python test_sim_dirs_per_worker.py
+   python test_sim_dirs_per_worker.py --nworkers 3 --comms local
+   python test_sim_dirs_per_worker.py --nworkers 3 --comms tcp
 
 The number of concurrent evaluations of the objective function will be 4-1=3.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: mpi local tcp
 # TESTSUITE_NPROCS: 2 4
+# TESTSUITE_EXTRA: true
 
 import numpy as np
 import os
 
 from libensemble.libE import libE
 from libensemble.tests.regression_tests.support import write_sim_func as sim_f
 from libensemble.gen_funcs.sampling import uniform_random_sample as gen_f
@@ -26,24 +27,24 @@
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     sim_input_dir = "./sim_input_dir"
     dir_to_copy = sim_input_dir + "/copy_this"
     dir_to_symlink = sim_input_dir + "/symlink_this"
-    c_ensemble = "./ensemble_calcdirs_w" + str(nworkers) + "_" + libE_specs.get("comms")
-    print("creating ensemble dir: ", c_ensemble, flush=True)
+    w_ensemble = "./ensemble_workdirs_w" + str(nworkers) + "_" + libE_specs.get("comms")
+    print("creating ensemble dir: ", w_ensemble, flush=True)
 
     for dir in [sim_input_dir, dir_to_copy, dir_to_symlink]:
         if not os.path.isdir(dir):
             os.makedirs(dir, exist_ok=True)
 
     libE_specs["sim_dirs_make"] = True
-    libE_specs["ensemble_dir_path"] = c_ensemble
-    libE_specs["use_worker_dirs"] = False
+    libE_specs["ensemble_dir_path"] = w_ensemble
+    libE_specs["use_worker_dirs"] = True
     libE_specs["sim_dir_copy_files"] = [dir_to_copy]
     libE_specs["sim_dir_symlink_files"] = [dir_to_symlink]
     libE_specs["ensemble_copy_back"] = True
 
     sim_specs = {
         "sim_f": sim_f,
         "in": ["x"],
@@ -63,28 +64,33 @@
     persis_info = add_unique_random_streams({}, nworkers + 1)
 
     exit_criteria = {"sim_max": 21}
 
     H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs)
 
     if is_manager:
-        assert os.path.isdir(c_ensemble), "Ensemble directory {} not created.".format(c_ensemble)
-        dir_sum = sum(["sim" in i for i in os.listdir(c_ensemble)])
-        assert (
-            dir_sum == exit_criteria["sim_max"]
-        ), "Number of sim directories ({}) does not match sim_max ({}).".format(dir_sum, exit_criteria["sim_max"])
+        assert os.path.isdir(w_ensemble), f"Ensemble directory {w_ensemble} not created."
+        worker_dir_sum = sum(["worker" in i for i in os.listdir(w_ensemble)])
+        assert worker_dir_sum == nworkers, "Number of worker dirs ({}) does not match nworkers ({}).".format(
+            worker_dir_sum, nworkers
+        )
 
         input_copied = []
+        sim_dir_sum = 0
 
-        for base, files, _ in os.walk(c_ensemble):
+        for base, files, _ in os.walk(w_ensemble):
             basedir = base.split("/")[-1]
             if basedir.startswith("sim"):
+                sim_dir_sum += 1
                 input_copied.append(
                     all(
                         [
                             os.path.basename(j) in files
                             for j in libE_specs["sim_dir_copy_files"] + libE_specs["sim_dir_symlink_files"]
                         ]
                     )
                 )
 
+        assert (
+            sim_dir_sum == exit_criteria["sim_max"]
+        ), f"Number of sim directories ({sim_dir_sum}) does not match sim_max ({exit_criteria['sim_max']})."
         assert all(input_copied), "Exact input files not copied or symlinked to each calculation directory"
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_sim_dirs_per_worker.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_sim_dirs_per_calc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
-Runs libEnsemble with uniform random sampling and writes results into sim dirs.
-This tests per-worker or per-calculation sim_input_dir copying capabilities
+Runs libEnsemble with uniform random sampling and writes results into sim
+dirs. This tests per-calculation sim_dir capabilities
 
 Execute via one of the following commands (e.g. 3 workers):
-   mpiexec -np 4 python test_sim_dirs_per_worker.py
-   python test_sim_dirs_per_worker.py --nworkers 3 --comms local
-   python test_sim_dirs_per_worker.py --nworkers 3 --comms tcp
+   mpiexec -np 4 python test_sim_dirs_per_calc.py
+   python test_sim_dirs_per_calc.py --nworkers 3 --comms local
+   python test_sim_dirs_per_calc.py --nworkers 3 --comms tcp
 
 The number of concurrent evaluations of the objective function will be 4-1=3.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: mpi local tcp
 # TESTSUITE_NPROCS: 2 4
@@ -26,24 +26,24 @@
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     sim_input_dir = "./sim_input_dir"
     dir_to_copy = sim_input_dir + "/copy_this"
     dir_to_symlink = sim_input_dir + "/symlink_this"
-    w_ensemble = "./ensemble_workdirs_w" + str(nworkers) + "_" + libE_specs.get("comms")
-    print("creating ensemble dir: ", w_ensemble, flush=True)
+    c_ensemble = "./ensemble_calcdirs_w" + str(nworkers) + "_" + libE_specs.get("comms")
+    print("creating ensemble dir: ", c_ensemble, flush=True)
 
     for dir in [sim_input_dir, dir_to_copy, dir_to_symlink]:
         if not os.path.isdir(dir):
             os.makedirs(dir, exist_ok=True)
 
     libE_specs["sim_dirs_make"] = True
-    libE_specs["ensemble_dir_path"] = w_ensemble
-    libE_specs["use_worker_dirs"] = True
+    libE_specs["ensemble_dir_path"] = c_ensemble
+    libE_specs["use_worker_dirs"] = False
     libE_specs["sim_dir_copy_files"] = [dir_to_copy]
     libE_specs["sim_dir_symlink_files"] = [dir_to_symlink]
     libE_specs["ensemble_copy_back"] = True
 
     sim_specs = {
         "sim_f": sim_f,
         "in": ["x"],
@@ -63,33 +63,28 @@
     persis_info = add_unique_random_streams({}, nworkers + 1)
 
     exit_criteria = {"sim_max": 21}
 
     H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs)
 
     if is_manager:
-        assert os.path.isdir(w_ensemble), "Ensemble directory {} not created.".format(w_ensemble)
-        worker_dir_sum = sum(["worker" in i for i in os.listdir(w_ensemble)])
-        assert worker_dir_sum == nworkers, "Number of worker dirs ({}) does not match nworkers ({}).".format(
-            worker_dir_sum, nworkers
-        )
+        assert os.path.isdir(c_ensemble), f"Ensemble directory {c_ensemble} not created."
+        dir_sum = sum(["sim" in i for i in os.listdir(c_ensemble)])
+        assert (
+            dir_sum == exit_criteria["sim_max"]
+        ), f"Number of sim directories ({dir_sum}) does not match sim_max ({exit_criteria['sim_max']})."
 
         input_copied = []
-        sim_dir_sum = 0
 
-        for base, files, _ in os.walk(w_ensemble):
+        for base, files, _ in os.walk(c_ensemble):
             basedir = base.split("/")[-1]
             if basedir.startswith("sim"):
-                sim_dir_sum += 1
                 input_copied.append(
                     all(
                         [
                             os.path.basename(j) in files
                             for j in libE_specs["sim_dir_copy_files"] + libE_specs["sim_dir_symlink_files"]
                         ]
                     )
                 )
 
-        assert (
-            sim_dir_sum == exit_criteria["sim_max"]
-        ), "Number of sim directories ({}) does not match sim_max ({}).".format(sim_dir_sum, exit_criteria["sim_max"])
         assert all(input_copied), "Exact input files not copied or symlinked to each calculation directory"
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_sim_dirs_with_exception.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_sim_dirs_with_exception.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,12 +57,12 @@
 
     exit_criteria = {"sim_max": 21}
 
     return_flag = 1
     try:
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs)
     except LoggedException as e:
-        print("Caught deliberate exception: {}".format(e))
+        print(f"Caught deliberate exception: {e}")
         return_flag = 0
 
     if is_manager:
         assert return_flag == 0
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_sim_dirs_with_gen_dirs.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_sim_dirs_with_gen_dirs.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,22 +88,22 @@
                         [
                             os.path.basename(j) in files
                             for j in libE_specs[type + "_dir_copy_files"] + libE_specs[type + "_dir_symlink_files"]
                         ]
                     )
                 )
 
-        assert all(input_copied), "All input files not copied or symlinked to each {} calc dir".format(type)
+        assert all(input_copied), f"All input files not copied or symlinked to each {type} calc dir"
 
     if is_manager:
-        assert os.path.isdir(c_ensemble), "Ensemble directory {} not created.".format(c_ensemble)
+        assert os.path.isdir(c_ensemble), f"Ensemble directory {c_ensemble} not created."
         sim_dir_sum = sum(["sim" in i for i in os.listdir(c_ensemble)])
         assert (
             sim_dir_sum == exit_criteria["sim_max"]
-        ), "Number of sim directories ({}) does not match sim_max ({}).".format(sim_dir_sum, exit_criteria["sim_max"])
+        ), f"Number of sim directories ({sim_dir_sum}) does not match sim_max ({exit_criteria['sim_max']})."
 
         assert any(["gen" in i for i in os.listdir(c_ensemble)]), "No gen directories created."
 
         check_copied("sim")
         check_copied("gen")
 
         assert all(
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_sim_input_dir_option.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_sim_input_dir_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,13 +60,13 @@
     persis_info = add_unique_random_streams({}, nworkers + 1)
 
     exit_criteria = {"sim_max": 21}
 
     H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs)
 
     if is_manager:
-        assert os.path.isdir(o_ensemble), "Ensemble directory {} not created.".format(o_ensemble)
+        assert os.path.isdir(o_ensemble), f"Ensemble directory {o_ensemble} not created."
         assert os.path.basename(dir_to_copy) in os.listdir(o_ensemble), "Input file not copied over."
         with open(os.path.join(o_ensemble, "test_sim_out.txt"), "r") as f:
             lines = f.readlines()
 
         assert len(lines) == exit_criteria["sim_max"], "Sim output not written to ensemble dir for each sim call"
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_worker_exceptions.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_worker_exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,12 +54,12 @@
     exit_criteria = {"wallclock_max": 10}
 
     # Perform the run
     return_flag = 1
     try:
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs)
     except LoggedException as e:
-        print("Caught deliberate exception: {}".format(e))
+        print(f"Caught deliberate exception: {e}")
         return_flag = 0
 
     if is_manager:
         assert return_flag == 0
```

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_zero_resource_workers.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_zero_resource_workers.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/functionality_tests/test_zero_resource_workers_subnode.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_zero_resource_workers_subnode.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     # For varying size test - relate node count to nworkers
     in_place = libE_specs["zero_resource_workers"]
     n_gens = len(in_place)
     nsim_workers = nworkers - n_gens
 
     if not (nsim_workers * nodes_per_worker).is_integer():
-        sys.exit("Sim workers ({}) must divide evenly into nodes".format(nsim_workers))
+        sys.exit(f"Sim workers ({nsim_workers}) must divide evenly into nodes")
 
     comms = libE_specs["comms"]
     node_file = "nodelist_zero_resource_workers_subnode_comms_" + str(comms) + "_wrks_" + str(nworkers)
     nnodes = int(nsim_workers * nodes_per_worker)
 
     # Mock up system
     custom_resources = {
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/common.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     import balsam
 
     rcfile = os.path.abspath("./libensemble/tests/regression_tests/.bal_coveragerc")
 
     old_line = "            path = ' '.join((exe, script_path, args))\n"
     new_line = (
         "            path = ' '.join((exe, '-m coverage run "
-        + "--parallel-mode --rcfile={}', script_path, args))\n".format(rcfile)
+        + f"--parallel-mode --rcfile={rcfile}', script_path, args))\n"
     )
 
     commandfile = "cli_commands.py"
     balsam_path = os.path.dirname(balsam.__file__) + "/scripts"
     balsam_commands_path = os.path.join(balsam_path, commandfile)
 
     with open(balsam_commands_path, "r") as f:
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/dont_run_test_persistent_aposmm_pounders.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_pounders.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 def combine_component(x):
     return np.sum(np.power(x, 2))
 
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/dont_run_test_persistent_aposmm_tao_blmvm.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_tao_blmvm.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
 from libensemble.tests.regression_tests.support import six_hump_camel_minima as minima
 from time import time
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if is_manager:
         start_time = time()
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/dont_run_test_persistent_aposmm_tao_nm.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_tao_nm.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 from libensemble.alloc_funcs.persistent_aposmm_alloc import persistent_aposmm_alloc as alloc_f
 from libensemble.tools import parse_args, add_unique_random_streams
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/dont_run_test_persistent_gp.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_gp.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/script_test_balsam_hworld.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/script_test_balsam_hworld.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     if is_manager:
         print("\nChecking expected task status against Workers ...\n")
         calc_status_list_in = np.asarray(
             [WORKER_DONE, WORKER_KILL_ON_ERR, WORKER_DONE, WORKER_KILL_ON_TIMEOUT, TASK_FAILED]
         )
         calc_status_list = np.repeat(calc_status_list_in, nworkers)
 
-        print("Expecting: {}".format(calc_status_list))
-        print("Received:  {}\n".format(H["cstat"]))
+        print(f"Expecting: {calc_status_list}")
+        print(f"Received:  {H['cstat']}\n")
 
         assert np.array_equal(H["cstat"], calc_status_list), "Error - unexpected calc status. Received: " + str(
             H["cstat"]
         )
 
         # Check dry_run submissions inside ensemble.log
         with open("ensemble.log", "r") as f:
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ECnoise.m` & `libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ECnoise.m`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m` & `libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/configure-balsam-test.sh` & `libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/configure-balsam-test.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/test_balsam_hworld.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/scripts_used_by_reg_tests/test_balsam_hworld.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # This test is NOT submitted as a job to Balsam. script_test_balsam_hworld.py is
 #   the executable submitted to Balsam as a job. This test executes that job
 #   through the 'runstr' line in run_Balsam_job()
 
 
 def run_Balsam_job():
     runstr = "balsam launcher --consume-all --job-mode=mpi --num-transition-threads=1"
-    print("Executing Balsam job with command: {}".format(runstr))
+    print(f"Executing Balsam job with command: {runstr}")
     subprocess.Popen(runstr.split())
 
 
 def build_simfunc():
     buildstring = "mpicc -o my_simtask.x ../unit_tests/simdir/my_simtask.c"
     subprocess.check_call(buildstring.split())
 
@@ -32,48 +32,48 @@
     print("Waiting for Balsam Database directory.")
     while sleeptime < limit:
         if os.path.isdir(basedb):
             break
         time.sleep(1)
         sleeptime += 1
 
-    assert sleeptime < limit, "Balsam Database directory not created within {} seconds.".format(limit)
+    assert sleeptime < limit, f"Balsam Database directory not created within {limit} seconds."
 
     # Stop sleeping once job directory detected within database directory
-    print("Waiting for Job Directory {}".format(sleeptime))
+    print(f"Waiting for Job Directory {sleeptime}")
     while sleeptime < limit:
         if len(os.listdir(basedb)) > 0:
             break
         print(sleeptime, end=" ", flush=True)
         time.sleep(1)
         sleeptime += 1
 
-    assert sleeptime < limit, "Balsam Job directory not created within {} seconds.".format(limit)
+    assert sleeptime < limit, f"Balsam Job directory not created within {limit} seconds."
 
     # Assumes database dir was empty, now contains single job dir
     jobdir = os.path.join(basedb, os.listdir(basedb)[0])
     return jobdir
 
 
 def wait_for_job_output(jobdir):
     sleeptime = 0
     limit = 60
 
     output = os.path.join(jobdir, "job_script_test_balsam_hworld.out")
-    print("Checking for Balsam output file: {}".format(output))
+    print(f"Checking for Balsam output file: {output}")
 
     while sleeptime < limit:
         if os.path.isfile(output):
             break
         print(sleeptime, end=" ", flush=True)
         print(os.listdir(jobdir), flush=True)
         time.sleep(1)
         sleeptime += 1
 
-    assert sleeptime < limit, "Balsam output file not created within {} seconds.".format(limit)
+    assert sleeptime < limit, f"Balsam output file not created within {limit} seconds."
 
     return output
 
 
 def print_job_output(outscript):
     sleeptime = 0
     limit = 90
@@ -90,15 +90,15 @@
         if succeed_line in lines:
             print("Success. Received task statuses match expected.")
             break
 
         time.sleep(1)
         sleeptime += 1
 
-    assert sleeptime < limit, "Expected Balsam Job output-file contents not detected after {} seconds.".format(limit)
+    assert sleeptime < limit, f"Expected Balsam Job output-file contents not detected after {limit} seconds."
 
 
 def move_job_coverage(jobdir):
     # Move coverage files from Balsam DB to ./regression_tests (for concatenation)
     print("Moving job coverage results.")
     here = os.getcwd()
     covname = ".cov_reg_out."
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/support.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/support.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,50 +28,50 @@
     return (H, persis_info)
 
 
 def write_sim_func(calc_in, persis_info, sim_specs, libE_info):
     out = np.zeros(1, dtype=sim_specs["out"])
     out["f"] = calc_in["x"]
     with open("test_sim_out.txt", "a") as f:
-        f.write("sim_f received: {}\n".format(out["f"]))
+        f.write(f"sim_f received: {out['f']}\n")
     return out, persis_info
 
 
 def remote_write_sim_func(calc_in, persis_info, sim_specs, libE_info):
     import numpy as np
 
     out = np.zeros(1, dtype=sim_specs["out"])
     calc_dir = sim_specs["user"]["calc_dir"]
     out["f"] = calc_in["x"]
     with open(calc_dir + "/test_sim_out.txt", "a") as f:
-        f.write("sim_f received: {}\n".format(out["f"]))
+        f.write(f"sim_f received: {out['f']}\n")
     return out, persis_info
 
 
 def remote_write_gen_func(calc_in, persis_info, gen_specs, libE_info):
     import socket
     import secrets
     import numpy as np
 
     H_o = np.zeros(1, dtype=gen_specs["out"])
     H_o["x"] = socket.gethostname() + "_" + secrets.token_hex(nbytes=3)
     with open("test_gen_out.txt", "a") as f:
-        f.write("gen_f produced: {}\n".format(H_o["x"]))
+        f.write(f"gen_f produced: {H_o['x']}\n")
     return H_o, persis_info
 
 
 def write_uniform_gen_func(H, persis_info, gen_specs, _):
     ub = gen_specs["user"]["ub"]
     lb = gen_specs["user"]["lb"]
     n = len(lb)
     b = gen_specs["user"]["gen_batch_size"]
     H_o = np.zeros(b, dtype=gen_specs["out"])
     H_o["x"] = persis_info["rand_stream"].uniform(lb, ub, (b, n))
     with open("test_gen_out.txt", "a") as f:
-        f.write("gen_f produced: {}\n".format(H_o["x"]))
+        f.write(f"gen_f produced: {H_o['x']}\n")
     return H_o, persis_info
 
 
 uniform_or_localopt_gen_out = [
     ("priority", float),
     ("local_pt", bool),
     ("known_to_aposmm", bool),
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_1d_sampling.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_1d_sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_1d_sampling_with_profile.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_executor_simple.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,82 @@
 """
-Runs libEnsemble 1D sampling test with worker profiling.
+Runs libEnsemble testing the executor functionality.
 
 Execute via one of the following commands (e.g. 3 workers):
-   mpiexec -np 4 python test_1d_sampling_with_profile.py
-   python test_1d_sampling_with_profile.py --nworkers 3 --comms local
-   python test_1d_sampling_with_profile.py --nworkers 3 --comms tcp
+   mpiexec -np 4 python test_executor_hworld.py
+   python test_executor_hworld.py --nworkers 3 --comms local
+   python test_executor_hworld.py --nworkers 3 --comms tcp
 
 The number of concurrent evaluations of the objective function will be 4-1=3.
 """
 
-# Do not change these lines - they are parsed by run-tests.sh
-# TESTSUITE_COMMS: mpi local tcp
-# TESTSUITE_NPROCS: 2 4
-# TESTSUITE_EXTRA: true
-
 import numpy as np
-import os
-import time
 
+# Import libEnsemble items for this test
+from libensemble.message_numbers import WORKER_DONE
 from libensemble.libE import libE
-from libensemble.sim_funcs.one_d_func import one_d_example as sim_f
-from libensemble.gen_funcs.sampling import latin_hypercube_sample as gen_f
+from libensemble.sim_funcs.executor_hworld import executor_hworld as sim_f
+import libensemble.sim_funcs.six_hump_camel as six_hump_camel
+from libensemble.gen_funcs.sampling import uniform_random_sample as gen_f
 from libensemble.tools import parse_args, add_unique_random_streams
+from libensemble.executors.mpi_executor import MPIExecutor
+
+
+# Do not change these lines - they are parsed by run-tests.sh
+# TESTSUITE_COMMS: mpi local
+# TESTSUITE_NPROCS: 4
+# TESTSUITE_OMPI_SKIP: true
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
-    libE_specs["profile"] = True
+    cores_per_task = 1
+    cores_all_tasks = nworkers * cores_per_task
+
+    sim_app2 = six_hump_camel.__file__
+
+    exctr = MPIExecutor()
+    exctr.register_app(full_path=sim_app2, app_name="six_hump_camel", calc_type="sim")  # Named app
 
     sim_specs = {
         "sim_f": sim_f,
         "in": ["x"],
-        "out": [("f", float)],
+        "out": [("f", float), ("cstat", int)],
+        "user": {"cores": cores_per_task},
     }
 
     gen_specs = {
         "gen_f": gen_f,
-        "out": [("x", float, (1,))],
+        "in": ["sim_id"],
+        "out": [("x", float, (2,))],
         "user": {
-            "gen_batch_size": 500,
-            "lb": np.array([-3]),
-            "ub": np.array([3]),
+            "lb": np.array([-3, -2]),
+            "ub": np.array([3, 2]),
+            "gen_batch_size": nworkers,
         },
     }
 
     persis_info = add_unique_random_streams({}, nworkers + 1)
 
-    exit_criteria = {"gen_max": 501}
+    # num sim_ended_count conditions in executor_hworld
+    exit_criteria = {"sim_max": nworkers * 5}
 
     # Perform the run
     H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs)
 
     if is_manager:
-        assert len(H) >= 501
-        print("\nlibEnsemble with random sampling has generated enough points")
+        print("\nChecking expected task status against Workers ...\n")
 
-        assert "manager.prof" in os.listdir(), "Expected manager profile not found after run"
-        os.remove("manager.prof")
+        calc_status_list_in = np.asarray([WORKER_DONE] * 5)
+        calc_status_list = np.repeat(calc_status_list_in, nworkers)
 
-        prof_files = ["worker_{}.prof".format(i + 1) for i in range(nworkers)]
+        # For debug
+        print(f"Expecting: {calc_status_list}")
+        print(f"Received:  {H['cstat']}\n")
 
-        # Ensure profile writes complete before checking
-        time.sleep(0.5)
-
-        for file in prof_files:
-            assert file in os.listdir(), "Expected profile {} not found after run".format(file)
-            with open(file, "r") as f:
-                data = f.read().split()
-                num_worker_funcs_profiled = sum(["worker" in i for i in data])
-            assert num_worker_funcs_profiled >= 8, (
-                "Insufficient number of " + "worker functions profiled: " + str(num_worker_funcs_profiled)
-            )
+        assert np.array_equal(H["cstat"], calc_status_list), "Error - unexpected calc status. Received: " + str(
+            H["cstat"]
+        )
 
-            os.remove(file)
+        print("\n\n\nRun completed.")
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_evaluate_existing_sample.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_evaluate_existing_sample.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_evaluate_mixed_sample.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_evaluate_mixed_sample.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_fast_alloc.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_nlopt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,100 @@
 """
-Tests various capabilities of the libEnsemble fast_alloc alloc_f
+Runs libEnsemble with APOSMM with the NLopt local optimizer.
 
 Execute via one of the following commands (e.g. 3 workers):
-   mpiexec -np 4 python test_fast_alloc.py
-   python test_fast_alloc.py --nworkers 3 --comms local
-
-The number of concurrent evaluations of the objective function will be 4-1=3.
+   mpiexec -np 4 python test_persistent_aposmm_nlopt.py
+   python test_persistent_aposmm_nlopt.py --nworkers 3 --comms local
+   python test_persistent_aposmm_nlopt.py --nworkers 3 --comms tcp
+
+When running with the above commands, the number of concurrent evaluations of
+the objective function will be 2, as one of the three workers will be the
+persistent generator.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
-# TESTSUITE_COMMS: mpi local
-# TESTSUITE_NPROCS: 2 4
+# TESTSUITE_COMMS: local mpi tcp
+# TESTSUITE_NPROCS: 3
 
 import sys
-import gc
 import numpy as np
 
 # Import libEnsemble items for this test
 from libensemble.libE import libE
-from libensemble.sim_funcs.six_hump_camel import six_hump_camel_simple as sim_f
-from libensemble.gen_funcs.sampling import uniform_random_sample as gen_f
-from libensemble.alloc_funcs.fast_alloc import give_sim_work_first as alloc_f
-from libensemble.alloc_funcs.only_one_gen_alloc import ensure_one_active_gen as alloc_f2
-from libensemble.tools import parse_args, add_unique_random_streams
+from math import gamma, pi, sqrt
+from libensemble.sim_funcs.six_hump_camel import six_hump_camel as sim_f
+
+import libensemble.gen_funcs
+
+libensemble.gen_funcs.rc.aposmm_optimizers = "nlopt"
+from libensemble.gen_funcs.persistent_aposmm import aposmm as gen_f
+
+from libensemble.alloc_funcs.persistent_aposmm_alloc import persistent_aposmm_alloc as alloc_f
+from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
+from libensemble.tests.regression_tests.support import six_hump_camel_minima as minima
+from time import time
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
-    num_pts = 30 * (nworkers)
+    if is_manager:
+        start_time = time()
 
+    if nworkers < 2:
+        sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
+
+    n = 2
     sim_specs = {
         "sim_f": sim_f,
         "in": ["x"],
-        "out": [("f", float), ("large", float, 1000000)],
-        "user": {},
+        "out": [("f", float)],
     }
 
+    gen_out = [
+        ("x", float, n),
+        ("x_on_cube", float, n),
+        ("sim_id", int),
+        ("local_min", bool),
+        ("local_pt", bool),
+    ]
+
     gen_specs = {
         "gen_f": gen_f,
-        "in": ["sim_id"],
-        "out": [("x", float, (2,))],
+        "persis_in": ["f"] + [n[0] for n in gen_out],
+        "out": gen_out,
         "user": {
-            "gen_batch_size": num_pts,
+            "initial_sample_size": 100,
+            "sample_points": np.round(minima, 1),
+            "localopt_method": "LN_BOBYQA",
+            "rk_const": 0.5 * ((gamma(1 + (n / 2)) * 5) ** (1 / n)) / sqrt(pi),
+            "xtol_abs": 1e-6,
+            "ftol_abs": 1e-6,
+            "dist_to_bound_multiple": 0.5,
+            "max_active_runs": 6,
             "lb": np.array([-3, -2]),
             "ub": np.array([3, 2]),
         },
     }
 
+    alloc_specs = {"alloc_f": alloc_f}
+
     persis_info = add_unique_random_streams({}, nworkers + 1)
 
-    exit_criteria = {"sim_max": 2 * num_pts, "wallclock_max": 300}
+    exit_criteria = {"sim_max": 2000}
+
+    # Perform the run
+    H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
-    if libE_specs["comms"] == "tcp":
-        # Can't use the same interface for manager and worker if we want
-        # repeated calls to libE -- the manager sets up a different server
-        # each time, and the worker will not know what port to connect to.
-        sys.exit("Cannot run with tcp when repeated calls to libE -- aborting...")
-
-    for time in np.append([0], np.logspace(-5, -1, 5)):
-        print("Starting for time: ", time, flush=True)
-        if time == 0:
-            alloc_specs = {"alloc_f": alloc_f2, "out": []}
-        else:
-            alloc_specs = {"alloc_f": alloc_f, "out": [], "user": {"num_active_gens": 1}}
-
-        for rep in range(1):
-            sim_specs["user"]["pause_time"] = time
-
-            if time == 0:
-                sim_specs["user"].pop("pause_time")
-                gen_specs["user"]["gen_batch_size"] = num_pts // 2
-
-            persis_info["next_to_give"] = 0
-            persis_info["total_gen_calls"] = 1
-
-            H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
-
-            if is_manager:
-                assert flag == 0
-                assert len(H) == 2 * num_pts
+    if is_manager:
+        print("[Manager]:", H[np.where(H["local_min"])]["x"])
+        print("[Manager]: Time taken =", time() - start_time, flush=True)
+
+        tol = 1e-5
+        for m in minima:
+            # The minima are known on this test problem.
+            # We use their values to test APOSMM has identified all minima
+            print(np.min(np.sum((H[H["local_min"]]["x"] - m) ** 2, 1)), flush=True)
+            assert np.min(np.sum((H[H["local_min"]]["x"] - m) ** 2, 1)) < tol
 
-            del H
-            gc.collect()  # If doing multiple libE calls, users might need to clean up their memory space.
+        save_libE_output(H, persis_info, __file__, nworkers)
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_heffte.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_heffte.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_inverse_bayes_example.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_inverse_bayes_example.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_dfols.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_dfols.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 def combine_component(x):
     return np.sum(np.power(x, 2))
 
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_exception.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         assert passed
         print("\n\nException received as expected")
 
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_external_localopt.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_external_localopt.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 persistent generator.
 
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: local mpi tcp
 # TESTSUITE_NPROCS: 4
-# TESTSUITE_OS_SKIP: OSX
+# TESTSUITE_OS_SKIP: OSX WIN
 # TESTSUITE_EXTRA: true
 
 import sys
 import multiprocessing
 import numpy as np
 import shutil  # For copying the external_localopt script
 
@@ -42,15 +42,14 @@
 from time import time
 
 np.set_printoptions(precision=16)
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if is_manager:
         start_time = time()
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_nlopt.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_timeout.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 """
-Runs libEnsemble with APOSMM with the NLopt local optimizer.
+Test the APOSMM generator function's capabilities to properly exit when a
+timeout has occurred.
 
 Execute via one of the following commands (e.g. 3 workers):
-   mpiexec -np 4 python test_persistent_aposmm_nlopt.py
-   python test_persistent_aposmm_nlopt.py --nworkers 3 --comms local
-   python test_persistent_aposmm_nlopt.py --nworkers 3 --comms tcp
+   mpiexec -np 4 python test_persistent_aposmm_timeout.py
+   python test_persistent_aposmm_timeout.py --nworkers 3 --comms local
+   python test_persistent_aposmm_timeout.py --nworkers 3 --comms tcp
 
 When running with the above commands, the number of concurrent evaluations of
 the objective function will be 2, as one of the three workers will be the
 persistent generator.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
 # TESTSUITE_COMMS: local mpi tcp
-# TESTSUITE_NPROCS: 3
+# TESTSUITE_NPROCS: 4
 # TESTSUITE_EXTRA: true
 
 import sys
 import multiprocessing
 import numpy as np
 
-# Import libEnsemble items for this test
-from libensemble.libE import libE
-from math import gamma, pi, sqrt
-from libensemble.sim_funcs.six_hump_camel import six_hump_camel as sim_f
-
 import libensemble.gen_funcs
 
 libensemble.gen_funcs.rc.aposmm_optimizers = "nlopt"
-from libensemble.gen_funcs.persistent_aposmm import aposmm as gen_f
 
+# Import libEnsemble items for this test
+from libensemble.libE import libE
+from libensemble.sim_funcs.periodic_func import func_wrapper as sim_f
+from libensemble.gen_funcs.persistent_aposmm import aposmm as gen_f
 from libensemble.alloc_funcs.persistent_aposmm_alloc import persistent_aposmm_alloc as alloc_f
-from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
-from libensemble.tests.regression_tests.support import six_hump_camel_minima as minima
-from time import time
+from libensemble.tools import parse_args, add_unique_random_streams, save_libE_output
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
-    if is_manager:
-        start_time = time()
-
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
 
     n = 2
     sim_specs = {
         "sim_f": sim_f,
         "in": ["x"],
@@ -66,40 +59,33 @@
 
     gen_specs = {
         "gen_f": gen_f,
         "persis_in": ["f"] + [n[0] for n in gen_out],
         "out": gen_out,
         "user": {
             "initial_sample_size": 100,
-            "sample_points": np.round(minima, 1),
             "localopt_method": "LN_BOBYQA",
-            "rk_const": 0.5 * ((gamma(1 + (n / 2)) * 5) ** (1 / n)) / sqrt(pi),
-            "xtol_abs": 1e-6,
-            "ftol_abs": 1e-6,
-            "dist_to_bound_multiple": 0.5,
-            "max_active_runs": 6,
-            "lb": np.array([-3, -2]),
-            "ub": np.array([3, 2]),
+            "xtol_abs": 1e-8,
+            "ftol_abs": 1e-8,
+            "run_max_eval": 30,
+            "lb": np.array([0, -np.pi / 2]),
+            "ub": np.array([2 * np.pi, 3 * np.pi / 2]),
+            "periodic": True,
+            "print": True,
         },
     }
 
     alloc_specs = {"alloc_f": alloc_f}
 
-    persis_info = add_unique_random_streams({}, nworkers + 1)
+    # Setting a very high sim_max value and a short wallclock_max so timeout will occur
+    exit_criteria = {"sim_max": 50000, "wallclock_max": 5}
 
-    exit_criteria = {"sim_max": 2000}
+    persis_info = add_unique_random_streams({}, nworkers + 1)
 
     # Perform the run
     H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
     if is_manager:
-        print("[Manager]:", H[np.where(H["local_min"])]["x"])
-        print("[Manager]: Time taken =", time() - start_time, flush=True)
-
-        tol = 1e-5
-        for m in minima:
-            # The minima are known on this test problem.
-            # We use their values to test APOSMM has identified all minima
-            print(np.min(np.sum((H[H["local_min"]]["x"] - m) ** 2, 1)), flush=True)
-            assert np.min(np.sum((H[H["local_min"]]["x"] - m) ** 2, 1)) < tol
-
+        assert flag == 2, "Test should have timed out"
+        assert persis_info[1].get("run_order"), "Run_order should have been given back"
+        min_ids = np.where(H["local_min"])
         save_libE_output(H, persis_info, __file__, nworkers)
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_periodic.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_periodic.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from libensemble.sim_funcs.periodic_func import func_wrapper as sim_f
 from libensemble.alloc_funcs.persistent_aposmm_alloc import persistent_aposmm_alloc as alloc_f
 from libensemble.tools import parse_args, add_unique_random_streams
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_scipy.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_scipy.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
 from libensemble.tests.regression_tests.support import six_hump_camel_minima as minima
 from time import time
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if is_manager:
         start_time = time()
 
@@ -105,15 +104,15 @@
             min_found = 0
             for m in minima:
                 # The minima are known on this test problem.
                 # We use their values to test APOSMM has identified all minima
                 print(np.min(np.sum((H[H["local_min"]]["x"] - m) ** 2, 1)), flush=True)
                 if np.min(np.sum((H[H["local_min"]]["x"] - m) ** 2, 1)) < tol:
                     min_found += 1
-            assert min_found >= 4, "Found {} minima".format(min_found)
+            assert min_found >= 4, f"Found {min_found} minima"
 
             save_libE_output(H, persis_info, __file__, nworkers)
 
     # Now let's run on the same problem with a really large n (but we won't test
     # convergence to all local min). Note that sim_f uses only entries x[0:2]
     n = 400
     persis_info = add_unique_random_streams({}, nworkers + 1)
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_timeout.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_fd_param_finder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,80 @@
 """
-Test the APOSMM generator function's capabilities to properly exit when a
-timeout has occurred.
+Runs libEnsemble with the fd_param_finder persistent gen_f, which finds an
+appropriate finite-difference parameter for the sim_f mapping from R^n to R^p
+around the point x.
 
 Execute via one of the following commands (e.g. 3 workers):
-   mpiexec -np 4 python test_persistent_aposmm_timeout.py
-   python test_persistent_aposmm_timeout.py --nworkers 3 --comms local
-   python test_persistent_aposmm_timeout.py --nworkers 3 --comms tcp
+   mpiexec -np 4 python test_persistent_fd_param_finder.py
 
-When running with the above commands, the number of concurrent evaluations of
+When running with the above command, the number of concurrent evaluations of
 the objective function will be 2, as one of the three workers will be the
 persistent generator.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
-# TESTSUITE_COMMS: local mpi tcp
+# TESTSUITE_COMMS: mpi
 # TESTSUITE_NPROCS: 4
+# TESTSUITE_OS_SKIP: OSX
 # TESTSUITE_EXTRA: true
 
 import sys
-import multiprocessing
 import numpy as np
-
-import libensemble.gen_funcs
-
-libensemble.gen_funcs.rc.aposmm_optimizers = "nlopt"
+import shutil  # For ECnoise.m
 
 # Import libEnsemble items for this test
 from libensemble.libE import libE
-from libensemble.sim_funcs.periodic_func import func_wrapper as sim_f
-from libensemble.gen_funcs.persistent_aposmm import aposmm as gen_f
-from libensemble.alloc_funcs.persistent_aposmm_alloc import persistent_aposmm_alloc as alloc_f
-from libensemble.tools import parse_args, add_unique_random_streams, save_libE_output
+from libensemble.sim_funcs.noisy_vector_mapping import func_wrapper as sim_f, noisy_function
+from libensemble.gen_funcs.persistent_fd_param_finder import fd_param_finder as gen_f
+from libensemble.alloc_funcs.start_fd_persistent import finite_diff_alloc as alloc_f
+from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
-    multiprocessing.set_start_method("fork", force=True)
-
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
 
-    n = 2
+    x0 = np.array([1.23, 4.56])  # point about which we are calculating finite difference parameters
+    f0 = noisy_function(x0)
+    n = len(x0)
+    p = len(f0)
+
     sim_specs = {
         "sim_f": sim_f,
-        "in": ["x"],
-        "out": [("f", float)],
+        "in": ["x", "f_ind"],
+        "out": [("f_val", float)],
     }
 
-    gen_out = [
-        ("x", float, n),
-        ("x_on_cube", float, n),
-        ("sim_id", int),
-        ("local_min", bool),
-        ("local_pt", bool),
-    ]
-
+    # The initial noise_h_mat is chosen to ECNoise both grows and shrinks the fd param
     gen_specs = {
         "gen_f": gen_f,
-        "persis_in": ["f"] + [n[0] for n in gen_out],
-        "out": gen_out,
+        "persis_in": ["x", "f_val", "n_ind", "f_ind", "x_ind", "sim_id"],
+        "out": [("x", float, (n,)), ("n_ind", int), ("f_ind", int), ("x_ind", int)],
         "user": {
-            "initial_sample_size": 100,
-            "localopt_method": "LN_BOBYQA",
-            "xtol_abs": 1e-8,
-            "ftol_abs": 1e-8,
-            "run_max_eval": 30,
-            "lb": np.array([0, -np.pi / 2]),
-            "ub": np.array([2 * np.pi, 3 * np.pi / 2]),
-            "periodic": True,
-            "print": True,
+            "x0": x0,
+            "f0": f0,
+            "nf": 10,
+            "p": p,
+            "n": n,
+            "noise_h_mat": np.multiply(np.logspace(-16, -1, p), np.ones((n, p))),
+            "maxnoiseits": 3,
         },
     }
+    shutil.copy("./scripts_used_by_reg_tests/ECnoise.m", "./")
 
     alloc_specs = {"alloc_f": alloc_f}
 
-    # Setting a very high sim_max value and a short wallclock_max so timeout will occur
-    exit_criteria = {"sim_max": 50000, "wallclock_max": 5}
-
     persis_info = add_unique_random_streams({}, nworkers + 1)
 
+    exit_criteria = {"gen_max": 1000}
+
     # Perform the run
     H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
     if is_manager:
-        assert flag == 2, "Test should have timed out"
-        assert persis_info[1].get("run_order"), "Run_order should have been given back"
-        min_ids = np.where(H["local_min"])
+        assert len(H) < exit_criteria["gen_max"], "Problem didn't stop early, which should have been the case."
+        assert np.all(persis_info[1]["Fnoise"] > 0), "gen_f didn't find noise for all F_i components."
+
         save_libE_output(H, persis_info, __file__, nworkers)
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_aposmm_with_grad.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_aposmm_with_grad.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
 from libensemble.tests.regression_tests.support import six_hump_camel_minima as minima
 from time import time
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Temporary solution while we investigate/resolve slowdowns with "spawn" start method.
     multiprocessing.set_start_method("fork", force=True)
 
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     if is_manager:
         start_time = time()
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_fd_param_finder.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/persistent_gp/run_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,101 @@
 """
-Runs libEnsemble with the fd_param_finder persistent gen_f, which finds an
-appropriate finite-difference parameter for the sim_f mapping from R^n to R^p
-around the point x.
-
-Execute via one of the following commands (e.g. 3 workers):
-   mpiexec -np 4 python test_persistent_fd_param_finder.py
-
-When running with the above command, the number of concurrent evaluations of
-the objective function will be 2, as one of the three workers will be the
-persistent generator.
-"""
+Example of optimization using a persistent GP gen_func, with multi-fidelity
 
-# Do not change these lines - they are parsed by run-tests.sh
-# TESTSUITE_COMMS: mpi
-# TESTSUITE_NPROCS: 4
-# TESTSUITE_OS_SKIP: OSX
-# TESTSUITE_EXTRA: true
+Usage:
+------
+python run_example.py --comms local --nworkers 4
+"""
 
-import sys
 import numpy as np
-import shutil  # For ECnoise.m
-
-# Import libEnsemble items for this test
 from libensemble.libE import libE
-from libensemble.sim_funcs.noisy_vector_mapping import func_wrapper as sim_f, noisy_function
-from libensemble.gen_funcs.persistent_fd_param_finder import fd_param_finder as gen_f
-from libensemble.alloc_funcs.start_fd_persistent import finite_diff_alloc as alloc_f
-from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
-
-# Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
-if __name__ == "__main__":
-
-    nworkers, is_manager, libE_specs, _ = parse_args()
-
-    if nworkers < 2:
-        sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
-
-    x0 = np.array([1.23, 4.56])  # point about which we are calculating finite difference parameters
-    f0 = noisy_function(x0)
-    n = len(x0)
-    p = len(f0)
-
-    sim_specs = {
-        "sim_f": sim_f,
-        "in": ["x", "f_ind"],
-        "out": [("f_val", float)],
-    }
-
-    # The initial noise_h_mat is chosen to ECNoise both grows and shrinks the fd param
-    gen_specs = {
-        "gen_f": gen_f,
-        "persis_in": ["x", "f_val", "n_ind", "f_ind", "x_ind", "sim_id"],
-        "out": [("x", float, (n,)), ("n_ind", int), ("f_ind", int), ("x_ind", int)],
-        "user": {
-            "x0": x0,
-            "f0": f0,
-            "nf": 10,
-            "p": p,
-            "n": n,
-            "noise_h_mat": np.multiply(np.logspace(-16, -1, p), np.ones((n, p))),
-            "maxnoiseits": 3,
-        },
-    }
-    shutil.copy("./scripts_used_by_reg_tests/ECnoise.m", "./")
-
-    alloc_specs = {"alloc_f": alloc_f}
-
-    persis_info = add_unique_random_streams({}, nworkers + 1)
-
-    exit_criteria = {"gen_max": 1000}
-
-    # Perform the run
-    H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
-
-    if is_manager:
-        assert len(H) < exit_criteria["gen_max"], "Problem didn't stop early, which should have been the case."
-        assert np.all(persis_info[1]["Fnoise"] > 0), "gen_f didn't find noise for all F_i components."
-
-        save_libE_output(H, persis_info, __file__, nworkers)
+from libensemble import logger
+from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens
+from libensemble.tools import save_libE_output, add_unique_random_streams
+from libensemble.tools import parse_args
+from libensemble.message_numbers import WORKER_DONE
+from libensemble.gen_funcs.persistent_ax_multitask import persistent_gp_mt_ax_gen_f
+
+nworkers, is_manager, libE_specs, _ = parse_args()
+
+mt_params = {
+    "name_hifi": "expensive_model",
+    "name_lofi": "cheap_model",
+    "n_init_hifi": 4,
+    "n_init_lofi": 4,
+    "n_opt_hifi": 2,
+    "n_opt_lofi": 4,
+}
+
+
+def run_simulation(H, persis_info, sim_specs, libE_info):
+    # Extract input parameters
+    values = list(H["x"][0])
+    x0 = values[0]
+    x1 = values[1]
+    # Extract fidelity parameter
+    task = H["task"][0]
+    if task == "expensive_model":
+        z = 8
+    elif task == "cheap_model":
+        z = 1
+
+    libE_output = np.zeros(1, dtype=sim_specs["out"])
+    calc_status = WORKER_DONE
+
+    # Function that depends on the resolution parameter
+    libE_output["f"] = -(x0 + 10 * np.cos(x0 + 0.1 * z)) * (x1 + 5 * np.cos(x1 - 0.2 * z))
+
+    return libE_output, persis_info, calc_status
+
+
+sim_specs = {
+    "sim_f": run_simulation,
+    "in": ["x", "task"],
+    "out": [("f", float)],
+}
+
+gen_specs = {
+    # Generator function. Will randomly generate new sim inputs 'x'.
+    "gen_f": persistent_gp_mt_ax_gen_f,
+    # Generator input. This is a RNG, no need for inputs.
+    "in": ["sim_id", "x", "f", "task"],
+    "persis_in": ["sim_id", "x", "f", "task"],
+    "out": [
+        # parameters to input into the simulation.
+        ("x", float, (2,)),
+        ("task", str, max([len(mt_params["name_hifi"]), len(mt_params["name_lofi"])])),
+        ("resource_sets", int),
+    ],
+    "user": {
+        "range": [1, 8],
+        # Total max number of sims running concurrently.
+        "gen_batch_size": nworkers - 1,
+        # Lower bound for the n parameters.
+        "lb": np.array([0, 0]),
+        # Upper bound for the n parameters.
+        "ub": np.array([15, 15]),
+    },
+}
+gen_specs["user"] = {**gen_specs["user"], **mt_params}
+
+alloc_specs = {
+    "alloc_f": only_persistent_gens,
+    "out": [("gen_informed", bool)],
+    "user": {"async_return": False},
+}
+
+# libE logger
+logger.set_level("INFO")
+
+# Exit criteria
+exit_criteria = {"sim_max": 20}  # Exit after running sim_max simulations
+
+# Create a different random number stream for each worker and the manager
+persis_info = add_unique_random_streams({}, nworkers + 1)
+
+# Run LibEnsemble, and store results in history array H
+H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
+
+# Save results to numpy file
+if is_manager:
+    save_libE_output(H, persis_info, __file__, nworkers)
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_gp_multitask_ax.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_gp_multitask_ax.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,56 +22,59 @@
 import numpy as np
 from libensemble.libE import libE
 from libensemble import logger
 from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens
 from libensemble.tools import save_libE_output, add_unique_random_streams
 from libensemble.tools import parse_args
 from libensemble.message_numbers import WORKER_DONE
-from libensemble.gen_funcs.persistent_ax_multitask import persistent_gp_mt_ax_gen_f
 
 import warnings
 
+# Ax uses a deprecated warn command.
+warnings.filterwarnings("ignore", category=UserWarning)
+warnings.filterwarnings("ignore", category=DeprecationWarning)
+
+from libensemble.gen_funcs.persistent_ax_multitask import persistent_gp_mt_ax_gen_f
+
+
+def run_simulation(H, persis_info, sim_specs, libE_info):
+    # Extract input parameters
+    values = list(H["x"][0])
+    x0 = values[0]
+    x1 = values[1]
+    # Extract fidelity parameter
+    task = H["task"][0]
+    if task == "expensive_model":
+        z = 8
+    elif task == "cheap_model":
+        z = 1
+
+    libE_output = np.zeros(1, dtype=sim_specs["out"])
+    calc_status = WORKER_DONE
+
+    # Function that depends on the resolution parameter
+    libE_output["f"] = -(x0 + 10 * np.cos(x0 + 0.1 * z)) * (x1 + 5 * np.cos(x1 - 0.2 * z))
+
+    return libE_output, persis_info, calc_status
+
+
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
-    # Ax uses a deprecated warn command.
-    warnings.filterwarnings("ignore", category=UserWarning)
-    warnings.filterwarnings("ignore", category=DeprecationWarning)
-
     nworkers, is_manager, libE_specs, _ = parse_args()
 
     mt_params = {
         "name_hifi": "expensive_model",
         "name_lofi": "cheap_model",
         "n_init_hifi": 4,
         "n_init_lofi": 4,
         "n_opt_hifi": 2,
         "n_opt_lofi": 4,
     }
 
-    def run_simulation(H, persis_info, sim_specs, libE_info):
-        # Extract input parameters
-        values = list(H["x"][0])
-        x0 = values[0]
-        x1 = values[1]
-        # Extract fidelity parameter
-        task = H["task"][0]
-        if task == "expensive_model":
-            z = 8
-        elif task == "cheap_model":
-            z = 1
-
-        libE_output = np.zeros(1, dtype=sim_specs["out"])
-        calc_status = WORKER_DONE
-
-        # Function that depends on the resolution parameter
-        libE_output["f"] = -(x0 + 10 * np.cos(x0 + 0.1 * z)) * (x1 + 5 * np.cos(x1 - 0.2 * z))
-
-        return libE_output, persis_info, calc_status
-
     sim_specs = {
         "sim_f": run_simulation,
         "in": ["x", "task"],
         "out": [("f", float)],
     }
 
     gen_specs = {
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_independent.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_independent.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_n_agent.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_n_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                 "rho": rho,
                 "N_const": N_const,  # multiplicative constant on numiters
                 "step_const": 1,
             }
         )
 
         if is_manager:
-            print("=== Optimizing {} ===".format(prob_name), flush=True)
+            print(f"=== Optimizing {prob_name} ===", flush=True)
 
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
         if is_manager:
             print("=== End algorithm ===", flush=True)
 
             # check we completed
@@ -232,8 +232,8 @@
 
             A_kron_I = spp.kron(A, spp.eye(n))
             consensus_val = np.dot(x, A_kron_I.dot(x))
 
             assert F - fstar < err_const * eps, "Error of {:.4e}, expected {:.4e} (assuming f*={:.4e})".format(
                 F - fstar, err_const * eps, fstar
             )
-            assert consensus_val < eps, "Consensus score of {:.4e}, expected {:.4e}\nx={}".format(consensus_val, eps, x)
+            assert consensus_val < eps, f"Consensus score of {consensus_val:.4e}, expected {eps:.4e}\nx={x}"
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_pds.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_pds.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                 "Vx_0x": n**0.5,  # Bregman divergence of x_0 and x_*
                 "eps": eps,  # error / tolerance
                 "A_norm": lam_max,  # ||A \otimes I||_2 = ||A||_2
             }
         )
 
         if is_manager:
-            print("=== Optimizing {} ===".format(prob_name), flush=True)
+            print(f"=== Optimizing {prob_name} ===", flush=True)
 
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
         if is_manager:
             print("=== End algorithm ===", flush=True)
 
             # check we completed
@@ -230,8 +230,8 @@
 
             A_kron_I = spp.kron(A, spp.eye(n))
             consensus_val = np.dot(x, A_kron_I.dot(x))
 
             assert F - fstar < err_const * eps, "Error of {:.4e}, expected {:.4e} (assuming f*={:.4e})".format(
                 F - fstar, err_const * eps, fstar
             )
-            assert consensus_val < eps, "Consensus score of {:.4e}, expected {:.4e}".format(consensus_val, eps)
+            assert consensus_val < eps, f"Consensus score of {consensus_val:.4e}, expected {eps:.4e}"
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_prox_slide.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_prox_slide.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
         # Include @f_i_eval and @df_i_eval if we want to compute gradient in gen
         persis_info["gen_params"].update(
             {"M": M, "R": 10**2, "nu": 1, "eps": eps, "D": 2 * n, "N_const": N_const, "lam_max": lam_max}
         )
 
         if is_manager:
-            print("=== Optimizing {} ===".format(prob_name), flush=True)
+            print(f"=== Optimizing {prob_name} ===", flush=True)
 
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
         if is_manager:
             print("=== End algorithm ===", flush=True)
 
             # check we completed
@@ -187,8 +187,8 @@
 
             A_kron_I = spp.kron(A, spp.eye(n))
             consensus_val = np.dot(x, A_kron_I.dot(x))
 
             assert F - fstar < err_const * eps, "Error of {:.4e}, expected {:.4e} (assuming f*={:.4e})".format(
                 F - fstar, err_const * eps, fstar
             )
-            assert consensus_val < eps, "Consensus score of {:.4e}, expected {:.4e}\nx={}".format(consensus_val, eps, x)
+            assert consensus_val < eps, f"Consensus score of {consensus_val:.4e}, expected {eps:.4e}\nx={x}"
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_sampling_CUDA_variable_resources.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_simple/run_libe_forces.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,57 @@
-"""
-Tests CUDA variable resource detection in libEnsemble
-
-Execute via one of the following commands (e.g. 3 workers):
-   mpiexec -np 4 python test_persistent_sampling_CUDA_variable_resources.py
-
-When running with the above command, the number of concurrent evaluations of
-the objective function will be 2, as one of the three workers will be the
-persistent generator.
-"""
-
-# Do not change these lines - they are parsed by run-tests.sh
-# TESTSUITE_COMMS: mpi local
-# TESTSUITE_NPROCS: 4
-
+#!/usr/bin/env python
+import os
 import sys
 import numpy as np
+from forces_simf import run_forces  # Sim func from current dir
 
-# Import libEnsemble items for this test
 from libensemble.libE import libE
-from libensemble.sim_funcs import six_hump_camel
-from libensemble.sim_funcs.six_hump_camel import six_hump_camel_CUDA_variable_resources as sim_f
-from libensemble.gen_funcs.persistent_sampling import uniform_random_sample_with_variable_resources as gen_f
-from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens as alloc_f
-from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
-from libensemble.executors.mpi_executor import MPIExecutor
+from libensemble.gen_funcs.sampling import uniform_random_sample
+from libensemble.tools import parse_args, add_unique_random_streams
+from libensemble.executors import MPIExecutor
 
-# Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
+    # Parse number of workers, comms type, etc. from arguments
     nworkers, is_manager, libE_specs, _ = parse_args()
 
-    libE_specs["zero_resource_workers"] = [1]
-    libE_specs["sim_dirs_make"] = True
-    libE_specs["ensemble_dir_path"] = "./ensemble_CUDA_variable_w" + str(nworkers)
+    # Initialize MPI Executor instance
+    exctr = MPIExecutor()
 
-    if libE_specs["comms"] == "tcp":
-        sys.exit("This test only runs with MPI or local -- aborting...")
+    # Register simulation executable with executor
+    sim_app = os.path.join(os.getcwd(), "../forces_app/forces.x")
 
-    # Get paths for applications to run
-    six_hump_camel_app = six_hump_camel.__file__
-    exctr = MPIExecutor()
-    exctr.register_app(full_path=six_hump_camel_app, app_name="six_hump_camel")
+    if not os.path.isfile(sim_app):
+        sys.exit("forces.x not found - please build first in ../forces_app dir")
 
-    n = 2
+    exctr.register_app(full_path=sim_app, app_name="forces")
+
+    # State the sim_f, inputs, outputs
     sim_specs = {
-        "sim_f": sim_f,
-        "in": ["x"],
-        "out": [("f", float)],
-        "user": {},
+        "sim_f": run_forces,  # sim_f, imported above
+        "in": ["x"],  # Name of input for sim_f
+        "out": [("energy", float)],  # Name, type of output from sim_f
     }
 
+    # State the gen_f, inputs, outputs, additional parameters
     gen_specs = {
-        "gen_f": gen_f,
-        "persis_in": ["f", "x", "sim_id"],
-        "out": [("priority", float), ("resource_sets", int), ("x", float, n)],
+        "gen_f": uniform_random_sample,  # Generator function
+        "in": [],  # Generator input
+        "out": [("x", float, (1,))],  # Name, type and size of data from gen_f
         "user": {
-            "initial_batch_size": nworkers - 1,
-            "max_resource_sets": nworkers - 1,  # Any sim created can req. 1 worker up to all.
-            "lb": np.array([-3, -2]),
-            "ub": np.array([3, 2]),
+            "lb": np.array([1000]),  # User parameters for the gen_f
+            "ub": np.array([3000]),
+            "gen_batch_size": 8,
         },
     }
 
-    alloc_specs = {
-        "alloc_f": alloc_f,
-        "user": {
-            "give_all_with_same_priority": False,
-            "async_return": True,
-        },
-    }
+    # Create and work inside separate per-simulation directories
+    libE_specs["sim_dirs_make"] = True
+
+    # Instruct libEnsemble to exit after this many simulations
+    exit_criteria = {"sim_max": 8}
 
-    libE_specs["scheduler_opts"] = {"match_slots": True}
+    # Seed random streams for each worker, particularly for gen_f
     persis_info = add_unique_random_streams({}, nworkers + 1)
-    exit_criteria = {"sim_max": 40, "wallclock_max": 300}
 
-    # Perform the run
-    H, persis_info, flag = libE(
-        sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs, alloc_specs=alloc_specs
-    )
-
-    if is_manager:
-        assert flag == 0
-        save_libE_output(H, persis_info, __file__, nworkers)
+    # Launch libEnsemble
+    H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info=persis_info, libE_specs=libE_specs)
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_sim_uniform_sampling.py` & `libensemble-0.9.3/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_cancel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,74 @@
 """
-Runs libEnsemble on the 6-hump camel problem. Documented here:
-   https://www.sfu.ca/~ssurjano/camel6.html
+Tests libEnsemble with a simple persistent uniform sampling generator
+function.
 
 Execute via one of the following commands (e.g. 3 workers):
-   mpiexec -np 4 python test_persistent_sim_uniform_sampling.py
-   python test_persistent_sim_uniform_sampling.py --nworkers 3 --comms local
-   python test_persistent_sim_uniform_sampling.py --nworkers 3 --comms tcp
+   mpiexec -np 4 python test_persistent_sampling.py
+   python test_persistent_uniform_sampling_cancel.py --nworkers 3 --comms local
+   python test_persistent_uniform_sampling_cancel.py --nworkers 3 --comms tcp
 
-When running with the above command, the number of concurrent evaluations of
+When running with the above commands, the number of concurrent evaluations of
 the objective function will be 2, as one of the three workers will be the
 persistent generator.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
-# TESTSUITE_COMMS: mpi local tcp
+# TESTSUITE_COMMS: mpi local
 # TESTSUITE_NPROCS: 3 4
 
 import sys
 import numpy as np
 
 # Import libEnsemble items for this test
 from libensemble.libE import libE
-from libensemble.sim_funcs.six_hump_camel import persistent_six_hump_camel as sim_f
-from libensemble.gen_funcs.persistent_sampling import persistent_uniform as gen_f
-from libensemble.alloc_funcs.start_only_persistent import only_persistent_workers as alloc_f
+from libensemble.sim_funcs.rosenbrock import rosenbrock_eval as sim_f
+from libensemble.gen_funcs.persistent_sampling import persistent_uniform_with_cancellations as gen_f
+from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens as alloc_f
 from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
 
-# from libensemble import logger
-# logger.set_level('DEBUG')
-
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
 
     nworkers, is_manager, libE_specs, _ = parse_args()
-    libE_specs["num_resource_sets"] = nworkers - 1  # Only matters if sims use resources.
-
-    # Only used to test returning/overwriting a point at the end of the persistent sim.
-    libE_specs["use_persis_return_sim"] = True
 
     if nworkers < 2:
         sys.exit("Cannot run with a persistent worker if only one worker -- aborting...")
 
     n = 2
 
     sim_specs = {
         "sim_f": sim_f,
         "in": ["x"],
-        "user": {"replace_final_fields": True},
         "out": [("f", float), ("grad", float, n)],
     }
 
     gen_specs = {
         "gen_f": gen_f,
-        "in": [],
-        "persis_in": ["sim_id", "f", "grad"],
+        "persis_in": ["x", "f", "grad", "sim_id"],
         "out": [("x", float, (n,))],
         "user": {
-            "initial_batch_size": 5,
+            "initial_batch_size": 100,
             "lb": np.array([-3, -2]),
             "ub": np.array([3, 2]),
         },
     }
 
-    alloc_specs = {"alloc_f": alloc_f}
+    alloc_specs = {
+        "alloc_f": alloc_f,
+        "user": {"async_return": True},
+    }
 
-    persis_info = add_unique_random_streams({}, nworkers + 1)
+    exit_criteria = {"gen_max": 150, "wallclock_max": 300}
 
-    exit_criteria = {"sim_max": 40, "wallclock_max": 300}
+    persis_info = add_unique_random_streams({}, nworkers + 1)
 
     # Perform the run
     H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
     if is_manager:
-        assert len(np.unique(H["gen_ended_time"])) == 8
-        assert not any((H["f"] == 0))
-        # Should overwrite the last value (in fact last (nworker-1) values) with f(1,1) = 3.23333333
-        assert not np.isclose(H["f"][0], 3.23333333)
-        assert np.isclose(H["f"][-1], 3.23333333)
+
+        # For reproducible test, only tests if cancel requested on points - not whether got evaluated
+        assert np.all(H["cancel_requested"][:49] == False), "Values cancelled which should not be"  # noqa: E712
+        assert np.all(H["cancel_requested"][50:100]), "Values not cancelled which should be"
+
         save_libE_output(H, persis_info, __file__, nworkers)
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_surmise_calib.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_surmise_calib.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,11 +113,11 @@
         sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs=alloc_specs, libE_specs=libE_specs
     )
 
     if is_manager:
         print("Cancelled sims", H["sim_id"][H["cancel_requested"]])
         sims_done = np.count_nonzero(H["sim_ended"])
         save_libE_output(H, persis_info, __file__, nworkers)
-        assert sims_done == max_evals, "Num of completed simulations should be {}. Is {}".format(max_evals, sims_done)
+        assert sims_done == max_evals, f"Num of completed simulations should be {max_evals}. Is {sims_done}"
 
         # The following line is only to cover parts of tstd2theta
         tstd2theta(H[0]["thetas"].squeeze(), hard=False)
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_surmise_killsims.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_surmise_killsims.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,18 @@
 
     # Rename ensemble dir for non-inteference with other regression tests
     libE_specs["ensemble_dir_path"] = "ensemble_calib_kills"
 
     sim_specs = {
         "sim_f": sim_f,
         "in": ["x", "thetas"],
-        "out": [("f", float)],
+        "out": [
+            ("f", float),
+            ("sim_killed", bool),  # "sim_killed" is used only for display at the end of this test
+        ],
         "user": {
             "num_obs": n_x,
             "init_sample_size": init_sample_size,
         },
     }
 
     gen_out = [
@@ -126,11 +129,12 @@
     # Perform the run
     H, persis_info, flag = libE(
         sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs=alloc_specs, libE_specs=libE_specs
     )
 
     if is_manager:
         print("Cancelled sims", H["sim_id"][H["cancel_requested"]])
-        print("Killed sims", H["sim_id"][H["kill_sent"]])
+        print("Kills sent by manager to running simulations", H["sim_id"][H["kill_sent"]])
+        print("Killed sims", H["sim_id"][H["sim_killed"]])
         sims_done = np.count_nonzero(H["sim_ended"])
         save_libE_output(H, persis_info, __file__, nworkers)
-        assert sims_done == max_evals, "Num of completed simulations should be {}. Is {}".format(max_evals, sims_done)
+        assert sims_done == max_evals, f"Num of completed simulations should be {max_evals}. Is {sims_done}"
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_tasmanian.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_tasmanian.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             exit_criteria = {"gen_max": 100}  # This will test persistent_tasmanian stopping early.
 
         # tasmanian_init has to be a method that returns an initialized TasmanianSparseGrid object
         # tasmanian_checkpoint_file will be overwritten between each step of the iterative refinement
         #   the final grid will also be stored in the file
         gen_specs["user"] = {
             "tasmanian_init": tasmanian_init_global if run < 2 else tasmanian_init_localp,
-            "tasmanian_checkpoint_file": "tasmanian{0}.grid".format(run),
+            "tasmanian_checkpoint_file": f"tasmanian{run}.grid",
         }
 
         # setup the refinement criteria
         if run == 0:
             gen_specs["user"]["refinement"] = "none"
 
         if run == 1:
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_persistent_tasmanian_async.py` & `libensemble-0.9.3/libensemble/tests/regression_tests/test_persistent_tasmanian_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,13 +95,13 @@
         sim_specs, gen_specs, alloc_specs, persis_info = get_sparse_grid_specs(user_specs, sim_f, 2, mode="async")
 
         if run_num == 0:
             gen_specs["user"]["tasmanian_checkpoint_file"] = "tasmanian.grid"
             run_num += 1
 
         if is_manager:
-            print("[Manager]: user_specs = {0}".format(user_specs))
-            print("[Manager]: exit_criteria = {0}".format(exit_criteria))
+            print(f"[Manager]: user_specs = {user_specs}")
+            print(f"[Manager]: exit_criteria = {exit_criteria}")
             start_time = time()
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
         if is_manager:
             print("[Manager]: Time taken = ", time() - start_time, "\n", flush=True)
```

### Comparing `libensemble-0.9.2/libensemble/tests/regression_tests/test_stats_output.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,127 +1,126 @@
-"""
-Runs libEnsemble doing uniform sampling with multiple tasks per simulation and
-varying amount of resources, and then checks structure of the libE_stats.txt file.
-
-Execute via one of the following commands (e.g. 3 workers):
-   mpiexec -np 4 python test_stats_output.py
-   python test_stats_output.py --nworkers 3 --comms local
-
-The number of concurrent evaluations of the objective function will be 4-1=3.
-
-Note: This test contains multiple iterations to test different libE_stats outputs.
-"""
-
-# Do not change these lines - they are parsed by run-tests.sh
-# TESTSUITE_COMMS: mpi local
-# TESTSUITE_NPROCS: 2 4
-
+#!/usr/bin/env python
+import os
 import sys
 import numpy as np
+from forces_simf import run_forces  # Sim func from current dir
 
-from check_libE_stats import check_libE_stats
-
-# Import libEnsemble items for this test
+# Import libEnsemble modules
 from libensemble.libE import libE
-from libensemble.sim_funcs import helloworld, six_hump_camel
-from libensemble.sim_funcs.six_hump_camel import six_hump_camel_with_variable_resources as sim_f
+from libensemble.manager import ManagerException
+from libensemble.tools import parse_args, save_libE_output, add_unique_random_streams
+from libensemble import logger
+from forces_support import test_libe_stats, test_ensemble_dir, check_log_exception
 
-from libensemble.gen_funcs.sampling import uniform_random_sample_with_variable_resources as gen_f
+# Note the Balsam option here is now LegacyBalsam - see balsam_forces for latest.
+USE_BALSAM = False
 
-# from libensemble.gen_funcs.sampling import uniform_random_sample_with_var_priorities_and_resources as gen_f
+PERSIS_GEN = False
 
-from libensemble.alloc_funcs.give_sim_work_first import give_sim_work_first
-from libensemble.tools import parse_args, add_unique_random_streams
-from libensemble.executors.mpi_executor import MPIExecutor
+if PERSIS_GEN:
+    from libensemble.gen_funcs.persistent_sampling import persistent_uniform as gen_f
+    from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens as alloc_f
+else:
+    from libensemble.gen_funcs.sampling import uniform_random_sample as gen_f
+    from libensemble.alloc_funcs.give_sim_work_first import give_sim_work_first as alloc_f
 
 
-if __name__ == "__main__":
+logger.set_level("INFO")  # INFO is now default
 
-    nworkers, is_manager, libE_specs, _ = parse_args()
+nworkers, is_manager, libE_specs, _ = parse_args()
 
-    libE_specs["sim_dirs_make"] = True
+sim_app = os.path.join(os.getcwd(), "../forces_app/forces.x")
 
-    if libE_specs["comms"] == "tcp":
-        sys.exit("This test only runs with MPI or local -- aborting...")
+if not os.path.isfile(sim_app):
+    sys.exit("forces.x not found - please build first in ../forces_app dir")
 
-    # Get paths for applications to run
-    hello_world_app = helloworld.__file__
-    six_hump_camel_app = six_hump_camel.__file__
+if is_manager:
+    print(f"\nRunning with {nworkers} workers\n")
 
-    # Sim can run either helloworld or six_hump_camel
-    exctr = MPIExecutor()
-    exctr.register_app(full_path=hello_world_app, app_name="helloworld")
-    exctr.register_app(full_path=six_hump_camel_app, app_name="six_hump_camel")
 
-    n = 2
-    sim_specs = {
-        "sim_f": sim_f,
-        "in": ["x"],
-        "out": [("f", float)],
-        "user": {"app": "helloworld"},  # helloworld or six_hump_camel
-    }
+# Create executor and register sim to it.
+if USE_BALSAM:
+    from libensemble.executors.legacy_balsam_executor import LegacyBalsamMPIExecutor
 
-    gen_specs = {
-        "gen_f": gen_f,
-        "in": ["sim_id"],
-        "out": [
-            ("priority", float),
-            ("resource_sets", int),  # Set in gen func, resourced by alloc func.
-            ("x", float, n),
-            ("x_on_cube", float, n),
-        ],
-        "user": {
-            "gen_batch_size": 5,
-            "max_resource_sets": nworkers,
-            "lb": np.array([-3, -2]),
-            "ub": np.array([3, 2]),
-        },
-    }
+    exctr = LegacyBalsamMPIExecutor()
+else:
+    from libensemble.executors.mpi_executor import MPIExecutor
+
+    exctr = MPIExecutor()
+exctr.register_app(full_path=sim_app, app_name="forces")
 
+# Note: Attributes such as kill_rate are to control forces tests, this would not be a typical parameter.
+
+# State the objective function, its arguments, output, and necessary parameters (and their sizes)
+sim_specs = {
+    "sim_f": run_forces,  # Function whose output is being minimized
+    "in": ["x"],  # Name of input for sim_f
+    "out": [("energy", float)],  # Name, type of output from sim_f
+    "user": {
+        "keys": ["seed"],
+        "cores": 2,
+        "sim_particles": 1e3,
+        "sim_timesteps": 5,
+        "sim_kill_minutes": 10.0,
+        "particle_variance": 0.2,
+        "kill_rate": 0.5,
+        "fail_on_sim": False,
+        "fail_on_submit": False,  # Won't occur if 'fail_on_sim' True
+    },
+}
+# end_sim_specs_rst_tag
+
+# State the generating function, its arguments, output, and necessary parameters.
+gen_specs = {
+    "gen_f": gen_f,  # Generator function
+    "in": [],  # Generator input
+    "out": [("x", float, (1,))],  # Name, type and size of data produced (must match sim_specs 'in')
+    "user": {
+        "lb": np.array([0]),  # Lower bound for random sample array (1D)
+        "ub": np.array([32767]),  # Upper bound for random sample array (1D)
+        "gen_batch_size": 1000,  # How many random samples to generate in one call
+    },
+}
+
+if PERSIS_GEN:
+    alloc_specs = {"alloc_f": alloc_f}
+else:
     alloc_specs = {
-        "alloc_f": give_sim_work_first,
-        "out": [],
+        "alloc_f": alloc_f,
         "user": {
-            "batch_mode": False,
-            "give_all_with_same_priority": True,
-            "num_active_gens": 1,
-            "async_return": True,
+            "batch_mode": True,  # If true wait for all sims to process before generate more
+            "num_active_gens": 1,  # Only one active generator at a time
         },
     }
 
-    # This can improve scheduling when tasks may run across multiple nodes
-    libE_specs["scheduler_opts"] = {"match_slots": False}
-
-    exit_criteria = {"sim_max": 40, "wallclock_max": 300}
-
-    iterations = 2
-
-    # Note that libE_stats.txt output will be appended across libE calls.
-    for prob_id in range(iterations):
-
-        sim_specs["user"]["app"] = "six_hump_camel"
-
-        libE_specs["ensemble_dir_path"] = (
-            "./ensemble_test_stats" + str(nworkers) + "_" + libE_specs.get("comms") + "_" + str(prob_id)
-        )
-
-        if prob_id == 0:
-            libE_specs["stats_fmt"] = {"task_timing": True}  # This adds total time for each task.
-            check_task_datetime = False
-
-        if prob_id == 1:
-            # task_datetime: Include task_timing and start/end times for each task
-            libE_specs["stats_fmt"] = {"task_datetime": True, "show_resource_sets": True}
-            check_task_datetime = True
-
-        persis_info = add_unique_random_streams({}, nworkers + 1)
-
-        # Perform the run
-        H, persis_info, flag = libE(
-            sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs, alloc_specs=alloc_specs
-        )
-
-        if is_manager:
-            assert flag == 0
-            check_libE_stats(task_datetime=check_task_datetime)
-
-            # save_libE_output(H, persis_info, __file__, nworkers)
+libE_specs["save_every_k_gens"] = 1000  # Save every K steps
+libE_specs["sim_dirs_make"] = True  # Separate each sim into a separate directory
+libE_specs["profile"] = False  # Whether to have libE profile on (default False)
+
+# Maximum number of simulations
+sim_max = 8
+exit_criteria = {"sim_max": sim_max}
+
+# Create a different random number stream for each worker and the manager
+persis_info = {}
+persis_info = add_unique_random_streams(persis_info, nworkers + 1)
+
+try:
+    H, persis_info, flag = libE(
+        sim_specs,
+        gen_specs,
+        exit_criteria,
+        persis_info=persis_info,
+        alloc_specs=alloc_specs,
+        libE_specs=libE_specs,
+    )
+
+except ManagerException:
+    if is_manager and sim_specs["user"]["fail_on_sim"]:
+        check_log_exception()
+        test_libe_stats("Exception occurred\n")
+else:
+    if is_manager:
+        save_libE_output(H, persis_info, __file__, nworkers)
+        if sim_specs["user"]["fail_on_submit"]:
+            test_libe_stats("Task Failed\n")
+        test_ensemble_dir(libE_specs, "./ensemble", nworkers, sim_max)
```

### Comparing `libensemble-0.9.2/libensemble/tests/run-tests.sh` & `libensemble-0.9.3/libensemble/tests/run-tests.sh`

 * *Files 1% similar despite different names*

```diff
@@ -88,32 +88,14 @@
   while [ $symbol_count -gt 0 ]
   do
     printf "="
     symbol_count=$((symbol_count-1))
   done
 }
 
-#Get current time in seconds
-#In:  Nothing
-#Out: Returns time in seconds (seconds since 1970-01-01 00:00:00 UTC) as a string
-#     Or if bc not available uses SECONDS (whole seconds that script has been running)
-current_time() {
-  local time
-  #Is bc present
-  USE_BC=f
-  bc --version >> /dev/null && USE_BC=t
-  if [ $USE_BC = 't' ]; then
-    #time=$(date +%s.%N)
-    time=$(python -c 'import time; print(time.time())')
-  else
-    time=$SECONDS
-  fi;
-  echo "$time"
-}
-
 #Return a time difference
 #In:  Start and End times as strings
 #Out: Time difference as a string
 total_time() {
   #Is bc present
   USE_BC=f
   bc --version >> /dev/null && USE_BC=t
@@ -335,14 +317,32 @@
   exit
 fi;
 
 #If not supplied will go to just python (no number) - eg. with tox/virtual envs
 PYTHON_RUN="python$PYTHON_VER $PYTHON_FLAGS"
 echo -e "Python run: $PYTHON_RUN"
 
+#Get current time in seconds
+#In:  Nothing
+#Out: Returns time in seconds (seconds since 1970-01-01 00:00:00 UTC) as a string
+#     Or if bc not available uses SECONDS (whole seconds that script has been running)
+current_time() {
+  local time
+  #Is bc present
+  USE_BC=f
+  bc --version >> /dev/null && USE_BC=t
+  if [ $USE_BC = 't' ]; then
+    #time=$(date +%s.%N)
+    time=$($PYTHON_RUN -c 'import time; print(time.time())')
+  else
+    time=$SECONDS
+  fi;
+  echo "$time"
+}
+
 textreset=$(tput sgr0)
 fail_color=$(tput bold; tput setaf 1) #red
 pass_color=$(tput bold; tput setaf 2) #green
 titl_color=$(tput bold; tput setaf 6) #cyan
 hint_color=$(tput bold; tput setaf 4) #blue
 
 # Note - pytest exit codes
@@ -496,19 +496,24 @@
             NWORKERS=$((NPROCS-1))
 
             RUN_TEST=false
             if [ "$RUN_MPI" = true ]   && [ "$LAUNCHER" = mpi ];   then RUN_TEST=true; fi
             if [ "$RUN_LOCAL" = true ] && [ "$LAUNCHER" = local ]; then RUN_TEST=true; fi
             if [ "$RUN_TCP" = true ]   && [ "$LAUNCHER" = tcp ];   then RUN_TEST=true; fi
 
-            if [[ "$OSTYPE" = *"darwin"* ]] && [[ "$OS_SKIP_LIST" = "OSX" ]]; then
+            if [[ "$OSTYPE" = *"darwin"* ]] && [[ "$OS_SKIP_LIST" = *"OSX"* ]]; then
               echo "Skipping test number for OSX: " $test_num
               continue
             fi
 
+            if [[ "$OSTYPE" = *"msys"* ]] && [[ "$OS_SKIP_LIST" = *"WIN"* ]]; then
+              echo "Skipping test number for Windows: " $test_num
+              continue
+            fi
+
             if [[ "$OMPI_SKIP" = "true" ]] && [[ "$MPIEXEC_FLAGS" = "--oversubscribe" ]] && [[ "$RUN_MPI" = true ]]; then
               echo "Skipping test number for Open MPI: " $test_num
               continue
             fi
 
             if [ $REG_STOP_ON_FAILURE = "true" ]; then
               #Before Each Test check code is 0 (passed so far) - or skip to test summary
```

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/define_apps.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/define_apps.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/forces_simf.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/forces_simf.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         "sim_particles": particles,
         "sim_timesteps": str(10),
         "seed": particles,
     }
 
     workdir = "sim" + str(libE_info["H_rows"][0]) + "_worker" + str(libE_info["workerID"])
 
-    statfile = "forces{}.stat".format(particles)
+    statfile = f"forces{particles}.stat"
 
     if THIS_SCRIPT_ON_THETA:
         transfer_statfile_path = GLOBUS_DEST_DIR + statfile
         local_statfile_path = "../" + workdir + "/" + transfer_statfile_path.split("/")[-1]
     else:
         transfer_statfile_path = os.getcwd() + "/" + statfile
         local_statfile_path = transfer_statfile_path
@@ -47,15 +47,15 @@
         transfers=transfer,
         workdir=workdir,
     )
 
     task.wait(timeout=300)
     task.poll()
 
-    print("Task {} polled. state: {}.".format(task.name, task.state))
+    print(f"Task {task.name} polled. state: {task.state}.")
 
     while True:
         time.sleep(1)
         if os.path.isfile(local_statfile_path) and os.path.getsize(local_statfile_path) > 0:
             break
 
     try:
```

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/readme.md` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/run_libe_forces_balsam.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/run_libe_forces_balsam.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/balsam_forces/submit_libe_forces_remotely.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/balsam_forces/submit_libe_forces_remotely.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/balsam_local.sh` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/balsam_local.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/forces.yaml` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/forces.yaml`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/forces_simf.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/forces_simf.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     particle_variance = sim_specs["user"].get("particle_variance", 0)
 
     # Composing variable names and x values to set up simulation
     seed = int(np.rint(x[0][0]))
 
     # This is to give a random variance of work-load
     sim_particles = perturb(sim_particles, seed, particle_variance)
-    print("seed: {}   particles: {}".format(seed, sim_particles))
+    print(f"seed: {seed}   particles: {sim_particles}")
 
     exctr = Executor.executor  # Get Executor
 
     args = str(int(sim_particles)) + " " + str(sim_timesteps) + " " + str(seed) + " " + str(kill_rate)
     # task = exctr.submit( app_name='forces', num_procs=cores, app_args=args, stdout='out.txt', stderr='err.txt')
 
     machinefile = None
@@ -113,27 +113,27 @@
             task.kill()  # Timeout
         else:
             time.sleep(poll_interval)
             task.poll()
 
     if task.finished:
         if task.state == "FINISHED":
-            print("Task {} completed".format(task.name))
+            print(f"Task {task.name} completed")
             calc_status = WORKER_DONE
             if read_last_line(filepath) == "kill":
                 # Generally mark as complete if want results (completed after poll - before readline)
                 print("Warning: Task completed although marked as a bad run (kill flag set in forces.stat)")
         elif task.state == "FAILED":
-            print("Warning: Task {} failed: Error code {}".format(task.name, task.errcode))
+            print(f"Warning: Task {task.name} failed: Error code {task.errcode}")
             calc_status = TASK_FAILED
         elif task.state == "USER_KILLED":
-            print("Warning: Task {} has been killed".format(task.name))
+            print(f"Warning: Task {task.name} has been killed")
             calc_status = WORKER_KILL
         else:
-            print("Warning: Task {} in unknown state {}. Error code {}".format(task.name, task.state, task.errcode))
+            print(f"Warning: Task {task.name} in unknown state {task.state}. Error code {task.errcode}")
 
     time.sleep(0.2)
     try:
         data = np.loadtxt(filepath)
         # task.read_file_in_workdir(statfile)
         final_energy = data[-1]
     except Exception:
```

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/forces_support.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/forces_support.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     assert all(
         [line.endswith(status) for line in out if "sim" in line]
     ), "Deliberate error status not logged or raised for all sim instances."
 
 
 def test_ensemble_dir(libE_specs, dir, nworkers, sim_max):
     if not os.path.isdir(dir):
-        print("Specified ensemble directory {} not found.".format(dir))
+        print(f"Specified ensemble directory {dir} not found.")
         return
 
     if not libE_specs.get("sim_dirs_make"):
         print("Typical tests of ensemble directories dont apply without sim_dirs.")
         return
 
     if libE_specs.get("use_worker_dirs"):
@@ -40,32 +40,32 @@
             num_sim_dirs += len(sim_dirs)
 
             for sim_dir in sim_dirs:
                 files_found.append(all([i in os.listdir(os.path.join(dir, worker_dir, sim_dir)) for i in outfiles]))
 
         assert (
             num_sim_dirs == sim_max
-        ), "Number of simulation specific-directories ({}) doesn't match sim_max ({})".format(num_sim_dirs, sim_max)
+        ), f"Number of simulation specific-directories ({num_sim_dirs}) doesn't match sim_max ({sim_max})"
 
         assert all(
             files_found
         ), "Set of expected files ['err.txt', 'forces.stat', 'out.txt'] not found in each sim_dir."
 
     else:
         sim_dirs = os.listdir(dir)
         assert all(
             [i.startswith("sim") for i in sim_dirs]
         ), "All directories within ensemble dir not labeled as (or aren't) sim_dirs."
 
         assert (
             len(sim_dirs) == sim_max
-        ), "Number of simulation specific-directories ({}) doesn't match sim_max ({})".format(len(sim_dirs), sim_max)
+        ), f"Number of simulation specific-directories ({len(sim_dirs)}) doesn't match sim_max ({sim_max})"
 
         files_found = []
         for sim_dir in sim_dirs:
             files_found.append(all([i in os.listdir(os.path.join(dir, sim_dir)) for i in outfiles]))
 
         assert all(
             files_found
         ), "Set of expected files ['err.txt', 'forces.stat', 'out.txt'] not found in each sim_dir."
 
-    print("Output directory {} passed tests.".format(dir))
+    print(f"Output directory {dir} passed tests.")
```

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/readme.md` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces_from_yaml.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces_from_yaml.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 forces = Ensemble()
 forces.from_yaml("forces.yaml")
 
 forces.logger.set_level("INFO")
 
 if forces.is_manager:
-    print("\nRunning with {} workers\n".format(forces.nworkers))
+    print(f"\nRunning with {forces.nworkers} workers\n")
 
 exctr = MPIExecutor()
 exctr.register_app(full_path=sim_app, app_name="forces")
 
 forces.libE_specs["ensemble_dir_path"] = "./ensemble"
 forces.gen_specs["user"].update(
     {
```

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/build_forces.sh` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/build_forces.sh`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 # Building with OpenMP for target device (e.g. GPU)
 # Need to toggle to OpenMP target directive in forces.c.
 
 # xl
 # xlc_r -O3 -qsmp=omp -qoffload -o forces.x forces.c
 
 # Nvidia (nvc) compiler with mpicc and on Cray system with target (Perlmutter)
-# mpicc -O3 -fopenmp -mp=gpu -o forces_gpu.x forces_gpu.c
+# mpicc -O3 -fopenmp -mp=gpu -o forces.x forces.c
 # cc -O3 -fopenmp -mp=gpu -target-accel=nvidia80 -o forces.x forces.c
 
 # Spock/Crusher (AMD ROCm compiler)
 # cc -I${ROCM_PATH}/include -L${ROCM_PATH}/lib -lamdhip64 -fopenmp -O3 -o forces.x forces.c
 
 # Intel oneAPI (Clang based) Compiler (JIT compiled for device)
 # mpiicx -O3 -fiopenmp -fopenmp-targets=spir64 -o forces.x forces.c
```

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/forces.c` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/forces.c`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/build_forces.sh` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/build_forces.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces.c` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces.c`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces_AoS.c` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces_AoS.c`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_app/readme.md` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_app/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_gpu/forces_simf.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_gpu/readme.md` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_gpu/run_libe_forces.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_gpu/run_libe_forces.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from libensemble.executors import MPIExecutor
 
 # Parse number of workers, comms type, etc. from arguments
 nworkers, is_manager, libE_specs, _ = parse_args()
 
 # Initialize MPI Executor instance
 exctr = MPIExecutor()
+# exctr = MPIExecutor(custom_info={'mpi_runner':'srun'})  # force srun - eg. perlmutter
 
 # Register simulation executable with executor
 sim_app = os.path.join(os.getcwd(), "../forces_app/forces.x")
 
 if not os.path.isfile(sim_app):
     sys.exit("forces.x not found - please build first in ../forces_app dir")
```

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_simple/forces_simf.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_simple/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/forces_simple/readme.md` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/forces_simple/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/funcx_forces/forces_simf.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/funcx_forces/forces_simf.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     particle_variance = sim_specs["user"].get("particle_variance", 0)
 
     # Composing variable names and x values to set up simulation
     seed = int(np.rint(x[0][0]))
 
     # This is to give a random variance of work-load
     sim_particles = perturb(sim_particles, seed, particle_variance)
-    print("seed: {}   particles: {}".format(seed, sim_particles))
+    print(f"seed: {seed}   particles: {sim_particles}")
 
     args = str(int(sim_particles)) + " " + str(sim_timesteps) + " " + str(seed) + " " + str(kill_rate)
 
     machinefile = None
     if sim_specs["user"]["fail_on_submit"]:
         machinefile = "fail"
 
@@ -103,27 +103,27 @@
             task.kill()  # Timeout
         else:
             time.sleep(poll_interval)
             task.poll()
 
     if task.finished:
         if task.state == "FINISHED":
-            print("Task {} completed".format(task.name))
+            print(f"Task {task.name} completed")
             calc_status = WORKER_DONE
             if read_last_line(filepath) == "kill":
                 # Generally mark as complete if want results (completed after poll - before readline)
                 print("Warning: Task completed although marked as a bad run (kill flag set in forces.stat)")
         elif task.state == "FAILED":
-            print("Warning: Task {} failed: Error code {}".format(task.name, task.errcode))
+            print(f"Warning: Task {task.name} failed: Error code {task.errcode}")
             calc_status = TASK_FAILED
         elif task.state == "USER_KILLED":
-            print("Warning: Task {} has been killed".format(task.name))
+            print(f"Warning: Task {task.name} has been killed")
             calc_status = WORKER_KILL
         else:
-            print("Warning: Task {} in unknown state {}. Error code {}".format(task.name, task.state, task.errcode))
+            print(f"Warning: Task {task.name} in unknown state {task.state}. Error code {task.errcode}")
 
     time.sleep(0.2)
     try:
         data = np.loadtxt(filepath)
         # task.read_file_in_workdir(statfile)
         final_energy = data[-1]
     except Exception:
```

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/funcx_forces/funcx_forces.yaml` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/funcx_forces/funcx_forces.yaml`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/funcx_forces/readme.md` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/funcx_forces/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/submission_scripts/summit_submit_mproc.sh` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/submission_scripts/summit_submit_mproc.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/submission_scripts/theta_submit_balsam.sh` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/submission_scripts/theta_submit_balsam.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/forces/submission_scripts/theta_submit_mproc.sh` & `libensemble-0.9.3/libensemble/tests/scaling_tests/forces/submission_scripts/theta_submit_mproc.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/all_machine_specs.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/all_machine_specs.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/plot_results.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/plot_results.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/read_sim_output.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/read_sim_output.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/readme.txt` & `libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/readme.txt`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/run_libensemble_on_warpx.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/run_libensemble_on_warpx.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/sim/inputs` & `libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/sim/inputs`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/summit_submit_mproc.sh` & `libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/summit_submit_mproc.sh`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/warpx_simf.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/warpx_simf.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,20 +72,20 @@
             task.kill()  # Timeout
 
     # Set calc_status with optional prints.
     if task.finished:
         if task.state == "FINISHED":
             calc_status = WORKER_DONE
         elif task.state == "FAILED":
-            print("Warning: Task {} failed: Error code {}".format(task.name, task.errcode))
+            print(f"Warning: Task {task.name} failed: Error code {task.errcode}")
             calc_status = TASK_FAILED
         elif task.state == "USER_KILLED":
-            print("Warning: Task {} has been killed".format(task.name))
+            print(f"Warning: Task {task.name} has been killed")
         else:
-            print("Warning: Task {} in unknown state {}. Error code {}".format(task.name, task.state, task.errcode))
+            print(f"Warning: Task {task.name} in unknown state {task.state}. Error code {task.errcode}")
 
     # Safety
     time.sleep(0.2)
 
     try:
         # Get output from a run and delete output files
         warpx_out = read_sim_output(task.workdir)
```

### Comparing `libensemble-0.9.2/libensemble/tests/scaling_tests/warpx/write_sim_input.py` & `libensemble-0.9.3/libensemble/tests/scaling_tests/warpx/write_sim_input.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/standalone_tests/comms_test/commtest.py` & `libensemble-0.9.3/libensemble/tests/standalone_tests/comms_test/commtest.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         ("scal_val", float),
     ]
 }  # Test if get error without this
 
 start_time = time.time()
 
 if rank == 0:
-    print("Running comms test on {} processors with {} workers".format(MPI.COMM_WORLD.Get_size(), num_workers))
+    print(f"Running comms test on {MPI.COMM_WORLD.Get_size()} processors with {num_workers} workers")
     # print("Hello from manager")
     status = MPI.Status()
     alldone = False
     mess_count = 0
     while not alldone:
         for w in worker_ranks:
             if comm.Iprobe(source=w, tag=MPI.ANY_TAG, status=status):
@@ -41,15 +41,15 @@
                 # To test values
                 x = w * 1000.0
                 assert np.all(D_recv["arr_vals"] == x), "Array values do not all match"
                 assert D_recv["scal_val"] == x + x / 1e7, "Scalar values do not all match"
         if mess_count >= total_num_mess:
             alldone = True
 
-    print("Manager received and checked {} messages".format(mess_count))
+    print(f"Manager received and checked {mess_count} messages")
     print("Manager finished in time", time.time() - start_time)
 
 else:
     # print("Hello from worker", rank)
     output = np.zeros(1, dtype=sim_specs["out"])
     for x in range(rounds):
         x = rank * 1000.0
```

### Comparing `libensemble-0.9.2/libensemble/tests/standalone_tests/comms_test/readme.txt` & `libensemble-0.9.3/libensemble/tests/standalone_tests/comms_test/readme.txt`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/burn_time.c` & `libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/burn_time.c`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/killtest.py` & `libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/killtest.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # sys.argv[0] is python exe.
 kill_type = int(sys.argv[1])  # 1, 2
 num_nodes = int(sys.argv[2])
 num_procs_per_node = int(sys.argv[3])
 num_procs = num_nodes * num_procs_per_node
 
 print("Running Kill test with program", user_code)
-print("Kill type: {}   num_nodes: {}   procs_per_node: {}".format(kill_type, num_nodes, num_procs_per_node))
+print(f"Kill type: {kill_type}   num_nodes: {num_nodes}   procs_per_node: {num_procs_per_node}")
 
 
 # Create common components of submit line (currently all of it)
 
 # Am I in an aprun environment
 launcher = "mpich"  # Includes mpich based - eg. intelmpi
 try:
@@ -68,15 +68,15 @@
 total_start_time = time.time()
 
 for run_num in range(2):
     time.sleep(4)  # Show gap where none should be running
     stdout = "out_" + str(run_num) + ".txt"
     # runline = ['mpirun', '-np', str(num_procs), user_code]
     print("---------------------------------------------------------------")
-    print("\nRun num: {}   Runline: {}\n".format(run_num, " ".join(runline)))
+    print(f"\nRun num: {run_num}   Runline: {' '.join(runline)}\n")
 
     if kill_type == 1:
         process = subprocess.Popen(runline, cwd="./", stdout=open(stdout, "w"), shell=False)  # with kill 1
     elif kill_type == 2:
         process = subprocess.Popen(
             runline, cwd="./", stdout=open(stdout, "w"), shell=False, preexec_fn=os.setsid
         )  # kill 2
@@ -122,27 +122,27 @@
     num_rechecks = 2  # Number of times to check for new output
 
     time.sleep(grace_period)  # Give chance to kill
 
     # Test if task is still producing output
     with open(stdout, "rb") as fh:
         line_on_kill = fh.readlines()[-1].decode().rstrip()
-    print("Last line after task kill:  {}".format(line_on_kill))
+    print(f"Last line after task kill:  {line_on_kill}")
 
     if "has finished" in line_on_kill:
         raise Exception("Task may have already finished - test invalid")
 
     for recheck in range(1, num_rechecks + 1):
         time.sleep(recheck_period)
         with open(stdout, "rb") as fh:
             lastline = fh.readlines()[-1].decode().rstrip()
-        print("Last line after {} seconds: {}".format(recheck_period * recheck, lastline))
+        print(f"Last line after {recheck_period * recheck} seconds: {lastline}")
 
         if lastline != line_on_kill:
-            print("Task {} still producing output".format(run_num))
+            print(f"Task {run_num} still producing output")
             # print("Last line check 1:", line_on_kill)
             # print("Last line check 2:", lastline)
             assert 0
 
 total_end_time = time.time()
 total_time = total_end_time - total_start_time
-print("\nTask kill test completed in {} seconds\n".format(total_time))
+print(f"\nTask kill test completed in {total_time} seconds\n")
```

### Comparing `libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/log.autotest.txt` & `libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/log.autotest.txt`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/log.burn_time_test_with_top.txt` & `libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/log.burn_time_test_with_top.txt`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/readme.txt` & `libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/readme.txt`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/standalone_tests/kill_test/sleep_and_print.c` & `libensemble-0.9.3/libensemble/tests/standalone_tests/kill_test/sleep_and_print.c`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/standalone_tests/mpi_launch_test/create_mpi_jobs.py` & `libensemble-0.9.3/libensemble/tests/standalone_tests/mpi_launch_test/create_mpi_jobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 rank = MPI.COMM_WORLD.Get_rank()
 runline = "mpirun -np ".split()
 runline.append(task_nprocs)
 runline.append("python")
 runline.append("helloworld.py")
 
 if rank == 0:
-    print("Total sub-task procs: {}".format(size * int(task_nprocs)))
-    print("Total procs (parent + sub-tasks): {}".format(size * (int(task_nprocs) + 1)))
+    print(f"Total sub-task procs: {size * int(task_nprocs)}")
+    print(f"Total procs (parent + sub-tasks): {size * (int(task_nprocs) + 1)}")
 
 # print("Rank {}: {}".format(rank, " ".join(runline)))
 output = "task_" + str(rank) + ".out"
 p = subprocess.Popen(runline, stdout=open(output, "w"), shell=False)
 p.wait()
```

### Comparing `libensemble-0.9.2/libensemble/tests/standalone_tests/mpi_launch_test/readme.txt` & `libensemble-0.9.3/libensemble/tests/standalone_tests/mpi_launch_test/readme.txt`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/conftest.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/mpich-only_test_api.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/mpich-only_test_api.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/setup.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/setup.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/simdir/borehole.c` & `libensemble-0.9.3/libensemble/tests/unit_tests/simdir/borehole.c`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/simdir/my_serialtask.c` & `libensemble-0.9.3/libensemble/tests/unit_tests/simdir/my_serialtask.c`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/simdir/my_simtask.c` & `libensemble-0.9.3/libensemble/tests/unit_tests/simdir/my_simtask.c`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/simdir/my_simtask.f90` & `libensemble-0.9.3/libensemble/tests/unit_tests/simdir/my_simtask.f90`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/simdir/test_example.yaml` & `libensemble-0.9.3/libensemble/tests/unit_tests/simdir/test_example.yaml`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/simdir/test_example_badfuncs_attribute.yaml` & `libensemble-0.9.3/libensemble/tests/unit_tests/simdir/test_example_badfuncs_attribute.yaml`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/simdir/test_example_badfuncs_notfound.yaml` & `libensemble-0.9.3/libensemble/tests/unit_tests/simdir/test_example_badfuncs_notfound.yaml`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_allocation_funcs_and_support.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_allocation_funcs_and_support.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_comms.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_comms.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_env_resources.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_env_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 
 def teardown_standalone_run():
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = ""
 
 
 def setup_function(function):
-    print("setup_function    function:%s" % function.__name__)
+    print(f"setup_function    function:{function.__name__}")
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = ""
 
 
 def teardown_function(function):
-    print("teardown_function    function:%s" % function.__name__)
+    print(f"teardown_function    function:{function.__name__}")
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = ""
 
 
 # Tests ========================================================================================
 
 # Tests for obtaining nodelist from environment variables
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_executor.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 # Test does not require running full libensemble
 import os
 import re
 import sys
 import time
 import pytest
 import socket
-import mpi4py
+import platform
 
-mpi4py.rc.initialize = False
-from mpi4py import MPI
+if platform.system() != "Windows":
+    import mpi4py
+
+    mpi4py.rc.initialize = False
+    from mpi4py import MPI
 
 from libensemble.resources.mpi_resources import MPIResourcesException
 from libensemble.executors.executor import Executor, ExecutorException, TimeoutExpired
 from libensemble.executors.executor import NOT_STARTED_STATES
 
 
 USE_BALSAM = False
@@ -26,35 +29,35 @@
 c_startup = "simdir/c_startup.x"
 py_startup = "simdir/py_startup.py"
 non_existent_app = "simdir/non_exist.x"
 
 
 def setup_module(module):
     try:
-        print("setup_module module:%s" % module.__name__)
+        print(f"setup_module module:{module.__name__}")
     except AttributeError:
-        print("setup_module (direct run) module:%s" % module)
+        print(f"setup_module (direct run) module:{module}")
     if Executor.executor is not None:
         del Executor.executor
         Executor.executor = None
     build_simfuncs()
 
 
 def setup_function(function):
-    print("setup_function function:%s" % function.__name__)
+    print(f"setup_function function:{function.__name__}")
     if Executor.executor is not None:
         del Executor.executor
         Executor.executor = None
 
 
 def teardown_module(module):
     try:
-        print("teardown_module module:%s" % module.__name__)
+        print(f"teardown_module module:{module.__name__}")
     except AttributeError:
-        print("teardown_module (direct run) module:%s" % module)
+        print(f"teardown_module (direct run) module:{module}")
     if Executor.executor is not None:
         del Executor.executor
         Executor.executor = None
 
 
 def build_simfuncs():
     import subprocess
@@ -198,47 +201,52 @@
                         exctr.kill(task)
                         time.sleep(delay)  # Give time for kill
                         continue
     return task_list
 
 
 # Tests ========================================================================================
+
+
+@pytest.mark.extra
 def test_launch_and_poll():
     """Test of launching and polling task and exiting on task finish"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 0.2"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     task = polling_loop(exctr, task)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
     assert task.run_attempts == 1, "task.run_attempts should be 1. Returned " + str(task.run_attempts)
 
 
+@pytest.mark.extra
 def test_launch_and_wait():
     """Test of launching and waiting on task"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 1"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     task.wait()
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
     task.wait()  # Already complete
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 def test_launch_and_wait_timeout():
     """Test of launching and waiting on task timeout (and kill)"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 5"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     try:
         task.wait(timeout=0.5)
@@ -247,69 +255,74 @@
         print(TimeoutExpired)
         assert not task.finished, "task.finished should be False. Returned " + str(task.finished)
         task.kill()
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "USER_KILLED", "task.state should be USER_KILLED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 def test_launch_wait_on_start():
     """Test of launching task with wait_on_start"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 0.2"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim, wait_on_start=True)
     assert task.state not in NOT_STARTED_STATES, "Task should not be in a NOT_STARTED state. State: " + str(task.state)
     exctr.poll(task)
     if not task.finished:
         task = polling_loop(exctr, task)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 def test_kill_on_file():
     """Test of killing task based on something in output file"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 0.1 Error"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     task = polling_loop(exctr, task)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "USER_KILLED", "task.state should be USER_KILLED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 def test_kill_on_timeout():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 10"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     task = polling_loop(exctr, task)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "USER_KILLED", "task.state should be USER_KILLED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 def test_kill_on_timeout_polling_loop_method():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 10"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     exctr.polling_loop(task, timeout=1)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "USER_KILLED", "task.state should be USER_KILLED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 def test_launch_and_poll_multitasks():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     task_list = []
     cores = NCORES
 
     for j in range(3):
         # outfilename = 'out_' + str(j) + '.txt' # Could allow launch to generate outfile names based on task.id
@@ -322,43 +335,45 @@
 
     task_list_return = polling_loop_multitask(exctr, task_list)
     for task in task_list_return:
         assert task.finished, "task.finished should be True. Returned " + str(task.finished)
         assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 def test_get_task():
     """Return task from given task id"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
 
     # Try with no tasks set up
     A = exctr.get_task("a")
     assert A is None, "Task found when tasklist should be empty"
 
     # Set up task and getid
     cores = NCORES
     args_for_sim = "sleep 0"
     task0 = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     taskid = task0.id
-    print("taskid is: {}".format(taskid))
+    print(f"taskid is: {taskid}")
     A = exctr.get_task(taskid)
     assert A is task0, "Task get_task returned unexpected task" + str(A)
     task0 = polling_loop(exctr, task0)
 
     # Get non-existent taskid
     A = exctr.get_task(taskid + 1)
     assert A is None, "Task found when supplied taskid should not exist"
 
 
+@pytest.mark.extra
 @pytest.mark.timeout(30)
 def test_procs_and_machinefile_logic():
     """Test of supplying various input configurations."""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
 
     # Note: Could test task_partition routine directly - without launching tasks...
 
     # Testing machinefile
     setup_executor()
     exctr = Executor.executor
     args_for_sim = "sleep 0"
@@ -433,21 +448,22 @@
     task = exctr.submit(calc_type="sim", num_nodes=1, num_procs=2, app_args=args_for_sim)
     assert 1
     task = polling_loop(exctr, task, delay=0.05)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 @pytest.mark.timeout(20)
 def test_doublekill():
     """Test attempt to kill already killed task
 
     Kill should have no effect (except warning message) and should remain in state killed
     """
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 2.0"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     task.poll()
     exctr.wait_time = 5
@@ -456,21 +472,22 @@
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "USER_KILLED", "task.state should be USER_KILLED. Returned " + str(task.state)
     exctr.kill(task)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "USER_KILLED", "task.state should be USER_KILLED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 @pytest.mark.timeout(20)
 def test_finish_and_kill():
     """Test attempt to kill already finished task
 
     Kill should have no effect (except warning message) and should remain in state FINISHED
     """
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 0.1"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     while not task.finished:
         time.sleep(0.1)
@@ -482,18 +499,19 @@
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
     # Try polling after finish - should return with no effect
     task.poll()
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 @pytest.mark.timeout(20)
 def test_launch_and_kill():
     """Test launching and immediately killing tasks with no poll"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 2.0"
     task_list = []
     exctr.wait_time = 1
     for taskid in range(5):
@@ -502,16 +520,17 @@
         task_list.append(task)
 
     for task in task_list:
         assert task.finished, "task.finished should be True. Returned " + str(task.finished)
         assert task.state == "USER_KILLED", "task.state should be USER_KILLED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 def test_launch_as_gen():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 0.1"
 
     # Try launching as gen when not registered as gen
     try:
@@ -532,16 +551,17 @@
         task = exctr.submit(calc_type="alloc", num_procs=cores, app_args=args_for_sim)
     except ExecutorException as e:
         assert e.args[0] + e.args[1] == "Unrecognized calculation type" + "alloc"
     else:
         assert 0
 
 
+@pytest.mark.extra
 def test_launch_no_app():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor_noapp()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 0.1"
     try:
         _ = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     except ExecutorException as e:
@@ -552,18 +572,19 @@
         _ = exctr.submit(num_procs=cores, app_args=args_for_sim)
     except ExecutorException as e:
         assert e.args[0] == "Either app_name or calc_type must be set"
     else:
         assert 0
 
 
+@pytest.mark.extra
 def test_kill_task_with_no_submit():
     from libensemble.executors.executor import Task
 
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
 
     # Try kill invalid task
     try:
         exctr.kill("mytask")
     except ExecutorException as e:
@@ -582,18 +603,19 @@
         exctr.kill(task1)
     except ExecutorException as e:
         assert bool(re.match(exp_re, e.args[0]))
     else:
         assert 0
 
 
+@pytest.mark.extra
 def test_poll_task_with_no_submit():
     from libensemble.executors.executor import Task
 
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
 
     # Create a task directly with no submit (Not supported for users)
     exp_msg = "Polled task libe_task_my_simtask.x_.+ " "has no process ID - check tasks been launched"
     exp_re = re.compile(exp_msg)
     myapp = exctr.sim_default_app
@@ -602,54 +624,58 @@
         task1.poll()
     except ExecutorException as e:
         assert bool(re.match(exp_re, e.args[0]))
     else:
         assert 0
 
 
+@pytest.mark.extra
 def test_task_failure():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 1.0 Fail"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     task = polling_loop(exctr, task, timeout_sec=3)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FAILED", "task.state should be FAILED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 def test_retries_launch_fail():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor_fakerunner()
     exctr = Executor.executor
     exctr.retry_delay_incr = 0.05
     cores = NCORES
     args_for_sim = "sleep 0"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     assert task.state == "CREATED", "task.state should be CREATED. Returned " + str(task.state)
     assert exctr.mpi_runner.subgroup_launch, "subgroup_launch should be True"
     assert task.run_attempts == 5, "task.run_attempts should be 5. Returned " + str(task.run_attempts)
 
 
+@pytest.mark.extra
 def test_retries_run_fail():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     exctr.retry_delay_incr = 0.05
     exctr.fail_time = 3
     cores = NCORES
     args_for_sim = "sleep 0 Fail"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim, wait_on_start=True)
     assert task.state == "FAILED", "task.state should be FAILED. Returned " + str(task.state)
     assert task.run_attempts == 5, "task.run_attempts should be 5. Returned " + str(task.run_attempts)
 
 
+@pytest.mark.extra
 def test_register_apps():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()  # This registers an app my_simtask.x (default sim)
     exctr = Executor.executor
     exctr.register_app(full_path="/path/to/fake_app1.x", app_name="fake_app1")
     exctr.register_app(full_path="/path/to/fake_app2.py", app_name="fake_app2")
     exctr.register_app(full_path="/path/to/fake_app3.pl", app_name="fake_app3", precedent="perl")
 
     # Check selected attributes
@@ -685,24 +711,26 @@
         app = exctr.get_app("fake_app4")
     except ExecutorException as e:
         assert e.args[0] == "Application fake_app4 not found in registry"
         # Ordering of dictionary may vary
         # assert e.args[1] == "Registered applications: ['my_simtask.x', 'fake_app1', 'fake_app2']"
 
 
+@pytest.mark.extra
 def test_serial_exes():
     setup_serial_executor()
     exctr = Executor.executor
     args_for_sim = "sleep 0.1"
     task = exctr.submit(calc_type="sim", app_args=args_for_sim, wait_on_start=True)
     task.wait()
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
 
 
+@pytest.mark.extra
 def test_serial_startup_times():
     setup_executor_startups()
     exctr = Executor.executor
 
     t1 = time.time()
     task = exctr.submit(app_name="c_startup")
     task.wait()
@@ -720,54 +748,57 @@
     startup_time = stime - t1
     print("start up time for python program", startup_time)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
     assert 0 < startup_time < 1, "Start up time for python program took " + str(startup_time)
 
 
+@pytest.mark.extra
 def test_futures_interface():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     cores = NCORES
     args_for_sim = "sleep 3"
     with Executor.executor as exctr:
         task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim, wait_on_start=True)
     time.sleep(0.1)
     assert task.running(), "task.running() should return True after wait_on_start task submission."
     assert task.result() == "FINISHED", "task.result() should return FINISHED. Returned " + str(task.state)
     assert task.done(), "task.done() should return True after task finishes."
 
 
+@pytest.mark.extra
 def test_futures_interface_cancel():
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     cores = NCORES
     args_for_sim = "sleep 3"
     with Executor.executor as exctr:
         task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim, wait_on_start=True)
     time.sleep(0.1)
     task.cancel()
     assert task.cancelled() and task.done(), "Task should be both cancelled() and done() after cancellation."
 
 
+@pytest.mark.extra
 def test_dry_run():
     """Test of dry_run in poll"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 0.2"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim, dry_run=True)
     task.poll()
     task.kill()
 
 
+@pytest.mark.extra
 def test_non_existent_app():
     """Tests exception on non-existent app"""
-
     from libensemble.executors.executor import Executor
 
     exctr = Executor()
 
     # Can register a non-existent app in case created as part of workflow.
     exctr.register_app(full_path=non_existent_app, app_name="nonexist")
 
@@ -777,17 +808,17 @@
         w_exctr.submit(app_name="nonexist")
     except ExecutorException as e:
         assert e.args[0] == "Application does not exist simdir/non_exist.x"
     else:
         assert 0
 
 
+@pytest.mark.extra
 def test_non_existent_app_mpi():
     """Tests exception on non-existent app"""
-
     from libensemble.executors.mpi_executor import MPIExecutor
 
     exctr = MPIExecutor()
 
     # Can register a non-existent app in case created as part of workflow.
     exctr.register_app(full_path=non_existent_app, app_name="nonexist")
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_history.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_history.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_launcher.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 
 """
 Unit test of launcher helpers for libensemble.
 """
 
 import sys
+import pytest
 import libensemble.utils.launcher as launcher
 
 
 def test_form_command():
     "Test the command templating."
 
     run_specs = {"mpirun": "mpirun", "nproc": 10, "nrank": 5, "mf": None}
@@ -55,19 +56,21 @@
 
     # Try simple kill
     process = launcher.launch([py_exe, "launch_busy.py", "1"])
     assert not launcher.process_is_stopped(process, 0.5), "Process stopped early."
     launcher.cancel(process, 0)
 
 
+@pytest.mark.extra
 def test_launch32():
     "If we are in Python > 3.2, still check that 3.2 wait func works"
     saved_wait = launcher.wait
     launcher.wait = launcher.wait_py32
     xtest_submit()
     launcher.wait = saved_wait
 
 
+@pytest.mark.extra
 def test_launch33():
     "If we are in Python > 3.2, also check the new-style wait func"
     if launcher.wait == launcher.wait_py33:
         xtest_submit()
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_libE_main.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_libE_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 alloc_specs = {"alloc_f": give_sim_work_first, "out": []}
 hfile_abort = "libE_history_at_abort_0.npy"
 pfile_abort = "libE_persis_info_at_abort_0.pickle"
 
 
 # Run by pytest before each function
 def setup_function(function):
-    print("setup_function function:%s" % function.__name__)
+    print(f"setup_function function:{function.__name__}")
     if Resources.resources is not None:
         del Resources.resources
         Resources.resources = None
 
 
 def remove_file_if_exists(filename):
     try:
@@ -249,14 +249,15 @@
 
     libE_specs["use_worker_dirs"] = True
     libE_specs["sim_input_dir"] = "./__init__.py"
     libE_specs["sim_dir_copy_files"] = ["./__init__.py"]
     check_inputs(libE_specs=libE_specs)
 
 
+@pytest.mark.extra
 def test_logging_disabling():
     remove_file_if_exists("ensemble.log")
     remove_file_if_exists("libE_stats.txt")
     sim_specs, gen_specs, exit_criteria = setup.make_criteria_and_specs_0()
     libE_specs = {"mpi_comm": fake_mpi, "comms": "mpi", "disable_log_files": True}
     logconfig = LogConfig.config
     logconfig.logger_set = False
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_loc_stack.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_loc_stack.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from libensemble.utils.loc_stack import LocationStack
 
 
 def test_location_stack():
     "Test correctness of location stack (all in a temp dir)."
 
     tmp_dirname = tempfile.mkdtemp()
-    assert os.path.isdir(tmp_dirname), "Failed to create temporary directory {}.".format(tmp_dirname)
+    assert os.path.isdir(tmp_dirname), f"Failed to create temporary directory {tmp_dirname}."
 
     try:
         # Record where we started
         start_dir = os.getcwd()
 
         # Set up directory for clone
         clone_dirname = os.path.join(tmp_dirname, "basedir")
@@ -28,18 +28,18 @@
         with open(test_fname, "w+") as f:
             f.write("This is a test file\n")
 
         s = LocationStack()
 
         # Register a valid location
         tname = s.register_loc(0, "testdir", prefix=tmp_dirname, copy_files=[test_fname])
-        assert os.path.isdir(tname), "New directory {} was not created.".format(tname)
+        assert os.path.isdir(tname), f"New directory {tname} was not created."
         assert os.path.isfile(
             os.path.join(tname, "test.txt")
-        ), "New directory {} failed to copy test.txt from {}.".format(tname, clone_dirname)
+        ), f"New directory {tname} failed to copy test.txt from {clone_dirname}."
 
         # Register an empty location
         d = s.register_loc(1, None)
         assert d is None, "Dir stack not correctly register None at location 1."
 
         # Register a dummy location (del should not work)
         d = s.register_loc(2, os.path.join(tmp_dirname, "dummy"))
@@ -57,52 +57,52 @@
         # Push registered location (we should move
         s.push_loc(0)
         assert s.stack == [None, start_dir], "Directory stack is incorrect." "Wanted [None, {}], got {}.".format(
             start_dir, s.stack
         )
         assert os.path.samefile(
             os.getcwd(), tname
-        ), "Directory stack push_loc failed to end up at desired dir." "Wanted {}, at {}".format(tname, os.getcwd())
+        ), f"Directory stack push_loc failed to end up at desired dir.Wanted {tname}, at {os.getcwd()}"
 
         # Pop the registered location
         s.pop()
-        assert s.stack == [None], "Directory stack is incorrect after pop." "Wanted [None], got {}.".format(s.stack)
+        assert s.stack == [None], f"Directory stack is incorrect after pop.Wanted [None], got {s.stack}."
         assert os.path.samefile(
             os.getcwd(), start_dir
         ), "Directory stack push_loc failed to stay put with input None." "Wanted {}, at {}".format(
             start_dir, os.getcwd()
         )
 
         # Context for moving again
         with s.loc(0):
             assert s.stack == [None, start_dir], "Directory stack is incorrect." "Wanted [None, {}], got {}.".format(
                 start_dir, s.stack
             )
             assert os.path.samefile(
                 os.getcwd(), tname
-            ), "Directory stack push_loc failed to end up at desired dir." "Wanted {}, at {}".format(tname, os.getcwd())
+            ), f"Directory stack push_loc failed to end up at desired dir.Wanted {tname}, at {os.getcwd()}"
 
         # Check directory after context
-        assert s.stack == [None], "Directory stack is incorrect after ctx." "Wanted [None], got {}.".format(s.stack)
+        assert s.stack == [None], f"Directory stack is incorrect after ctx.Wanted [None], got {s.stack}."
         assert os.path.samefile(os.getcwd(), start_dir), "Directory looks wrong after ctx." "Wanted {}, at {}".format(
             start_dir, os.getcwd()
         )
 
         with s.dir(None):
             assert s.stack == [None, None], "Directory stack is incorrect in ctx."
         assert s.stack == [None], "Directory stack is incorrect after ctx."
 
         # Pop the unregistered location
         s.pop()
-        assert not s.stack, "Directory stack should be empty, actually {}.".format(s.stack)
+        assert not s.stack, f"Directory stack should be empty, actually {s.stack}."
         assert os.path.samefile(
             os.getcwd(), start_dir
         ), "Directory stack push_loc failed to stay put with input None." "Wanted {}, at {}".format(
             start_dir, os.getcwd()
         )
 
         # Clean up
         s.clean_locs()
-        assert not os.path.isdir(tname), "Directory {} should have been removed on cleanup.".format(tname)
+        assert not os.path.isdir(tname), f"Directory {tname} should have been removed on cleanup."
 
     finally:
         shutil.rmtree(tmp_dirname)
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_manager_main.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_manager_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import time
+import pytest
+import platform
 import numpy as np
 import numpy.lib.recfunctions
-from mpi4py import MPI
 
 import libensemble.manager as man
 import libensemble.tests.unit_tests.setup as setup
 
-libE_specs = {"mpi_comm": MPI.COMM_WORLD}
+if platform.system() != "Windows":
+    from mpi4py import MPI
 
+    libE_specs = {"mpi_comm": MPI.COMM_WORLD}
 
+
+@pytest.mark.extra
 def test_term_test_1():
     # termination_test should be True when we want to stop
 
     # sh - Should separate the tests
     # Test 1
     hist, sim_specs, gen_specs, exit_criteria, al = setup.hist_setup1()
     mgr = man.Manager(hist, libE_specs, al, sim_specs, gen_specs, exit_criteria)
     assert not mgr.term_test()
 
 
+@pytest.mark.extra
 def test_term_test_2():
     # Test 2 - these could also be sep - with a setup or fixture....
     # Shouldn't terminate
     hist, sim_specs, gen_specs, exit_criteria, al = setup.hist_setup2()
     mgr = man.Manager(hist, libE_specs, al, sim_specs, gen_specs, exit_criteria)
     assert not mgr.term_test()
     #
@@ -35,14 +41,15 @@
     #
     # Terminate because everything has been given.
     hist.H["sim_started"] = np.ones
     hist.sim_started_count = len(hist.H)
     assert mgr.term_test()
 
 
+@pytest.mark.extra
 def test_term_test_3():
     # Test 3.
     # Terminate because enough time has passed
     H0 = np.zeros(3, dtype=[("g", float)] + [("x", float), ("priority", float)])
     hist, sim_specs, gen_specs, exit_criteria, al = setup.hist_setup2(H0_in=H0)
     mgr = man.Manager(hist, libE_specs, al, sim_specs, gen_specs, exit_criteria)
     hist.index = 4
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_node_resources.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_node_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 
 def teardown_standalone_run():
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = ""
 
 
 def setup_function(function):
-    print("setup_function    function:%s" % function.__name__)
+    print(f"setup_function    function:{function.__name__}")
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = ""
 
 
 def teardown_function(function):
-    print("teardown_function    function:%s" % function.__name__)
+    print(f"teardown_function    function:{function.__name__}")
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = ""
 
 
 # Tests ========================================================================================
 
 
 def test_get_cpu_resources_from_env_empty():
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_persistent_aposmm.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_persistent_aposmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import pytest
+import platform
 import multiprocessing
 
-multiprocessing.set_start_method("fork", force=True)
-
 import libensemble.gen_funcs
 
 libensemble.gen_funcs.rc.aposmm_optimizers = "nlopt"
-from libensemble.gen_funcs.persistent_aposmm import aposmm, update_history_optimal
+
+if platform.system() in ["Linux", "Darwin"]:
+    multiprocessing.set_start_method("fork", force=True)
+    from libensemble.gen_funcs.persistent_aposmm import aposmm, update_history_optimal
 
 import numpy as np
 import libensemble.tests.unit_tests.setup as setup
 from libensemble.sim_funcs.six_hump_camel import six_hump_camel_func, six_hump_camel_grad
 
 libE_info = {"comm": {}}
 
@@ -107,15 +109,15 @@
     min_found = 0
     for m in minima:
         # The minima are known on this test problem.
         # We use their values to test APOSMM has identified all minima
         print(np.min(np.sum((H[H["local_min"]]["x"] - m) ** 2, 1)), flush=True)
         if np.min(np.sum((H[H["local_min"]]["x"] - m) ** 2, 1)) < tol:
             min_found += 1
-    assert min_found >= 6, "Found {} minima".format(min_found)
+    assert min_found >= 6, f"Found {min_found} minima"
 
 
 @pytest.mark.extra
 def test_standalone_persistent_aposmm_combined_func():
     from libensemble.tests.regression_tests.support import six_hump_camel_minima as minima
     from math import gamma, pi, sqrt
     from libensemble.message_numbers import FINISHED_PERSISTENT_GEN_TAG
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_resource_scheduler.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_resource_scheduler.py`

 * *Files 17% similar despite different names*

```diff
@@ -50,55 +50,55 @@
         self.rsets["assigned"] = assignment
         self.rsets_free = np.count_nonzero(self.rsets["assigned"] == 0)
 
 
 def _fail_to_resource(sched, rsets):
     with pytest.raises(InsufficientFreeResources):
         rset_team = sched.assign_resources(rsets_req=rsets)
-        pytest.fail("Expected InsufficientFreeResources. Found {}".format(rset_team))
+        pytest.fail(f"Expected InsufficientFreeResources. Found {rset_team}")
 
 
 def _print_assigned(resources):
     """For debugging. Print assigned rsets by group"""
     rsets = resources.rsets
     max_groups = max(rsets["group"])
     print("\nAssigned")
     for g in range(max_groups + 1):
         filt = rsets["group"] == g
         print(rsets["assigned"][filt])
-    print("free rsets {}\n".format(resources.free_rsets))
+    print(f"free rsets {resources.free_rsets}\n")
 
 
 def test_request_zero_rsets():
     """Tests requesting zero resource sets"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
 
     # No options
     sched = ResourceScheduler(user_resources=resources)
     rset_team = sched.assign_resources(rsets_req=0)
-    assert rset_team == [], "rset_team is {}. Expected zero".format(rset_team)
+    assert rset_team == [], f"rset_team is {rset_team}. Expected zero"
     del sched
     rset_team = None
 
     # Options should make no difference
     for match_slots in [False, True]:
         for split2fit in [False, True]:
             sched_options = {"match_slots": match_slots, "split2fit": split2fit}
             sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
             rset_team = sched.assign_resources(rsets_req=0)
-            assert rset_team == [], "rset_team is {}. Expected zero".format(rset_team)
+            assert rset_team == [], f"rset_team is {rset_team}. Expected zero"
             del sched
             rset_team = None
     del resources
 
 
 def test_too_many_rsets():
     """Tests request of more resource sets than exist"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
 
     # No options
     sched = ResourceScheduler(user_resources=resources)
 
     with pytest.raises(InsufficientResourcesError):
         rset_team = sched.assign_resources(rsets_req=10)  # noqa F841
@@ -117,38 +117,38 @@
                 pytest.fail("Expected InsufficientResourcesError")
             del sched
     del resources
 
 
 def test_cannot_split_quick_return():
     """Tests the quick return when splitting finds no free even gaps"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(6, 3)
     resources.fixed_assignment(([1, 0, 0, 0, 3, 3]))
     sched = ResourceScheduler(user_resources=resources)
     _fail_to_resource(sched, 3)
 
 
 def test_schedule_find_gaps_1node():
     """Tests assignment of rsets on one node.
 
     This test also checks the list is correctly assigned to workers
     and the freeing of assigned resources.
     """
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 1)
 
     # Options should make no difference
     for match_slots in [False, True]:
         for split2fit in [False, True]:
             sched_options = {"match_slots": match_slots, "split2fit": split2fit}
             sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
 
             rset_team = sched.assign_resources(rsets_req=2)
-            assert rset_team == [0, 1], "rset_team is {}".format(rset_team)
+            assert rset_team == [0, 1], f"rset_team is {rset_team}"
 
             rset_team = sched.assign_resources(rsets_req=3)
             assert rset_team == [2, 3, 4]
 
             # Check not enough slots
             _fail_to_resource(sched, 4)
 
@@ -170,77 +170,77 @@
             rset_team = None
             resources.free_rsets()
     del resources
 
 
 def test_schedule_find_gaps_2nodes():
     """Tests finding gaps on two nodes with equal resource sets"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
     inputs = [2, 3, 1, 2]
     exp_out = [[0, 1], [4, 5, 6], [7], [2, 3]]
 
     for match_slots in [False, True]:
         for split2fit in [False, True]:
             sched_options = {"match_slots": match_slots, "split2fit": split2fit}
             sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
             for i in range(4):
                 rset_team = sched.assign_resources(rsets_req=inputs[i])
-                assert rset_team == exp_out[i], "Expected {}, Received rset_team {}".format(exp_out[i], rset_team)
+                assert rset_team == exp_out[i], f"Expected {exp_out[i]}, Received rset_team {rset_team}"
             _fail_to_resource(sched, 1)
             del sched
             rset_team = None
     del resources
 
 
 def test_split_across_no_matching_slots():
     """Must split across - but no split2fit and no matching slots"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(6, 3)  # 3 nodes of 2 slots
 
     for split2fit in [False, True]:
         resources.fixed_assignment(([0, 1, 1, 0, 0, 1]))
         sched_options = {"split2fit": split2fit}
         sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
         _fail_to_resource(sched, 3)
 
         sched.match_slots = False
         rset_team = sched.assign_resources(rsets_req=3)
-        assert rset_team == [0, 3, 4], "rset_team is {}.".format(rset_team)
+        assert rset_team == [0, 3, 4], f"rset_team is {rset_team}."
         del sched
         rset_team = None
     del resources
 
 
 def test_across_nodes_even_split():
     """Tests even assignment over two and three nodes
 
     Also tests cached variables in scheduler.
     """
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
 
     # Options should make no difference
     for match_slots in [False, True]:
         for split2fit in [False, True]:
             resources = MyResources(8, 2)
             sched_options = {"match_slots": match_slots, "split2fit": split2fit}
             sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
 
             rset_team = sched.assign_resources(rsets_req=6)
             # Expecting even split
-            assert rset_team == [0, 1, 2, 4, 5, 6], "Even split test did not get expected result {}".format(rset_team)
-            assert sched.rsets_free == 2, "rsets_free should be 2. Found {}".format(sched.rsets_free)
+            assert rset_team == [0, 1, 2, 4, 5, 6], f"Even split test did not get expected result {rset_team}"
+            assert sched.rsets_free == 2, f"rsets_free should be 2. Found {sched.rsets_free}"
             assert sched.avail_rsets_by_group == {0: [3], 1: [7]}
 
             # Now find the remaining 2 slots
             if not sched_options["split2fit"]:
                 _fail_to_resource(sched, 2)
             else:
                 rset_team = sched.assign_resources(rsets_req=2)
-                assert rset_team == [3, 7], "rsets found {}".format(rset_team)
+                assert rset_team == [3, 7], f"rsets found {rset_team}"
                 assert sched.rsets_free == 0
                 assert sched.avail_rsets_by_group == {0: [], 1: []}
             del sched
             rset_team = None
 
             # This time it must use 3 nodes for even split (though 2 would cover uneven).
             resources = MyResources(15, 3)
@@ -251,64 +251,64 @@
             assert rset_team == [0, 1, 2, 5, 6, 7, 10, 11, 12], "Even split test did not get expected result {}".format(
                 rset_team
             )
             if not sched_options["split2fit"]:
                 _fail_to_resource(sched, 6)
             else:
                 rset_team = sched.assign_resources(rsets_req=6)
-                assert rset_team == [3, 4, 8, 9, 13, 14], "rsets found {}".format(rset_team)
+                assert rset_team == [3, 4, 8, 9, 13, 14], f"rsets found {rset_team}"
 
             del sched
             rset_team = None
     del resources
 
 
 def test_across_nodes_roundup_option_2nodes():
     """Tests assignment over two nodes"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
 
     # Options should make no difference
     for match_slots in [False, True]:
         for split2fit in [False, True]:
             sched_options = {"match_slots": match_slots, "split2fit": split2fit}
             sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
             rset_team = sched.assign_resources(rsets_req=5)
             # Expecting even split
-            assert rset_team == [0, 1, 2, 4, 5, 6], "Even split test did not get expected result {}".format(rset_team)
-            assert sched.rsets_free == 2, "Free slots found {}".format(sched.rsets_free)
+            assert rset_team == [0, 1, 2, 4, 5, 6], f"Even split test did not get expected result {rset_team}"
+            assert sched.rsets_free == 2, f"Free slots found {sched.rsets_free}"
             del sched
             rset_team = None
     del resources
 
 
 def test_across_nodes_roundup_option_3nodes():
     """Tests assignment over two nodes"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(9, 3)
 
     # Options should make no difference
     for match_slots in [False, True]:
         for split2fit in [False, True]:
             sched_options = {"match_slots": match_slots, "split2fit": split2fit}
             sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
             rset_team = sched.assign_resources(rsets_req=7)
             # Expecting even split
             assert rset_team == [0, 1, 2, 3, 4, 5, 6, 7, 8], "Even split test did not get expected result {}".format(
                 rset_team
             )
-            assert sched.rsets_free == 0, "Free slots found {}".format(sched.rsets_free)
+            assert sched.rsets_free == 0, f"Free slots found {sched.rsets_free}"
             del sched
             rset_team = None
     del resources
 
 
 def test_try1node_findon_2nodes_matching_slots():
     """Tests finding gaps on two nodes with matching slots"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
 
     fixed_assignments = [
         ([1, 1, 0, 0, 3, 3, 0, 0]),
         ([0, 1, 0, 2, 0, 4, 0, 4]),
         ([0, 1, 1, 0, 0, 2, 2, 0]),
         ([1, 0, 1, 0, 3, 0, 3, 0]),
@@ -329,15 +329,15 @@
         del sched
         rset_team = None
     del resources
 
 
 def test_try1node_findon_2nodes_different_slots():
     """Tests finding gaps on two nodes with non-matching slots"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
 
     fixed_assignments = [
         ([1, 1, 0, 0, 0, 2, 2, 0]),
         ([1, 1, 0, 0, 0, 0, 3, 3]),
         ([1, 0, 0, 1, 0, 3, 0, 3]),
     ]
@@ -354,50 +354,50 @@
         sched.match_slots = False
         sched.split2fit = False
         _fail_to_resource(sched, 4)
 
         # Now with match slots False and split2fit True - should find.
         sched.split2fit = True
         rset_team = sched.assign_resources(rsets_req=4)
-        assert rset_team == exp_out[i], "Expected {}, Received rset_team {}".format(exp_out[i], rset_team)
+        assert rset_team == exp_out[i], f"Expected {exp_out[i]}, Received rset_team {rset_team}"
 
         del sched
         rset_team = None
     del resources
 
 
 def test_try1node_findon_3nodes():
     """Tests finding gaps on two nodes as cannot fit on one due to others assigned"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(12, 3)
     resources.fixed_assignment(([1, 1, 0, 0, 0, 2, 2, 0, 3, 0, 3, 3]))
     sched = ResourceScheduler(user_resources=resources)
 
     # Default - with match_slots - cannot find a split with matching slots
     _fail_to_resource(sched, 3)
 
     # Can find non-matching slots across three nodes
     sched_options = {"match_slots": False}
     del sched
     sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
     rset_team = sched.assign_resources(rsets_req=3)
-    assert rset_team == [2, 4, 9], "rsets found {}".format(rset_team)
+    assert rset_team == [2, 4, 9], f"rsets found {rset_team}"
 
     # Without split2fit, will not split over nodes.
     sched_options = {"match_slots": False, "split2fit": False}
     del sched
     sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
     _fail_to_resource(sched, 3)
 
     # Now free up resources on 1st group and call alloc again (new sched as change to resources).
     resources.free_rsets(worker=1)
     del sched
     sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
     rset_team = sched.assign_resources(rsets_req=3)
-    assert rset_team == [0, 1, 2], "rsets found {}".format(rset_team)
+    assert rset_team == [0, 1, 2], f"rsets found {rset_team}"
     del resources
 
 
 def test_try2nodes_findon_3nodes():
     """Tests finding gaps on two nodes as cannot fit on one due to others assigned
 
     Assigned means assigned to workerID (1 and 3 in this case).
@@ -417,29 +417,29 @@
 
     match slots:    x
     rset ID:     0  1  2  3  4  5   6  7  8  9  10 11   12 13 14 15 16 17
     slots ID:    0  1  2  3  4  5   0  1  2  3  4  5    0  1  2  3  4  5
     assigned:    0  1  0  0  0  0   0  0  0  0  0  0    0  0  0  0  0  0
 
     """
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(18, 3)
     resources.fixed_assignment(([0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3]))
     sched = ResourceScheduler(user_resources=resources)
 
     # Can't find 2 groups of 6 so find 3 groups of 4 - with matching slots.
     rset_team = sched.assign_resources(rsets_req=12)
-    assert rset_team == [0, 2, 3, 4, 6, 8, 9, 10, 12, 14, 15, 16], "rsets found {}".format(rset_team)
+    assert rset_team == [0, 2, 3, 4, 6, 8, 9, 10, 12, 14, 15, 16], f"rsets found {rset_team}"
 
     # Without matching slots, will find first available slots on each node.
     sched_options = {"match_slots": False}
     del sched
     sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
     rset_team = sched.assign_resources(rsets_req=12)
-    assert rset_team == [0, 2, 3, 4, 6, 7, 8, 9, 12, 13, 14, 15], "rsets found {}".format(rset_team)
+    assert rset_team == [0, 2, 3, 4, 6, 7, 8, 9, 12, 13, 14, 15], f"rsets found {rset_team}"
 
     # Simulate a new call to allocation function with split2fit False - unable to split to 3 nodes.
     sched_options = {"match_slots": False, "split2fit": False}
     del sched
     sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
     _fail_to_resource(sched, 12)
 
@@ -449,75 +449,75 @@
     for match_slots in [False, True]:
         for split2fit in [False, True]:
             sched_options = {"match_slots": match_slots, "split2fit": split2fit}
 
             del sched
             sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
             rset_team = sched.assign_resources(rsets_req=12)
-            assert rset_team == [6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17], "rsets found {}".format(rset_team)
+            assert rset_team == [6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17], f"rsets found {rset_team}"
 
             del sched
             sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
             rset_team = sched.assign_resources(rsets_req=12)
-            assert rset_team == [6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17], "rsets found {}".format(rset_team)
+            assert rset_team == [6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17], f"rsets found {rset_team}"
     del resources
 
 
 def test_split2fit_even_required_fails():
     """Test tries one node then two, and both fail"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
     resources.fixed_assignment(([1, 1, 1, 0, 2, 2, 0, 0]))
 
     for match_slots in [False, True]:
         sched_options = {"match_slots": match_slots}
         sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
         _fail_to_resource(sched, 4)
         assert sched.rsets_free == 3
 
 
 def test_split2fit_even_required_various():
     """Tests trying to fit to an non-even partition, and setting of local rsets_free"""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
     resources.fixed_assignment(([1, 1, 1, 0, 0, 0, 0, 0]))
     sched = ResourceScheduler(user_resources=resources)
     assert sched.rsets_free == 5
 
     rset_team = sched.assign_resources(rsets_req=2)
-    assert rset_team == [4, 5], "rsets found {}".format(rset_team)
+    assert rset_team == [4, 5], f"rsets found {rset_team}"
     assert sched.rsets_free == 3
 
     # In same alloc - now try getting 4 rsets, then 3
     _fail_to_resource(sched, 4)
     assert sched.rsets_free == 3
     _fail_to_resource(sched, 3)
     assert sched.rsets_free == 3
 
     rset_team = sched.assign_resources(rsets_req=2)
-    assert rset_team == [6, 7], "rsets found {}".format(rset_team)
+    assert rset_team == [6, 7], f"rsets found {rset_team}"
     assert sched.rsets_free == 1
 
 
 def test_try1node_findon_2_or_4nodes():
     """Tests splitting to fit. Needs 4 nodes if matching slots, else 2."""
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(16, 4)
     resources.fixed_assignment(([1, 1, 0, 1, 2, 2, 0, 0, 1, 0, 0, 1, 0, 4, 0, 4]))
 
     sched = ResourceScheduler(user_resources=resources)
     rset_team = sched.assign_resources(rsets_req=4)
-    assert rset_team == [2, 6, 10, 14], "rsets found {}".format(rset_team)
+    assert rset_team == [2, 6, 10, 14], f"rsets found {rset_team}"
     del sched
     rset_team = None  # I think should always do between tests (esp if expected output is the same).
 
     sched_options = {"match_slots": False}  # will prob be default.
     sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)  # noqa E702
     rset_team = sched.assign_resources(rsets_req=4)
-    assert rset_team == [6, 7, 9, 10], "rsets found {}".format(rset_team)
+    assert rset_team == [6, 7, 9, 10], f"rsets found {rset_team}"
     del resources
 
 
 def _construct_large_problem(resources):
     """Constructs rset assignment for large problem"""
     rsets = resources.rsets
 
@@ -553,15 +553,15 @@
 def test_large_match_slots():
     """Tests multiple match slots iterations
 
     Aim is try one of 16, then 2 of 8, then 4 or 4 and 8 or 2 then 16 of one.
     To do this need enough slots at each step so tries to find, but in the
     wrong places, until final iteration. Performance is of interest.
     """
-    print("\nTest: {}\n".format(sys._getframe().f_code.co_name))
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
 
     # Construct rset assignment
     resources = MyResources(256, 16)
     _construct_large_problem(resources)
 
     exp_out = [
         [0, 1, 2, 3, 4, 5, 6, 7, 24, 25, 26, 27, 28, 29, 30, 31],
@@ -573,15 +573,15 @@
         sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
         time1 = time.time()
         rset_team = sched.assign_resources(rsets_req=16)
         time2 = time.time() - time1
         assert rset_team == exp_out[match_slots], "Expected {}, Received rset_team {}".format(
             exp_out[match_slots], rset_team
         )
-        print("Time for large problem (match_slots {}): {}".format(match_slots, time2))
+        print(f"Time for large problem (match_slots {match_slots}): {time2}")
         del sched
         rset_team = None
     del resources
 
 
 if __name__ == "__main__":
     test_request_zero_rsets()
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_resources.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 def teardown_standalone_run():
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = ""
     if os.path.isfile("node_list"):
         os.remove("node_list")
 
 
 def setup_function(function):
-    print("setup_function    function:%s" % function.__name__)
+    print(f"setup_function    function:{function.__name__}")
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = ""
     # if os.environ['LIBE_RESOURCES_TEST_NODE_LIST']:
     #     del os.environ['LIBE_RESOURCES_TEST_NODE_LIST']
     # if os.environ['THIS_ENV_VARIABLE_IS_DEF_NOT_SET']:
     #     del os.environ['THIS_ENV_VARIABLE_IS_DEF_NOT_SET']
     if os.path.isfile("node_list"):
         os.remove("node_list")
 
 
 def teardown_function(function):
-    print("teardown_function    function:%s" % function.__name__)
+    print(f"teardown_function    function:{function.__name__}")
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = ""
     # if os.environ['LIBE_RESOURCES_TEST_NODE_LIST']:
     #     del os.environ['LIBE_RESOURCES_TEST_NODE_LIST']
     # if os.environ['THIS_ENV_VARIABLE_IS_DEF_NOT_SET']:
     #     del os.environ['THIS_ENV_VARIABLE_IS_DEF_NOT_SET']
     if os.path.isfile("node_list"):
         os.remove("node_list")
@@ -255,15 +255,15 @@
             nodes_in.append(mynode)
     nodes_out = GlobalResources.remove_nodes(nodes_in, mynode)
     assert nodes_out == exp_out, "nodelist returned does not match expected"
 
 
 def _assert_worker_attr(wres, attr, exp):
     ret = getattr(wres, attr)
-    assert ret == exp, "{} returned does not match expected.  \nRet: {}\nExp: {}".format(attr, ret, exp)
+    assert ret == exp, f"{attr} returned does not match expected.  \nRet: {ret}\nExp: {exp}"
 
 
 # These are all 1 worker per rset.
 def _worker_asserts(wres, split_list, exp_slots, wrk, nworkers, nnodes, reps=1):
 
     # Create dictionary of attributes and expected values
     exp_dict = {
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_scipy.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_scipy.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 def test_cdist_issue():
     try:
         from scipy.spatial.distance import cdist
     except ModuleNotFoundError:
         pytest.skip("scipy or its dependencies not importable. Skipping.")
 
     """There is an issue (at least in scipy 1.1.0) with cdist segfaulting."""
-
     H = np.zeros(
         20,
         dtype=[
             ("x", "<f8", (2,)),
             ("m", "<i8"),
             ("a", "<f8"),
             ("b", "?"),
@@ -36,15 +35,14 @@
     dist_1 = cdist(np.atleast_2d(H["x"][3]), H["x"], "euclidean")
     assert len(dist_1), "We didn't segfault"
 
 
 @pytest.mark.extra
 def test_save():
     """Seeing if I can save parts of the H array."""
-
     from libensemble.tests.regression_tests.support import uniform_or_localopt_gen_out as gen_out
 
     n = 2
     gen_out += [("x", float, n), ("x_on_cube", float, n)]
     H = np.zeros(20, dtype=gen_out + [("f", float), ("grad", float, n)])
     np.random.seed(1)
     H["x"] = np.random.uniform(0, 1, (20, 2))
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_sim_dir_properties.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_sim_dir_properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 import os
+import pytest
 import shutil
 import numpy as np
 from libensemble.output_directory import EnsembleDirectory
 from libensemble.utils.loc_stack import LocationStack
+from libensemble.utils.misc import extract_H_ranges
 
 
 def test_range_single_element():
     """Single H_row labeling"""
-
     work = {"H_fields": ["x", "num_nodes", "procs_per_node"], "libE_info": {"H_rows": np.array([5]), "workerID": 1}}
-    assert EnsembleDirectory.extract_H_ranges(work) == "5", "Failed to correctly parse single H row"
+    assert extract_H_ranges(work) == "5", "Failed to correctly parse single H row"
 
 
 def test_range_two_separate_elements():
     """Multiple H_rows, non-sequential"""
-
     work = {"H_fields": ["x", "num_nodes", "procs_per_node"], "libE_info": {"H_rows": np.array([2, 8]), "workerID": 1}}
-    assert EnsembleDirectory.extract_H_ranges(work) == "2_8", "Failed to correctly parse nonsequential H rows"
+    assert extract_H_ranges(work) == "2_8", "Failed to correctly parse nonsequential H rows"
 
 
 def test_range_two_ranges():
     """Multiple sequences of H_rows"""
-
     work = {
         "H_fields": ["x", "num_nodes", "procs_per_node"],
         "libE_info": {"H_rows": np.array([0, 1, 2, 3, 7, 8]), "workerID": 1},
     }
-    assert EnsembleDirectory.extract_H_ranges(work) == "0-3_7-8", "Failed to correctly parse multiple H ranges"
+    assert extract_H_ranges(work) == "0-3_7-8", "Failed to correctly parse multiple H ranges"
 
 
 def test_range_mixes():
     """Mix of single rows and sequences of H_rows"""
-
     work = {
         "H_fields": ["x", "num_nodes", "procs_per_node"],
         "libE_info": {"H_rows": np.array([2, 3, 4, 6, 8, 9, 11, 14]), "workerID": 1},
     }
-    assert (
-        EnsembleDirectory.extract_H_ranges(work) == "2-4_6_8-9_11_14"
-    ), "Failed to correctly parse H row single elements and ranges."
+    assert extract_H_ranges(work) == "2-4_6_8-9_11_14", "Failed to correctly parse H row single elements and ranges."
 
 
 def test_copy_back():
     """When workers conclude their work, workers have the option of copying
     back their work into a directory created by the manager."""
 
     inputdir = "./calc"
@@ -84,14 +80,15 @@
     assert "worker1" in os.listdir(ensemble_dir)
     assert "file" in os.listdir(os.path.join(ensemble_dir, "worker1"))
 
     for dir in [inputdir, ensemble_dir]:
         shutil.rmtree(dir)
 
 
+@pytest.mark.extra
 def test_loc_stack_FileExists_exceptions():
     inputdir = "./calc"
     copyfile = "./calc/copy"
     symlinkfile = "./calc/symlink"
     ensemble_dir = "./test_ens"
 
     for dir in [inputdir, copyfile, symlinkfile]:
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_task_funcs.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_task_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import time
 
 from libensemble.executors.executor import Task, Executor, ExecutorException
 from libensemble.executors.mpi_executor import MPIExecutor
 
 
 def setup_module(module):
-    print("setup_module      module:%s" % module.__name__)
+    print(f"setup_module      module:{module.__name__}")
     if Executor.executor is not None:
         del Executor.executor
         Executor.executor = None
 
 
 def setup_function(function):
-    print("setup_function    function:%s" % function.__name__)
+    print(f"setup_function    function:{function.__name__}")
     if Executor.executor is not None:
         del Executor.executor
         Executor.executor = None
 
 
 def teardown_module(module):
-    print("teardown_module   module:%s" % module.__name__)
+    print(f"teardown_module   module:{module.__name__}")
     if Executor.executor is not None:
         del Executor.executor
         Executor.executor = None
 
 
 def test_task_funcs():
     dummyappname = os.getcwd() + "/myapp.x"
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/test_timer.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/test_timer.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     assert e2 == e3, "Check elapsed time stable when timer inactive."
 
     s1 = timer.date_start
     s2 = timer.date_end
     assert s1[0:2] == "20", "Start year is 20xx"
     assert s2[0:2] == "20", "End year is 20xx"
 
-    s3 = "{}".format(timer)
-    assert s3 == "Time: {0:.3f} Start: {1} End: {2}".format(e3, s1, s2), "Check string formatting."
+    s3 = f"{timer}"
+    assert s3 == f"Time: {e3:.3f} Start: {s1} End: {s2}", "Check string formatting."
 
     time.sleep(0.2)
     time_start = time.time()
     with timer:
         time.sleep(0.5)
         total1 = timer.total
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests/tofix__test_worker.py` & `libensemble-0.9.3/libensemble/tests/unit_tests/tofix__test_worker.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests_logger/test_logger.py` & `libensemble-0.9.3/libensemble/tests/unit_tests_logger/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,18 @@
     logger.set_filename("toolate.log")
     assert logs.filename == alt_name, "Log filename expected " + str(alt_name) + ". Found: " + logs.filename
 
     assert os.path.isfile(alt_name), "Expected creation of file" + str(alt_name)
     with open(alt_name, "r") as f:
         line = f.readline()
         assert "Cannot set filename after loggers initialized" in line
-    os.remove(alt_name)
+    try:
+        os.remove(alt_name)
+    except PermissionError:  # windows only
+        pass
 
     logs = LogConfig.config
     logs.logger_set = True
     logs.set_level("DEBUG")
 
 
 def test_set_stderr_level():
```

### Comparing `libensemble-0.9.2/libensemble/tests/unit_tests_nompi/test_aaa_comms.py` & `libensemble-0.9.3/libensemble/tests/unit_tests_nompi/test_aaa_comms.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 Note that this must come before anything that loads PETSc, since PETSc
 installs a SIGTERM handler.  Temporarily uninstalled from the test suite,
 since pytest slurps up everything (including all the modules) in one go.
 """
 
 import time
+import pytest
 import signal
 import libensemble.comms.comms as comms
 
 
 def worker_main(comm):
     return
 
@@ -51,14 +52,15 @@
         assert not mgr_comm.running
 
 
 def ignore_handler(signum, frame):
     print("Ignoring SIGTERM")
 
 
+@pytest.mark.extra
 def test_qcomm_proc_terminate3():
     "Test that a QCommProcess ignoring SIGTERM manages."
 
     with comms.QCommProcess(worker_main_waiting, 2) as mgr_comm:
         time.sleep(0.5)
 
         flag = True
```

### Comparing `libensemble-0.9.2/libensemble/tools/alloc_support.py` & `libensemble-0.9.3/libensemble/tools/alloc_support.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import logging
 from libensemble.message_numbers import EVAL_SIM_TAG, EVAL_GEN_TAG
 from libensemble.resources.resources import Resources
 from libensemble.resources.scheduler import ResourceScheduler, InsufficientFreeResources  # noqa: F401
-from libensemble.output_directory import EnsembleDirectory
+from libensemble.utils.misc import extract_H_ranges
 
 logger = logging.getLogger(__name__)
 # For debug messages - uncomment
 # logger.setLevel(logging.DEBUG)
 
 
 class AllocException(Exception):
@@ -174,19 +174,15 @@
         work = {
             "H_fields": H_fields,
             "persis_info": persis_info,
             "tag": EVAL_SIM_TAG,
             "libE_info": libE_info,
         }
 
-        logger.debug(
-            "Alloc func packing SIM work for worker {}. Packing sim_ids: {}".format(
-                wid, EnsembleDirectory.extract_H_ranges(work) or None
-            )
-        )
+        logger.debug(f"Alloc func packing SIM work for worker {wid}. Packing sim_ids: {extract_H_ranges(work) or None}")
         return work
 
     def gen_work(self, wid, H_fields, H_rows, persis_info, **libE_info):
         """Add gen work record to given ``Work`` dictionary.
 
          Includes evaluation of required resources if the worker is not in a
          persistent state.
@@ -218,19 +214,15 @@
         work = {
             "H_fields": H_fields,
             "persis_info": persis_info,
             "tag": EVAL_GEN_TAG,
             "libE_info": libE_info,
         }
 
-        logger.debug(
-            "Alloc func packing GEN work for worker {}. Packing sim_ids: {}".format(
-                wid, EnsembleDirectory.extract_H_ranges(work) or None
-            )
-        )
+        logger.debug(f"Alloc func packing GEN work for worker {wid}. Packing sim_ids: {extract_H_ranges(work) or None}")
         return work
 
     def _filter_points(self, H_in, pt_filter, low_bound):
         """Returns H and pt_filter filted by lower bound
 
         :param pt_filter: Optional boolean array filtering expected returned points in ``H``.
         :param low_bound: Optional lower bound for testing all returned.
@@ -316,18 +308,18 @@
         H_rows = np.atleast_1d(H_rows)  # Makes sure a numpy scalar is an ndarray
 
         if isinstance(H_rows, np.ndarray):
             return H_rows
         try:
             H_rows = np.fromiter(H_rows, int)
         except Exception:
-            raise AllocException("H_rows could not be converted to a numpy array. Type {}".format(type(H_rows)))
+            raise AllocException(f"H_rows could not be converted to a numpy array. Type {type(H_rows)}")
         return H_rows
 
     @staticmethod
     def _check_H_fields(H_fields):
         """Ensure no duplicates in H_fields"""
         if len(H_fields) != len(set(H_fields)):
-            logger.debug("Removing duplicate field(s) when packing work request. {}".format(H_fields))
+            logger.debug(f"Removing duplicate field(s) when packing work request. {H_fields}")
             H_fields = list(set(H_fields))
             # H_fields = list(OrderedDict.fromkeys(H_fields))  # Maintain order
         return H_fields
```

### Comparing `libensemble-0.9.2/libensemble/tools/check_inputs.py` & `libensemble-0.9.3/libensemble/tools/check_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 )
 
 logger = logging.getLogger(__name__)
 
 
 def _check_consistent_field(name, field0, field1):
     """Checks that new field (field1) is compatible with an old field (field0)."""
-    assert field0.ndim == field1.ndim, "H0 and H have different ndim for field {}".format(name)
+    assert field0.ndim == field1.ndim, f"H0 and H have different ndim for field {name}"
     assert np.all(
         np.array(field1.shape) >= np.array(field0.shape)
-    ), "H too small to receive all components of H0 in field {}".format(name)
+    ), f"H too small to receive all components of H0 in field {name}"
 
 
 def check_libE_specs(libE_specs, serial_check=False):
     assert isinstance(libE_specs, dict), "libE_specs must be a dictionary"
 
     comms_type = libE_specs.get("comms", "mpi")
     if comms_type in ["mpi"]:
@@ -36,33 +36,27 @@
     for k in libE_specs.keys():
         assert k in allowed_libE_spec_keys, "Key %s is not allowed in libE_specs. Supported keys are: %s " % (
             k,
             allowed_libE_spec_keys,
         )
 
         if k in ["ensemble_copy_back", "use_worker_dirs", "sim_dirs_make", "gen_dirs_make"]:
-            assert isinstance(libE_specs[k], bool), "Value for libE_specs['{}'] must be boolean".format(k)
+            assert isinstance(libE_specs[k], bool), f"Value for libE_specs['{k}'] must be boolean"
 
         if k in ["sim_input_dir", "gen_input_dir"]:
-            assert isinstance(
-                libE_specs[k], str
-            ), "Value for libE_specs['{}'] must be a single path-like string".format(k)
-            assert os.path.exists(libE_specs[k]), "libE_specs['{}'] does not refer to an existing path.".format(k)
+            assert isinstance(libE_specs[k], str), f"Value for libE_specs['{k}'] must be a single path-like string"
+            assert os.path.exists(libE_specs[k]), f"libE_specs['{k}'] does not refer to an existing path."
 
         if k == "ensemble_dir_path":
-            assert isinstance(
-                libE_specs[k], str
-            ), "Value for libE_specs['{}'] must be a single path-like string".format(k)
+            assert isinstance(libE_specs[k], str), f"Value for libE_specs['{k}'] must be a single path-like string"
 
         if k in ["sim_dir_copy_files", "sim_dir_symlink_files", "gen_dir_copy_files", "gen_dir_symlink_files"]:
-            assert isinstance(
-                libE_specs[k], list
-            ), "Value for libE_specs['{}'] must be a list of path-like strings".format(k)
+            assert isinstance(libE_specs[k], list), f"Value for libE_specs['{k}'] must be a list of path-like strings"
             for j in libE_specs[k]:
-                assert os.path.exists(j), "'{}' in libE_specs['{}'] does not refer to an existing path.".format(j, k)
+                assert os.path.exists(j), f"'{j}' in libE_specs['{k}'] does not refer to an existing path."
 
 
 def check_alloc_specs(alloc_specs):
     assert isinstance(alloc_specs, dict), "alloc_specs must be a dictionary"
 
     assert alloc_specs["alloc_f"], "Allocation function must be specified"
```

### Comparing `libensemble-0.9.2/libensemble/tools/consensus_subroutines.py` & `libensemble-0.9.3/libensemble/tools/consensus_subroutines.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,15 +306,15 @@
     for line in fp.readlines():
         line = line.rsplit()[0]
         data = line.split(",")
         label[i] = data[1] == "M"
         datas[i, :] = [float(val) for val in data[2:32]]
         i += 1
 
-    assert i == n, "Expected {} datapoints, recorded {}".format(n, i)
+    assert i == n, f"Expected {n} datapoints, recorded {i}"
 
     return label, datas
 
 
 def gm_opt(b, m):
     """Computes optimal geometric median score
 
@@ -363,15 +363,15 @@
     if reg == "l1":
         p = 1
     elif reg == "l2":
         p = 2
     elif reg is None:
         p = -1
     else:
-        assert False, 'illegal regularization "{}"'.format(reg)
+        assert False, f'illegal regularization "{reg}"'
 
     def obj_fn(X, y, beta, c, p):
         m = X.shape[0]
         if p == 1:
             return (1 / m) * np.linalg.norm(X @ beta - y, ord=2) ** 2 + c * np.linalg.norm(beta, ord=1)
         return (1 / m) * np.linalg.norm(X @ beta - y, ord=2) ** 2 + c * np.linalg.norm(beta, ord=2) ** 2
```

### Comparing `libensemble-0.9.2/libensemble/tools/fields_keys.py` & `libensemble-0.9.3/libensemble/tools/fields_keys.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tools/forkable_pdb.py` & `libensemble-0.9.3/libensemble/tools/forkable_pdb.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/tools/parse_args.py` & `libensemble-0.9.3/libensemble/tools/parse_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,18 @@
     nargs="?",
     choices=["local", "tcp", "ssh", "client", "mpi"],
     default="mpi",
     help="Type of communicator",
 )
 parser.add_argument("--nworkers", type=int, nargs="?", help="Number of local forked processes")
 parser.add_argument(
-    "--nsim_workers", type=int, nargs="?", help="Number of workers for sims. 1+ zero-resource gen worker will be added"
+    "--nsim_workers",
+    type=int,
+    nargs="?",
+    help="Number of workers for sims. 1+ unresourced workers for a persistent generator will be added",
 )
 parser.add_argument("--nresource_sets", type=int, nargs="?", help="Number of resource sets")
 parser.add_argument("--workers", type=str, nargs="+", help="List of worker nodes")
 parser.add_argument("--workerID", type=int, nargs="?", help="Client worker ID")
 parser.add_argument("--server", type=str, nargs=3, help="Triple of (ip, port, authkey) used to reach manager")
 parser.add_argument("--pwd", type=str, nargs="?", help="Working directory to be used")
 parser.add_argument("--worker_pwd", type=str, nargs="?", help="Working directory on remote client")
@@ -52,33 +55,34 @@
 
     if args.nresource_sets is not None:
         libE_specs["num_resource_sets"] = args.nresource_sets
 
     # Convenience option which sets other libE_specs options.
     nsim_workers = args.nsim_workers
     if nsim_workers is not None:
-        libE_specs["zero_resource_workers"] = _get_zrw(nworkers, nsim_workers)
+        # libE_specs["zero_resource_workers"] = _get_zrw(nworkers, nsim_workers)
+        libE_specs["num_resource_sets"] = libE_specs.get("num_resource_sets", nsim_workers)
 
     return nworkers, is_manager, libE_specs, args.tester_args
 
 
 def _local_parse_args(args):
     """Parses arguments for forked processes using multiprocessing."""
-
     libE_specs = {"comms": "local"}
     nworkers = args.nworkers
 
     if args.nresource_sets is not None:
         libE_specs["num_resource_sets"] = args.nresource_sets
 
     # Convenience option which sets other libE_specs options.
     nsim_workers = args.nsim_workers
     if nsim_workers is not None:
         nworkers = nworkers or nsim_workers + 1
-        libE_specs["zero_resource_workers"] = _get_zrw(nworkers, nsim_workers)
+        # libE_specs["zero_resource_workers"] = _get_zrw(nworkers, nsim_workers)
+        libE_specs["num_resource_sets"] = libE_specs.get("num_resource_sets", nsim_workers)
 
     nworkers = nworkers or 4
     libE_specs["nworkers"] = nworkers
 
     return nworkers, True, libE_specs, args.tester_args
 
 
@@ -121,15 +125,15 @@
         "{authkey}",
         "--workerID",
         "{workerID}",
         "--nworkers",
         str(nworkers),
     ]
     cmd = " ".join(cmd)
-    cmd = "( cd {} ; {} )".format(worker_pwd, cmd)
+    cmd = f"( cd {worker_pwd} ; {cmd} )"
     ssh.append(cmd)
     libE_specs = {"workers": args.workers, "worker_cmd": ssh, "ip": "localhost", "comms": "tcp"}
     return nworkers, True, libE_specs, args.tester_args
 
 
 def _client_parse_args(args):
     """Parses arguments for a TCP client."""
@@ -174,29 +178,31 @@
 
         Note that running via an MPI runner uses the default 'mpi' comms, and '--nworkers'
         will be ignored. The number of processes are supplied via the MPI run line. One being
         the manager, and the rest are workers.
 
         --comms,          Communications medium for manager and workers. Default is 'mpi'.
         --nworkers,       (For 'local' or 'tcp' comms) Set number of workers.
-        --nsim_workers,   (For 'local' or 'mpi' comms) A convenience option for common cases.
-                          If used with no other criteria, will generate one additional
-                          zero-resource worker for use as a generator. If the number of workers
-                          has also been specified, will generate enough zero-resource workers to
-                          match the other criteria.
         --nresource_sets, Explicitly set the number of resource sets. This sets
                           libE_specs['num_resource_sets']. By default, resources will be
                           divided by workers (excluding zero_resource_workers).
+        --nsim_workers,   (For 'local' or 'mpi' comms) A convenience option for cases with
+                          persistent generators - sets the number of simulation workers.
+                          If used with no other criteria, one additional worker for running a
+                          generator will be added, and the number of resource sets will be assigned
+                          the given value. If '--nworkers' has also been specified, will generate
+                          enough additional workers to match the other criteria. If '--nresource_sets'
+                          is also specified, will not override resource sets.
 
         Example command lines:
 
         Run with 'local' comms and 4 workers
         $ python calling_script --comms local --nworkers 4
 
-        Run with 'local' comms and 5 workers - one gen (no resources), and 4 sims.
+        Run with 'local' comms and 5 workers - one gen worker (no resources), and 4 sim workers.
         $ python calling_script --comms local --nsim_workers 4
 
         Run with 'local' comms with 4 workers and 8 resource sets. The extra resource sets will
         be used for larger simulations (using variable resource assignment).
         $ python calling_script --comms local --nresource_sets 8
 
         Previous example with 'mpi' comms.
@@ -224,9 +230,9 @@
         "ssh": _ssh_parse_args,
         "client": _client_parse_args,
     }
     if args.pwd is not None:
         os.chdir(args.pwd)
     nworkers, is_manager, libE_specs, tester_args = front_ends[args.comms or "mpi"](args)
     if is_manager and unknown:
-        logger.warning("parse_args ignoring unrecognized arguments: {}".format(" ".join(unknown)))
+        logger.warning(f"parse_args ignoring unrecognized arguments: {' '.join(unknown)}")
     return nworkers, is_manager, libE_specs, tester_args
```

### Comparing `libensemble-0.9.2/libensemble/tools/persistent_support.py` & `libensemble-0.9.3/libensemble/tools/persistent_support.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from libensemble.message_numbers import STOP_TAG, PERSIS_STOP, UNSET_TAG, EVAL_GEN_TAG, EVAL_SIM_TAG, calc_type_strings
 import logging
+import numpy as np
 
 logger = logging.getLogger(__name__)
 
 
 class PersistentSupport:
     """A helper class to assist with writing persistent user functions."""
 
@@ -17,88 +18,108 @@
         """
         self.libE_info = libE_info
         self.comm = self.libE_info["comm"]
         self.calc_type = calc_type
         assert self.calc_type in [
             EVAL_GEN_TAG,
             EVAL_SIM_TAG,
-        ], "The calc_type: {} specifies neither a simulator nor generator.".format(self.calc_type)
+        ], f"The calc_type: {self.calc_type} specifies neither a simulator nor generator."
         self.calc_str = calc_type_strings[self.calc_type]
 
-    def send(self, output, calc_status=UNSET_TAG):
+    def send(self, output, calc_status=UNSET_TAG, keep_state=False):
         """
         Send message from worker to manager.
 
         :param output: Output array to be sent to manager
         :param calc_status: Optional, Provides a task status
+        :param keep_state: Optional, If True the manager will not modify its
+            record of the workers state (usually the manager changes the
+            worker's state to inactive, indicating the worker is ready to receive
+            more work, unless using active receive mode).
 
         :returns: None
 
         """
         if "comm" in self.libE_info:
             # Need to make copy before remove comm as original could be reused
             libE_info = dict(self.libE_info)
             libE_info.pop("comm")
         else:
             libE_info = self.libE_info
 
+        libE_info["keep_state"] = keep_state
+
         D = {
             "calc_out": output,
             "libE_info": libE_info,
             "calc_status": calc_status,
             "calc_type": self.calc_type,
         }
-        logger.debug("Persistent {} function sending data message to manager".format(self.calc_str))
+        logger.debug(f"Persistent {self.calc_str} function sending data message to manager")
         self.comm.send(self.calc_type, D)
 
     def recv(self, blocking=True):
         """
         Receive message to worker from manager.
 
+        :param blocking: Optional, If True (default), will block until a message is received.
+
         :returns: message tag, Work dictionary, calc_in array
 
         """
 
         if not blocking:
             if not self.comm.mail_flag():
                 return None, None, None
 
         tag, Work = self.comm.recv()  # Receive meta-data or signal
         if tag in [STOP_TAG, PERSIS_STOP]:
-            logger.debug("Persistent {} received signal {} from manager".format(self.calc_str, tag))
+            logger.debug(f"Persistent {self.calc_str} received signal {tag} from manager")
             self.comm.push_to_buffer(tag, Work)
             return tag, Work, None
         else:
-            logger.debug("Persistent {} received work request from manager".format(self.calc_str))
+            logger.debug(f"Persistent {self.calc_str} received work request from manager")
 
         # Update libE_info
         # self.libE_info = Work['libE_info']
 
         # Only replace rows - keep same dictionary
         self.libE_info["H_rows"] = Work["libE_info"]["H_rows"]
 
         data_tag, calc_in = self.comm.recv()  # Receive work rows
 
         # Check for unexpected STOP (e.g. error between sending Work info and rows)
         if data_tag in [STOP_TAG, PERSIS_STOP]:
             logger.debug(
-                "Persistent {} received signal {} ".format(self.calc_str, tag)
-                + "from manager while expecting work rows"
+                f"Persistent {self.calc_str} received signal {tag} " + "from manager while expecting work rows"
             )
             self.comm.push_to_buffer(data_tag, calc_in)
             return data_tag, calc_in, None  # calc_in is signal identifier
 
-        logger.debug("Persistent {} received work rows from manager".format(self.calc_str))
+        logger.debug(f"Persistent {self.calc_str} received work rows from manager")
         return tag, Work, calc_in
 
     def send_recv(self, output, calc_status=UNSET_TAG):
         """
         Send message from worker to manager and receive response.
 
         :param output: Output array to be sent to manager
         :param calc_status: Optional, Provides a task status
 
         :returns: message tag, Work dictionary, calc_in array
 
         """
         self.send(output, calc_status)
         return self.recv()
+
+    def request_cancel_sim_ids(self, sim_ids):
+        """Request cancellation of sim_ids
+
+        :param sim_ids: A list of sim_ids to cancel
+
+        A message is sent to the manager to mark requested sim_ids as cancel_requested
+        """
+        H_o = np.zeros(len(sim_ids), dtype=[("sim_id", int), ("cancel_requested", bool)])
+        H_o["sim_id"] = sim_ids
+        H_o["cancel_requested"] = True
+        print(H_o)
+        self.send(H_o, keep_state=True)
```

### Comparing `libensemble-0.9.2/libensemble/tools/tools.py` & `libensemble-0.9.3/libensemble/tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     short_name = script_name.split("test_", 1).pop()
     prob_str = "length=" + str(len(H)) + "_evals=" + str(sum(H["sim_ended"])) + "_workers=" + str(nworkers)
 
     h_filename = short_name + "_history_" + prob_str
     p_filename = short_name + "_persis_info_" + prob_str
 
     status_mess = " ".join(["------------------", mess, "-------------------"])
-    logger.info("{}\nSaving results to file: {}".format(status_mess, h_filename))
+    logger.info(f"{status_mess}\nSaving results to file: {h_filename}")
     np.save(h_filename, H)
 
     with open(p_filename + ".pickle", "wb") as f:
         pickle.dump(persis_info, f)
 
 
 # ===================== per-process numpy random-streams =======================
```

### Comparing `libensemble-0.9.2/libensemble/utils/launcher.py` & `libensemble-0.9.3/libensemble/utils/launcher.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/utils/loc_stack.py` & `libensemble-0.9.3/libensemble/utils/loc_stack.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/libensemble/utils/timer.py` & `libensemble-0.9.3/libensemble/utils/timer.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.tcum = 0.0
         self.tstart = 0.0
         self.tend = 0.0
         self.timing = False
 
     def __str__(self):
         """Return a string representation of the timer."""
-        return "Time: {0:.3f} Start: {1} End: {2}".format(self.total, self.date_start, self.date_end)
+        return f"Time: {self.total:.3f} Start: {self.date_start} End: {self.date_end}"
 
     @property
     def date_start(self):
         """Return a string representing the start datetime."""
         start_time = datetime.datetime.fromtimestamp(self.tstart / 1000)
         return start_time.strftime("%Y-%m-%d %H:%M:%S") + "." + str(self.tstart)[-3:]
 
@@ -87,12 +87,12 @@
 
 
 class TaskTimer(Timer):
     """Timer class used in executor tasks."""
 
     def __str__(self):
         """Return a string representation of the timer."""
-        return "{0:.3f} Tstart: {1} Tend: {2}".format(self.total, self.date_start, self.date_end)
+        return f"{self.total:.3f} Tstart: {self.date_start} Tend: {self.date_end}"
 
     def summary(self):
         """Return the total time as a string"""
-        return "{0:.3f}".format(self.total)
+        return f"{self.total:.3f}"
```

### Comparing `libensemble-0.9.2/libensemble/worker.py` & `libensemble-0.9.3/libensemble/worker.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 import numpy as np
 
 from libensemble.message_numbers import EVAL_SIM_TAG, EVAL_GEN_TAG, UNSET_TAG, STOP_TAG, PERSIS_STOP, CALC_EXCEPTION
 from libensemble.message_numbers import MAN_SIGNAL_FINISH, MAN_SIGNAL_KILL
 from libensemble.message_numbers import calc_type_strings, calc_status_strings
 from libensemble.output_directory import EnsembleDirectory
 
+from libensemble.utils.misc import extract_H_ranges
 from libensemble.utils.timer import Timer
+from libensemble.utils.runners import Runners
 from libensemble.executors.executor import Executor
 from libensemble.resources.resources import Resources
 from libensemble.comms.logs import worker_logging_config
 from libensemble.comms.logs import LogConfig
 import cProfile
 import pstats
 
@@ -130,81 +132,20 @@
         self.comm = comm
         self.dtypes = dtypes
         self.workerID = workerID
         self.libE_specs = libE_specs
         self.stats_fmt = libE_specs.get("stats_fmt", {})
 
         self.calc_iter = {EVAL_SIM_TAG: 0, EVAL_GEN_TAG: 0}
-        self._run_calc = Worker._make_runners(sim_specs, gen_specs)
+        self._run_calc = Runners(sim_specs, gen_specs).make_runners()
         Worker._set_executor(self.workerID, self.comm)
         Worker._set_resources(self.workerID, self.comm)
         self.EnsembleDirectory = EnsembleDirectory(libE_specs=libE_specs)
 
     @staticmethod
-    def _funcx_result(funcx_exctr, user_f, calc_in, persis_info, specs, libE_info):
-        libE_info["comm"] = None  # 'comm' object not pickle-able
-        Worker._set_executor(0, None)  # ditto for executor
-
-        future = funcx_exctr.submit(user_f, calc_in, persis_info, specs, libE_info, endpoint_id=specs["funcx_endpoint"])
-        remote_exc = future.exception()  # blocks until exception or None
-        if remote_exc is None:
-            return future.result()
-        else:
-            raise remote_exc
-
-    @staticmethod
-    def _get_funcx_exctr(sim_specs, gen_specs):
-        funcx_sim = len(sim_specs.get("funcx_endpoint", "")) > 0
-        funcx_gen = len(gen_specs.get("funcx_endpoint", "")) > 0
-
-        if any([funcx_sim, funcx_gen]):
-            try:
-                from funcx import FuncXClient
-                from funcx.sdk.executor import FuncXExecutor
-
-                return FuncXExecutor(FuncXClient()), funcx_sim, funcx_gen
-            except ModuleNotFoundError:
-                logger.warning("funcX use detected but funcX not importable. Is it installed?")
-                return None, False, False
-            except Exception:
-                return None, False, False
-        else:
-            return None, False, False
-
-    @staticmethod
-    def _make_runners(sim_specs, gen_specs):
-        """Creates functions to run a sim or gen. These functions are either
-        called directly by the worker or submitted to a funcX endpoint."""
-
-        funcx_exctr, funcx_sim, funcx_gen = Worker._get_funcx_exctr(sim_specs, gen_specs)
-        sim_f = sim_specs["sim_f"]
-
-        def run_sim(calc_in, persis_info, libE_info):
-            """Calls or submits the sim func."""
-            if funcx_sim and funcx_exctr:
-                return Worker._funcx_result(funcx_exctr, sim_f, calc_in, persis_info, sim_specs, libE_info)
-            else:
-                return sim_f(calc_in, persis_info, sim_specs, libE_info)
-
-        if gen_specs:
-            gen_f = gen_specs["gen_f"]
-
-            def run_gen(calc_in, persis_info, libE_info):
-                """Calls or submits the gen func."""
-                if funcx_gen and funcx_exctr:
-                    return Worker._funcx_result(funcx_exctr, gen_f, calc_in, persis_info, gen_specs, libE_info)
-                else:
-                    return gen_f(calc_in, persis_info, gen_specs, libE_info)
-
-        else:
-            run_gen = []
-
-        return {EVAL_SIM_TAG: run_sim, EVAL_GEN_TAG: run_gen}
-
-    @staticmethod
     def _set_rset_team(rset_team):
         """Pass new rset_team to worker resources"""
         resources = Resources.resources
         if isinstance(resources, Resources):
             resources.worker_resources.set_rset_team(rset_team)
             return True
         else:
@@ -214,26 +155,26 @@
     def _set_executor(workerID, comm):
         """Sets worker ID in the executor, return True if set"""
         exctr = Executor.executor
         if isinstance(exctr, Executor):
             exctr.set_worker_info(comm, workerID)  # When merge update
             return True
         else:
-            logger.debug("No executor set on worker {}".format(workerID))
+            logger.debug(f"No executor set on worker {workerID}")
             return False
 
     @staticmethod
     def _set_resources(workerID, comm):
         """Sets worker ID in the resources, return True if set"""
         resources = Resources.resources
         if isinstance(resources, Resources):
             resources.set_worker_resources(comm.get_num_workers(), workerID)
             return True
         else:
-            logger.debug("No resources set on worker {}".format(workerID))
+            logger.debug(f"No resources set on worker {workerID}")
             return False
 
     def _handle_calc(self, Work, calc_in):
         """Runs a calculation on this worker object.
 
         This routine calls the user calculations. Exceptions are caught,
         dumped to the summary file, and raised.
@@ -253,44 +194,44 @@
 
         # calc_stats stores timing and summary info for this Calc (sim or gen)
         # calc_id = next(self._calc_id_counter)
 
         # from output_directory.py
         if calc_type == EVAL_SIM_TAG:
             enum_desc = "sim_id"
-            calc_id = EnsembleDirectory.extract_H_ranges(Work)
+            calc_id = extract_H_ranges(Work)
         else:
             enum_desc = "Gen no"
             # Use global gen count if available
             if Work["libE_info"].get("gen_count"):
                 calc_id = str(Work["libE_info"]["gen_count"])
             else:
                 calc_id = str(self.calc_iter[calc_type])
         # Add a right adjust (minimum width).
         calc_id = calc_id.rjust(5, " ")
 
         timer = Timer()
 
         try:
-            logger.debug("Starting {}: {}".format(enum_desc, calc_id))
+            logger.debug(f"Starting {enum_desc}: {calc_id}")
             calc = self._run_calc[calc_type]
             with timer:
                 if self.EnsembleDirectory.use_calc_dirs(calc_type):
                     loc_stack, calc_dir = self.EnsembleDirectory.prep_calc_dir(
                         Work,
                         self.calc_iter,
                         self.workerID,
                         calc_type,
                     )
                     with loc_stack.loc(calc_dir):  # Changes to calculation directory
                         out = calc(calc_in, Work["persis_info"], Work["libE_info"])
                 else:
                     out = calc(calc_in, Work["persis_info"], Work["libE_info"])
 
-                logger.debug("Returned from user function for {} {}".format(enum_desc, calc_id))
+                logger.debug(f"Returned from user function for {enum_desc} {calc_id}")
 
             assert isinstance(out, tuple), "Calculation output must be a tuple."
             assert len(out) >= 2, "Calculation output must be at least two elements."
 
             if len(out) >= 3:
                 calc_status = out[2]
             else:
@@ -301,61 +242,58 @@
                 tag, message = self.comm.recv()
                 if tag in [STOP_TAG, PERSIS_STOP]:
                     if message is MAN_SIGNAL_FINISH:
                         calc_status = MAN_SIGNAL_FINISH
 
             return out[0], out[1], calc_status
         except Exception as e:
-            logger.debug("Re-raising exception from calc {}".format(e))
+            logger.debug(f"Re-raising exception from calc {e}")
             calc_status = CALC_EXCEPTION
             raise
         finally:
             ctype_str = calc_type_strings[calc_type]
             status = calc_status_strings.get(calc_status, calc_status)
             calc_msg = self._get_calc_msg(enum_desc, calc_id, ctype_str, timer, status)
 
             logging.getLogger(LogConfig.config.stats_name).info(calc_msg)
             # logging.getLogger(LogConfig.config.random_name).info(calc_msg)
 
     def _get_calc_msg(self, enum_desc, calc_id, calc_type, timer, status):
         """Construct line for libE_stats.txt file"""
-
-        calc_msg = "{} {}: {} {}".format(enum_desc, calc_id, calc_type, timer)
+        calc_msg = f"{enum_desc} {calc_id}: {calc_type} {timer}"
 
         if self.stats_fmt.get("task_timing", False) or self.stats_fmt.get("task_datetime", False):
             calc_msg += Executor.executor.new_tasks_timing(datetime=self.stats_fmt.get("task_datetime", False))
 
         if self.stats_fmt.get("show_resource_sets", False):
             # Maybe just call option resource_sets if already in sub-dictionary
             resources = Resources.resources.worker_resources
-            calc_msg += " rsets: {}".format(resources.rset_team)
+            calc_msg += f" rsets: {resources.rset_team}"
 
         # Always put status last as could involve different numbers of words. Some scripts may assume this.
-        calc_msg += " Status: {}".format(status)
+        calc_msg += f" Status: {status}"
 
         return calc_msg
 
     def _recv_H_rows(self, Work):
         """Unpacks Work request and receives any history rows"""
-
         libE_info = Work["libE_info"]
         calc_type = Work["tag"]
         if len(libE_info["H_rows"]) > 0:
             _, calc_in = self.comm.recv()
         else:
             calc_in = np.zeros(0, dtype=self.dtypes[calc_type])
 
-        logger.debug("Received calc_in ({}) of len {}".format(calc_type_strings[calc_type], np.size(calc_in)))
+        logger.debug(f"Received calc_in ({calc_type_strings[calc_type]}) of len {np.size(calc_in)}")
         assert calc_type in [EVAL_SIM_TAG, EVAL_GEN_TAG], "calc_type must either be EVAL_SIM_TAG or EVAL_GEN_TAG"
 
         return libE_info, calc_type, calc_in
 
     def _handle(self, Work):
         """Handles a work request from the manager"""
-
         # Check work request and receive second message (if needed)
         libE_info, calc_type, calc_in = self._recv_H_rows(Work)
 
         # Call user function
         libE_info["comm"] = self.comm
         libE_info["workerID"] = self.workerID
         libE_info["rset_team"] = libE_info.get("rset_team", [])
@@ -370,31 +308,30 @@
             del libE_info["comm"]
 
         # If there was a finish signal, bail
         if calc_status == MAN_SIGNAL_FINISH:
             return None
 
         # Otherwise, send a calc result back to manager
-        logger.debug("Sending to Manager with status {}".format(calc_status))
+        logger.debug(f"Sending to Manager with status {calc_status}")
         return {
             "calc_out": calc_out,
             "persis_info": persis_info,
             "libE_info": libE_info,
             "calc_status": calc_status,
             "calc_type": calc_type,
         }
 
     def run(self):
         """Runs the main worker loop."""
-
         try:
-            logger.info("Worker {} initiated on node {}".format(self.workerID, socket.gethostname()))
+            logger.info(f"Worker {self.workerID} initiated on node {socket.gethostname()}")
 
             for worker_iter in count(start=1):
-                logger.debug("Iteration {}".format(worker_iter))
+                logger.debug(f"Iteration {worker_iter}")
 
                 mtag, Work = self.comm.recv()
 
                 if mtag in [STOP_TAG, PERSIS_STOP]:
                     if Work is MAN_SIGNAL_FINISH:
                         break
                     elif Work is MAN_SIGNAL_KILL:
```

### Comparing `libensemble-0.9.2/libensemble.egg-info/PKG-INFO` & `libensemble-0.9.3/libensemble.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: libensemble
-Version: 0.9.2
+Version: 0.9.3
 Summary: Library to coordinate the concurrent evaluation of dynamic ensembles of calculations
 Home-page: https://github.com/Libensemble/libensemble
 Author: Jeffrey Larson, Stephen Hudson, Stefan M. Wild, David Bindel and John-Luke Navarro
 Author-email: libensemble@lists.mcs.anl.gov
 License: BSD 3-clause
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
@@ -30,9 +29,7 @@
 libEnsemble is a Python toolkit for coordinating workflows of asynchronous
 and dynamic ensembles of calculations.
 
 libEnsemble can help users take advantage of massively parallel resources to
 solve design, decision, and inference problems and expand the class of
 problems that can benefit from increased parallelism.
 
-
-
```

### Comparing `libensemble-0.9.2/libensemble.egg-info/SOURCES.txt` & `libensemble-0.9.3/libensemble.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -85,53 +85,42 @@
 docs/function_guides/generator.rst
 docs/function_guides/simulator.rst
 docs/images/ANL_CMYK.png
 docs/images/ECP_logo.png
 docs/images/balsam2.png
 docs/images/basic_6hc.png
 docs/images/basic_6hc_simple.png
-docs/images/central_balsam.png
-docs/images/centralized_new.png
 docs/images/centralized_new_detailed.png
 docs/images/centralized_new_detailed_balsam.png
 docs/images/diagram_with_persis.png
-docs/images/distributed_new.png
 docs/images/distributed_new_detailed.png
-docs/images/funcx.png
 docs/images/funcxmodel.png
 docs/images/gen_v_fail_or_cancel.png
 docs/images/history_gen1.png
 docs/images/history_gen2.png
 docs/images/history_init.png
 docs/images/history_sim1.png
 docs/images/libE_logo.png
-docs/images/libE_logo_smaller.png
 docs/images/libE_logo_white.png
 docs/images/libEnsemble_Logo.svg
 docs/images/libe_opal_complete_v_killed_511w_2044sims_1030nodes.png
 docs/images/libe_opal_util_v_time_511w_2044sims_1030nodes.png
 docs/images/localopt_6hc.png
-docs/images/logo_manager_worker.png
 docs/images/persis_add_worker.png
 docs/images/persis_wasted_node.png
 docs/images/sampling_6hc.png
 docs/images/sinex.png
-docs/images/using_new.png
 docs/images/variable_resources1.png
 docs/images/variable_resources2.png
 docs/images/variable_resources3.png
 docs/images/variable_resources_larger_rsets1.png
 docs/images/variable_resources_more_rsets1.png
 docs/images/variable_resources_persis_gen1.png
 docs/images/variable_resources_sched_opts.png
-docs/images/white.png
 docs/images/diagram_xml/balsam2.xml
-docs/images/diagram_xml/centralized_new.xml
-docs/images/diagram_xml/distributed_new.xml
-docs/images/diagram_xml/funcx.xml
 docs/images/diagram_xml/persis_add_worker.xml
 docs/images/diagram_xml/persis_wasted_node.xml
 docs/platforms/bebop.rst
 docs/platforms/cori.rst
 docs/platforms/example_scripts.rst
 docs/platforms/perlmutter.rst
 docs/platforms/platforms_index.rst
@@ -159,63 +148,45 @@
 examples/alloc_funcs/start_persistent_local_opt_gens.py
 examples/calling_scripts/run_libe_forces.py
 examples/calling_scripts/run_libe_forces_from_yaml.py
 examples/calling_scripts/run_libensemble_on_warpx.py
 examples/calling_scripts/tutorial_calling.py
 examples/calling_scripts/regression_tests/.bal_coveragerc
 examples/calling_scripts/regression_tests/.coveragerc
-examples/calling_scripts/regression_tests/1d_sampling.yaml
 examples/calling_scripts/regression_tests/__init__.py
-examples/calling_scripts/regression_tests/check_libE_stats.py
 examples/calling_scripts/regression_tests/common.py
-examples/calling_scripts/regression_tests/dont_run_test_persistent_aposmm_pounders.py
-examples/calling_scripts/regression_tests/dont_run_test_persistent_aposmm_tao_blmvm.py
-examples/calling_scripts/regression_tests/dont_run_test_persistent_aposmm_tao_nm.py
-examples/calling_scripts/regression_tests/dont_run_test_persistent_gp.py
 examples/calling_scripts/regression_tests/script_test_balsam_hworld.py
 examples/calling_scripts/regression_tests/support.py
 examples/calling_scripts/regression_tests/test_1d_sampling.py
-examples/calling_scripts/regression_tests/test_1d_sampling_from_yaml.py
-examples/calling_scripts/regression_tests/test_1d_sampling_with_profile.py
 examples/calling_scripts/regression_tests/test_evaluate_existing_sample.py
 examples/calling_scripts/regression_tests/test_evaluate_mixed_sample.py
-examples/calling_scripts/regression_tests/test_fast_alloc.py
 examples/calling_scripts/regression_tests/test_heffte.py
 examples/calling_scripts/regression_tests/test_inverse_bayes_example.py
 examples/calling_scripts/regression_tests/test_persistent_aposmm_dfols.py
 examples/calling_scripts/regression_tests/test_persistent_aposmm_exception.py
 examples/calling_scripts/regression_tests/test_persistent_aposmm_external_localopt.py
 examples/calling_scripts/regression_tests/test_persistent_aposmm_nlopt.py
 examples/calling_scripts/regression_tests/test_persistent_aposmm_periodic.py
+examples/calling_scripts/regression_tests/test_persistent_aposmm_pounders.py
 examples/calling_scripts/regression_tests/test_persistent_aposmm_scipy.py
+examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_blmvm.py
+examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_nm.py
 examples/calling_scripts/regression_tests/test_persistent_aposmm_timeout.py
 examples/calling_scripts/regression_tests/test_persistent_aposmm_with_grad.py
 examples/calling_scripts/regression_tests/test_persistent_fd_param_finder.py
+examples/calling_scripts/regression_tests/test_persistent_gp.py
 examples/calling_scripts/regression_tests/test_persistent_gp_multitask_ax.py
 examples/calling_scripts/regression_tests/test_persistent_independent.py
 examples/calling_scripts/regression_tests/test_persistent_n_agent.py
 examples/calling_scripts/regression_tests/test_persistent_pds.py
 examples/calling_scripts/regression_tests/test_persistent_prox_slide.py
-examples/calling_scripts/regression_tests/test_persistent_sampling_CUDA_variable_resources.py
-examples/calling_scripts/regression_tests/test_persistent_sim_uniform_sampling.py
 examples/calling_scripts/regression_tests/test_persistent_surmise_calib.py
 examples/calling_scripts/regression_tests/test_persistent_surmise_killsims.py
 examples/calling_scripts/regression_tests/test_persistent_tasmanian.py
 examples/calling_scripts/regression_tests/test_persistent_tasmanian_async.py
-examples/calling_scripts/regression_tests/test_persistent_uniform_gen_decides_stop.py
-examples/calling_scripts/regression_tests/test_persistent_uniform_sampling.py
-examples/calling_scripts/regression_tests/test_persistent_uniform_sampling_adv.py
-examples/calling_scripts/regression_tests/test_persistent_uniform_sampling_async.py
-examples/calling_scripts/regression_tests/test_persistent_uniform_sampling_nonblocking.py
-examples/calling_scripts/regression_tests/test_stats_output.py
-examples/calling_scripts/regression_tests/test_uniform_sampling.py
-examples/calling_scripts/regression_tests/test_uniform_sampling_cancel.py
-examples/calling_scripts/regression_tests/test_uniform_sampling_one_residual_at_a_time.py
-examples/calling_scripts/regression_tests/test_uniform_sampling_then_persistent_localopt_runs.py
-examples/calling_scripts/regression_tests/test_uniform_sampling_with_variable_resources.py
 examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ECnoise.m
 examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m
 examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/cleanup-balsam-test.sh
 examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/configure-balsam-test.sh
 examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/test_balsam_hworld.py
 examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/wrapper_obj_fun.m
 examples/gen_funcs/persistent_sampling.py
@@ -379,91 +350,93 @@
 libensemble/tests/deprecated_tests/standalone_executor_tests/set.balsam.database.sh
 libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor.py
 libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor_manager_poll.py
 libensemble/tests/deprecated_tests/standalone_executor_tests/test_executor_multi.py
 libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/my_simtask.c
 libensemble/tests/deprecated_tests/standalone_executor_tests/simdir/my_simtask.f90
 libensemble/tests/functionality_tests/.coveragerc
+libensemble/tests/functionality_tests/1d_sampling.yaml
+libensemble/tests/functionality_tests/check_libE_stats.py
+libensemble/tests/functionality_tests/test_1d_sampling_from_yaml.py
+libensemble/tests/functionality_tests/test_1d_sampling_with_profile.py
 libensemble/tests/functionality_tests/test_1d_uniform_sampling_with_comm_dup.py
 libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py
 libensemble/tests/functionality_tests/test_calc_exception.py
 libensemble/tests/functionality_tests/test_cancel_in_alloc.py
 libensemble/tests/functionality_tests/test_comms.py
 libensemble/tests/functionality_tests/test_elapsed_time_abort.py
 libensemble/tests/functionality_tests/test_executor_hworld_pass_fail.py
 libensemble/tests/functionality_tests/test_executor_hworld_timeout.py
+libensemble/tests/functionality_tests/test_executor_simple.py
+libensemble/tests/functionality_tests/test_fast_alloc.py
 libensemble/tests/functionality_tests/test_mpi_comms.py
 libensemble/tests/functionality_tests/test_mpi_runners.py
 libensemble/tests/functionality_tests/test_mpi_runners_subnode.py
 libensemble/tests/functionality_tests/test_mpi_runners_subnode_uneven.py
 libensemble/tests/functionality_tests/test_mpi_runners_supernode_uneven.py
 libensemble/tests/functionality_tests/test_mpi_runners_zrw_subnode_uneven.py
 libensemble/tests/functionality_tests/test_mpi_runners_zrw_supernode_uneven.py
+libensemble/tests/functionality_tests/test_persistent_sampling_CUDA_variable_resources.py
+libensemble/tests/functionality_tests/test_persistent_sim_uniform_sampling.py
+libensemble/tests/functionality_tests/test_persistent_uniform_gen_decides_stop.py
+libensemble/tests/functionality_tests/test_persistent_uniform_sampling.py
+libensemble/tests/functionality_tests/test_persistent_uniform_sampling_adv.py
+libensemble/tests/functionality_tests/test_persistent_uniform_sampling_async.py
+libensemble/tests/functionality_tests/test_persistent_uniform_sampling_cancel.py
+libensemble/tests/functionality_tests/test_persistent_uniform_sampling_nonblocking.py
 libensemble/tests/functionality_tests/test_runlines_adaptive_workers.py
 libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent.py
 libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent_oversubscribe_rsets.py
 libensemble/tests/functionality_tests/test_sim_dirs_per_calc.py
 libensemble/tests/functionality_tests/test_sim_dirs_per_worker.py
 libensemble/tests/functionality_tests/test_sim_dirs_with_exception.py
 libensemble/tests/functionality_tests/test_sim_dirs_with_gen_dirs.py
 libensemble/tests/functionality_tests/test_sim_input_dir_option.py
+libensemble/tests/functionality_tests/test_stats_output.py
+libensemble/tests/functionality_tests/test_uniform_sampling.py
+libensemble/tests/functionality_tests/test_uniform_sampling_cancel.py
+libensemble/tests/functionality_tests/test_uniform_sampling_one_residual_at_a_time.py
+libensemble/tests/functionality_tests/test_uniform_sampling_then_persistent_localopt_runs.py
+libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py
 libensemble/tests/functionality_tests/test_worker_exceptions.py
 libensemble/tests/functionality_tests/test_zero_resource_workers.py
 libensemble/tests/functionality_tests/test_zero_resource_workers_subnode.py
 libensemble/tests/regression_tests/.bal_coveragerc
 libensemble/tests/regression_tests/.coveragerc
-libensemble/tests/regression_tests/1d_sampling.yaml
 libensemble/tests/regression_tests/__init__.py
-libensemble/tests/regression_tests/check_libE_stats.py
 libensemble/tests/regression_tests/common.py
-libensemble/tests/regression_tests/dont_run_test_persistent_aposmm_pounders.py
-libensemble/tests/regression_tests/dont_run_test_persistent_aposmm_tao_blmvm.py
-libensemble/tests/regression_tests/dont_run_test_persistent_aposmm_tao_nm.py
-libensemble/tests/regression_tests/dont_run_test_persistent_gp.py
 libensemble/tests/regression_tests/script_test_balsam_hworld.py
 libensemble/tests/regression_tests/support.py
 libensemble/tests/regression_tests/test_1d_sampling.py
-libensemble/tests/regression_tests/test_1d_sampling_from_yaml.py
-libensemble/tests/regression_tests/test_1d_sampling_with_profile.py
 libensemble/tests/regression_tests/test_evaluate_existing_sample.py
 libensemble/tests/regression_tests/test_evaluate_mixed_sample.py
-libensemble/tests/regression_tests/test_fast_alloc.py
 libensemble/tests/regression_tests/test_heffte.py
 libensemble/tests/regression_tests/test_inverse_bayes_example.py
 libensemble/tests/regression_tests/test_persistent_aposmm_dfols.py
 libensemble/tests/regression_tests/test_persistent_aposmm_exception.py
 libensemble/tests/regression_tests/test_persistent_aposmm_external_localopt.py
 libensemble/tests/regression_tests/test_persistent_aposmm_nlopt.py
 libensemble/tests/regression_tests/test_persistent_aposmm_periodic.py
+libensemble/tests/regression_tests/test_persistent_aposmm_pounders.py
 libensemble/tests/regression_tests/test_persistent_aposmm_scipy.py
+libensemble/tests/regression_tests/test_persistent_aposmm_tao_blmvm.py
+libensemble/tests/regression_tests/test_persistent_aposmm_tao_nm.py
 libensemble/tests/regression_tests/test_persistent_aposmm_timeout.py
 libensemble/tests/regression_tests/test_persistent_aposmm_with_grad.py
 libensemble/tests/regression_tests/test_persistent_fd_param_finder.py
+libensemble/tests/regression_tests/test_persistent_gp.py
 libensemble/tests/regression_tests/test_persistent_gp_multitask_ax.py
 libensemble/tests/regression_tests/test_persistent_independent.py
 libensemble/tests/regression_tests/test_persistent_n_agent.py
 libensemble/tests/regression_tests/test_persistent_pds.py
 libensemble/tests/regression_tests/test_persistent_prox_slide.py
-libensemble/tests/regression_tests/test_persistent_sampling_CUDA_variable_resources.py
-libensemble/tests/regression_tests/test_persistent_sim_uniform_sampling.py
 libensemble/tests/regression_tests/test_persistent_surmise_calib.py
 libensemble/tests/regression_tests/test_persistent_surmise_killsims.py
 libensemble/tests/regression_tests/test_persistent_tasmanian.py
 libensemble/tests/regression_tests/test_persistent_tasmanian_async.py
-libensemble/tests/regression_tests/test_persistent_uniform_gen_decides_stop.py
-libensemble/tests/regression_tests/test_persistent_uniform_sampling.py
-libensemble/tests/regression_tests/test_persistent_uniform_sampling_adv.py
-libensemble/tests/regression_tests/test_persistent_uniform_sampling_async.py
-libensemble/tests/regression_tests/test_persistent_uniform_sampling_nonblocking.py
-libensemble/tests/regression_tests/test_stats_output.py
-libensemble/tests/regression_tests/test_uniform_sampling.py
-libensemble/tests/regression_tests/test_uniform_sampling_cancel.py
-libensemble/tests/regression_tests/test_uniform_sampling_one_residual_at_a_time.py
-libensemble/tests/regression_tests/test_uniform_sampling_then_persistent_localopt_runs.py
-libensemble/tests/regression_tests/test_uniform_sampling_with_variable_resources.py
 libensemble/tests/regression_tests/scripts_used_by_reg_tests/ECnoise.m
 libensemble/tests/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m
 libensemble/tests/regression_tests/scripts_used_by_reg_tests/cleanup-balsam-test.sh
 libensemble/tests/regression_tests/scripts_used_by_reg_tests/configure-balsam-test.sh
 libensemble/tests/regression_tests/scripts_used_by_reg_tests/test_balsam_hworld.py
 libensemble/tests/regression_tests/scripts_used_by_reg_tests/wrapper_obj_fun.m
 libensemble/tests/scaling_tests/note_moved_examples.md
@@ -480,23 +453,50 @@
 libensemble/tests/scaling_tests/forces/forces_adv/forces_simf.py
 libensemble/tests/scaling_tests/forces/forces_adv/forces_support.py
 libensemble/tests/scaling_tests/forces/forces_adv/readme.md
 libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces.py
 libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces_from_yaml.py
 libensemble/tests/scaling_tests/forces/forces_app/build_forces.sh
 libensemble/tests/scaling_tests/forces/forces_app/forces.c
+libensemble/tests/scaling_tests/forces/forces_app/forces.x
 libensemble/tests/scaling_tests/forces/forces_app/readme.md
 libensemble/tests/scaling_tests/forces/forces_app/mini_forces/build_forces.sh
 libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces.c
 libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces_AoS.c
 libensemble/tests/scaling_tests/forces/forces_gpu/cleanup.sh
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble.log
 libensemble/tests/scaling_tests/forces/forces_gpu/forces_simf.py
+libensemble/tests/scaling_tests/forces/forces_gpu/libE_stats.txt
 libensemble/tests/scaling_tests/forces/forces_gpu/readme.md
 libensemble/tests/scaling_tests/forces/forces_gpu/run_libe_forces.py
 libensemble/tests/scaling_tests/forces/forces_gpu/submit_perlmutter.sh
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim0_worker1/forces.stat
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim0_worker1/libe_task_forces_worker1_0.err
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim0_worker1/libe_task_forces_worker1_0.out
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim1_worker2/forces.stat
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim1_worker2/libe_task_forces_worker2_0.err
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim1_worker2/libe_task_forces_worker2_0.out
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim2_worker3/forces.stat
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim2_worker3/libe_task_forces_worker3_0.err
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim2_worker3/libe_task_forces_worker3_0.out
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim3_worker4/forces.stat
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim3_worker4/libe_task_forces_worker4_0.err
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim3_worker4/libe_task_forces_worker4_0.out
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim4_worker3/forces.stat
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim4_worker3/libe_task_forces_worker3_1.err
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim4_worker3/libe_task_forces_worker3_1.out
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim5_worker1/forces.stat
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim5_worker1/libe_task_forces_worker1_1.err
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim5_worker1/libe_task_forces_worker1_1.out
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim6_worker3/forces.stat
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim6_worker3/libe_task_forces_worker3_2.err
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim6_worker3/libe_task_forces_worker3_2.out
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim7_worker1/forces.stat
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim7_worker1/libe_task_forces_worker1_2.err
+libensemble/tests/scaling_tests/forces/forces_gpu/ensemble/sim7_worker1/libe_task_forces_worker1_2.out
 libensemble/tests/scaling_tests/forces/forces_simple/cleanup.sh
 libensemble/tests/scaling_tests/forces/forces_simple/forces_simf.py
 libensemble/tests/scaling_tests/forces/forces_simple/readme.md
 libensemble/tests/scaling_tests/forces/forces_simple/run_libe_forces.py
 libensemble/tests/scaling_tests/forces/funcx_forces/cleanup.sh
 libensemble/tests/scaling_tests/forces/funcx_forces/forces_simf.py
 libensemble/tests/scaling_tests/forces/funcx_forces/funcx_forces.yaml
@@ -535,18 +535,20 @@
 libensemble/tests/unit_tests/launch_busy.py
 libensemble/tests/unit_tests/mpich-only_test_api.py
 libensemble/tests/unit_tests/setup.py
 libensemble/tests/unit_tests/test_allocation_funcs_and_support.py
 libensemble/tests/unit_tests/test_comms.py
 libensemble/tests/unit_tests/test_env_resources.py
 libensemble/tests/unit_tests/test_executor.py
+libensemble/tests/unit_tests/test_executor_balsam.py
 libensemble/tests/unit_tests/test_history.py
 libensemble/tests/unit_tests/test_launcher.py
 libensemble/tests/unit_tests/test_libE_main.py
 libensemble/tests/unit_tests/test_loc_stack.py
+libensemble/tests/unit_tests/test_make_runners.py
 libensemble/tests/unit_tests/test_manager_main.py
 libensemble/tests/unit_tests/test_mpi4py.py
 libensemble/tests/unit_tests/test_node_resources.py
 libensemble/tests/unit_tests/test_persistent_aposmm.py
 libensemble/tests/unit_tests/test_resource_scheduler.py
 libensemble/tests/unit_tests/test_resources.py
 libensemble/tests/unit_tests/test_scipy.py
@@ -562,30 +564,35 @@
 libensemble/tests/unit_tests/simdir/py_startup.py
 libensemble/tests/unit_tests/simdir/test_example.yaml
 libensemble/tests/unit_tests/simdir/test_example_badfuncs_attribute.yaml
 libensemble/tests/unit_tests/simdir/test_example_badfuncs_notfound.yaml
 libensemble/tests/unit_tests_logger/.coveragerc
 libensemble/tests/unit_tests_logger/test_logger.py
 libensemble/tests/unit_tests_nompi/.coveragerc
+libensemble/tests/unit_tests_nompi/conftest.py
 libensemble/tests/unit_tests_nompi/test_aaa_comms.py
 libensemble/tools/__init__.py
 libensemble/tools/alloc_support.py
 libensemble/tools/check_inputs.py
 libensemble/tools/consensus_subroutines.py
 libensemble/tools/fields_keys.py
 libensemble/tools/forkable_pdb.py
 libensemble/tools/parse_args.py
 libensemble/tools/persistent_support.py
 libensemble/tools/tools.py
 libensemble/utils/__init__.py
 libensemble/utils/launcher.py
 libensemble/utils/loc_stack.py
+libensemble/utils/misc.py
+libensemble/utils/runners.py
 libensemble/utils/timer.py
 scripts/__init__.py
 scripts/compare_npy.py
+scripts/liberegister
+scripts/libesubmit
 scripts/plot_contours_and_history_points.py
 scripts/plot_libe_calcs_util_v_time.py
 scripts/plot_libe_histogram.py
 scripts/plot_libe_tasks_util_v_time.py
 scripts/plot_pareto_2d.py
 scripts/plot_pareto_3d.py
 scripts/print_fields.py
```

### Comparing `libensemble-0.9.2/scripts/balsam/plot_tasks_v_time.py` & `libensemble-0.9.3/scripts/balsam/plot_tasks_v_time.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/balsam/plot_util_v_time.py` & `libensemble-0.9.3/scripts/balsam/plot_util_v_time.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/balsam/plot_waiting_v_time.py` & `libensemble-0.9.3/scripts/balsam/plot_waiting_v_time.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/compare_npy.py` & `libensemble-0.9.3/scripts/compare_npy.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     sys.exit()
 
 compare_fields = tuple(filter(lambda x: x not in exclude_fields, exp_results.dtype.names))
 match = all(
     [np.allclose(exp_results[name], results[name], rtol=rtol, atol=atol, equal_nan=True) for name in compare_fields]
 )
 
-print("Compare results: {}\n".format(match))
+print(f"Compare results: {match}\n")
 
 if not locate_mismatch:
     assert match, "Error: Results do NOT match"
 
 if not match:
     for name in compare_fields:
         for i in range(len(results)):
```

### Comparing `libensemble-0.9.2/scripts/plot_contours_and_history_points.py` & `libensemble-0.9.3/scripts/plot_contours_and_history_points.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/plot_libe_calcs_util_v_time.py` & `libensemble-0.9.3/scripts/plot_libe_calcs_util_v_time.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/plot_libe_histogram.py` & `libensemble-0.9.3/scripts/plot_libe_histogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,22 +77,22 @@
                     append_to_list(in_times_ran, in_times, found_time)  # Assumes Time comes first
                 elif search_for_keyword(lst[i + 1 : len(lst)], run_killed):
                     append_to_list(in_times_kill, in_times, found_time)  # Assumes Time comes first
                 elif search_for_keyword(lst[i + 1 : len(lst)], run_exception):
                     exceptions = True
                     append_to_list(in_times_exception, in_times, found_time)  # Assumes Time comes first
                 else:
-                    print("Error: Unknown status - rest of line: {}".format(lst[i + 1 : len(lst)]))
+                    print(f"Error: Unknown status - rest of line: {lst[i + 1:len(lst)]}")
                     sys.exit()
                 found_status = True
             if found_time and found_status:
                 active_line_count += 1
                 break
 
-print("Processed {} calcs".format(active_line_count))
+print(f"Processed {active_line_count} calcs")
 
 times = np.asarray(in_times, dtype=float)
 times_ran = np.asarray(in_times_ran, dtype=float)
 times_kill = np.asarray(in_times_kill, dtype=float)
 times_exc = np.asarray(in_times_exception, dtype=float)
 
 num_bins = min(active_line_count, max_bins)
```

### Comparing `libensemble-0.9.2/scripts/plot_libe_tasks_util_v_time.py` & `libensemble-0.9.3/scripts/plot_libe_tasks_util_v_time.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/plot_pareto_2d.py` & `libensemble-0.9.3/scripts/plot_pareto_2d.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/plot_pareto_3d.py` & `libensemble-0.9.3/scripts/plot_pareto_3d.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/print_fields.py` & `libensemble-0.9.3/scripts/print_fields.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/print_npy.py` & `libensemble-0.9.3/scripts/print_npy.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/process_history_to_make_chart.py` & `libensemble-0.9.3/scripts/process_history_to_make_chart.py`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/scripts/readme.rst` & `libensemble-0.9.3/scripts/readme.rst`

 * *Files identical despite different names*

### Comparing `libensemble-0.9.2/setup.py` & `libensemble-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,31 +78,36 @@
         "pytest-cov>=2.5",
         "pytest-pep8>=1.0",
         "pytest-timeout",
         "mock",
     ],
     extras_require={
         "extras": [
-            "pyyaml",
-            "scipy",
-            "nlopt",
+            "ax-platform",
+            "DFO-LS",
+            "dragonfly-opt",
+            "funcx",
             "mpi4py",
+            "mpmath",
+            "nlopt",
             "petsc",
             "petsc4py",
-            "DFO-LS",
-            "mpmath",
-            "dragonfly-opt",
-            "ax-platform",
+            "pyyaml",
+            "scipy",
         ],
         "docs": [
             "sphinx",
             "sphinxcontrib.bibtex",
             "sphinx_rtd_theme",
         ],
     },
+    scripts=[
+        "scripts/liberegister",
+        "scripts/libesubmit",
+    ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
```

