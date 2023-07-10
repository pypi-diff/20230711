# Comparing `tmp/NeuralFoil-0.1.2.tar.gz` & `tmp/NeuralFoil-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralFoil-0.1.2.tar", last modified: Mon Jul 10 20:15:22 2023, max compression
+gzip compressed data, was "NeuralFoil-0.1.3.tar", last modified: Mon Jul 10 21:58:11 2023, max compression
```

## Comparing `NeuralFoil-0.1.2.tar` & `NeuralFoil-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:15:22.778305 NeuralFoil-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:15:22.766305 NeuralFoil-0.1.2/NeuralFoil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-07-10 20:15:22.000000 NeuralFoil-0.1.2/NeuralFoil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-10 20:15:22.000000 NeuralFoil-0.1.2/NeuralFoil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:15:22.000000 NeuralFoil-0.1.2/NeuralFoil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 20:15:22.000000 NeuralFoil-0.1.2/NeuralFoil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 20:15:22.000000 NeuralFoil-0.1.2/NeuralFoil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-07-10 20:15:22.774305 NeuralFoil-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19083 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:15:22.766305 NeuralFoil-0.1.2/neuralfoil/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/CL_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/neuralfoil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:15:22.770305 NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/
--rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-large.npz
--rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-medium.npz
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-small.npz
--rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
--rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
--rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:15:22.778305 NeuralFoil-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-10 20:15:10.000000 NeuralFoil-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:58:11.230127 NeuralFoil-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:58:11.226127 NeuralFoil-0.1.3/NeuralFoil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21446 2023-07-10 21:58:11.000000 NeuralFoil-0.1.3/NeuralFoil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-10 21:58:11.000000 NeuralFoil-0.1.3/NeuralFoil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:58:11.000000 NeuralFoil-0.1.3/NeuralFoil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 21:58:11.000000 NeuralFoil-0.1.3/NeuralFoil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 21:58:11.000000 NeuralFoil-0.1.3/NeuralFoil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21446 2023-07-10 21:58:11.230127 NeuralFoil-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:58:11.226127 NeuralFoil-0.1.3/neuralfoil/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/CL_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/neuralfoil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:58:11.226127 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/
+-rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-large.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-medium.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-small.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:58:11.230127 NeuralFoil-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/setup.py
```

### Comparing `NeuralFoil-0.1.2/LICENSE.txt` & `NeuralFoil-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/NeuralFoil.egg-info/PKG-INFO` & `NeuralFoil-0.1.3/NeuralFoil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.2
+Version: 0.1.3
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
@@ -29,15 +29,15 @@
 
 [![PyPI version](https://badge.fury.io/py/NeuralFoil.svg)](https://badge.fury.io/py/NeuralFoil)
 [![Build Status](https://github.com/peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/licenses/MIT)
 
 -----
 
-NeuralFoil is a small Python/NumPy tool for rapid aerodynamics analysis of airfoils. It is also a small subset of the larger [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here as a standalone. Under the hood, NeuralFoil consists of physics-informed neural networks trained on tens of millions of [XFoil](https://web.mit.edu/drela/Public/web/xfoil/) runs. NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient code-base](./neuralfoil).
+NeuralFoil is a small Python/NumPy tool for rapid aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/). It is also a small subset of the larger [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here as a standalone. Under the hood, NeuralFoil consists of physics-informed neural networks trained on [tens of millions of XFoil runs](#geometry-parameterization-and-training-data). NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient code-base](./neuralfoil).
 
 NeuralFoil is ~10x faster than XFoil for a single analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in accuracy compared to XFoil](#performance). It also has [many nice features](#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/NumPy) that make it much easier to use.
 
 ## Overview
 
 NeuralFoil comes with 8 different neural network models, with increasing levels of complexity:
 
@@ -85,34 +85,38 @@
 )
 
 # `aero` is a dict with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
 ```
 
 ## Performance
 
-Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L$-$C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a real-world aircraft development program and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
+Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
 
+<a name="clcd-polar"></a>
 <p align="center">
 	<img src="./benchmarking/neuralfoil_point_validation.svg" width="1000" />
 </p>
 
-NeuralFoil is typically accurate to within a few percent of XFoil's predictions. The error is largest at transitional $Re$ where the physics is the most nuanced, but is still quite close. NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ in the $Re=\mathrm{1M}$ case, where the bottom-surface boundary layer suddenly laminarizes, and the drag plummets), which would otherwise make optimization difficult. 
+NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the UIUC-database training set will have even more accurate results. 
+
+NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is obviously incorrect, which would otherwise make optimization difficult. 
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
 
 This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild".
 
-<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>18 ms</td><td>0.020 s</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>27 ms</td><td>0.204 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>29 ms</td><td>0.304 s</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>31 ms</td><td>0.437 s</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>33 ms</td><td>0.749 s</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>35 ms</td><td>1.542 s</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>36 ms</td><td>3.495 s</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>39 ms</td><td>4.557 s</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>65 ms</td><td>11.633 s</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>447 ms</td><td>3610 sec</td></tr></tbody></table>
-
-† The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.051, you can think of it as "typically, drag is accurate to within roughly 5.1%".
+<a name="table"></a>
+<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>18 ms</td><td>0.020 s</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>27 ms</td><td>0.204 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>29 ms</td><td>0.304 s</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>31 ms</td><td>0.437 s</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>33 ms</td><td>0.749 s</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>35 ms</td><td>1.542 s</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>36 ms</td><td>3.495 s</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>39 ms</td><td>4.557 s</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>65 ms</td><td>11.633 s</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>447 ms</td><td>3610 sec</td></tr></tbody></table>
 
-‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
+> † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may be better than the numbers in this table.
+> 
+> ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
 
 Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
 Notably, most of the computational overhead of calling NeuralFoil is actually in the airfoil preprocessing step, where the airfoil is converted from a set of coordinates to a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-and-training-data)) - not in the aerodynamics analysis itself. This pre-processing takes around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://github.com/peterdsharpe/AeroSandbox/blob/c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/airfoil_families.py#L265), but in theory a pure-NumPy implementation is possible that would be much faster by exploiting linearity (sub-millisecond). If you're interested in working on this, open an issue and let me know! In the meantime, you can eliminate this overhead by using [`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to one of NeuralFoil's other functions.
 
@@ -129,14 +133,22 @@
 * [NumPy](https://numpy.org/)
 * [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) 4.0.10+
 
 Currently, NeuralFoil only uses AeroSandbox for airfoil geometry parameterization (i.e., converting from a set of points to a CST parameterization, which is solved as an optimization problem)—the actual math is implemented in pure NumPy. Recent progress on this CST parameterization-fitting problem has allowed it to be recast as a least-squares problem, which is potentially amenable to a pure-NumPy implementation. That being said, AeroSandbox provides a bunch of nice peripheral utilities (e.g., geometry manipulation, visualization, etc.), so it's a nice dependency to have anyway. However, if you'd like to work on a pure-NumPy implementation, open an issue and let me know!
 
 ## Geometry Parameterization and Training Data
 
+#### Geometry Parameterization
+
+To be written, but it's basically an 8-parameter-per-side CST (Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM) and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18 parameters to describe a given airfoil shape. I'll write more here, but in the meantime read:
+- [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
+- The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
+
+#### Training Data
+
 To be written, but in the meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes. Contact me if you need it sooner.
 
 ## FAQs
 
 Will NeuralFoil be integrated directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)?
 
 > Yes, absolutely. However, the goal is to keep this NeuralFoil repository also available as a stand-alone module, if desired. This simplifies dependencies for people using NeuralFoil in other applications (e.g., flight simulation, real-time control on embedded systems, etc.), and makes it easier if someone wanted to port NeuralFoil to another language (e.g., C++, for use on an Arduino).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.2 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.3 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
@@ -16,21 +16,22 @@
 by [Peter Sharpe](https://peterdsharpe.github.io) (
 at] mit [dot] edu>) [![PyPI version](https://badge.fury.io/py/NeuralFoil.svg)]
 (https://badge.fury.io/py/NeuralFoil) [![Build Status](https://github.com/
 peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/
 peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/
 licenses/MIT) ----- NeuralFoil is a small Python/NumPy tool for rapid
-aerodynamics analysis of airfoils. It is also a small subset of the larger
-[AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is
-offered here as a standalone. Under the hood, NeuralFoil consists of physics-
-informed neural networks trained on tens of millions of [XFoil](https://
-web.mit.edu/drela/Public/web/xfoil/) runs. NeuralFoil aims to be lightweight,
-with [minimal dependencies](#dependencies-question) and a [tight, efficient
-code-base](./neuralfoil). NeuralFoil is ~10x faster than XFoil for a single
+aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/
+drela/Public/web/xfoil/). It is also a small subset of the larger [AeroSandbox]
+(https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here
+as a standalone. Under the hood, NeuralFoil consists of physics-informed neural
+networks trained on [tens of millions of XFoil runs](#geometry-
+parameterization-and-training-data). NeuralFoil aims to be lightweight, with
+[minimal dependencies](#dependencies-question) and a [tight, efficient code-
+base](./neuralfoil). NeuralFoil is ~10x faster than XFoil for a single
 analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in
 accuracy compared to XFoil](#performance). It also has [many nice features]
 (#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/
 NumPy) that make it much easier to use. ## Overview NeuralFoil comes with 8
 different neural network models, with increasing levels of complexity:
    "xxsmall" "xsmall" "small" "medium" "large" "xlarge" "xxlarge" "xxxlarge"
 This spectrum offers a tradeoff between accuracy and computational cost. In
@@ -51,38 +52,39 @@
 25, 1000), # Vectorize your evaluations across `alpha` and `Re` Re=5e6, ) aero
 = nf.get_aero_from_airfoil( # You can AeroSandbox airfoils as an entry point
 airfoil=asb.Airfoil("naca4412"), # `import aerosandbox as asb`, any UIUC or
 NACA airfoil name works alpha=5, Re=5e6, ) # `aero` is a dict with keys: ["CL",
 "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"] ``` ## Performance Qualitatively,
 NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$
 values. In the figure below, we compare the performance of NeuralFoil to XFoil
-on $C_L$-$C_D$ polar prediction. Notably, the airfoil analyzed here was
-developed "from scratch" for a real-world aircraft development program and is
-completely separate from [the airfoils used during NeuralFoil's training]
-(#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by
-"memorizing" this airfoil's performance:
+on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was
+developed "from scratch" for a [real-world aircraft development program](https:
+//www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-
+research-aircraft-301633713.html) and is completely separate from [the airfoils
+used during NeuralFoil's training](#geometry-parameterization-and-training-
+data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance:
                [./benchmarking/neuralfoil_point_validation.svg]
 NeuralFoil is typically accurate to within a few percent of XFoil's
-predictions. The error is largest at transitional $Re$ where the physics is the
-most nuanced, but is still quite close. NeuralFoil also [has the benefit of
-smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for
-example, near $C_L=0.75$ in the $Re=\mathrm{1M}$ case, where the bottom-surface
-boundary layer suddenly laminarizes, and the drag plummets), which would
-otherwise make optimization difficult. In the table below, we quantify the
-performance of the NeuralFoil ("NF") models with respect to XFoil more
-precisely. At a basic level, we care about two things: - **Accuracy**: how
-close are the predictions to XFoil's? - **Computational Cost**: how long does
-it take to run? This table details both of these considerations. The first few
-columns show the error with respect to XFoil on the test dataset. [The test
-dataset is completely isolated from the training dataset, and NeuralFoil was
-not allowed to learn from the test dataset](#geometry-parameterization-and-
-training-data). Thus, the performance on the test dataset gives a good idea of
-NeuralFoil's performance "in the wild".
-Aerodynamics Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to   Computational
-Model        XFoil                                                                             Cost to Run
+predictions. Note that this figure is on a truly out-of-sample airfoil, so
+airfoils that are closer to the UIUC-database training set will have even more
+accurate results. NeuralFoil also [has the benefit of smoothing out XFoil's
+"jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at
+$Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is
+obviously incorrect, which would otherwise make optimization difficult. In the
+table below, we quantify the performance of the NeuralFoil ("NF") models with
+respect to XFoil more precisely. At a basic level, we care about two things: -
+**Accuracy**: how close are the predictions to XFoil's? - **Computational
+Cost**: how long does it take to run? This table details both of these
+considerations. The first few columns show the error with respect to XFoil on
+the test dataset. [The test dataset is completely isolated from the training
+dataset, and NeuralFoil was not allowed to learn from the test dataset]
+(#geometry-parameterization-and-training-data). Thus, the performance on the
+test dataset gives a good idea of NeuralFoil's performance "in the wild".
+Aerodynamics Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset,  Computational
+Model        with respect to XFoil                                                             Cost to Run
                                                                                         Bottom
                                                                              Top        Trans.         Total
              Lift   Fractional Drag   Moment Max Overspeed                   Transition Loc.   Runtime Runtime
              Coeff. Coeff.            Coeff. $u_\max / u_\infty$   â¡ Loc.       $x_    (1 run) (100,000
              $C_L$  $\ln(C_D)$ â  $C_M$                                  $x_{tr,    {tr,           runs)
                                                                              top}/c$    bot}/
                                                                                         c$
@@ -95,31 +97,35 @@
 NF "medium"  0.027  0.051             0.004  0.088                           0.022      0.033  33 ms   0.749 s
 NF "large"   0.024  0.045             0.004  0.079                           0.020      0.029  35 ms   1.542 s
 NF "xlarge"  0.023  0.043             0.004  0.076                           0.019      0.028  36 ms   3.495 s
 NF "xxlarge" 0.021  0.040             0.003  0.071                           0.018      0.025  39 ms   4.557 s
 NF           0.020  0.039             0.003  0.070                           0.016      0.024  65 ms   11.633 s
 "xxxlarge"
 XFoil        0      0                 0      0                               0          0      447 ms  3610 sec
-â  The deviation of $\ln(C_D)$ can be thought of as "the typical relative
+> â  The deviation of $\ln(C_D)$ can be thought of as "the typical relative
 error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm)
-of $\ln(C_D)$ is 0.051, you can think of it as "typically, drag is accurate to
-within roughly 5.1%". â¡ This "maximum overspeed" lets you compute $C_
-{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm
-{crit}$. [More details below.](#compressibility-question) Based on these
-performance numbers, you can select the right tradeoff between accuracy and
-computational cost for your application. In general, I recommend starting with
-the "large" model and adjusting from there. In addition to accuracy vs. speed,
-another consideration when choosing the right model is what you're trying to
-use NeuralFoil for. Larger models will be more complicated ("less
-parsimonious," as the math kids would say), which means that they may have more
-"wiggles" in their outputsâthis might be undesirable for gradient-based
-optimization. On the other hand, larger models will be able to capture a wider
-range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be
-seen mid-optimization), so larger models could have a benefit in that sense. If
-you try a specific application and have better/worse results with a specific
+of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to
+within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil
+is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly
+not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure
+above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may
+be better than the numbers in this table. > > â¡ This "maximum overspeed" lets
+you compute $C_{p,\min}$, which can be used to calculate the critical Mach
+number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
+Based on these performance numbers, you can select the right tradeoff between
+accuracy and computational cost for your application. In general, I recommend
+starting with the "large" model and adjusting from there. In addition to
+accuracy vs. speed, another consideration when choosing the right model is what
+you're trying to use NeuralFoil for. Larger models will be more complicated
+("less parsimonious," as the math kids would say), which means that they may
+have more "wiggles" in their outputsâthis might be undesirable for gradient-
+based optimization. On the other hand, larger models will be able to capture a
+wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might
+be seen mid-optimization), so larger models could have a benefit in that sense.
+If you try a specific application and have better/worse results with a specific
 model, let me know by opening a GitHub issue! Notably, most of the
 computational overhead of calling NeuralFoil is actually in the airfoil
 preprocessing step, where the airfoil is converted from a set of coordinates to
 a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-
 and-training-data)) - not in the aerodynamics analysis itself. This pre-
 processing takes around 20 milliseconds using [AeroSandbox's general nonlinear
 solvers](https://github.com/peterdsharpe/AeroSandbox/blob/
@@ -138,26 +144,35 @@
 parameterization, which is solved as an optimization problem)âthe actual math
 is implemented in pure NumPy. Recent progress on this CST parameterization-
 fitting problem has allowed it to be recast as a least-squares problem, which
 is potentially amenable to a pure-NumPy implementation. That being said,
 AeroSandbox provides a bunch of nice peripheral utilities (e.g., geometry
 manipulation, visualization, etc.), so it's a nice dependency to have anyway.
 However, if you'd like to work on a pure-NumPy implementation, open an issue
-and let me know! ## Geometry Parameterization and Training Data To be written,
-but in the meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/
-master/training_data). Training data is not (yet) uploaded to GitHub, but will
-be soon - need to figure out Git LFS, as it's many gigabytes. Contact me if you
-need it sooner. ## FAQs Will NeuralFoil be integrated directly into
-[AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)? > Yes, absolutely.
-However, the goal is to keep this NeuralFoil repository also available as a
-stand-alone module, if desired. This simplifies dependencies for people using
-NeuralFoil in other applications (e.g., flight simulation, real-time control on
-embedded systems, etc.), and makes it easier if someone wanted to port
-NeuralFoil to another language (e.g., C++, for use on an Arduino).  Why not
-just use XFoil directly? > XFoil is a truly excellent piece of aerospace
+and let me know! ## Geometry Parameterization and Training Data #### Geometry
+Parameterization To be written, but it's basically an 8-parameter-per-side CST
+(Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM)
+and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) =
+18 parameters to describe a given airfoil shape. I'll write more here, but in
+the meantime read: - [D. A. Masters, "Geometric Comparison of Aerofoil Shape
+Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/
+10.2514/1.J054943) - The seminal paper on the CST (Kulfan) parameterization
+technique: [Brenda Kulfan, "Universal Parametric Geometry Representation
+Method"](http://mx1.brendakulfan.com/docs/CST6.pdf) #### Training Data To be
+written, but in the meantime [see here](https://github.com/peterdsharpe/
+NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to
+GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes.
+Contact me if you need it sooner. ## FAQs Will NeuralFoil be integrated
+directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)? >
+Yes, absolutely. However, the goal is to keep this NeuralFoil repository also
+available as a stand-alone module, if desired. This simplifies dependencies for
+people using NeuralFoil in other applications (e.g., flight simulation, real-
+time control on embedded systems, etc.), and makes it easier if someone wanted
+to port NeuralFoil to another language (e.g., C++, for use on an Arduino).  Why
+not just use XFoil directly? > XFoil is a truly excellent piece of aerospace
 software engineering and is the gold standard of airfoil analysis, for good
 reason. When its assumptions hold (airfoils in subsonic flow without massive
 separation), its accuracy exceeds that of RANS CFD, yet it has ~1000x lower
 computational cost. XFoil shines in particular for human-in-the-loop airfoil
 design. However, XFoil is not the right tool for all applications, for a few
 reasons: > > - XFoil exhibits hysteresis: you can get slightly different
 solutions (for the same airfoil, $\alpha$, and $Re$) depending on whether you
```

### Comparing `NeuralFoil-0.1.2/NeuralFoil.egg-info/SOURCES.txt` & `NeuralFoil-0.1.3/NeuralFoil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/PKG-INFO` & `NeuralFoil-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.2
+Version: 0.1.3
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
@@ -29,15 +29,15 @@
 
 [![PyPI version](https://badge.fury.io/py/NeuralFoil.svg)](https://badge.fury.io/py/NeuralFoil)
 [![Build Status](https://github.com/peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/licenses/MIT)
 
 -----
 
-NeuralFoil is a small Python/NumPy tool for rapid aerodynamics analysis of airfoils. It is also a small subset of the larger [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here as a standalone. Under the hood, NeuralFoil consists of physics-informed neural networks trained on tens of millions of [XFoil](https://web.mit.edu/drela/Public/web/xfoil/) runs. NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient code-base](./neuralfoil).
+NeuralFoil is a small Python/NumPy tool for rapid aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/). It is also a small subset of the larger [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here as a standalone. Under the hood, NeuralFoil consists of physics-informed neural networks trained on [tens of millions of XFoil runs](#geometry-parameterization-and-training-data). NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient code-base](./neuralfoil).
 
 NeuralFoil is ~10x faster than XFoil for a single analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in accuracy compared to XFoil](#performance). It also has [many nice features](#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/NumPy) that make it much easier to use.
 
 ## Overview
 
 NeuralFoil comes with 8 different neural network models, with increasing levels of complexity:
 
@@ -85,34 +85,38 @@
 )
 
 # `aero` is a dict with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
 ```
 
 ## Performance
 
-Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L$-$C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a real-world aircraft development program and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
+Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
 
+<a name="clcd-polar"></a>
 <p align="center">
 	<img src="./benchmarking/neuralfoil_point_validation.svg" width="1000" />
 </p>
 
-NeuralFoil is typically accurate to within a few percent of XFoil's predictions. The error is largest at transitional $Re$ where the physics is the most nuanced, but is still quite close. NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ in the $Re=\mathrm{1M}$ case, where the bottom-surface boundary layer suddenly laminarizes, and the drag plummets), which would otherwise make optimization difficult. 
+NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the UIUC-database training set will have even more accurate results. 
+
+NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is obviously incorrect, which would otherwise make optimization difficult. 
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
 
 This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild".
 
-<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>18 ms</td><td>0.020 s</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>27 ms</td><td>0.204 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>29 ms</td><td>0.304 s</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>31 ms</td><td>0.437 s</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>33 ms</td><td>0.749 s</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>35 ms</td><td>1.542 s</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>36 ms</td><td>3.495 s</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>39 ms</td><td>4.557 s</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>65 ms</td><td>11.633 s</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>447 ms</td><td>3610 sec</td></tr></tbody></table>
-
-† The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.051, you can think of it as "typically, drag is accurate to within roughly 5.1%".
+<a name="table"></a>
+<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>18 ms</td><td>0.020 s</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>27 ms</td><td>0.204 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>29 ms</td><td>0.304 s</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>31 ms</td><td>0.437 s</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>33 ms</td><td>0.749 s</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>35 ms</td><td>1.542 s</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>36 ms</td><td>3.495 s</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>39 ms</td><td>4.557 s</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>65 ms</td><td>11.633 s</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>447 ms</td><td>3610 sec</td></tr></tbody></table>
 
-‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
+> † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may be better than the numbers in this table.
+> 
+> ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
 
 Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
 Notably, most of the computational overhead of calling NeuralFoil is actually in the airfoil preprocessing step, where the airfoil is converted from a set of coordinates to a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-and-training-data)) - not in the aerodynamics analysis itself. This pre-processing takes around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://github.com/peterdsharpe/AeroSandbox/blob/c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/airfoil_families.py#L265), but in theory a pure-NumPy implementation is possible that would be much faster by exploiting linearity (sub-millisecond). If you're interested in working on this, open an issue and let me know! In the meantime, you can eliminate this overhead by using [`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to one of NeuralFoil's other functions.
 
@@ -129,14 +133,22 @@
 * [NumPy](https://numpy.org/)
 * [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) 4.0.10+
 
 Currently, NeuralFoil only uses AeroSandbox for airfoil geometry parameterization (i.e., converting from a set of points to a CST parameterization, which is solved as an optimization problem)—the actual math is implemented in pure NumPy. Recent progress on this CST parameterization-fitting problem has allowed it to be recast as a least-squares problem, which is potentially amenable to a pure-NumPy implementation. That being said, AeroSandbox provides a bunch of nice peripheral utilities (e.g., geometry manipulation, visualization, etc.), so it's a nice dependency to have anyway. However, if you'd like to work on a pure-NumPy implementation, open an issue and let me know!
 
 ## Geometry Parameterization and Training Data
 
+#### Geometry Parameterization
+
+To be written, but it's basically an 8-parameter-per-side CST (Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM) and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18 parameters to describe a given airfoil shape. I'll write more here, but in the meantime read:
+- [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
+- The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
+
+#### Training Data
+
 To be written, but in the meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes. Contact me if you need it sooner.
 
 ## FAQs
 
 Will NeuralFoil be integrated directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)?
 
 > Yes, absolutely. However, the goal is to keep this NeuralFoil repository also available as a stand-alone module, if desired. This simplifies dependencies for people using NeuralFoil in other applications (e.g., flight simulation, real-time control on embedded systems, etc.), and makes it easier if someone wanted to port NeuralFoil to another language (e.g., C++, for use on an Arduino).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.2 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.3 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
@@ -16,21 +16,22 @@
 by [Peter Sharpe](https://peterdsharpe.github.io) (
 at] mit [dot] edu>) [![PyPI version](https://badge.fury.io/py/NeuralFoil.svg)]
 (https://badge.fury.io/py/NeuralFoil) [![Build Status](https://github.com/
 peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/
 peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/
 licenses/MIT) ----- NeuralFoil is a small Python/NumPy tool for rapid
-aerodynamics analysis of airfoils. It is also a small subset of the larger
-[AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is
-offered here as a standalone. Under the hood, NeuralFoil consists of physics-
-informed neural networks trained on tens of millions of [XFoil](https://
-web.mit.edu/drela/Public/web/xfoil/) runs. NeuralFoil aims to be lightweight,
-with [minimal dependencies](#dependencies-question) and a [tight, efficient
-code-base](./neuralfoil). NeuralFoil is ~10x faster than XFoil for a single
+aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/
+drela/Public/web/xfoil/). It is also a small subset of the larger [AeroSandbox]
+(https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here
+as a standalone. Under the hood, NeuralFoil consists of physics-informed neural
+networks trained on [tens of millions of XFoil runs](#geometry-
+parameterization-and-training-data). NeuralFoil aims to be lightweight, with
+[minimal dependencies](#dependencies-question) and a [tight, efficient code-
+base](./neuralfoil). NeuralFoil is ~10x faster than XFoil for a single
 analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in
 accuracy compared to XFoil](#performance). It also has [many nice features]
 (#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/
 NumPy) that make it much easier to use. ## Overview NeuralFoil comes with 8
 different neural network models, with increasing levels of complexity:
    "xxsmall" "xsmall" "small" "medium" "large" "xlarge" "xxlarge" "xxxlarge"
 This spectrum offers a tradeoff between accuracy and computational cost. In
@@ -51,38 +52,39 @@
 25, 1000), # Vectorize your evaluations across `alpha` and `Re` Re=5e6, ) aero
 = nf.get_aero_from_airfoil( # You can AeroSandbox airfoils as an entry point
 airfoil=asb.Airfoil("naca4412"), # `import aerosandbox as asb`, any UIUC or
 NACA airfoil name works alpha=5, Re=5e6, ) # `aero` is a dict with keys: ["CL",
 "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"] ``` ## Performance Qualitatively,
 NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$
 values. In the figure below, we compare the performance of NeuralFoil to XFoil
-on $C_L$-$C_D$ polar prediction. Notably, the airfoil analyzed here was
-developed "from scratch" for a real-world aircraft development program and is
-completely separate from [the airfoils used during NeuralFoil's training]
-(#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by
-"memorizing" this airfoil's performance:
+on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was
+developed "from scratch" for a [real-world aircraft development program](https:
+//www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-
+research-aircraft-301633713.html) and is completely separate from [the airfoils
+used during NeuralFoil's training](#geometry-parameterization-and-training-
+data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance:
                [./benchmarking/neuralfoil_point_validation.svg]
 NeuralFoil is typically accurate to within a few percent of XFoil's
-predictions. The error is largest at transitional $Re$ where the physics is the
-most nuanced, but is still quite close. NeuralFoil also [has the benefit of
-smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for
-example, near $C_L=0.75$ in the $Re=\mathrm{1M}$ case, where the bottom-surface
-boundary layer suddenly laminarizes, and the drag plummets), which would
-otherwise make optimization difficult. In the table below, we quantify the
-performance of the NeuralFoil ("NF") models with respect to XFoil more
-precisely. At a basic level, we care about two things: - **Accuracy**: how
-close are the predictions to XFoil's? - **Computational Cost**: how long does
-it take to run? This table details both of these considerations. The first few
-columns show the error with respect to XFoil on the test dataset. [The test
-dataset is completely isolated from the training dataset, and NeuralFoil was
-not allowed to learn from the test dataset](#geometry-parameterization-and-
-training-data). Thus, the performance on the test dataset gives a good idea of
-NeuralFoil's performance "in the wild".
-Aerodynamics Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to   Computational
-Model        XFoil                                                                             Cost to Run
+predictions. Note that this figure is on a truly out-of-sample airfoil, so
+airfoils that are closer to the UIUC-database training set will have even more
+accurate results. NeuralFoil also [has the benefit of smoothing out XFoil's
+"jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at
+$Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is
+obviously incorrect, which would otherwise make optimization difficult. In the
+table below, we quantify the performance of the NeuralFoil ("NF") models with
+respect to XFoil more precisely. At a basic level, we care about two things: -
+**Accuracy**: how close are the predictions to XFoil's? - **Computational
+Cost**: how long does it take to run? This table details both of these
+considerations. The first few columns show the error with respect to XFoil on
+the test dataset. [The test dataset is completely isolated from the training
+dataset, and NeuralFoil was not allowed to learn from the test dataset]
+(#geometry-parameterization-and-training-data). Thus, the performance on the
+test dataset gives a good idea of NeuralFoil's performance "in the wild".
+Aerodynamics Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset,  Computational
+Model        with respect to XFoil                                                             Cost to Run
                                                                                         Bottom
                                                                              Top        Trans.         Total
              Lift   Fractional Drag   Moment Max Overspeed                   Transition Loc.   Runtime Runtime
              Coeff. Coeff.            Coeff. $u_\max / u_\infty$   â¡ Loc.       $x_    (1 run) (100,000
              $C_L$  $\ln(C_D)$ â  $C_M$                                  $x_{tr,    {tr,           runs)
                                                                              top}/c$    bot}/
                                                                                         c$
@@ -95,31 +97,35 @@
 NF "medium"  0.027  0.051             0.004  0.088                           0.022      0.033  33 ms   0.749 s
 NF "large"   0.024  0.045             0.004  0.079                           0.020      0.029  35 ms   1.542 s
 NF "xlarge"  0.023  0.043             0.004  0.076                           0.019      0.028  36 ms   3.495 s
 NF "xxlarge" 0.021  0.040             0.003  0.071                           0.018      0.025  39 ms   4.557 s
 NF           0.020  0.039             0.003  0.070                           0.016      0.024  65 ms   11.633 s
 "xxxlarge"
 XFoil        0      0                 0      0                               0          0      447 ms  3610 sec
-â  The deviation of $\ln(C_D)$ can be thought of as "the typical relative
+> â  The deviation of $\ln(C_D)$ can be thought of as "the typical relative
 error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm)
-of $\ln(C_D)$ is 0.051, you can think of it as "typically, drag is accurate to
-within roughly 5.1%". â¡ This "maximum overspeed" lets you compute $C_
-{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm
-{crit}$. [More details below.](#compressibility-question) Based on these
-performance numbers, you can select the right tradeoff between accuracy and
-computational cost for your application. In general, I recommend starting with
-the "large" model and adjusting from there. In addition to accuracy vs. speed,
-another consideration when choosing the right model is what you're trying to
-use NeuralFoil for. Larger models will be more complicated ("less
-parsimonious," as the math kids would say), which means that they may have more
-"wiggles" in their outputsâthis might be undesirable for gradient-based
-optimization. On the other hand, larger models will be able to capture a wider
-range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be
-seen mid-optimization), so larger models could have a benefit in that sense. If
-you try a specific application and have better/worse results with a specific
+of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to
+within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil
+is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly
+not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure
+above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may
+be better than the numbers in this table. > > â¡ This "maximum overspeed" lets
+you compute $C_{p,\min}$, which can be used to calculate the critical Mach
+number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
+Based on these performance numbers, you can select the right tradeoff between
+accuracy and computational cost for your application. In general, I recommend
+starting with the "large" model and adjusting from there. In addition to
+accuracy vs. speed, another consideration when choosing the right model is what
+you're trying to use NeuralFoil for. Larger models will be more complicated
+("less parsimonious," as the math kids would say), which means that they may
+have more "wiggles" in their outputsâthis might be undesirable for gradient-
+based optimization. On the other hand, larger models will be able to capture a
+wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might
+be seen mid-optimization), so larger models could have a benefit in that sense.
+If you try a specific application and have better/worse results with a specific
 model, let me know by opening a GitHub issue! Notably, most of the
 computational overhead of calling NeuralFoil is actually in the airfoil
 preprocessing step, where the airfoil is converted from a set of coordinates to
 a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-
 and-training-data)) - not in the aerodynamics analysis itself. This pre-
 processing takes around 20 milliseconds using [AeroSandbox's general nonlinear
 solvers](https://github.com/peterdsharpe/AeroSandbox/blob/
@@ -138,26 +144,35 @@
 parameterization, which is solved as an optimization problem)âthe actual math
 is implemented in pure NumPy. Recent progress on this CST parameterization-
 fitting problem has allowed it to be recast as a least-squares problem, which
 is potentially amenable to a pure-NumPy implementation. That being said,
 AeroSandbox provides a bunch of nice peripheral utilities (e.g., geometry
 manipulation, visualization, etc.), so it's a nice dependency to have anyway.
 However, if you'd like to work on a pure-NumPy implementation, open an issue
-and let me know! ## Geometry Parameterization and Training Data To be written,
-but in the meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/
-master/training_data). Training data is not (yet) uploaded to GitHub, but will
-be soon - need to figure out Git LFS, as it's many gigabytes. Contact me if you
-need it sooner. ## FAQs Will NeuralFoil be integrated directly into
-[AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)? > Yes, absolutely.
-However, the goal is to keep this NeuralFoil repository also available as a
-stand-alone module, if desired. This simplifies dependencies for people using
-NeuralFoil in other applications (e.g., flight simulation, real-time control on
-embedded systems, etc.), and makes it easier if someone wanted to port
-NeuralFoil to another language (e.g., C++, for use on an Arduino).  Why not
-just use XFoil directly? > XFoil is a truly excellent piece of aerospace
+and let me know! ## Geometry Parameterization and Training Data #### Geometry
+Parameterization To be written, but it's basically an 8-parameter-per-side CST
+(Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM)
+and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) =
+18 parameters to describe a given airfoil shape. I'll write more here, but in
+the meantime read: - [D. A. Masters, "Geometric Comparison of Aerofoil Shape
+Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/
+10.2514/1.J054943) - The seminal paper on the CST (Kulfan) parameterization
+technique: [Brenda Kulfan, "Universal Parametric Geometry Representation
+Method"](http://mx1.brendakulfan.com/docs/CST6.pdf) #### Training Data To be
+written, but in the meantime [see here](https://github.com/peterdsharpe/
+NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to
+GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes.
+Contact me if you need it sooner. ## FAQs Will NeuralFoil be integrated
+directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)? >
+Yes, absolutely. However, the goal is to keep this NeuralFoil repository also
+available as a stand-alone module, if desired. This simplifies dependencies for
+people using NeuralFoil in other applications (e.g., flight simulation, real-
+time control on embedded systems, etc.), and makes it easier if someone wanted
+to port NeuralFoil to another language (e.g., C++, for use on an Arduino).  Why
+not just use XFoil directly? > XFoil is a truly excellent piece of aerospace
 software engineering and is the gold standard of airfoil analysis, for good
 reason. When its assumptions hold (airfoils in subsonic flow without massive
 separation), its accuracy exceeds that of RANS CFD, yet it has ~1000x lower
 computational cost. XFoil shines in particular for human-in-the-loop airfoil
 design. However, XFoil is not the right tool for all applications, for a few
 reasons: > > - XFoil exhibits hysteresis: you can get slightly different
 solutions (for the same airfoil, $\alpha$, and $Re$) depending on whether you
```

### Comparing `NeuralFoil-0.1.2/README.md` & `NeuralFoil-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [![PyPI version](https://badge.fury.io/py/NeuralFoil.svg)](https://badge.fury.io/py/NeuralFoil)
 [![Build Status](https://github.com/peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/licenses/MIT)
 
 -----
 
-NeuralFoil is a small Python/NumPy tool for rapid aerodynamics analysis of airfoils. It is also a small subset of the larger [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here as a standalone. Under the hood, NeuralFoil consists of physics-informed neural networks trained on tens of millions of [XFoil](https://web.mit.edu/drela/Public/web/xfoil/) runs. NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient code-base](./neuralfoil).
+NeuralFoil is a small Python/NumPy tool for rapid aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/). It is also a small subset of the larger [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here as a standalone. Under the hood, NeuralFoil consists of physics-informed neural networks trained on [tens of millions of XFoil runs](#geometry-parameterization-and-training-data). NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient code-base](./neuralfoil).
 
 NeuralFoil is ~10x faster than XFoil for a single analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in accuracy compared to XFoil](#performance). It also has [many nice features](#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/NumPy) that make it much easier to use.
 
 ## Overview
 
 NeuralFoil comes with 8 different neural network models, with increasing levels of complexity:
 
@@ -63,34 +63,38 @@
 )
 
 # `aero` is a dict with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
 ```
 
 ## Performance
 
-Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L$-$C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a real-world aircraft development program and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
+Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
 
+<a name="clcd-polar"></a>
 <p align="center">
 	<img src="./benchmarking/neuralfoil_point_validation.svg" width="1000" />
 </p>
 
-NeuralFoil is typically accurate to within a few percent of XFoil's predictions. The error is largest at transitional $Re$ where the physics is the most nuanced, but is still quite close. NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ in the $Re=\mathrm{1M}$ case, where the bottom-surface boundary layer suddenly laminarizes, and the drag plummets), which would otherwise make optimization difficult. 
+NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the UIUC-database training set will have even more accurate results. 
+
+NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is obviously incorrect, which would otherwise make optimization difficult. 
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
 
 This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild".
 
-<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>18 ms</td><td>0.020 s</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>27 ms</td><td>0.204 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>29 ms</td><td>0.304 s</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>31 ms</td><td>0.437 s</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>33 ms</td><td>0.749 s</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>35 ms</td><td>1.542 s</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>36 ms</td><td>3.495 s</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>39 ms</td><td>4.557 s</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>65 ms</td><td>11.633 s</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>447 ms</td><td>3610 sec</td></tr></tbody></table>
-
-† The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.051, you can think of it as "typically, drag is accurate to within roughly 5.1%".
+<a name="table"></a>
+<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>18 ms</td><td>0.020 s</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>27 ms</td><td>0.204 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>29 ms</td><td>0.304 s</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>31 ms</td><td>0.437 s</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>33 ms</td><td>0.749 s</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>35 ms</td><td>1.542 s</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>36 ms</td><td>3.495 s</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>39 ms</td><td>4.557 s</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>65 ms</td><td>11.633 s</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>447 ms</td><td>3610 sec</td></tr></tbody></table>
 
-‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
+> † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may be better than the numbers in this table.
+> 
+> ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
 
 Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
 Notably, most of the computational overhead of calling NeuralFoil is actually in the airfoil preprocessing step, where the airfoil is converted from a set of coordinates to a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-and-training-data)) - not in the aerodynamics analysis itself. This pre-processing takes around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://github.com/peterdsharpe/AeroSandbox/blob/c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/airfoil_families.py#L265), but in theory a pure-NumPy implementation is possible that would be much faster by exploiting linearity (sub-millisecond). If you're interested in working on this, open an issue and let me know! In the meantime, you can eliminate this overhead by using [`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to one of NeuralFoil's other functions.
 
@@ -107,14 +111,22 @@
 * [NumPy](https://numpy.org/)
 * [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) 4.0.10+
 
 Currently, NeuralFoil only uses AeroSandbox for airfoil geometry parameterization (i.e., converting from a set of points to a CST parameterization, which is solved as an optimization problem)—the actual math is implemented in pure NumPy. Recent progress on this CST parameterization-fitting problem has allowed it to be recast as a least-squares problem, which is potentially amenable to a pure-NumPy implementation. That being said, AeroSandbox provides a bunch of nice peripheral utilities (e.g., geometry manipulation, visualization, etc.), so it's a nice dependency to have anyway. However, if you'd like to work on a pure-NumPy implementation, open an issue and let me know!
 
 ## Geometry Parameterization and Training Data
 
+#### Geometry Parameterization
+
+To be written, but it's basically an 8-parameter-per-side CST (Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM) and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18 parameters to describe a given airfoil shape. I'll write more here, but in the meantime read:
+- [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
+- The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
+
+#### Training Data
+
 To be written, but in the meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes. Contact me if you need it sooner.
 
 ## FAQs
 
 Will NeuralFoil be integrated directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)?
 
 > Yes, absolutely. However, the goal is to keep this NeuralFoil repository also available as a stand-alone module, if desired. This simplifies dependencies for people using NeuralFoil in other applications (e.g., flight simulation, real-time control on embedded systems, etc.), and makes it easier if someone wanted to port NeuralFoil to another language (e.g., C++, for use on an Arduino).
```

#### html2text {}

```diff
@@ -2,21 +2,22 @@
 by [Peter Sharpe](https://peterdsharpe.github.io) (
 at] mit [dot] edu>) [![PyPI version](https://badge.fury.io/py/NeuralFoil.svg)]
 (https://badge.fury.io/py/NeuralFoil) [![Build Status](https://github.com/
 peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/
 peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/
 licenses/MIT) ----- NeuralFoil is a small Python/NumPy tool for rapid
-aerodynamics analysis of airfoils. It is also a small subset of the larger
-[AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is
-offered here as a standalone. Under the hood, NeuralFoil consists of physics-
-informed neural networks trained on tens of millions of [XFoil](https://
-web.mit.edu/drela/Public/web/xfoil/) runs. NeuralFoil aims to be lightweight,
-with [minimal dependencies](#dependencies-question) and a [tight, efficient
-code-base](./neuralfoil). NeuralFoil is ~10x faster than XFoil for a single
+aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/
+drela/Public/web/xfoil/). It is also a small subset of the larger [AeroSandbox]
+(https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here
+as a standalone. Under the hood, NeuralFoil consists of physics-informed neural
+networks trained on [tens of millions of XFoil runs](#geometry-
+parameterization-and-training-data). NeuralFoil aims to be lightweight, with
+[minimal dependencies](#dependencies-question) and a [tight, efficient code-
+base](./neuralfoil). NeuralFoil is ~10x faster than XFoil for a single
 analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in
 accuracy compared to XFoil](#performance). It also has [many nice features]
 (#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/
 NumPy) that make it much easier to use. ## Overview NeuralFoil comes with 8
 different neural network models, with increasing levels of complexity:
    "xxsmall" "xsmall" "small" "medium" "large" "xlarge" "xxlarge" "xxxlarge"
 This spectrum offers a tradeoff between accuracy and computational cost. In
@@ -37,38 +38,39 @@
 25, 1000), # Vectorize your evaluations across `alpha` and `Re` Re=5e6, ) aero
 = nf.get_aero_from_airfoil( # You can AeroSandbox airfoils as an entry point
 airfoil=asb.Airfoil("naca4412"), # `import aerosandbox as asb`, any UIUC or
 NACA airfoil name works alpha=5, Re=5e6, ) # `aero` is a dict with keys: ["CL",
 "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"] ``` ## Performance Qualitatively,
 NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$
 values. In the figure below, we compare the performance of NeuralFoil to XFoil
-on $C_L$-$C_D$ polar prediction. Notably, the airfoil analyzed here was
-developed "from scratch" for a real-world aircraft development program and is
-completely separate from [the airfoils used during NeuralFoil's training]
-(#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by
-"memorizing" this airfoil's performance:
+on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was
+developed "from scratch" for a [real-world aircraft development program](https:
+//www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-
+research-aircraft-301633713.html) and is completely separate from [the airfoils
+used during NeuralFoil's training](#geometry-parameterization-and-training-
+data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance:
                [./benchmarking/neuralfoil_point_validation.svg]
 NeuralFoil is typically accurate to within a few percent of XFoil's
-predictions. The error is largest at transitional $Re$ where the physics is the
-most nuanced, but is still quite close. NeuralFoil also [has the benefit of
-smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for
-example, near $C_L=0.75$ in the $Re=\mathrm{1M}$ case, where the bottom-surface
-boundary layer suddenly laminarizes, and the drag plummets), which would
-otherwise make optimization difficult. In the table below, we quantify the
-performance of the NeuralFoil ("NF") models with respect to XFoil more
-precisely. At a basic level, we care about two things: - **Accuracy**: how
-close are the predictions to XFoil's? - **Computational Cost**: how long does
-it take to run? This table details both of these considerations. The first few
-columns show the error with respect to XFoil on the test dataset. [The test
-dataset is completely isolated from the training dataset, and NeuralFoil was
-not allowed to learn from the test dataset](#geometry-parameterization-and-
-training-data). Thus, the performance on the test dataset gives a good idea of
-NeuralFoil's performance "in the wild".
-Aerodynamics Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to   Computational
-Model        XFoil                                                                             Cost to Run
+predictions. Note that this figure is on a truly out-of-sample airfoil, so
+airfoils that are closer to the UIUC-database training set will have even more
+accurate results. NeuralFoil also [has the benefit of smoothing out XFoil's
+"jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at
+$Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is
+obviously incorrect, which would otherwise make optimization difficult. In the
+table below, we quantify the performance of the NeuralFoil ("NF") models with
+respect to XFoil more precisely. At a basic level, we care about two things: -
+**Accuracy**: how close are the predictions to XFoil's? - **Computational
+Cost**: how long does it take to run? This table details both of these
+considerations. The first few columns show the error with respect to XFoil on
+the test dataset. [The test dataset is completely isolated from the training
+dataset, and NeuralFoil was not allowed to learn from the test dataset]
+(#geometry-parameterization-and-training-data). Thus, the performance on the
+test dataset gives a good idea of NeuralFoil's performance "in the wild".
+Aerodynamics Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset,  Computational
+Model        with respect to XFoil                                                             Cost to Run
                                                                                         Bottom
                                                                              Top        Trans.         Total
              Lift   Fractional Drag   Moment Max Overspeed                   Transition Loc.   Runtime Runtime
              Coeff. Coeff.            Coeff. $u_\max / u_\infty$   â¡ Loc.       $x_    (1 run) (100,000
              $C_L$  $\ln(C_D)$ â  $C_M$                                  $x_{tr,    {tr,           runs)
                                                                              top}/c$    bot}/
                                                                                         c$
@@ -81,31 +83,35 @@
 NF "medium"  0.027  0.051             0.004  0.088                           0.022      0.033  33 ms   0.749 s
 NF "large"   0.024  0.045             0.004  0.079                           0.020      0.029  35 ms   1.542 s
 NF "xlarge"  0.023  0.043             0.004  0.076                           0.019      0.028  36 ms   3.495 s
 NF "xxlarge" 0.021  0.040             0.003  0.071                           0.018      0.025  39 ms   4.557 s
 NF           0.020  0.039             0.003  0.070                           0.016      0.024  65 ms   11.633 s
 "xxxlarge"
 XFoil        0      0                 0      0                               0          0      447 ms  3610 sec
-â  The deviation of $\ln(C_D)$ can be thought of as "the typical relative
+> â  The deviation of $\ln(C_D)$ can be thought of as "the typical relative
 error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm)
-of $\ln(C_D)$ is 0.051, you can think of it as "typically, drag is accurate to
-within roughly 5.1%". â¡ This "maximum overspeed" lets you compute $C_
-{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm
-{crit}$. [More details below.](#compressibility-question) Based on these
-performance numbers, you can select the right tradeoff between accuracy and
-computational cost for your application. In general, I recommend starting with
-the "large" model and adjusting from there. In addition to accuracy vs. speed,
-another consideration when choosing the right model is what you're trying to
-use NeuralFoil for. Larger models will be more complicated ("less
-parsimonious," as the math kids would say), which means that they may have more
-"wiggles" in their outputsâthis might be undesirable for gradient-based
-optimization. On the other hand, larger models will be able to capture a wider
-range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be
-seen mid-optimization), so larger models could have a benefit in that sense. If
-you try a specific application and have better/worse results with a specific
+of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to
+within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil
+is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly
+not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure
+above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may
+be better than the numbers in this table. > > â¡ This "maximum overspeed" lets
+you compute $C_{p,\min}$, which can be used to calculate the critical Mach
+number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
+Based on these performance numbers, you can select the right tradeoff between
+accuracy and computational cost for your application. In general, I recommend
+starting with the "large" model and adjusting from there. In addition to
+accuracy vs. speed, another consideration when choosing the right model is what
+you're trying to use NeuralFoil for. Larger models will be more complicated
+("less parsimonious," as the math kids would say), which means that they may
+have more "wiggles" in their outputsâthis might be undesirable for gradient-
+based optimization. On the other hand, larger models will be able to capture a
+wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might
+be seen mid-optimization), so larger models could have a benefit in that sense.
+If you try a specific application and have better/worse results with a specific
 model, let me know by opening a GitHub issue! Notably, most of the
 computational overhead of calling NeuralFoil is actually in the airfoil
 preprocessing step, where the airfoil is converted from a set of coordinates to
 a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-
 and-training-data)) - not in the aerodynamics analysis itself. This pre-
 processing takes around 20 milliseconds using [AeroSandbox's general nonlinear
 solvers](https://github.com/peterdsharpe/AeroSandbox/blob/
@@ -124,26 +130,35 @@
 parameterization, which is solved as an optimization problem)âthe actual math
 is implemented in pure NumPy. Recent progress on this CST parameterization-
 fitting problem has allowed it to be recast as a least-squares problem, which
 is potentially amenable to a pure-NumPy implementation. That being said,
 AeroSandbox provides a bunch of nice peripheral utilities (e.g., geometry
 manipulation, visualization, etc.), so it's a nice dependency to have anyway.
 However, if you'd like to work on a pure-NumPy implementation, open an issue
-and let me know! ## Geometry Parameterization and Training Data To be written,
-but in the meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/
-master/training_data). Training data is not (yet) uploaded to GitHub, but will
-be soon - need to figure out Git LFS, as it's many gigabytes. Contact me if you
-need it sooner. ## FAQs Will NeuralFoil be integrated directly into
-[AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)? > Yes, absolutely.
-However, the goal is to keep this NeuralFoil repository also available as a
-stand-alone module, if desired. This simplifies dependencies for people using
-NeuralFoil in other applications (e.g., flight simulation, real-time control on
-embedded systems, etc.), and makes it easier if someone wanted to port
-NeuralFoil to another language (e.g., C++, for use on an Arduino).  Why not
-just use XFoil directly? > XFoil is a truly excellent piece of aerospace
+and let me know! ## Geometry Parameterization and Training Data #### Geometry
+Parameterization To be written, but it's basically an 8-parameter-per-side CST
+(Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM)
+and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) =
+18 parameters to describe a given airfoil shape. I'll write more here, but in
+the meantime read: - [D. A. Masters, "Geometric Comparison of Aerofoil Shape
+Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/
+10.2514/1.J054943) - The seminal paper on the CST (Kulfan) parameterization
+technique: [Brenda Kulfan, "Universal Parametric Geometry Representation
+Method"](http://mx1.brendakulfan.com/docs/CST6.pdf) #### Training Data To be
+written, but in the meantime [see here](https://github.com/peterdsharpe/
+NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to
+GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes.
+Contact me if you need it sooner. ## FAQs Will NeuralFoil be integrated
+directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)? >
+Yes, absolutely. However, the goal is to keep this NeuralFoil repository also
+available as a stand-alone module, if desired. This simplifies dependencies for
+people using NeuralFoil in other applications (e.g., flight simulation, real-
+time control on embedded systems, etc.), and makes it easier if someone wanted
+to port NeuralFoil to another language (e.g., C++, for use on an Arduino).  Why
+not just use XFoil directly? > XFoil is a truly excellent piece of aerospace
 software engineering and is the gold standard of airfoil analysis, for good
 reason. When its assumptions hold (airfoils in subsonic flow without massive
 separation), its accuracy exceeds that of RANS CFD, yet it has ~1000x lower
 computational cost. XFoil shines in particular for human-in-the-loop airfoil
 design. However, XFoil is not the right tool for all applications, for a few
 reasons: > > - XFoil exhibits hysteresis: you can get slightly different
 solutions (for the same airfoil, $\alpha$, and $Re$) depending on whether you
```

### Comparing `NeuralFoil-0.1.2/neuralfoil/CL_linear_regression.py` & `NeuralFoil-0.1.3/neuralfoil/CL_linear_regression.py`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/neuralfoil/neuralfoil.py` & `NeuralFoil-0.1.3/neuralfoil/neuralfoil.py`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-large.npz` & `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-large.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-medium.npz` & `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-medium.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-small.npz` & `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-small.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-xlarge.npz` & `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-xsmall.npz` & `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xsmall.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz` & `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz` & `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz` & `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.2/setup.py` & `NeuralFoil-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     python_requires='>=3.7',
     install_requires=[
         'numpy >= 1',
         'aerosandbox >= 4.0.10'
     ],
     extras_require={
         "training": [
-            'pytorch',
+            'torch',
             'ray',
             'polars',
             'tqdm'
         ],
         "test"    : [
             'pytest',
             'nbval'
```

