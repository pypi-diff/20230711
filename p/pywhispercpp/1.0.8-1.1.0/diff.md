# Comparing `tmp/pywhispercpp-1.0.8.tar.gz` & `tmp/pywhispercpp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywhispercpp-1.0.8.tar", last modified: Wed May  3 23:10:05 2023, max compression
+gzip compressed data, was "pywhispercpp-1.1.0.tar", last modified: Tue Jul 11 21:22:48 2023, max compression
```

## Comparing `pywhispercpp-1.0.8.tar` & `pywhispercpp-1.1.0.tar`

### file list

```diff
@@ -1,137 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.434759 pywhispercpp-1.0.8/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.426759 pywhispercpp-1.0.8/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.442759 pywhispercpp-1.0.8/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.442759 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.442759 pywhispercpp-1.0.8/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.442759 pywhispercpp-1.0.8/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.446759 pywhispercpp-1.0.8/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.450759 pywhispercpp-1.0.8/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.434759 pywhispercpp-1.0.8/pywhispercpp/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.434759 pywhispercpp-1.0.8/pywhispercpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/examples/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/examples/livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/examples/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/pywhispercpp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.450759 pywhispercpp-1.0.8/pywhispercpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 23:10:05.000000 pywhispercpp-1.0.8/pywhispercpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.450759 pywhispercpp-1.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)    26781 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/tests/test_c_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-03 23:09:49.000000 pywhispercpp-1.0.8/tests/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/bindings/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/bindings/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/bindings/javascript/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/cmake/BuildTypes.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/cmake/DefaultTargetOptions.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/cmake/GitVars.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/addon.node/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/addon.node/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/bench/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/bench.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/bench.wasm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/command/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/command/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/command.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/command.wasm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/main/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.454759 pywhispercpp-1.0.8/whisper.cpp/examples/stream/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/stream/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/whisper.cpp/examples/stream.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/stream.wasm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/whisper.cpp/examples/talk/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/talk/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/whisper.cpp/examples/talk.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/talk.wasm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/whisper.cpp/examples/whisper.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:10:05.458759 pywhispercpp-1.0.8/whisper.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-03 23:09:51.000000 pywhispercpp-1.0.8/whisper.cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.702112 pywhispercpp-1.1.0/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.698112 pywhispercpp-1.1.0/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.702112 pywhispercpp-1.1.0/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.702112 pywhispercpp-1.1.0/pywhispercpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pywhispercpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pywhispercpp/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pywhispercpp/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.702112 pywhispercpp-1.1.0/pywhispercpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pywhispercpp/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pywhispercpp/examples/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pywhispercpp/examples/livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pywhispercpp/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pywhispercpp/examples/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pywhispercpp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/pywhispercpp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/pywhispercpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-07-11 21:22:48.000000 pywhispercpp-1.1.0/pywhispercpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-11 21:22:48.000000 pywhispercpp-1.1.0/pywhispercpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:22:48.000000 pywhispercpp-1.1.0/pywhispercpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 21:22:48.000000 pywhispercpp-1.1.0/pywhispercpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:22:48.000000 pywhispercpp-1.1.0/pywhispercpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 21:22:48.000000 pywhispercpp-1.1.0/pywhispercpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 21:22:48.000000 pywhispercpp-1.1.0/pywhispercpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    26958 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/tests/test_c_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-11 21:22:36.000000 pywhispercpp-1.1.0/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/whisper.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/whisper.cpp/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/bindings/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.706112 pywhispercpp-1.1.0/whisper.cpp/bindings/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/bindings/javascript/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/cmake/BuildTypes.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/cmake/DefaultTargetOptions.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/cmake/GitVars.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/addon.node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/addon.node/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/bench/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/bench.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/bench.wasm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/command/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/command.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/command.wasm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/main/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/quantize/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/stream/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/stream.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/stream.wasm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/talk/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/talk/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/talk-llama/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/talk-llama/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/talk.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/talk.wasm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/examples/whisper.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:22:48.710112 pywhispercpp-1.1.0/whisper.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-11 21:22:38.000000 pywhispercpp-1.1.0/whisper.cpp/tests/CMakeLists.txt
```

### Comparing `pywhispercpp-1.0.8/CMakeLists.txt` & `pywhispercpp-1.1.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/LICENSE` & `pywhispercpp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/PKG-INFO` & `pywhispercpp-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywhispercpp
-Version: 1.0.8
+Version: 1.1.0
 Summary: Python bindings for whisper.cpp
 Author: abdeladim-s
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pywhispercpp/
 Project-URL: Source, https://github.com/abdeladim-s/pywhispercpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pywhispercpp/issues
 Requires-Python: >=3.8
