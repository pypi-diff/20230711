# Comparing `tmp/phayes-0.1.0.tar.gz` & `tmp/phayes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phayes-0.1.0.tar", last modified: Fri Jun 30 17:18:43 2023, max compression
+gzip compressed data, was "phayes-0.1.1.tar", last modified: Tue Jul 11 13:29:17 2023, max compression
```

## Comparing `phayes-0.1.0.tar` & `phayes-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 samddd     (501) staff       (20)        0 2023-06-30 17:18:43.367931 phayes-0.1.0/
--rw-r--r--   0 samddd     (501) staff       (20)    10140 2023-01-20 11:23:57.000000 phayes-0.1.0/LICENSE
--rw-r--r--   0 samddd     (501) staff       (20)     3862 2023-06-30 17:18:43.367821 phayes-0.1.0/PKG-INFO
--rw-r--r--   0 samddd     (501) staff       (20)     3333 2023-06-30 17:18:09.000000 phayes-0.1.0/README.md
-drwxr-xr-x   0 samddd     (501) staff       (20)        0 2023-06-30 17:18:43.366914 phayes-0.1.0/phayes/
--rw-r--r--   0 samddd     (501) staff       (20)     2101 2023-06-05 10:45:19.000000 phayes-0.1.0/phayes/__init__.py
--rw-r--r--   0 samddd     (501) staff       (20)    13046 2023-06-05 14:53:27.000000 phayes-0.1.0/phayes/adaptive.py
--rw-r--r--   0 samddd     (501) staff       (20)    19920 2023-06-05 15:01:14.000000 phayes-0.1.0/phayes/fourier.py
--rw-r--r--   0 samddd     (501) staff       (20)     5714 2023-04-11 09:55:03.000000 phayes-0.1.0/phayes/maximise.py
--rw-r--r--   0 samddd     (501) staff       (20)     1445 2023-04-11 09:55:03.000000 phayes-0.1.0/phayes/sympy_solve_negative_variance.py
--rw-r--r--   0 samddd     (501) staff       (20)       22 2023-06-30 17:11:14.000000 phayes-0.1.0/phayes/version.py
--rw-r--r--   0 samddd     (501) staff       (20)    17124 2023-06-05 14:58:48.000000 phayes-0.1.0/phayes/von_mises.py
-drwxr-xr-x   0 samddd     (501) staff       (20)        0 2023-06-30 17:18:43.367644 phayes-0.1.0/phayes.egg-info/
--rw-r--r--   0 samddd     (501) staff       (20)     3862 2023-06-30 17:18:43.000000 phayes-0.1.0/phayes.egg-info/PKG-INFO
--rw-r--r--   0 samddd     (501) staff       (20)      328 2023-06-30 17:18:43.000000 phayes-0.1.0/phayes.egg-info/SOURCES.txt
--rw-r--r--   0 samddd     (501) staff       (20)        1 2023-06-30 17:18:43.000000 phayes-0.1.0/phayes.egg-info/dependency_links.txt
--rw-r--r--   0 samddd     (501) staff       (20)       34 2023-06-30 17:18:43.000000 phayes-0.1.0/phayes.egg-info/requires.txt
--rw-r--r--   0 samddd     (501) staff       (20)        7 2023-06-30 17:18:43.000000 phayes-0.1.0/phayes.egg-info/top_level.txt
--rw-r--r--   0 samddd     (501) staff       (20)       38 2023-06-30 17:18:43.367967 phayes-0.1.0/setup.cfg
--rw-r--r--   0 samddd     (501) staff       (20)      841 2023-04-06 07:56:44.000000 phayes-0.1.0/setup.py
+drwxr-xr-x   0 samddd     (501) staff       (20)        0 2023-07-11 13:29:17.265710 phayes-0.1.1/
+-rw-r--r--   0 samddd     (501) staff       (20)    10140 2023-01-20 11:23:57.000000 phayes-0.1.1/LICENSE
+-rw-r--r--   0 samddd     (501) staff       (20)     3902 2023-07-11 13:29:17.265582 phayes-0.1.1/PKG-INFO
+-rw-r--r--   0 samddd     (501) staff       (20)     3373 2023-06-30 17:21:00.000000 phayes-0.1.1/README.md
+drwxr-xr-x   0 samddd     (501) staff       (20)        0 2023-07-11 13:29:17.264544 phayes-0.1.1/phayes/
+-rw-r--r--   0 samddd     (501) staff       (20)     2229 2023-07-11 13:26:32.000000 phayes-0.1.1/phayes/__init__.py
+-rw-r--r--   0 samddd     (501) staff       (20)    15188 2023-07-11 13:28:36.000000 phayes-0.1.1/phayes/adaptive.py
+-rw-r--r--   0 samddd     (501) staff       (20)    19948 2023-07-11 13:28:21.000000 phayes-0.1.1/phayes/fourier.py
+-rw-r--r--   0 samddd     (501) staff       (20)     5714 2023-04-11 09:55:03.000000 phayes-0.1.1/phayes/maximise.py
+-rw-r--r--   0 samddd     (501) staff       (20)     1445 2023-04-11 09:55:03.000000 phayes-0.1.1/phayes/sympy_solve_negative_variance.py
+-rw-r--r--   0 samddd     (501) staff       (20)       22 2023-07-11 13:25:40.000000 phayes-0.1.1/phayes/version.py
+-rw-r--r--   0 samddd     (501) staff       (20)    17152 2023-07-11 13:28:21.000000 phayes-0.1.1/phayes/von_mises.py
+drwxr-xr-x   0 samddd     (501) staff       (20)        0 2023-07-11 13:29:17.265369 phayes-0.1.1/phayes.egg-info/
+-rw-r--r--   0 samddd     (501) staff       (20)     3902 2023-07-11 13:29:17.000000 phayes-0.1.1/phayes.egg-info/PKG-INFO
+-rw-r--r--   0 samddd     (501) staff       (20)      328 2023-07-11 13:29:17.000000 phayes-0.1.1/phayes.egg-info/SOURCES.txt
+-rw-r--r--   0 samddd     (501) staff       (20)        1 2023-07-11 13:29:17.000000 phayes-0.1.1/phayes.egg-info/dependency_links.txt
+-rw-r--r--   0 samddd     (501) staff       (20)       34 2023-07-11 13:29:17.000000 phayes-0.1.1/phayes.egg-info/requires.txt
+-rw-r--r--   0 samddd     (501) staff       (20)        7 2023-07-11 13:29:17.000000 phayes-0.1.1/phayes.egg-info/top_level.txt
+-rw-r--r--   0 samddd     (501) staff       (20)       38 2023-07-11 13:29:17.265752 phayes-0.1.1/setup.cfg
+-rw-r--r--   0 samddd     (501) staff       (20)      841 2023-04-06 07:56:44.000000 phayes-0.1.1/setup.py
```

### Comparing `phayes-0.1.0/LICENSE` & `phayes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phayes-0.1.0/PKG-INFO` & `phayes-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phayes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Bayesian phase and amplitude estimation
 Home-page: https://github.com/SamDuffield/bayesian-phase-estimation
 Author: Sam Duffield
 Author-email: sam.duffield@quantinuum.com
 License: Apache 2
 Platform: any
 Classifier: Programming Language :: Python
