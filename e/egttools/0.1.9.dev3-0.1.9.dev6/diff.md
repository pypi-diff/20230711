# Comparing `tmp/egttools-0.1.9.dev3.tar.gz` & `tmp/egttools-0.1.9.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egttools-0.1.9.dev3.tar", last modified: Thu Feb  3 08:36:39 2022, max compression
+gzip compressed data, was "egttools-0.1.9.dev6.tar", last modified: Wed Feb 16 16:18:48 2022, max compression
```

## Comparing `egttools-0.1.9.dev3.tar` & `egttools-0.1.9.dev6.tar`

### file list

```diff
@@ -1,437 +1,439 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.237995 egttools-0.1.9.dev3/
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/.clang-format
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)     3110 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5233 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    17396 2022-02-03 08:36:39.237995 egttools-0.1.9.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16004 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.157994 egttools-0.1.9.dev3/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.161995 egttools-0.1.9.dev3/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/cmake/Modules/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/cmake/Modules/FindLpSolve.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.161995 egttools-0.1.9.dev3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.161995 egttools-0.1.9.dev3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/_static/pydata-custom.css
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/_static/readthedocs-custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.161995 egttools-0.1.9.dev3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9819 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.165995 egttools-0.1.9.dev3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)   193899 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/examples/hawk_dove_dynamics.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   102543 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/examples/normal_form_game_mc_simulations.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    91749 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/examples/plot_invasion_diagram.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   825735 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/examples/plot_simplex.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   817067 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/examples/plot_simplex_simplified.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.165995 egttools-0.1.9.dev3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)    14652 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/hawk_dove_analytical_full_sd.png
--rw-r--r--   0 runner    (1001) docker     (121)    14756 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/hawk_dove_analytical_gradient.png
--rw-r--r--   0 runner    (1001) docker     (121)    16051 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/hawk_dove_comparison.png
--rw-r--r--   0 runner    (1001) docker     (121)    21462 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/hawk_dove_indep_runs.png
--rw-r--r--   0 runner    (1001) docker     (121)    20400 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/logo-full.pdf
--rw-r--r--   0 runner    (1001) docker     (121)     7220 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/logo-full.png
--rw-r--r--   0 runner    (1001) docker     (121)     8096 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/logo-full.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14744 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/logo.pdf
--rw-r--r--   0 runner    (1001) docker     (121)     6212 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     4796 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    99153 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/simplex_example_infinite_pop_1.png
--rw-r--r--   0 runner    (1001) docker     (121)    60130 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/images/simplex_example_infinite_pop_2.png
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/pybind11_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/analytical/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/analytical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22203 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/analytical/sed_analytical.py
--rw-r--r--   0 runner    (1001) docker     (121)     4811 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/analytical/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/behaviors/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/behaviors/CRD/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/behaviors/CRD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/behaviors/CRD/moving_average.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/behaviors/NormalForm/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/behaviors/NormalForm/TwoActions/
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/behaviors/NormalForm/TwoActions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5026 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/behaviors/NormalForm/TwoActions/nfg_strategies.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/behaviors/NormalForm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/behaviors/pgg_behaviors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/datastructures/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/datastructures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/distributions/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/distributions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/games/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9363 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/games/crd.py
--rw-r--r--   0 runner    (1001) docker     (121)     6556 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/games/informal_risk.py
--rw-r--r--   0 runner    (1001) docker     (121)     6635 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/games/pgg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/helpers/vectorized.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/egttools/plotting/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20722 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/plotting/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10721 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/plotting/indicators.py
--rw-r--r--   0 runner    (1001) docker     (121)    38963 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/plotting/simplex2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     7446 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/plotting/simplified.py
--rw-r--r--   0 runner    (1001) docker     (121)    11602 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/egttools/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.157994 egttools-0.1.9.dev3/include/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/include/egttools/
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/Data.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7597 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/Distributions.h
--rw-r--r--   0 runner    (1001) docker     (121)     6732 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/LruCache.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/OpenMPUtils.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    10063 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/Sampling.h
--rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/SeedGenerator.h
--rw-r--r--   0 runner    (1001) docker     (121)     3359 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/Types.h
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/Utils.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.169994 egttools-0.1.9.dev3/include/egttools/finite_populations/
--rw-r--r--   0 runner    (1001) docker     (121)    70879 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/MLS.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    52897 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/PairwiseMoran.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7255 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/Utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.173995 egttools-0.1.9.dev3/include/egttools/finite_populations/behaviors/
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/behaviors/AbstractCRDStrategy.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/behaviors/AbstractNFGStrategy.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/behaviors/CRDStrategies.h
--rw-r--r--   0 runner    (1001) docker     (121)     9567 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/behaviors/NFGStrategies.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.173995 egttools-0.1.9.dev3/include/egttools/finite_populations/games/
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/games/AbstractGame.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7747 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/games/CRDGame.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     8412 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/games/CRDGameTU.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     5933 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/games/NormalFormGame.h
--rw-r--r--   0 runner    (1001) docker     (121)     6740 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/games/OneShotCRD.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.173995 egttools-0.1.9.dev3/include/egttools/finite_populations/structure/
--rw-r--r--   0 runner    (1001) docker     (121)     8556 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/structure/GarciaGroup.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7627 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/finite_populations/structure/Group.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.173995 egttools-0.1.9.dev3/include/egttools/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/utils/CalculateExpectedIndicators.h
--rw-r--r--   0 runner    (1001) docker     (121)     3202 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/include/egttools/utils/TimingUncertainty.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.173995 egttools-0.1.9.dev3/pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.clang-format
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.clang-tidy
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.cmake-format.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.173995 egttools-0.1.9.dev3/pybind11/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (121)    15186 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.173995 egttools-0.1.9.dev3/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/labeler_merged.yml
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.177995 egttools-0.1.9.dev3/pybind11/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)    28145 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2516 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11005 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7647 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.185995 egttools-0.1.9.dev3/pybind11/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (121)     7417 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.185995 egttools-0.1.9.dev3/pybind11/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.185995 egttools-0.1.9.dev3/pybind11/docs/advanced/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.189995 egttools-0.1.9.dev3/pybind11/docs/advanced/cast/
--rw-r--r--   0 runner    (1001) docker     (121)     3937 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3400 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14287 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3889 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12073 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9703 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9363 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 runner    (1001) docker     (121)    47042 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8453 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (121)    17812 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)    25383 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12446 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.189995 egttools-0.1.9.dev3/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    17447 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9030 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5710 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6367 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9369 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (121)    90570 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)    16451 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/classes.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.189995 egttools-0.1.9.dev3/pybind11/docs/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/cmake/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    26266 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/compiling.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12082 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    14599 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3277 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (121)    58510 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    44653 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 runner    (1001) docker     (121)    87708 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 runner    (1001) docker     (121)    41121 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 runner    (1001) docker     (121)    85853 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2647 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    23281 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.157994 egttools-0.1.9.dev3/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.197995 egttools-0.1.9.dev3/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)    23059 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (121)     6131 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (121)    60192 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (121)     8674 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.197995 egttools-0.1.9.dev3/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (121)    27922 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (121)    47724 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (121)     3766 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (121)    16961 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (121)    21551 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (121)    42197 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (121)    29436 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (121)    11439 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (121)     5431 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (121)     4573 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (121)     6520 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (121)     8882 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (121)    71895 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (121)     8771 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (121)   116190 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (121)    74609 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.201995 egttools-0.1.9.dev3/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (121)    13650 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (121)    26460 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.201995 egttools-0.1.9.dev3/pybind11/pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/pybind11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/pybind11/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/pybind11/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/pybind11/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/pybind11/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/pybind11/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    16907 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/pybind11/setup_helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.225995 egttools-0.1.9.dev3/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    17744 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4841 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    11157 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/constructor_stats.h
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/env.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.225995 egttools-0.1.9.dev3/pybind11/tests/extra_python_package/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     7578 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.225995 egttools-0.1.9.dev3/pybind11/tests/extra_setuptools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3923 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2838 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/local_bindings.h
--rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/object.h
--rw-r--r--   0 runner    (1001) docker     (121)     6220 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_async.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (121)     8246 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13616 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    17601 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 runner    (1001) docker     (121)     4011 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6573 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_call_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     8935 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6044 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5727 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_chrono.py
--rw-r--r--   0 runner    (1001) docker     (121)    22365 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_class.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    14508 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_class.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.225995 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.225995 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.225995 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.225995 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.225995 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.225995 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.225995 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5885 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10094 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4646 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_copy_move.py
--rw-r--r--   0 runner    (1001) docker     (121)     5709 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2514 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 runner    (1001) docker     (121)    17490 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    28283 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.229995 egttools-0.1.9.dev3/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11871 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5740 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9132 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_eval.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_eval_call.py
--rw-r--r--   0 runner    (1001) docker     (121)     9649 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_exceptions.h
--rw-r--r--   0 runner    (1001) docker     (121)     8616 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    17330 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    16731 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 runner    (1001) docker     (121)     4076 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7958 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_iostream.py
--rw-r--r--   0 runner    (1001) docker     (121)     6661 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10047 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     4403 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8101 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)    20409 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    17616 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_modules.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     9390 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9494 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (121)    18960 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    20339 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 runner    (1001) docker     (121)    18904 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    13999 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9710 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8597 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 runner    (1001) docker     (121)     6623 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (121)    20399 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    18860 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_pytypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    19446 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8059 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)    18870 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9620 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 runner    (1001) docker     (121)    20521 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_stl.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11662 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4438 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8071 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_thread.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_union.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (121)    20182 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12736 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.229995 egttools-0.1.9.dev3/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     9977 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (121)     1423 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1306 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (121)    14348 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (121)     9588 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     7447 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-02-03 08:34:44.000000 egttools-0.1.9.dev3/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.157994 egttools-0.1.9.dev3/res/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.157994 egttools-0.1.9.dev3/res/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.229995 egttools-0.1.9.dev3/res/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/res/cmake/Modules/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/res/cmake/Modules/FindLpSolve.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3790 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.233995 egttools-0.1.9.dev3/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.233995 egttools-0.1.9.dev3/src/egttools/
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/Data.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3030 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/Distributions.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/SeedGenerator.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.233995 egttools-0.1.9.dev3/src/egttools/finite_populations/
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16015 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/MLS.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7519 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/Utils.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.233995 egttools-0.1.9.dev3/src/egttools/finite_populations/behaviors/
--rw-r--r--   0 runner    (1001) docker     (121)     2767 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/behaviors/CRDStrategies.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9284 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/behaviors/NFGStrategies.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.233995 egttools-0.1.9.dev3/src/egttools/finite_populations/games/
--rw-r--r--   0 runner    (1001) docker     (121)    17809 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/games/CRDGame.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    18823 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/games/CRDGameTU.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11161 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/games/NormalFormGame.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10189 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/games/OneShotCRD.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.233995 egttools-0.1.9.dev3/src/egttools/finite_populations/structure/
--rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/structure/GarciaGroup.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/finite_populations/structure/Group.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.233995 egttools-0.1.9.dev3/src/egttools/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/utils/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools/utils/CalculateExpectedIndicators.cpp
--rw-r--r--   0 runner    (1001) docker     (121)   104156 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/egttools.h
--rw-r--r--   0 runner    (1001) docker     (121)    11708 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/python_stubs.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/src/version.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 08:36:39.237995 egttools-0.1.9.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_PairwiseMoran_run.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_PairwiseMoran_stationary_distribution_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3631 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_PairwiseMoran_stationary_distribution_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_analytical.py
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_crd_game.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_crd_tu_game.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_eigen_sparse_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_mc_simulations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_numerical.py
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_oneshotcrd_game.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_openmp.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_ordered_sampling_without_replacement.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_timing_uncertainty.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-02-03 08:34:43.000000 egttools-0.1.9.dev3/tests/test_virtual_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.359691 egttools-0.1.9.dev6/
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (121)     3651 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (121)     6382 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5233 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    17634 2022-02-16 16:18:48.359691 egttools-0.1.9.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    16242 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.311690 egttools-0.1.9.dev6/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.319690 egttools-0.1.9.dev6/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/cmake/Modules/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/cmake/Modules/FindLpSolve.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.319690 egttools-0.1.9.dev6/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.319690 egttools-0.1.9.dev6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/_static/pydata-custom.css
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/_static/readthedocs-custom.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.319690 egttools-0.1.9.dev6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9819 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.323690 egttools-0.1.9.dev6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)   194355 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/examples/hawk_dove_dynamics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   102543 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/examples/normal_form_game_mc_simulations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   100786 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/examples/plot_invasion_diagram.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   681962 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/examples/plot_simplex.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   676103 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/examples/plot_simplex_simplified.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.323690 egttools-0.1.9.dev6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    14652 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/hawk_dove_analytical_full_sd.png
+-rw-r--r--   0 runner    (1001) docker     (121)    14756 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/hawk_dove_analytical_gradient.png
+-rw-r--r--   0 runner    (1001) docker     (121)    16051 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/hawk_dove_comparison.png
+-rw-r--r--   0 runner    (1001) docker     (121)    21462 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/hawk_dove_indep_runs.png
+-rw-r--r--   0 runner    (1001) docker     (121)    20400 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/logo-full.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)     7220 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/logo-full.png
+-rw-r--r--   0 runner    (1001) docker     (121)     8096 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/logo-full.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    14744 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)     6212 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4796 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    99153 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/simplex_example_infinite_pop_1.png
+-rw-r--r--   0 runner    (1001) docker     (121)    60130 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/images/simplex_example_infinite_pop_2.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/pybind11_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.323690 egttools-0.1.9.dev6/egttools/
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.323690 egttools-0.1.9.dev6/egttools/analytical/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/analytical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24500 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/analytical/sed_analytical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4811 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/analytical/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.323690 egttools-0.1.9.dev6/egttools/behaviors/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.323690 egttools-0.1.9.dev6/egttools/behaviors/CRD/
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/behaviors/CRD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/behaviors/CRD/moving_average.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.323690 egttools-0.1.9.dev6/egttools/behaviors/NormalForm/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.323690 egttools-0.1.9.dev6/egttools/behaviors/NormalForm/TwoActions/
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/behaviors/NormalForm/TwoActions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5026 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/behaviors/NormalForm/TwoActions/nfg_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/behaviors/NormalForm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/behaviors/opinion_behaviors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/behaviors/pgg_behaviors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.323690 egttools-0.1.9.dev6/egttools/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/datastructures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.323690 egttools-0.1.9.dev6/egttools/distributions/
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/distributions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.327690 egttools-0.1.9.dev6/egttools/games/
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9363 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/games/crd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6556 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/games/informal_risk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7188 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/games/opinion_game.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6635 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/games/pgg.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.327690 egttools-0.1.9.dev6/egttools/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/helpers/vectorized.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.327690 egttools-0.1.9.dev6/egttools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20722 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/plotting/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10721 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/plotting/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38963 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/plotting/simplex2d.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11822 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/plotting/simplified.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12563 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/egttools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.315690 egttools-0.1.9.dev6/include/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.327690 egttools-0.1.9.dev6/include/egttools/
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/Data.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7597 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/Distributions.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6732 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/LruCache.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/OpenMPUtils.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    10063 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/Sampling.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/SeedGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3359 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/Types.h
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/Utils.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.327690 egttools-0.1.9.dev6/include/egttools/finite_populations/
+-rw-r--r--   0 runner    (1001) docker     (121)    70879 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/MLS.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    52889 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/PairwiseMoran.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7255 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/Utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.327690 egttools-0.1.9.dev6/include/egttools/finite_populations/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/behaviors/AbstractCRDStrategy.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/behaviors/AbstractNFGStrategy.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/behaviors/CRDStrategies.h
+-rw-r--r--   0 runner    (1001) docker     (121)     9567 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/behaviors/NFGStrategies.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.327690 egttools-0.1.9.dev6/include/egttools/finite_populations/games/
+-rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/games/AbstractGame.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7747 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/games/CRDGame.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8412 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/games/CRDGameTU.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5933 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/games/NormalFormGame.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6740 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/games/OneShotCRD.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.327690 egttools-0.1.9.dev6/include/egttools/finite_populations/structure/
+-rw-r--r--   0 runner    (1001) docker     (121)     8556 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/structure/GarciaGroup.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7627 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/finite_populations/structure/Group.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.327690 egttools-0.1.9.dev6/include/egttools/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/utils/CalculateExpectedIndicators.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3202 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/include/egttools/utils/TimingUncertainty.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.331690 egttools-0.1.9.dev6/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.clang-tidy
+-rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.cmake-format.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.331690 egttools-0.1.9.dev6/pybind11/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (121)    15186 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.331690 egttools-0.1.9.dev6/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/labeler_merged.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.331690 egttools-0.1.9.dev6/pybind11/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)    28145 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2516 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    11005 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7647 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.335690 egttools-0.1.9.dev6/pybind11/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (121)     7417 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.335690 egttools-0.1.9.dev6/pybind11/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.335690 egttools-0.1.9.dev6/pybind11/docs/advanced/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.335690 egttools-0.1.9.dev6/pybind11/docs/advanced/cast/
+-rw-r--r--   0 runner    (1001) docker     (121)     3937 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3400 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    14287 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3889 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12073 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9703 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9363 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    47042 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8453 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    17812 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    25383 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12446 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.335690 egttools-0.1.9.dev6/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    17447 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9030 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5710 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6367 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9369 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    90570 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    16451 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/classes.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.339691 egttools-0.1.9.dev6/pybind11/docs/cmake/
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    26266 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/compiling.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12082 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14599 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3277 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    58510 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)    44653 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 runner    (1001) docker     (121)    87708 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    41121 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 runner    (1001) docker     (121)    85853 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     2647 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4366 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    23281 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.315690 egttools-0.1.9.dev6/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.339691 egttools-0.1.9.dev6/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)    23059 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6131 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (121)    60192 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8674 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.339691 egttools-0.1.9.dev6/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (121)    27922 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (121)    47724 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3766 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (121)    16961 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (121)    21551 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (121)    42197 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (121)    29436 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (121)    11439 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5431 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4573 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6520 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8882 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    71895 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8771 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (121)   116190 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (121)    74609 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.339691 egttools-0.1.9.dev6/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (121)    13650 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    26460 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.343690 egttools-0.1.9.dev6/pybind11/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/pybind11/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/pybind11/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    16907 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/pybind11/setup_helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.351691 egttools-0.1.9.dev6/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    17744 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4841 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11157 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/env.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.351691 egttools-0.1.9.dev6/pybind11/tests/extra_python_package/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     7578 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.351691 egttools-0.1.9.dev6/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     3923 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2838 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/local_bindings.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/object.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6220 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 runner    (1001) docker     (121)      693 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      864 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8246 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13616 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    17601 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4011 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6573 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8935 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6044 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5727 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_chrono.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22365 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_class.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    14508 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.351691 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.351691 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.355691 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.355691 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.355691 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.355691 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.355691 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5885 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10094 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4646 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5709 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2514 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17490 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    28283 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_eigen.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.355691 egttools-0.1.9.dev6/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    11871 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5740 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9132 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9649 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8616 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17330 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    16731 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4076 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7958 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_iostream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6661 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    10047 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4403 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8101 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20409 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    17616 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9390 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9494 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18960 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    20339 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18904 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    13999 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9710 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8597 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6623 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20399 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    18860 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19446 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8059 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18870 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9620 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20521 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    11662 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4438 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8071 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_union.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20182 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12736 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.355691 egttools-0.1.9.dev6/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)     2295 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     9977 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1423 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1306 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14348 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9588 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     7447 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-02-16 16:17:45.000000 egttools-0.1.9.dev6/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.315690 egttools-0.1.9.dev6/res/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.315690 egttools-0.1.9.dev6/res/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.355691 egttools-0.1.9.dev6/res/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/res/cmake/Modules/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/res/cmake/Modules/FindLpSolve.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3790 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.355691 egttools-0.1.9.dev6/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.355691 egttools-0.1.9.dev6/src/egttools/
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/Data.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3030 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/Distributions.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/SeedGenerator.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.359691 egttools-0.1.9.dev6/src/egttools/finite_populations/
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16015 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/MLS.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7519 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/Utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.359691 egttools-0.1.9.dev6/src/egttools/finite_populations/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (121)     2767 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/behaviors/CRDStrategies.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9284 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/behaviors/NFGStrategies.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.359691 egttools-0.1.9.dev6/src/egttools/finite_populations/games/
+-rw-r--r--   0 runner    (1001) docker     (121)    17809 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/games/CRDGame.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    18823 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/games/CRDGameTU.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    11161 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/games/NormalFormGame.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    10189 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/games/OneShotCRD.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.359691 egttools-0.1.9.dev6/src/egttools/finite_populations/structure/
+-rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/structure/GarciaGroup.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3026 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/finite_populations/structure/Group.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.359691 egttools-0.1.9.dev6/src/egttools/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      784 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/utils/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools/utils/CalculateExpectedIndicators.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)   104291 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/egttools.h
+-rw-r--r--   0 runner    (1001) docker     (121)    11708 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/python_stubs.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/src/version.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 16:18:48.359691 egttools-0.1.9.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     3948 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_PairwiseMoran_run.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_PairwiseMoran_stationary_distribution_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3631 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_PairwiseMoran_stationary_distribution_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_analytical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_crd_game.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_crd_tu_game.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_eigen_sparse_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_mc_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_oneshotcrd_game.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_openmp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_ordered_sampling_without_replacement.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_timing_uncertainty.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-02-16 16:17:43.000000 egttools-0.1.9.dev6/tests/test_virtual_functions.py
```

### Comparing `egttools-0.1.9.dev3/.clang-format` & `egttools-0.1.9.dev6/.clang-format`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/CHANGELOG.md` & `egttools-0.1.9.dev6/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,37 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this project adheres
 to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.1.9-patch6] - 16-02-2022
+
+### Fixed
+
+- Fixed error on version formatting, it should be `0.1.9.dev6` instead of `0.1.9.patch6`.
+
+## [0.1.9-patch5] - 16-02-2022
+
+### Fixed
+
+- Fixed wrong version tag on git.
+
+## [0.1.9-patch4] - 16-02-2022
+
+## Fixed
+
+- There was a problem with setting a `geometric_distribution` in C++ as a private variable for OpenMP which caused some
+  errors when estimating stationary distributions. This was fixed by setting it as a shared variable.
+
+## Added
+
+- Binder links to run examples and updated notebooks
+
 ## [0.1.9-patch3] - 03-02-2022
 
 ### Added
 
 - Added `gitter` chat and `binder` launch.
 
 ### Fixed
```