```

### Comparing `pywhispercpp-1.0.8/README.md` & `pywhispercpp-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/CMakeLists.txt` & `pywhispercpp-1.1.0/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/LICENSE` & `pywhispercpp-1.1.0/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/attr.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/buffer_info.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/cast.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/chrono.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/complex.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/class.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/common.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/descr.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/init.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/internals.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/type_caster_base.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/detail/typeid.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/eigen.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/embed.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/eval.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/functional.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/gil.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/iostream.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/numpy.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/operators.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/options.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/pybind11.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/pytypes.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/stl/filesystem.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/stl.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/include/pybind11/stl_bind.h` & `pywhispercpp-1.1.0/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tests/CMakeLists.txt` & `pywhispercpp-1.1.0/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pywhispercpp-1.1.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tests/test_embed/CMakeLists.txt` & `pywhispercpp-1.1.0/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/FindCatch.cmake` & `pywhispercpp-1.1.0/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/FindEigen3.cmake` & `pywhispercpp-1.1.0/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/FindPythonLibsNew.cmake` & `pywhispercpp-1.1.0/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/check-style.sh` & `pywhispercpp-1.1.0/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/cmake_uninstall.cmake.in` & `pywhispercpp-1.1.0/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/libsize.py` & `pywhispercpp-1.1.0/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/make_changelog.py` & `pywhispercpp-1.1.0/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/pybind11Common.cmake` & `pywhispercpp-1.1.0/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/pybind11Config.cmake.in` & `pywhispercpp-1.1.0/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/pybind11NewTools.cmake` & `pywhispercpp-1.1.0/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/pybind11Tools.cmake` & `pywhispercpp-1.1.0/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/setup_global.py.in` & `pywhispercpp-1.1.0/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pybind11/tools/setup_main.py.in` & `pywhispercpp-1.1.0/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pyproject.toml` & `pywhispercpp-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pywhispercpp/_logger.py` & `pywhispercpp-1.1.0/pywhispercpp/_logger.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pywhispercpp/constants.py` & `pywhispercpp-1.1.0/pywhispercpp/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,20 @@
     },
     'audio_ctx': {
             'type': int,
             'description': "overwrite the audio context size (0 = use default)",
             'options': None,
             'default': 0
     },
