# Comparing `tmp/Brian2Cuda-1.0a2.tar.gz` & `tmp/Brian2Cuda-1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Brian2Cuda-1.0a2.tar", last modified: Sun Jul  9 11:51:08 2023, max compression
+gzip compressed data, was "Brian2Cuda-1.0a3.tar", last modified: Tue Jul 11 10:13:02 2023, max compression
```

## Comparing `Brian2Cuda-1.0a2.tar` & `Brian2Cuda-1.0a3.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.946671 Brian2Cuda-1.0a2/
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.922670 Brian2Cuda-1.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.926670 Brian2Cuda-1.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)      763 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.926670 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4520 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (122)    35130 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-07-09 11:51:08.946671 Brian2Cuda-1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.930670 Brian2Cuda-1.0a2/brian2cuda/
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/brian2cuda/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4192 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/binomial.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.930670 Brian2Cuda-1.0a2/brian2cuda/brianlib/
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/clocks.h
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/common_math.h
--rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/cudaVector.h
--rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/cuda_utils.h
--rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/curand_buffer.h
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/dynamic_array.h
--rw-r--r--   0 runner    (1001) docker     (122)    22818 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/spikequeue.h
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/stdint_compat.h
--rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/codeobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    45760 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/cuda_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11671 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/cuda_prefs.py
--rw-r--r--   0 runner    (1001) docker     (122)   105791 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/device.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.930670 Brian2Cuda-1.0a2/brian2cuda/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9577 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/briandoc.py
--rw-r--r--   0 runner    (1001) docker     (122)    15909 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/docscrape.py
--rw-r--r--   0 runner    (1001) docker     (122)     8470 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/docscrape_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/examplefinder.py
--rw-r--r--   0 runner    (1001) docker     (122)     7704 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/generate_examples.py
--rw-r--r--   0 runner    (1001) docker     (122)     9655 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/generate_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.934671 Brian2Cuda-1.0a2/brian2cuda/templates/
--rw-r--r--   0 runner    (1001) docker     (122)    11160 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/common_group.cu
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/common_synapses.cu
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/group_variable_set.cu
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/group_variable_set_conditional.cu
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/main.cu
--rw-r--r--   0 runner    (1001) docker     (122)      553 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/makefile
--rw-r--r--   0 runner    (1001) docker     (122)     5179 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/network.cu
--rw-r--r--   0 runner    (1001) docker     (122)    27500 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/objects.cu
--rw-r--r--   0 runner    (1001) docker     (122)    21643 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/rand.cu
--rw-r--r--   0 runner    (1001) docker     (122)     3240 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/ratemonitor.cu
--rw-r--r--   0 runner    (1001) docker     (122)      718 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/reset.cu
--rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/run.cu
--rw-r--r--   0 runner    (1001) docker     (122)    19800 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/spatialstateupdate.cu
--rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/spikegenerator.cu
--rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/spikemonitor.cu
--rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/statemonitor.cu
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/stateupdate.cu
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/summed_variable.cu
--rw-r--r--   0 runner    (1001) docker     (122)    12745 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/synapses.cu
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/synapses_classes.cu
--rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/synapses_create_array.cu
--rw-r--r--   0 runner    (1001) docker     (122)    18225 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/synapses_create_generator.cu
--rw-r--r--   0 runner    (1001) docker     (122)    47020 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/synapses_push_spikes.cu
--rw-r--r--   0 runner    (1001) docker     (122)     4272 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/threshold.cu
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/win_makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.938671 Brian2Cuda-1.0a2/brian2cuda/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      637 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.938671 Brian2Cuda-1.0a2/brian2cuda/tests/features/
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19764 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/features/cuda_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    33044 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/features/speed.py
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/func_def_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/func_def_cuda.h
--rw-r--r--   0 runner    (1001) docker     (122)     7021 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_cpp_cuda_consistency.py
--rw-r--r--   0 runner    (1001) docker     (122)    10456 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_cuda_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)    14513 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_cuda_standalone.py
--rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6378 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_gpu_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5420 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_network_multiple_runs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2733 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_neurongroup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (122)    47363 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_random_number_generation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_spikegenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     9678 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_stateupdaters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3455 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_stringtools.py
--rw-r--r--   0 runner    (1001) docker     (122)    15757 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_synaptic_propagations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/timedarray.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.938671 Brian2Cuda-1.0a2/brian2cuda/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21225 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/utils/gputools.py
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     4201 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/utils/stringtools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.938671 Brian2Cuda-1.0a2/docs_sphinx/
--rw-r--r--   0 runner    (1001) docker     (122)      580 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)    11360 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.938671 Brian2Cuda-1.0a2/docs_sphinx/introduction/
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/cuda_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4468 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/install.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/performance.rst
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/preferences.rst
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.942671 Brian2Cuda-1.0a2/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/TODO.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7242 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/brunelhakim.py
--rw-r--r--   0 runner    (1001) docker     (122)     7993 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/cobahh.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.942671 Brian2Cuda-1.0a2/examples/compartmental/
--rw-r--r--   0 runner    (1001) docker     (122)     1976 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_cell_cpp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_cell_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs2_cpp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs2_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs_cpp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     3107 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/hh_with_spikes_cpp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/hh_with_spikes_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/hodgkin_huxley_1952_cpp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/hodgkin_huxley_1952_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     3384 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/lfp_cpp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3428 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/lfp_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.942671 Brian2Cuda-1.0a2/examples/compartmental/plots/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/plots/all_plots_combined.sh
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/plots/hh_with_spikes_checkresults.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/rall_cpp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/rall_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/spike_initiation_cpp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/spike_initiation_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/cuba.py
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/figures.mplstyle
--rw-r--r--   0 runner    (1001) docker     (122)    10691 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/mushroombody.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/run_examples.sh
--rw-r--r--   0 runner    (1001) docker     (122)     8794 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/stdp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5443 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.942671 Brian2Cuda-1.0a2/frozen_repos/
--rw-r--r--   0 runner    (1001) docker     (122)    21214 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/brian2.diff
--rw-r--r--   0 runner    (1001) docker     (122)     4490 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/brian2genn.diff
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/init_genn.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/submodules_update.sh
--rw-r--r--   0 runner    (1001) docker     (122)      443 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/update_brian2.sh
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/update_brian2genn.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-09 11:51:08.946671 Brian2Cuda-1.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:02.001227 Brian2Cuda-1.0a3/
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.961225 Brian2Cuda-1.0a3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.965225 Brian2Cuda-1.0a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      763 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.969226 Brian2Cuda-1.0a3/Brian2Cuda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-07-11 10:13:01.000000 Brian2Cuda-1.0a3/Brian2Cuda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4510 2023-07-11 10:13:01.000000 Brian2Cuda-1.0a3/Brian2Cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 10:13:01.000000 Brian2Cuda-1.0a3/Brian2Cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-07-11 10:13:01.000000 Brian2Cuda-1.0a3/Brian2Cuda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-11 10:13:01.000000 Brian2Cuda-1.0a3/Brian2Cuda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (122)    35130 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-07-11 10:13:02.001227 Brian2Cuda-1.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.973226 Brian2Cuda-1.0a3/brian2cuda/
+-rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-11 10:13:01.000000 Brian2Cuda-1.0a3/brian2cuda/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4192 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/binomial.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.977226 Brian2Cuda-1.0a3/brian2cuda/brianlib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/brianlib/clocks.h
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/brianlib/common_math.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/brianlib/cudaVector.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/brianlib/cuda_utils.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/brianlib/curand_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/brianlib/dynamic_array.h
+-rw-r--r--   0 runner    (1001) docker     (122)    22818 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/brianlib/spikequeue.h
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/brianlib/stdint_compat.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/codeobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46039 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/cuda_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11671 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/cuda_prefs.py
+-rw-r--r--   0 runner    (1001) docker     (122)   105791 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/device.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.977226 Brian2Cuda-1.0a3/brian2cuda/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9577 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/sphinxext/briandoc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15909 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/sphinxext/docscrape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8470 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/sphinxext/docscrape_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/sphinxext/examplefinder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7704 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/sphinxext/generate_examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9655 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/sphinxext/generate_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.989227 Brian2Cuda-1.0a3/brian2cuda/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)    11220 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/common_group.cu
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/common_synapses.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/group_variable_set.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/group_variable_set_conditional.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/main.cu
+-rw-r--r--   0 runner    (1001) docker     (122)      553 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     5179 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/network.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    27500 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/objects.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    21643 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/rand.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     3240 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/ratemonitor.cu
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/reset.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/run.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    19916 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/spatialstateupdate.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/spikegenerator.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     6913 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/spikemonitor.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/statemonitor.cu
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/stateupdate.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/summed_variable.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    12745 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/synapses.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/synapses_classes.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/synapses_create_array.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    18225 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/synapses_create_generator.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    47020 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/synapses_push_spikes.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     4272 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/threshold.cu
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/templates/win_makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.993227 Brian2Cuda-1.0a3/brian2cuda/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.993227 Brian2Cuda-1.0a3/brian2cuda/tests/features/
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19764 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/features/cuda_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33044 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/features/speed.py
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/func_def_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/func_def_cuda.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7001 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_cpp_cuda_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10456 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_cuda_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14513 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_cuda_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6378 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_gpu_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5420 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_network_multiple_runs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2737 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_neurongroup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47363 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_random_number_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_spikegenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9678 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_stateupdaters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3455 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_stringtools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15757 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/tests/test_synaptic_propagations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/timedarray.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.997227 Brian2Cuda-1.0a3/brian2cuda/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21208 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/utils/gputools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4201 2023-07-11 10:12:46.000000 Brian2Cuda-1.0a3/brian2cuda/utils/stringtools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.997227 Brian2Cuda-1.0a3/docs_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (122)      580 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/docs_sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    11360 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/docs_sphinx/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/docs_sphinx/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.997227 Brian2Cuda-1.0a3/docs_sphinx/introduction/
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/docs_sphinx/introduction/cuda_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/docs_sphinx/introduction/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4468 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/docs_sphinx/introduction/install.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/docs_sphinx/introduction/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/docs_sphinx/introduction/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/docs_sphinx/introduction/preferences.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/docs_sphinx/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:01.997227 Brian2Cuda-1.0a3/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/TODO.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7242 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/brunelhakim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7993 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/cobahh.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:02.001227 Brian2Cuda-1.0a3/examples/compartmental/
+-rw-r--r--   0 runner    (1001) docker     (122)     1976 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/bipolar_cell_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/bipolar_cell_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/bipolar_with_inputs2_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/bipolar_with_inputs2_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/bipolar_with_inputs_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/bipolar_with_inputs_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3107 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/hh_with_spikes_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/hh_with_spikes_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/hodgkin_huxley_1952_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/hodgkin_huxley_1952_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3384 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/lfp_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3428 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/lfp_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:02.001227 Brian2Cuda-1.0a3/examples/compartmental/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/plots/all_plots_combined.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/plots/hh_with_spikes_checkresults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/rall_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/rall_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/spike_initiation_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/compartmental/spike_initiation_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/cuba.py
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/figures.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (122)    10691 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/mushroombody.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/run_examples.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     8794 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/stdp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5443 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 10:13:02.001227 Brian2Cuda-1.0a3/frozen_repos/
+-rw-r--r--   0 runner    (1001) docker     (122)    26525 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/frozen_repos/brian2.diff
+-rw-r--r--   0 runner    (1001) docker     (122)     4490 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/frozen_repos/brian2genn.diff
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/frozen_repos/init_genn.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/frozen_repos/submodules_update.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/frozen_repos/update_brian2.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/frozen_repos/update_brian2genn.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-11 10:12:47.000000 Brian2Cuda-1.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 10:13:02.001227 Brian2Cuda-1.0a3/setup.cfg
```

### Comparing `Brian2Cuda-1.0a2/.github/workflows/publish_to_pypi.yml` & `Brian2Cuda-1.0a3/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/.gitignore` & `Brian2Cuda-1.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/Brian2Cuda.egg-info/PKG-INFO` & `Brian2Cuda-1.0a3/Brian2Cuda.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Brian2Cuda
-Version: 1.0a2
+Version: 1.0a3
 Summary: A Brian2 extension to simulate spiking neural networks on GPUs
 Author: Denis Alevi, Moritz Augustin, Marcel Stimberg
 Project-URL: Documentation, https://brian2cuda.readthedocs.io/
 Project-URL: Source, https://github.com/brian-team/brian2cuda
 Project-URL: Tracker, https://github.com/brian-team/brian2cuda/issues
 Keywords: computational neuroscience,simulation,neural networks,spiking neurons,gpu,cuda
 Classifier: Development Status :: 3 - Alpha
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 Brian2CUDA
 ==========