### Comparing `egttools-0.1.9.dev3/CITATION.cff` & `egttools-0.1.9.dev6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/CMakeLists.txt` & `egttools-0.1.9.dev6/CMakeLists.txt`

 * *Files 16% similar despite different names*

```diff
@@ -56,29 +56,43 @@
     message(STATUS "${_msg}")
     set(MACOSX_DEPLOYMENT_TARGET ${CMAKE_OSX_DEPLOYMENT_TARGET})
     message(STATUS "${_msg} - ${MACOSX_DEPLOYMENT_TARGET}")
 endif()
 
 # Necessary for certain MacOX versions to find homebrew OpenMP
 if (APPLE AND NOT SKIP_OPENMP)
-#    message("-- Try to install OpenMP")
-#    execute_process(COMMAND brew install libomp)
+    message("-- Try to install OpenMP")
+#    message(STATUS "BUILD_ARCH=$ENV{BUILD_ARCH}")
+#    if ("$ENV{BUILD_ARCH}" MATCHES "macosx_x86_64|macosx_universal2")
+#        message(STATUS "Using ANACONDA OpenMP")
+#        set(OPENMP_URL "https://anaconda.org/conda-forge/llvm-openmp/11.1.0/download/osx-64/llvm-openmp-11.1.0-hda6cdc1_1.tar.bz2")
+#        execute_process(COMMAND conda install ${OPENMP_URL})
+#        set(LIBOMP_DIR $ENV{CONDA_PREFIX})
+#    else()
+#        execute_process(COMMAND brew install libomp)
+#        execute_process(COMMAND brew --prefix libomp OUTPUT_VARIABLE LIBOMP_DIR)
+#        string(STRIP ${LIBOMP_DIR} LIBOMP_DIR)
+#    endif()
+
+    execute_process(COMMAND brew install libomp)
     execute_process(COMMAND brew --prefix libomp OUTPUT_VARIABLE LIBOMP_DIR)
     string(STRIP ${LIBOMP_DIR} LIBOMP_DIR)
 
     if (CMAKE_C_COMPILER_ID MATCHES "Clang\$")
         set(OpenMP_C_FLAGS "-Xpreprocessor -fopenmp -I${LIBOMP_DIR}/include")
         set(OpenMP_C_LIB_NAMES "omp")
         set(OpenMP_omp_LIBRARY ${LIBOMP_DIR}/lib/libomp.dylib)
+        set(LDFLAGS "$LDFLAGS -Wl,-rpath,${LIBOMP_DIR}/lib -L${LIBOMP_DIR}/lib -lomp")
     endif ()
 
     if (CMAKE_CXX_COMPILER_ID MATCHES "Clang\$")
         set(OpenMP_CXX_FLAGS "-Xpreprocessor -fopenmp -I${LIBOMP_DIR}/include")
         set(OpenMP_CXX_LIB_NAMES "omp")
         set(OpenMP_omp_LIBRARY ${LIBOMP_DIR}/lib/libomp.dylib)
+        set(LDFLAGS "$LDFLAGS -Wl,-rpath,${LIBOMP_DIR}/lib -L${LIBOMP_DIR}/lib -lomp")
     endif ()
 
 endif ()
 
 if (NOT WIN32)
     add_definitions(
             -Wall
@@ -112,15 +126,18 @@
     find_package(OpenMP)
     if (OPENMP_FOUND)
         include_directories(SYSTEM ${OPENMP_INCLUDE_DIR})
         message(STATUS "OpenMP enabled")
         if (NOT APPLE)
             SET(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${OpenMP_C_FLAGS}")
             SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS} -fopenmp")
-        endif ()
+        else()
+            SET(CMAKE_C_FLAGS "${CMAKE_C_FLAGS}")
+            SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")
+        endif()
     endif ()
 endif ()
 
 # Currently, scikit-build does not support FindPython.
 if (SKBUILD)
     set(Python_EXECUTABLE "${PYTHON_EXECUTABLE}")
     set(Python_INCLUDE_DIR "${PYTHON_INCLUDE_DIR}")
```

### Comparing `egttools-0.1.9.dev3/CODE_OF_CONDUCT.md` & `egttools-0.1.9.dev6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/LICENSE` & `egttools-0.1.9.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/MANIFEST.in` & `egttools-0.1.9.dev6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/PKG-INFO` & `egttools-0.1.9.dev6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egttools
-Version: 0.1.9.dev3
+Version: 0.1.9.dev6
 Summary: Efficient Python library for EGT
 Home-page: https://github.com/Socrats/EGTTools
 Author: Elias F. Domingos
 Author-email: elias.fernandez.domingos@vub.be
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/Socrats/EGTTools/issues
 Project-URL: Documentation, https://egttools.readthedocs.io/en/latest/
@@ -30,18 +30,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![EGTtools](docs/images/logo-full.png)
 
 # Toolbox for Evolutionary Game Theory
 
