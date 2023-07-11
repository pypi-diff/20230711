# Comparing `tmp/mccoygroup-psience-0.0.9.tar.gz` & `tmp/mccoygroup-psience-0.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccoygroup-psience-0.0.9.tar", last modified: Wed Jul  5 17:52:07 2023, max compression
+gzip compressed data, was "mccoygroup-psience-0.0.9.1.tar", last modified: Tue Jul 11 18:54:10 2023, max compression
```

## Comparing `mccoygroup-psience-0.0.9.tar` & `mccoygroup-psience-0.0.9.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.682384 mccoygroup-psience-0.0.9/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-05 17:52:07.682384 mccoygroup-psience-0.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/AIMD/
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AIMD/Simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AIMD/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/AnalyticModels/
--rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43001 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AnalyticModels/AnalyticModelConstructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AnalyticModels/Helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/AnalyticModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/BasisReps/
--rwxr-xr-x   0 runner    (1001) docker     (123)    18017 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/Bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/ClassicalBases.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30348 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/HarmonicOscillator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51651 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/Operators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46924 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/Representations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/StateFilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/StateIndexers.py
--rw-r--r--   0 runner    (1001) docker     (123)   184429 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/StateSpaces.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10328 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/BasisReps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/DGB/
--rw-r--r--   0 runner    (1001) docker     (123)    76300 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DGB/DGB.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DGB/Wavefunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DGB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.674384 mccoygroup-psience-0.0.9/Psience/DVR/
--rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/BaseDVR.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/ColbertMiller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/DVR.py
--rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/DirectProduct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/FiniteBasisDVR.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6770 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/DVR/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/Data/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Data/KEData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/Data/PsiDatasets/
--rw-r--r--   0 runner    (1001) docker     (123)    28550 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Data/PsiDatasets/KEData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Data/PsiDatasets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10276 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Data/Surfaces.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/Molecools/
--rwxr-xr-x   0 runner    (1001) docker     (123)    27306 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/CoordinateSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)    37771 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/MolecularFunctionExpansion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55296 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/Molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/MoleculeInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    68334 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/Properties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/Transformations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20193 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/Vibrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Molecools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/Spectra/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14581 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Spectra/BaseSpectrum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      170 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Spectra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/VPT2/
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Analyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      692 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Common.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    45549 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/DegeneracySpecs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49293 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    86022 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    99465 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Solver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   128543 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Terms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    77064 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3756 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VPT2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/VSCF/
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VSCF/VSCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/VSCF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.678384 mccoygroup-psience-0.0.9/Psience/Wavefun/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Wavefun/DirectProduct.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11061 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Wavefun/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/Wavefun/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/Psience/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3079 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:52:07.682384 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-05 17:52:07.000000 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-05 17:52:07.000000 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:52:07.000000 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 17:52:07.000000 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 17:52:07.000000 mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 17:52:07.682384 mccoygroup-psience-0.0.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-07-05 17:51:56.000000 mccoygroup-psience-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.848983 mccoygroup-psience-0.0.9.1/Psience/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.848983 mccoygroup-psience-0.0.9.1/Psience/AIMD/
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AIMD/Simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AIMD/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.848983 mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/
+-rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43001 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/AnalyticModelConstructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/Helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.848983 mccoygroup-psience-0.0.9.1/Psience/BasisReps/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18017 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/Bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/ClassicalBases.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30900 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/HarmonicOscillator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51651 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/Operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46924 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/Representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateFilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateIndexers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   184560 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateSpaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10328 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/DGB/
+-rw-r--r--   0 runner    (1001) docker     (123)    76300 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DGB/DGB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DGB/Wavefunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DGB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/DVR/
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/BaseDVR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/ColbertMiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/DVR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/DirectProduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/FiniteBasisDVR.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6770 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/Data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Data/KEData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/Data/PsiDatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    28550 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Data/PsiDatasets/KEData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Data/PsiDatasets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10276 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Data/Surfaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/Molecools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27306 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/CoordinateSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37771 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/MolecularFunctionExpansion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55296 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/Molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/MoleculeInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68334 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/Properties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/Transformations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20193 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/Vibrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/Spectra/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14581 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Spectra/BaseSpectrum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      170 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Spectra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/VPT2/
+-rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Analyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      692 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45597 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/DegeneracySpecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49402 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86022 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99465 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Solver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   128543 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Terms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77064 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3756 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/Psience/VSCF/
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VSCF/VSCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VSCF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/Psience/Wavefun/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Wavefun/DirectProduct.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11061 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Wavefun/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Wavefun/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3079 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-11 18:54:10.000000 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-11 18:54:10.000000 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:54:10.000000 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 18:54:10.000000 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 18:54:10.000000 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/setup.py
```

### Comparing `mccoygroup-psience-0.0.9/LICENSE.txt` & `mccoygroup-psience-0.0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/PKG-INFO` & `mccoygroup-psience-0.0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-psience
-Version: 0.0.9
+Version: 0.0.9.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # Psience [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/McCoyGroup/Binder-McUtils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252FMcCoyGroup%252FPsience%26urlpath%3Dlab%252Ftree%252FPsience%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-psience-0.0.9/Psience/AIMD/Simulator.py` & `mccoygroup-psience-0.0.9.1/Psience/AIMD/Simulator.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py` & `mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/AnalyticModels/AnalyticModelConstructors.py` & `mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/AnalyticModelConstructors.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/AnalyticModels/Helpers.py` & `mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/Helpers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/BasisReps/Bases.py` & `mccoygroup-psience-0.0.9.1/Psience/BasisReps/Bases.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/BasisReps/ClassicalBases.py` & `mccoygroup-psience-0.0.9.1/Psience/BasisReps/ClassicalBases.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/BasisReps/HarmonicOscillator.py` & `mccoygroup-psience-0.0.9.1/Psience/BasisReps/HarmonicOscillator.py`

 * *Files 3% similar despite different names*