@@ -31,14 +31,20 @@
 quantum amplitude estimation [Suzuki et al, 2019](https://arxiv.org/abs/1904.10246)) can be implemented as an instance of Bayesian inference. Shots are generated from a quantum circuit with likelihood
 $$p(m \mid \phi, k, \beta) = \frac12\left(1 + (1 - q)\cos(k\phi + \beta - m \pi)\right),$$
 where $m \in \{0,1\}$ is the binary _shot_ produced by the quantum device, $\phi$ is the unknown underlying _phase_, $q$ is a noise parameter or error rate. $k$ and $\beta$ are circuit parameters that are chosen by the user (or `phayes`).
 
 Starting with a uniform prior over $\phi$, `phayes` uses Bayesian inference to hone in on the true value (with uncertainty quantification) through repeated measurements.
 
 
+## Install
+
+```
+pip install phayes
+```
+
 ## Bayesian updates
 
 The core functions are `phayes.get_k_and_beta` and `phayes.update`, which determine the experiment parameters and then update the posterior distribution in light of a new measurement (or series of measurements)
 
 ```python
 from jax import numpy as jnp
 import phayes
```

### Comparing `phayes-0.1.0/README.md` & `phayes-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 quantum amplitude estimation [Suzuki et al, 2019](https://arxiv.org/abs/1904.10246)) can be implemented as an instance of Bayesian inference. Shots are generated from a quantum circuit with likelihood
 $$p(m \mid \phi, k, \beta) = \frac12\left(1 + (1 - q)\cos(k\phi + \beta - m \pi)\right),$$
 where $m \in \{0,1\}$ is the binary _shot_ produced by the quantum device, $\phi$ is the unknown underlying _phase_, $q$ is a noise parameter or error rate. $k$ and $\beta$ are circuit parameters that are chosen by the user (or `phayes`).
 
 Starting with a uniform prior over $\phi$, `phayes` uses Bayesian inference to hone in on the true value (with uncertainty quantification) through repeated measurements.
 
 
+## Install
+
+```
+pip install phayes
+```
+
 ## Bayesian updates
 
 The core functions are `phayes.get_k_and_beta` and `phayes.update`, which determine the experiment parameters and then update the posterior distribution in light of a new measurement (or series of measurements)
 
 ```python
 from jax import numpy as jnp
 import phayes
```

### Comparing `phayes-0.1.0/phayes/__init__.py` & `phayes-0.1.1/phayes/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from phayes.adaptive import circular_m1
 from phayes.adaptive import circular_mean
 from phayes.adaptive import circular_variance
 from phayes.adaptive import holevo_variance
 from phayes.adaptive import cosine_distance
 from phayes.adaptive import evidence
 from phayes.adaptive import pdf
+from phayes.adaptive import expected_posterior_circular_variance
+from phayes.adaptive import expected_posterior_holevo_variance
 from phayes.adaptive import get_beta_given_k
 from phayes.adaptive import get_k_and_beta
 
 from phayes.fourier import fourier_update
 from phayes.fourier import fourier_circular_m1
 from phayes.fourier import fourier_circular_mean
 from phayes.fourier import fourier_circular_variance
```

### Comparing `phayes-0.1.0/phayes/adaptive.py` & `phayes-0.1.1/phayes/adaptive.py`

 * *Files 9% similar despite different names*

```diff
@@ -341,14 +341,84 @@
         state.fourier_mode,
         lambda s: fourier.fourier_pdf(val, s.fourier_coefficients),
         lambda s: von_mises.von_mises_pdf(val, *s.von_mises_parameters),
         state,
     )
 
 
