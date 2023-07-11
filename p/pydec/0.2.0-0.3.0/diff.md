# Comparing `tmp/pydec-0.2.0.tar.gz` & `tmp/pydec-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydec-0.2.0.tar", last modified: Mon Feb  6 15:54:05 2023, max compression
+gzip compressed data, was "pydec-0.3.0.tar", last modified: Tue Jul 11 12:27:20 2023, max compression
```

## Comparing `pydec-0.2.0.tar` & `pydec-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:54:05.197049 pydec-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-06 15:53:54.000000 pydec-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-02-06 15:54:05.197049 pydec-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-02-06 15:53:54.000000 pydec-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:54:05.189049 pydec-0.2.0/pydec/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/_composition_str.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:54:05.193049 pydec-0.2.0/pydec/autotracing/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/autotracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/autotracing/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/autotracing/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/autotracing/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/autotracing/tracing_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    52985 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/composition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:54:05.193049 pydec-0.2.0/pydec/decomposition/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19295 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/decomposition/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/decomposition/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/error_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/exception_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:54:05.193049 pydec-0.2.0/pydec/nn/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/nn/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:54:05.197049 pydec-0.2.0/pydec/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/nn/modules/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/nn/modules/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/nn/modules/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/nn/modules/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/nn/modules/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26233 2023-02-06 15:53:54.000000 pydec-0.2.0/pydec/variable_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:54:05.189049 pydec-0.2.0/pydec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-02-06 15:54:05.000000 pydec-0.2.0/pydec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-06 15:54:05.000000 pydec-0.2.0/pydec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 15:54:05.000000 pydec-0.2.0/pydec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-06 15:54:05.000000 pydec-0.2.0/pydec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-06 15:54:05.000000 pydec-0.2.0/pydec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 15:54:05.197049 pydec-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-02-06 15:53:54.000000 pydec-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 15:54:05.197049 pydec-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-06 15:53:54.000000 pydec-0.2.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-02-06 15:53:54.000000 pydec-0.2.0/test/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-02-06 15:53:54.000000 pydec-0.2.0/test/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-02-06 15:53:54.000000 pydec-0.2.0/test/test_nn_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-02-06 15:53:54.000000 pydec-0.2.0/test/test_variable_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.533491 pydec-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-11 12:27:10.000000 pydec-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-07-11 12:27:20.533491 pydec-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-11 12:27:10.000000 pydec-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.529491 pydec-0.3.0/pydec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49509 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/_composition_str.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.529491 pydec-0.3.0/pydec/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.529491 pydec-0.3.0/pydec/core/decBLAS/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/core/decBLAS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/core/decBLAS/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.529491 pydec-0.3.0/pydec/core/decMVF/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/core/decMVF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/core/decMVF/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/core/decMVF/shapley.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.533491 pydec-0.3.0/pydec/core/decOVF/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/core/decOVF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/core/decOVF/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/core/decOVF/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/core/decOVF/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/exception_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.533491 pydec-0.3.0/pydec/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34210 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/nn/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.533491 pydec-0.3.0/pydec/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/nn/modules/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/nn/modules/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/nn/modules/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/nn/modules/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/nn/modules/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.533491 pydec-0.3.0/pydec/nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/nn/utils/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68392 2023-07-11 12:27:10.000000 pydec-0.3.0/pydec/variable_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.529491 pydec-0.3.0/pydec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-07-11 12:27:20.000000 pydec-0.3.0/pydec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-11 12:27:20.000000 pydec-0.3.0/pydec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:27:20.000000 pydec-0.3.0/pydec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 12:27:20.000000 pydec-0.3.0/pydec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 12:27:20.000000 pydec-0.3.0/pydec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:27:20.533491 pydec-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-11 12:27:10.000000 pydec-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:27:20.533491 pydec-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 12:27:10.000000 pydec-0.3.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-07-11 12:27:10.000000 pydec-0.3.0/test/_composition_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-11 12:27:10.000000 pydec-0.3.0/test/decomposition_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-11 12:27:10.000000 pydec-0.3.0/test/variable_functions_test.py
```

### Comparing `pydec-0.2.0/LICENSE` & `pydec-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydec-0.2.0/PKG-INFO` & `pydec-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydec
-Version: 0.2.0
+Version: 0.3.0
 Summary: Linear decomposition toolkit for neural network based on pytorch.
 Home-page: https://github.com/DoubleVII/pydec/
 Author: Sen Yang
 Author-email: yangsen@smail.nju.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,47 +13,50 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-[![PyPI](https://img.shields.io/pypi/v/pydec)](https://pypi.org/project/pydec/)
-[![Test](https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml/badge.svg?branch=master)](https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml)
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/DoubleVII/pydec/jekyll-gh-pages.yml?label=docs)](https://doublevii.github.io/pydec/)
-[![codecov](https://codecov.io/gh/DoubleVII/pydec/branch/master/graph/badge.svg?token=UGXWFEKQA9)](https://codecov.io/gh/DoubleVII/pydec)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+<p align="center">
+  <img src="docs/_images/PyDec_Logo1.png" width="200">
+</p>
+
+<p align="center">
+  <br />
+  <br />
+  <a href="https://pypi.org/project/pydec/"><img alt="PyPi" src="https://img.shields.io/pypi/v/pydec" /></a>
+  <a href="https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml"><img alt="Test" src="https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml/badge.svg?branch=master" /></a>
+  <a href="https://doublevii.github.io/pydec/"><img alt="Docs Build Status" src="https://img.shields.io/github/actions/workflow/status/DoubleVII/pydec/deploy-static-pages.yml?label=docs" /></a>
+  <a href="https://codecov.io/gh/DoubleVII/pydec"><img alt="codecov" src="https://codecov.io/gh/DoubleVII/pydec/branch/master/graph/badge.svg?token=UGXWFEKQA9" /></a>
+  <a href="https://opensource.org/licenses/MIT"><img alt="MIT License" src="https://img.shields.io/badge/License-MIT-yellow.svg" /></a>
+</p>
 
-
-<h1 align="center" style="font-size:60px">
-  PyDec
-</h1>
+--------------------------------------------------------------------------------
 
 PyDec is a linear decomposition toolkit for neural network based on [PyTorch](https://pytorch.org/), which can decompose the tensor in the forward process into given components with a small amount of code. The result of decomposition can be applied to tasks such as attribution analysis.
 
 ### Features:
 * Fast. Compute decomposition in foward process and benefit from GPU acceleration.
-* Real-time. Outputs attribution along with the model output results.
+* Run once, decompose anywhere. Obtain the decomposition of all hidden states (if you saved them) in forward propagation.
 * Applicable to networks such as Transformer, CNN and RNN.
 
 # Examples
-## Attribution
+<!-- ## Attribution
 Contribution Heat maps of the Roberta model (fine-tuned on SST-2). Warm colors indicate high
 contribution while cool colors indicate low contribution. The outputs of the model were positive, negative and positive, but the latter two samples did not match the labels.
 
 <div align="center">
 <img src="./docs/assets/img/pydec_demo1.png" width="70%">
-</div>
+</div> -->
 
 ## Data flow visualization
 
-![demo2](./docs/assets/img/pydec_demo2_1.gif)
-
-![demo2](./docs/assets/img/pydec_demo2_2.gif)
+![Data flow demo](docs/_images/pydec_demo2_1.gif)
 
 # Requirements and Installation
 * [PyTorch](https://pytorch.org/) version >= 1.11.0
 * Python version >= 3.7
 * To install PyDec and develop locally:
 
 ``` bash
@@ -67,15 +70,15 @@
 pip install pydec
 ```
 
 # Getting Started
 
 ## Example: deompose a tiny network
 
-As a simple example, here’s a very simple model with two linear layers and an activation function. We’ll create an instance of it andand get the decomposition of the output by autotracing:
+As a simple example, here's a very simple model with two linear layers and an activation function. We'll create an instance of it and get the decomposition of the output:
 ```python
 import torch
 
 class TinyModel(torch.nn.Module):
     def __init__(self):
         super(TinyModel, self).__init__()
 
@@ -107,18 +110,16 @@
 Input tensor:
 tensor([0.7023, 0.3492, 0.7771, 0.0157])
 
 
 Output tensor:
 tensor([0.2751, 0.3626], grad_fn=<AddBackward0>)
 ```
-To decompose the output, first wrap the model using `pydec.autotracing.compile` and then input the Composition initialized from `x`:
+To decompose the output, just input the Composition initialized from `x`:
 ```python
-tinymodel = pydec.autotracing.compile(tinymodel)
-
 c = pydec.zeros(x.size(), c_num=x.size(0))
 c = pydec.diagonal_init(c, src=x, dim=0)
 
 print("Input composition:")
 print(c)
 
 c_out = tinymodel(c)
@@ -158,23 +159,15 @@
 print(c_out.c_sum())
 ```
 Out:
 ```
 Sum of each component:
 tensor([0.2751, 0.3626], grad_fn=<AddBackward0>)
 ```
-To restore the ability of the model to forward tensor, use `trace()` to turn off autotracing:
-```python
-tinymodel.trace(False)
-
-print("Output tensor:")
-print(tinymodel(x))
-```
-Out:
-```
-Output tensor:
-tensor([0.2751, 0.3626], grad_fn=<AddBackward0>)
-```
 
 # Documentation
 
-The [full documentation](https://doublevii.github.io/pydec/) contains examples of implementations on realistic models, tutorials, notes and Python API.
+The [full documentation](https://doublevii.github.io/pydec/) contains examples of implementations on real-world models, tutorials, notes and Python API descriptions.
+
+
+# Linear Decomposition Theory
+To understand the principles and theories behind PyDec, see our paper [Local Interpretation of Transformer Based on Linear Decomposition](https://aclanthology.org/2023.acl-long.572/).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydec-0.2.0/README.md` & `pydec-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-[![PyPI](https://img.shields.io/pypi/v/pydec)](https://pypi.org/project/pydec/)
-[![Test](https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml/badge.svg?branch=master)](https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml)
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/DoubleVII/pydec/jekyll-gh-pages.yml?label=docs)](https://doublevii.github.io/pydec/)
-[![codecov](https://codecov.io/gh/DoubleVII/pydec/branch/master/graph/badge.svg?token=UGXWFEKQA9)](https://codecov.io/gh/DoubleVII/pydec)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+<p align="center">
+  <img src="docs/_images/PyDec_Logo1.png" width="200">
+</p>
+
+<p align="center">
+  <br />
+  <br />
+  <a href="https://pypi.org/project/pydec/"><img alt="PyPi" src="https://img.shields.io/pypi/v/pydec" /></a>
+  <a href="https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml"><img alt="Test" src="https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml/badge.svg?branch=master" /></a>
+  <a href="https://doublevii.github.io/pydec/"><img alt="Docs Build Status" src="https://img.shields.io/github/actions/workflow/status/DoubleVII/pydec/deploy-static-pages.yml?label=docs" /></a>
+  <a href="https://codecov.io/gh/DoubleVII/pydec"><img alt="codecov" src="https://codecov.io/gh/DoubleVII/pydec/branch/master/graph/badge.svg?token=UGXWFEKQA9" /></a>
+  <a href="https://opensource.org/licenses/MIT"><img alt="MIT License" src="https://img.shields.io/badge/License-MIT-yellow.svg" /></a>
+</p>
 
-
-<h1 align="center" style="font-size:60px">
-  PyDec
-</h1>
+--------------------------------------------------------------------------------
 
 PyDec is a linear decomposition toolkit for neural network based on [PyTorch](https://pytorch.org/), which can decompose the tensor in the forward process into given components with a small amount of code. The result of decomposition can be applied to tasks such as attribution analysis.
 
 ### Features:
 * Fast. Compute decomposition in foward process and benefit from GPU acceleration.
-* Real-time. Outputs attribution along with the model output results.
+* Run once, decompose anywhere. Obtain the decomposition of all hidden states (if you saved them) in forward propagation.
 * Applicable to networks such as Transformer, CNN and RNN.
 
 # Examples
-## Attribution
+<!-- ## Attribution
 Contribution Heat maps of the Roberta model (fine-tuned on SST-2). Warm colors indicate high
 contribution while cool colors indicate low contribution. The outputs of the model were positive, negative and positive, but the latter two samples did not match the labels.
 
 <div align="center">
 <img src="./docs/assets/img/pydec_demo1.png" width="70%">
-</div>
+</div> -->
 
 ## Data flow visualization
 
-![demo2](./docs/assets/img/pydec_demo2_1.gif)
-
-![demo2](./docs/assets/img/pydec_demo2_2.gif)
+![Data flow demo](docs/_images/pydec_demo2_1.gif)
 
 # Requirements and Installation
 * [PyTorch](https://pytorch.org/) version >= 1.11.0
 * Python version >= 3.7
 * To install PyDec and develop locally:
 
 ``` bash
@@ -48,15 +51,15 @@
 pip install pydec
 ```
 
 # Getting Started
 
 ## Example: deompose a tiny network
 
-As a simple example, here’s a very simple model with two linear layers and an activation function. We’ll create an instance of it andand get the decomposition of the output by autotracing:
+As a simple example, here's a very simple model with two linear layers and an activation function. We'll create an instance of it and get the decomposition of the output:
 ```python
 import torch
 
 class TinyModel(torch.nn.Module):
     def __init__(self):
         super(TinyModel, self).__init__()
 
@@ -88,18 +91,16 @@
 Input tensor:
 tensor([0.7023, 0.3492, 0.7771, 0.0157])
 
 
 Output tensor:
 tensor([0.2751, 0.3626], grad_fn=<AddBackward0>)
 ```
-To decompose the output, first wrap the model using `pydec.autotracing.compile` and then input the Composition initialized from `x`:
+To decompose the output, just input the Composition initialized from `x`:
 ```python
-tinymodel = pydec.autotracing.compile(tinymodel)
-
 c = pydec.zeros(x.size(), c_num=x.size(0))
 c = pydec.diagonal_init(c, src=x, dim=0)
 
 print("Input composition:")
 print(c)
 
 c_out = tinymodel(c)
@@ -139,23 +140,15 @@
 print(c_out.c_sum())
 ```
 Out:
 ```
 Sum of each component:
 tensor([0.2751, 0.3626], grad_fn=<AddBackward0>)
 ```
-To restore the ability of the model to forward tensor, use `trace()` to turn off autotracing:
-```python
-tinymodel.trace(False)
-
-print("Output tensor:")
-print(tinymodel(x))
-```
-Out:
-```
-Output tensor:
-tensor([0.2751, 0.3626], grad_fn=<AddBackward0>)
-```
 
 # Documentation
 
-The [full documentation](https://doublevii.github.io/pydec/) contains examples of implementations on realistic models, tutorials, notes and Python API.
+The [full documentation](https://doublevii.github.io/pydec/) contains examples of implementations on real-world models, tutorials, notes and Python API descriptions.
+
+
+# Linear Decomposition Theory
+To understand the principles and theories behind PyDec, see our paper [Local Interpretation of Transformer Based on Linear Decomposition](https://aclanthology.org/2023.acl-long.572/).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydec-0.2.0/pydec/_composition_str.py` & `pydec-0.3.0/pydec/_composition_str.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from torch._tensor_str import _tensor_str, _add_suffixes, PRINT_OPTS
-from typing import List, Tuple
+from typing import List, Tuple, Optional, Union
 
 
 def _c_add_suffixes(composition_str, suffixes, indent, force_newline):
     tensor_strs = [composition_str]
     last_line_len = len(composition_str) - composition_str.rfind("\n") + 1
     for suffix in suffixes:
         suffix_len = len(suffix)
@@ -249,51 +249,56 @@
         # pydec: move the prefix indent to the beginning
         string_repr = " " * prefix_indent + f"Parameter({string_repr[prefix_indent:]})"
 
     return string_repr, suffixes
 
 
 def _t_str(
-    self: torch.Tensor, *, tensor_contents: str = None, prefix_indent=0
+    self: torch.Tensor,
+    *,
+    tensor_contents: Optional[str] = None,
+    prefix_indent: Optional[int] = 0,
 ) -> Tuple:
     with torch.no_grad():
         return _tensor_str_intern(
             self, tensor_contents=tensor_contents, prefix_indent=prefix_indent
         )
 
 
-def _c_str(self, *, composition_contents: List[str] = None):
+def _c_str(self, *, composition_contents: Optional[List[Union[str, None]]] = None):
     """
     Args:
         self: the composition to be represented
         composition_contents: should be a list of string and the length of the list should be
         equal to the number of components (include the residual). For components that do not
         use customized content, use `None` placeholder in the list.
     """
+    if self.components is None:
+        return r"composition{}"
     if composition_contents is not None:
         contents_num = len(composition_contents)
         components_num = self.numc() + 1
         if contents_num != components_num:
             if contents_num < components_num:
                 composition_contents.extend([None] * (self.numc() + 1 - contents_num))
             else:
                 # ignore the redundant
                 composition_contents = composition_contents[:components_num]
     prefix = "composition{"
     indent = 2  # fix to 2 looks nice
 
     components_reprs = [
         _t_str(
-            self[i],
+            self()[i],
             tensor_contents=composition_contents[i]
             if composition_contents is not None
             else None,
             prefix_indent=indent + 2,  # second indent
         )[0]
-        for i in range(len(self))
+        for i in range(self.numc())
     ]
     residual_repr, suffixes = _t_str(
         self._residual_tensor,
         tensor_contents=composition_contents[-1]
         if composition_contents is not None
         else None,
         prefix_indent=indent + 2,  # second indent
```

### Comparing `pydec-0.2.0/pydec/composition.py` & `pydec-0.3.0/pydec/_composition.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,76 @@
 from __future__ import annotations
 
 import torch
+from . import core
+
 from typing import Any, Dict, Union, List, Tuple, Sequence, Optional, Callable, overload
 from torch import Tensor
 from torch._C import memory_format
+from torch.autograd.grad_mode import _DecoratorContextManager
 import pydec
 from ._composition_str import _c_str
 import types
-import warnings
+import sys
+from .overrides import (
+    _register_builtin_function,
+    _auto_registration,
+    is_registered,
+    dispatch_torch_function,
+)
 
 # In some cases, these basic types are shadowed by corresponding
 # top-level values.  The underscore variants let us refer to these
 # types.  See https://github.com/python/mypy/issues/4146 for why these
 # workarounds is necessary
+# In the future, this will become useful if mypy is introduced into pydec
 from torch.types import (
     _int,
     _float,
     _bool,
     Number,
     _dtype,
     _device,
     _qscheme,
     _size,
     _layout,
-    SymInt,
 )
 
 from pydec.exception_utils import (
     args_error,
     size_error,
     component_num_error,
     unsupported_operand_error,
     arg_value_error,
+    none_decomposition_func_error,
 )
 
 
-from pydec.utils import _shift_dim, _shift_dims
-
+from pydec.utils import _shift_dim, _shift_dims, parse_args
 
 r"""
 To avoid circular import, we have to initialize the following method in __init__.py.
 """
 
 
-def _from_replce(
-    composition_tensor: Tensor, residual_tensor: Tensor = None
-) -> Composition:
-    ...
-
-
-_registered_method_dict = {}
-
-
-def _c_register_method(name: str, func: Callable):
-    # this function is not public, invoked by pydec.autotracing.library (stacklevel=3)
-    if name in _registered_method_dict:
-        warnings.warn("override registered method ({})".format(name), stacklevel=3)
-    _registered_method_dict[name] = func
-
-
-class _CompositionMeta(type):
+class Composition:
     r"""
-    This metaclass is used to support customized method registration for Composition.
-    """
-
-    def __new__(cls, clsname, bases, attrs):
-        assert len(bases) == 0
-        c_init = attrs["__init__"] if "__init__" in attrs else None
-
-        def meta_init(self, *args, **kwargs):
-            if c_init is not None:
-                c_init(self, *args, **kwargs)
-
-            # do registeration
-            for name, func in _registered_method_dict.items():
-                setattr(self, name, types.MethodType(func, self))
-
-        attrs["__init__"] = meta_init
-
-        return super().__new__(cls, clsname, bases, attrs)
-
-
-class Composition(metaclass=_CompositionMeta):
-    __doc__ = r"""
     TODO: Composition doc
     """
 
+    @classmethod
+    def __torch_function__(cls, func, types, args=(), kwargs=None):
+        if kwargs is None:
+            kwargs = {}
+        if not is_registered(func) or not all(
+            issubclass(t, (torch.Tensor, pydec.Composition)) for t in types
+        ):
+            return NotImplemented
+        return dispatch_torch_function(func)(*args, **kwargs)
+
     @property
     def requires_grad(self) -> _bool:
         return self._residual_tensor.requires_grad
 
     @property
     def shape(self) -> torch.Size:
         return self._residual_tensor.shape
@@ -99,213 +80,266 @@
         return self._residual_tensor.device
 
     @property
     def dtype(self) -> _dtype:
         return self._residual_tensor.dtype
 
     @property
+    def layout(self) -> _dtype:
+        return self._residual_tensor.layout
+
+    @property
     def T(self) -> Composition:
         return self.permute(*torch.arange(self.ndim - 1, -1, -1))
 
     @property
     def mT(self) -> Composition:
         return self.transpose(-2, -1)
 
     @property
     def ndim(self) -> _int:
         return self.dim()
 
+    @property
+    def components(self) -> Tensor:
+        return self._component_tensor
+
+    @property
+    def residual(self) -> Tensor:
+        return self._residual_tensor
+
+    @property
+    def recovery(self) -> Tensor:
+        return self.c_sum()
+
+    @property
+    def is_cuda(self):
+        return self._residual_tensor.is_cuda
+
     @overload
     def __init__(
-        self, composition_tensor: Tensor, residual_tensor: Tensor = None
+        self, component_tensor: Tensor, residual_tensor: Optional[Tensor] = None
     ) -> None:
         ...
 
     @overload
     def __init__(self, composition: Composition) -> None:
         ...
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         def init_from_tensor(
-            composition_tensor: Tensor, residual_tensor: Tensor = None
+            component_tensor: Tensor, residual_tensor: Optional[Tensor] = None
         ):
             if residual_tensor is not None:
-                if composition_tensor.dtype != residual_tensor.dtype:
+                if component_tensor.dtype != residual_tensor.dtype:
                     raise arg_value_error(
-                        f"the dtype of composition_tensor ({composition_tensor.dtype}) should be the same as that of residual_tensor ({residual_tensor.dtype})."
+                        f"the dtype of component_tensor ({component_tensor.dtype}) should be the same as that of residual_tensor ({residual_tensor.dtype})"
                     )
-                if composition_tensor.device != residual_tensor.device:
+                if component_tensor.device != residual_tensor.device:
                     raise arg_value_error(
-                        f"the device of composition_tensor ({composition_tensor.device}) should be the same as that of residual_tensor ({residual_tensor.device})."
+                        f"the device of component_tensor ({component_tensor.device}) should be the same as that of residual_tensor ({residual_tensor.device})"
                     )
-                if composition_tensor.requires_grad != residual_tensor.requires_grad:
+                if component_tensor.requires_grad != residual_tensor.requires_grad:
                     raise arg_value_error(
-                        f"composition_tensor.requires_grad ({composition_tensor.requires_grad}) should be the same as residual_tensor.requires_grad ({residual_tensor.requires_grad})."
+                        f"component_tensor.requires_grad ({component_tensor.requires_grad}) should be the same as residual_tensor.requires_grad ({residual_tensor.requires_grad})"
                     )
 
             # formal way but may cause problems, see https://github.com/pytorch/pytorch/issues/85094
-            self._composition_tensor = composition_tensor.clone().detach()
+            self._component_tensor = component_tensor.clone().detach()
             if residual_tensor is not None:
-                if composition_tensor.size()[1:] != residual_tensor.size():
+                if component_tensor.size()[1:] != residual_tensor.size():
                     raise size_error(
-                        composition_tensor.size()[1:],
+                        component_tensor.size()[1:],
                         residual_tensor.size(),
                         "composition",
                         "residual",
                     )
                 self._residual_tensor = residual_tensor.clone().detach()
             else:
-                self._residual_tensor = torch.zeros(composition_tensor.size()[1:]).to(
-                    composition_tensor
+                self._residual_tensor = torch.zeros(component_tensor.size()[1:]).to(
+                    component_tensor
                 )
 
-        def parse_args(args: list, key_list: List):
-            for i in range(len(args)):
-                kwargs[key_list[i]] = args[i]
+        self._component_tensor: Tensor = None  # type: ignore[no-redef, assignment]
+        self._residual_tensor: Tensor = None  # type: ignore[no-redef, assignment]
+        input_kwargs = kwargs.copy()  # for error hint
 
-        self._composition_tensor: Tensor = None
-        self._residual_tensor: Tensor = None
-
-        if len(args) == 1:
+        if len(args) == 0 and len(kwargs) == 0:
+            # a private constructor to create a void composition with no data,
+            # which is usually assigned in `_from_replace`.
+            return
+        elif len(args) > 0:
             if isinstance(args[0], Composition):
-                parse_args(args, ["composition"])
-            elif isinstance(args[0], Tensor):
-                parse_args(args, ["composition_tensor"])
+                parse_args(args, ["composition"], kwargs)
             else:
-                raise args_error("Composition.__init__", args, kwargs)
-        elif len(args) == 2:
-            if isinstance(args[0], Tensor) and isinstance(args[1], Tensor):
-                parse_args(args, ["composition_tensor", "residual_tensor"])
-            else:
-                raise args_error("Composition.__init__", args, kwargs)
+                parse_args(args, ["component_tensor", "residual_tensor"], kwargs)
         elif len(args) > 2:
-            raise args_error("Composition.__init__", args, kwargs)
+            raise args_error("Composition.__init__", args, input_kwargs)
 
         if "composition" in kwargs:
-            c: Composition = kwargs["composition"]
-            init_from_tensor(c._composition_tensor, c._residual_tensor)
-        elif "composition_tensor" in kwargs:
-            init_from_tensor(**kwargs)
+            c = kwargs["composition"]
+            if isinstance(c, Composition):
+                init_from_tensor(c._component_tensor, c._residual_tensor)
+            else:
+                raise args_error("Composition.__init__", args, input_kwargs)
+        elif "component_tensor" in kwargs:
+            if "residual_tensor" in kwargs and not isinstance(
+                kwargs["residual_tensor"], Tensor
+            ):
+                raise args_error("Composition.__init__", args, input_kwargs)
+            if isinstance(kwargs["component_tensor"], Tensor):
+                init_from_tensor(**kwargs)
+            else:
+                raise args_error("Composition.__init__", args, input_kwargs)
         else:
-            raise args_error("Composition.__init__", args, kwargs)
+            raise args_error("Composition.__init__", args, input_kwargs)
 
+    @_auto_registration
     def __getitem__(
         self, indices: Union[None, _int, slice, Tensor, List, Tuple]
-    ) -> Union[Composition, Tensor]:
-        # support autotracing
-        if pydec.autotracing.is_tracing_enabled():
-            if isinstance(indices, Tuple):
+    ) -> Composition:
+        if not pydec.is_c_accessing_enabled():
+            if isinstance(indices, tuple):
+                indices = (slice(None, None, None),) + indices
+            else:
+                indices = (
+                    slice(None, None, None),
+                    indices,
+                )
+        return self.__c_getitem__(indices)  # type: ignore[return-value]
+
+    @_auto_registration
+    def __setitem__(
+        self,
+        indices: Union[None, _int, slice, Tensor, List, Tuple],
+        val: Union[Composition, Tensor, Number],
+    ) -> None:
+        if not pydec.is_c_accessing_enabled():
+            if isinstance(indices, tuple):
                 indices = (slice(None, None, None),) + indices
             else:
                 indices = (
                     slice(None, None, None),
                     indices,
                 )
+        return self.__c_setitem__(indices, val)
 
+    def __c_getitem__(
+        self, indices: Union[None, _int, slice, Tensor, List, Tuple]
+    ) -> Union[Composition, Tensor]:
         if isinstance(indices, (type(None), _int, slice, List, Tensor)):
             indices = (indices,)
+        assert isinstance(indices, tuple)  # make mypy ignore [index] errors
         if indices[0] is None:
             raise arg_value_error(
-                "The first dimension of indices should not be NoneType."
+                "The first dimension of indices should not be NoneType"
             )
         if isinstance(indices[0], _int):
-            return self._composition_tensor[indices]
+            return self._component_tensor[indices]
         else:
-            out_composition_tensor = self._composition_tensor[indices]
+            out_component_tensor = self._component_tensor[indices]
             out_residual_tensor = self._residual_tensor[indices[1:]]
-            return _from_replce(out_composition_tensor, out_residual_tensor)
+            return pydec.as_composition(out_component_tensor, out_residual_tensor)
 
-    def __setitem__(
+    def __c_setitem__(
         self,
         indices: Union[None, _int, slice, Tensor, List, Tuple],
         val: Union[Composition, Tensor, Number],
     ) -> None:
-        # support autotracing
-        if pydec.autotracing.is_tracing_enabled():
-            if isinstance(indices, Tuple):
-                indices = (slice(None, None, None),) + indices
-            else:
-                indices = (
-                    slice(None, None, None),
-                    indices,
-                )
-
         if isinstance(indices, (type(None), _int, slice, List, Tensor)):
             indices = (indices,)
+        assert isinstance(indices, tuple)  # make mypy ignore [index] errors
         if indices[0] is None:
             raise arg_value_error(
-                "The first dimension of indices should not be NoneType."
+                "The first dimension of indices should not be NoneType"
             )
 
         if isinstance(val, (Tensor, _int, _float, _bool)):
-            self._composition_tensor[indices] = val
+            # TODO: also set item for residual? `c[:]=0` not work with c.residual
+            self._component_tensor[indices] = val
             return
         if isinstance(val, (Composition)):
             if isinstance(indices[0], _int):
                 raise arg_value_error(
-                    f"A single component assignment is being made, and the right part of the equal sign should be (Tensor) or (Number), not ({type(val).__name__})."
+                    f"Expected the assignment value to be (Tensor) or (Number), not ({type(val).__name__}) for single component assignment"
                 )
             else:
-                self._composition_tensor[indices] = val._composition_tensor
+                self._component_tensor[indices] = val._component_tensor
                 self._residual_tensor[indices[1:]] = val._residual_tensor
 
+    def __call__(self) -> _C_AccessingComposition:
+        """
+        Shortcut for `__c_getitem__` and `__c_setitem__`, e.g., `c()[2]` equals to `c.__c_getitem__(2)`.
+        """
+        return _C_AccessingComposition(self)
+
+    @_auto_registration
     def __len__(self):
-        return self._composition_tensor.__len__()
+        if pydec.is_c_accessing_enabled():
+            return self.components.__len__()
+        else:
+            return self.residual.__len__()
 
     def __iter__(self):
-        return self._composition_tensor.__iter__()
+        if pydec.is_c_accessing_enabled():
+            # TODO: should return composition
+            return self._component_tensor.__iter__()
+        else:
+            # TODO: return a iterator
+            raise NotImplementedError
 
+    @_auto_registration
     def __reversed__(self):
-        return self._composition_tensor.__reversed__()
+        return self._component_tensor.__reversed__()
 
+    @_auto_registration
     def __contains__(self, element):
-        return self._composition_tensor.__contains__(element)
+        return self._component_tensor.__contains__(element)
 
-    def __repr__(self, *, composition_contents: List[str] = None) -> str:
+    @_auto_registration  # type: ignore[arg-type]
+    def __repr__(
+        self, *, composition_contents: Optional[List[Union[str, None]]] = None
+    ) -> str:
         return _c_str(self, composition_contents=composition_contents)
 
+    @_auto_registration
     def numel(self) -> _int:
-        return self._residual_tensor.numel()
+        return pydec.numel(self)
 
     def c_numel(self, count_residual=False) -> _int:
-        if count_residual:
-            return self._composition_tensor.numel() + self._residual_tensor.numel()
-        else:
-            return self._composition_tensor.numel()
+        return pydec.c_numel(self, count_residual=count_residual)
 
     def numc(self) -> _int:
-        return len(self)
+        return pydec.numc(self)
 
+    @_auto_registration
     def clone(self, *, memory_format: Optional[memory_format] = None) -> Composition:
-        out = Composition(tuple(), 0)
-        out._composition_tensor = self._composition_tensor.clone(
-            memory_format=memory_format
-        )
-        out._residual_tensor = self._residual_tensor.clone(memory_format=memory_format)
-        return out
+        return pydec.clone(self, memory_format=memory_format)
 
+    @_auto_registration
     def detach(self) -> Composition:
-        out = Composition(tuple(), 0)
-        out._composition_tensor = self._composition_tensor.detach()
-        out._residual_tensor = self._residual_tensor.detach()
-        return out
+        return pydec.detach(self)
 
+    @_auto_registration
     def detach_(self) -> Composition:
-        self._composition_tensor.detach_()
-        self._residual_tensor.detach_()
-        return self
+        return pydec.detach_(self)
 
     @overload
     def size(self) -> torch.Size:
         ...
 
     @overload
     def size(self, dim: _int) -> _int:
         ...
 
+    @overload
+    def size(self, dim: Optional[_int] = None) -> Union[torch.Size, _int]:
+        ...
+
+    @_auto_registration
     def size(self, dim: Optional[_int] = None) -> Union[torch.Size, _int]:
         if dim is None:
             return self.c_size()[1:]
         else:
             return self.size()[dim]
 
     @overload
@@ -314,495 +348,471 @@
 
     @overload
     def c_size(self, dim: _int) -> _int:
         ...
 
     def c_size(self, dim: Optional[_int] = None) -> Union[torch.Size, _int]:
         if dim is None:
-            return self._composition_tensor.size()
+            return self._component_tensor.size()
         else:
-            return self._composition_tensor.size(dim)
+            return self._component_tensor.size(dim)
 
+    @_auto_registration
     def dim(self) -> _int:
         return self._residual_tensor.dim()
 
+    @_auto_registration
     def __neg__(self) -> Composition:
-        return _from_replce(-self._composition_tensor, -self._residual_tensor)
+        return pydec.as_composition(-self._component_tensor, -self._residual_tensor)
 
+    @_auto_registration
     def __pos__(self) -> Composition:
-        return _from_replce(+self._composition_tensor, +self._residual_tensor)
+        return pydec.as_composition(+self._component_tensor, +self._residual_tensor)
 
+    @_auto_registration
     def __iadd__(self, other) -> Composition:
+        if not isinstance(self, Composition):
+            # TODO: maybe return a composition is a good choice
+            raise unsupported_operand_error("+=", type(self), type(other))
         if isinstance(other, Composition):
-            if self.numc() != other.numc():
-                raise component_num_error(self.numc(), other.numc())
-            self._composition_tensor += other._composition_tensor
-            self._residual_tensor += other._residual_tensor
-            return self
+            return core.decBLAS.cc_add_(self, other)
         elif isinstance(other, (_int, _float, _bool, Tensor)):
-            self._residual_tensor += other
-            return self
+            return core.decBLAS.ct_add_(self, other)
         else:
             raise unsupported_operand_error("+=", type(self), type(other))
 
+    @_auto_registration
     def __add__(self, other) -> Composition:
-        if isinstance(other, Composition):
-            if self.numc() != other.numc():
-                raise component_num_error(self.numc(), other.numc())
-            out_composition_tensor = (
-                self._composition_tensor + other._composition_tensor
-            )
-            out_residual_tensor = self._residual_tensor + other._residual_tensor
-            return _from_replce(out_composition_tensor, out_residual_tensor)
-        elif isinstance(other, (_int, _float, _bool, Tensor)):
-            out_composition_tensor = self._composition_tensor.clone()
-            out_residual_tensor = self._residual_tensor + other
-            return _from_replce(out_composition_tensor, out_residual_tensor)
-        else:
+        try:
+            return pydec.add(self, other)
+        except TypeError:
             raise unsupported_operand_error("+", type(self), type(other))
 
+    @_auto_registration
     def __radd__(self, other) -> Composition:
         try:
-            return self + other
+            return pydec.add(other, self)
         except TypeError:
             raise unsupported_operand_error("+", type(other), type(self))
 
+    @_auto_registration
     def __sub__(self, other) -> Composition:
         try:
-            return self + (-other)
+            return pydec.sub(self, other)
         except TypeError:
             raise unsupported_operand_error("-", type(self), type(other))
 
+    @_auto_registration
     def __rsub__(self, other) -> Composition:
         try:
-            return other + (-self)
+            return pydec.sub(other, self)
         except TypeError:
             raise unsupported_operand_error("-", type(other), type(self))
 
+    @_auto_registration
     def __isub__(self, other) -> Composition:
-        try:
-            self += -other
-        except TypeError:
+        if not isinstance(self, Composition):
             raise unsupported_operand_error("-=", type(self), type(other))
-        return self
-
-    def __imatmul__(self, other) -> Composition:
-        if isinstance(other, Tensor):
-            self._composition_tensor @= other
-            self._residual_tensor @= other
-            return self
+        if isinstance(other, Composition):
+            return core.decBLAS.cc_sub_(self, other)
+        elif isinstance(other, (_int, _float, _bool, Tensor)):
+            return core.decBLAS.ct_sub_(self, other)
         else:
-            raise unsupported_operand_error("@=", type(self), type(other))
+            raise unsupported_operand_error("-=", type(self), type(other))
 
+    @_auto_registration
     def __matmul__(self, other) -> Composition:
         if isinstance(other, Tensor):
-            out_composition_tensor = self._composition_tensor @ other
-            out_residual_tensor = self._residual_tensor @ other
-            return _from_replce(out_composition_tensor, out_residual_tensor)
+            return core.decBLAS.ct_matmul(self, other)
         else:
             raise unsupported_operand_error("@", type(self), type(other))
 
+    @_auto_registration
     def __rmatmul__(self, other) -> Composition:
         if isinstance(other, Tensor):
-            if self.dim() == 1:
-                # if the composition_tensor's ndim is 2, the component dim
-                # will be incorrectly included in the multiplication
-                out_composition_tensor = other @ self._composition_tensor.unsqueeze(-1)
-                out_composition_tensor.squeeze_(-1)
-                out_residual_tensor = other @ self._residual_tensor
-            else:
-                out_composition_tensor = other @ self._composition_tensor
-                out_residual_tensor = other @ self._residual_tensor
-            return _from_replce(out_composition_tensor, out_residual_tensor)
+            return core.decBLAS.tc_matmul(other, self)
         else:
-            raise unsupported_operand_error("@=", type(self), type(other))
+            raise unsupported_operand_error("@=", type(other), type(other))
 
+    @_auto_registration
     def __imul__(self, other) -> Composition:
-        if isinstance(other, Composition):
+        if not isinstance(self, Composition):
+            # TODO: maybe return a composition is a good choice
             raise unsupported_operand_error("*=", type(self), type(other))
-        if isinstance(other, Tensor):
-            if other.dim() > self.dim():
-                new_size = (
-                    (self.numc(),) + (1,) * (other.dim() - self.dim()) + self.size()
-                )
-                self._composition_tensor = self._composition_tensor.view(new_size)
-            self._composition_tensor *= other
-            self._residual_tensor *= other
+        if isinstance(other, Composition):
+            return core.decMVF.cc_mul_(self, other)
+        elif isinstance(other, (_int, _float, _bool, Tensor)):
+            return core.decBLAS.ct_mul_(self, other)
         else:
-            self._composition_tensor *= other
-            self._residual_tensor *= other
-        return self
+            raise unsupported_operand_error("*=", type(self), type(other))
 
+    @_auto_registration
     def __mul__(self, other) -> Composition:
-        if isinstance(other, Composition):
+        try:
+            return pydec.mul(self, other)
+        except TypeError:
             raise unsupported_operand_error("*", type(self), type(other))
-        if isinstance(other, Tensor):
-            if other.dim() > self.dim():
-                new_size = (
-                    (self.numc(),) + (1,) * (other.dim() - self.dim()) + self.size()
-                )
-                out_composition_tensor = self._composition_tensor.view(new_size) * other
-            else:
-                out_composition_tensor = self._composition_tensor * other
-            out_residual_tensor = self._residual_tensor * other
-        else:
-            out_composition_tensor = self._composition_tensor * other
-            out_residual_tensor = self._residual_tensor * other
-        return _from_replce(out_composition_tensor, out_residual_tensor)
 
+    @_auto_registration
     def __rmul__(self, other) -> Composition:
         try:
-            return self * other
+            return pydec.mul(other, self)
         except TypeError:
             raise unsupported_operand_error("*", type(other), type(self))
 
+    @_auto_registration
     def __itruediv__(self, other: Any) -> Composition:
+        if not isinstance(self, Composition):
+            raise unsupported_operand_error("/=", type(self), type(other))
         if isinstance(other, Composition):
+            # TODO: not implement yet
             raise unsupported_operand_error("/=", type(self), type(other))
-        if isinstance(other, Tensor):
-            if other.dim() > self.dim():
-                new_size = (
-                    (self.numc(),) + (1,) * (other.dim() - self.dim()) + self.size()
-                )
-                self._composition_tensor = self._composition_tensor.view(new_size)
-            self._composition_tensor /= other
-            self._residual_tensor /= other
+        elif isinstance(other, (_int, _float, _bool, Tensor)):
+            return core.decBLAS.ct_div_(self, other)
         else:
-            self._composition_tensor /= other
-            self._residual_tensor /= other
-        return self
+            raise unsupported_operand_error("/=", type(self), type(other))
 
+    @_auto_registration
     def __truediv__(self, other: Any) -> Composition:
-        if isinstance(other, Composition):
+        try:
+            return pydec.div(self, other)
+        except TypeError:
             raise unsupported_operand_error("/", type(self), type(other))
-        if isinstance(other, Tensor):
-            if other.dim() > self.dim():
-                new_size = (
-                    (self.numc(),) + (1,) * (other.dim() - self.dim()) + self.size()
-                )
-                out_composition_tensor = self._composition_tensor.view(new_size) / other
-            else:
-                out_composition_tensor = self._composition_tensor / other
-            out_residual_tensor = self._residual_tensor / other
-        else:
-            out_composition_tensor = self._composition_tensor / other
-            out_residual_tensor = self._residual_tensor / other
-        return _from_replce(out_composition_tensor, out_residual_tensor)
 
+    @_auto_registration
     def __rtruediv__(self, other: Any) -> Composition:
         try:
-            return self * other
+            return pydec.div(other, self)
         except TypeError:
             raise unsupported_operand_error("/", type(other), type(self))
 
-    def __eq__(self, other: Any) -> Tensor:
+    @_auto_registration
+    def __eq__(self, other: Any) -> Tensor:  # type: ignore[override]
         if isinstance(other, Composition):
-            return other.__eq__(self.c_sum())
+            return self.c_sum().__eq__(other.c_sum())
         return self.c_sum().__eq__(other)
 
-    def __ne__(self, other: Any) -> Tensor:
+    @_auto_registration
+    def __ne__(self, other: Any) -> Tensor:  # type: ignore[override]
         if isinstance(other, Composition):
-            return other.__ne__(self.c_sum())
+            return self.c_sum().__ne__(other.c_sum())
         return self.c_sum().__ne__(other)
 
+    @_auto_registration
     def __gt__(self, other: Any) -> Tensor:
         if isinstance(other, Composition):
-            return other.__lt__(self.c_sum())
+            return self.c_sum().__gt__(other.c_sum())
         return self.c_sum().__gt__(other)
 
+    @_auto_registration
     def __lt__(self, other: Any) -> Tensor:
         if isinstance(other, Composition):
-            return other.__gt__(self.c_sum())
+            return self.c_sum().__lt__(other.c_sum())
         return self.c_sum().__lt__(other)
 
+    @_auto_registration
     def __ge__(self, other: Any) -> Tensor:
         if isinstance(other, Composition):
-            return other.__le__(self.c_sum())
+            return self.c_sum().__ge__(other.c_sum())
         return self.c_sum().__ge__(other)
 
+    @_auto_registration
     def __le__(self, other: Any) -> Tensor:
         if isinstance(other, Composition):
-            return other.__ge__(self.c_sum())
+            return self.c_sum().__le__(other.c_sum())
         return self.c_sum().__le__(other)
 
+    @_auto_registration
     def add(
         self,
         other: Union[Composition, Tensor, Number],
         *,
         alpha: Optional[Number] = 1,
-        out: Optional[Composition] = None,
-        **kwargs,
     ) -> Composition:
-        if isinstance(other, Composition):
-            if self.numc() != other.numc():
-                raise component_num_error(self.numc(), other.numc())
-            if out is None:
-                out_composition_tensor = self._composition_tensor.add(
-                    other._composition_tensor, alpha=alpha
-                )
-                out_residual_tensor = self._residual_tensor.add(
-                    other._residual_tensor, alpha=alpha
-                )
-            else:
-                out_composition_tensor = self._composition_tensor.add(
-                    other._composition_tensor, alpha=alpha, out=out._composition_tensor
-                )
-                out_residual_tensor = self._residual_tensor.add(
-                    other._residual_tensor, alpha=alpha, out=out._residual_tensor
-                )
-            return _from_replce(out_composition_tensor, out_residual_tensor)
-        elif isinstance(other, (_int, _float, _bool, Tensor)):
-            out_composition_tensor = self._composition_tensor.clone()
-            out_residual_tensor = self._residual_tensor.add(
-                other, alpha=alpha, out=out._residual_tensor
-            )
-            if out is not None:
-                out._composition_tensor[:] = out_composition_tensor
-            return _from_replce(out_composition_tensor, out_residual_tensor)
-        else:
-            raise unsupported_operand_error("add", type(self), type(other))
+        """
+        Note: although the function signature of `torch.Tensor.add` has parameter `out`, it is not working
+        """
+        return pydec.add(self, other, alpha=alpha)
 
+    @_auto_registration
     def add_(
         self,
         other: Union[Composition, Tensor, Number],
         *,
         alpha: Optional[Number] = 1,
-        **kwargs,
     ) -> Composition:
+        if not isinstance(self, Composition):
+            # TODO: maybe return a composition is a good choice
+            raise unsupported_operand_error("add_", type(self), type(other))
         if isinstance(other, Composition):
-            if self.numc() != other.numc():
-                raise component_num_error(self.numc(), other.numc())
-            self._composition_tensor.add_(other.composition_tensor, alpha=alpha)
-            self._residual_tensor.add_(other._residual_tensor, alpha=alpha)
-            return self
+            return core.decBLAS.cc_add_(self, other, alpha=alpha)
         elif isinstance(other, (_int, _float, _bool, Tensor)):
-            self._residual_tensor.add_(other, alpha=alpha)
-            return self
+            return core.decBLAS.ct_add_(self, other, alpha=alpha)
         else:
             raise unsupported_operand_error("add_", type(self), type(other))
 
+    @_auto_registration
     def sub(
         self,
         other: Union[Composition, Tensor, Number],
         *,
         alpha: Optional[Number] = 1,
-        out: Optional[Composition] = None,
-        **kwargs,
     ) -> Composition:
-        return self.add(-other, alpha=alpha, out=out, **kwargs)
+        return pydec.sub(self, other, alpha=alpha)
 
+    @_auto_registration
     def sub_(
         self, other: Union[Composition, Tensor, Number], *, alpha: Optional[Number] = 1
     ) -> Composition:
-        return self.add_(-other, alpha=alpha)
-
-    def mul(
-        self, other: Union[Tensor, Number], *, out: Optional[Composition] = None
-    ) -> Composition:
+        if not isinstance(self, Composition):
+            # TODO: maybe return a composition is a good choice
+            raise unsupported_operand_error("sub_", type(self), type(other))
         if isinstance(other, Composition):
-            raise args_error(Composition.mul.__name__, self, other, out=out)
-        if isinstance(other, Tensor):
-            if other.dim() > self.dim():
-                new_size = (
-                    (self.numc(),) + (1,) * (other.dim() - self.dim()) + self.size()
-                )
-                out_composition_tensor = self._composition_tensor.view(new_size).mul(
-                    other, out=out._composition_tensor
-                )
-            else:
-                out_composition_tensor = self._composition_tensor.mul(
-                    other, out=out._composition_tensor
-                )
-            out_residual_tensor = self._residual_tensor.mul(
-                other, out=out._residual_tensor
-            )
+            return core.decBLAS.cc_sub_(self, other)
+        elif isinstance(other, (_int, _float, _bool, Tensor)):
+            return core.decBLAS.ct_sub_(self, other)
         else:
-            out_composition_tensor = self._composition_tensor * other
-            out_residual_tensor = self._residual_tensor * other
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+            raise unsupported_operand_error("sub_", type(self), type(other))
 
+    @_auto_registration
+    def mul(self, other: Union[Tensor, Number]) -> Composition:
+        return pydec.mul(self, other)
+
+    @_auto_registration
     def mul_(self, other: Union[Tensor, Number]) -> Composition:
-        self *= other
-        return self
+        if not isinstance(self, Composition):
+            # TODO: maybe return a composition is a good choice
+            raise unsupported_operand_error("mul_", type(self), type(other))
+        if isinstance(other, Composition):
+            # TODO: not implement yet
+            raise unsupported_operand_error("mul_", type(self), type(other))
+        elif isinstance(other, (_int, _float, _bool, Tensor)):
+            return core.decBLAS.ct_mul_(self, other)
+        else:
+            raise unsupported_operand_error("mul_", type(self), type(other))
 
+    @_auto_registration
     def div(
         self, other: Union[Tensor, Number], *, rounding_mode: Optional[str] = None
     ) -> Composition:
-        if isinstance(other, Composition):
-            raise args_error(
-                Composition.div.__name__, self, other, rounding_mode=rounding_mode
-            )
-        if isinstance(other, Tensor):
-            if other.dim() > self.dim():
-                new_size = (
-                    (self.numc(),) + (1,) * (other.dim() - self.dim()) + self.size()
-                )
-                out_composition_tensor = self._composition_tensor.view(new_size).div(
-                    other, rounding_mode=rounding_mode
-                )
-            else:
-                out_composition_tensor = self._composition_tensor.div(
-                    other, rounding_mode == rounding_mode
-                )
-            out_residual_tensor = self._residual_tensor.div(
-                other, rounding_mode=rounding_mode
-            )
-        else:
-            out_composition_tensor = self._composition_tensor.div(
-                other, rounding_mode=rounding_mode
-            )
-            out_residual_tensor = self._residual_tensor.div(
-                other, rounding_mode=rounding_mode
-            )
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.div(self, other, rounding_mode=rounding_mode)
 
+    @_auto_registration
     def div_(
         self, other: Union[Tensor, Number], *, rounding_mode: Optional[str] = None
     ) -> Composition:
+        if not isinstance(self, Composition):
+            # TODO: maybe return a composition is a good choice
+            raise unsupported_operand_error("div_", type(self), type(other))
         if isinstance(other, Composition):
-            raise args_error(
-                Composition.div_.__name__, self, other, rounding_mode=rounding_mode
-            )
-        if isinstance(other, Tensor):
-            if other.dim() > self.dim():
-                new_size = (
-                    (self.numc(),) + (1,) * (other.dim() - self.dim()) + self.size()
-                )
-                self._composition_tensor.view(new_size).div_(
-                    other, rounding_mode=rounding_mode
-                )
-            else:
-                self._composition_tensor.div_(other, rounding_mode == rounding_mode)
-            self._residual_tensor.div_(other, rounding_mode=rounding_mode)
+            # TODO: not implement yet
+            raise unsupported_operand_error("div_", type(self), type(other))
+        elif isinstance(other, (_int, _float, _bool, Tensor)):
+            return core.decBLAS.ct_div_(self, other, rounding_mode=rounding_mode)
         else:
-            self._composition_tensor.div_(other, rounding_mode=rounding_mode)
-            self._residual_tensor.div_(other, rounding_mode=rounding_mode)
-        return self
+            raise unsupported_operand_error("div_", type(self), type(other))
 
+    @_auto_registration
     def mv(self, vec: Tensor) -> Composition:
-        r"""
-        Note that the use of Tensor.mv(Composition) is not supported and may raise an error in autoracing.
-        Use pydec.mv() instead or use torch.mv() in autotracing instead.
-        """
-        out_residual_tensor = self._residual_tensor.mv(vec)
-        out_composition_tensor = self._composition_tensor @ vec
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.mv(self, vec)
 
+    @_auto_registration
     def mm(self, mat2: Tensor) -> Composition:
-        r"""
-        Note that the use of Tensor.mm(Composition) is not supported and may raise an error in autoracing.
-        Use pydec.mm() instead or use torch.mm() in autotracing instead.
-        """
-        out_residual_tensor = self._residual_tensor.mm(mat2)
-        out_composition_tensor = self._composition_tensor @ mat2
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.mm(self, mat2)
 
     @overload
     def any(self) -> Tensor:
         ...
 
     @overload
     def any(self, dim: _int, keepdim: _bool = False) -> Tensor:
         ...
 
+    @_auto_registration
     def any(self, *args: Any, **kwargs: Any) -> Tensor:
-        return self.c_sum().any(*args, **kwargs)
+        return pydec.any(self, *args, **kwargs)
 
     @overload
     def all(self) -> Tensor:
         ...
 
     @overload
     def all(self, dim: _int, keepdim: _bool = False) -> Tensor:
         ...
 
+    @_auto_registration
     def all(self, *args: Any, **kwargs: Any) -> Tensor:
-        return self.c_sum().all(*args, **kwargs)
+        return pydec.all(self, *args, **kwargs)
+
+    @overload
+    def eq(self, other: Tensor) -> Composition:
+        ...
+
+    @overload
+    def eq(self, other: Composition) -> Composition:
+        ...
+
+    @overload
+    def eq(self, other: Number) -> Composition:
+        ...
+
+    @_auto_registration
+    def eq(self, other):
+        return pydec.eq(self, other)
+
+    @overload
+    def ne(self, other: Tensor) -> Composition:
+        ...
 
+    @overload
+    def ne(self, other: Composition) -> Composition:
+        ...
+
+    @overload
+    def ne(self, other: Number) -> Composition:
+        ...
+
+    @_auto_registration
+    def ne(self, other):
+        return pydec.ne(self, other)
+
+    @overload
+    def gt(self, other: Tensor) -> Composition:
+        ...
+
+    @overload
+    def gt(self, other: Composition) -> Composition:
+        ...
+
+    @overload
+    def gt(self, other: Number) -> Composition:
+        ...
+
+    @_auto_registration
+    def gt(self, other):
+        return pydec.gt(self, other)
+
+    @overload
+    def lt(self, other: Tensor) -> Composition:
+        ...
+
+    @overload
+    def lt(self, other: Composition) -> Composition:
+        ...
+
+    @overload
+    def lt(self, other: Number) -> Composition:
+        ...
+
+    @_auto_registration
+    def lt(self, other):
+        return pydec.lt(self, other)
+
+    @overload
+    def ge(self, other: Tensor) -> Composition:
+        ...
+
+    @overload
+    def ge(self, other: Composition) -> Composition:
+        ...
+
+    @overload
+    def ge(self, other: Number) -> Composition:
+        ...
+
+    @_auto_registration
+    def ge(self, other):
+        return pydec.ge(self, other)
+
+    @overload
+    def le(self, other: Tensor) -> Composition:
+        ...
+
+    @overload
+    def le(self, other: Composition) -> Composition:
+        ...
+
+    @overload
+    def le(self, other: Number) -> Composition:
+        ...
+
+    @_auto_registration
+    def le(self, other):
+        return pydec.le(self, other)
+
+    @_auto_registration
     def unsqueeze(self, dim: _int) -> Composition:
-        out_residual_tensor = self._residual_tensor.unsqueeze(dim)
-        out_composition_tensor = self._composition_tensor.unsqueeze(_shift_dim(dim))
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.unsqueeze(self, dim)
 
     @overload
     def squeeze(self) -> Composition:
         ...
 
     @overload
     def squeeze(self, dim: _int) -> Composition:
         ...
 
-    def squeeze(self, dim: _int = None) -> Composition:
-        if dim is None:
-            out_residual_tensor = self._residual_tensor.squeeze()
-            out_composition_tensor = self._composition_tensor.squeeze()
-            if self.numc() == 1:
-                out_composition_tensor = out_composition_tensor.unsqueeze(0)
-        else:
-            out_residual_tensor = self._residual_tensor.squeeze(dim)
-            out_composition_tensor = self._composition_tensor.squeeze(_shift_dim(dim))
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+    @_auto_registration
+    def squeeze(self, dim=None) -> Composition:
+        return pydec.squeeze(self, dim)
 
+    @_auto_registration
     def unsqueeze_(self, dim: _int) -> Composition:
         self._residual_tensor.unsqueeze_(dim)
-        self._composition_tensor.unsqueeze_(_shift_dim(dim))
+        self._component_tensor.unsqueeze_(_shift_dim(dim))
         return self
 
     @overload
     def squeeze_(self) -> Composition:
         ...
 
     @overload
     def squeeze_(self, dim: _int) -> Composition:
         ...
 
-    def squeeze_(self, dim: _int = None) -> Composition:
+    @_auto_registration
+    def squeeze_(self, dim=None) -> Composition:
         if dim is None:
             self._residual_tensor.squeeze_()
             if self.numc() == 1:
-                self._composition_tensor.squeeze_().unsqueeze_(0)
+                self._component_tensor.squeeze_().unsqueeze_(0)
             else:
-                self._composition_tensor.squeeze_()
+                self._component_tensor.squeeze_()
         else:
             self._residual_tensor.squeeze_(dim)
-            self._composition_tensor.squeeze_(_shift_dim(dim))
+            self._component_tensor.squeeze_(_shift_dim(dim))
         return self
 
+    @_auto_registration
     def transpose(self, dim0: _int, dim1: _int) -> Composition:
-        out_residual_tensor = self._residual_tensor.transpose(dim0, dim1)
-        out_composition_tensor = self._composition_tensor.transpose(
-            _shift_dim(dim0), _shift_dim(dim1)
-        )
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.transpose(self, dim0, dim1)
 
+    @_auto_registration
     def transpose_(self, dim0: _int, dim1: _int) -> Composition:
         self._residual_tensor.transpose_(dim0, dim1)
-        self._composition_tensor.transpose_(_shift_dim(dim0), _shift_dim(dim1))
+        self._component_tensor.transpose_(_shift_dim(dim0), _shift_dim(dim1))
         return self
 
     @overload
     def permute(self, dims: _size) -> Composition:
         ...
 
     @overload
     def permute(self, *dims: _int) -> Composition:
         ...
 
+    @_auto_registration
     def permute(self, *args, **kwargs) -> Composition:
         if len(kwargs) == 1:
             dims = kwargs["dims"]
         elif isinstance(args[0], _int):
             dims = torch.Size(args)
         else:
             dims = args[0]
-        out_residual_tensor = self._residual_tensor.permute(dims)
-        out_composition_tensor = self._composition_tensor.permute(
-            (0,) + _shift_dims(dims)
-        )
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.permute(self, dims=dims)
 
     @overload
     def sum(self, *, dtype: Optional[_dtype] = None) -> Composition:
         ...
 
     @overload
     def sum(
@@ -810,36 +820,22 @@
         dim: Union[_int, _size],
         keepdim: _bool = False,
         *,
         dtype: Optional[_dtype] = None,
     ) -> Composition:
         ...
 
+    @_auto_registration
     def sum(
         self, dim=None, keepdim: _bool = False, *, dtype: Optional[_dtype] = None
     ) -> Composition:
-        if dim is None:
-            dim = tuple(range(1, self._composition_tensor.dim()))
-            out_composition_tensor = self._composition_tensor.sum(dim, dtype=dtype)
-            out_residual_tensor = self._residual_tensor.sum(dtype=dtype)
-        else:
-            out_residual_tensor = self._residual_tensor.sum(
-                dim=dim, keepdim=keepdim, dtype=dtype
-            )
-            if isinstance(dim, _int):
-                dim = (dim,)
-            out_composition_tensor = self._composition_tensor.sum(
-                dim=_shift_dims(dim), keepdim=keepdim, dtype=dtype
-            )
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.sum(self, dim=dim, keepdim=keepdim, dtype=dtype)
 
     def c_sum(self, *, dtype: Optional[_dtype] = None) -> Tensor:
-        return self._composition_tensor.sum(
-            dim=0, dtype=dtype
-        ) + self._residual_tensor.to(dtype=dtype)
+        return pydec.c_sum(self, dtype=dtype)
 
     @overload
     def mean(self, *, dtype: Optional[_dtype] = None) -> Composition:
         ...
 
     @overload
     def mean(
@@ -847,101 +843,102 @@
         dim: Union[_int, _size],
         keepdim: _bool = False,
         *,
         dtype: Optional[_dtype] = None,
     ) -> Composition:
         ...
 
+    @_auto_registration
     def mean(
         self,
-        dim: Union[_int, _size] = None,
+        dim=None,
         keepdim: _bool = False,
         *,
         dtype: Optional[_dtype] = None,
     ):
-        if dim is None:
-            dim = tuple(range(1, self._composition_tensor.dim()))
-            out_composition_tensor = self._composition_tensor.mean(dim, dtype=dtype)
-            out_residual_tensor = self._residual_tensor.mean(dtype=dtype)
-        else:
-            out_residual_tensor = self._residual_tensor.mean(
-                dim=dim, keepdim=keepdim, dtype=dtype
-            )
-            if isinstance(dim, _int):
-                dim = (dim,)
-            out_composition_tensor = self._composition_tensor.mean(
-                dim=_shift_dims(dim), keepdim=keepdim, dtype=dtype
-            )
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.mean(self, dim, keepdim, dtype=dtype)
 
     @overload
     def view(self, dtype: _dtype) -> Composition:
         ...
 
     @overload
     def view(self, size: _size) -> Composition:
         ...
 
     @overload
     def view(self, *size: _int) -> Composition:
         ...
 
+    @_auto_registration
     def view(self, *args, dtype=None, size=None) -> Composition:
         if dtype is None and size is None:
             if isinstance(args[0], _dtype):
                 dtype = args[0]
             elif isinstance(args[0], _int):
                 size = torch.Size(args)
             else:
                 size = args[0]
 
         if dtype is not None:
-            out_composition_tensor = self._composition_tensor.view(dtype)
+            out_component_tensor = self._component_tensor.view(dtype)
             out_residual_tensor = self._residual_tensor.view(dtype)
         else:
-            out_composition_tensor = self._composition_tensor.view(
-                (self.numc(),) + size
-            )
+            out_component_tensor = self._component_tensor.view((self.numc(),) + size)
             out_residual_tensor = self._residual_tensor.view(size)
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.as_composition(out_component_tensor, out_residual_tensor)
+
+    @overload
+    def view_as(self, other: Tensor) -> Composition:
+        ...
 
+    @overload
+    def view_as(self, other: Composition) -> Composition:
+        ...
+
+    @_auto_registration
     def view_as(self, other: Union[Tensor, Composition]) -> Composition:
         return self.view(other.size())
 
     @overload
     def reshape(self, shape: _size) -> Composition:
         ...
 
     @overload
     def reshape(self, *shape: _int) -> Composition:
         ...
 
+    @_auto_registration
     def reshape(self, *args, shape=None) -> Composition:
         if shape is None:
             if isinstance(args[0], _int):
                 shape = torch.Size(args)
             else:
                 shape = args[0]
-        out_composition_tensor = self._composition_tensor.view((self.numc(),) + shape)
-        out_residual_tensor = self._residual_tensor.view(shape)
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.reshape(self, shape=shape)
 
+    @_auto_registration
     def reshape_as(self, other: Tensor) -> Composition:
-        return self.reshape_as(other.size())
+        return self.reshape(other.size())
 
+    @_auto_registration
     def contiguous(self, memory_format=torch.contiguous_format) -> Composition:
-        out_composition_tensor = self._composition_tensor.contiguous()
-        out_residual_tensor = self._residual_tensor.contiguous()
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        out_component_tensor = self._component_tensor.contiguous(
+            memory_format=memory_format
+        )
+        out_residual_tensor = self._residual_tensor.contiguous(
+            memory_format=memory_format
+        )
+        return pydec.as_composition(out_component_tensor, out_residual_tensor)
 
+    @_auto_registration
     def is_contiguous(self, memory_format=torch.contiguous_format) -> _bool:
-        return (
-            self._composition_tensor.is_contiguous()
-            and self._residual_tensor.is_contiguous()
-        )
+        return self._component_tensor.is_contiguous(
+            memory_format=memory_format
+        ) and self._residual_tensor.is_contiguous(memory_format=memory_format)
 
     @overload
     def to(
         self, dtype: _dtype, non_blocking: _bool = False, copy: _bool = False
     ) -> Composition:
         ...
 
@@ -954,63 +951,80 @@
         copy: _bool = False,
     ) -> Composition:
         ...
 
     @overload
     def to(
         self,
-        other: Union[Tensor, Composition],
+        other: Tensor,
+        non_blocking: _bool = False,
+        copy: _bool = False,
+    ) -> Composition:
+        ...
+
+    @overload
+    def to(
+        self,
+        other: Composition,
         non_blocking: _bool = False,
         copy: _bool = False,
     ) -> Composition:
         ...
 
+    @_auto_registration
     def to(self, *args, **kwargs) -> Composition:
+        if isinstance(self, Tensor):
+            assert isinstance(args[0], Composition)
+            return self.to(args[0].residual, *args[1:], **kwargs)
         if isinstance(args[0], Composition):
-            return self.to(args[0]._composition_tensor, *args[1:], **kwargs)
+            return self.to(args[0]._component_tensor, *args[1:], **kwargs)
         else:
-            out_composition_tensor = self._composition_tensor.to(*args, **kwargs)
+            out_component_tensor = self._component_tensor.to(*args, **kwargs)
             out_residual_tensor = self._residual_tensor.to(*args, **kwargs)
-            return _from_replce(out_composition_tensor, out_residual_tensor)
+            return pydec.as_composition(out_component_tensor, out_residual_tensor)
 
     @overload
     def masked_fill(self, mask: Tensor, value: Tensor) -> Composition:
         ...
 
     @overload
     def masked_fill(self, mask: Tensor, value: Number) -> Composition:
         ...
 
+    @_auto_registration
     def masked_fill(self, mask: Tensor, value: Any) -> Composition:
+        return pydec.masked_fill(self, mask, value)
+
+    @overload
+    def masked_fill_(self, mask: Tensor, value: Tensor) -> Composition:
+        ...
+
+    @overload
+    def masked_fill_(self, mask: Tensor, value: Number) -> Composition:
+        ...
+
+    @_auto_registration
+    def masked_fill_(self, mask: Tensor, value: Any) -> Composition:
         r"""
         Unsafe.
         """
-        out_composition_tensor = self._composition_tensor.masked_fill(mask[None], value)
-        out_residual_tensor = self._residual_tensor.masked_fill(mask, value)
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        self._component_tensor.masked_fill_(mask[None], value)
+        self._residual_tensor.masked_fill_(mask, value)
+        return self
 
     @overload
     def c_masked_fill(self, mask: Tensor, value: Tensor) -> Composition:
         ...
 
     @overload
     def c_masked_fill(self, mask: Tensor, value: Number) -> Composition:
         ...
 
     def c_masked_fill(self, mask: Tensor, value: Any) -> Composition:
-        if mask.dim() == 1:
-            if len(mask) != self.numc():
-                raise arg_value_error(
-                    f"the length of mask ({len(mask)}) should match component number ({self.numc()})"
-                )
-            mask_size = (self.numc(),) + (1,) * self.dim()
-            mask = mask.view(mask_size)
-        out_composition_tensor = self._composition_tensor.masked_fill(mask, value)
-        out_residual_tensor = self._residual_tensor.clone()
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.c_masked_fill(self, mask, value)
 
     @overload
     def c_masked_fill_(self, mask: Tensor, value: Tensor) -> Composition:
         ...
 
     @overload
     def c_masked_fill_(self, mask: Tensor, value: Number) -> Composition:
@@ -1020,75 +1034,37 @@
         if mask.dim() == 1:
             if len(mask) != self.numc():
                 raise arg_value_error(
                     f"the length of mask ({len(mask)}) should match component number ({self.numc()})"
                 )
             mask_size = (self.numc(),) + (1,) * self.dim()
             mask = mask.view(mask_size)
-        self._composition_tensor.masked_fill_(mask, value)
-        return self
-
-    @overload
-    def masked_fill_(self, mask: Tensor, value: Tensor) -> Composition:
-        ...
-
-    @overload
-    def masked_fill_(self, mask: Tensor, value: Number) -> Composition:
-        ...
-
-    def masked_fill_(self, mask: Tensor, value: Any) -> Composition:
-        r"""
-        Unsafe.
-        """
-        self._composition_tensor.masked_fill_(mask[None], value)
-        self._residual_tensor.masked_fill_(mask, value)
+        self._component_tensor.masked_fill_(mask, value)
         return self
 
+    @_auto_registration
     def masked_select(self, mask: Tensor) -> Composition:
-        out_composition_tensor = self._composition_tensor.masked_select(
-            mask[None]
-        ).reshape(self.numc(), -1)
-        out_residual_tensor = self._residual_tensor.masked_select(mask)
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.masked_select(self, mask)
 
+    @_auto_registration
     def masked_scatter(self, mask: Tensor, source: Tensor) -> Composition:
-        r"""
-        Unsafe.
-        """
-        out_composition_tensor = self._composition_tensor.masked_scatter(
-            mask[None], source
-        )
-        out_residual_tensor = self._residual_tensor.masked_scatter(mask, source)
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.masked_scatter(self, mask, source)
 
+    @_auto_registration
     def masked_scatter_(self, mask: Tensor, source: Tensor) -> Composition:
-        r"""
-        Unsafe.
-        """
-        self._composition_tensor.masked_scatter_(mask[None], source)
+        # TODO: seems not make sense, see examples in docs
+        self._component_tensor.masked_scatter_(mask[None], source)
         self._residual_tensor.masked_scatter_(mask, source)
         return self
 
-    @overload
+    @_auto_registration
     def gather(
         self, dim: _int, index: Tensor, *, sparse_grad: _bool = False
     ) -> Composition:
-        ...
-
-    def gather(
-        self, dim: Any, index: Tensor, *, sparse_grad: _bool = False
-    ) -> Composition:
-        c_index = index[None].expand((self.numc(),) + (-1,) * index.dim())
-        out_composition_tensor = self._composition_tensor.gather(
-            _shift_dim(dim), c_index, sparse_grad=sparse_grad
-        )
-        out_residual_tensor = self._residual_tensor.gather(
-            dim, index, sparse_grad=sparse_grad
-        )
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.gather(self, dim, index, sparse_grad=sparse_grad)
 
     @overload
     def scatter(self, dim: _int, index: Tensor, src: Tensor) -> Composition:
         ...
 
     @overload
     def scatter(
@@ -1102,52 +1078,28 @@
     ) -> Composition:
         ...
 
     @overload
     def scatter(self, dim: _int, index: Tensor, value: Number) -> Composition:
         ...
 
+    @_auto_registration
     def scatter(
         self,
         dim: _int,
         index: Tensor,
-        src: Any = None,
-        value: Any = None,
+        src_value: Optional[Union[Tensor, Number]] = None,
         *,
-        reduce: str = None,
-    ) -> Composition:
-        r"""
-        Unsafe.
-        Safe when reduce is not None.
-        """
-        if src is None:
-            src = value
-        if reduce == "add":
-            holder = torch.zeros_like(self._residual_tensor).to(self._residual_tensor)
-            holder = holder.scatter(dim, index, src, reduce=reduce)
-            return self + holder
-        else:
-            c_index = index[None].expand((self.numc(),) + (-1,) * index.dim())
-            if isinstance(src, Tensor):
-                c_src = src[None].expand((self.numc(),) + (-1,) * src.dim())
-            else:
-                c_src = src
-            if reduce is None:
-                out_composition_tensor = self._composition_tensor.scatter(
-                    _shift_dim(dim), c_index, c_src
-                )
-                out_residual_tensor = self._residual_tensor.scatter(dim, index, src)
-            else:
-                out_composition_tensor = self._composition_tensor.scatter(
-                    _shift_dim(dim), c_index, c_src, reduce=reduce
-                )
-                out_residual_tensor = self._residual_tensor.scatter(
-                    dim, index, src, reduce=reduce
-                )
-            return _from_replce(out_composition_tensor, out_residual_tensor)
+        reduce: Optional[str] = None,
+        src: Optional[Tensor] = None,
+        value: Optional[Number] = None,
+    ) -> Composition:
+        if src_value is None:
+            src_value = src if src is not None else value
+        return pydec.scatter(self, dim, index, src_value, reduce=reduce)  # type: ignore[arg-type]
 
     @overload
     def scatter_(self, dim: _int, index: Tensor, src: Tensor) -> Tensor:
         ...
 
     @overload
     def scatter_(self, dim: _int, index: Tensor, src: Tensor, *, reduce: str) -> Tensor:
@@ -1159,251 +1111,391 @@
     ) -> Tensor:
         ...
 
     @overload
     def scatter_(self, dim: _int, index: Tensor, value: Number) -> Tensor:
         ...
 
+    @_auto_registration
     def scatter_(
         self, dim: Any, index: Tensor, src: Any, *, reduce: str = None
     ) -> Composition:
-        r"""
-        Unsafe.
-        """
         if reduce == "add":
             holder = torch.zeros_like(self._residual_tensor).to(self._residual_tensor)
             holder = holder.scatter(dim, index, src, reduce=reduce)
             self += holder
             return self
         else:
             c_index = index[None].expand((self.numc(),) + (-1,) * index.dim())
             if isinstance(src, Tensor):
                 c_src = src[None].expand((self.numc(),) + (-1,) * src.dim())
             else:
                 c_src = src
             if reduce is None:
-                self._composition_tensor.scatter_(_shift_dim(dim), c_index, c_src)
+                self._component_tensor.scatter_(_shift_dim(dim), c_index, c_src)
                 self._residual_tensor.scatter_(dim, index, src)
             else:
-                self._composition_tensor.scatter_(
+                self._component_tensor.scatter_(
                     _shift_dim(dim), c_index, c_src, reduce=reduce
                 )
                 self._residual_tensor.scatter_(dim, index, src, reduce=reduce)
             return self
 
+    @_auto_registration
     def diagonal_scatter(
         self, src: Tensor, offset: _int = 0, dim1: _int = 0, dim2: _int = 1
     ) -> Composition:
-        r"""
-        Unsafe.
-        """
-        c_src = src[None].expand((self.numc(),) + (-1,) * src.dim())
-        out_composition_tensor = self._composition_tensor.diagonal_scatter(
-            c_src, offset, _shift_dim(dim1), _shift_dim(dim2)
-        )
-        out_residual_tensor = self._residual_tensor.diagonal_scatter(
-            src, offset, dim1, dim2
-        )
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.diagonal_scatter(self, src, offset, dim1, dim2)
 
+    @_auto_registration
     def cuda(
         self,
         device: Optional[Union[_device, _int, str]] = None,
         non_blocking: _bool = False,
     ) -> Composition:
-        out_composition_tensor = self._composition_tensor.cuda(
+        out_component_tensor = self._component_tensor.cuda(
             device=device, non_blocking=non_blocking
         )
         out_residual_tensor = self._residual_tensor.cuda(
             device=device, non_blocking=non_blocking
         )
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.as_composition(out_component_tensor, out_residual_tensor)
 
+    @_auto_registration
     def cpu(self) -> Composition:
-        out_composition_tensor = self._composition_tensor.cpu()
+        out_component_tensor = self._component_tensor.cpu()
         out_residual_tensor = self._residual_tensor.cpu()
-        return _from_replce(out_composition_tensor, out_residual_tensor)
-
-    def is_cuda(self):
-        return self._composition_tensor.is_cuda and self._residual_tensor.is_cuda
+        return pydec.as_composition(out_component_tensor, out_residual_tensor)
 
     @overload
     def index_select(self, dim: _int, index: Tensor) -> Composition:
         ...
 
+    @_auto_registration
     def index_select(self, dim: _int, index: Tensor) -> Composition:
-        out_composition_tensor = self._composition_tensor.index_select(
-            dim=_shift_dim(dim), index=index
-        )
-        out_residual_tensor = self._residual_tensor.index_select(dim=dim, index=index)
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.index_select(self, dim=dim, index=index)
 
     @overload
     def c_index_select(self, index: Tensor, with_residual: _bool = True) -> Composition:
         ...
 
     def c_index_select(self, index: Tensor, with_residual: _bool = True) -> Composition:
-        out_composition_tensor = self._composition_tensor.index_select(
-            dim=0, index=index
-        )
-        if with_residual:
-            out_residual_tensor = self._residual_tensor.clone()
-        else:
-            out_residual_tensor = torch.zeros_like(self._residual_tensor).to(
-                self._residual_tensor
-            )
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.c_index_select(self, index=index, with_residual=with_residual)
 
+    @_auto_registration
     def masked_select(self, mask: Tensor) -> Composition:
-        out_composition_tensor = self._composition_tensor.masked_select(mask=mask[None])
-        out_residual_tensor = self._residual_tensor.masked_select(mask=mask)
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.masked_select(self, mask)
 
     @overload
     def index_fill(self, dim: _int, index: Tensor, value: Tensor) -> Composition:
         ...
 
     @overload
     def index_fill(self, dim: _int, index: Tensor, value: Number) -> Composition:
         ...
 
+    @_auto_registration
     def index_fill(self, dim: _int, index: Tensor, value: Any) -> Composition:
-        r"""
-        Unsafe.
-        """
-        out_composition_tensor = self._composition_tensor.index_fill(
-            dim=_shift_dim(dim), index=index, value=value
-        )
-        out_residual_tensor = self._residual_tensor.index_fill(
-            dim=dim, index=index, value=value
-        )
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.index_fill(self, dim=dim, index=index, value=value)
 
     @overload
     def index_fill_(self, dim: _int, index: Tensor, value: Tensor) -> Composition:
         ...
 
     @overload
     def index_fill_(self, dim: _int, index: Tensor, value: Number) -> Composition:
         ...
 
+    @_auto_registration
     def index_fill_(self, dim: _int, index: Tensor, value: Number) -> Composition:
-        r"""
-        Unsafe.
-        """
-        self._composition_tensor.index_fill_(
+        self._component_tensor.index_fill_(
             dim=_shift_dim(dim), index=index, value=value
         )
         self._residual_tensor.index_fill_(dim=dim, index=index, value=value)
         return self
 
     @overload
     def select(self, dim: _int, index: _int) -> Composition:
         ...
 
+    @_auto_registration
     def select(self, dim: _int, index: _int) -> Composition:
-        out_composition_tensor = self._composition_tensor.select(
-            dim=_shift_dim(dim), index=index
-        )
-        out_residual_tensor = self._residual_tensor.select(dim=dim, index=index)
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.select(self, dim=dim, index=index)
 
     @overload
     def type(self, dtype: None = None, non_blocking: _bool = False) -> str:
         ...
 
     @overload
     def type(self, dtype: Union[str, _dtype], non_blocking: _bool = False) -> Tensor:
         ...
 
+    @_auto_registration
     def type(self, dtype=None, non_blocking: _bool = False):
         if dtype is None:
             return self._residual_tensor.type()
         else:
-            out_composition_tensor = self._composition_tensor.type(
+            out_component_tensor = self._component_tensor.type(
                 dtype=dtype, non_blocking=non_blocking
             )
             out_residual_tensor = self._residual_tensor.type(
                 dtype=dtype, non_blocking=non_blocking
             )
-            return _from_replce(out_composition_tensor, out_residual_tensor)
+            return pydec.as_composition(out_component_tensor, out_residual_tensor)
 
+    @overload
+    def type_as(self, other: Tensor) -> Composition:
+        ...
+
+    @overload
+    def type_as(self, other: Composition) -> Composition:
+        ...
+
+    @_auto_registration
     def type_as(self, other: Union[Tensor, Composition]) -> Composition:
         if isinstance(other, Composition):
-            out_composition_tensor = self._composition_tensor.type_as(
-                other._composition_tensor
-            )
-            out_residual_tensor = self._residual_tensor.type_as(
-                other._composition_tensor
+            out_component_tensor = self._component_tensor.type_as(
+                other._component_tensor
             )
+            out_residual_tensor = self._residual_tensor.type_as(other._component_tensor)
         else:
-            out_composition_tensor = self._composition_tensor.type_as(other)
+            out_component_tensor = self._component_tensor.type_as(other)
             out_residual_tensor = self._residual_tensor.type_as(other)
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.as_composition(out_component_tensor, out_residual_tensor)
 
     @overload
     def round(self) -> Composition:
         ...
 
     @overload
     def round(self, *, decimals: _int) -> Composition:
         ...
 
+    @_auto_registration
     def round(self, *, decimals: _int = None):
-        if decimals is not None:
-            out_composition_tensor = self._composition_tensor.round(decimals=decimals)
-            out_residual_tensor = self._residual_tensor.round(decimals=decimals)
-        else:
-            out_composition_tensor = self._composition_tensor.round()
-            out_residual_tensor = self._residual_tensor.round()
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.round(self, decimals=decimals)
 
     @overload
     def round_(self) -> Composition:
         ...
 
     @overload
     def round_(self, *, decimals: _int) -> Composition:
         ...
 
+    @_auto_registration
     def round_(self, *, decimals: _int = None) -> Composition:
-        if decimals is not None:
-            self._composition_tensor.round_(decimals=decimals)
-            self._residual_tensor.round_(decimals=decimals)
-        else:
-            self._composition_tensor.round_()
-            self._residual_tensor.round_()
-        return self
+        return pydec.round_(self, decimals=decimals)
 
+    @_auto_registration
     def abs(self) -> Composition:
-        out_composition_tensor = self._composition_tensor.abs()
-        out_residual_tensor = self._residual_tensor.abs()
-        return _from_replce(out_composition_tensor, out_residual_tensor)
+        return pydec.abs(self)
 
+    @_auto_registration
     def abs_(self) -> Composition:
-        self._composition_tensor.abs_()
-        self._residual_tensor.abs_()
-        return self
+        return pydec.abs_(self)
 
+    @_auto_registration
     def requires_grad_(self, mode: _bool = True) -> Composition:
-        self._composition_tensor.requires_grad_(mode)
+        self._component_tensor.requires_grad_(mode)
         self._residual_tensor.requires_grad_(mode)
         return self
 
+    @_auto_registration
     def apply_(self, callable: Callable) -> Composition:
-        self._composition_tensor.apply_(callable)
+        self._component_tensor.apply_(callable)
         self._residual_tensor.apply_(callable)
         return self
 
+    @_auto_registration
     def map_(self, composition: Composition, callable: Callable) -> Composition:
         self._residual_tensor.map_(composition._residual_tensor, callable)
         # permute to be broadcastable
-        p_dims = [i for i in range(1, self._composition_tensor.dim())] + [0]
-        p_composition_tensor = self._composition_tensor.permute(*p_dims)
-        p_dims = [i for i in range(1, composition._composition_tensor.dim())] + [0]
-        p_other_composition_tensor = composition.permute(*p_dims)
-        p_composition_tensor.map_(p_other_composition_tensor, callable)
+        p_dims = [i for i in range(1, self._component_tensor.dim())] + [0]
+        p_component_tensor = self._component_tensor.permute(*p_dims)
+        p_dims = [i for i in range(1, composition._component_tensor.dim())] + [0]
+        p_other_component_tensor = composition.permute(*p_dims)
+        p_component_tensor.map_(p_other_component_tensor, callable)
 
         # recover
-        p_dims = [-1] + [i for i in range(0, p_composition_tensor.dim() - 1)]
-        self._composition_tensor = p_composition_tensor.permute(p_dims)
+        p_dims = [-1] + [i for i in range(0, p_component_tensor.dim() - 1)]
+        self._component_tensor = p_component_tensor.permute(p_dims)
         return self
+
+    @_auto_registration
+    def relu(self, *, ref: Optional[Tensor] = None) -> Composition:
+        return pydec.relu(self, ref=ref)
+
+    @_auto_registration
+    def relu_(self, *, ref: Optional[Tensor] = None) -> Composition:
+        return pydec.relu_(self, ref=ref)
+
+    @_auto_registration
+    def tanh(self, *, ref: Optional[Tensor] = None) -> Composition:
+        return pydec.tanh(self, ref=ref)
+
+    @_auto_registration
+    def tanh_(self, *, ref: Optional[Tensor] = None) -> Composition:
+        return pydec.tanh_(self, ref=ref)
+
+    @_auto_registration
+    def sigmoid(self, *, ref: Optional[Tensor] = None) -> Composition:
+        return pydec.sigmoid(self, ref=ref)
+
+    @_auto_registration
+    def sigmoid_(self, *, ref: Optional[Tensor] = None) -> Composition:
+        return pydec.sigmoid_(self, ref=ref)
+
+    @_auto_registration
+    def reciprocal(self) -> Composition:
+        return pydec.reciprocal(self)
+
+    @_auto_registration
+    def reciprocal_(self) -> Composition:
+        return pydec.reciprocal_(self)
+
+    @_auto_registration
+    def exp(self) -> Composition:
+        return pydec.exp(self)
+
+    @_auto_registration
+    def exp(self) -> Composition:
+        return pydec.exp_(self)
+
+    @overload
+    def softmax(self, dim: _int, dtype: Optional[_dtype] = None) -> Composition:
+        ...
+
+    @overload
+    def softmax(
+        self, dim: Union[str, ellipsis, None], *, dtype: Optional[_dtype] = None
+    ) -> Composition:
+        ...
+
+    @_auto_registration
+    def softmax(self, dim: Any, dtype: Optional[_dtype] = None) -> Composition:
+        return pydec.softmax(self, dim, dtype)
+
+    def sqrt(self) -> Composition:
+        return pydec.sqrt(self)
+
+    def sqrt_(self) -> Composition:
+        return pydec.sqrt_(self)
+
+
+class IndexComposition(Composition):
+    """
+    TODO
+    """
+
+    # we use this number to represent empty value
+    # all indices should avoid this value
+    MASK_NUM = -2147483648
+
+    @property
+    def empty_mask(self) -> Tensor:
+        return (
+            self.components == IndexComposition.MASK_NUM,
+            self.residual == IndexComposition.MASK_NUM,
+        )
+
+    @overload
+    def __init__(
+        self,
+        component_tensor: Tensor,
+        residual_tensor: Tensor = None,
+    ) -> None:
+        ...
+
+    @overload
+    def __init__(self, composition: IndexComposition) -> None:
+        ...
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+
+        if len(args) + len(kwargs) == 0:
+            # a private constructor to create a void composition with no data,
+            # which is usually assigned in `_from_replace`.
+            return
+
+        # Type checking
+        accept_dtypes = [torch.int, torch.long]
+        msg = "Expected arguments to have one of the following scalar types: {}; but got {} instead (while checking arguments for IndexComposition)"
+
+        if self.dtype not in accept_dtypes:
+            raise RuntimeError(msg.format(accept_dtypes, self.dtype))
+
+    def __repr__(self, *, composition_contents: List[str] = None) -> str:
+        # TODO
+        # TODO: add example for docs
+        return super().__repr__(composition_contents=composition_contents)
+
+
+class _C_AccessingMode:
+    is_enabled = False
+
+    @classmethod
+    def set_enabled(cls, enabled: _bool):
+        cls.is_enabled = enabled
+
+
+def is_c_accessing_enabled() -> _bool:
+    return _C_AccessingMode.is_enabled
+
+
+class enable_c_accessing(_DecoratorContextManager):
+    r"""Context-manager that enables component indexing and slicing."""
+
+    def __enter__(self) -> None:
+        self.prev = is_c_accessing_enabled()
+        _C_AccessingMode.set_enabled(True)
+
+    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
+        _C_AccessingMode.set_enabled(self.prev)
+
+
+class set_c_accessing_enabled(_DecoratorContextManager):
+    r"""Context-manager that sets c_accessing to on or off."""
+
+    def __init__(self, mode: bool) -> None:
+        self.prev = is_c_accessing_enabled()
+        _C_AccessingMode.set_enabled(mode)
+        self.mode = mode
+
+    def __enter__(self) -> None:
+        pass
+
+    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
+        _C_AccessingMode.set_enabled(self.prev)
+
+    def clone(self):
+        return self.__class__(self.mode)
+
+
+class _C_AccessingComposition(Composition):
+    r"""
+    TODO: A temporary type for implementation of component subscript accessing for Composition.
+    """
+
+    def __init__(self, composition: Composition):
+        super().__init__()  # void initialization
+        self._component_tensor = composition._component_tensor
+        self._residual_tensor = composition._residual_tensor
+
+    def __getitem__(
+        self, indices: Union[None, _int, slice, Tensor, List, Tuple]
+    ) -> Union[Composition, Tensor]:
+        return super().__c_getitem__(indices)
+
+    def __setitem__(
+        self,
+        indices: Union[None, _int, slice, Tensor, List, Tuple],
+        val: Union[Composition, Tensor, Number],
+    ) -> None:
+        return super().__c_setitem__(indices, val)
+
+    def __len__(self):
+        return self.components.__len__()
+
+    def __iter__(self):
+        return self._component_tensor.__iter__()
```

### Comparing `pydec-0.2.0/pydec/decomposition/states.py` & `pydec-0.3.0/pydec/core/decOVF/states.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+from __future__ import annotations
 import functools
 import inspect
 
 from torch.autograd.grad_mode import _DecoratorContextManager
 
 from typing import Dict, Tuple, Union, Any, Callable, Optional, TYPE_CHECKING
 
-from ..composition import Composition
+if TYPE_CHECKING:
+    from ..._composition import Composition
 
 from torch.types import (
     _int,
     _float,
     _bool,
     Number,
     _dtype,
     _device,
     _qscheme,
     _size,
     _layout,
-    SymInt,
 )
 
 _DECOMPOSITION_FUNC_REGISTRY = {}
 
 
 class _DecompositionState:
     decomposition_name: str = None
@@ -111,28 +112,14 @@
     def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
         _DecompositionState.decomposition_name = self.prev
 
     def clone(self):
         return self.__class__(self.using_name)
 
 
-class no_decomposition(_DecoratorContextManager):
-    def __init__(
-        self,
-    ) -> None:
-        self.prev = None
-
-    def __enter__(self):
-        self.prev = _DecompositionState.decomposition_name
-        _DecompositionState.decomposition_name = "none"
-
-    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
-        _DecompositionState.decomposition_name = self.prev
-
-
 def set_decomposition_args(update: _bool = True, **kwargs) -> None:
     if update:
         _DecompositionState.decomposition_args.update(kwargs)
     else:
         _DecompositionState.decomposition_args = kwargs
```

### Comparing `pydec-0.2.0/pydec/exception_utils.py` & `pydec-0.3.0/pydec/exception_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Type, Union
+from typing import Type, Union, Optional
 import torch
 from torch.types import _int, _float
 
 
 def args_error(
     funcion_name: str, args: Union[list, tuple], kwargs: dict = {}
 ) -> TypeError:
@@ -20,46 +20,47 @@
     return RuntimeError(msg)
 
 
 def size_error(
     s1: torch.Size, s2: torch.Size, t1_name="tensor1", t2_name="tensor2"
 ) -> RuntimeError:
     return RuntimeError(
-        f"The size of {t1_name} [{s1}] doesn't match the size of {t2_name} [{s2}]."
+        f"The size of {t1_name} [{s1}] doesn't match the size of {t2_name} [{s2}]"
     )
 
 
 def component_num_error(
     num1: _int, num2: _int, c1_name="composition1", c2_name="composition2"
 ) -> RuntimeError:
     return RuntimeError(
-        f"The component number of {c1_name} ({num1}) doesn't match the component number of {c2_name} ({num2})."
+        f"The component number of {c1_name} ({num1}) doesn't match the component number of {c2_name} ({num2})"
     )
 
 
 def unsupported_operand_error(
     operation_name: str, operand_type1: Type, operand_type2: Type
 ) -> TypeError:
     return TypeError(
         f"unsupported operand type(s) for {operation_name}: '{operand_type1.__name__}' and '{operand_type2.__name__}'"
     )
 
 
 def overflow_error(error: _float, error_bound=1e-2) -> RuntimeError:
     return RuntimeError(
-        f"Error overflow in checking, error {error} out of bound {error_bound}."
+        f"Error overflow in checking, error {error} out of bound {error_bound}"
     )
 
 
-def none_decomposition_func_error(func_name: str = None) -> RuntimeError:
+def none_decomposition_func_error(func_name: Optional[str] = None) -> RuntimeError:
     return RuntimeError(
-        f"Cannot find the currently used decomposition function with key name ({func_name})."
+        f"Cannot find the currently used decomposition function with key name ({func_name})"
     )
 
 
+# TODO: deprecated
 def args_error_not_in_tracing(*args, **kwargs):
     error_msg = (
         "received Composition type argument but not in the tracing mode - got ({}).\nTo fix this error: "
         "(1) input tensor instead if you do not want to do tracing or (2) set tracing enabled by Tracer.trace() or pydec.set_tracing_enabled()"
     )
     arg_types = tuple(type(arg).__name__ for arg in args)
     kwarg_types = tuple(
```

### Comparing `pydec-0.2.0/pydec/nn/modules/container.py` & `pydec-0.3.0/pydec/nn/modules/container.py`

 * *Files identical despite different names*

### Comparing `pydec-0.2.0/pydec/nn/modules/linear.py` & `pydec-0.3.0/pydec/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `pydec-0.2.0/pydec/nn/modules/meta.py` & `pydec-0.3.0/pydec/nn/modules/meta.py`

 * *Files identical despite different names*

### Comparing `pydec-0.2.0/pydec/nn/modules/module.py` & `pydec-0.3.0/pydec/nn/modules/module.py`

 * *Files identical despite different names*

### Comparing `pydec-0.2.0/pydec/utils.py` & `pydec-0.3.0/pydec/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 import torch
-from typing import Any, Union, List, Tuple, Optional, Callable, overload
+from typing import (
+    Any,
+    Union,
+    List,
+    Dict,
+    Tuple,
+    Optional,
+    Callable,
+    overload,
+    Sequence,
+    Iterable,
+)
 
 # In some cases, these basic types are shadowed by corresponding
 # top-level values.  The underscore variants let us refer to these
 # types.  See https://github.com/python/mypy/issues/4146 for why these
 # workarounds is necessary
+# In the future, this will become useful if mypy is introduced into pydec
 from torch.types import (
     _int,
     _float,
     _bool,
     Number,
     _dtype,
     _device,
     _qscheme,
     _size,
     _layout,
-    SymInt,
 )
 
 
 def _shift_dim(dim: _int) -> _int:
     if dim >= 0:
         dim += 1
     return dim
 
 
 @overload
-def _shift_dims(dims: _size) -> torch.Size:
+def _shift_dims(dims: _size, /) -> torch.Size:
     ...
 
 
 @overload
 def _shift_dims(*dims: _int) -> torch.Size:
     ...
 
 
-def _shift_dims(*dims) -> torch.Size:
+def _shift_dims(*dims: Any) -> torch.Size:
     if len(dims) == 1:
         dims = dims[0]
     out = list(dims)
     for i in range(len(dims)):
         out[i] = _shift_dim(dims[i])
     return torch.Size(out)
+
+
+def parse_args(args: Iterable[Any], key_list: Iterable[str], kwargs: Dict[str, Any]):
+    for key, arg in zip(key_list, args):
+        kwargs[key] = arg
```

### Comparing `pydec-0.2.0/pydec.egg-info/PKG-INFO` & `pydec-0.3.0/pydec.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydec
-Version: 0.2.0
+Version: 0.3.0
 Summary: Linear decomposition toolkit for neural network based on pytorch.
 Home-page: https://github.com/DoubleVII/pydec/
 Author: Sen Yang
 Author-email: yangsen@smail.nju.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,47 +13,50 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-[![PyPI](https://img.shields.io/pypi/v/pydec)](https://pypi.org/project/pydec/)
-[![Test](https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml/badge.svg?branch=master)](https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml)
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/DoubleVII/pydec/jekyll-gh-pages.yml?label=docs)](https://doublevii.github.io/pydec/)
-[![codecov](https://codecov.io/gh/DoubleVII/pydec/branch/master/graph/badge.svg?token=UGXWFEKQA9)](https://codecov.io/gh/DoubleVII/pydec)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+<p align="center">
+  <img src="docs/_images/PyDec_Logo1.png" width="200">
+</p>
+
+<p align="center">
+  <br />
+  <br />
+  <a href="https://pypi.org/project/pydec/"><img alt="PyPi" src="https://img.shields.io/pypi/v/pydec" /></a>
+  <a href="https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml"><img alt="Test" src="https://github.com/DoubleVII/pydec/actions/workflows/python-package-conda.yml/badge.svg?branch=master" /></a>
+  <a href="https://doublevii.github.io/pydec/"><img alt="Docs Build Status" src="https://img.shields.io/github/actions/workflow/status/DoubleVII/pydec/deploy-static-pages.yml?label=docs" /></a>
+  <a href="https://codecov.io/gh/DoubleVII/pydec"><img alt="codecov" src="https://codecov.io/gh/DoubleVII/pydec/branch/master/graph/badge.svg?token=UGXWFEKQA9" /></a>
+  <a href="https://opensource.org/licenses/MIT"><img alt="MIT License" src="https://img.shields.io/badge/License-MIT-yellow.svg" /></a>
+</p>
 
-
-<h1 align="center" style="font-size:60px">
-  PyDec
-</h1>
+--------------------------------------------------------------------------------
 
 PyDec is a linear decomposition toolkit for neural network based on [PyTorch](https://pytorch.org/), which can decompose the tensor in the forward process into given components with a small amount of code. The result of decomposition can be applied to tasks such as attribution analysis.
 
 ### Features:
 * Fast. Compute decomposition in foward process and benefit from GPU acceleration.
-* Real-time. Outputs attribution along with the model output results.
+* Run once, decompose anywhere. Obtain the decomposition of all hidden states (if you saved them) in forward propagation.
 * Applicable to networks such as Transformer, CNN and RNN.
 
 # Examples
-## Attribution
+<!-- ## Attribution
 Contribution Heat maps of the Roberta model (fine-tuned on SST-2). Warm colors indicate high
 contribution while cool colors indicate low contribution. The outputs of the model were positive, negative and positive, but the latter two samples did not match the labels.
 
 <div align="center">
 <img src="./docs/assets/img/pydec_demo1.png" width="70%">
-</div>
+</div> -->
 
 ## Data flow visualization
 
-![demo2](./docs/assets/img/pydec_demo2_1.gif)
-
-![demo2](./docs/assets/img/pydec_demo2_2.gif)
+![Data flow demo](docs/_images/pydec_demo2_1.gif)
 
 # Requirements and Installation
 * [PyTorch](https://pytorch.org/) version >= 1.11.0
 * Python version >= 3.7
 * To install PyDec and develop locally:
 
 ``` bash
@@ -67,15 +70,15 @@
 pip install pydec
 ```
 
 # Getting Started
 
 ## Example: deompose a tiny network
 
-As a simple example, here’s a very simple model with two linear layers and an activation function. We’ll create an instance of it andand get the decomposition of the output by autotracing:
+As a simple example, here's a very simple model with two linear layers and an activation function. We'll create an instance of it and get the decomposition of the output:
 ```python
 import torch
 
 class TinyModel(torch.nn.Module):
     def __init__(self):
         super(TinyModel, self).__init__()
 
@@ -107,18 +110,16 @@
 Input tensor:
 tensor([0.7023, 0.3492, 0.7771, 0.0157])
 
 
 Output tensor:
 tensor([0.2751, 0.3626], grad_fn=<AddBackward0>)
 ```
-To decompose the output, first wrap the model using `pydec.autotracing.compile` and then input the Composition initialized from `x`:
+To decompose the output, just input the Composition initialized from `x`:
 ```python
-tinymodel = pydec.autotracing.compile(tinymodel)
-
 c = pydec.zeros(x.size(), c_num=x.size(0))
 c = pydec.diagonal_init(c, src=x, dim=0)
 
 print("Input composition:")
 print(c)
 
 c_out = tinymodel(c)
@@ -158,23 +159,15 @@
 print(c_out.c_sum())
 ```
 Out:
 ```
 Sum of each component:
 tensor([0.2751, 0.3626], grad_fn=<AddBackward0>)
 ```
-To restore the ability of the model to forward tensor, use `trace()` to turn off autotracing:
-```python
-tinymodel.trace(False)
-
-print("Output tensor:")
-print(tinymodel(x))
-```
-Out:
-```
-Output tensor:
-tensor([0.2751, 0.3626], grad_fn=<AddBackward0>)
-```
 
 # Documentation
 
-The [full documentation](https://doublevii.github.io/pydec/) contains examples of implementations on realistic models, tutorials, notes and Python API.
+The [full documentation](https://doublevii.github.io/pydec/) contains examples of implementations on real-world models, tutorials, notes and Python API descriptions.
+
+
+# Linear Decomposition Theory
+To understand the principles and theories behind PyDec, see our paper [Local Interpretation of Transformer Based on Linear Decomposition](https://aclanthology.org/2023.acl-long.572/).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydec-0.2.0/pydec.egg-info/SOURCES.txt` & `pydec-0.3.0/pydec.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 LICENSE
 README.md
 setup.py
 pydec/__init__.py
+pydec/_composition.py
 pydec/_composition_str.py
-pydec/composition.py
-pydec/error_check.py
 pydec/exception_utils.py
+pydec/overrides.py
 pydec/utils.py
 pydec/variable_functions.py
 pydec.egg-info/PKG-INFO
 pydec.egg-info/SOURCES.txt
 pydec.egg-info/dependency_links.txt
 pydec.egg-info/requires.txt
 pydec.egg-info/top_level.txt
-pydec/autotracing/__init__.py
-pydec/autotracing/compiler.py
-pydec/autotracing/library.py
-pydec/autotracing/tracer.py
-pydec/autotracing/tracing_mode.py
-pydec/decomposition/__init__.py
-pydec/decomposition/algorithms.py
-pydec/decomposition/states.py
+pydec/core/__init__.py
+pydec/core/decBLAS/__init__.py
+pydec/core/decBLAS/ops.py
+pydec/core/decMVF/__init__.py
+pydec/core/decMVF/ops.py
+pydec/core/decMVF/shapley.py
+pydec/core/decOVF/__init__.py
+pydec/core/decOVF/algorithms.py
+pydec/core/decOVF/ops.py
+pydec/core/decOVF/states.py
 pydec/nn/__init__.py
 pydec/nn/functional.py
 pydec/nn/modules/__init__.py
 pydec/nn/modules/activation.py
 pydec/nn/modules/container.py
 pydec/nn/modules/linear.py
 pydec/nn/modules/meta.py
 pydec/nn/modules/module.py
+pydec/nn/utils/__init__.py
+pydec/nn/utils/rnn.py
 test/__init__.py
-test/test_composition.py
-test/test_decomposition.py
-test/test_nn_functional.py
-test/test_variable_functions.py
+test/_composition_test.py
+test/decomposition_test.py
+test/variable_functions_test.py
```

### Comparing `pydec-0.2.0/setup.py` & `pydec-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "pydec"
 DESCRIPTION = "Linear decomposition toolkit for neural network based on pytorch."
 URL = "https://github.com/DoubleVII/pydec/"
 EMAIL = "yangsen@smail.nju.edu.cn"
 AUTHOR = "Sen Yang"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["torch>=1.11.0", "numpy"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

### Comparing `pydec-0.2.0/test/test_composition.py` & `pydec-0.3.0/test/_composition_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,132 +5,167 @@
 
 torch.manual_seed(114514)
 
 
 def init_composition(size, c_num=3, requires_grad=False):
     c = pydec.zeros(size, c_num, dtype=torch.float)
     for i in range(c_num):
-        c[i] = torch.randn(size, requires_grad=requires_grad)
+        c()[i] = torch.randn(size, requires_grad=requires_grad)
     return c
 
 
 class TestIndexing:
     @classmethod
     def init_composition(cls) -> Composition:
         size = (3, 4)
         c = pydec.zeros(size, c_num=4)
         return c
 
     def test1(self):
         c = TestIndexing.init_composition()
+        c_ = c[None]
+        assert c_.numc() == c.numc()
+        assert c_.size() == (1,) + c.size()
+
+        c[None] = 1
+        assert torch.all(c._residual_tensor == 0)
+        assert torch.all(c._component_tensor == 1)
+
+    def test2(self):
+        c = TestIndexing.init_composition()
+        c0 = c[0]
+        assert isinstance(c0, Composition)
+        assert c0.numc() == c.numc()
+        assert c0.size() == c.size()[1:]
+        c02 = c[0:2]
+        assert isinstance(c02, Composition)
+        assert c02.numc() == c.numc()
+        assert c02.size() == (2,) + c.size()[1:]
+        c02_ = c[:, 0:2]
+        assert c02_.numc() == c.numc()
+        assert c02_.size() == c.size()[:1] + (2,)
+        c0202 = c[:2, :2]
+        assert c0202.numc() == c.numc()
+        assert c0202.size() == (2, 2)
+
+    def test3(self):
+        c = TestIndexing.init_composition()
+        c_ = c[:, None]
+        assert c_.size() == c.size()[:1] + (1,) + c.size()[1:]
+        index_list = [0, 2]
+        c_ = c[index_list]
+        assert isinstance(c_, Composition)
+        assert c_.numc() == c.numc()
+        assert c_.size() == (2,) + c.size()[1:]
+        c_ = c[index_list, index_list]
+        assert c_.c_size() == (c.numc(), 2)
+
+        with pytest.raises(IndexError):
+            c_ = c[index_list, index_list, index_list]
+
+        with pytest.raises(IndexError):
+            c_ = c[:, index_list, index_list]
+
+
+class TestIndexingWithSyntacticSugar:
+    def test1(self):
+        c = TestIndexing.init_composition()
         with pytest.raises(RuntimeError):
-            c[None]
+            c()[None]
         with pytest.raises(RuntimeError):
-            c[None] = 1
+            c()[None] = 1
 
     def test2(self):
         c = TestIndexing.init_composition()
-        c0 = c[0]
+        c0 = c()[0]
         assert isinstance(c0, torch.Tensor)
         assert c0.size() == c.size()
-        c02 = c[0:2]
+        c02 = c()[0:2]
         assert isinstance(c02, Composition)
         assert c02.numc() == 2
         assert c02.size() == c.size()
-        c02_ = c[:, 0:2]
+        c02_ = c()[:, 0:2]
         assert c02_.numc() == c.numc()
         assert c02_.size() == (2,) + c.size()[1:]
-        c0202 = c[:2, :2]
+        c0202 = c()[:2, :2]
         assert c0202.numc() == 2
         assert c0202.size() == (2,) + c.size()[1:]
 
     def test3(self):
         c = TestIndexing.init_composition()
-        c_ = c[:, None]
+        c_ = c()[:, None]
         assert c_.size() == (1,) + c.size()
         index_list = [0, 2]
-        c_ = c[index_list]
+        c_ = c()[index_list]
         assert isinstance(c_, Composition)
         assert c_.numc() == 2
         assert c_.size() == c.size()
-        c_ = c[index_list, index_list]
+        c_ = c()[index_list, index_list]
         assert c_.c_size() == (2,) + c.c_size()[2:]
 
-        c_ = c[index_list, index_list, index_list]
+        c_ = c()[index_list, index_list, index_list]
         assert c_.c_size() == (2,)
 
-        c_ = c[:, index_list, index_list]
+        c_ = c()[:, index_list, index_list]
         assert c_.c_size() == (4, 2)
 
 
-class TestIndexingInAutotracing:
-    @classmethod
-    def init_composition(cls) -> Composition:
-        size = (3, 4)
-        c = Composition(size, component_num=4)
-        return c
-
+class Test_C_AccessingIndexing:
+    @pydec.enable_c_accessing()
     def test1(self):
         c = TestIndexing.init_composition()
-        with pydec.autotracing.set_tracing_enabled(True):
-            c_ = c[None]
-            assert c_.numc() == c.numc()
-            assert c_.size() == (1,) + c.size()
-
+        with pytest.raises(RuntimeError):
+            c[None]
+        with pytest.raises(RuntimeError):
             c[None] = 1
-            assert torch.all(c._residual_tensor == 0)
-            assert torch.all(c._composition_tensor == 1)
 
+    @pydec.enable_c_accessing()
     def test2(self):
         c = TestIndexing.init_composition()
-        with pydec.autotracing.set_tracing_enabled(True):
-            c0 = c[0]
-            assert isinstance(c0, Composition)
-            assert c0.numc() == c.numc()
-            assert c0.size() == c.size()[1:]
-            c02 = c[0:2]
-            assert isinstance(c02, Composition)
-            assert c02.numc() == c.numc()
-            assert c02.size() == (2,) + c.size()[1:]
-            c02_ = c[:, 0:2]
-            assert c02_.numc() == c.numc()
-            assert c02_.size() == c.size()[:1] + (2,)
-            c0202 = c[:2, :2]
-            assert c0202.numc() == c.numc()
-            assert c0202.size() == (2, 2)
+        c0 = c[0]
+        assert isinstance(c0, torch.Tensor)
+        assert c0.size() == c.size()
+        c02 = c[0:2]
+        assert isinstance(c02, Composition)
+        assert c02.numc() == 2
+        assert c02.size() == c.size()
+        c02_ = c[:, 0:2]
+        assert c02_.numc() == c.numc()
+        assert c02_.size() == (2,) + c.size()[1:]
+        c0202 = c[:2, :2]
+        assert c0202.numc() == 2
+        assert c0202.size() == (2,) + c.size()[1:]
 
+    @pydec.enable_c_accessing()
     def test3(self):
         c = TestIndexing.init_composition()
-        with pydec.autotracing.set_tracing_enabled(True):
-            c_ = c[:, None]
-            assert c_.size() == c.size()[:1] + (1,) + c.size()[1:]
-            index_list = [0, 2]
-            c_ = c[index_list]
-            assert isinstance(c_, Composition)
-            assert c_.numc() == c.numc()
-            assert c_.size() == (2,) + c.size()[1:]
-            c_ = c[index_list, index_list]
-            assert c_.c_size() == (c.numc(), 2)
+        c_ = c[:, None]
+        assert c_.size() == (1,) + c.size()
+        index_list = [0, 2]
+        c_ = c[index_list]
+        assert isinstance(c_, Composition)
+        assert c_.numc() == 2
+        assert c_.size() == c.size()
+        c_ = c[index_list, index_list]
+        assert c_.c_size() == (2,) + c.c_size()[2:]
 
-            with pytest.raises(IndexError):
-                c_ = c[index_list, index_list, index_list]
+        c_ = c[index_list, index_list, index_list]
+        assert c_.c_size() == (2,)
 
-            with pytest.raises(IndexError):
-                c_ = c[:, index_list, index_list]
+        c_ = c[:, index_list, index_list]
+        assert c_.c_size() == (4, 2)
 
 
 class TestView:
     c = init_composition((2, 3))
 
     def test_view1(self):
-        assert self.c.view(torch.float16)._composition_tensor.dtype == torch.float16
+        assert self.c.view(torch.float16)._component_tensor.dtype == torch.float16
 
-        assert (
-            self.c.view(dtype=torch.float16)._composition_tensor.dtype == torch.float16
-        )
+        assert self.c.view(dtype=torch.float16)._component_tensor.dtype == torch.float16
 
     def test_view2(self):
         assert self.c.view((3, 2)).size() == (3, 2)
         assert self.c.view(size=(3, 2)).size() == (3, 2)
         assert self.c.view(3, 2).size() == (3, 2)
 
 
@@ -143,42 +178,41 @@
         assert self.c.reshape(3, 2).size() == (3, 2)
 
 
 class TestPlus:
     c = init_composition((2, 3))
 
     def test1(self):
-        from pydec import set_decomposition_func
+        from pydec import decOVF
 
         self.c[:] = 1.5
-        set_decomposition_func("abs_decomposition")
+        decOVF.set_decomposition_func("abs_affine")
         c = self.c + 3
         assert (self.c._residual_tensor + 3 == c._residual_tensor).all()
 
         # set_decomposition_func("norm_decomposition")
         # c = self.c + 3
         # assert (self.c._residual_tensor + 3 == c._residual_tensor).all()
 
-        set_decomposition_func("hybrid_decomposition")
+        decOVF.set_decomposition_func("hybrid_affine")
         c = self.c + 3
         assert (self.c._residual_tensor + 3 == c._residual_tensor).all()
 
         # set_decomposition_func("sign_decomposition")
         # c = self.c + 3
         # assert (self.c._residual_tensor + 3 == c._residual_tensor).all()
 
         # set_decomposition_func("hybrid_decomposition_threshold")
         # c = self.c + 3
         # assert (self.c._residual_tensor + 3 == c._residual_tensor).all()
 
-        with pydec.no_decomposition():
+        with decOVF.using_decomposition_func("none"):
             c = self.c + 3
-            assert (self.c._composition_tensor == c._composition_tensor).all()
+            assert (self.c._component_tensor == c._component_tensor).all()
             assert (self.c._residual_tensor + 3 == c._residual_tensor).all()
 
     def test2(self):
         c = init_composition((2, 3))
         out = c + self.c
         assert torch.all(
-            self.c._composition_tensor + c._composition_tensor
-            == out._composition_tensor
+            self.c._component_tensor + c._component_tensor == out._component_tensor
         )
```

### Comparing `pydec-0.2.0/test/test_decomposition.py` & `pydec-0.3.0/test/decomposition_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import pydec
-from .test_composition import init_composition
+from ._composition_test import init_composition
+from pydec import decOVF
 
 
 class TestBiasArgs:
     c = init_composition((2, 3))
 
     def test_set_args1(self):
         args = {"eps": 1e-2, "arg1": "foo"}
-        pydec.set_decomposition_args(**args)
-        bias_args = pydec.get_decomposition_args()
+        decOVF.set_decomposition_args(**args)
+        bias_args = decOVF.get_decomposition_args()
         for k, v in args.items():
             assert bias_args[k] == v
 
         args = {"eps": 1e-3, "arg2": None}
-        pydec.set_decomposition_args(**args)
-        bias_args = pydec.get_decomposition_args()
+        decOVF.set_decomposition_args(**args)
+        bias_args = decOVF.get_decomposition_args()
         assert bias_args["arg1"] == "foo"
         for k, v in args.items():
             assert bias_args[k] == v
 
     def test_set_args2(self):
         args = {"eps": 1e-2, "arg1": "foo"}
-        pydec.set_decomposition_args(update=False, **args)
-        bias_args = pydec.get_decomposition_args()
+        decOVF.set_decomposition_args(update=False, **args)
+        bias_args = decOVF.get_decomposition_args()
         assert len(bias_args) == len(args)
         for k, v in args.items():
             assert bias_args[k] == v
 
         args = {"eps": 1e-3, "arg2": None}
-        pydec.set_decomposition_args(update=False, **args)
-        bias_args = pydec.get_decomposition_args()
+        decOVF.set_decomposition_args(update=False, **args)
+        bias_args = decOVF.get_decomposition_args()
         assert len(bias_args) == len(args)
         for k, v in args.items():
             assert bias_args[k] == v
 
     def test_using_args1(self):
         args = {"threshold": 0.8}
-        pydec.set_decomposition_func("hybrid_decomposition")
-        assert "threshold" not in pydec.get_decomposition_args()
-        with pydec.using_decomposition_args(**args):
-            assert pydec.get_decomposition_args()["threshold"] == args["threshold"]
+        decOVF.set_decomposition_func("hybrid_affine")
+        assert "threshold" not in decOVF.get_decomposition_args()
+        with decOVF.using_decomposition_args(**args):
+            assert decOVF.get_decomposition_args()["threshold"] == args["threshold"]
             c = self.c + 3
 
-        assert "threshold" not in pydec.get_decomposition_args()
+        assert "threshold" not in decOVF.get_decomposition_args()
```

