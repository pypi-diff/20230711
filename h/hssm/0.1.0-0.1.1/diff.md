# Comparing `tmp/hssm-0.1.0.tar.gz` & `tmp/hssm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hssm-0.1.0.tar", max compression
+gzip compressed data, was "hssm-0.1.1.tar", max compression
```

## Comparing `hssm-0.1.0.tar` & `hssm-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1100 2023-06-28 13:42:06.739838 hssm-0.1.0/LICENSE
--rw-r--r--   0        0        0     3194 2023-06-29 17:28:42.098050 hssm-0.1.0/README.md
--rw-r--r--   0        0        0     3968 2023-06-29 20:29:06.384495 hssm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      154 2023-06-29 20:29:06.384839 hssm-0.1.0/src/hssm/__init__.py
--rw-r--r--   0        0        0     4844 2023-06-29 20:29:06.385124 hssm-0.1.0/src/hssm/config.py
--rw-r--r--   0        0        0   193800 2023-06-29 17:28:42.110365 hssm-0.1.0/src/hssm/datasets/cavanagh_theta_nn.csv
--rw-r--r--   0        0        0     2451 2023-06-29 20:29:06.385419 hssm-0.1.0/src/hssm/datasets.py
--rw-r--r--   0        0        0      466 2023-06-29 20:29:06.385750 hssm-0.1.0/src/hssm/distribution_utils/__init__.py
--rw-r--r--   0        0        0    17589 2023-06-29 20:29:06.386367 hssm-0.1.0/src/hssm/distribution_utils/dist.py
--rw-r--r--   0        0        0      387 2023-06-29 20:29:06.386702 hssm-0.1.0/src/hssm/distribution_utils/onnx/__init__.py
--rw-r--r--   0        0        0     9978 2023-06-27 19:37:55.283352 hssm-0.1.0/src/hssm/distribution_utils/onnx/onnx.py
--rw-r--r--   0        0        0     1877 2023-06-27 19:37:55.283473 hssm-0.1.0/src/hssm/distribution_utils/onnx/onnx2pt.py
--rw-r--r--   0        0        0     5203 2023-06-27 19:37:55.283601 hssm-0.1.0/src/hssm/distribution_utils/onnx/onnx2xla.py
--rw-r--r--   0        0        0    26986 2023-06-29 20:29:06.387162 hssm-0.1.0/src/hssm/hssm.py
--rw-r--r--   0        0        0      180 2023-06-29 20:29:06.387621 hssm-0.1.0/src/hssm/likelihoods/__init__.py
--rw-r--r--   0        0        0    10994 2023-06-29 20:29:06.388040 hssm-0.1.0/src/hssm/likelihoods/analytical.py
--rw-r--r--   0        0        0    13536 2023-06-29 20:29:06.388494 hssm-0.1.0/src/hssm/param.py
--rw-r--r--   0        0        0     8405 2023-06-29 20:29:06.388885 hssm-0.1.0/src/hssm/utils.py
--rw-r--r--   0        0        0     4296 1970-01-01 00:00:00.000000 hssm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-11 20:33:47.394172 hssm-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4895 2023-07-11 20:33:47.394172 hssm-0.1.1/README.md
+-rw-r--r--   0        0        0     3968 2023-07-11 20:33:47.470173 hssm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-07-11 20:33:47.470173 hssm-0.1.1/src/hssm/__init__.py
+-rw-r--r--   0        0        0     4844 2023-07-11 20:33:47.470173 hssm-0.1.1/src/hssm/config.py
+-rw-r--r--   0        0        0   193800 2023-07-11 20:33:47.470173 hssm-0.1.1/src/hssm/datasets/cavanagh_theta_nn.csv
+-rw-r--r--   0        0        0     2451 2023-07-11 20:33:47.470173 hssm-0.1.1/src/hssm/datasets.py
+-rw-r--r--   0        0        0      466 2023-07-11 20:33:47.470173 hssm-0.1.1/src/hssm/distribution_utils/__init__.py
+-rw-r--r--   0        0        0    17589 2023-07-11 20:33:47.470173 hssm-0.1.1/src/hssm/distribution_utils/dist.py
+-rw-r--r--   0        0        0      387 2023-07-11 20:33:47.470173 hssm-0.1.1/src/hssm/distribution_utils/onnx/__init__.py
+-rw-r--r--   0        0        0     9978 2023-07-11 20:33:47.470173 hssm-0.1.1/src/hssm/distribution_utils/onnx/onnx.py
+-rw-r--r--   0        0        0     1877 2023-07-11 20:33:47.470173 hssm-0.1.1/src/hssm/distribution_utils/onnx/onnx2pt.py
+-rw-r--r--   0        0        0     5203 2023-07-11 20:33:47.470173 hssm-0.1.1/src/hssm/distribution_utils/onnx/onnx2xla.py
+-rw-r--r--   0        0        0    27913 2023-07-11 20:33:47.474173 hssm-0.1.1/src/hssm/hssm.py
+-rw-r--r--   0        0        0      180 2023-07-11 20:33:47.474173 hssm-0.1.1/src/hssm/likelihoods/__init__.py
+-rw-r--r--   0        0        0    10994 2023-07-11 20:33:47.474173 hssm-0.1.1/src/hssm/likelihoods/analytical.py
+-rw-r--r--   0        0        0    15271 2023-07-11 20:33:47.474173 hssm-0.1.1/src/hssm/param.py
+-rw-r--r--   0        0        0     2504 2023-07-11 20:33:47.474173 hssm-0.1.1/src/hssm/simulator.py
+-rw-r--r--   0        0        0     9531 2023-07-11 20:33:47.474173 hssm-0.1.1/src/hssm/utils.py
+-rw-r--r--   0        0        0     5997 1970-01-01 00:00:00.000000 hssm-0.1.1/PKG-INFO
```

### Comparing `hssm-0.1.0/LICENSE` & `hssm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hssm-0.1.0/pyproject.toml` & `hssm-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "HSSM"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = [
     "Aisulu Omar <aisulu_omar@brown.edu>",
     "Paul Xu <yang_xu@brown.edu>",
     "Alexander Fengler <alexander_fengler@brown.edu>",
     "Michael Frank <michael_frank@brown.edu>",
 ]