```diff
@@ -334,14 +334,15 @@
         else:
             p_pos = []
             for i, o in enumerate(terms):
                 if o == "p":
                     p_pos.append(i)
             self.p_pos = tuple(p_pos)
         self._state_group_cache = MaxSizeCache(self.state_cache_size)
+        self._poly_cache = {}
 
     def __repr__(self):
         return "{}({})".format(
             type(self).__name__,
             ", ".join(self.terms)
         )
 
@@ -544,14 +545,25 @@
                     poly = np.pad(poly, [0, len(poly_contrib)-len(poly)])
                 elif len(poly_contrib) < len(poly):
                     poly_contrib = np.pad(poly_contrib, [0, len(poly)-len(poly_contrib)])
                 poly = poly + poly_contrib
 
         return poly / np.sqrt(2)**len(terms)
 
+    def poly_coeffs(self, delta, shift=0):
+        if (delta, shift) not in self._poly_cache:
+            if delta not in self._poly_cache:
+                self._poly_cache[delta] = self._get_poly_coeffs(self.terms, delta)
+            if shift != 0:
+                self._poly_cache[(delta, shift)] = DensePolynomial._compute_shifted_coeffs(self._poly_cache[delta], shift=shift)
+            else:
+                self._poly_cache[(delta, shift)] = self._poly_cache[delta]
+        return self._poly_cache[(delta, shift)]
+
+
     @classmethod
     def get_poly_coeffs(cls, terms, delta, shift=0):
         coeffs = cls._get_poly_coeffs(terms, delta)
         if shift != 0:
             coeffs = DensePolynomial._compute_shifted_coeffs(coeffs, shift=shift)
         return coeffs
```

### Comparing `mccoygroup-psience-0.0.9/Psience/BasisReps/Operators.py` & `mccoygroup-psience-0.0.9.1/Psience/BasisReps/Operators.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/BasisReps/Representations.py` & `mccoygroup-psience-0.0.9.1/Psience/BasisReps/Representations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/BasisReps/StateFilters.py` & `mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateFilters.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/BasisReps/StateIndexers.py` & `mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateIndexers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/BasisReps/StateSpaces.py` & `mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateSpaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,17 +679,19 @@
             return np.reshape(states, (-1, self.ndim))
         elif states_type is self.StateSpaceSpec.Indices:
             if self.full_basis is not None:
                 if self._max_ind is None:
                     self._max_ind = np.max(self.indices)
                 return self.full_basis.take(self.indices, max_size=self._max_ind, uncoerce=False)
 
+            # print(">>>", states.flatten().dtype, states.flatten())
             states, self._indexer, uinds, inv = nput.unique(states, sorting=self._indexer, return_index=True, return_inverse=True)
             self._sort_uinds = uinds
             self._uinds = np.sort(uinds)
+            # print(states.flatten().dtype, states.flatten())
             raw_exc = self.basis.unravel_state_inds(states.flatten())
             return raw_exc[inv]
         else:
             raise ValueError("don't know what to do with state spec {}".format(
                 states_type
             ))