@@ -68,7 +68,12 @@
 If you use this software in a published article, please cite
 [our Brian2CUDA publication](https://www.frontiersin.org/articles/10.3389/fninf.2022.883700):
 
 > Alevi, D, Stimberg, M, Sprekeler, H, Obermayer, K, Augustin, M. “Brian2CUDA: flexible and efficient simulation of spiking neural network models on GPUs” Frontiers in Neuroinformatics (2022). doi: 10.3389/fninf.2022.883700.
 
 ## License
 Brian2CUDA is free software licensed under the [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).
+
+## Testing
+To run the test suite on Google Collab (no installation or GPU required), click on the badge below:
+
+[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/brian-team/brian2cuda/blob/master/brian2cuda/tools/test_suite/run_tests.ipynb)
```

### Comparing `Brian2Cuda-1.0a2/Brian2Cuda.egg-info/SOURCES.txt` & `Brian2Cuda-1.0a3/Brian2Cuda.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 .gitmodules
 .readthedocs.yml
 CITATION.cff
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 .github/workflows/publish_to_pypi.yml
 Brian2Cuda.egg-info/PKG-INFO
 Brian2Cuda.egg-info/SOURCES.txt
 Brian2Cuda.egg-info/dependency_links.txt
 Brian2Cuda.egg-info/requires.txt
 Brian2Cuda.egg-info/top_level.txt
 brian2cuda/__init__.py
```

### Comparing `Brian2Cuda-1.0a2/CITATION.cff` & `Brian2Cuda-1.0a3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/LICENSE` & `Brian2Cuda-1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/PKG-INFO` & `Brian2Cuda-1.0a3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Brian2Cuda
-Version: 1.0a2
+Version: 1.0a3
 Summary: A Brian2 extension to simulate spiking neural networks on GPUs
 Author: Denis Alevi, Moritz Augustin, Marcel Stimberg
 Project-URL: Documentation, https://brian2cuda.readthedocs.io/
 Project-URL: Source, https://github.com/brian-team/brian2cuda
 Project-URL: Tracker, https://github.com/brian-team/brian2cuda/issues
 Keywords: computational neuroscience,simulation,neural networks,spiking neurons,gpu,cuda
 Classifier: Development Status :: 3 - Alpha
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 Brian2CUDA
 ==========
@@ -68,7 +68,12 @@
 If you use this software in a published article, please cite
 [our Brian2CUDA publication](https://www.frontiersin.org/articles/10.3389/fninf.2022.883700):
 
 > Alevi, D, Stimberg, M, Sprekeler, H, Obermayer, K, Augustin, M. “Brian2CUDA: flexible and efficient simulation of spiking neural network models on GPUs” Frontiers in Neuroinformatics (2022). doi: 10.3389/fninf.2022.883700.
 
 ## License
 Brian2CUDA is free software licensed under the [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).
+
+## Testing
+To run the test suite on Google Collab (no installation or GPU required), click on the badge below:
+
+[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/brian-team/brian2cuda/blob/master/brian2cuda/tools/test_suite/run_tests.ipynb)
```

### Comparing `Brian2Cuda-1.0a2/README.md` & `Brian2Cuda-1.0a3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -44,7 +44,12 @@
 If you use this software in a published article, please cite
 [our Brian2CUDA publication](https://www.frontiersin.org/articles/10.3389/fninf.2022.883700):
 
 > Alevi, D, Stimberg, M, Sprekeler, H, Obermayer, K, Augustin, M. “Brian2CUDA: flexible and efficient simulation of spiking neural network models on GPUs” Frontiers in Neuroinformatics (2022). doi: 10.3389/fninf.2022.883700.
 
 ## License
 Brian2CUDA is free software licensed under the [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).
+
+## Testing
+To run the test suite on Google Collab (no installation or GPU required), click on the badge below:
+
+[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/brian-team/brian2cuda/blob/master/brian2cuda/tools/test_suite/run_tests.ipynb)
```

### Comparing `Brian2Cuda-1.0a2/brian2cuda/__init__.py` & `Brian2Cuda-1.0a3/brian2cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/binomial.py` & `Brian2Cuda-1.0a3/brian2cuda/binomial.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/brianlib/clocks.h` & `Brian2Cuda-1.0a3/brian2cuda/brianlib/clocks.h`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/brianlib/cudaVector.h` & `Brian2Cuda-1.0a3/brian2cuda/brianlib/cudaVector.h`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/brianlib/cuda_utils.h` & `Brian2Cuda-1.0a3/brian2cuda/brianlib/cuda_utils.h`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/brianlib/curand_buffer.h` & `Brian2Cuda-1.0a3/brian2cuda/brianlib/curand_buffer.h`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/brianlib/dynamic_array.h` & `Brian2Cuda-1.0a3/brian2cuda/brianlib/dynamic_array.h`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/brianlib/spikequeue.h` & `Brian2Cuda-1.0a3/brian2cuda/brianlib/spikequeue.h`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/codeobject.py` & `Brian2Cuda-1.0a3/brian2cuda/codeobject.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/cuda_generator.py` & `Brian2Cuda-1.0a3/brian2cuda/cuda_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -700,16 +700,19 @@
                 user_functions,
                 dep_kernel_lines + kernel_lines)
 
     def determine_keywords(self):
         # set up the restricted pointers, these are used so that the compiler
         # knows there is no aliasing in the pointers, for optimisation
         pointers = []
-        # Add additional lines inside the kernel functions
+        # Add additional lines inside the kernel functions, also contains the clock_pointers
+        # lines from below for backwards compatibility
         kernel_lines = []
+        # Translate clock variables back into pointers
+        clock_pointers = []
         # It is possible that several different variable names refer to the
         # same array. E.g. in gapjunction code, v_pre and v_post refer to the
         # same array if a group is connected to itself
         handled_pointers = set()
         template_kwds = {}
         # Again, do the import here to avoid a circular dependency.
         from brian2.devices.device import get_device
@@ -779,24 +782,25 @@
                 arrayname = self.get_array_name(variable, prefix='')
                 # kernel_lines appear before dt is cast to float (in scalar_code), hence
                 # we need to still use double (used in kernel parameters), see #148
                 if varname == "dt" and prefs.core.default_float_dtype == np.float32:
                     # c_data_type(variable.dtype) is float, but we need double
                     dtype = "double"
                 else:
-                    dtype = dtype=c_data_type(variable.dtype)
+                    dtype = c_data_type(variable.dtype)
                 line = f"const {dtype}* _ptr{arrayname} = &_value{arrayname};"
-                if line not in kernel_lines:
-                    kernel_lines.append(line)
+                if line not in clock_pointers:
+                    clock_pointers.append(line)
 
         keywords = {'pointers_lines': stripped_deindented_lines('\n'.join(pointers)),
                     'support_code_lines': stripped_deindented_lines('\n'.join(support_code)),
                     'hashdefine_lines': stripped_deindented_lines('\n'.join(hash_defines)),
                     'denormals_code_lines': stripped_deindented_lines('\n'.join(self.denormals_to_zero_code())),
-                    'kernel_lines': stripped_deindented_lines('\n'.join(kernel_lines)),
+                    'kernel_lines': stripped_deindented_lines('\n'.join(kernel_lines + clock_pointers)),
+                    'clock_pointers': stripped_deindented_lines('\n'.join(clock_pointers)),
                     'uses_atomics': self.uses_atomics
                     }
         keywords.update(template_kwds)
         return keywords
 
 
 class CUDAAtomicsCodeGenerator(CUDACodeGenerator):
```

### Comparing `Brian2Cuda-1.0a2/brian2cuda/cuda_prefs.py` & `Brian2Cuda-1.0a3/brian2cuda/cuda_prefs.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/device.py` & `Brian2Cuda-1.0a3/brian2cuda/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         # TODO: Add to brian2 and remove here
         self.code_lines.update({'before_network_run': [],
                                 'after_network_run': []})
         ### Attributes specific to CUDAStandaloneDevice:
         # only true during first run call (relevant for synaptic pre/post ID deletion)
         self.first_run = True
         # the minimal supported GPU compute capability
-        self.minimal_compute_capability = 3.5
+        self.minimal_compute_capability = 5.0
         # store the ID of the used GPU and it's compute capability
         self.gpu_id = None
         self.compute_capability = None
         # list of pre/post ID and delay arrays that are not needed in device memory
         self.delete_synaptic_pre = {}
         self.delete_synaptic_post = {}
         self.delete_synaptic_delay = {}
```

### Comparing `Brian2Cuda-1.0a2/brian2cuda/sphinxext/briandoc.py` & `Brian2Cuda-1.0a3/brian2cuda/sphinxext/briandoc.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/sphinxext/docscrape.py` & `Brian2Cuda-1.0a3/brian2cuda/sphinxext/docscrape.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/sphinxext/docscrape_sphinx.py` & `Brian2Cuda-1.0a3/brian2cuda/sphinxext/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/sphinxext/examplefinder.py` & `Brian2Cuda-1.0a3/brian2cuda/sphinxext/examplefinder.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/sphinxext/generate_examples.py` & `Brian2Cuda-1.0a3/brian2cuda/sphinxext/generate_examples.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/sphinxext/generate_reference.py` & `Brian2Cuda-1.0a3/brian2cuda/sphinxext/generate_reference.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/common_group.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/common_group.cu`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 #include <ctime>
 #include <stdio.h>
 {% endblock before_run_headers %}
 
 {% block before_run_defines %}
 {% endblock %}
 
+///// Support code /////
+{{support_code_lines|autoindent}}
+
 void _before_run_{{codeobj_name}}()
 {
     using namespace brian;
 
     {% block before_run_host_maincode %}
     // EMPTY_CODE_BLOCK  -- will be overwritten in child templates
     {% endblock %}
```

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/group_variable_set.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/group_variable_set.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/group_variable_set_conditional.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/group_variable_set_conditional.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/main.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/main.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/makefile` & `Brian2Cuda-1.0a3/brian2cuda/templates/makefile`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/network.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/network.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/objects.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/objects.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/rand.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/rand.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/ratemonitor.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/ratemonitor.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/reset.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/reset.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/run.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/run.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/spatialstateupdate.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/spatialstateupdate.cu`

 * *Files 3% similar despite different names*

```diff
@@ -136,16 +136,16 @@
     int tid = threadIdx.x;
     int bid = blockIdx.x;
     int _idx = bid * blockDim.x + tid;
 
     ///// KERNEL_CONSTANTS /////
     %KERNEL_CONSTANTS%
 
-    ///// kernel_lines /////
-    {{kernel_lines|autoindent}}
+    ///// translate clock variables into pointers /////
+    {{clock_pointers|autoindent}}
 
     // we need to run the kernel with 1 thread per block (to be changed by optimization)
     assert(tid == 0 && bid == _idx);
 
     // each thread processes the tridiagsystem of one branch
     const int _i = _idx;
 
@@ -210,16 +210,16 @@
     int tid = threadIdx.x;
     int bid = blockIdx.x;
     int _idx = bid * blockDim.x + tid;
 
     ///// KERNEL_CONSTANTS /////
     %KERNEL_CONSTANTS%
 
-    ///// kernel_lines /////
-    {{kernel_lines|autoindent}}
+    ///// translate clock variables into pointers /////
+    {{clock_pointers|autoindent}}
 
     // we need to run the kernel with 1 thread, 1 block
     assert(_idx == 0);
 
     // below all the code is simply copied from spatialstateupdate.cpp
 
         // indexing for _P_children which contains the elements above the diagonal of the coupling matrix _P
@@ -324,16 +324,16 @@
     int tid = threadIdx.x;
     int bid = blockIdx.x;
     int _idx = bid * blockDim.x + tid;
 
     ///// KERNEL_CONSTANTS /////
     %KERNEL_CONSTANTS%
 
-    ///// kernel_lines /////
-    {{kernel_lines|autoindent}}
+    ///// translate clock variables into pointers /////
+    {{clock_pointers|autoindent}}
 
     // we need to run the kernel with 1 thread per block (to be changed by optimization)
     assert(tid == 0 && bid == _idx);
 
     // each thread combines the tridiagsystem of one branch
     const int _i = _idx;
 
@@ -367,16 +367,16 @@
     int tid = threadIdx.x;
     int bid = blockIdx.x;
     int _idx = bid * blockDim.x + tid;
 
     ///// KERNEL_CONSTANTS /////
     %KERNEL_CONSTANTS%
 
-    ///// kernel_lines /////
-    {{kernel_lines|autoindent}}
+    ///// translate clock variables into pointers /////
+    {{clock_pointers|autoindent}}
 
     if(_idx >= _N)
     {
         return;
     }
 
     // each thread processes the tridiagsystem of one branch
```

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/spikegenerator.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/spikegenerator.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/spikemonitor.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/spikemonitor.cu`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {# USES_VARIABLES { N, count, _source_start, _source_stop, _source_idx} #}
 {# WRITES_TO_READ_ONLY_VARIABLES { N, count } #}
 {% extends 'common_group.cu' %}
 
 
 {% block extra_headers %}
-// TODO: uncomment when thrust calls below are fixed
-//#include <thrust/count.h>
-//#include <thrust/execution_policy.h>
+#include <thrust/copy.h>
+#include <thrust/count.h>
+#include <thrust/execution_policy.h>
 {% endblock %}
 
 
 {% block extra_device_helper %}
 {% if owner.source.__class__.__name__ == 'Subgroup' %}
 struct is_in_subgroup
 {
```

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/statemonitor.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/statemonitor.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/summed_variable.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/summed_variable.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/synapses.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/synapses.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/synapses_classes.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/synapses_classes.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/synapses_create_array.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/synapses_create_array.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/synapses_create_generator.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/synapses_create_generator.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/synapses_push_spikes.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/synapses_push_spikes.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/templates/threshold.cu` & `Brian2Cuda-1.0a3/brian2cuda/templates/threshold.cu`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/__init__.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/conftest.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/features/cuda_configuration.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/features/cuda_configuration.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/features/speed.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/features/speed.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_cpp_cuda_consistency.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_cpp_cuda_consistency.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     taupre     = 20 * ms
     taupost    = taupre
     dApost     = -dApre * taupre / taupost * 1.05
     dApost    *=  0.1*gmax
     dApre     *=  0.1*gmax
 
     connectivity = numpy.random.randn(n_cells, n_cells)
-    sources = numpy.random.random_integers(0, n_cells-1, 10*n_cells)
+    sources = numpy.random.randint(0, n_cells, 10*n_cells)
     # Only use one spike per time step (to rule out that a single source neuron
     # has more than one spike in a time step)
     times = numpy.random.choice(numpy.arange(10*n_cells), 10*n_cells, replace=False)*ms
     v_init = Vr + numpy.random.rand(n_cells) * (Vt - Vr)
 
     eqs  = Equations('''
     dv/dt = (g-(v-El))/taum : volt
@@ -106,15 +106,15 @@
     taupre     = 20 * ms
     taupost    = taupre
     dApost     = -dApre * taupre / taupost * 1.05
     dApost    *=  0.1*gmax
     dApre     *=  0.1*gmax
 
     connectivity = numpy.random.randn(n_cells, n_cells)
-    sources = numpy.random.random_integers(0, n_cells-1, 10*n_cells)
+    sources = numpy.random.randint(0, n_cells, 10*n_cells)
     # Only use one spike per time step (to rule out that a single source neuron
     # has more than one spike in a time step)
     times = numpy.random.choice(numpy.arange(10*n_cells), 10*n_cells, replace=False)*ms
     v_init = Vr + numpy.random.rand(n_cells) * (Vt - Vr)
 
     eqs  = Equations('''
     dv/dt = (g-(v-El))/taum : volt
```

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_cuda_generator.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_cuda_generator.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_cuda_standalone.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_cuda_standalone.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_functions.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_gpu_detection.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_gpu_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     assert log[2].startswith("Couldn't find `nvcc` binary ")
 
 
 @pytest.mark.cuda_standalone
 @pytest.mark.standalone_only
 def test_manual_setting_compute_capability(reset_gpu_detection):
     set_device("cuda_standalone", directory=None)
-    compute_capability_pref = '3.5'
+    compute_capability_pref = '6.0'
     prefs.devices.cuda_standalone.cuda_backend.compute_capability = float(compute_capability_pref)
     with catch_logs(log_level=logging.INFO) as logs:
         run(0*ms)
     log_start = "Compiling device code for compute capability "
     log_start_num_chars = len(log_start)
     for log in logs:
         if log[2].startswith(log_start):
@@ -137,16 +137,16 @@
         run(0*ms)
 
 
 @pytest.mark.cuda_standalone
 @pytest.mark.standalone_only
 def test_warning_compute_capability_set_twice(reset_gpu_detection, use_default_prefs):
     set_device("cuda_standalone", directory=None)
-    prefs.devices.cuda_standalone.cuda_backend.compute_capability = 3.5
-    prefs.devices.cuda_standalone.cuda_backend.extra_compile_args_nvcc.append('-arch=sm_37')
+    prefs.devices.cuda_standalone.cuda_backend.compute_capability = 5.3
+    prefs.devices.cuda_standalone.cuda_backend.extra_compile_args_nvcc.append('-arch=sm_52')
     with catch_logs() as logs:
         run(0*ms)
 
     assert len(logs) == 1, logs
     log = logs[0]
     assert log[0] == "WARNING"
     assert log[1] == "brian2.devices.cuda_standalone"
```

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_monitor.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_network.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_network_multiple_runs.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_network_multiple_runs.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_neurongroup.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_neurongroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     G = NeuronGroup(11, '''a : integer
                            b : integer
                            x : 1
                            y : 1
                            fvalue : 1
                            ivalue : integer''',
                     dtype={'a': np.int32, 'b': np.int64,
-                           'x': np.float, 'y': np.double})
+                           'x': np.float32, 'y': np.float64})
     int_values = np.arange(-5, 6)
-    float_values = np.arange(-5.0, 6.0, dtype=np.double)
+    float_values = np.arange(-5.0, 6.0, dtype=np.float64)
     G.ivalue = int_values
     G.fvalue = float_values
     with catch_logs() as l:
         G.run_regularly('''
         a = ivalue//3
         b = ivalue//3
         x = fvalue//3
```

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_profiling.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_random_number_generation.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_random_number_generation.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_spikegenerator.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_spikegenerator.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_stateupdaters.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_stateupdaters.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_stringtools.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_stringtools.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/tests/test_synaptic_propagations.py` & `Brian2Cuda-1.0a3/brian2cuda/tests/test_synaptic_propagations.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/timedarray.py` & `Brian2Cuda-1.0a3/brian2cuda/timedarray.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/utils/gputools.py` & `Brian2Cuda-1.0a3/brian2cuda/utils/gputools.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 
 import os
 import subprocess
 import shutil
 import shlex
 import re
-import distutils
 
 from brian2.core.preferences import prefs, PreferenceError
 from brian2.codegen.cpp_prefs import get_compiler_and_args
 from brian2.utils.logger import get_logger
 from brian2cuda.utils.logger import report_issue_message
 
 logger = get_logger("brian2.devices.cuda_standalone")
```

### Comparing `Brian2Cuda-1.0a2/brian2cuda/utils/logger.py` & `Brian2Cuda-1.0a3/brian2cuda/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/brian2cuda/utils/stringtools.py` & `Brian2Cuda-1.0a3/brian2cuda/utils/stringtools.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/docs_sphinx/Makefile` & `Brian2Cuda-1.0a3/docs_sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/docs_sphinx/conf.py` & `Brian2Cuda-1.0a3/docs_sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/docs_sphinx/introduction/cuda_configuration.rst` & `Brian2Cuda-1.0a3/docs_sphinx/introduction/cuda_configuration.rst`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/docs_sphinx/introduction/index.rst` & `Brian2Cuda-1.0a3/docs_sphinx/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/docs_sphinx/introduction/install.rst` & `Brian2Cuda-1.0a3/docs_sphinx/introduction/install.rst`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/docs_sphinx/introduction/known_issues.rst` & `Brian2Cuda-1.0a3/docs_sphinx/introduction/known_issues.rst`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/docs_sphinx/introduction/preferences.rst` & `Brian2Cuda-1.0a3/docs_sphinx/introduction/preferences.rst`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/docs_sphinx/make.bat` & `Brian2Cuda-1.0a3/docs_sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/brunelhakim.py` & `Brian2Cuda-1.0a3/examples/brunelhakim.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/cobahh.py` & `Brian2Cuda-1.0a3/examples/cobahh.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/bipolar_cell_cpp.py` & `Brian2Cuda-1.0a3/examples/compartmental/bipolar_cell_cpp.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/bipolar_cell_cuda.py` & `Brian2Cuda-1.0a3/examples/compartmental/bipolar_cell_cuda.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs2_cpp.py` & `Brian2Cuda-1.0a3/examples/compartmental/bipolar_with_inputs2_cpp.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs2_cuda.py` & `Brian2Cuda-1.0a3/examples/compartmental/bipolar_with_inputs2_cuda.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs_cpp.py` & `Brian2Cuda-1.0a3/examples/compartmental/bipolar_with_inputs_cpp.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs_cuda.py` & `Brian2Cuda-1.0a3/examples/compartmental/bipolar_with_inputs_cuda.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/hh_with_spikes_cpp.py` & `Brian2Cuda-1.0a3/examples/compartmental/hh_with_spikes_cpp.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/hh_with_spikes_cuda.py` & `Brian2Cuda-1.0a3/examples/compartmental/hh_with_spikes_cuda.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/hodgkin_huxley_1952_cpp.py` & `Brian2Cuda-1.0a3/examples/compartmental/hodgkin_huxley_1952_cpp.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/hodgkin_huxley_1952_cuda.py` & `Brian2Cuda-1.0a3/examples/compartmental/hodgkin_huxley_1952_cuda.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/lfp_cpp.py` & `Brian2Cuda-1.0a3/examples/compartmental/lfp_cpp.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/lfp_cuda.py` & `Brian2Cuda-1.0a3/examples/compartmental/lfp_cuda.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/plots/hh_with_spikes_checkresults.py` & `Brian2Cuda-1.0a3/examples/compartmental/plots/hh_with_spikes_checkresults.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/rall_cpp.py` & `Brian2Cuda-1.0a3/examples/compartmental/rall_cpp.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/rall_cuda.py` & `Brian2Cuda-1.0a3/examples/compartmental/rall_cuda.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/spike_initiation_cpp.py` & `Brian2Cuda-1.0a3/examples/compartmental/spike_initiation_cpp.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/compartmental/spike_initiation_cuda.py` & `Brian2Cuda-1.0a3/examples/compartmental/spike_initiation_cuda.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/cuba.py` & `Brian2Cuda-1.0a3/examples/cuba.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/mushroombody.py` & `Brian2Cuda-1.0a3/examples/mushroombody.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/run_examples.sh` & `Brian2Cuda-1.0a3/examples/run_examples.sh`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/stdp.py` & `Brian2Cuda-1.0a3/examples/stdp.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/examples/utils.py` & `Brian2Cuda-1.0a3/examples/utils.py`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/frozen_repos/brian2genn.diff` & `Brian2Cuda-1.0a3/frozen_repos/brian2genn.diff`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/frozen_repos/submodules_update.sh` & `Brian2Cuda-1.0a3/frozen_repos/submodules_update.sh`

 * *Files identical despite different names*

### Comparing `Brian2Cuda-1.0a2/pyproject.toml` & `Brian2Cuda-1.0a3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "Brian2Cuda"
 authors = [
     {name = 'Denis Alevi'},
     {name = 'Moritz Augustin'},
     {name ='Marcel Stimberg'}
 ]
-requires-python = '>=3.7'
+requires-python = '>=3.9'
 dependencies = [
-    'brian2==2.5.1',
+    'brian2==2.5.4',
 ]
 dynamic = ["version", "readme"]
 description = 'A Brian2 extension to simulate spiking neural networks on GPUs'
 keywords = ['computational neuroscience', 'simulation', 'neural networks', 'spiking neurons', 'gpu', 'cuda']
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
```