@@ -13,24 +13,24 @@
 packages = [{ include = "hssm", from = "src" }]
 repository = "https://github.com/lnccbrown/HSSM"
 keywords = ["HSSM", "sequential sampling models", "bayesian", "bayes", "mcmc"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 scipy = "1.10.1"
-pymc = "^5.0.1"
+pymc = "^5.6.0"
 arviz = "^0.14.0"
 numpy = "^1.23.4"
 onnx = "^1.12.0"
 jax = "^0.4.0"
 jaxlib = "^0.4.0"
 ssm-simulators = "^0.3.0"
 huggingface-hub = "^0.15.1"
 onnxruntime = "^1.15.0"
-bambi = "^0.11.0"
+bambi = "^0.12.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^22.8.0"
 mypy = "^1.4.1"
 pre-commit = "^2.20.0"
 jupyterlab = "^4.0.2"
```

### Comparing `hssm-0.1.0/src/hssm/config.py` & `hssm-0.1.1/src/hssm/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "ddm": {
         "analytical": {
             "loglik": logp_ddm,
             "bounds": ddm_bounds,
             "default_priors": {
                 "v": {"name": "Uniform", "lower": -10.0, "upper": 10.0},
                 "a": {"name": "HalfNormal", "sigma": 2.0},
-                "t": {"name": "Uniform", "lower": 0.0, "upper": 0.5, "initval": 0.1},
+                "t": {"name": "Uniform", "lower": 0.0, "upper": 2.0, "initval": 0.1},
             },
         },
         "approx_differentiable": {
             "loglik": "ddm.onnx",
             "backend": "jax",
             "bounds": {
                 "v": (-3.0, 3.0),
```

### Comparing `hssm-0.1.0/src/hssm/datasets/cavanagh_theta_nn.csv` & `hssm-0.1.1/src/hssm/datasets/cavanagh_theta_nn.csv`

 * *Files identical despite different names*

### Comparing `hssm-0.1.0/src/hssm/datasets.py` & `hssm-0.1.1/src/hssm/datasets.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.0/src/hssm/distribution_utils/dist.py` & `hssm-0.1.1/src/hssm/distribution_utils/dist.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.0/src/hssm/distribution_utils/onnx/onnx.py` & `hssm-0.1.1/src/hssm/distribution_utils/onnx/onnx.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.0/src/hssm/distribution_utils/onnx/onnx2pt.py` & `hssm-0.1.1/src/hssm/distribution_utils/onnx/onnx2pt.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.0/src/hssm/distribution_utils/onnx/onnx2xla.py` & `hssm-0.1.1/src/hssm/distribution_utils/onnx/onnx2xla.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.0/src/hssm/hssm.py` & `hssm-0.1.1/src/hssm/hssm.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 This file defines the entry class HSSM.
 """
 
 from __future__ import annotations
 
 from inspect import isclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Literal, cast
+from typing import TYPE_CHECKING, Any, Callable, Literal, cast
 
 import bambi as bmb
 import pymc as pm
 from numpy.typing import ArrayLike
 from pytensor.graph.op import Op
 
 from hssm.config import (
@@ -252,19 +252,21 @@
         other_kwargs: dict[Any, Any] = {}
         for k, v in kwargs.items():
             if k in self.list_params:
                 if k in params_in_include:
                     raise ValueError(
                         f'Parameter "{k}" is already specified in `include`.'
                     )
-
                 if isinstance(v, (int, float, bmb.Prior)):
                     include.append({"name": k, "prior": v})
                 elif isinstance(v, dict):
-                    include.append(v | {"name": k})
+                    if ("prior" in v) or ("bounds" in v):
+                        include.append(v | {"name": k})
+                    else:
+                        include.append({"name": k, "prior": v})
                 else:
                     raise ValueError(
                         f"Parameter {k} must be a float, a dict, or a bmb.Prior object."
                     )
             else:
                 other_kwargs |= {k: v}
 
@@ -389,14 +391,19 @@
         """
         processed = []
         params = []
         if include:
             for param_dict in include:
                 name = param_dict["name"]
                 processed.append(name)
+                for k in param_dict.keys():
+                    if k not in ["name", "formula", "prior", "link", "bounds"]:
+                        raise ValueError(
+                            f"Invalid key {k} for the specification of {name}!"
+                        )
                 param = _create_param(
                     param_dict, model_config, is_parent=name == self._parent
                 )
                 params.append(param)
 
         for param_str in self.list_params:
             if param_str not in processed:
@@ -411,31 +418,28 @@
         return params, *_parse_bambi(params)
 
     def sample(
         self,
         sampler: Literal[
             "mcmc", "nuts_numpyro", "nuts_blackjax", "laplace", "vi"
         ] = "mcmc",
-        step: Callable | Iterable[Callable] | None = None,
         **kwargs,
     ) -> az.InferenceData | pm.Approximation:
         """Perform sampling using the `fit` method via bambi.Model.
 
         Parameters
         ----------
         sampler
             The sampler to use. Can be either "mcmc" (default), "nuts_numpyro",
-            "nuts_blackjax", "laplace", or "vi".
-        step
-            A step function or collection of functions. If there are variables without
-            step methods, step methods for those variables will be assigned
-            automatically. By default the NUTS step method will be used, if appropriate
-            to the model.
+            "nuts_blackjax", "laplace", or "vi". If using `blackbox` likelihoods,
+            this cannot be "nuts_numpyro" or "nuts_blackjax".
         kwargs
-            Other arguments passed to bmb.Model.fit().
+            Other arguments passed to bmb.Model.fit(). Please see [here]
+            (https://bambinos.github.io/bambi/api_reference.html#bambi.models.Model.fit)
+            for full documentation.
 
         Returns
         -------
         az.InferenceData | pm.Approximation
             An ArviZ `InferenceData` instance if inference_method is `"mcmc"`
             (default), "nuts_numpyro", "nuts_blackjax" or "laplace". An `Approximation`
             object if `"vi"`.
@@ -443,20 +447,24 @@
         supported_samplers = ["mcmc", "nuts_numpyro", "nuts_blackjax", "laplace", "vi"]
 
         if sampler not in supported_samplers:
             raise ValueError(
                 f"Unsupported sampler '{sampler}', must be one of {supported_samplers}"
             )
 
-        if self.loglik_kind == "blackbox" and step is None:
-            step = pm.Slice(model=self.pymc_model)
+        if self.loglik_kind == "blackbox":
+            if sampler in ["nuts_blackjax", "nuts_numpyro"]:
+                raise ValueError(
+                    f"{sampler} sampler does not work with blackbox likelihoods."
+                )
 
-        self._inference_obj = self.model.fit(
-            inference_method=sampler, step=step, **kwargs
-        )
+            if "step" not in kwargs:
+                kwargs["step"] = pm.Slice(model=self.pymc_model)
+
+        self._inference_obj = self.model.fit(inference_method=sampler, **kwargs)
 
         return self.traces
 
     def sample_posterior_predictive(
         self,
         idata: az.InferenceData | None = None,
         data: pd.DataFrame | None = None,
@@ -595,14 +603,15 @@
         output = []
 
         output.append("Hierarchical Sequential Sampling Model")
         output.append(f"Model: {self.model_name}")
         output.append("")
 
         output.append("Response variable: rt,response")
+        output.append(f"Likelihood: {self.loglik_kind}")
         output.append(f"Observations: {len(self.data)}")
         output.append("")
 
         output.append("Parameters:")
         output.append("")
 
         for param in self.params:
@@ -673,24 +682,39 @@
     Returns
     -------
     Param
         A Param object with info form param and model_config injected.
     """
     if isinstance(param, dict):
         name = param["name"]
-        bounds = (
-            model_config["bounds"].get(name, None) if "bounds" in model_config else None
-        )
+        if "bounds" not in param:
+            bounds = (
+                model_config["bounds"].get(name, None)
+                if "bounds" in model_config
+                else None
+            )
+        else:
+            bounds = param["bounds"]
         if "prior" not in param or param["prior"] is None:
             if (
                 "default_priors" in model_config
                 and name in model_config["default_priors"]
+                and "formula" not in model_config
             ):
-                param["prior"] = model_config["default_priors"][name]
-        return Param(bounds=bounds, is_parent=is_parent, **param)
+                prior = model_config["default_priors"][name]
+        else:
+            prior = param["prior"]
+        return Param(
+            name=name,
+            prior=prior,
+            formula=param.get("formula"),
+            link=param.get("link"),
+            bounds=bounds,
+            is_parent=is_parent,
+        )
 
     bounds = (
         model_config["bounds"].get(param, None) if "bounds" in model_config else None
     )
     prior = (
         model_config["default_priors"].get(param, None)
         if "default_priors" in model_config
```

### Comparing `hssm-0.1.0/src/hssm/likelihoods/analytical.py` & `hssm-0.1.1/src/hssm/likelihoods/analytical.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.0/src/hssm/param.py` & `hssm-0.1.1/src/hssm/param.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,19 @@
         link: str | bmb.Link | None = None,
         bounds: BoundsSpec | None = None,
         is_parent: bool = False,
     ):
         self.name = name
         self.formula = formula
         self._parent = is_parent
-        self.bounds = bounds
+        self.bounds = tuple(float(x) for x in bounds) if bounds is not None else None
+        self._is_truncated = False
+
+        if isinstance(prior, int):
+            prior = float(prior)
 
         if formula is not None:
             # The regression case
 
             self.formula = formula if "~" in formula else f"{name} ~ {formula}"
 
             if isinstance(prior, (float, bmb.Prior)):
@@ -93,15 +97,31 @@
                     raise ValueError(
                         f"Please specify the prior or bounds for {self.name}."
                     )
                 self.prior = bmb.Prior(name="Uniform", lower=bounds[0], upper=bounds[1])
             else:
                 # Explicitly cast the type of prior, no runtime performance penalty
                 prior = cast(ParamSpec, prior)
-                self.prior = make_bounded_prior(prior, bounds)
+
+                if bounds is None:
+                    if isinstance(prior, (float, bmb.Prior)):
+                        self.prior = prior
+                    else:
+                        self.prior = bmb.Prior(**prior)
+                else:
+                    if isinstance(prior, float):
+                        self.prior = prior
+                    else:
+                        self.prior = make_bounded_prior(prior, bounds)
+                        # self._prior is internally used for informative output
+                        # Not used in inference
+                        self._prior = (
+                            bmb.Prior(**prior) if isinstance(prior, dict) else prior
+                        )
+                        self._is_truncated = True
 
             if link is not None:
                 raise ValueError("`link` should be None if no regression is specified.")
 
             self.link = None
 
     @property
@@ -122,14 +142,38 @@
         Returns
         -------
         bool
             A boolean that indicates if the parameter is a parent or not.
         """
         return self._parent
 
+    @property
+    def is_fixed(self) -> bool:
+        """Determine if a parameter is a fixed value.
+
+        Returns
+        -------
+        bool
+            A boolean that indicates if the parameter is a fixed value.
+        """
+        return isinstance(self.prior, float)
+
+    @property
+    def is_truncated(self) -> bool:
+        """Determines if a parameter is truncated.
+
+        A parameter is truncated when it is not a regression, is not fixed and has
+        bounds.
+
+        Returns
+        -------
+            A boolean that indicates if a parameter is truncated.
+        """
+        return self._is_truncated
+
     def _parse_bambi(
         self,
     ) -> tuple:
         """
         Return a 3-tuple that helps with constructing the Bambi model.
 
         Returns
@@ -172,37 +216,50 @@
 
         Returns
         -------
         str
             A string whose construction depends on whether the specification contains a
             regression or not.
         """
-        if not self.is_regression:
-            if isinstance(self.prior, bmb.Prior):
-                if self.bounds is None:
-                    return f"{self.name} ~ {self.prior}"
-                return f"{self.name} ~ {self.prior}\tbounds: {self.bounds}"
-            return f"{self.name} = {self.prior}"
-
-        link = self.link if isinstance(self.link, str) else self.link.name
-
-        assert not isinstance(self.prior, float)
-        assert self.formula is not None
-
-        priors = (
-            "\r\n".join([f"\t{param} ~ {prior}" for param, prior in self.prior.items()])
-            if self.prior is not None
-            else "Unspecified, using defaults"
-        )
+        output = []
+        output.append(self.name + ":")
 
-        if self.bounds is not None:
-            return "\r\n".join(
-                [self.formula, f"\tLink: {link}", f"\tbounds: {self.bounds}", priors]
-            )
-        return "\r\n".join([self.formula, f"\tLink: {link}", priors])
+        # Simplest case: float
+        # Output Value: 0.2
+        if isinstance(self.prior, float):
+            output.append(f"    Value: {self.prior}")
+            return "\r\n".join(output)
+
+        # Regression case:
+        # Output formula, priors, and link functions
+        if self.is_regression:
+            assert self.formula is not None
+            output.append(f"    Formula: {self.formula}")
+            output.append("    Priors:")
+
+            if self.prior is not None:
+                assert isinstance(self.prior, dict)
+
+                for param, prior in self.prior.items():
+                    output.append(f"        {param} ~ {prior}")
+            else:
+                output.append("        Unspecified. Using defaults")
+
+            link = self.link if isinstance(self.link, str) else self.link.name
+            output.append(f"    Link: {link}")
+
+        # None regression case:
+        # Output prior and bounds
+        else:
+            assert isinstance(self.prior, bmb.Prior)
+            prior_output = self._prior if self.is_truncated else self.prior
+            output.append(f"    Prior: {prior_output}")
+
+        output.append(f"    Explicit bounds: {self.bounds}")
+        return "\r\n".join(output)
 
     def __str__(self) -> str:
         """Return the string representation of the class.
 
         Returns
         -------
         str
@@ -322,17 +379,15 @@
     result_priors = None if not priors else priors
 
     result_links: dict | str = "identity" if not links else links
 
     return result_formula, result_priors, result_links
 
 
-def make_bounded_prior(
-    prior: ParamSpec, bounds: BoundsSpec | None = None
-) -> float | bmb.Prior:
+def make_bounded_prior(prior: ParamSpec, bounds: BoundsSpec) -> float | bmb.Prior:
     """Create prior within specific bounds.
 
     Helper function that creates a prior within specified bounds. Works in the
     following cases:
 
     1. If a prior passed is a fixed value, then check if the value is specified within
     the bounds. Raises a ValueError if not.
@@ -343,26 +398,23 @@
     The above boundary checks do not happen when bounds is None.
 
     Parameters
     ----------
     prior
         A prior definition. Could be a float, a dict that can be passed to a bmb.Prior
         to create a prior distribution, or a bmb.Prior.
-    bounds, optional
+    bounds : optional
         If provided, needs to be a tuple of floats that indicates the lower and upper
         bounds of the parameter.
 
     Returns
     -------
     float | bmb.Prior
         A float if `prior` is a float, otherwise a bmb.Prior object.
     """
-    if bounds is None:
-        return bmb.Prior(**prior) if isinstance(prior, dict) else prior
-
     lower, upper = bounds
 
     if isinstance(prior, float):
         if not lower <= prior <= upper:
             raise ValueError(
                 f"The fixed prior should be between {lower:.4f} and {upper:.4f}, "
                 + f"got {prior:.4f}."
@@ -378,17 +430,16 @@
     if prior.dist is not None:
         return prior
 
     name = prior.name
     args = prior.args
 
     dist = make_truncated_dist(lower, upper, name=name, **args)
-    prior.update(dist=dist)
 
-    return prior
+    return bmb.Prior(name=name, dist=dist)
 
 
 def make_truncated_dist(lower_bound: float, upper_bound: float, **kwargs) -> Callable:
     """Create custom functions with truncated priors.
 
     Helper function that creates a custom function with truncated priors.
 
@@ -411,15 +462,15 @@
     dist_kwargs = {k: v for k, v in kwargs.items() if k != "name"}
 
     initval = dist_kwargs.pop("initval") if "initval" in dist_kwargs else None
 
     def TruncatedDist(name):
         dist = get_distribution(dist_name).dist(**dist_kwargs)
         return pm.Truncated(
-            name="Truncated_" + name,
+            name=name,
             dist=dist,
             lower=lower_bound,
             upper=upper_bound,
             initval=initval,
         )
 
     return TruncatedDist
```

### Comparing `hssm-0.1.0/src/hssm/utils.py` & `hssm-0.1.1/src/hssm/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 The Param class is an abstraction that stores the parameter specifications and turns
 these representations in Bambi-compatible formats through convenience function
 _parse_bambi().
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Iterable, NewType
+import logging
+from typing import TYPE_CHECKING, Any, Iterable, Literal, NewType
 
+import pytensor
 from bambi.terms import CommonTerm, GroupSpecificTerm
 from huggingface_hub import hf_hub_download
+from jax.config import config
 from pymc.model_graph import ModelGraph
 from pytensor import function
 
 if TYPE_CHECKING:
     import bambi as bmb
 
     from .param import Param
@@ -247,7 +250,37 @@
                 else:
                     graph.edge(parent.replace(":", "&"), child.replace(":", "&"))
 
         if self.parent.is_regression:
             graph.edge(self.parent.name, "rt,response")
 
         return graph
+
+
+def set_floatX(dtype: Literal["float32", "float64"], jax: bool = True):
+    """Set float types for pytensor and Jax.
+
+    Often we wish to work with a specific type of float in both PyTensor and JAX.
+    This function helps set float types in both packages.
+
+    Parameters
+    ----------
+    dtype
+        Either `float32` or `float64`. Float type for pytensor (and jax if `jax=True`).
+    jax : optional
+        Whether this function also sets float type for JAX by changing the
+        `jax_enable_x64` setting in JAX config. Defaults to True.
+    """
+    if dtype not in ["float32", "float64"]:
+        raise ValueError('`dtype` must be either "float32" or "float64".')
+
+    pytensor.config.floatX = dtype
+    logging.info(f"Setting PyTensor floatX type to {dtype}")
+
+    if jax:
+        mapping = dict(float32=False, float64=True)
+        config.update("jax_enable_x64", mapping[dtype])
+
+        logging.info(
+            f'Setting "jax_enable_x64" to {mapping[dtype]}. '
+            + "If this is not intended, please set `jax` to False"
+        )
```

### Comparing `hssm-0.1.0/PKG-INFO` & `hssm-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,98 @@
-Metadata-Version: 2.1
-Name: hssm
-Version: 0.1.0
-Summary: 
-Home-page: https://github.com/lnccbrown/HSSM
-License: Copyright 2023, Brown University, Providence, RI.
-Keywords: HSSM,sequential sampling models,bayesian,bayes,mcmc
-Author: Aisulu Omar
-Author-email: aisulu_omar@brown.edu
-Requires-Python: >=3.9,<3.12
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: arviz (>=0.14.0,<0.15.0)
-Requires-Dist: bambi (>=0.11.0,<0.12.0)
-Requires-Dist: huggingface-hub (>=0.15.1,<0.16.0)
-Requires-Dist: jax (>=0.4.0,<0.5.0)
-Requires-Dist: jaxlib (>=0.4.0,<0.5.0)
-Requires-Dist: numpy (>=1.23.4,<2.0.0)
-Requires-Dist: onnx (>=1.12.0,<2.0.0)
-Requires-Dist: onnxruntime (>=1.15.0,<2.0.0)
-Requires-Dist: pymc (>=5.0.1,<6.0.0)
-Requires-Dist: scipy (==1.10.1)
-Requires-Dist: ssm-simulators (>=0.3.0,<0.4.0)
-Project-URL: Repository, https://github.com/lnccbrown/HSSM
-Description-Content-Type: text/markdown
-
 <p align="left">
   <img src="docs/images/mainlogo.png" width="250">
 </p>
 
 ## HSSM - Hierarchical Sequential Sampling Modeling
 
+![PyPI](https://img.shields.io/pypi/v/hssm)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hssm)
+![GitHub pull requests](https://img.shields.io/github/issues-pr/lnccbrown/HSSM)
+![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/lnccbrown/HSSM/run_tests.yml)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
 ### Overview
+
 HSSM is a Python toolbox that provides a seamless combination of state-of-the-art likelihood approximation methods with the wider ecosystem of probabilistic programming languages. It facilitates flexible hierarchical model building and inference via modern MCMC samplers. HSSM is user-friendly and provides the ability to rigorously estimate the impact of neural and other trial-by-trial covariates through parameter-wise mixed-effects models for a large variety of cognitive process models.
 
 - Allows approximate hierarchical Bayesian inference via various likelihood approximators.
 - Estimate impact of neural and other trial-by-trial covariates via native hierarchical mixed-regression support.
 - Extensible for users to add novel models with corresponding likelihoods.
 - Built on PyMC with support from the Python Bayesian ecosystem at large.
 - Incorporates Bambi's intuitive `lmer`-like regression parameter specification for within- and between-subject effects.
 - Native ArviZ support for plotting and other convenience functions to aid the Bayesian workflow.
 - Utilizes the ONNX format for translation of differentiable likelihood approximators across backends.
 
+### Official documentation link can be found [here](https://lnccbrown.github.io/HSSM/).
+
 ## Installation
 
 `hssm` is available through PyPI. You can install it with Pip via:
 
 ```
 pip install hssm
 ```
+
 You can also install the bleeding edge version of `hssm` directly from this repo:
 
 ```
-pip install git+https://github.com/lnccbrown/hssm.git
+pip install git+https://github.com/lnccbrown/HSSM.git
 ```
 
+### Optional Installation
+
+**Dependency for graph() Function**
+
+Note: In addition to the installation of the main hssm class, there is an optional dependency for the graph() function. This dependency requires graphviz, which can be installed conveniently using conda with the following command:
+
+```
+conda install -c conda-forge python-graphviz
+```
+
+Alternatively, you have the option to install the graphviz binaries manually and then install the Python bindings using pip with the following command:
+
+```
+pip install graphviz
+```
+
+**Dependency for sampler="nuts_numpyro"**
+
+To utilize the nuts_numpyro sampler, please follow these steps:
+
+1. Install numpyro by executing the following command:
+
+```
+pip install numpyro
+```
+
+2. Import the necessary modules and configure the required settings:
+
+```
+import numpyro
+from jax.config import config
+
+numpyro.set_host_device_count(jax.local_device_count())
+config.update("jax_enable_x64", False)
+```
+
+For more information please refer to [jax documentation](https://jax.readthedocs.io/en/latest/installation.html).
+
 ## Example
 
 Here is a simple example of how to use HSSM:
 
-```
+```python
 import hssm
-from hssm import load_data
+
+# Set float type to float32 to avoid a current bug in PyMC
+# This will not be necessary in the future
+hssm.set_floatX("float32")
 
 # Load a package-supplied dataset
-cav_data = load_data('cavanagh_theta')
+cav_data = hssm.load_data('cavanagh_theta')
 
 # Define a basic hierarchical model with trial-level covariates
 model = hssm.HSSM(
     model="ddm",
     data=cav_data,
     include=[
         {
@@ -86,23 +108,25 @@
 )
 
 # Sample from the posterior for this model
 model.sample()
 ```
 
 ## Example
+
 HSSM is licensed under [Copyright 2023, Brown University, Providence, RI](LICENSE)
 
 ## Support
+
 For questions, bug reports, or other unexpected issues, please open an issue on the GitHub repository.
 
 ## Contribution
+
 If you want to contribute to this project, please familiarize yourself with our [contribution guidelines](docs/CONTRIBUTING.md).
 
 ## Acknowledgements
 
 We would like to extend our gratitude to the following individuals for their valuable contributions to the development of the HSSM package:
 
 - [Bambi](https://github.com/bambinos/bambi) - A special thanks to the Bambi project for providing inspiration, guidance, and support throughout the development process. [Tomás Capretto](https://github.com/tomicapretto), a key contributor to Bambi, provided invaluable assistance in the development of the HSSM package.
 
 Those contributions have greatly enhanced the functionality and quality of the HSSM.
-
```