```

### Comparing `mccoygroup-psience-0.0.9/Psience/BasisReps/Wavefunctions.py` & `mccoygroup-psience-0.0.9.1/Psience/BasisReps/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/BasisReps/__init__.py` & `mccoygroup-psience-0.0.9.1/Psience/BasisReps/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/DGB/DGB.py` & `mccoygroup-psience-0.0.9.1/Psience/DGB/DGB.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/DGB/Wavefunctions.py` & `mccoygroup-psience-0.0.9.1/Psience/DGB/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/DVR/BaseDVR.py` & `mccoygroup-psience-0.0.9.1/Psience/DVR/BaseDVR.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/DVR/ColbertMiller.py` & `mccoygroup-psience-0.0.9.1/Psience/DVR/ColbertMiller.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/DVR/DVR.py` & `mccoygroup-psience-0.0.9.1/Psience/DVR/DVR.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/DVR/DirectProduct.py` & `mccoygroup-psience-0.0.9.1/Psience/DVR/DirectProduct.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/DVR/Extensions.py` & `mccoygroup-psience-0.0.9.1/Psience/DVR/Extensions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/DVR/FiniteBasisDVR.py` & `mccoygroup-psience-0.0.9.1/Psience/DVR/FiniteBasisDVR.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/DVR/Wavefunctions.py` & `mccoygroup-psience-0.0.9.1/Psience/DVR/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/DVR/__init__.py` & `mccoygroup-psience-0.0.9.1/Psience/DVR/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Data/KEData.py` & `mccoygroup-psience-0.0.9.1/Psience/Data/KEData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Data/PsiDatasets/KEData.py` & `mccoygroup-psience-0.0.9.1/Psience/Data/PsiDatasets/KEData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Data/Surfaces.py` & `mccoygroup-psience-0.0.9.1/Psience/Data/Surfaces.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Data/__init__.py` & `mccoygroup-psience-0.0.9.1/Psience/Data/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Molecools/CoordinateSystems.py` & `mccoygroup-psience-0.0.9.1/Psience/Molecools/CoordinateSystems.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Molecools/MolecularFunctionExpansion.py` & `mccoygroup-psience-0.0.9.1/Psience/Molecools/MolecularFunctionExpansion.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Molecools/Molecule.py` & `mccoygroup-psience-0.0.9.1/Psience/Molecools/Molecule.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Molecools/MoleculeInterface.py` & `mccoygroup-psience-0.0.9.1/Psience/Molecools/MoleculeInterface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Molecools/Properties.py` & `mccoygroup-psience-0.0.9.1/Psience/Molecools/Properties.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Molecools/Transformations.py` & `mccoygroup-psience-0.0.9.1/Psience/Molecools/Transformations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Molecools/Vibrations.py` & `mccoygroup-psience-0.0.9.1/Psience/Molecools/Vibrations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Spectra/BaseSpectrum.py` & `mccoygroup-psience-0.0.9.1/Psience/Spectra/BaseSpectrum.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/VPT2/Analyzer.py` & `mccoygroup-psience-0.0.9.1/Psience/VPT2/Analyzer.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/VPT2/Common.py` & `mccoygroup-psience-0.0.9.1/Psience/VPT2/Common.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/VPT2/Corrections.py` & `mccoygroup-psience-0.0.9.1/Psience/VPT2/Corrections.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/VPT2/DegeneracySpecs.py` & `mccoygroup-psience-0.0.9.1/Psience/VPT2/DegeneracySpecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,18 +425,24 @@
             else:
                 groups[n] = [i]
 
         if extra_groups is None:
             extra_groups = []
         extra_groups = [(indexer.to_indices(g), np.asanyarray(g)) for g in extra_groups]
 
+        # print("premerge groups:", groups)
+
         groups = PermutationRelationGraph.merge_groups(
             [(g, indexer.from_indices(g)) for g in groups] + extra_groups
         )
 
+        # print("????", [g[0] for g in groups]) # need to track down why we're getting a negative index here
+                              # presumably from an integer overflow in a int8 or a conversion
+                              # of some sort...
+
         return [g[1] for g in groups]
 
 class GroupsDegeneracySpec(DegeneracySpec):
     """
 
     """
 
@@ -580,22 +586,14 @@
                                                      max_sum=max_quanta,
                                                      max_iterations=iterations,
                                                      raise_iteration_error=require_converged
                                                      ))
                     _.append(sub)
                 groups = _
         groups = [g for g in groups if len(g) > 1]