+def expected_posterior_circular_variance(
+    state: PhayesState,
+    k: int,
+    beta: float,
+    error_rate: Union[float, Callable[[int], float]] = 0.0,
+) -> float:
+    """
+    Calculates expected circular variance of the single update posterior distribution.
+
+    E[var_C(p(phi | m, k, beta))] = Σ_m p(m | k, beta) var_C(p(phi | m, k, beta))
+
+    Args:
+        PhayesState
+            (namedtuple with fields: fourier_mode, fourier_coefficients, von_mises_parameters)
+        k: Integer exponent
+        beta: Phase shift in [0, 2π)
+        error_rate: Noise parameter, e.g. error_rate = 1 - exp(-k/T2)
+            Can be either a float or a Callable function of k
+
+    Returns:
+        float value in [0, 1]
+
+    """
+    return cond(
+        state.fourier_mode,
+        lambda s: fourier.fourier_expected_posterior_circular_variance(
+            s.fourier_coefficients, k, beta, error_rate
+        ),
+        lambda s: von_mises.von_mises_expected_posterior_circular_variance(
+            *s.von_mises_parameters, k, beta, error_rate
+        ),
+        state,
+    )
+
+
+def expected_posterior_holevo_variance(
+    state: PhayesState,
+    k: int,
+    beta: float,
+    error_rate: Union[float, Callable[[int], float]] = 0.0,
+) -> float:
+    """
+    Calculates expected Holevo variance of the single update posterior distribution.
+
+    E[var_H(p(phi | m, k, beta))] = Σ_m p(m | k, beta) var_H(p(phi | m, k, beta))
+
+    Args:
+        PhayesState
+            (namedtuple with fields: fourier_mode, fourier_coefficients, von_mises_parameters)
+        k: Integer exponent
+        beta: Phase shift in [0, 2π)
+        error_rate: Noise parameter, e.g. error_rate = 1 - exp(-k/T2)
+            Can be either a float or a Callable function of k
+
+    Returns:
+        float value in [0, ∞)
+
+    """
+    return cond(
+        state.fourier_mode,
+        lambda s: fourier.fourier_expected_posterior_holveo_variance(
+            s.fourier_coefficients, k, beta, error_rate
+        ),
+        lambda s: von_mises.von_mises_expected_posterior_holevo_variance(
+            *s.von_mises_parameters, k, beta, error_rate
+        ),
+        state,
+    )
+
+
 def get_beta_given_k(
     state: PhayesState,
     k: int,
     error_rate: Union[float, Callable[[int], float]] = 0.0,
 ) -> float:
     """
     Calculates beta that minimises the expected circular variance of a single update, for a given k.
```

### Comparing `phayes-0.1.0/phayes/fourier.py` & `phayes-0.1.1/phayes/fourier.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,17 @@
         fourier_coefficients: Array of shape (2, J) storing Fourier coefficients.
             First row for cosine, second for sine.
 
     Returns:
         Float or vector of pdf evaluations, same shape as val
     """
     val = jnp.atleast_1d(val)