+    'initial_prompt': {
+                'type': str,
+                'description': "Initial prompt, these are prepended to any existing text context from a previous call",
+                'options': None,
+                'default': None
+        },
     'prompt_tokens': {
             'type': Tuple,
             'description': "tokens to provide to the whisper decoder as initial prompt",
             'options': None,
             'default': None
     },
     'prompt_n_tokens': {
```

### Comparing `pywhispercpp-1.0.8/pywhispercpp/examples/assistant.py` & `pywhispercpp-1.1.0/pywhispercpp/examples/assistant.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pywhispercpp/examples/livestream.py` & `pywhispercpp-1.1.0/pywhispercpp/examples/livestream.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pywhispercpp/examples/main.py` & `pywhispercpp-1.1.0/pywhispercpp/examples/main.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pywhispercpp/examples/recording.py` & `pywhispercpp-1.1.0/pywhispercpp/examples/recording.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pywhispercpp/model.py` & `pywhispercpp-1.1.0/pywhispercpp/model.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pywhispercpp/utils.py` & `pywhispercpp-1.1.0/pywhispercpp/utils.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/pywhispercpp.egg-info/PKG-INFO` & `pywhispercpp-1.1.0/pywhispercpp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywhispercpp
-Version: 1.0.8
+Version: 1.1.0
 Summary: Python bindings for whisper.cpp
 Author: abdeladim-s
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pywhispercpp/
 Project-URL: Source, https://github.com/abdeladim-s/pywhispercpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pywhispercpp/issues
 Requires-Python: >=3.8
```

### Comparing `pywhispercpp-1.0.8/pywhispercpp.egg-info/SOURCES.txt` & `pywhispercpp-1.1.0/pywhispercpp.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -85,13 +85,15 @@
 whisper.cpp/examples/CMakeLists.txt
 whisper.cpp/examples/addon.node/CMakeLists.txt
 whisper.cpp/examples/bench/CMakeLists.txt
 whisper.cpp/examples/bench.wasm/CMakeLists.txt
 whisper.cpp/examples/command/CMakeLists.txt
 whisper.cpp/examples/command.wasm/CMakeLists.txt
 whisper.cpp/examples/main/CMakeLists.txt
+whisper.cpp/examples/quantize/CMakeLists.txt
 whisper.cpp/examples/stream/CMakeLists.txt
 whisper.cpp/examples/stream.wasm/CMakeLists.txt
 whisper.cpp/examples/talk/CMakeLists.txt
+whisper.cpp/examples/talk-llama/CMakeLists.txt
 whisper.cpp/examples/talk.wasm/CMakeLists.txt
 whisper.cpp/examples/whisper.wasm/CMakeLists.txt
 whisper.cpp/tests/CMakeLists.txt
```

### Comparing `pywhispercpp-1.0.8/setup.py` & `pywhispercpp-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pywhispercpp",
-    version="1.0.8",
+    version="1.1.0",
     author="abdeladim-s",
     description="Python bindings for whisper.cpp",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pywhispercpp")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
```

### Comparing `pywhispercpp-1.0.8/src/main.cpp` & `pywhispercpp-1.1.0/src/main.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -276,28 +276,28 @@
     return whisper_full_get_token_p(ctx->ptr, i_segment, i_token);
 }
 
 
 
 // callbacks mechanism
 