-[![DOI](https://zenodo.org/badge/242180332.svg)](https://zenodo.org/badge/latestdoi/242180332)
+[![PyPI version](https://badge.fury.io/py/egttools.svg)](https://badge.fury.io/py/egttools)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/egttools.svg?label=PyPI%20downloads)](https://pypi.org/project/egttools/)
 [![Documentation Status](https://readthedocs.org/projects/egttools/badge/?version=latest)](https://egttools.readthedocs.io/en/latest/?badge=latest)
 [![Build](https://github.com/Socrats/EGTTools/actions/workflows/ci.yml/badge.svg)](https://github.com/Socrats/EGTTools/actions/workflows/ci.yml) [![Join the chat at https://gitter.im/EGTTools/community](https://badges.gitter.im/EGTTools/community.svg)](https://gitter.im/EGTTools/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Socrats/EGTTools/HEAD?labpath=docs%2Fexamples)
+[![DOI](https://zenodo.org/badge/242180332.svg)](https://zenodo.org/badge/latestdoi/242180332)
 
 **EGTtools** provides a centralized repository with analytical and numerical methods to study/model game theoretical
 problems under the Evolutionary Game Theory (EGT) framework.
 
 This library is composed of two parts:
 
 - a set of analytical methods implemented in Python 3
@@ -113,14 +115,15 @@
 ```bash
 conda create -n egtenv python=3.9
 conda activate egtenv
 conda install numpy
 conda install scipy
 conda install matplotlib
 conda install networkx
+conda install seaborn
 ```
 
 ### Build from source
 
 To build `egttools` from source follow the following steps.
 
 To **install all required packages** run:
```

### Comparing `egttools-0.1.9.dev3/README.md` & `egttools-0.1.9.dev6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 ![EGTtools](docs/images/logo-full.png)
 
 # Toolbox for Evolutionary Game Theory
 
-[![DOI](https://zenodo.org/badge/242180332.svg)](https://zenodo.org/badge/latestdoi/242180332)
+[![PyPI version](https://badge.fury.io/py/egttools.svg)](https://badge.fury.io/py/egttools)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/egttools.svg?label=PyPI%20downloads)](https://pypi.org/project/egttools/)
 [![Documentation Status](https://readthedocs.org/projects/egttools/badge/?version=latest)](https://egttools.readthedocs.io/en/latest/?badge=latest)
 [![Build](https://github.com/Socrats/EGTTools/actions/workflows/ci.yml/badge.svg)](https://github.com/Socrats/EGTTools/actions/workflows/ci.yml) [![Join the chat at https://gitter.im/EGTTools/community](https://badges.gitter.im/EGTTools/community.svg)](https://gitter.im/EGTTools/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Socrats/EGTTools/HEAD?labpath=docs%2Fexamples)
+[![DOI](https://zenodo.org/badge/242180332.svg)](https://zenodo.org/badge/latestdoi/242180332)
 
 **EGTtools** provides a centralized repository with analytical and numerical methods to study/model game theoretical
 problems under the Evolutionary Game Theory (EGT) framework.
 
 This library is composed of two parts:
 
 - a set of analytical methods implemented in Python 3
@@ -81,14 +83,15 @@
 ```bash
 conda create -n egtenv python=3.9
 conda activate egtenv
 conda install numpy
 conda install scipy
 conda install matplotlib
 conda install networkx
+conda install seaborn
 ```
 
 ### Build from source
 
 To build `egttools` from source follow the following steps.
 
 To **install all required packages** run:
```

### Comparing `egttools-0.1.9.dev3/cmake/Modules/FindEigen3.cmake` & `egttools-0.1.9.dev6/cmake/Modules/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/cmake/Modules/FindLpSolve.cmake` & `egttools-0.1.9.dev6/cmake/Modules/FindLpSolve.cmake`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/CMakeLists.txt` & `egttools-0.1.9.dev6/docs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/Makefile` & `egttools-0.1.9.dev6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/_static/readthedocs-custom.css` & `egttools-0.1.9.dev6/docs/_static/readthedocs-custom.css`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/_templates/custom-class-template.rst` & `egttools-0.1.9.dev6/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/_templates/custom-module-template.rst` & `egttools-0.1.9.dev6/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/api.rst` & `egttools-0.1.9.dev6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/conf.py` & `egttools-0.1.9.dev6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/examples/hawk_dove_dynamics.ipynb` & `egttools-0.1.9.dev6/docs/examples/hawk_dove_dynamics.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997378947060713%*

 * *Differences: {"'cells'": "{9: {'outputs': {0: {'data': {'image/svg+xml': {insert: [(8, '    "*

 * *            "<dc:date>2022-02-16T15:38:23.257171</dc:date>\\n'), (40, '    <path "*

 * *            'clip-path="url(#pb10e2db317)" d="M 50.14375 214.255607 \\n\'), (144, \'    <path '*

 * *            'clip-path="url(#pb10e2db317)" d="M 50.14375 214.255607 \\n\'), (154, \'" '*

 * *            'id="m4d2406df1c" style="stroke:#000000;stroke-width:0.8;"/>\\n\'), (157, \'       '*

 * *            '<use style="stroke:#000000;stroke-width:0.8;" x="50.14 […]*

```diff
@@ -120,15 +120,15 @@
                             "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
                             "  \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
                             "<svg height=\"277.314375pt\" version=\"1.1\" viewBox=\"0 0 344.295312 277.314375\" width=\"344.295312pt\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
                             " <metadata>\n",
                             "  <rdf:RDF xmlns:cc=\"http://creativecommons.org/ns#\" xmlns:dc=\"http://purl.org/dc/elements/1.1/\" xmlns:rdf=\"http://www.w3.org/1999/02/22-rdf-syntax-ns#\">\n",
                             "   <cc:Work>\n",
                             "    <dc:type rdf:resource=\"http://purl.org/dc/dcmitype/StillImage\"/>\n",
-                            "    <dc:date>2022-02-02T11:27:54.354086</dc:date>\n",
+                            "    <dc:date>2022-02-16T15:38:23.257171</dc:date>\n",
                             "    <dc:format>image/svg+xml</dc:format>\n",
                             "    <dc:creator>\n",
                             "     <cc:Agent>\n",
                             "      <dc:title>Matplotlib v3.4.3, https://matplotlib.org/</dc:title>\n",
                             "     </cc:Agent>\n",
                             "    </dc:creator>\n",
                             "   </cc:Work>\n",
@@ -152,15 +152,15 @@
                             "L 329.14375 239.758125 \n",
                             "L 329.14375 22.318125 \n",
                             "L 50.14375 22.318125 \n",
                             "z\n",
                             "\" style=\"fill:#ffffff;\"/>\n",
                             "   </g>\n",
                             "   <g id=\"line2d_1\">\n",
-                            "    <path clip-path=\"url(#p8ae3ec6857)\" d=\"M 50.14375 214.255607 \n",
+                            "    <path clip-path=\"url(#pb10e2db317)\" d=\"M 50.14375 214.255607 \n",
                             "L 52.93375 200.696359 \n",
                             "L 55.72375 187.750839 \n",
                             "L 58.51375 175.408646 \n",
                             "L 61.30375 163.659378 \n",
                             "L 64.09375 152.492632 \n",
                             "L 66.88375 141.898006 \n",
                             "L 69.67375 131.865099 \n",
@@ -256,28 +256,28 @@
                             "L 320.77375 222.832209 \n",
                             "L 323.56375 220.372092 \n",
                             "L 326.35375 217.516692 \n",
                             "L 329.14375 214.255607 \n",
                             "\" style=\"fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;\"/>\n",
                             "   </g>\n",
                             "   <g id=\"line2d_2\">\n",
-                            "    <path clip-path=\"url(#p8ae3ec6857)\" d=\"M 50.14375 214.255607 \n",
+                            "    <path clip-path=\"url(#pb10e2db317)\" d=\"M 50.14375 214.255607 \n",
                             "L 329.14375 214.255607 \n",
                             "\" style=\"fill:none;stroke:#000000;stroke-linecap:square;stroke-width:1.5;\"/>\n",
                             "   </g>\n",
                             "   <g id=\"matplotlib.axis_1\">\n",
                             "    <g id=\"xtick_1\">\n",
                             "     <g id=\"line2d_3\">\n",
                             "      <defs>\n",
                             "       <path d=\"M 0 0 \n",
                             "L 0 3.5 \n",
-                            "\" id=\"mdb490bf413\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
+                            "\" id=\"m4d2406df1c\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
                             "      </defs>\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#mdb490bf413\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m4d2406df1c\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_1\">\n",
                             "      <!-- 0.0 -->\n",
                             "      <g transform=\"translate(42.192188 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2034 4250 \n",
@@ -314,15 +314,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-30\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_2\">\n",
                             "     <g id=\"line2d_4\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"105.94375\" xlink:href=\"#mdb490bf413\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"105.94375\" xlink:href=\"#m4d2406df1c\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_2\">\n",
                             "      <!-- 0.2 -->\n",
                             "      <g transform=\"translate(97.992188 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 1228 531 \n",
@@ -355,15 +355,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-32\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_3\">\n",
                             "     <g id=\"line2d_5\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"161.74375\" xlink:href=\"#mdb490bf413\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"161.74375\" xlink:href=\"#m4d2406df1c\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_3\">\n",
                             "      <!-- 0.4 -->\n",
                             "      <g transform=\"translate(153.792188 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2419 4116 \n",
@@ -391,15 +391,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-34\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_4\">\n",
                             "     <g id=\"line2d_6\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"217.54375\" xlink:href=\"#mdb490bf413\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"217.54375\" xlink:href=\"#m4d2406df1c\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_4\">\n",
                             "      <!-- 0.6 -->\n",
                             "      <g transform=\"translate(209.592188 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2113 2584 \n",
@@ -438,15 +438,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-36\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_5\">\n",
                             "     <g id=\"line2d_7\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"273.34375\" xlink:href=\"#mdb490bf413\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"273.34375\" xlink:href=\"#m4d2406df1c\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_5\">\n",
                             "      <!-- 0.8 -->\n",
                             "      <g transform=\"translate(265.392187 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2034 2216 \n",
@@ -494,15 +494,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-38\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_6\">\n",
                             "     <g id=\"line2d_8\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"329.14375\" xlink:href=\"#mdb490bf413\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"329.14375\" xlink:href=\"#m4d2406df1c\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_6\">\n",
                             "      <!-- 1.0 -->\n",
                             "      <g transform=\"translate(321.192187 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 794 531 \n",
@@ -552,18 +552,18 @@
                             "   </g>\n",
                             "   <g id=\"matplotlib.axis_2\">\n",
                             "    <g id=\"ytick_1\">\n",
                             "     <g id=\"line2d_9\">\n",
                             "      <defs>\n",
                             "       <path d=\"M 0 0 \n",
                             "L -3.5 0 \n",
-                            "\" id=\"mefb64c89f7\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
+                            "\" id=\"m3b81b6d414\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
                             "      </defs>\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#mefb64c89f7\" y=\"214.255607\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m3b81b6d414\" y=\"214.255607\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_8\">\n",
                             "      <!-- 0.00 -->\n",
                             "      <g transform=\"translate(20.878125 218.054826)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -571,15 +571,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-30\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_2\">\n",
                             "     <g id=\"line2d_10\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#mefb64c89f7\" y=\"179.581656\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m3b81b6d414\" y=\"179.581656\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_9\">\n",
                             "      <!-- 0.05 -->\n",
                             "      <g transform=\"translate(20.878125 183.380875)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 691 4666 \n",
@@ -614,15 +614,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-35\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_3\">\n",
                             "     <g id=\"line2d_11\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#mefb64c89f7\" y=\"144.907705\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m3b81b6d414\" y=\"144.907705\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_10\">\n",
                             "      <!-- 0.10 -->\n",
                             "      <g transform=\"translate(20.878125 148.706924)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -630,15 +630,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-30\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_4\">\n",
                             "     <g id=\"line2d_12\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#mefb64c89f7\" y=\"110.233754\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m3b81b6d414\" y=\"110.233754\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_11\">\n",
                             "      <!-- 0.15 -->\n",
                             "      <g transform=\"translate(20.878125 114.032973)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -646,15 +646,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-35\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_5\">\n",
                             "     <g id=\"line2d_13\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#mefb64c89f7\" y=\"75.559803\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m3b81b6d414\" y=\"75.559803\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_12\">\n",
                             "      <!-- 0.20 -->\n",
                             "      <g transform=\"translate(20.878125 79.359022)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -662,15 +662,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-30\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_6\">\n",
                             "     <g id=\"line2d_14\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#mefb64c89f7\" y=\"40.885852\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m3b81b6d414\" y=\"40.885852\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_13\">\n",
                             "      <!-- 0.25 -->\n",
                             "      <g transform=\"translate(20.878125 44.685071)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -792,37 +792,37 @@
                             "C 4.472136 -1.186024 4.000923 -2.323632 3.162278 -3.162278 \n",
                             "C 2.323632 -4.000923 1.186024 -4.472136 0 -4.472136 \n",
                             "C -1.186024 -4.472136 -2.323632 -4.000923 -3.162278 -3.162278 \n",
                             "C -4.000923 -2.323632 -4.472136 -1.186024 -4.472136 0 \n",
                             "C -4.472136 1.186024 -4.000923 2.323632 -3.162278 3.162278 \n",
                             "C -2.323632 4.000923 -1.186024 4.472136 0 4.472136 \n",
                             "z\n",
-                            "\" id=\"mfa355994e8\" style=\"stroke:#000000;\"/>\n",
+                            "\" id=\"ma60f5c3192\" style=\"stroke:#000000;\"/>\n",
                             "    </defs>\n",
                             "    <g>\n",
-                            "     <use style=\"fill:#ffffff;stroke:#000000;\" x=\"50.14375\" xlink:href=\"#mfa355994e8\" y=\"214.255607\"/>\n",
-                            "     <use style=\"fill:#ffffff;stroke:#000000;\" x=\"329.14375\" xlink:href=\"#mfa355994e8\" y=\"214.255607\"/>\n",
+                            "     <use style=\"fill:#ffffff;stroke:#000000;\" x=\"50.14375\" xlink:href=\"#ma60f5c3192\" y=\"214.255607\"/>\n",
+                            "     <use style=\"fill:#ffffff;stroke:#000000;\" x=\"329.14375\" xlink:href=\"#ma60f5c3192\" y=\"214.255607\"/>\n",
                             "    </g>\n",
                             "   </g>\n",
                             "   <g id=\"PathCollection_2\">\n",
                             "    <defs>\n",
                             "     <path d=\"M 0 4.472136 \n",
                             "C 1.186024 4.472136 2.323632 4.000923 3.162278 3.162278 \n",
                             "C 4.000923 2.323632 4.472136 1.186024 4.472136 0 \n",
                             "C 4.472136 -1.186024 4.000923 -2.323632 3.162278 -3.162278 \n",
                             "C 2.323632 -4.000923 1.186024 -4.472136 0 -4.472136 \n",
                             "C -1.186024 -4.472136 -2.323632 -4.000923 -3.162278 -3.162278 \n",
                             "C -4.000923 -2.323632 -4.472136 -1.186024 -4.472136 0 \n",
                             "C -4.472136 1.186024 -4.000923 2.323632 -3.162278 3.162278 \n",
                             "C -2.323632 4.000923 -1.186024 4.472136 0 4.472136 \n",
                             "z\n",
-                            "\" id=\"ma204b0ea55\" style=\"stroke:#000000;\"/>\n",
+                            "\" id=\"me0ded9ef49\" style=\"stroke:#000000;\"/>\n",
                             "    </defs>\n",
                             "    <g>\n",
-                            "     <use style=\"stroke:#000000;\" x=\"273.34375\" xlink:href=\"#ma204b0ea55\" y=\"214.255607\"/>\n",
+                            "     <use style=\"stroke:#000000;\" x=\"273.34375\" xlink:href=\"#me0ded9ef49\" y=\"214.255607\"/>\n",
                             "    </g>\n",
                             "   </g>\n",
                             "   <g id=\"text_15\">\n",
                             "    <!-- Hawk-Dove game replicator dynamics -->\n",
                             "    <g transform=\"translate(75.22375 16.318125)scale(0.12 -0.12)\">\n",
                             "     <defs>\n",
                             "      <path d=\"M 628 4666 \n",
@@ -1284,15 +1284,15 @@
                             "     <use x=\"1799.898438\" xlink:href=\"#DejaVuSans-63\"/>\n",
                             "     <use x=\"1854.878906\" xlink:href=\"#DejaVuSans-73\"/>\n",
                             "    </g>\n",
                             "   </g>\n",
                             "  </g>\n",
                             " </g>\n",
                             " <defs>\n",
-                            "  <clipPath id=\"p8ae3ec6857\">\n",
+                            "  <clipPath id=\"pb10e2db317\">\n",
                             "   <rect height=\"217.44\" width=\"279\" x=\"50.14375\" y=\"22.318125\"/>\n",
                             "  </clipPath>\n",
                             " </defs>\n",
                             "</svg>\n"
                         ],
                         "text/plain": [
                             "<Figure size 360x288 with 1 Axes>"
@@ -1402,15 +1402,15 @@
                             "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
                             "  \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
                             "<svg height=\"277.314375pt\" version=\"1.1\" viewBox=\"0 0 344.295312 277.314375\" width=\"344.295312pt\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
                             " <metadata>\n",
                             "  <rdf:RDF xmlns:cc=\"http://creativecommons.org/ns#\" xmlns:dc=\"http://purl.org/dc/elements/1.1/\" xmlns:rdf=\"http://www.w3.org/1999/02/22-rdf-syntax-ns#\">\n",
                             "   <cc:Work>\n",
                             "    <dc:type rdf:resource=\"http://purl.org/dc/dcmitype/StillImage\"/>\n",
-                            "    <dc:date>2022-02-02T11:27:54.469379</dc:date>\n",
+                            "    <dc:date>2022-02-16T15:38:23.374835</dc:date>\n",
                             "    <dc:format>image/svg+xml</dc:format>\n",
                             "    <dc:creator>\n",
                             "     <cc:Agent>\n",
                             "      <dc:title>Matplotlib v3.4.3, https://matplotlib.org/</dc:title>\n",
                             "     </cc:Agent>\n",
                             "    </dc:creator>\n",
                             "   </cc:Work>\n",
@@ -1434,15 +1434,15 @@
                             "L 329.14375 239.758125 \n",
                             "L 329.14375 22.318125 \n",
                             "L 50.14375 22.318125 \n",
                             "z\n",
                             "\" style=\"fill:#ffffff;\"/>\n",
                             "   </g>\n",
                             "   <g id=\"line2d_1\">\n",
-                            "    <path clip-path=\"url(#pcf4bc6fcd4)\" d=\"M 50.14375 212.903715 \n",
+                            "    <path clip-path=\"url(#pb30e65b7da)\" d=\"M 50.14375 212.903715 \n",
                             "L 52.93375 201.375601 \n",
                             "L 55.72375 190.240823 \n",
                             "L 58.51375 179.499063 \n",
                             "L 61.30375 169.149884 \n",
                             "L 64.09375 159.192726 \n",
                             "L 66.88375 149.626903 \n",
                             "L 69.67375 140.451594 \n",
@@ -1538,28 +1538,28 @@
                             "L 320.77375 222.202588 \n",
                             "L 323.56375 219.527756 \n",
                             "L 326.35375 216.4308 \n",
                             "L 329.14375 212.903715 \n",
                             "\" style=\"fill:none;stroke:#1f77b4;stroke-linecap:square;stroke-width:1.5;\"/>\n",
                             "   </g>\n",
                             "   <g id=\"line2d_2\">\n",
-                            "    <path clip-path=\"url(#pcf4bc6fcd4)\" d=\"M 50.14375 212.903715 \n",
+                            "    <path clip-path=\"url(#pb30e65b7da)\" d=\"M 50.14375 212.903715 \n",
                             "L 329.14375 212.903715 \n",
                             "\" style=\"fill:none;stroke:#000000;stroke-linecap:square;stroke-width:1.5;\"/>\n",
                             "   </g>\n",
                             "   <g id=\"matplotlib.axis_1\">\n",
                             "    <g id=\"xtick_1\">\n",
                             "     <g id=\"line2d_3\">\n",
                             "      <defs>\n",
                             "       <path d=\"M 0 0 \n",
                             "L 0 3.5 \n",
-                            "\" id=\"m0b9410b160\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
+                            "\" id=\"m8c8d0b0d67\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
                             "      </defs>\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m0b9410b160\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m8c8d0b0d67\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_1\">\n",
                             "      <!-- 0.0 -->\n",
                             "      <g transform=\"translate(42.192188 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2034 4250 \n",
@@ -1596,15 +1596,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-30\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_2\">\n",
                             "     <g id=\"line2d_4\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"105.94375\" xlink:href=\"#m0b9410b160\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"105.94375\" xlink:href=\"#m8c8d0b0d67\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_2\">\n",
                             "      <!-- 0.2 -->\n",
                             "      <g transform=\"translate(97.992188 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 1228 531 \n",
@@ -1637,15 +1637,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-32\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_3\">\n",
                             "     <g id=\"line2d_5\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"161.74375\" xlink:href=\"#m0b9410b160\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"161.74375\" xlink:href=\"#m8c8d0b0d67\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_3\">\n",
                             "      <!-- 0.4 -->\n",
                             "      <g transform=\"translate(153.792188 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2419 4116 \n",
@@ -1673,15 +1673,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-34\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_4\">\n",
                             "     <g id=\"line2d_6\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"217.54375\" xlink:href=\"#m0b9410b160\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"217.54375\" xlink:href=\"#m8c8d0b0d67\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_4\">\n",
                             "      <!-- 0.6 -->\n",
                             "      <g transform=\"translate(209.592188 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2113 2584 \n",
@@ -1720,15 +1720,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-36\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_5\">\n",
                             "     <g id=\"line2d_7\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"273.34375\" xlink:href=\"#m0b9410b160\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"273.34375\" xlink:href=\"#m8c8d0b0d67\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_5\">\n",
                             "      <!-- 0.8 -->\n",
                             "      <g transform=\"translate(265.392187 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2034 2216 \n",
@@ -1776,15 +1776,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-38\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_6\">\n",
                             "     <g id=\"line2d_8\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"329.14375\" xlink:href=\"#m0b9410b160\" y=\"239.758125\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"329.14375\" xlink:href=\"#m8c8d0b0d67\" y=\"239.758125\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_6\">\n",
                             "      <!-- 1.0 -->\n",
                             "      <g transform=\"translate(321.192187 254.356562)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 794 531 \n",
@@ -1855,18 +1855,18 @@
                             "   </g>\n",
                             "   <g id=\"matplotlib.axis_2\">\n",
                             "    <g id=\"ytick_1\">\n",
                             "     <g id=\"line2d_9\">\n",
                             "      <defs>\n",
                             "       <path d=\"M 0 0 \n",
                             "L -3.5 0 \n",
-                            "\" id=\"ma62f4a7818\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
+                            "\" id=\"m8b5a2169a7\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
                             "      </defs>\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#ma62f4a7818\" y=\"212.903715\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m8b5a2169a7\" y=\"212.903715\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_8\">\n",
                             "      <!-- 0.00 -->\n",
                             "      <g transform=\"translate(20.878125 216.702934)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -1874,15 +1874,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-30\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_2\">\n",
                             "     <g id=\"line2d_10\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#ma62f4a7818\" y=\"182.630074\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m8b5a2169a7\" y=\"182.630074\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_9\">\n",
                             "      <!-- 0.02 -->\n",
                             "      <g transform=\"translate(20.878125 186.429293)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -1890,15 +1890,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-32\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_3\">\n",
                             "     <g id=\"line2d_11\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#ma62f4a7818\" y=\"152.356434\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m8b5a2169a7\" y=\"152.356434\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_10\">\n",
                             "      <!-- 0.04 -->\n",
                             "      <g transform=\"translate(20.878125 156.155653)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -1906,15 +1906,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-34\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_4\">\n",
                             "     <g id=\"line2d_12\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#ma62f4a7818\" y=\"122.082793\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m8b5a2169a7\" y=\"122.082793\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_11\">\n",
                             "      <!-- 0.06 -->\n",
                             "      <g transform=\"translate(20.878125 125.882012)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -1922,15 +1922,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-36\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_5\">\n",
                             "     <g id=\"line2d_13\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#ma62f4a7818\" y=\"91.809153\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m8b5a2169a7\" y=\"91.809153\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_12\">\n",
                             "      <!-- 0.08 -->\n",
                             "      <g transform=\"translate(20.878125 95.608372)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -1938,15 +1938,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-38\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_6\">\n",
                             "     <g id=\"line2d_14\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#ma62f4a7818\" y=\"61.535512\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m8b5a2169a7\" y=\"61.535512\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_13\">\n",
                             "      <!-- 0.10 -->\n",
                             "      <g transform=\"translate(20.878125 65.334731)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -1954,15 +1954,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-30\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_7\">\n",
                             "     <g id=\"line2d_15\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#ma62f4a7818\" y=\"31.261872\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"50.14375\" xlink:href=\"#m8b5a2169a7\" y=\"31.261872\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_14\">\n",
                             "      <!-- 0.12 -->\n",
                             "      <g transform=\"translate(20.878125 35.061091)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -2099,37 +2099,37 @@
                             "C 4.472136 -1.186024 4.000923 -2.323632 3.162278 -3.162278 \n",
                             "C 2.323632 -4.000923 1.186024 -4.472136 0 -4.472136 \n",
                             "C -1.186024 -4.472136 -2.323632 -4.000923 -3.162278 -3.162278 \n",
                             "C -4.000923 -2.323632 -4.472136 -1.186024 -4.472136 0 \n",
                             "C -4.472136 1.186024 -4.000923 2.323632 -3.162278 3.162278 \n",
                             "C -2.323632 4.000923 -1.186024 4.472136 0 4.472136 \n",
                             "z\n",
-                            "\" id=\"maf8f208a74\" style=\"stroke:#000000;\"/>\n",
+                            "\" id=\"m891bceacd1\" style=\"stroke:#000000;\"/>\n",
                             "    </defs>\n",
                             "    <g>\n",
-                            "     <use style=\"fill:#ffffff;stroke:#000000;\" x=\"50.14375\" xlink:href=\"#maf8f208a74\" y=\"212.903715\"/>\n",
-                            "     <use style=\"fill:#ffffff;stroke:#000000;\" x=\"329.14375\" xlink:href=\"#maf8f208a74\" y=\"212.903715\"/>\n",
+                            "     <use style=\"fill:#ffffff;stroke:#000000;\" x=\"50.14375\" xlink:href=\"#m891bceacd1\" y=\"212.903715\"/>\n",
+                            "     <use style=\"fill:#ffffff;stroke:#000000;\" x=\"329.14375\" xlink:href=\"#m891bceacd1\" y=\"212.903715\"/>\n",
                             "    </g>\n",
                             "   </g>\n",
                             "   <g id=\"PathCollection_2\">\n",
                             "    <defs>\n",
                             "     <path d=\"M 0 4.472136 \n",
                             "C 1.186024 4.472136 2.323632 4.000923 3.162278 3.162278 \n",
                             "C 4.000923 2.323632 4.472136 1.186024 4.472136 0 \n",
                             "C 4.472136 -1.186024 4.000923 -2.323632 3.162278 -3.162278 \n",
                             "C 2.323632 -4.000923 1.186024 -4.472136 0 -4.472136 \n",
                             "C -1.186024 -4.472136 -2.323632 -4.000923 -3.162278 -3.162278 \n",
                             "C -4.000923 -2.323632 -4.472136 -1.186024 -4.472136 0 \n",
                             "C -4.472136 1.186024 -4.000923 2.323632 -3.162278 3.162278 \n",
                             "C -2.323632 4.000923 -1.186024 4.472136 0 4.472136 \n",
                             "z\n",
-                            "\" id=\"mb09e3edb3a\" style=\"stroke:#000000;\"/>\n",
+                            "\" id=\"m455a462a47\" style=\"stroke:#000000;\"/>\n",
                             "    </defs>\n",
                             "    <g>\n",
-                            "     <use style=\"stroke:#000000;\" x=\"273.34375\" xlink:href=\"#mb09e3edb3a\" y=\"212.903715\"/>\n",
+                            "     <use style=\"stroke:#000000;\" x=\"273.34375\" xlink:href=\"#m455a462a47\" y=\"212.903715\"/>\n",
                             "    </g>\n",
                             "   </g>\n",
                             "   <g id=\"text_16\">\n",
                             "    <!-- Hawk-Dove game on Finite populations -->\n",
                             "    <g transform=\"translate(72.000625 16.318125)scale(0.12 -0.12)\">\n",
                             "     <defs>\n",
                             "      <path d=\"M 628 4666 \n",
@@ -2547,15 +2547,15 @@
                             "     <use x=\"1845.240234\" xlink:href=\"#DejaVuSans-6e\"/>\n",
                             "     <use x=\"1908.619141\" xlink:href=\"#DejaVuSans-73\"/>\n",
                             "    </g>\n",
                             "   </g>\n",
                             "  </g>\n",
                             " </g>\n",
                             " <defs>\n",
-                            "  <clipPath id=\"pcf4bc6fcd4\">\n",
+                            "  <clipPath id=\"pb30e65b7da\">\n",
                             "   <rect height=\"217.44\" width=\"279\" x=\"50.14375\" y=\"22.318125\"/>\n",
                             "  </clipPath>\n",
                             " </defs>\n",
                             "</svg>\n"
                         ],
                         "text/plain": [
                             "<Figure size 360x288 with 1 Axes>"
@@ -2592,14 +2592,22 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "time spent as Hawk: 1.0 & time spent as Dove: 0.0\n"
                     ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/Users/eliasfernandez/PycharmProjects/EGTtools/egttools/analytical/sed_analytical.py:604: RuntimeWarning: Some of the entries in the transition matrix are close to 1 (with a tolerance of 1e-11). This could result in more than one eigenvalue of magnitute 1 (the Markov Chain is degenerate), so please be careful when analysing the results.\n",
+                        "  warn(\n"
+                    ]
                 }
             ],
             "source": [
                 "evolver.mu = 0\n",
                 "stationary_SML = evolver.calculate_stationary_distribution(beta)\n",
                 "print(\"time spent as Hawk: {} & time spent as Dove: {}\".format(*stationary_SML))"
             ]
@@ -2653,15 +2661,15 @@
                             "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
                             "  \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
                             "<svg height=\"271.127542pt\" version=\"1.1\" viewBox=\"0 0 350.102187 271.127542\" width=\"350.102187pt\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
                             " <metadata>\n",
                             "  <rdf:RDF xmlns:cc=\"http://creativecommons.org/ns#\" xmlns:dc=\"http://purl.org/dc/elements/1.1/\" xmlns:rdf=\"http://www.w3.org/1999/02/22-rdf-syntax-ns#\">\n",
                             "   <cc:Work>\n",
                             "    <dc:type rdf:resource=\"http://purl.org/dc/dcmitype/StillImage\"/>\n",
-                            "    <dc:date>2022-02-02T11:27:54.589209</dc:date>\n",
+                            "    <dc:date>2022-02-16T15:38:23.500831</dc:date>\n",
                             "    <dc:format>image/svg+xml</dc:format>\n",
                             "    <dc:creator>\n",
                             "     <cc:Agent>\n",
                             "      <dc:title>Matplotlib v3.4.3, https://matplotlib.org/</dc:title>\n",
                             "     </cc:Agent>\n",
                             "    </dc:creator>\n",
                             "   </cc:Work>\n",
@@ -2690,18 +2698,18 @@
                             "   </g>\n",
                             "   <g id=\"matplotlib.axis_1\">\n",
                             "    <g id=\"xtick_1\">\n",
                             "     <g id=\"line2d_1\">\n",
                             "      <defs>\n",
                             "       <path d=\"M 0 0 \n",
                             "L 0 3.5 \n",
-                            "\" id=\"m8c1e42a9cc\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
+                            "\" id=\"m5f0223af2f\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
                             "      </defs>\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m8c1e42a9cc\" y=\"227.764417\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m5f0223af2f\" y=\"227.764417\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_1\">\n",
                             "      <!-- 0.0 -->\n",
                             "      <g transform=\"translate(47.999063 242.362855)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2034 4250 \n",
@@ -2738,15 +2746,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-30\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_2\">\n",
                             "     <g id=\"line2d_2\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"111.750625\" xlink:href=\"#m8c1e42a9cc\" y=\"227.764417\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"111.750625\" xlink:href=\"#m5f0223af2f\" y=\"227.764417\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_2\">\n",
                             "      <!-- 0.2 -->\n",
                             "      <g transform=\"translate(103.799063 242.362855)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 1228 531 \n",
@@ -2779,15 +2787,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-32\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_3\">\n",
                             "     <g id=\"line2d_3\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"167.550625\" xlink:href=\"#m8c1e42a9cc\" y=\"227.764417\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"167.550625\" xlink:href=\"#m5f0223af2f\" y=\"227.764417\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_3\">\n",
                             "      <!-- 0.4 -->\n",
                             "      <g transform=\"translate(159.599063 242.362855)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2419 4116 \n",
@@ -2815,15 +2823,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-34\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_4\">\n",
                             "     <g id=\"line2d_4\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"223.350625\" xlink:href=\"#m8c1e42a9cc\" y=\"227.764417\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"223.350625\" xlink:href=\"#m5f0223af2f\" y=\"227.764417\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_4\">\n",
                             "      <!-- 0.6 -->\n",
                             "      <g transform=\"translate(215.399063 242.362855)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2113 2584 \n",
@@ -2862,15 +2870,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-36\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_5\">\n",
                             "     <g id=\"line2d_5\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"279.150625\" xlink:href=\"#m8c1e42a9cc\" y=\"227.764417\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"279.150625\" xlink:href=\"#m5f0223af2f\" y=\"227.764417\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_5\">\n",
                             "      <!-- 0.8 -->\n",
                             "      <g transform=\"translate(271.199063 242.362855)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2034 2216 \n",
@@ -2918,15 +2926,15 @@
                             "       <use x=\"95.410156\" xlink:href=\"#DejaVuSans-38\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"xtick_6\">\n",
                             "     <g id=\"line2d_6\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"334.950625\" xlink:href=\"#m8c1e42a9cc\" y=\"227.764417\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"334.950625\" xlink:href=\"#m5f0223af2f\" y=\"227.764417\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_6\">\n",
                             "      <!-- 1.0 -->\n",
                             "      <g transform=\"translate(326.999062 242.362855)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 794 531 \n",
@@ -2997,18 +3005,18 @@
                             "   </g>\n",
                             "   <g id=\"matplotlib.axis_2\">\n",
                             "    <g id=\"ytick_1\">\n",
                             "     <g id=\"line2d_7\">\n",
                             "      <defs>\n",
                             "       <path d=\"M 0 0 \n",
                             "L -3.5 0 \n",
-                            "\" id=\"m9049cab6e6\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
+                            "\" id=\"m679f87d7e4\" style=\"stroke:#000000;stroke-width:0.8;\"/>\n",
                             "      </defs>\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m9049cab6e6\" y=\"217.880781\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m679f87d7e4\" y=\"217.880781\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_8\">\n",
                             "      <!-- 0.00 -->\n",
                             "      <g transform=\"translate(26.685 221.68)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -3016,15 +3024,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-30\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_2\">\n",
                             "     <g id=\"line2d_8\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m9049cab6e6\" y=\"183.400521\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m679f87d7e4\" y=\"183.400521\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_9\">\n",
                             "      <!-- 0.01 -->\n",
                             "      <g transform=\"translate(26.685 187.199739)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -3032,15 +3040,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-31\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_3\">\n",
                             "     <g id=\"line2d_9\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m9049cab6e6\" y=\"148.92026\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m679f87d7e4\" y=\"148.92026\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_10\">\n",
                             "      <!-- 0.02 -->\n",
                             "      <g transform=\"translate(26.685 152.719479)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -3048,15 +3056,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-32\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_4\">\n",
                             "     <g id=\"line2d_10\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m9049cab6e6\" y=\"114.44\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m679f87d7e4\" y=\"114.44\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_11\">\n",
                             "      <!-- 0.03 -->\n",
                             "      <g transform=\"translate(26.685 118.239219)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 2597 2516 \n",
@@ -3098,15 +3106,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-33\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_5\">\n",
                             "     <g id=\"line2d_11\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m9049cab6e6\" y=\"79.95974\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m679f87d7e4\" y=\"79.95974\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_12\">\n",
                             "      <!-- 0.04 -->\n",
                             "      <g transform=\"translate(26.685 83.758958)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -3114,15 +3122,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-34\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_6\">\n",
                             "     <g id=\"line2d_12\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m9049cab6e6\" y=\"45.479479\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m679f87d7e4\" y=\"45.479479\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_13\">\n",
                             "      <!-- 0.05 -->\n",
                             "      <g transform=\"translate(26.685 49.278698)scale(0.1 -0.1)\">\n",
                             "       <defs>\n",
                             "        <path d=\"M 691 4666 \n",
@@ -3157,15 +3165,15 @@
                             "       <use x=\"159.033203\" xlink:href=\"#DejaVuSans-35\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "    <g id=\"ytick_7\">\n",
                             "     <g id=\"line2d_13\">\n",
                             "      <g>\n",
-                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m9049cab6e6\" y=\"10.999219\"/>\n",
+                            "       <use style=\"stroke:#000000;stroke-width:0.8;\" x=\"55.950625\" xlink:href=\"#m679f87d7e4\" y=\"10.999219\"/>\n",
                             "      </g>\n",
                             "     </g>\n",
                             "     <g id=\"text_14\">\n",
                             "      <!-- 0.06 -->\n",
                             "      <g transform=\"translate(26.685 14.798438)scale(0.1 -0.1)\">\n",
                             "       <use xlink:href=\"#DejaVuSans-30\"/>\n",
                             "       <use x=\"63.623047\" xlink:href=\"#DejaVuSans-2e\"/>\n",
@@ -3449,15 +3457,15 @@
                             "      <use x=\"955.029297\" xlink:href=\"#DejaVuSans-69\"/>\n",
                             "      <use x=\"982.8125\" xlink:href=\"#DejaVuSans-6f\"/>\n",
                             "      <use x=\"1043.994141\" xlink:href=\"#DejaVuSans-6e\"/>\n",
                             "     </g>\n",
                             "    </g>\n",
                             "   </g>\n",
                             "   <g id=\"line2d_14\">\n",
-                            "    <path clip-path=\"url(#pb8ca7eb8b3)\" d=\"M 55.950625 217.880781 \n",
+                            "    <path clip-path=\"url(#p9a2c419453)\" d=\"M 55.950625 217.880781 \n",
                             "L 58.740625 217.880781 \n",
                             "L 61.530625 217.880781 \n",
                             "L 64.320625 217.880781 \n",
                             "L 67.110625 217.880781 \n",
                             "L 69.900625 217.880781 \n",
                             "L 72.690625 217.880781 \n",
                             "L 75.480625 217.880781 \n",
@@ -3575,15 +3583,15 @@
                             "    <path d=\"M 55.950625 10.324417 \n",
                             "L 334.950625 10.324417 \n",
                             "\" style=\"fill:none;stroke:#000000;stroke-linecap:square;stroke-linejoin:miter;stroke-width:0.8;\"/>\n",
                             "   </g>\n",
                             "  </g>\n",
                             " </g>\n",
                             " <defs>\n",
-                            "  <clipPath id=\"pb8ca7eb8b3\">\n",
+                            "  <clipPath id=\"p9a2c419453\">\n",
                             "   <rect height=\"217.44\" width=\"279\" x=\"55.950625\" y=\"10.324417\"/>\n",
                             "  </clipPath>\n",
                             " </defs>\n",
                             "</svg>\n"
                         ],
                         "text/plain": [
                             "<Figure size 360x288 with 1 Axes>"
```

### Comparing `egttools-0.1.9.dev3/docs/examples/normal_form_game_mc_simulations.ipynb` & `egttools-0.1.9.dev6/docs/examples/normal_form_game_mc_simulations.ipynb`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/examples/plot_invasion_diagram.ipynb` & `egttools-0.1.9.dev6/docs/examples/plot_invasion_diagram.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977437444885362%*

 * *Differences: {"'cells'": "{16: {'outputs': {0: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAAmMAAAJfCAYAAAAzcNGrAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjQuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/MnkTPAAAACXBIWXMAABcSAAAXEgFnn9JSAAEAAElEQVR4nOydeZxN9RvH38/MGLtEsiQi+15CUlJKC0ppoQ1JQiFbkS3SRqVNhaxJmxKJUtYW+8+uDVlSZN9izMzz++N77hjMcu+de+fc5ft+ve5r5pz7Pec8d+aec57zfJ/n84iqYrFYLBaLxWJxhxi3DbBYLBaLxWKJZqwzZrFYLBaLxeIi1hmzWCwWi8VicRHrjFksFovFYrG4iHXGLBaLxWKxWFzEOmMWi8VisVgsLmKdMYvFYrFYLBYXsc6YxWKxWCwWi4tYZ8x […]*

```diff
@@ -192,15 +192,15 @@
             "cell_type": "code",
             "execution_count": 11,
             "id": "248391fa-55f6-409f-ab67-f16bc866c616",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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A0BVFwDdcW3DduJSBI7zzr8sZ5ziBs24APiQ8HHEwD00zYkbNKO834bkh4hzxrypyadxkhXhyEMresiAzCtEpKSIJOL0UurjKra64NoZRbV2SoTj59S34SqiewL9vZvCUFwlWJb06dOHzZs389BDD/H000/zzTffMGbMGAD27t3L+vXr2bdvX35yydbk037jSArznLLzN0C8xuMTcYVkX+GKl3oDXUTkqMxj4wbNOAs3NRmOSvuNgI/iBs0ozIf2oBBxzhhO/qGf30bkwtMresgFACLSDliGm5uPA6YAdVT1TYuGhZZJkybRu3fvXMfNnTuXpUut8CoM+RSn+Va1R48efYDrshv47rvvsnLlShITE3nooYfo27cvl19+Ob/++iu33347tWrVon379txzzz2sXLkyr3YEVUvQMMIVVf3L6/BSDefM1gcmi0h3EZG4QTOq4mSFSvhpZy6cgUtniCgiyhlb0UNq4JSyw55U5ZXKJWQCMAfXImID0FFVr1PVf/y1LjaYMGECZcvmrvc7bdo0hgwZkus4o3BR1R04IU+6d+9+Lzlcr9566y06duxInTp1AChSpAhnn302//d//8eSJUu4//77qV+/PmPGjGHUqFGkpgacjz8PWFuwT2IYkYUnq/QSTmKmNHAjyDg9sGcyThIj3OkaN2jG5X4bkRcixhnzpidfwX0xwp44ofodTdKnUl8C6qnqRz6aFHP88ssvtGzZ8pB1GzZsoE+fPofkDZ111lksW2aSbmHKhLPOOiu+ffv2x2U3QFUpWbIkK1euPGQK8plnnuGSSy7h/fffp1+/fnzwwQc8+OCDvP7662zYsCHQ448qoP2GEZGo6lZcsdlrwAGaXHymFCt1TgRN6LwYN2hGRb+NCJSIccZwFVTn+m1EoKjCVSfB8Fbco6p9vM72RiGyc+dOqlQ5VH9wy5YtvPzyy4dERqpXr87WrabvGo6o6q6xY8fmmIgtIlSrVo1vvvmGZ555hrfffptbb72VZcuWcdddd1G5cuV057tx48Ycf/zxrF4dkILM18BnBf8URm6sXr36iAeizz77jNatW1O6dGnKli1Lhw4d+O677DqaGaFAVVNU9VVaXjWEs7vXAoKh31dYVMH1d44IIsIZW9FDKuPan0QMad/Xq07i9hU9pLA0kYxMlC5dmn/+OXRGeMsW145tx44d6ev27NlD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eDKWnu7BTtfViefKIlLop+lly5bxzjvvcO+99zJ+/Hjat2/PjjvuuNkLfLAVtip3e8lDd4mkquuBd0XkN+BmoAmwA1ZT9lyUsWWx47G/+7hWw1avXk2VKlWoUaMGO+64I0cddRStWrXaWNu1dOlSatSowYknnsj69es3rnzFTlLC5l36RYRDDz2U9evX07VrV1q2LNEgh6sAH5sVAVX9TER+B4oeLuoyR9SNzvyrxF/XajE8++yzescdd+iqVas2fm/58uU6atQobdeunYqI7rPPPvroo4/qr7/+quvWrSvorhaoas0U+P3j+iINm76W4nethtUVKtYG5R2sCFuiji2Lvlqo6kqN0+2336433HCDzps3T1VVFy1a9K/r9OvXTytVqqRt2rTR5s2b69ChQ3Xp0qWqqhufp2+88YZecMEFumLFClXVeBs6FxiWqqbEvxmyrOkr0AqoEXUc/lX2X17An77uB+bFe+XJkyczYMAApk2bxpo1a3j77bc5/vjj6dKlC8uXL+f+++/nmWeeoXv37jRp0oQKFSrEXhzyqoN1g3ap53SgHrAI+AqbaXoI0FVEakQZWBZ5ljgOunz44Yc0atSIp556irVr1/L779aPt1atWoAV4c+fP58GDRowfPhwrrvuOs4880waNWpEv379NpYQxFbJBg0axPDhw3n77beBYjV13tSfwNHAtUTcXywbicgeWKnBZSLih6WyTdTZoH+V6utKLYb69evrSSedpEceeaSKiDZv3lzvuece/emnn3Tt2rXFuavFqlo7BX7/Ir/IkpUxrA/czPC79sGKxw/DTsFejp26bAmUizrWDP7aSuMwbtw43XnnnbV37946bdq0jatcqv8eVTRw4ECdNm3axpWuFStW6KGHHqqNGjXSGTNmbLz+77//rg888EA8D1+QBzUFV7zJopUxrI/kWODyqGPxr7L/8pqx9PYw9sa7XTxXHjx4ML169aJJkybccccdHH300ey8884bh4YXRPVftWNbAv/B3uhdajgP6wf3N/Cgqm4AxojIN1gidiDQDmglIp+o6rToQs1YzeK50vPPP8+2225Lnz592GGHHQBYtWoVVatW3fg8W7duHRUrVmTQoEEbb5eTk0O1atU46KCD+Prrr6lRowYiQk5ODg0bNqRXr14liXkaNmHjk5Lc2CWGiOwD7IkdnHgz4nBcBHybMr2tAm6J98oXXXQR2267Lfvuuy89evSgadOmRSZio0aN4rLL8p0idAVQvzjBuuQIWxqxxPhWVV0Z+5lajd9sYDFW1L8f8JCIXCoiFcs82Mw2uagrLF++nM8++4z99ttvYyJ27733csIJJ9C5c2euvfZalixZQsWK9r8mJydn423LlSvH7Nmz+eijjzj44IM3bmmWcEsyB7gDO3nriVj0Yk21v1DV6ZFG4iLhyVj6exwbJh2XAQMG8OKLLzJ16tS4rl+xYkUefPBBfvvtt7w/qg5cE3eULpkuxFZHYwPl/0VVJwIPYh35K2C1KU+JyN5lFGM2mAsU2Zl1xowZ1KpVi3Xr1rH//vtz0003sdVWWzFnzhzuvvvujaOLIDfRysnJ4e+//+bhhx9m1qxZdOvWrdCJGkX4HtgXqw3zE3sRE5GDsHYW67HWQS4LeTKW/taQ2229SBdeeCG77bbbxpl1RenUqRNHHnkkV1xxRX4/vgSbteciIiLVsf5vADdrIcPDVXUJtqJ5H9YrbjvgLhG50FfJEubuwn5YpUoVWrRowcsvv8wHH3xA9erVGTNmDE899RSffvopDz/8MKNHj2bkyJGsXGkLnKNGjeL555/nhBNOYNiwYdx6662cfPLJJYltLTZntg3wdUnuwCVWGGXWI1z8TFV/jzIeF6Goi9b8KyFfFVX1V02SDz74QEVEp0yZkt+PhyXx9yr1FxlewI+tTsZaWVQsxu3qA3diBcO3AZcB20f9+2TAVzlVHaeFGDJkiFaoUEFr1Kihp5566r9+fvLJJ2vjxo118eLFumjRIm3durXutttueu655+qyZcsKu+vCfK6qTSP8eynRFxlewA/sCjyDTc7YLup4/Cu6L18ZywzrgEHFucH69esBYi8IQG59yoYNGza7bocOHTj22GO58sor87urC7Emo66MiUhNbKsJ4EZVXRfvbVX1H1XtE27/D1AbyBGR5iJSOfHRZo0crCB+bUFXuOyyy9hqq61YsWIFe+xh4x83bNiw8bl42GGH8ddffzFz5kxq1arFM888wyuvvMITTzxBjRrF7lCyEjtN2w4bUu5SSy3gZ+zD4l8Rx+Ii5MlY5nieYnTMjtWbbHpKMlafEhuPtGTJEgBmzZpF586dee+995gy5V+v55XwU5VRiU1hmIr1tyo2Vf0aO1L/Enbq8iSgl4i0TlSQWegnChlXVr16dZ5++mkAXnrpJWbPnk358uU3PhcnTpxIo0aN2HlnG0+4++6706xZXAc183ofO+E5DDul51KMqo7H/v98EHUsLlre2iJzbMBWx16M9wYrV65k8eLFTJ8+nfLly/Pbb7/x+++/s2bNGr755hvWrFnDX3/9xZw5cza+UQwZMoSRI0fmvase2CiePxLzq7iiiEhtrL0IwEC1sUgloqqrgZ9FZEesYWwDYKiIjAeGqs+3LImhwKnkzgndTMeOHenTpw933nknl112GVdddRUNGjRg/PjxjB07ltNOO41q1aqh+q+2MvFYjI0zehJv3pqSQq3YUcAktdPOLst5MpZZXsFOSu0Vz5V//vln2rRps3F2ZWybsmbNmlSrVo3q1auz2267seuuu7LTTjvRsGFDKlasuNlMvKACtjUzMMG/jyvYf7B+bz9iq1qlpqq/i8hDwEVAa6wNxlMi8ijwpm66p+2Ksg77kDIea8D7L4MHD6ZWrVoMGTKE0aNHs8suuzB9+nTOP/98brkl7o41m5k3b96HW2yxxVlVq1adU/LQXRk4FOgEtBCR/9NCDt647ODJWGbJAQYAo+K5cqtWrbjllltYsGABrVu3pkqVKtStW5emTZuyYMECdtttN3JycsjJyYnnGL1va5UREamPbVGCrYrlFHb94lDVtcAwEfkcayi8DbbK0k5EBqvqskQ9VqYTkZ9ee+21CV26dNkvv59XqVKF66+/nk6dOjFt2jTmz59P+/btadEi38W0QqnqvAEDBnx6yy23VFTV3VXVk7EUJSLlgQuArYGRnog5CAOEXUYR7NN4m3iuvH79+kITrdgqWD6rYXlNw04GpRQRGYwd579fVfPtXptuRGQolih9C7RO1oqViFQCegGdgV+wfnbvqOqkZDxeJgm9ox6vUqXKrt999x277bZbMh/uaeAqEbkIG4E1C+iWCSuZInIStuL/qaoeHHU8iSAiJwK9sR5vp6u1nHFZzgv4M49iyUdcYolY7ARl3tfvWAIWR5dv7xpdBkRkG6y/G0D/ZL7hqupaVb0HuBhL/KoA1USkcahZc3mIyBYicj/wKbDr6tWr57zwwgvXJ+nhZmF1R92ABcBj2CnOhsDhSXpMVwphVezMcHG0J2IuxpOxzPQ/4PPi3CB2grIExcIxr5b0hq5Y+gJVgS+Bt8viAVV1KjbpYRRWk3gyduKyY3hzcYCIHInV8MWS5ceApgMHDhyCTT9IpPuxk5Lvxr6hqnOBMeHiOVKKJ7NLmlOAeljT5SejDcWlEk/GMpNStu0mPsQaF7okEpEdsOJ6SPKqWF6qmqOq32F1pv8AlbFDBI+LSNOyiiMViUhdEXkKeAdblZoBdFLVnqq6OFytL4k5bfwL1jPsMiC/+r0RwGpge+DYBDyeS5Aw5eK0cPG/qroiynhcavFkLHN9GL6S7X2spshn3CXfDVhft0+wzvllLmyrPAV8gb1+NMIK/ntn20glMadgzVTPwT4E3Q00V9W8/3+WYg2SS2oDMATYG/isoCuFNiT/CxfP8pXLlNIS+yDzD/Cv/kAuu3kyltnirh0rgZnYG9AR2JK7SyIR2Qk4L1ws01WxvNS8E+L5EVstOxFrg9EoqrjKkohsC7yGtRXZCkvIDlDVqwpZ8XiHkr0JfwfsA1yPrXoVZQTWeR9gzxI8nkuOlVi3/aGq6h9e3WY8Gcts49ikpiRBZmNbZbthbywJa6vgCtUfS3rGqOonUQcDEJpVXgbcgyXkAnQTkcMzdUUmrIb1wLrsnwCsx+aftlLVL+O4iyuBuXE+3BosAdsH+CbeGMPq5Y3ArViy7FKAqv6IddufGHUsLvV4Mpb5BiTofuZiva12Bh6hkNl7LrFEZFdsFRKSu9pZbGGVbBQW33+xhKw+UCPTVslEpDHwHnaYYUvgaywJG1iMXlELgK5YEleYz7EtySFYA9liUdWvVPX7RPagcyUjIhVFpIeI7AXkqKqPpnL/4slY5puAvUmWyPz58xk6dOjPwE7Yp7p4tklcYg3CnqujVfWriGPJl6ouUNUXgOeA0Vjx+Lki0kVEtow2utIRkfIicjm2ytQJew70AfZX1R9KcJfvAx3If4VsAXYasx22pVUqIlJPRI7Ntnq+FHMW0Bbruu8nXF2+PBnLDgMo/oy6Jb/99ts9O+2004ZrrrlmdxEpfltwV2oi0gw4PVxM1Cpn0oQ2GMuBWP+kU4GnRSQt+16Fk6KfYVux1YCPsQL9u0ozDzTcZwus7u5RrFVFF6Ax1gaj1CtaIlIOuBbbSj69iKu7JBCRLbB2FnsAs3xVzBXEk7Hs8D3wcJzXXY4N/W7cpEmTK5ctW/ZU+P5NSYnMFeVG7NP0q6r6bdTBxENVN6jqaGyVrCK2pXe9iAwNo5xSnohUEpH+WLPb/bA2EhcCh6rqrwl6mLlYsf2FWMI0ivzbVZRI2KKcgrUhOVlEKifqvl3czgWqA/MoxQ6Fy3yejGWPK4E3Cvn5KuAO7JN5f2BR+P5NWM1KRxFpn8T4XB4i0hI7paik4RD2sEp2NnaIJAfbqnlSRNqnckNSEWmDbe8PxlqJvAU0VdVH07AG6zlgMZYQd402lOwSplQcHS4+56tirjCejGWPNdhy+e3YGBWwN/mZWJHwTtiWxvxNb6SqM7FO4gA3pfKbaAYaHP58QVUnRxpJCanqKlW9Daux+gtb5TsUOF1EakQaXB4iUlVE7gC+AvbCngtnAp1V9c9IgyuhcLDg5XDxBBGpFmU8WaY7Ni3jb3xVzBXBk7Hssha4DmvU2QRbPm+MHZ//u5Db3YIlcwdhg4hdkonIflgRfA5WwJ/WVPUbbIbiA9hKawMgR0T2TIUEX0QOwbbzr8ZeF5/DVsOez4CB2y9hBwO2IPdUrkuisCp2RLg4MgP+Dbkk82QsOyk22DuuxoOhn9RD4aKvjpWN2KrY02G7L+2p6jpVfQtrjfIqVsB+CtabbMcoYhKRmiLyEPAR1rZlNnCcqp6lqv9EEVOiqeo6LCED6ByKyl1ytcF60U2mjGbIuvTmyZiL121YB+l98Jl3SSUiB2MrkLGGohlFVeep6nTs91uH/ZsaLiIXlGWzWBE5BnuzjM37fATYU1XfLKsYytArWKI5F1sVd8k1FVtpvcdXxVw8PBlzcVHVucB94eLgcGzeJVhYdYydXH1cVWdEGU8yqeoErI3DBqxQ/kzgCRFJ6gif0HvrGawfWgPgN+yU5EWhe33GCcXjN2CjtL6LOJyMJiIVVPV34AkgUSdvXYbzN1RXHEOxo/d7Y6f8XOJ1BA7G6vtuiTiWpFPVRUBvrNfWKqAhNni8p4hUSORjhVFGp2PbR2dh9Xh3Anup6oeJfKxUpKozQ8mBSxIRqQlcJSKHAuKrYi5enoy5uKnqAqz5JcCNmTp/MCphVezmcPFhVf0jynjKShip9BzQA5iEvS7tClwgItsl4jFEZHusj9fzQD3gB2A/Vb1aVVcWdttMEhLS3UTkYhGpE3U8GehybDh7E4rfaNtlMU/GXHH9H9a3qClwWrShZJyjgX2xFaIhEcdS5lR1DnAF1uduHrAVUFlEdhGRSiW5z5B89MSanx6H1agNBNqEbdJs1B07ONEz6kAySZjF2h7YEZjsq2KuODwZc8WiqouxrR2AQYneSspWeWrF7lfVwlqNZKywSvYZ1gJjFDYH8gzg4jAaKm4i0gQYi22B1sT6h7VU1cGqmpWD7kOC8AH22t9RRLaOOKRMcgFQHvhZVT+POhiXXjwZcyUxDGuIuQvWYd2VXhegJTaO6o6IY4mcqq4MheaVsDrFbYF7ReTmogaPh8HeV2FbkR2wlcargAPTtXlugo3Bmj1XwlfHEkJEdsbGZkFuk2zn4ubJmCs2VV2GdfIHGFDSLSRnQu1drIXFvao6v7DrZ5NwKu1BrHt/eazx8EgROTK/64fVs8+Bu7Du5x8AzVT1bh9HY8Lq2JPhYvtQT+dK50Ls/fRHVf066mBc+vFkzJXUg1jX/kZY4bUruVOxot8lWBLhNqGqa1R1GDYp4h9sy/E6EblNRKrDxsHeA4FvsL5lS7FVn06hp5nb3MdYS48K2PaaK6FQK9YqXBweYSgujXky5koknEC7NVzsJyJVoownXYWau0Hh4l2h1YPLR6jDOQcb3L0BqAtcKiJnABOxv8eKwBvYKKPHvIg6f+Hv5fFw8aCoJiBkiLbYYPn/qeqkqINx6cmLr11pDAeuwRpnXgjcG204aeksrI3DAvzvr0iqugoYKiLvYifXzsBOoJbD6hgvAV72JKxoqvq5iHyNbf9WjzqeNDYGm937ZdSBuPTlyZgrMVVdLSI3YWNk+orI8Gzq2VRaIlIRa7MAcIeqLo0ynjRTD2uDsVO4/DXwLjAnqoDS1K3AWlVdHnUg6UhEaofV7DeijsWlN9+mdKX1BDAD2BpblXDx6w40xnpqPRBxLGlBRLYUkUexwvydgD+Bk4GHsY761wCPhdNtrgiqujCWiHkT5+IRkYbA5SJycmhN41yJeTLmSkVV15F7EvBaEdkiynjSRaix6x8u3qqqK6KMJx2ISGeseWusHcND2GDvV7EPBV9h7RqaAA+JyEWeYBQtNMY9AJs5u1vU8aSRvtjBm8q+Le5Ky5MxlwjPAFOxgurLI44lXfTEau1mY9u8rgAiUl9Ense2grYDpgGHqGqv2Nauquao6tvYycCfsUL+04EnvTi9cCGROAw4ELgo4nDSQkhe9wDqAOMiDsdlAE/GXKmp6npyTwT2EZHaEYaT8kSkGtamAeAWVV0dZTypKqzYnIkN9j4dO0F5O9BCVT/J7zahL9nF2KrZKqzXWDcROdRXyQr1MrbN21JEmkcdTCoLW5LnhYufqerMCMNxGcKTMZcoLwI/Alti3c5dwXoB2wC/k9tewG1CRHYA3gSexVZcJwH7qup14URlgcJIpRexmrw3sNe5nYAq4X5dHqo6BWsPAt53rCgHY1vh6/G+Yi5BPBlzCaGqOeSeDLxCROpFGU+qCjV114aLWTsjsSAiUk5ELgImA8cAa4F+QFtVnVjojfNQ1b9V9WngJeC/wBFADxE5JtYs1m3mEWx1rLmItIk6mFQUVsW6h4sfq+qfUcbjMocnYy6RXge+BWpgp9rcv12GtWX4FXg64lhSiojsgp2SfAjYAvgC2FtVbwkHRUokrPoswBINAU4DnhGRDqWPOnOo6q/YIQiA86OMJYW1xOoW12ID6J1LCE/GXMKEQuDYCcFLRWSbKONJNSJSC7g6XBwUau2ynohUEJGrge+BQ4CV2EGQdqr6UyIeIxT4jwJewD4s1AYGisgtXuO4mUew2rzdRGTviGNJRXtgCevTqjo36mBc5vBkzCXa29iLVVXguohjSTVXArWw9gwvRBtKahCRvbAVsDuAKsD72GDvYckY7K2qP2MjlcZiK2UHAk+LyMGJfqx0FIrR38D+frzdyr+9hL3GvRZ1IC6zeDLmEiqsjvULFy8WkQZRxpMqRKQulowBDExGopFORKSyiAzGisbbAIuxgfOHq+qMZD62qi5X1ZuwE63zsN5kh4vIqV5LBtjq2BBVnRZ1IKki1DLuBqxX1S980ohLNE/GXDKMBT7B3uRuiDiWVHE1Vgc1iSz/VC0i+wHfYFvaFbBaw6aq+kRZNs9U1S+Bs7Han7XYCbkKIrJzNndUV9XVsQ8LIlIrm/8uNrEvNgf1XP/7cMngyZhLuDy1Y+eLSOMo44maiGyNFe4D9A8nT7OOiFQXkbuBz4GmwFzgZFU9UVUjmSmpqmtCB/9HgVFAI6ArcFa21zyKyDHAECCrDzqE/nRXAW2BBd5t3yWDJ2MuKUJTzjHYykf/Iq6e6a4DqgHjgdERxxIJEemE9aG7AjvR+BS2GvZqlHHFhDYYPwGVsf5RbYGnRCSbV0J2xwrWe2Tx3wHY7NP64b8/jDIQl7k8GXPJFEvCzhGRXSONJCIisj3WER5gQLZ9qg7bXI9jiXkjYBZwpKqeq6oLIw0uH6o6Hhs6Xh5LzM4FHs/Sf79PAWuwsV1HRxxLJESkInBquPimqi6LMh6XuTwZc0mjql9hK0HlyW0Im21uwN7UPwPeiziWMiUiJ2AnR3uEb92PnZT8X2RBxUFV52Pbyk9gychOwAMi0iObRiqFv4fY/6uzs3R17FRsAsQyYGTEsbgM5smYS7YB4c8zRGTPSCMpY2FAdax5Zv9sWRUTka1F5CWsMH9b4BesZ9hl6bKyEEYqPYWNBpqCDR5vjtVAZlMt2RPYjM9tgOMjjqVMiUhl4JRwcZSqeqsPlzSejLmkUtVvsdODAtwYcThlrT/2Jj5WVT+KOJakC4O9z8aSl1Ow5qFDsC76n0UaXAmFweOXALcAf2PJZR0RaSgiFSINrgyo6iLgnXDxzGxaGcR60JUDlgDPRByLy3CejLmyMBBQ4KRs6eotIjtj9UaQBQcYRKQh1gzzaaAO8B02T/J6VV0dZWylFVbJxgAPYNt2f2MtMS4KI5wy3RPYVIQ62JDsbLEV1oLl/1R1TdTBuMzmyZhLOlX9kdyO84OjjKUMDcRq5d5R1S+iDiZZQjPMS7DB3kdiNVbXA/uEVdGMEZrFfoH1i1uDrZLdLyIDwgD4jBS2lh/DnsNTIw6nLL0IPIvVezqXVJ6MubIyCBs/01lE9o04lqQSkabAWeFixq6KhY7kH2OF+TWAcdiW5JDSDPZOdWHr8gFgPnY441BgpIgcGmlgyfW6qj6mqrOjDiTZRKSSiLQDKqnqtGyfluHKhidjrkyo6lRsCwsyf3VsEFYjN0pVJ0YcS8KFwd7XYdMEDsJmGF4GHBxmP2Y8VV2lqndjK6CLsJmjA0TkVhGpGmlwSRA7fBLqAptkeL3cccAR2Fa0c2XCkzFXlgZjDTUPD588M46ItMCK15Xck6QZI9T8fYUV5lfGaqj2VNX7s3GygKp+jHXsH4Ot/G4HXBpWRzPRmdiHjTMjjiMpRGRL4Dxs/JHP5nRlxpMxV2bCAOjHw8WbMrRvUWzV7yVV/SHSSBJIRKqIyC3A10ArbDWoG3BU2LbLWqq6QlVvAa7B/n6qAzuJSL0MrCUrD+wAnJKJK4BAd6AqsBCvFXNlyJMxV9ZuwYYyH4LV2mQMEWmLbXHkYKsHGUFEDsROR16PvRm/Auyhqk9nS++0eKjq11j3/rHAB9gYnUtEZJ8M+uDxPJaIb0GGbeOJSF3sEArAM14r5sqSJ2OuTKnqH8Aj4eLNGfQmBXBT+POZTKidEpEaIjIM+BTYDWvpcJKqnqKqc6ONLjWp6npV/RRLWnOAKkBf4KHQBDithYMZL4aLx4tI9SjjSbAe2P+v2WTpDFkXHU/GXBSGYF299wOOijiWhAirR0dgjU7T/oCCiByODfa+DDuM8AQ22Pu1SANLE5u0g5iAnTTdHRieISOVXsZOklYnt5deWhORrYHDwsWRvuLryponY67MqeocrDUAZE7tWGxV7AlV/S3SSEpBROqIyBNYYf6OwEzgcFXtEbqxuzipao6qvgVcBPwKVALOAR4LTXLTUti+ez5cPDYUvae7/bE6sZnkzuN0rsx4MuaicgewHCsGPyHaUEon9JfqgNXC3VTE1VOWiJyEjTI6FzsNei/QPHSfdyUUkvOe2OGV1Vgn+24icnAar5KNAuZi/04yofZzPfATcKuvirkoeDLmIqGq/2Bv9gCDRSQt/y2GVb1YAjZcVWdFGU9JiMg2IvIKVpi/NfamdKCqXqGqy6ONLjOEkUojsbYJo7Gasr2ASiKybaTBlUBYHbsTeBA7sJDWVHU0MAxvZ+EikpZvgC5j3IUN4W0GnBpxLCV1BHAAtuJxa8SxFEto4HkulnydhK0O3Ay0zOQRTlEKHewfA17FVpcOAXqKyGHp1ipCVSeo6mhVXRp1LCUlIrVE5EQRqaeqi3xVzEXFkzEXmVCDdFe4OCjdunrnWRV7UFX/ijKe4hCRRlhtzBNY9/iJQBtV7e9DkZMrrJL9gJ3aq469Dp8OPC0iB0QaXAmEiQz7pmlPte5k0EEil748GXNRuxcrnN2N9OvqfRzQBhsHdHvEscQlDPa+DDspeRi2onctsJ+qToo0uCwTkrJXsVYRdYD6wK0iMijNEpseWMPby6IOpDhEZCfgWKAtkFFD7V368WTMRSpsccQSmYEiUjHKeOIVatxiq2LDVHVelPHEQ0T2wHqGDcNWZD4FWqjqHaq6PtLgspiq/oQdmvgkfKs9Nnj8oKhiKqZfgbpABxHZLupgiuFCrHZviqr+GHUwLrt5MuZSwQPAPGAn0qdv0clAc2ApVsicskSkoohcj3XRPwBYBvQC2ocB7i5iqrpEVQcA/YEFWG+yo0M9U7VooyvSh8B0oCJ2ajTlicju2IoYWA2fc5HyZMxFTlVXYI1gAfqLSOUo4ylKaEdwY7j4f6q6MMp4CiMirbDGo7dgfa7ewQZ7P5SNg71TXeje3xWr5VsD7AlUF5EdUrUfXyh6HxEutkuTSQM9sfe/SarqW5Qucp6MuVTxMFbQvAOp/+n6TKyj+iLgnmhDyZ+IVBWR24DxQAtstaUrcEwYSeVSlKquUtVnsb5kbwG1sZYYp4tInUiDK4CqfgZMBSqQ4s9fEWkOtMbGVT0acTjOAZ6MuRShqqux1RuAG1J1aybUtA0MF4eq6pIo48mPiLTDtiSvxWpiXsRGGT3rR/fTh6r+qarfYMnYBuywyLMicmaKrpLFtvv2D8XxqaoFtq36lapOjjoY58CTMZdaHgd+B7YBLo44loJ0A5oA/wD3RRzLZkRkCxF5ACsE3xWYA5ygqqenwwEDlz9V/QpbwakCVAUuAB4RkcaRBpaHqo4HJmMrxm2LuHokQhI7E/iZ3LY6zkXOkzGXMlR1LblDtq8TkRpRxpNXqGXrHy7elkrd6UXkKOyNsFf41mPYath/o4vKJYqqzgV6A89hY7d2xRKybik2vWIIMBRrapuSwpbq/6nq/KhjcS4mlZ7EzgE8jR2Vr0fq9S06D2iIrTg9FHEsAIhIXRF5Gngbq7ebDnRS1Z6qujjS4FxCqeoGVX0UGzw+DTuQ0QY4T0S2ijS4IGytflXSVimhD15bETk0zHxtFn60Zex74avYtXNhOHtPEdnFW7m4VJNWHc9d5lPV9SIyCHgGuFpEHkyFuqwwqqZfuHiLqq6KOB4BTgHux5qF5mCHCQaE06kuQ6nqdBG5AOiMnbbcHmgYVsj+CXMjIyUiNYGDgcmqOqMYNz0TGJnP9/di8xmYX1P8rdDLsQR2Dj6D0qUYXxlzqegFYApWuHxlxLHEXARsC/xBxH2JQmPN17DC/PrY39UBqvofT8SyQ+je/wbWo+8TrAaqG3BhirSWOB3bMr+imLeL96RvsU4Eh0MtrYE9gG+KGZNzSefJmEs54ZN97MTiVSJSN8p4Qu1a33BxcFSzG8Ng7/Ow5OsEbLD3jUCrUOTtsoyqLlXVD7AO+Ip9YHhIRK6LePD4x9iBgxYi0rIYt/sEmwxRlJuKvooJq8g9YvcfhrU7l1I8GXOp6jVgErAF0CfiWC7FVqCmA09FEUBoFTAGW5XbEtumaaWqg3ywt1PV37Et64VANeBIIhyppKq/YD3uoBh9x0LrlUFFXO2/xWzU2gFoDKwDhhfjds6VGU/GXEoK3eEHhIu9oypQFpEtsSHIADeq6royfvzyInIF8APQERvs3QfYX1V/KMtYXGpT1ZWqejdwK7AEOwRzs4gMFpEqEYT0KNYframI7FuM231I4atjNxbys82EVbHu4eIHqjqnGHE4V2Y8GXOp7E1slE814LqIYrgCq137GXi2LB9YRJoCnwF3Y38HHwHNVfUuPw3mCqKq72HTFj4K32oC9BKRXcs4junAF+HiecW4XWGrY8VdFeuEnTJeg8+gdCnMkzGXssKLcqyv18Uisn1ZPn44Pn9VuDiorE6piUglEemPddHfDxtGfiHQUVV/LYsYXHpT1WWqOgi4AdvSrgm0FJEtRaR6GYbyKFbbuGsooo9XQatjxV0V2xnrv/dfVf2nGI/vXJnyZMyluvew1aEqwPVl/Nj/wd7EfgBeLosHFJG22JvnYKAiMBob7P2oD/Z2xaWq47Bask+wOZddgEtEZO+yGKmkqrOwxGoWdsgg3tvltzpW3FUxwmNPxAavO5eyxEfVuVQnIu2xF9V1wC6hWDne2w7GVtfuV9W4m8iKSH1gBlAd6KKqo4oRcrGFWZyDsASwHDAf67j+gs+TdIkQVsTOAbYGmgLzgCHJPl0oIlsAWwHTi/NvOSSLk7F2FGAHVuJKxkLPtQphqodzKc9XxlzKU9WPgA+wlaJ+hV87Ya7FErGJQFJHConIIdjJ0aux5+Rz2Cij5z0Rc4kSetA9iq281sG62z8uIl2TuUoWtkx/i/1bjvexwvVvDRenFnNVrBlwuYi0Ll60zkXDV8ZcWhCRA4Bx2Oms3QuqnZrYd2x1YG+sweO2n08f32H24r/33apG3UmH7Hrgu8BcrOnjt62HdFxawGNtB/yGbY0erarvJPwXYuNJzduxejCA2cDFqvpmMh7PuZhwOOQaoFH41q9YXeSfSXzMHYAjgCmq+nl+15kwrEclLJFqjbWjqLJ4+ep6W1SrtKR8uXIrsSHk3wET2/YekW8NmIhUxFrQrAKeVtWPE/7LOJdgnoy5tCEibwNHASNV9RyAiX3HVsHGAh2GvYDvTnwrvgpMxVa+PgBeaD2k44rwOPdhvcW+AA5MxuqUiBwDPIKNsiH897WpMPrJZQcRKQ+cC5yGlQB8iY0c+jIZ9Yki0jU83jzgLFXVCcN6lMd6onXGnr97YSOL4vEH9vz9DBjZtveIeeFxzgQuAJYDp/lUCpcOPBlzaSNsOXwN5PQ88OyjLmzX7TCss3axhwbnYynw5KhJ74y6+Z273sXeEDqG7ubFiVGAlsCP+dWrhFq0e7AZfGArcOeHrVjnypyINAKOxfqSLQUeAmok+vShiNQGngeqNG9U/7HHrzx2e2zMWKME3P064OVFy1YNP7LfC1co1AKeVVVv8urSgidjLq203bHlB2fve2qHA5vsk7THmPD7tzz15YvffDF9QrHrTUKD1ruBl1X11E2+L9gKxH3Ym14O8H/AQFVdmZDAnSuh8O9zb2AZsB3QHmstMS6RRfDNG2018NzD97r4gD0a1K9QvlxSapZn/bN0xfMfTv7p1XE/H6yqq5LxGM4lmidjLi1M7Du2EtBPVa8XkfKqSjJqjmP3q6oqIv8H9G89pGNcL+gisi229VkjfOtkVX019Ed7CNuKAWuVcZ6qTkh0/M6VRkjKTsLqtrbFVpiGqurXpbnfCcN6CNBdVe8WkZqlDrQAeV4XXgEuiW1fOpfKPBlzKW9i37GtgCeB5hE8/FSge+shHfMtON6UiDwJdNvkW3OBIVjPsJrYVsrNwG1+5N6lqpCQ7Yn9W62FreK+D9xbkvqrCcN6NMBmQh6ZwDALtUlStgC4BHipbe8R/mbnUpYnYy6lTew79kpgKFA+wjAU6/w9uPWQjvk+YURkf6CwhO0rbDVschLicy7hRKQu1m5lv/CtBcBdBZ2EzM+EYT2OxcaIJW01LE7PAT3a9h6xJuI4nMuXJ2MuJU3sO1awT+Zl3XW/MA8AvVsP6bjZSbPQYHI8dhosPw8Dl5bVOCXnEklEOmGni2tis2LHAe+p6urCbjdhWI+zsBYTUX6Q2tQYoEvb3iP8dKVLOZ6MuZQTErE7gD5Rx5KPx4ALNl0hE5HzKHwI8e9AM1VdnuzgnEuG0EX/FKAhtlL8OLBWVfOtx5owrMc5WGlB0kcuFdMnwFFte4/wQzMupXgHfpeKric1EzGA84E7QsKIiNTC6sIKsyO5ncSdSzuhi/4IbMbjGCzJulhETg6J2kYThvU4ARhB6iViAAcDr4Tmss6lDE/GXEqZ2HfsCdj2ZCrrQ26h/kNA/Thuc6mIbJ28kJxLPlX9PdSMbYutkO0DPC8iJ4mITBjWYw/gBVJnazI/R2Er786lDE/GXMqY2HdsXay+Kh3cc2n781sDpxdxvXXATOwNakGyg3KuLKjqeOyEZHWslctlFcuXe2DNug3PAZUjDS4+vScM69Eu6iCci/GaMZcyJvYd+xxwRtRxxCsnJ+fdfe44vCn25vMl1k3/jzxfc5MxWsa5VBDmQF4AdLm0c5vG53RqvlOyegAmwa9AC68fc6nAkzGXEib2HdsFeC3qOEqge+shHZ+MOogUJNjp0iOwbdwK0YZTKgoswU4RjgW8R1wefU7a76iTDtp9dLK66ifRvW17j7gi6iCc82TMRW5i37HVgOlAOtZULQEatx7ScVHUgaSQFsCrQJOoA0mCRcDlwMioA0klE4b1+Bgrjk83CrRt23vExKgDcdkt3T7FuMx0GumZiAFsyeZd97PdXsAHZGYiBlAb653VNepAUsWEYT1akZ6JGNgK7mVRB+GcJ2MuUqFFxCVRx1FKvSb2HevPJTMQqBN1EEkmwF2k99ZrIvWKOoBSOn3CsB71og7CZTd/A3FRa0vBnevTxS5Ax6iDSAE1gKOjDqKMbEX6rgYlzIRhPWoDZ0YdRylVBrpHHYTLbp6Muail+6fqmEz5PUqjBVAl6iDK0P5RB5ACugFVow4iAS6eMKyHvx+6yPg/PheZiX3HVsBGrGSC4yb2HbtF0VfLaFtGHUAZy7bfNz9p04qmCI2BfaMOwmUvr3lwUWoKVItdeOTTpxg+bvNDauWlHDWr1mSPbXblzLYnsl/jNmUd42YGjb6D0T++B8DDZ9xJmx33jv2oHLA38GkkgaWGQptLffTRR3To0CHfn33xxRfst99+bNiwgXvvvZf33nuPH3/8kYULF7Ljjjty/PHHc91111GrVq1CA1i6dCn33XcfY8aM4eeff2b58uU0btyYrl27cvnll1OlSsELd++//z6HHXYYAP/88w/16hVZRpQWzbSSJYwU2jvv95evWst/v5jKZ5P/4Lc5i1i+eh3Vq1SkTo0q7NqgLvvvsT2Ht9qJCuXLcdF97/DNr39vdvuK5ctRt2ZVWu68DT0Ob8GOW22e8+5z+RMb/3vUgJPZrq59Bjr+xpeZszB3/OvAs9pxzD47b3bb2176nNfG/bLx8mEtG3PLue1jF9sAXxT7L8K5BPBkzEWpyFqxDZrDopWL+Xz6eL6YPoH/O/km2u28X1nEVhKtye5kLC633nrrv5KyZs2aAbBq1SoGDRrEGWecwfnnn0+9evX45ptvuPnmm3nzzTf5+uuvqVq14F2xWbNmcc8993D22Wdz1VVXUaNGDT799FMGDRrEmDFjGDNmTL4NSZcvX07Pnj3Zbrvt+OuvvxL7C6cRsb+cPYBpqrquiKvvCWw24/H7GfO4/okPmbdk8z6qS1asYcmKNcyYu4T/TZzOAXs0oFaN/BPjdRty+HvRCt6Z8BvjJv/Bs9eewNa1qhf7d3npk582S8aWr1rLOxN+K+wm6V676tKYJ2MuSgW++B3b7HAGHXsNC1Ys4sa37uDz6RNQlBe+fj3VkzFXhF122YX99sv//2HVqlWZMWMGdevW3fi99u3b07BhQ0455RReffVVunYtuKtE48aNmTlzJtWr5755H3rooVSvXp2rr76acePGcdBBB/3rdtdddx21a9fmmGOO4eabU300alJ1w4aBzxSRW4CnCknKNvv3Pnv+Mq54ZAzLV1lP3FY7b8MFR7WkacN6iMCchcuZOO1v3prwa753NuDMgzhmn52ZPmcxVzwyhrmLV7B05VreHv8r3Q9vUexf5Kc/5vPDzHk0b7QVAG98OY1Va9cXdhN//rrIeDLmolTknmPd6rU5qWVnPp8+AYA5S+du/Nlr341mzE8f8/vCP1i6ejnrN6ynTvVatGjQjB77n8kuW+208bqbbi/eddJgxs/8hvd//oRV61ax61ZN+E+nXuyxza4br5+jOTzxxfOM+u5tFqxYSKO6DTnvgLNK/fu4wpUvX36zRCxmn332AeCPP/4o9PabJmHx3v7TTz/l0Ucf5csvv+SNN94obsiZptEmfw4HbigkKdvs3/uj73y7MRFr2rAe9/c6ggrlc8uSG21di0Zb1+Kkg3Yv8MFFhCbb1ebQvRvx/EeTAfh70fICr1+Q7erW4K8Fy3npk59o3mgrVJVXP/tps5/lo+mEYT2qt+09YkWxH9C5UvICfhelgl+VN7HplIg61Wpt/O9xv41nwu/fMm/ZfFavW836nPXMWzafMT99xHnPXM6shX/me383vjWUFyeOYsGKhaxcu4rv/vyRy17sy/I1ua/Bd73/IA998gRzls5l7YZ1TJ33G9eOGsxXMwtt1L3bxL5jy8fzO2WzSy65hAoVKlCzZk2OOOIIPvvssyJv88EHHwCw5557lugxC7r9qlWrOO+887jiiito1apVie47wzXCkrKpInJ+mEUZs/H5m5OjfDo5N9E9q8OemyVixbXpc752jeIf1jw5JHxjv5vJ/KUrGTflT/6Yv4wK5ctxwv67FXSzclibGufKnK+MuSgVWQiyYMUiXv32zY2Xj27WaeN/n9LqOM4/sCvbbrk1NSrXYMWaFTw34VUe//xZVq5dxavfjubKjhf96z6rVKzMfacNYfta23Lt64OZOGsSi1ctYdxv4zmiaQf+XPQXL038LwAVy1fk9hMG0GbHvfngl08Z9NYdhYUrff9783Zjbuu0Kv6/gswxZcqUmnvssUeBP99yyy25/PLLad++PXXr1uXXX39l6NChtG/fnrfeeosjjjgi39vNnj2b6667jjZt2nDssccWO67vv/+eO+64gy5durDXXntt9rP+/fuzYcMGbrzxxmLf7+LFi6vWrl0705qFVivg+42wpKy/iNwNPDD+3u4bn79LVq7ZuCoGsPN2uX1/R30xlVtfGLfZnZ3TsTmXHvfvhWRVZfrfi/lw0u8AlC8nHNaqcbF/iQOa7sBr437hz/nLeH3cL/ww8x8ADm2xI/VqFprcFfT7O5dUnoy5SIS2FgX++xv943sbtxUBqlWqyrn7ncGJe+e+GdetXocnvnieSbN/ZOGKxazbsPkuyowFv+d73+fsexp7bmufnA/drR0TZ00CYM4SO9X11cxvUOyTebud9+PgXayd1LHND+e170bz/ewpBf5e42d8M6vAH2a4Pn368NZbbxX485YtW9KyZcuNl9u1a0eXLl1o3rw511xzTb7J2MKFCzn66KNRVV588UXKFXMO9cyZMzn22GPZYYcdeOyxxzb72fjx47nnnnt49913Cz0UUJDhw4dfQvpPjyiuhsDdwDXAwtg38844Xrt+Q7HvePBznzH4udxV0m3r1KDPSfvSZNvaxb6vcgInH7QH94waz4ufTGFZSBRPPXgPZs1bWthNM6FnmktDvk3p0sKGnBxWrctdcJqzZC49RvbmvZ8+ZO7Sf/6ViAGsXrcm3/tqVLfhxv+uWjH3RNea9faCvXjVko3f23qL+pvddpuahY/QjCVxLj61atXi2GOP5fvvv2fVqs0XFBctWsRhhx3G7NmzGTNmDDvttFMB95K/33//nQ4dOlChQgXGjh1LnTqbT2nq0aMHJ554Im3atGHx4sUsXryY1atXA9YiY9myZaX75TLbSsj9x16rehWqV8ndwZzx9+KN/33C/rsy/t7unH/k3sV6gDVr17N2fU6JAzxuv12oWqkCS1euRRV2b1CXvRoXOQLXn8AuEp6MuUi0HtJxPVDg0aZjmx3OV9f8j8e63kPd6rVZs34NT3zxPC9OHAXAR1PHsWqdvXG23bEl71zyAl9f9z7/d9JNRT52hXK5ZV2ST6uoWlVz+xrNXfbPZj/7e5MDBPl5peeI6tjzKuu+3njjjeLvIZK7qrJpy4lFixbRqVMnZsyYwZgxY/61vViU33//nfbt26OqfPjhhzRo0OBf15k8eTIvv/wytWvX3vh1++23A9CkSRPatWtX6GP06dPnTlLg7z3BX0Xt104CugC7Aqtj3yxXTmi35w4br/T02B/YkFO8RGrAmQfx2V3n0O+MAyknwsLlq+n31Ef88ueCYt1PTI2qlTi6bW5ri1MPLngLfROri76Kc4nnyZiLUqHHpMqXK8/eDZrR94grNn7voU+eYPHKJZTfJKGqWL4CVStW4c9Ff/H458+WOqh9G7XamKR9+uuXfPrrl6xcu4rRP7xX6BYlkFOneu3VmqXKly/+2YVFixYxevRo9t57740NWWOJ2PTp03nvvfc229qMx6xZs2jfvj0bNmzggw8+YMcdd8z3eh9++OG/vrp16wbAqFGj/rWtmZeIEPXfeaIV8uvGkrBWqjpKVXPI8/zteVRLqle21bFf/1pEn+FjmTJrPmvXb2D5qrXMW1z0IcVKFcpz3H67bkycNuQoQ1/5ssjbFeT0Q5pycPOGHLp3o3hrz4p/dNO5BPCaMRelycCBRV2p/a4H0rphCybOmsTyNSt45LOn6brPyVT5qAqr163m8+kTaH/PCQA0rPPvFZDialB7O05tfTwvThzFug3ruPKVfht/VrtaLRatXFzQTae0HtKx5PsqGe7MM8+kYcOGtGnThnr16jFt2jTuuusu5s6dy5NPPgnY6cYjjjiCb7/9lnvuuYf169fz5Ze5b8b169enSZMmGy9XqFCBQw45hLFjxwIwb948OnTowJw5c3j88ceZN28e8+bN23j9Bg0abFwla9++/b9i/OijjwA48MAD4+nAnw0mAYOAN0ICtqnJQPvYhR3q1+SuCzpx/RMfsnD5asZN+ZNxU/I/0VyU84/cm7cn/MbSlWv4fsY8xn43k457Nyr2/ey49ZbceX7HeK++Hpha7AdxLgE8GXNRmkgcyRjAlYdexNlP9kJRXvtuNKe1Pp57T7mF+z96jGn/zKBG5eoc1fRQ9mnUiste6lvqwP7TqRd1qtfmte9Gs3DFYhrW2Z7u+53BlzMmbnawIJ/fxxVgr7324sUXX+Thhx9m+fLl1KlTh4MOOoiRI0fStm1bAObOncuECdZT7vLLL//XfXTr1m1j4gawYcMGNmzILRafMmUK06dPB8i3OezAgQMZNGhQAn+rjPNT+LOwJCzmX//eW+28DS9c34XXx/3CZ5P/YObcJaxau54tq1em7hZV2XX7OrRr1pD9dt+u0CBqVqvMeUe04O7XxwNw/xtfc3CzHahYIamdYya37T3CtyldJKTwlWnnkmdi37FnA09HHUcCXdZ6SMf7ow4iQscAo6MOogzdCVwddRCJJiJbA/8UkoQBMGFYj+bA92UTVZl4vG3vEedHHYTLTl4z5qKUaStJmfb7uCykqnOLSsSCn4BM6qnnz18XGU/GXJR+ATKlf8A6bGsnm2VbvVy2/b6badt7xHrgm6jjSKAJUQfgspcnYy4yrYd03AA8F3UcCfJq6yEdV0YdRMSWFH2VjLI46gBSwDNRB5AgP+MrYy5Cnoy5qD0UdQAJ8mDUAaSAb8mu1gCfRB1ACniWzFjdfrBt7xFeQO0i48mYi1TrIR0nAeOKvGJq+xEoetp15ltF9hTwzwa+iDqIqLXtPWIZ6X8IZyXp/zu4NOfJmEsF6b6q9GDrIR39U7XpjyUqmWwd0IssrxnbRLqvbj/TtveIbNtidynGkzGXCl4F8p/qnfr+IXPqZhLhV6ADMD7qQJLkd+Bk4I2oA0kVbXuPmAy8G3UcJbQBGBZ1EM55nzGXEib2HXsYUGA31RR2SushHV+JOogU1Rg4AqhPejeYVqxYfxzwNT5M+l8mDOvRGPgBqB51LMV0c9veI/pHHYRznoy5lDGx79hHgAuijqMYXmo9pONpUQfhXCqYMKxHL+CBqOMohh+ANm17j1gbdSDO+TalSyVXA7OiDiJO/wCXRh2EcynkYeDDqIOI0waguydiLlV4MuZSRushHZcC50UdR5wubj2k4z9RB+Fcqmjbe0QO0IP0aHVxa9veI7yvmEsZnoy5lNJ6SMf3Sf0Vp+tbD+n4atRBOJdq2vYeMRM4AVgTbSSFegG4MeognNuUJ2Mu5bQe0vEB4Pqo4yjAHcBtUQfhXKpq23vEB8BpwPqoY8nHaOCctr1HbIg6EOc25cmYS0mth3QcAvwn6jjyuBG4znuKOVe4tr1H/BdbIVsdcSibehk4qW3vEeuiDsS5vPw0pUtpE/uO7YY1lawaYRhrgavCip1zLk4ThvU4GHgR2CbiUO4DrvQVMZeqPBlzKW9i37E7AyOAdhE8/NfAua2HdJwcwWM7l/YmDOtRB7gX6BrBw88Czmvbe8T7ETy2c3HzZMylhYl9x5bDCvtvo2xWydYCg4ChrYd0TMXaF+fSyoRhPY4DHqHsVskeAa4O8zOdS2mejLm0ElbJBgKnApWS8BDrgdeBG301zLnECqtk/bAWGFsm6WE+AG4JBwmcSwuejLm0NLHv2PrYC/pFQKME3OVs7JP0Y62HdJyTgPtzzhVgwrAe1YHTgUuAlgm4y6XAk8DDbXuP+CkB9+dcmfJkzKW1iX3HlsfmH3YCWgOtgBpx3HQl8C0wEesaPtq3I50rWxOG9RBgH+A47PnbGqgXx03XAT9iz99xwMtte49Ykaw4nUs2T8ZcRgm1ZbsAbbDalKpAZawJ5WpgLvAN8HPrIR39ZJVzKSQkZztgSVljoAr2HF6HPX8XYR+ifmjbe0QqN5Z1rlg8GXPOOeeci5A3fXXOOeeci5AnY84555xzEfJkzDnnnHMuQp6MOeecc85FyJMx55xzzrkIeTLmnHPOORchT8acc8455yLkyZhzzjnnXIQ8GXPOOeeci5AnY84555xzEfJkzDnnnHMuQp6MOeecc85FyJMx55xzzrkIeTLmnHPOORchT8acc8455yLkyZhLeSJSQ0TuEZG/RGS1iHwnIqfHedutRORJEZkvIitF5AsR6VjAdTuFn68M139SRLZK7G/jXHYpzfM3z/3cLCIqIj/m87OPws/yfr2bmN/CueSqEHUAzsXhNaAtcB0wFTgTeF5EyqnqcwXdSEQqA2OBWsDlwDzgEuBdEemkqh9vct1DgHeAt4Djga2A24GxItJGVdck4xdzLguU6Pm7KRHZG+gDzC3katOBs/J8b3Fxg3UuCqKqUcfgXIFE5GgsQTpTVZ/f5PvvAXsCDVV1QwG37QU8ABygql+E71UAJgHLVXXfTa47HqgOtFDV9eF7BwDjgF6q+lAyfj/nMllpnr+bXLcCMAH4BGgB1FPVZnmu81F+33cuXfg2pUt1XYDlwMt5vv8EsB2w779usfltf4klYgAh0XoG2EdEtgcIf7YFRsYSsXDdz7FP8l0S8Hs4l41K8/yNuQ6oA9yQ2NCcSx2ejLlU1wz4adMkKfh+k58Xdtvv8/l+7Ht75rmPgq7rn7adK5nSPH8RkaZAP+BiVV1exGM1EZGFIrJeRH4TkVtEpGrJwnaubHnNmEt1dbFakLwWbvLzwm67MJ/v571t3Tzfz3vdwh7DOVewEj9/RaQcMAJ4TVXfLuJxPgNeBH4GqgJHAdcAB4lIB1XNKW7gzpUlT8ZcOiissLGoosfi3Lag63phpXMlV9Ln71XALsBxRT6Aar8833pbRGYCd2IHcl4v6j6ci5JvU7pUt4D8Pz3XCX/mt5pV3NsuCH8WdN3CHsM5V7ASPX9FpCEwGLgRWCsitUSkFraAUC5cLmoL8pnw537Fjtq5MubJmEt1PwB7hBNVm2oe/vxXz6E8t22ez/fz3vbHPN/Pe93CHsM5V7CSPn93wrYb7wUWbfJ1ILBH+O8hccbgW5Qu5Xky5lLd60AN4KQ83+8G/AV8VcRtdxeRTVtYVAC6Al+p6l8AqjobGA90FZHym1x3P2A3rE+Sc674Svr8/Q7okM/XJGBm+O/7i3jsbuHPL4sZs3NlzvuMuZQXehK1Aa4FfgXOAHoCXVX12XCdx7EX3yaq+nv4XmVgIlATOx4/D+gFdAbyNn1tD4wB3gQexJq+3gYsAbzpq3MlVNLnbwH39RF5+omJSDus7cXr2GGBKlgB/wXAx8BhXsDvUp0X8Lt0cCJwC1ZDUgc7MXWGqr6wyXXKhy+JfUNV14TRR3cA9wHVsE/cR22aiIXrfhQaVA7GErKVwGjgak/EnCuVEj1/i2EOsAHoD9TDDgVMAwYAd3ki5tKBr4w555xzzkXIa8acc8455yLkyZhzzjnnXIQ8GXPOOeeci5AnY84555xzEfJkzDnnnHMuQp6MOeecc85FyJMx55xzzrkIeTLmnHPOORchT8acc8455yLkyZhzzjnnXIQ8GXPOOeeci5AnY84555xzEfJkzDnnnHMuQp6MOeecc85FyJMx55xzzrkIeTLmnHPOOReh/wfYnsASkYAeWgAAAABJRU5ErkJggg==\n",
+                        "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 750x750 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -241,13 +241,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.8"
+            "version": "3.8.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `egttools-0.1.9.dev3/docs/examples.rst` & `egttools-0.1.9.dev6/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/hawk_dove_analytical_full_sd.png` & `egttools-0.1.9.dev6/docs/images/hawk_dove_analytical_full_sd.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/hawk_dove_analytical_gradient.png` & `egttools-0.1.9.dev6/docs/images/hawk_dove_analytical_gradient.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/hawk_dove_comparison.png` & `egttools-0.1.9.dev6/docs/images/hawk_dove_comparison.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/hawk_dove_indep_runs.png` & `egttools-0.1.9.dev6/docs/images/hawk_dove_indep_runs.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/logo-full.pdf` & `egttools-0.1.9.dev6/docs/images/logo-full.pdf`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/logo-full.png` & `egttools-0.1.9.dev6/docs/images/logo-full.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/logo-full.svg` & `egttools-0.1.9.dev6/docs/images/logo-full.svg`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/logo.pdf` & `egttools-0.1.9.dev6/docs/images/logo.pdf`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/logo.png` & `egttools-0.1.9.dev6/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/logo.svg` & `egttools-0.1.9.dev6/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/simplex_example_infinite_pop_1.png` & `egttools-0.1.9.dev6/docs/images/simplex_example_infinite_pop_1.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/images/simplex_example_infinite_pop_2.png` & `egttools-0.1.9.dev6/docs/images/simplex_example_infinite_pop_2.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/index.rst` & `egttools-0.1.9.dev6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/installation.rst` & `egttools-0.1.9.dev6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/docs/make.bat` & `egttools-0.1.9.dev6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/__init__.py` & `egttools-0.1.9.dev6/egttools/__init__.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/analytical/sed_analytical.py` & `egttools-0.1.9.dev6/egttools/analytical/sed_analytical.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 import numpy as np
 import numpy.typing as npt
 from scipy.sparse import lil_matrix
 from scipy.stats import hypergeom, multivariate_hypergeom
 from itertools import permutations
 from typing import Tuple, Optional
+from warnings import warn
 from egttools import sample_simplex, calculate_nb_states, calculate_state
 
 
 def replicator_equation(x: np.ndarray, payoffs: np.ndarray) -> np.ndarray:
     """
     Produces the discrete time derivative of the replicator dynamics
 
@@ -90,14 +91,59 @@
         if group_size > 2:  # pairwise game
             self.fitness = self.fitness_group
             self.full_fitness = self.full_fitness_difference_group
         else:  # group game
             self.fitness = self.fitness_pair
             self.full_fitness = self.full_fitness_difference_pairwise
 
+    def update_population_size(self, pop_size: int):
+        """
+        Updates the size of the population and the number of possible population states.
+
+        Parameters
+        ----------
+        pop_size: New population size
+        """
+        self.Z = pop_size
+        self.nb_states_population = calculate_nb_states(pop_size, self.nb_strategies)
+
+    def update_group_size(self, group_size: int):
+        """
+        Updates the groups size of the game (and the methods used to compute the fitness)
+
+        Parameters
+        ----------
+        group_size: new group size
+        """
+        self.N = group_size
+        self.nb_group_combinations = calculate_nb_states(group_size, self.nb_strategies)
+        if group_size > 2:  # pairwise game
+            self.fitness = self.fitness_group
+            self.full_fitness = self.full_fitness_difference_group
+        else:  # group game
+            self.fitness = self.fitness_pair
+            self.full_fitness = self.full_fitness_difference_pairwise
+
+    def update_payoffs(self, payoffs: np.ndarray, nb_strategies: Optional[int] = None):
+        """
+        Updates the payoff matrix
+
+        Parameters
+        ----------
+        payoffs: payoff matrix
+        nb_strategies: total number of strategies (optional). If not indicated, then the new payoff
+                       matrix must have the same dimensions as the previous one
+        """
+        if nb_strategies is None:
+            if payoffs.shape[0] != self.nb_strategies:
+                raise Exception("The number of rows of the payoff matrix must be equal to the number of strategies.")
+        else:
+            self.nb_strategies = nb_strategies
+        self.payoffs = payoffs
+
     def fitness_pair(self, x: int, i: int, j: int, *args: Optional[list]) -> float:
         """
         Calculates the fitness of strategy i versus strategy j, in
         a population of x i-strategists and (Z-x) j strategists, considering
         a 2-player game.
 
         Parameters
@@ -215,23 +261,23 @@
         population_state[i] += 1
         population_state[j] -= 1
         rv_j = multivariate_hypergeom(population_state, self.N - 1)
         population_state[j] += 1
 
         fitness_i, fitness_j = 0., 0.
         for state_index in range(self.nb_group_combinations):
-            group = sample_simplex(i, self.N, self.nb_strategies)
+            group = sample_simplex(state_index, self.N, self.nb_strategies)
             if group[i] > 0:
                 group[i] -= 1
                 fitness_i += self.payoffs[i, state_index] * rv_i.pmf(x=group)
                 group[i] += 1
             if group[j] > 0:
-                group[i] -= 1
+                group[j] -= 1
                 fitness_j += self.payoffs[j, state_index] * rv_j.pmf(x=group)
-                group[i] += 1
+                group[j] += 1
 
         return fitness_i - fitness_j
 
     @staticmethod
     def fermi(beta: float, fitness_diff: float) -> npt.ArrayLike:
         """
         The fermi function determines the probability that the first type imitates the second.
@@ -364,14 +410,15 @@
             Matrix indicating the likelihood of change in the population given an starting point.
         """
         probability_selecting_strategy_first = population_state / self.Z
         probability_selecting_strategy_second = population_state / (self.Z - 1)
         probabilities = np.outer(probability_selecting_strategy_first, probability_selecting_strategy_second)
         fitness = np.asarray([[self.full_fitness(i, j, population_state) for i in
                                range(len(population_state))] for j in range(len(population_state))])
+        fitness[np.isnan(fitness)] = 0
         return (probabilities * np.tanh((beta / 2) * fitness)).sum(axis=0) * (1 - self.mu) + self.mu
 
     def full_gradient_selection_without_mutation(self, population_state: np.ndarray, beta: float) -> np.ndarray:
         """
         Calculates the gradient of selection for an invading strategy, given a population state. It does
         not take into account mutation.
 
@@ -390,14 +437,15 @@
         """
 
         probability_selecting_strategy_first = population_state / self.Z
         probability_selecting_strategy_second = population_state / (self.Z - 1)
         probabilities = np.outer(probability_selecting_strategy_first, probability_selecting_strategy_second)
         fitness = np.asarray([[self.full_fitness(i, j, population_state) for i in
                                range(len(population_state))] for j in range(len(population_state))])
+        fitness[np.isnan(fitness)] = 0
 
         return (probabilities * np.tanh((beta / 2) * fitness)).sum(axis=0)
 
     def fixation_probability(self, invader: int, resident: int, beta: float, *args: Optional[list]) -> float:
         """
         Function for calculating the fixation_probability probability of the invader
         in a population of residents.
@@ -547,14 +595,21 @@
             A vector containing the stationary distribution
         """
         if self.mu > 0:
             t = self.calculate_full_transition_matrix(beta, *args).toarray()
         else:
             t, _ = self.transition_and_fixation_matrix(beta, *args)
 
+        # Check if there is any transition with value 1 - this would mean that the game is degenerate
+        if np.isclose(t, 1., atol=1e-11).any():
+            warn(
+                "Some of the entries in the transition matrix are close to 1 (with a tolerance of 1e-11). "
+                "This could result in more than one eigenvalue of magnitute 1 "
+                "(the Markov Chain is degenerate), so please be careful when analysing the results.", RuntimeWarning)
+
         # calculate stationary distributions using eigenvalues and eigenvectors
         eigenvalues, eigenvectors = np.linalg.eig(t)
         index_stationary = np.argmin(
             abs(eigenvalues - 1.0))  # look for the element closest to 1 in the list of eigenvalues
         sd = abs(eigenvectors[:, index_stationary].real)  # it is essential to access the matrix by column
 
         return sd / sd.sum()
```

### Comparing `egttools-0.1.9.dev3/egttools/analytical/utils.py` & `egttools-0.1.9.dev6/egttools/analytical/utils.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/behaviors/CRD/moving_average.py` & `egttools-0.1.9.dev6/egttools/behaviors/CRD/moving_average.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/behaviors/NormalForm/TwoActions/nfg_strategies.py` & `egttools-0.1.9.dev6/egttools/behaviors/NormalForm/TwoActions/nfg_strategies.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/behaviors/pgg_behaviors.py` & `egttools-0.1.9.dev6/egttools/behaviors/pgg_behaviors.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/games/crd.py` & `egttools-0.1.9.dev6/egttools/games/crd.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/games/informal_risk.py` & `egttools-0.1.9.dev6/egttools/games/informal_risk.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/games/pgg.py` & `egttools-0.1.9.dev6/egttools/games/pgg.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/helpers/vectorized.py` & `egttools-0.1.9.dev6/egttools/helpers/vectorized.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/plotting/helpers.py` & `egttools-0.1.9.dev6/egttools/plotting/helpers.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/plotting/indicators.py` & `egttools-0.1.9.dev6/egttools/plotting/indicators.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/plotting/simplex2d.py` & `egttools-0.1.9.dev6/egttools/plotting/simplex2d.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/egttools/plotting/simplified.py` & `egttools-0.1.9.dev6/egttools/plotting/simplified.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with EGTtools.  If not, see <http://www.gnu.org/licenses/>
 
 """Simplified plotting functions"""
-
+import egttools.games
 import matplotlib.pyplot as plt
 import numpy as np
 
 from typing import Optional, Tuple, Callable, List
 from egttools.numerical import (calculate_nb_states, )
 from egttools.plotting.helpers import (barycentric_to_xy_coordinates,
                                        xy_to_barycentric_coordinates, calculate_stationary_points, calculate_stability,
                                        find_roots_in_discrete_barycentric_coordinates)
 from egttools.analytical import (replicator_equation, StochDynamics)
 from egttools.analytical.utils import check_if_there_is_random_drift
 from egttools.helpers.vectorized import (vectorized_replicator_equation, vectorized_barycentric_to_xy_coordinates)
 from egttools.plotting import Simplex2D
+from egttools.utils import transform_payoffs_to_pairwise
 
 
 def plot_replicator_dynamics_in_simplex(payoff_matrix: np.ndarray, atol: Optional[float] = 1e-7,
                                         figsize: Optional[Tuple[int, int]] = (10, 8),
                                         ax: Optional[plt.axis] = None) -> \
         Tuple[Simplex2D, Callable[[np.ndarray, int], np.ndarray], List[np.ndarray], List[np.ndarray], List[bool]]:
     """
@@ -74,35 +75,38 @@
     roots, roots_xy = calculate_stationary_points(simplex.trimesh.x, simplex.trimesh.y, simplex.corners,
                                                   lambda u: replicator_equation(u, payoff_matrix))
     stability = calculate_stability(roots, lambda u: replicator_equation(u, payoff_matrix))
 
     return simplex, lambda u, t: replicator_equation(u, payoff_matrix), roots, roots_xy, stability
 
 
-def plot_moran_dynamics_in_simplex(payoff_matrix: np.ndarray,
-                                   population_size: int,
+def plot_moran_dynamics_in_simplex(population_size: int,
                                    beta: float,
+                                   payoff_matrix: np.ndarray = None,
+                                   game: egttools.games.AbstractGame = None,
                                    group_size: Optional[int] = 2,
                                    atol: Optional[float] = 1e-7,
                                    figsize: Optional[Tuple[int, int]] = (10, 8),
                                    ax: Optional[plt.axis] = None) -> \
         Tuple[Simplex2D, Callable[[np.ndarray, int], np.ndarray], List[np.ndarray], List[np.ndarray], List[
             bool], StochDynamics]:
     """
     Helper function to simplified the plotting of the moran dynamics in a 2 Simplex.
 
     Parameters
     ----------
-    payoff_matrix:
-        The square payoff matrix. Group games are still unsupported in the replicator dynamics. This feature will
-        soon be added.
     population_size:
         Size of the finite population.
     beta:
         Intensity of selection.
+    payoff_matrix:
+        The square payoff matrix. Group games are still unsupported in the replicator dynamics. This feature will
+        soon be added.
+    game:
+        Game that should contain a set of payoff matrices
     group_size:
         Size of the group. By default we assume that interactions are pairwise (the group size is 2).
     atol:
         Tolerance to consider a value equal to zero. This is used to check if an edge has random drift. By default
         the tolerance is 1e-7.
     figsize:
         Size of the figure. This parameter is only used if the ax parameter is not defined.
@@ -112,38 +116,128 @@
     Returns
     -------
     A tuple with the simplex object which can be used to add more features to the plot, the function that
     can be used to calculate gradients and should be passed to `Simplex2D.draw_trajectory_from_roots` and
     `Simplex2D.draw_scatter_shadow`, a list of the roots in barycentric coordinates, a list of the roots in
     cartesian coordinates and a list of booleans indicating whether the roots are stable.
     """
+    if (group_size == 2) and payoff_matrix is None:
+        raise Exception("You need to define a payoff matrix for pairwise games.")
+
     simplex = Simplex2D(discrete=True, size=population_size, nb_points=population_size + 1)
     simplex.add_axis(figsize, ax)
 
-    random_drift = check_if_there_is_random_drift(payoff_matrix=payoff_matrix, population_size=population_size,
+    if group_size > 2:
+        payoffs = transform_payoffs_to_pairwise(game.payoffs().shape[0], game)
+        payoff_matrix = game.payoffs()
+    else:
+        payoffs = payoff_matrix
+
+    random_drift = check_if_there_is_random_drift(payoff_matrix=payoffs, population_size=population_size,
                                                   group_size=group_size, beta=beta, atol=atol)
     simplex.add_edges_with_random_drift(random_drift)
 
     v = np.asarray(xy_to_barycentric_coordinates(simplex.X, simplex.Y, simplex.corners))
     v_int = np.floor(v * population_size).astype(np.int64)
 
     evolver = StochDynamics(nb_strategies=3, payoffs=payoff_matrix, pop_size=population_size, group_size=group_size)
-    result = np.asarray([[evolver.full_gradient_selection(v_int[:, i, j], beta) for j in range(v_int.shape[2])] for i in
-                         range(v_int.shape[1])]).swapaxes(0, 1).swapaxes(0, 2)
+    result = np.zeros(shape=(v_int.shape[1], v_int.shape[2], 3))
+    for i in range(v_int.shape[1]):
+        for j in range(v_int.shape[2]):
+            result[i, j, :] = evolver.full_gradient_selection_without_mutation(v_int[:, i, j], beta)
+
+    result = result.swapaxes(0, 1).swapaxes(0, 2)
     xy_results = vectorized_barycentric_to_xy_coordinates(result, simplex.corners)
 
     Ux = xy_results[:, :, 0].astype(np.float64)
     Uy = xy_results[:, :, 1].astype(np.float64)
 
     simplex.apply_simplex_boundaries_to_gradients(Ux, Uy)
 
     roots = find_roots_in_discrete_barycentric_coordinates(
-        lambda u: population_size * evolver.full_gradient_selection(u, beta), population_size,
+        lambda u: population_size * evolver.full_gradient_selection_without_mutation(u, beta), population_size,
         nb_interior_points=calculate_nb_states(population_size,
                                                3),
         atol=1e-1)
     roots_xy = [barycentric_to_xy_coordinates(x, simplex.corners) for x in roots]
     stability = calculate_stability(roots, lambda u: population_size * evolver.full_gradient_selection(u, beta))
 
     return (simplex,
             lambda u, t: population_size * evolver.full_gradient_selection_without_mutation(u, beta),
             roots, roots_xy, stability, evolver)
+
+
+def plot_moran_dynamics_in_simplex_without_roots(population_size: int,
+                                                 beta: float,
+                                                 payoff_matrix: np.ndarray = None,
+                                                 game: egttools.games.AbstractGame = None,
+                                                 group_size: Optional[int] = 2,
+                                                 atol: Optional[float] = 1e-7,
+                                                 figsize: Optional[Tuple[int, int]] = (10, 8),
+                                                 ax: Optional[plt.axis] = None) -> \
+        Tuple[Simplex2D, Callable[[np.ndarray, int], np.ndarray], StochDynamics]:
+    """
+    Helper function to simplified the plotting of the moran dynamics in a 2 Simplex.
+
+    Parameters
+    ----------
+    population_size:
+        Size of the finite population.
+    beta:
+        Intensity of selection.
+    payoff_matrix:
+        The square payoff matrix. Group games are still unsupported in the replicator dynamics. This feature will
+        soon be added.
+    game:
+        Game that should contain a set of payoff matrices
+    group_size:
+        Size of the group. By default we assume that interactions are pairwise (the group size is 2).
+    atol:
+        Tolerance to consider a value equal to zero. This is used to check if an edge has random drift. By default
+        the tolerance is 1e-7.
+    figsize:
+        Size of the figure. This parameter is only used if the ax parameter is not defined.
+    ax:
+        A matplotlib figure axis.
+
+    Returns
+    -------
+    A tuple with the simplex object which can be used to add more features to the plot, the function that
+    can be used to calculate gradients and should be passed to `Simplex2D.draw_trajectory_from_roots` and
+    `Simplex2D.draw_scatter_shadow`, a list of the roots in barycentric coordinates, a list of the roots in
+    cartesian coordinates and a list of booleans indicating whether the roots are stable.
+    """
+    if (group_size == 2) and payoff_matrix is None:
+        raise Exception("You need to define a payoff matrix for pairwise games.")
+
+    simplex = Simplex2D(discrete=True, size=population_size, nb_points=population_size + 1)
+    simplex.add_axis(figsize, ax)
+
+    if group_size > 2:
+        payoffs = transform_payoffs_to_pairwise(game.payoffs().shape[0], game)
+        payoff_matrix = game.payoffs()
+    else:
+        payoffs = payoff_matrix
+
+    random_drift = check_if_there_is_random_drift(payoff_matrix=payoffs, population_size=population_size,
+                                                  group_size=group_size, beta=beta, atol=atol)
+    simplex.add_edges_with_random_drift(random_drift)
+
+    v = np.asarray(xy_to_barycentric_coordinates(simplex.X, simplex.Y, simplex.corners))
+    v_int = np.floor(v * population_size).astype(np.int64)
+
+    evolver = StochDynamics(nb_strategies=3, payoffs=payoff_matrix, pop_size=population_size, group_size=group_size)
+    result = np.zeros(shape=(v_int.shape[1], v_int.shape[2], 3))
+    for i in range(v_int.shape[1]):
+        for j in range(v_int.shape[2]):
+            if v_int[:, i, j].sum() <= population_size:
+                result[i, j, :] = evolver.full_gradient_selection_without_mutation(v_int[:, i, j], beta)
+
+    result = result.swapaxes(0, 1).swapaxes(0, 2)
+    xy_results = vectorized_barycentric_to_xy_coordinates(result, simplex.corners)
+
+    Ux = xy_results[:, :, 0].astype(np.float64)
+    Uy = xy_results[:, :, 1].astype(np.float64)
+
+    simplex.apply_simplex_boundaries_to_gradients(Ux, Uy)
+
+    return simplex, lambda u, t: population_size * evolver.full_gradient_selection_without_mutation(u, beta), evolver
```

### Comparing `egttools-0.1.9.dev3/egttools/utils.py` & `egttools-0.1.9.dev6/egttools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 # You should have received a copy of the GNU General Public License
 # along with EGTtools.  If not, see <http://www.gnu.org/licenses/>
 
 """
 This python module contains some utility functions
 to find saddle points and plot gradients in 2 player, 2 strategy games.
 """
+from warnings import warn
+
 import numpy as np
 from scipy.linalg import schur, eigvals
 from typing import Optional, List, Generator, Union, Callable
 from egttools.games import AbstractGame
 
 
 def find_saddle_type_and_gradient_direction(gradient: Union[List[float], np.ndarray],
@@ -197,14 +199,21 @@
         A 1-dimensional vector containing the stationary distribution
 
     See Also
     --------
     egttools.utils.calculate_stationary_distribution_non_hermitian
 
     """
+    # Check if there is any transition with value 1 - this would mean that the game is degenerate
+    if np.isclose(transition_matrix, 1., atol=1e-11).any():
+        warn(
+            "Some of the entries in the transition matrix are close to 1 (with a tolerance of 1e-11). "
+            "This could result in more than one eigenvalue of magnitute 1 "
+            "(the Markov Chain is degenerate), so please be careful when analysing the results.", RuntimeWarning)
+
     # calculate stationary distributions using eigenvalues and eigenvectors
     eigenvalues, eigenvectors = np.linalg.eig(transition_matrix)
     index_stationary = np.argmin(abs(eigenvalues - 1.0))  # look for the element closest to 1 in the list of eigenvalues
     sd = abs(eigenvectors[:, index_stationary].T.real)  # it is essential to access the matrix by column
     return sd / sd.sum()  # normalize
 
 
@@ -225,14 +234,21 @@
         A 1-dimensional vector containing the stationary distribution
 
     See Also
     --------
     egttools.utils.calculate_stationary_distribution
 
     """
+    # Check if there is any transition with value 1 - this would mean that the game is degenerate
+    if np.isclose(transition_matrix, 1., atol=1e-11).any():
+        warn(
+            "Some of the entries in the transition matrix are close to 1 (with a tolerance of 1e-11). "
+            "This could result in more than one eigenvalue of magnitute 1 "
+            "(the Markov Chain is degenerate), so please be careful when analysing the results.", RuntimeWarning)
+
     # calculate stationary distributions using eigenvalues and eigenvectors
     # noinspection PyTupleAssignmentBalance
     schur_form, eigenvectors = schur(transition_matrix)
     eigenvalues = eigvals(schur_form)
     index_stationary = np.argmin(abs(eigenvalues - 1.0))  # look for the element closest to 1 in the list of eigenvalues
     sd = abs(eigenvectors[:, index_stationary].T.real)  # it is essential to access the matrix by column
     return sd / sd.sum()  # normalize
```

### Comparing `egttools-0.1.9.dev3/include/egttools/Data.hpp` & `egttools-0.1.9.dev6/include/egttools/Data.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/Distributions.h` & `egttools-0.1.9.dev6/include/egttools/Distributions.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/LruCache.hpp` & `egttools-0.1.9.dev6/include/egttools/LruCache.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/OpenMPUtils.hpp` & `egttools-0.1.9.dev6/include/egttools/OpenMPUtils.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/Sampling.h` & `egttools-0.1.9.dev6/include/egttools/Sampling.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/SeedGenerator.h` & `egttools-0.1.9.dev6/include/egttools/SeedGenerator.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/Types.h` & `egttools-0.1.9.dev6/include/egttools/Types.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/Utils.h` & `egttools-0.1.9.dev6/include/egttools/Utils.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/MLS.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/MLS.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/PairwiseMoran.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/PairwiseMoran.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -626,15 +626,15 @@
                                                            double mu) {
         // First we initialise the container for the stationary distribution
         VectorXui sdist = VectorXui::Zero(_nb_states);
         // Distribution number of generations for a mutation to happen
         std::geometric_distribution<size_t> geometric(mu);
 
 #pragma omp parallel for reduction(+ \
-                                   : sdist) default(none) private(geometric) shared(nb_runs, nb_generations, transitory, beta, mu)
+                                   : sdist) default(none) shared(geometric, nb_runs, nb_generations, transitory, beta, mu)
         for (size_t i = 0; i < nb_runs; ++i) {
             // Random generators - each thread should have its own generator
             std::mt19937_64 generator{egttools::Random::SeedGenerator::getInstance().getSeed()};
 
             // Then we sample a random population state
             VectorXui strategies = VectorXui::Zero(_nb_strategies);
             auto current_state = _state_sampler(generator);
@@ -676,38 +676,38 @@
 
             // Then we start counting
             for (; j < nb_generations; ++j) {
                 // If the strategies are the same, there will be no change in the population
                 if (homogeneous) {
                     k = geometric(generator);
                     // Update state count by k steps
-                    sdist(static_cast<int>(current_state)) += k + 1;
+                    sdist(static_cast<int64_t>(current_state)) += k + 1;
                     mutate_(generator, birth, idx_homo);
 
-                    strategies(static_cast<int>(birth)) += 1;
+                    strategies(static_cast<int64_t>(birth)) += 1;
                     strategies(idx_homo) -= 1;
 
                     // Update state count by 1 step
                     current_state = egttools::FinitePopulations::calculate_state(_pop_size, strategies);
                     // and now update distribution after mutation
-                    ++sdist(static_cast<int>(current_state));
+                    ++sdist(static_cast<int64_t>(current_state));
                     homogeneous = false;
 
                     // Update state count by k steps
                     j += k;
                 } else {
                     // First we pick 2 players randomly
                     _sample_players(strategy_p1, strategy_p2, strategies, generator);
 
                     _update_step(strategy_p1, strategy_p2, beta, mu,
                                  birth, die, homogeneous, idx_homo,
                                  strategies, cache, generator);
                     // Update state count by k steps
                     current_state = egttools::FinitePopulations::calculate_state(_pop_size, strategies);
-                    ++sdist(static_cast<int>(current_state));
+                    ++sdist(static_cast<int64_t>(current_state));
                 }
             }
         }
         return sdist.cast<double>() / (nb_runs * (nb_generations - transitory));
     }
 
     template<class Cache>
@@ -717,15 +717,15 @@
         // First we initialise the container for the stationary distribution
         auto sdist = SparseMatrix2DXui(1, _nb_states);
         //        sdist.reserve(VectorXi::Constant(_nb_states, std::min(10000, static_cast<int>(_nb_states))));
         // Distribution number of generations for a mutation to happen
         std::geometric_distribution<size_t> geometric(mu);
 
 #pragma omp parallel for reduction(+ \
-                                   : sdist) default(none) private(geometric) shared(nb_runs, nb_generations, transitory, beta, mu)
+                                   : sdist) default(none) shared(geometric, nb_runs, nb_generations, transitory, beta, mu)
         for (size_t i = 0; i < nb_runs; ++i) {
             // Random generators - each thread should have its own generator
             std::mt19937_64 generator{egttools::Random::SeedGenerator::getInstance().getSeed()};
 
             // Then we sample a random population state
             VectorXui strategies = VectorXui::Zero(_nb_strategies);
             auto current_state = _state_sampler(generator);
@@ -811,15 +811,15 @@
 
         VectorXui strategy_dist = VectorXui::Zero(_nb_strategies);
 
         // Distribution number of generations for a mutation to happen
         std::geometric_distribution<size_t> geometric(mu);
 
 #pragma omp parallel for reduction(+ \
-                                   : strategy_dist) default(none) private(geometric) shared(nb_runs, nb_generations, transitory, beta, mu)
+                                   : strategy_dist) default(none) shared(geometric, nb_runs, nb_generations, transitory, beta, mu)
         for (size_t i = 0; i < nb_runs; ++i) {
 
             // Random generators - each thread should have its own generator
             std::mt19937_64 generator{egttools::Random::SeedGenerator::getInstance().getSeed()};
 
             // Then we sample a random population state
             VectorXui strategies = VectorXui::Zero(_nb_strategies);
```

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/Utils.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/Utils.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/behaviors/AbstractCRDStrategy.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/behaviors/AbstractCRDStrategy.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/behaviors/AbstractNFGStrategy.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/behaviors/AbstractNFGStrategy.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/behaviors/CRDStrategies.h` & `egttools-0.1.9.dev6/include/egttools/finite_populations/behaviors/CRDStrategies.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/behaviors/NFGStrategies.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/behaviors/NFGStrategies.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/games/AbstractGame.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/games/AbstractGame.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/games/CRDGame.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/games/CRDGame.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/games/CRDGameTU.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/games/CRDGameTU.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/games/NormalFormGame.h` & `egttools-0.1.9.dev6/include/egttools/finite_populations/games/NormalFormGame.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/games/OneShotCRD.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/games/OneShotCRD.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/structure/GarciaGroup.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/structure/GarciaGroup.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/finite_populations/structure/Group.hpp` & `egttools-0.1.9.dev6/include/egttools/finite_populations/structure/Group.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/utils/CalculateExpectedIndicators.h` & `egttools-0.1.9.dev6/include/egttools/utils/CalculateExpectedIndicators.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/include/egttools/utils/TimingUncertainty.hpp` & `egttools-0.1.9.dev6/include/egttools/utils/TimingUncertainty.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.appveyor.yml` & `egttools-0.1.9.dev6/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.clang-tidy` & `egttools-0.1.9.dev6/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.cmake-format.yaml` & `egttools-0.1.9.dev6/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.github/CONTRIBUTING.md` & `egttools-0.1.9.dev6/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `egttools-0.1.9.dev6/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.github/dependabot.yml` & `egttools-0.1.9.dev6/pybind11/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.github/pull_request_template.md` & `egttools-0.1.9.dev6/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.github/workflows/ci.yml` & `egttools-0.1.9.dev6/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.github/workflows/configure.yml` & `egttools-0.1.9.dev6/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.github/workflows/format.yml` & `egttools-0.1.9.dev6/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.github/workflows/pip.yml` & `egttools-0.1.9.dev6/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/.pre-commit-config.yaml` & `egttools-0.1.9.dev6/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/CMakeLists.txt` & `egttools-0.1.9.dev6/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/LICENSE` & `egttools-0.1.9.dev6/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/README.rst` & `egttools-0.1.9.dev6/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/Doxyfile` & `egttools-0.1.9.dev6/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/Makefile` & `egttools-0.1.9.dev6/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/cast/chrono.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/cast/custom.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/cast/eigen.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/cast/functional.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/cast/index.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/cast/overview.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/cast/stl.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/cast/strings.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/classes.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/embedding.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/exceptions.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/functions.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/misc.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/pycpp/numpy.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/pycpp/object.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/pycpp/utilities.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/advanced/smart_ptrs.rst` & `egttools-0.1.9.dev6/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/basics.rst` & `egttools-0.1.9.dev6/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/benchmark.py` & `egttools-0.1.9.dev6/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/benchmark.rst` & `egttools-0.1.9.dev6/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/changelog.rst` & `egttools-0.1.9.dev6/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/classes.rst` & `egttools-0.1.9.dev6/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/compiling.rst` & `egttools-0.1.9.dev6/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/conf.py` & `egttools-0.1.9.dev6/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/faq.rst` & `egttools-0.1.9.dev6/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/index.rst` & `egttools-0.1.9.dev6/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/installing.rst` & `egttools-0.1.9.dev6/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/limitations.rst` & `egttools-0.1.9.dev6/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/pybind11-logo.png` & `egttools-0.1.9.dev6/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/pybind11_vs_boost_python1.png` & `egttools-0.1.9.dev6/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/pybind11_vs_boost_python1.svg` & `egttools-0.1.9.dev6/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/pybind11_vs_boost_python2.png` & `egttools-0.1.9.dev6/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/pybind11_vs_boost_python2.svg` & `egttools-0.1.9.dev6/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/reference.rst` & `egttools-0.1.9.dev6/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/release.rst` & `egttools-0.1.9.dev6/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/docs/upgrade.rst` & `egttools-0.1.9.dev6/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/attr.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/buffer_info.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/cast.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/chrono.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/complex.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/detail/class.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/detail/common.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/detail/descr.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/detail/init.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/detail/internals.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/detail/type_caster_base.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/detail/typeid.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/eigen.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/embed.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/eval.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/functional.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/gil.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/iostream.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/numpy.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/operators.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/options.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/pybind11.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/pytypes.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/stl/filesystem.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/stl.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/include/pybind11/stl_bind.h` & `egttools-0.1.9.dev6/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/noxfile.py` & `egttools-0.1.9.dev6/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/pybind11/__main__.py` & `egttools-0.1.9.dev6/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/pybind11/commands.py` & `egttools-0.1.9.dev6/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/pybind11/setup_helpers.py` & `egttools-0.1.9.dev6/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/pybind11/setup_helpers.pyi` & `egttools-0.1.9.dev6/pybind11/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/pyproject.toml` & `egttools-0.1.9.dev6/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/setup.cfg` & `egttools-0.1.9.dev6/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/setup.py` & `egttools-0.1.9.dev6/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/CMakeLists.txt` & `egttools-0.1.9.dev6/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/conftest.py` & `egttools-0.1.9.dev6/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/constructor_stats.h` & `egttools-0.1.9.dev6/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/cross_module_gil_utils.cpp` & `egttools-0.1.9.dev6/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/env.py` & `egttools-0.1.9.dev6/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/extra_python_package/test_files.py` & `egttools-0.1.9.dev6/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/extra_setuptools/test_setuphelper.py` & `egttools-0.1.9.dev6/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/local_bindings.h` & `egttools-0.1.9.dev6/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/object.h` & `egttools-0.1.9.dev6/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/pybind11_cross_module_tests.cpp` & `egttools-0.1.9.dev6/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/pybind11_tests.cpp` & `egttools-0.1.9.dev6/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/pybind11_tests.h` & `egttools-0.1.9.dev6/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/pytest.ini` & `egttools-0.1.9.dev6/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/requirements.txt` & `egttools-0.1.9.dev6/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_async.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_async.py` & `egttools-0.1.9.dev6/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_buffers.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_buffers.py` & `egttools-0.1.9.dev6/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_builtin_casters.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_builtin_casters.py` & `egttools-0.1.9.dev6/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_call_policies.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_call_policies.py` & `egttools-0.1.9.dev6/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_callbacks.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_callbacks.py` & `egttools-0.1.9.dev6/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_chrono.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_chrono.py` & `egttools-0.1.9.dev6/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_class.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_class.py` & `egttools-0.1.9.dev6/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/CMakeLists.txt` & `egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/embed.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `egttools-0.1.9.dev6/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_constants_and_functions.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_constants_and_functions.py` & `egttools-0.1.9.dev6/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_copy_move.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_copy_move.py` & `egttools-0.1.9.dev6/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_custom_type_casters.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_custom_type_casters.py` & `egttools-0.1.9.dev6/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_custom_type_setup.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_custom_type_setup.py` & `egttools-0.1.9.dev6/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_docstring_options.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_docstring_options.py` & `egttools-0.1.9.dev6/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_eigen.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_eigen.py` & `egttools-0.1.9.dev6/pybind11/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_embed/CMakeLists.txt` & `egttools-0.1.9.dev6/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_embed/catch.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_embed/external_module.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_embed/test_interpreter.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_enum.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_enum.py` & `egttools-0.1.9.dev6/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_eval.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_eval.py` & `egttools-0.1.9.dev6/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_exceptions.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_exceptions.py` & `egttools-0.1.9.dev6/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_factory_constructors.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_factory_constructors.py` & `egttools-0.1.9.dev6/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_gil_scoped.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_gil_scoped.py` & `egttools-0.1.9.dev6/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_iostream.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_iostream.py` & `egttools-0.1.9.dev6/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_kwargs_and_defaults.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_kwargs_and_defaults.py` & `egttools-0.1.9.dev6/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_local_bindings.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_local_bindings.py` & `egttools-0.1.9.dev6/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_methods_and_attributes.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_methods_and_attributes.py` & `egttools-0.1.9.dev6/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_modules.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_modules.py` & `egttools-0.1.9.dev6/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_multiple_inheritance.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_multiple_inheritance.py` & `egttools-0.1.9.dev6/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_numpy_array.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_numpy_array.py` & `egttools-0.1.9.dev6/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_numpy_dtypes.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_numpy_dtypes.py` & `egttools-0.1.9.dev6/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_numpy_vectorize.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_numpy_vectorize.py` & `egttools-0.1.9.dev6/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_opaque_types.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_opaque_types.py` & `egttools-0.1.9.dev6/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_operator_overloading.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_operator_overloading.py` & `egttools-0.1.9.dev6/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_pickling.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_pickling.py` & `egttools-0.1.9.dev6/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_pytypes.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_pytypes.py` & `egttools-0.1.9.dev6/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_sequences_and_iterators.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_sequences_and_iterators.py` & `egttools-0.1.9.dev6/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_smart_ptr.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_smart_ptr.py` & `egttools-0.1.9.dev6/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_stl.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_stl.py` & `egttools-0.1.9.dev6/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_stl_binders.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_stl_binders.py` & `egttools-0.1.9.dev6/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_tagbased_polymorphic.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_tagbased_polymorphic.py` & `egttools-0.1.9.dev6/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_thread.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_thread.py` & `egttools-0.1.9.dev6/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_union.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_virtual_functions.cpp` & `egttools-0.1.9.dev6/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/test_virtual_functions.py` & `egttools-0.1.9.dev6/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/valgrind-numpy-scipy.supp` & `egttools-0.1.9.dev6/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tests/valgrind-python.supp` & `egttools-0.1.9.dev6/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/FindCatch.cmake` & `egttools-0.1.9.dev6/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/FindEigen3.cmake` & `egttools-0.1.9.dev6/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/FindPythonLibsNew.cmake` & `egttools-0.1.9.dev6/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/check-style.sh` & `egttools-0.1.9.dev6/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/cmake_uninstall.cmake.in` & `egttools-0.1.9.dev6/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/libsize.py` & `egttools-0.1.9.dev6/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/make_changelog.py` & `egttools-0.1.9.dev6/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/pybind11Common.cmake` & `egttools-0.1.9.dev6/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/pybind11Config.cmake.in` & `egttools-0.1.9.dev6/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/pybind11NewTools.cmake` & `egttools-0.1.9.dev6/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/pybind11Tools.cmake` & `egttools-0.1.9.dev6/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/setup_global.py.in` & `egttools-0.1.9.dev6/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/pybind11/tools/setup_main.py.in` & `egttools-0.1.9.dev6/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/res/cmake/Modules/FindEigen3.cmake` & `egttools-0.1.9.dev6/res/cmake/Modules/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/res/cmake/Modules/FindLpSolve.cmake` & `egttools-0.1.9.dev6/res/cmake/Modules/FindLpSolve.cmake`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/setup.cfg` & `egttools-0.1.9.dev6/setup.cfg`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/setup.py` & `egttools-0.1.9.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/CMakeLists.txt` & `egttools-0.1.9.dev6/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/CMakeLists.txt` & `egttools-0.1.9.dev6/src/egttools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/Data.cpp` & `egttools-0.1.9.dev6/src/egttools/Data.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/Distributions.cpp` & `egttools-0.1.9.dev6/src/egttools/Distributions.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/SeedGenerator.cpp` & `egttools-0.1.9.dev6/src/egttools/SeedGenerator.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/CMakeLists.txt` & `egttools-0.1.9.dev6/src/egttools/finite_populations/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/MLS.cpp` & `egttools-0.1.9.dev6/src/egttools/finite_populations/MLS.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/Utils.cpp` & `egttools-0.1.9.dev6/src/egttools/finite_populations/Utils.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/behaviors/CRDStrategies.cpp` & `egttools-0.1.9.dev6/src/egttools/finite_populations/behaviors/CRDStrategies.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/behaviors/NFGStrategies.cpp` & `egttools-0.1.9.dev6/src/egttools/finite_populations/behaviors/NFGStrategies.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/games/CRDGame.cpp` & `egttools-0.1.9.dev6/src/egttools/finite_populations/games/CRDGame.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/games/CRDGameTU.cpp` & `egttools-0.1.9.dev6/src/egttools/finite_populations/games/CRDGameTU.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/games/NormalFormGame.cpp` & `egttools-0.1.9.dev6/src/egttools/finite_populations/games/NormalFormGame.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/games/OneShotCRD.cpp` & `egttools-0.1.9.dev6/src/egttools/finite_populations/games/OneShotCRD.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/structure/GarciaGroup.cpp` & `egttools-0.1.9.dev6/src/egttools/finite_populations/structure/GarciaGroup.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/finite_populations/structure/Group.cpp` & `egttools-0.1.9.dev6/src/egttools/finite_populations/structure/Group.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/utils/CMakeLists.txt` & `egttools-0.1.9.dev6/src/egttools/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools/utils/CalculateExpectedIndicators.cpp` & `egttools-0.1.9.dev6/src/egttools/utils/CalculateExpectedIndicators.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/egttools.cpp` & `egttools-0.1.9.dev6/src/egttools.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,15 @@
                     --------
                     egttools.games.AbstractGame,
                     egttools.games.CRDGame,
                     egttools.games.CRDGameTU,
                     egttools.behaviors.NormalForm.TwoActions
                     )pbdoc",
                  py::arg("nb_rounds"),
-                 py::arg("payoff_matrix"))
+                 py::arg("payoff_matrix"), py::return_value_policy::reference_internal)
             .def(py::init(&egttools::init_normal_form_game_from_python_list),
                  R"pbdoc(
                     Normal Form Game. This constructor allows you to define any number of strategies
                     by passing a list of pointers to them. All strategies must by of type AbstractNFGStrategy *.
 
                     Parameters
                     ----------
@@ -637,15 +637,15 @@
                  R"pbdoc(
                     Returns the payoff matrix of the game.
 
                     Returns
                     -------
                     numpy.ndarray
                         The payoff matrix.
-                    )pbdoc")
+                    )pbdoc", py::return_value_policy::reference_internal)
             .def("payoff", &egttools::FinitePopulations::NormalFormGame::payoff,
                  R"pbdoc(
                     Returns the payoff of a strategy given a strategy pair.
 
                     If the group composition does not include the strategy, the payoff should be zero.
 
                     Parameters
@@ -658,15 +658,15 @@
 
                     Returns
                     -------
                     float
                         The payoff value.
                     )pbdoc", py::arg("strategy"),
                  py::arg("strategy_pair"))
-            .def("expected_payoffs", &egttools::FinitePopulations::NormalFormGame::expected_payoffs, "returns the expected payoffs of each strategy vs another")
+            .def("expected_payoffs", &egttools::FinitePopulations::NormalFormGame::expected_payoffs, "returns the expected payoffs of each strategy vs another", py::return_value_policy::reference_internal)
             .def("nb_strategies", &egttools::FinitePopulations::NormalFormGame::nb_strategies,
                  "Number of different strategies which are playing the game.")
             .def_property_readonly("nb_rounds", &egttools::FinitePopulations::NormalFormGame::nb_rounds,
                                    "Number of rounds of the game.")
             .def_property_readonly("nb_states", &egttools::FinitePopulations::NormalFormGame::nb_states,
                                    "Number of combinations of 2 strategies that can be matched in the game.")
             .def_property_readonly("strategies", &egttools::FinitePopulations::NormalFormGame::strategies,
```

### Comparing `egttools-0.1.9.dev3/src/egttools.h` & `egttools-0.1.9.dev6/src/egttools.h`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/python_stubs.hpp` & `egttools-0.1.9.dev6/src/python_stubs.hpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/src/version.h` & `egttools-0.1.9.dev6/src/version.h`

 * *Files 1% similar despite different names*

```diff
@@ -14,10 +14,10 @@
   *
   * You should have received a copy of the GNU General Public License
   * along with EGTtools.  If not, see <http://www.gnu.org/licenses/>
 */
 #ifndef EGTTOOLS_VERSION_H
 #define EGTTOOLS_VERSION_H
 
-#define EGTTOOLS_VERSION 0.1.9.dev3
+#define EGTTOOLS_VERSION 0.1.9.dev6
 
 #endif//EGTTOOLS_VERSION_H
```

### Comparing `egttools-0.1.9.dev3/tests/CMakeLists.txt` & `egttools-0.1.9.dev6/tests/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,19 @@
 #        POSITION_INDEPENDENT_CODE TRUE
 #         Fixing "ld: warning: direct access in function '...' from file '...' to global weak symbol '...' from file '...' means the weak symbol cannot
 #         be overridden at runtime. This was likely caused by different translation units being compiled with different visibility settings."
 #        C_VISIBILITY_PRESET hidden
 #        CXX_VISIBILITY_PRESET hidden
         )
 
+#if (OPENMP_FOUND)
+#    target_link_libraries(egttoolsNumerical OpenMP::OpenMP_CXX)
+#else ()
 target_link_libraries(egttoolsNumerical)
+#endif()
 
 add_executable(testPMrun test_PairwiseMoran_run.cpp)
 #set_target_properties(testPM PROPERTIES INTERPROCEDURAL_OPTIMIZATION ${LTO_SUPPORTED})
 target_link_libraries(testPMrun egttoolsNumerical)
 
 add_executable(testPMBstationary_distribution_sparse test_PairwiseMoran_stationary_distribution_sparse.cpp)
 #set_target_properties(testPM PROPERTIES INTERPROCEDURAL_OPTIMIZATION ${LTO_SUPPORTED})
```

### Comparing `egttools-0.1.9.dev3/tests/conftest.py` & `egttools-0.1.9.dev6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_PairwiseMoran_run.cpp` & `egttools-0.1.9.dev6/tests/test_PairwiseMoran_run.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_PairwiseMoran_stationary_distribution_dense.cpp` & `egttools-0.1.9.dev6/tests/test_PairwiseMoran_stationary_distribution_dense.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_PairwiseMoran_stationary_distribution_sparse.cpp` & `egttools-0.1.9.dev6/tests/test_PairwiseMoran_stationary_distribution_sparse.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     egttools::FinitePopulations::NormalFormGame game(nb_rounds, payoff_matrix, strategies);
 
     // Initialise selection mutation process
     auto smProcess = egttools::FinitePopulations::PairwiseMoran(pop_size, game, 100000);
 
     auto start = high_resolution_clock::now();
 
-    auto dist = smProcess.estimate_stationary_distribution_sparse(5, 1000000, 1000, 10, 1e-3);
+    auto dist = smProcess.estimate_stationary_distribution_sparse(7, 1000000, 1000, 10, 1e-3);
 
     auto stop = high_resolution_clock::now();
     auto duration = duration_cast<microseconds>(stop - start);
     std::cout << "Time taken by function: "
               << duration.count() << " microseconds" << std::endl;
 
     assert(dist.cols() == static_cast<long>(nb_states));
```

### Comparing `egttools-0.1.9.dev3/tests/test_crd_game.cpp` & `egttools-0.1.9.dev6/tests/test_crd_game.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_crd_tu_game.cpp` & `egttools-0.1.9.dev6/tests/test_crd_tu_game.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_eigen_sparse_matrix.cpp` & `egttools-0.1.9.dev6/tests/test_eigen_sparse_matrix.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_mc_simulations.py` & `egttools-0.1.9.dev6/tests/test_mc_simulations.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_numerical.py` & `egttools-0.1.9.dev6/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_openmp.py` & `egttools-0.1.9.dev6/tests/test_openmp.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,10 +20,14 @@
         [0, (V / 2) - T],
     ])
 
     game = egt.games.NormalFormGame(1, A)
     assert game.type() == 'NormalFormGame'
 
     evolver = egt.numerical.PairwiseMoran(Z, game, 1000)
-    dist = evolver.estimate_stationary_distribution_sparse(1, 100000, 1000, 1, 1e-3)
+    dist = evolver.estimate_stationary_distribution_sparse(10, 100000, 1000, 1, 1e-3)
 
-    assert dist.toarray().shape == (1, Z+1)
+    assert dist.toarray().shape == (1, Z + 1)
+
+
+if __name__ == "__main__":
+    test_openmp_simulations()
```

### Comparing `egttools-0.1.9.dev3/tests/test_ordered_sampling_without_replacement.cpp` & `egttools-0.1.9.dev6/tests/test_ordered_sampling_without_replacement.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_timing_uncertainty.cpp` & `egttools-0.1.9.dev6/tests/test_timing_uncertainty.cpp`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_utils.py` & `egttools-0.1.9.dev6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `egttools-0.1.9.dev3/tests/test_virtual_functions.py` & `egttools-0.1.9.dev6/tests/test_virtual_functions.py`

 * *Files identical despite different names*