-    return jnp.squeeze(vmap(_single_fourier_pdf, in_axes=(0, None))(val, fourier_coefficients))
+    return jnp.squeeze(
+        vmap(_single_fourier_pdf, in_axes=(0, None))(val, fourier_coefficients)
+    )
 
 
 def fourier_circular_m1(fourier_coefficients: jnp.ndarray) -> complex:
     """
     First circular moment of a Fourier distribution.
     Equal to E[exp(i * phi)] =  c1 + i s1.
 
@@ -334,15 +336,17 @@
         fourier_coefficients: Array of shape (2, J) storing Fourier coefficients.
             First row for cosine, second for sine.
 
     Returns:
         Float or vector of expected cosine distances, same shape as val
     """
     val = jnp.atleast_1d(val)
-    return jnp.squeeze(vmap(_fourier_cosine_distance, in_axes=(0, None))(val, fourier_coefficients))
+    return jnp.squeeze(
+        vmap(_fourier_cosine_distance, in_axes=(0, None))(val, fourier_coefficients)
+    )
 
 
 def fourier_evidence(
     fourier_coefficients: jnp.ndarray,
     m: int,
     k: int,
     beta: float,
```

### Comparing `phayes-0.1.0/phayes/maximise.py` & `phayes-0.1.1/phayes/maximise.py`

 * *Files identical despite different names*

### Comparing `phayes-0.1.0/phayes/sympy_solve_negative_variance.py` & `phayes-0.1.1/phayes/sympy_solve_negative_variance.py`

 * *Files identical despite different names*

### Comparing `phayes-0.1.0/phayes/von_mises.py` & `phayes-0.1.1/phayes/von_mises.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,17 @@
         kappa: Prior von Mises concentration parameter, float in [0, ∞)
 
     Returns:
         Float or vector of expected cosine distances, same shape as val
     """
     val = jnp.atleast_1d(val)
     A = bessel_ratio(kappa)
-    return jnp.squeeze(1 - A * (jnp.cos(mu) * jnp.cos(val) + jnp.sin(mu) * jnp.sin(val)))
+    return jnp.squeeze(
+        1 - A * (jnp.cos(mu) * jnp.cos(val) + jnp.sin(mu) * jnp.sin(val))
+    )
 
 
 def von_mises_entropy(kappa: float) -> float:
     """
     Evaluates H(mu, kappa) = - kappa * I1(kappa) / I0(kappa) + log(2 * pi * I0(kappa)),
     the entropy of a von Mises distribution.
 
@@ -288,15 +290,17 @@
         mu: Prior von Mises mean parameter, float in [0, 2π)
         kappa: Prior von Mises concentration parameter, float in [0, ∞)
 
     Returns:
         Float or vector of pdf evaluations, same shape as val
     """
     val = jnp.atleast_1d(val)
-    return jnp.squeeze(jnp.exp(kappa * (jnp.cos(val - mu) - 1)) / (2 * jnp.pi * special.i0e(kappa)))
+    return jnp.squeeze(
+        jnp.exp(kappa * (jnp.cos(val - mu) - 1)) / (2 * jnp.pi * special.i0e(kappa))
+    )
 
 
 def von_mises_evidence(
     mu: jnp.ndarray,
     kappa: float,
     m: int,
     k: int,
@@ -399,28 +403,28 @@
     mu: jnp.ndarray,
     kappa: float,
     k: int,
     beta: float,
     error_rate: Union[float, Callable[[int], float]] = 0.0,
 ) -> float:
     """
-    Calculates expected circular variance of the single update posterior distribution.
+    Calculates expected Holevo variance of the single update posterior distribution.
 
-    E[var_C(p(phi | m, k, beta))] = Σ_m p(m | k, beta) var_C(p(phi | m, k, beta))
+    E[var_H(p(phi | m, k, beta))] = Σ_m p(m | k, beta) var_H(p(phi | m, k, beta))
 
     Args:
         mu: Prior von Mises mean parameter, float in [0, 2π)
         kappa: Prior von Mises concentration parameter, float in [0, ∞)
         k: Integer exponent
         beta: Phase shift in [0, 2π)
         error_rate: Noise parameter, e.g. error_rate = 1 - exp(-k/T2)
             Can be either a float or a Callable function of k
 
     Returns:
-        float value in [0, 1]
+        float value in [0, ∞)
 
     """
     if callable(error_rate):
         error_rate = error_rate(k)
 
     abar, bbar, cbar, dbar, ebar, fbar = _posterior_m1_coeffs(mu, kappa, k, error_rate)
```

### Comparing `phayes-0.1.0/phayes.egg-info/PKG-INFO` & `phayes-0.1.1/phayes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phayes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Bayesian phase and amplitude estimation
 Home-page: https://github.com/SamDuffield/bayesian-phase-estimation
 Author: Sam Duffield
 Author-email: sam.duffield@quantinuum.com
 License: Apache 2
 Platform: any
 Classifier: Programming Language :: Python
@@ -31,14 +31,20 @@
 quantum amplitude estimation [Suzuki et al, 2019](https://arxiv.org/abs/1904.10246)) can be implemented as an instance of Bayesian inference. Shots are generated from a quantum circuit with likelihood
 $$p(m \mid \phi, k, \beta) = \frac12\left(1 + (1 - q)\cos(k\phi + \beta - m \pi)\right),$$
 where $m \in \{0,1\}$ is the binary _shot_ produced by the quantum device, $\phi$ is the unknown underlying _phase_, $q$ is a noise parameter or error rate. $k$ and $\beta$ are circuit parameters that are chosen by the user (or `phayes`).
 
 Starting with a uniform prior over $\phi$, `phayes` uses Bayesian inference to hone in on the true value (with uncertainty quantification) through repeated measurements.
 
 
+## Install
+
+```
+pip install phayes
+```
+
 ## Bayesian updates
 
 The core functions are `phayes.get_k_and_beta` and `phayes.update`, which determine the experiment parameters and then update the posterior distribution in light of a new measurement (or series of measurements)
 
 ```python
 from jax import numpy as jnp
 import phayes
```

### Comparing `phayes-0.1.0/setup.py` & `phayes-0.1.1/setup.py`

 * *Files identical despite different names*