-void _new_segment_callback(struct whisper_context * ctx, int n_new, void * user_data){
+void _new_segment_callback(struct whisper_context * ctx, struct whisper_state * state, int n_new, void * user_data){
     struct whisper_context_wrapper ctx_w;
     ctx_w.ptr = ctx;
     // call the python callback
 //    py::gil_scoped_acquire gil;  // Acquire the GIL while in this scope.
     py_new_segment_callback(ctx_w, n_new, user_data);
 };
 
 void assign_new_segment_callback(struct whisper_full_params *params, py::function f){
     params->new_segment_callback = _new_segment_callback;
     py_new_segment_callback = f;
 };
 
-bool _encoder_begin_callback(struct whisper_context * ctx, void * user_data){
+bool _encoder_begin_callback(struct whisper_context * ctx, struct whisper_state * state, void * user_data){
     struct whisper_context_wrapper ctx_w;
     ctx_w.ptr = ctx;
     // call the python callback
     py::object result_py = py_encoder_begin_callback(ctx_w, user_data);
     bool res = result_py.cast<bool>();
     return res;
 }
@@ -305,14 +305,15 @@
 void assign_encoder_begin_callback(struct whisper_full_params *params, py::function f){
     params->encoder_begin_callback = _encoder_begin_callback;
     py_encoder_begin_callback = f;
 }
 
 void _logits_filter_callback(
         struct whisper_context * ctx,
+        struct whisper_state * state,
         const whisper_token_data * tokens,
         int   n_tokens,
         float * logits,
         void * user_data){
     struct whisper_context_wrapper ctx_w;
     ctx_w.ptr = ctx;
     // call the python callback
@@ -480,14 +481,15 @@
         .def_readwrite("thold_pt", &whisper_full_params::thold_pt)
         .def_readwrite("thold_ptsum", &whisper_full_params::thold_ptsum)
         .def_readwrite("max_len", &whisper_full_params::max_len)
         .def_readwrite("split_on_word", &whisper_full_params::split_on_word)
         .def_readwrite("max_tokens", &whisper_full_params::max_tokens)
         .def_readwrite("speed_up", &whisper_full_params::speed_up)
         .def_readwrite("audio_ctx", &whisper_full_params::audio_ctx)
+        .def_readwrite("initial_prompt", &whisper_full_params::initial_prompt)
         .def_readwrite("prompt_tokens", &whisper_full_params::prompt_tokens)
         .def_readwrite("prompt_n_tokens", &whisper_full_params::prompt_n_tokens)
         .def_property("language", [](whisper_full_params &self) {return py::str(self.language);},
                                  [](whisper_full_params &self, const char *new_c) {char* c = (char *)malloc(sizeof(new_c));
                                                                                     strcpy(c, new_c); self.language = c;})
 
         .def_readwrite("suppress_blank", &whisper_full_params::suppress_blank)
```

### Comparing `pywhispercpp-1.0.8/tests/test_c_api.py` & `pywhispercpp-1.1.0/tests/test_c_api.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/tests/test_model.py` & `pywhispercpp-1.1.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/whisper.cpp/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/CMakeLists.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 cmake_minimum_required (VERSION 3.0)
 
-project(whisper.cpp VERSION 1.2.1)
+project(whisper.cpp VERSION 1.4.0)
+
+if ("${CMAKE_CXX_COMPILER_ID}" STREQUAL "MSVC")
+    add_compile_options(/utf-8)
+endif ()
 
 # Add path to modules
 list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake/")
 
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
 
 if(CMAKE_SOURCE_DIR STREQUAL CMAKE_CURRENT_SOURCE_DIR)
@@ -31,38 +35,42 @@
     else()
         set(BUILD_SHARED_LIBS_DEFAULT ON)
     endif()
 endif()
 
 # options
 
-option(BUILD_SHARED_LIBS               "whisper: build shared libs" ${BUILD_SHARED_LIBS_DEFAULT})
+option(BUILD_SHARED_LIBS              "whisper: build shared libs" ${BUILD_SHARED_LIBS_DEFAULT})
 
-option(WHISPER_ALL_WARNINGS            "whisper: enable all compiler warnings"                   ON)
-option(WHISPER_ALL_WARNINGS_3RD_PARTY  "whisper: enable all compiler warnings in 3rd party libs" OFF)
+option(WHISPER_ALL_WARNINGS           "whisper: enable all compiler warnings"                   ON)
+option(WHISPER_ALL_WARNINGS_3RD_PARTY "whisper: enable all compiler warnings in 3rd party libs" OFF)
 
-option(WHISPER_SANITIZE_THREAD         "whisper: enable thread sanitizer"    OFF)
-option(WHISPER_SANITIZE_ADDRESS        "whisper: enable address sanitizer"   OFF)
-option(WHISPER_SANITIZE_UNDEFINED      "whisper: enable undefined sanitizer" OFF)
+option(WHISPER_SANITIZE_THREAD        "whisper: enable thread sanitizer"    OFF)
+option(WHISPER_SANITIZE_ADDRESS       "whisper: enable address sanitizer"   OFF)
+option(WHISPER_SANITIZE_UNDEFINED     "whisper: enable undefined sanitizer" OFF)
 
-option(WHISPER_BUILD_TESTS             "whisper: build tests"    ${WHISPER_STANDALONE})
-option(WHISPER_BUILD_EXAMPLES          "whisper: build examples" ${WHISPER_STANDALONE})
+option(WHISPER_BUILD_TESTS            "whisper: build tests"    ${WHISPER_STANDALONE})
+option(WHISPER_BUILD_EXAMPLES         "whisper: build examples" ${WHISPER_STANDALONE})
 
-option(WHISPER_SUPPORT_SDL2            "whisper: support for libSDL2" OFF)
+option(WHISPER_SDL2                   "whisper: support for libSDL2" OFF)
 
 if (APPLE)
-    option(WHISPER_NO_ACCELERATE       "whisper: disable Accelerate framework" OFF)
-    option(WHISPER_NO_AVX              "whisper: disable AVX" OFF)
-    option(WHISPER_NO_AVX2             "whisper: disable AVX2" OFF)
-    option(WHISPER_NO_FMA              "whisper: disable FMA" OFF)
+    option(WHISPER_NO_ACCELERATE         "whisper: disable Accelerate framework" OFF)
+    option(WHISPER_NO_AVX                "whisper: disable AVX" OFF)
+    option(WHISPER_NO_AVX2               "whisper: disable AVX2" OFF)
+    option(WHISPER_NO_FMA                "whisper: disable FMA" OFF)
+
+    option(WHISPER_COREML                "whisper: enable Core ML framework" OFF)
+    option(WHISPER_COREML_ALLOW_FALLBACK "whisper: allow non-CoreML fallback" OFF)
 else()
-    option(WHISPER_SUPPORT_OPENBLAS    "whisper: support for OpenBLAS" OFF)
+    option(WHISPER_OPENBLAS              "whisper: support for OpenBLAS" OFF)
+    option(WHISPER_CUBLAS                "whisper: support for cuBLAS" OFF)
 endif()
 
-option(WHISPER_PERF                    "whisper: enable perf timings" OFF)
+option(WHISPER_PERF "whisper: enable perf timings" OFF)
 
 # sanitizers
 
 if (NOT MSVC)
     if (WHISPER_SANITIZE_THREAD)
         set(CMAKE_C_FLAGS   "${CMAKE_C_FLAGS}   -fsanitize=thread")
         set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fsanitize=thread")
@@ -82,41 +90,87 @@
 #set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -ffast-math")
 #set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -march=native")
 
 # dependencies
 
 find_package(Threads REQUIRED)
 
-# on APPLE - include Accelerate framework
-if (APPLE AND NOT WHISPER_NO_ACCELERATE)
-    find_library(ACCELERATE_FRAMEWORK Accelerate)
-    if (ACCELERATE_FRAMEWORK)
-        message(STATUS "Accelerate framework found")
+# on APPLE
+if (APPLE)
+    # include Accelerate framework
+    if (NOT WHISPER_NO_ACCELERATE)
+        find_library(ACCELERATE_FRAMEWORK Accelerate)
 
-        set(WHISPER_EXTRA_LIBS  ${WHISPER_EXTRA_LIBS}  ${ACCELERATE_FRAMEWORK})
-        set(WHISPER_EXTRA_FLAGS ${WHISPER_EXTRA_FLAGS} -DGGML_USE_ACCELERATE)
-    else()
-        message(WARNING "Accelerate framework not found")
+        if (ACCELERATE_FRAMEWORK)
+            message(STATUS "Accelerate framework found")
+
+            set(WHISPER_EXTRA_LIBS  ${WHISPER_EXTRA_LIBS}  ${ACCELERATE_FRAMEWORK})
+            set(WHISPER_EXTRA_FLAGS ${WHISPER_EXTRA_FLAGS} -DGGML_USE_ACCELERATE)
+        else()
+            message(WARNING "Accelerate framework not found")
+        endif()
+    endif()
+
+    if (WHISPER_COREML)
+        find_library(FOUNDATION_FRAMEWORK Foundation)
+        find_library(COREML_FRAMEWORK CoreML)
+
+        if (COREML_FRAMEWORK)
+            message(STATUS "CoreML framework found")
+
+            set(WHISPER_EXTRA_FLAGS ${WHISPER_EXTRA_FLAGS} -DWHISPER_USE_COREML)
+        else()
+            message(WARNING "CoreML framework not found")
+        endif()
+
+        if (WHISPER_COREML_ALLOW_FALLBACK)
+            set(WHISPER_EXTRA_FLAGS ${WHISPER_EXTRA_FLAGS} -DWHISPER_USE_COREML_ALLOW_FALLBACK)
+        endif()
     endif()
 endif()
 
-if (WHISPER_SUPPORT_OPENBLAS)
+if (WHISPER_OPENBLAS)
     find_library(OPENBLAS_LIB
         NAMES openblas libopenblas
         )
     if (OPENBLAS_LIB)
         message(STATUS "OpenBLAS found")
 
         set(WHISPER_EXTRA_LIBS  ${WHISPER_EXTRA_LIBS}  ${OPENBLAS_LIB})
         set(WHISPER_EXTRA_FLAGS ${WHISPER_EXTRA_FLAGS} -DGGML_USE_OPENBLAS)
     else()
         message(WARNING "OpenBLAS not found")
     endif()
 endif()
 
+if (WHISPER_CUBLAS)
+    cmake_minimum_required(VERSION 3.17)
+
+    find_package(CUDAToolkit)
+
+    if (CUDAToolkit_FOUND)
+        message(STATUS "cuBLAS found")
+
+        enable_language(CUDA)
+
+        set(GGML_CUDA_SOURCES ggml-cuda.cu ggml-cuda.h)
+
+        add_compile_definitions(GGML_USE_CUBLAS)
+
+        if (WHISPER_STATIC)
+            set(WHISPER_EXTRA_LIBS ${WHISPER_EXTRA_LIBS} CUDA::cudart_static CUDA::cublas_static CUDA::cublasLt_static)
+        else()
+            set(WHISPER_EXTRA_LIBS ${WHISPER_EXTRA_LIBS} CUDA::cudart CUDA::cublas CUDA::cublasLt)
+        endif()
+
+    else()
+        message(WARNING "cuBLAS not found")
+    endif()
+endif()
+
 # compiler flags
 
 if (NOT CMAKE_BUILD_TYPE AND NOT CMAKE_CONFIGURATION_TYPES)
     set(CMAKE_BUILD_TYPE Release CACHE STRING "Build type" FORCE)
     set_property(CACHE CMAKE_BUILD_TYPE PROPERTY STRINGS "Debug" "Release" "RelWithDebInfo")
 endif ()
 
@@ -168,42 +222,76 @@
             endif()
             if(NOT WHISPER_NO_AVX2)
                 set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -mavx2")
             endif()
             if(NOT WHISPER_NO_FMA)
                 set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -mfma")
             endif()
-            set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -mf16c")
+            if(NOT WHISPER_NO_F16C)
+                set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -mf16c")
+            endif()
         endif()
     endif()
 endif()
 
 if (WHISPER_PERF)
     set(WHISPER_EXTRA_FLAGS ${WHISPER_EXTRA_FLAGS} -DGGML_PERF)
 endif()
 
 #
+# whisper.coreml - Core ML support
+#
+
+if (WHISPER_COREML)
+    set(TARGET whisper.coreml)
+
+    add_library(${TARGET}
+        coreml/whisper-encoder.h
+        coreml/whisper-encoder.mm
+        coreml/whisper-encoder-impl.h
+        coreml/whisper-encoder-impl.m
+        )
+
+    include(DefaultTargetOptions)
+
+    target_include_directories(${TARGET} PUBLIC
+        .
+        )
+
+    target_link_libraries(${TARGET} PRIVATE ${FOUNDATION_FRAMEWORK} ${COREML_FRAMEWORK})
+
+    set_target_properties(${TARGET} PROPERTIES
+        COMPILE_FLAGS "-fobjc-arc"
+        )
+endif()
+
+#
 # whisper - this is the main library of the project
 #
 
 set(TARGET whisper)
 
 add_library(${TARGET}
     ggml.h
     ggml.c
+    ${GGML_CUDA_SOURCES}
     whisper.h
     whisper.cpp
     )
 
 include(DefaultTargetOptions)
 
 target_include_directories(${TARGET} PUBLIC
     .
     )
 
+if (WHISPER_COREML)
+    target_link_libraries(${TARGET} PRIVATE whisper.coreml)
+endif()
+
 if (MSVC)
     target_link_libraries(${TARGET} PRIVATE ${WHISPER_EXTRA_LIBS} ${CMAKE_THREAD_LIBS_INIT})
 
     set(WHISPER_EXTRA_FLAGS ${WHISPER_EXTRA_FLAGS} -D_CRT_SECURE_NO_WARNINGS)
 else()
     target_link_libraries(${TARGET} PRIVATE m ${WHISPER_EXTRA_LIBS} ${CMAKE_THREAD_LIBS_INIT})
 endif()
@@ -211,17 +299,29 @@
 if (BUILD_SHARED_LIBS)
     target_link_libraries(${TARGET} PUBLIC
         ${CMAKE_DL_LIBS}
         )
 
     target_compile_definitions(${TARGET} PUBLIC
         WHISPER_SHARED
+        GGML_SHARED
+        )
+
+    target_compile_definitions(${TARGET} PRIVATE
+        WHISPER_BUILD
+        GGML_BUILD
         )
 endif()
 
+if (GGML_CUDA_SOURCES)
+    message(STATUS "GGML CUDA sources found, configuring CUDA architecture")
+    set_property(TARGET whisper PROPERTY CUDA_ARCHITECTURES OFF)
+    set_property(TARGET whisper PROPERTY CUDA_SELECT_NVCC_ARCH_FLAGS "Auto")
+endif()
+
 if (EMSCRIPTEN)
     set_target_properties(${TARGET} PROPERTIES COMPILE_FLAGS "-msimd128")
 endif()
 
 target_compile_definitions(${TARGET} PUBLIC
     ${WHISPER_EXTRA_FLAGS}
     )
```

### Comparing `pywhispercpp-1.0.8/whisper.cpp/bindings/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/whisper.cpp/bindings/javascript/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/bindings/javascript/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/whisper.cpp/cmake/BuildTypes.cmake` & `pywhispercpp-1.1.0/whisper.cpp/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/whisper.cpp/cmake/GitVars.cmake` & `pywhispercpp-1.1.0/whisper.cpp/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/whisper.cpp/examples/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/examples/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # dependencies
 
 find_package(Threads REQUIRED)
 
 # third-party
 
-if (WHISPER_SUPPORT_SDL2)
+if (WHISPER_SDL2)
     # SDL2
     find_package(SDL2 REQUIRED)
 
     string(STRIP "${SDL2_LIBRARIES}" SDL2_LIBRARIES)
 
     message(STATUS "SDL2_INCLUDE_DIRS = ${SDL2_INCLUDE_DIRS}")
     message(STATUS "SDL2_LIBRARIES = ${SDL2_LIBRARIES}")
@@ -17,21 +17,25 @@
 # common
 
 set(TARGET common)
 
 add_library(${TARGET} STATIC
     common.h
     common.cpp
+    common-ggml.h
+    common-ggml.cpp
     )
 
 include(DefaultTargetOptions)
 
+target_link_libraries(${TARGET} PRIVATE whisper)
+
 set_target_properties(${TARGET} PROPERTIES POSITION_INDEPENDENT_CODE ON)
 
-if (WHISPER_SUPPORT_SDL2)
+if (WHISPER_SDL2)
     # common-sdl
 
     set(TARGET common-sdl)
 
     add_library(${TARGET} STATIC
         common-sdl.h
         common-sdl.cpp
@@ -58,9 +62,11 @@
 elseif(CMAKE_JS_VERSION)
     add_subdirectory(addon.node)
 else()
     add_subdirectory(main)
     add_subdirectory(stream)
     add_subdirectory(command)
     add_subdirectory(bench)
+    add_subdirectory(quantize)
     add_subdirectory(talk)
+    add_subdirectory(talk-llama)
 endif()
```

### Comparing `pywhispercpp-1.0.8/whisper.cpp/examples/addon.node/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/examples/addon.node/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/whisper.cpp/examples/bench.wasm/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/examples/bench.wasm/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         ${CMAKE_RUNTIME_OUTPUT_DIRECTORY}/bench.wasm/bench.js
         )
 endif()
 
 set_target_properties(${TARGET} PROPERTIES LINK_FLAGS " \
     --bind \
     -s USE_PTHREADS=1 \
-    -s PTHREAD_POOL_SIZE=8 \
-    -s INITIAL_MEMORY=1024MB \
-    -s TOTAL_MEMORY=1024MB \
+    -s PTHREAD_POOL_SIZE_STRICT=0 \
+    -s INITIAL_MEMORY=2000MB \
+    -s TOTAL_MEMORY=2000MB \
     -s FORCE_FILESYSTEM=1 \
     -s EXPORTED_RUNTIME_METHODS=\"['print', 'printErr', 'ccall', 'cwrap']\" \
     ${EXTRA_FLAGS} \
     ")
 
 #
 # bench.wasm
```

### Comparing `pywhispercpp-1.0.8/whisper.cpp/examples/command.wasm/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/examples/command.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/whisper.cpp/examples/stream.wasm/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/examples/stream.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywhispercpp-1.0.8/whisper.cpp/examples/talk/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/examples/talk-llama/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-if (WHISPER_SUPPORT_SDL2)
-    # talk
-    set(TARGET talk)
-    #add_executable(${TARGET} talk.cpp gpt-2.cpp)
+if (WHISPER_SDL2)
+    # talk-llama
+    set(TARGET talk-llama)
+    #add_executable(${TARGET} talk-llama.cpp llama.cpp)
     #target_include_directories(${TARGET} PRIVATE ${SDL2_INCLUDE_DIRS})
-    #target_link_libraries(${TARGET} PRIVATE whisper ${SDL2_LIBRARIES} ${CMAKE_THREAD_LIBS_INIT})
+    #target_link_libraries(${TARGET} PRIVATE common common-sdl whisper ${SDL2_LIBRARIES} ${CMAKE_THREAD_LIBS_INIT})
 
     # TODO: this is temporary
     #       need to export ggml symbols for MSVC, but too lazy ..
-    add_executable(${TARGET} talk.cpp gpt-2.cpp ../common.cpp ../common-sdl.cpp ../../ggml.c ../../whisper.cpp)
-
-    include(DefaultTargetOptions)
+    add_executable(${TARGET} talk-llama.cpp llama.cpp ../common.cpp ../common-sdl.cpp ../../ggml.c ../../whisper.cpp)
 
     target_include_directories(${TARGET} PRIVATE ${SDL2_INCLUDE_DIRS} ../../)
     target_link_libraries(${TARGET} PRIVATE ${SDL2_LIBRARIES} ${CMAKE_THREAD_LIBS_INIT})
+
+    include(DefaultTargetOptions)
 endif ()
```

### Comparing `pywhispercpp-1.0.8/whisper.cpp/examples/talk.wasm/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/examples/talk.wasm/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     gpt-2.cpp
     )
 
 include(DefaultTargetOptions)
 
 target_link_libraries(${TARGET} PRIVATE
     whisper
+    common
     )
 
 unset(EXTRA_FLAGS)
 
 if (WHISPER_WASM_SINGLE_FILE)
     set(EXTRA_FLAGS "-s SINGLE_FILE=1")
     message(STATUS "Embedding WASM inside talk.js")
```

### Comparing `pywhispercpp-1.0.8/whisper.cpp/examples/whisper.wasm/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/examples/whisper.wasm/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         ${CMAKE_RUNTIME_OUTPUT_DIRECTORY}/whisper.wasm/main.js
         )
 endif()
 
 set_target_properties(${TARGET} PROPERTIES LINK_FLAGS " \
     --bind \
     -s USE_PTHREADS=1 \
-    -s PTHREAD_POOL_SIZE=8 \
-    -s INITIAL_MEMORY=1500MB \
-    -s TOTAL_MEMORY=1500MB \
+    -s PTHREAD_POOL_SIZE_STRICT=0 \
+    -s INITIAL_MEMORY=2000MB \
+    -s TOTAL_MEMORY=2000MB \
     -s FORCE_FILESYSTEM=1 \
     -s EXPORTED_RUNTIME_METHODS=\"['print', 'printErr', 'ccall', 'cwrap']\" \
     ${EXTRA_FLAGS} \
     ")
 
 #
 # whisper.wasm
```

### Comparing `pywhispercpp-1.0.8/whisper.cpp/tests/CMakeLists.txt` & `pywhispercpp-1.1.0/whisper.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