-        # new = []
-        # for g in groups:
-        #     inds = SymmetricGroupGenerator(len(g[0])).to_indices(g)
-        #     print(inds)
-        #     print(g)
-        #     print("-"*50)
-        #     new.append(g[np.argsort(inds)])
-        # groups = new
         return groups
 
     @staticmethod
     def _is_polyad_rule(d, n_modes):
         try:
             return (
                     len(d) == 2
@@ -777,17 +775,14 @@
                 state_inds = states.find(group, dtype=int, missing_val=len(states))
                 found_pos = state_inds < len(states)
                 found_states = state_inds[found_pos]
                 kill_spots = (np.arange(len(group_inds))[found_pos], found_states)
                 corrections = np.abs(corrections[:, group_inds].asarray().T)
                 max_corr = None
                 corrections[kill_spots] = 0
-                # print(group.excitations)
-                # print(states.excitations)
-                # raise Exception(corrections)
                 if max_corr is None:
                     max_corr = np.max(corrections, axis=1)
                 else:
                     submax = np.max(corrections, axis=1)
                     p = submax > max_corr
                     max_corr[p] = submax[p]
                 if threshold is not None:
@@ -811,16 +806,14 @@
                 bad_pos = np.where(np.logical_and(
                     diff_sums == 1,
                     tots_sums > 0
                 ))  # np.logical_or(diff_sums == 1, diff_sums == 0))
             else:
                 e_vec = energies[group_inds]
                 bad_pos = np.where(np.abs(np.subtract.outer(e_vec, e_vec)) > energy_cutoff)
-                # print(">>>", group.excitations)
-                # print(bad_pos)
             if len(bad_pos) > 0 and len(bad_pos[0]) > 0:
                 N = len(group_inds)
                 base_corr = corrections
                 base_vals = base_corr[:, state_inds[found_pos]]
                 base_mat = np.zeros((N, N), dtype=float)
                 base_mat[:, np.where(found_pos)[0]] = base_vals
                 base_mat = (base_mat.T + base_mat) - 2*np.diag(np.diag(base_mat))
@@ -1026,14 +1019,19 @@
 
                 degenerate_states = [
                     BasisStateSpace(states.basis, s)#.as_sorted(track_indices=False, track_excitations=False)
                     if not isinstance(s, BasisStateSpace) else s
                     for s in degenerate_states
                 ]
 
+                # dds = [d.indices for d in degenerate_states]
+                # neg_ps = [i for i,d in enumerate(dds) if np.any(d < 0)]
+
+                # print("DD:", neg_ps, [degenerate_states[i].excitations for i in neg_ps])
+
                 if log_groups:
                     with logger.block(tag="initial degenerate groups:"):
                         for g in degenerate_states:
                             if len(g) > 1:
                                 logger.log_print(str(g.excitations).splitlines())
                 else:
                     logger.log_print(
```

### Comparing `mccoygroup-psience-0.0.9/Psience/VPT2/Hamiltonian.py` & `mccoygroup-psience-0.0.9.1/Psience/VPT2/Hamiltonian.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,14 +368,15 @@
             elif V is None:
                 self._expansions[o] = T
             else:
                 self._expansions[o] = T + V
             if o > 1:
                 oz = o - 2
                 if include_coriolis:
+                    #TODO: nail down exactly how the 4-th and higher-order extensions of this really work...
                     Z = self.coriolis_terms[oz]
                     if Z is not None:
                         if o > 0 and  isinstance(Z, np.ndarray) and excluded_modes is not None:
                             Z = Z.copy()
                             zero_sel = np.ix_(*[excluded_modes] * Z.ndim)
                             Z[zero_sel] = 0.
```

### Comparing `mccoygroup-psience-0.0.9/Psience/VPT2/Runner.py` & `mccoygroup-psience-0.0.9.1/Psience/VPT2/Runner.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/VPT2/Solver.py` & `mccoygroup-psience-0.0.9.1/Psience/VPT2/Solver.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/VPT2/Terms.py` & `mccoygroup-psience-0.0.9.1/Psience/VPT2/Terms.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/VPT2/Wavefunctions.py` & `mccoygroup-psience-0.0.9.1/Psience/VPT2/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/VPT2/__init__.py` & `mccoygroup-psience-0.0.9.1/Psience/VPT2/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/VSCF/VSCF.py` & `mccoygroup-psience-0.0.9.1/Psience/VSCF/VSCF.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Wavefun/DirectProduct.py` & `mccoygroup-psience-0.0.9.1/Psience/Wavefun/DirectProduct.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/Wavefun/Wavefunctions.py` & `mccoygroup-psience-0.0.9.1/Psience/Wavefun/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/Psience/__init__.py` & `mccoygroup-psience-0.0.9.1/Psience/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/README.md` & `mccoygroup-psience-0.0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/PKG-INFO` & `mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-psience
-Version: 0.0.9
+Version: 0.0.9.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # Psience [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/McCoyGroup/Binder-McUtils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252FMcCoyGroup%252FPsience%26urlpath%3Dlab%252Ftree%252FPsience%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-psience-0.0.9/mccoygroup_psience.egg-info/SOURCES.txt` & `mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9/setup.py` & `mccoygroup-psience-0.0.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     packages=find_packages(),
 
     # Optional include package data to ship with your package
     # Customize MANIFEST.in if the general case does not suit your needs
     # Comment out this line to prevent the files from being packaged with your software
     # include_package_data=True
     install_requires=[
-        'mccoygroup-mcutils>=0.1.1'
+        'mccoygroup-mcutils>=0.1.1.1'
     ]
 )
```

