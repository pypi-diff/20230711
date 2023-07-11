# Comparing `tmp/gecs-0.28.3.tar.gz` & `tmp/gecs-0.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecs-0.28.3.tar", max compression
+gzip compressed data, was "gecs-0.29.0.tar", max compression
```

## Comparing `gecs-0.28.3.tar` & `gecs-0.29.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.28.3/LICENSE
--rw-r--r--   0        0        0     2220 2023-07-03 10:39:36.682086 gecs-0.28.3/README.md
--rw-r--r--   0        0        0      697 2023-07-03 17:47:08.299609 gecs-0.28.3/pyproject.toml
--rw-r--r--   0        0        0    44198 2023-07-03 17:47:08.299609 gecs-0.28.3/src/gecs/gec.py
--rw-r--r--   0        0        0     2112 2023-06-19 14:54:28.150721 gecs-0.28.3/src/gecs/utils/gaussian_process_visualisation.py
--rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 gecs-0.28.3/setup.py
--rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 gecs-0.28.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-07-11 17:36:42.496116 gecs-0.29.0/LICENSE
+-rw-r--r--   0        0        0     2220 2023-07-11 17:36:43.424133 gecs-0.29.0/README.md
+-rw-r--r--   0        0        0      697 2023-07-11 18:17:15.906277 gecs-0.29.0/pyproject.toml
+-rw-r--r--   0        0        0    47487 2023-07-11 18:17:15.906277 gecs-0.29.0/src/gecs/gec.py
+-rw-r--r--   0        0        0     2152 2023-07-11 18:17:15.906277 gecs-0.29.0/src/gecs/utils/gaussian_process_visualisation.py
+-rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 gecs-0.29.0/setup.py
+-rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 gecs-0.29.0/PKG-INFO
```

### Comparing `gecs-0.28.3/LICENSE` & `gecs-0.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gecs-0.28.3/README.md` & `gecs-0.29.0/README.md`

 * *Files identical despite different names*

### Comparing `gecs-0.28.3/pyproject.toml` & `gecs-0.29.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gecs"
-version = "0.28.3"
+version = "0.29.0"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "LightGBM Classifier with integrated bayesian hyperparameter optimization"
 keywords = ["lightgbm", "classification", "machine learning", "hyperparameter optimization", "classifier"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `gecs-0.28.3/src/gecs/gec.py` & `gecs-0.29.0/src/gecs/gec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
+import contextlib
+import copy
 import inspect
 import itertools
-from typing import Optional, Union, Dict, Callable
+import json
+import math
 import os
-import contextlib
-from tqdm import tqdm
+import warnings
 from datetime import datetime
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-import warnings
+import matplotlib.pyplot as plt
 import numpy as np
-import json
-import math
-import copy
 import scipy
-
-import matplotlib.pyplot as plt
+from lightgbm import LGBMClassifier
+from lightgbm.basic import LightGBMError
+from lightgbm.compat import SKLEARN_INSTALLED
 from matplotlib import cm
-
-from sklearn.exceptions import ConvergenceWarning
+from matplotlib.axes._axes import Axes
+from matplotlib.figure import Figure
+from numpy import float16, float64, ndarray, str_
+from numpy.random.mtrand import RandomState
 from scipy.stats import beta
-from sklearn.gaussian_process.kernels import RBF
-from sklearn.utils.extmath import cartesian
+from sklearn.exceptions import ConvergenceWarning
 from sklearn.gaussian_process import GaussianProcessRegressor
+from sklearn.gaussian_process.kernels import RBF
 from sklearn.model_selection import cross_val_score
-
-from lightgbm import LGBMClassifier
-from lightgbm.basic import LightGBMError
-from lightgbm.compat import SKLEARN_INSTALLED
+from sklearn.utils.extmath import cartesian
+from tqdm import tqdm
 
 
 class GEC(LGBMClassifier):
     def __init__(
         self,
         boosting_type: str = "gbdt",
         num_leaves: int = 31,
@@ -49,20 +50,25 @@
         reg_lambda: float = 0.0,
         random_state: Optional[Union[int, np.random.RandomState]] = None,
         n_jobs: int = -1,
         silent: Union[bool, str] = "warn",
         importance_type: str = "split",
         frozen: bool = False,
         **kwargs,
-    ):
-        adapted_lgbm_params = str(inspect.signature(LGBMClassifier.__init__)).replace(
-            "importance_type: str = 'split'", "importance_type: str = 'split', frozen: bool = False"
-        ) 
-        gec_params = str( inspect.signature(GEC.__init__))
-        assert adapted_lgbm_params == gec_params, gec_params
+    ) -> None:
+        adapted_lgbm_params = (
+            str(inspect.signature(LGBMClassifier.__init__))
+            .replace(
+                "importance_type: str = 'split'",
+                "importance_type: str = 'split', frozen: bool = False",
+            )
+            .replace("**kwargs)", "**kwargs) -> None")
+        )
+        gec_params = str(inspect.signature(GEC.__init__))
+        assert adapted_lgbm_params == gec_params, adapted_lgbm_params
 
         r"""Construct a gradient boosting model.
 
         Parameters
         ----------
         boosting_type : str, optional (default='gbdt')
             'gbdt', traditional Gradient Boosting Decision Tree.
@@ -202,35 +208,34 @@
         self._n_features = None
         self._n_features_in = None
         self._classes = None
         self._n_classes = None
         self.set_params(**kwargs)
 
         self._init_kwargs = {
-            k: v for k, v in kwargs.items()
+            k: v
+            for k, v in kwargs.items()
             if k not in ["bagging_freq", "bagging_fraction"]
         }
 
         self.frozen = frozen
         non_optimized_init_args = [
             "max_depth",
             "subsample_for_bin",
             "objective",
             "class_weight",
-            "min_split_gain", 
+            "min_split_gain",
             "subsample",
             "subsample_freq",
             "random_state",
             "n_jobs",
             "silent",
-            "importance_type"
+            "importance_type",
         ]
-        self._init_args = {
-            arg: getattr(self, arg) for arg in non_optimized_init_args
-        }
+        self._init_args = {arg: getattr(self, arg) for arg in non_optimized_init_args}
 
         self.gec_hyperparameters = {
             "l": 1.0,
             "l_bagging": 0.1,
             "hyperparams_acquisition_percentile": 0.7,
             "bagging_acquisition_percentile": 0.7,
             "bandit_greediness": 1.0,
@@ -242,23 +247,22 @@
                 "learning_rate",
                 "n_estimators",
                 "num_leaves",
                 "reg_alpha",
                 "reg_lambda",
                 "min_child_samples",
                 "min_child_weight",
-                "colsample_bytree", #feature_fraction
+                "colsample_bytree",  # feature_fraction
             ],
-            "randomize": True
+            "randomize": True,
         }
         self._set_gec_attributes()
         self._set_gec_fields()
 
-
-    def _set_gec_attributes(self):
+    def _set_gec_attributes(self) -> None:
         self.categorical_hyperparameters = [
             ("boosting_type", ["gbdt", "dart", "rf"]),
             ("bagging", ["yes_bagging", "no_bagging"]),
         ]
 
         self._categorical_hyperparameter_names, _ = zip(
             *self.categorical_hyperparameters
@@ -279,32 +283,62 @@
                 np.arange(100, 200, 20),
                 np.arange(200, 500, 50),
                 np.arange(500, 100, 100),
                 np.arange(1000, 10001, 1000),
             ]
         )
         self._real_hyperparameters_all = [
-            ("learning_rate", (np.concatenate([np.arange(0.001, 0.5, 0.003), np.arange(0.5, 0.95, 0.02)])**2)),
-            ("num_leaves",  np.array(list(range(1, 100))+list(range(100, 1000, 5)))),
+            (
+                "learning_rate",
+                (
+                    np.concatenate(
+                        [np.arange(0.001, 0.5, 0.003), np.arange(0.5, 0.95, 0.02)]
+                    )
+                    ** 2
+                ),
+            ),
+            ("num_leaves", np.array(list(range(1, 100)) + list(range(100, 1000, 5)))),
             ("n_estimators", ten_to_ten_thousand),
-            ("reg_alpha", (np.concatenate([np.arange(0.0, 0.5, 0.01), np.arange(0.5, 1.00, 0.02)])**2)),
-            ("reg_lambda", (np.concatenate([np.arange(0.0, 0.5, 0.01), np.arange(0.5, 1.00, 0.02)])**2)),
-            ("min_child_weight", list( np.concatenate([np.arange(0.0, 0.1, 0.001), np.arange(0.1, 0.5, 0.05)])**2)),
+            (
+                "reg_alpha",
+                (
+                    np.concatenate(
+                        [np.arange(0.0, 0.5, 0.01), np.arange(0.5, 1.00, 0.02)]
+                    )
+                    ** 2
+                ),
+            ),
+            (
+                "reg_lambda",
+                (
+                    np.concatenate(
+                        [np.arange(0.0, 0.5, 0.01), np.arange(0.5, 1.00, 0.02)]
+                    )
+                    ** 2
+                ),
+            ),
+            (
+                "min_child_weight",
+                list(
+                    np.concatenate(
+                        [np.arange(0.0, 0.1, 0.001), np.arange(0.1, 0.5, 0.05)]
+                    )
+                    ** 2
+                ),
+            ),
             ("min_child_samples", np.arange(2, 50, 1)),
-            ("colsample_bytree",np.arange(0.1, 1.00, 0.01))
+            ("colsample_bytree", np.arange(0.1, 1.00, 0.01)),
         ]
 
         self.fixed_params = {
             hyperparameter: getattr(self, hyperparameter)
             for hyperparameter, _ in self._real_hyperparameters_all
             if hyperparameter not in self.gec_hyperparameters["hyperparameters"]
         }
 
-
-
         self._real_hyperparameters = [
             (hp_name, range_)
             for hp_name, range_ in self._real_hyperparameters_all
             if hp_name in self.gec_hyperparameters["hyperparameters"]
         ]
         self._real_hyperparameters_linear = [
             (name, np.arange(-1, 1, 2 / len(values)).astype(np.float16))
@@ -323,43 +357,56 @@
             for ((name, linear_values), (_, real_values)) in zip(
                 self._real_hyperparameters_linear, self._real_hyperparameters
             )
         }
 
         self._validate_parameter_maps()
 
-
         self._real_hyperparameter_names, self._real_hyperparameter_ranges = zip(
             *self._real_hyperparameters_linear
         )
 
         self._real_hypermarameter_types = [
             np.array(s).dtype for _, s in self._real_hyperparameters
         ]
 
-    def _set_gec_fields(self):
+    def _set_gec_fields(self) -> None:
         self.kernel = RBF(self.gec_hyperparameters["l"])
-        self.hyperparameter_scores = {"inputs": [], "output": [], "means": [], "sigmas": []}
+        self.hyperparameter_scores = {
+            "inputs": [],
+            "output": [],
+            "means": [],
+            "sigmas": [],
+        }
 
         self.kernel_bagging = RBF(self.gec_hyperparameters["l_bagging"])
 
         self.bagging_scores = {"inputs": [], "output": [], "means": [], "sigmas": []}
 
         self._bagging_combinations = list(
             itertools.product(
                 *[
                     list(range(1, 11, 1)),
                     np.arange(0.5, 1.0, 0.01),
                 ]
             )
         )
 
-        self._rescale_bagging_combination = lambda freq, frac: (((freq/5)-1), ((frac*4)-3))
-        self._invert_rescaled_bagging_combination =  lambda freq, frac: (((freq+1)*5), ((frac+3)/4))
-        self._bagging_combinations_rescaled = [self._rescale_bagging_combination(freq, frac) for freq, frac in self._bagging_combinations]
+        self._rescale_bagging_combination = lambda freq, frac: (
+            ((freq / 5) - 1),
+            ((frac * 4) - 3),
+        )
+        self._invert_rescaled_bagging_combination = lambda freq, frac: (
+            ((freq + 1) * 5),
+            ((frac + 3) / 4),
+        )
+        self._bagging_combinations_rescaled = [
+            self._rescale_bagging_combination(freq, frac)
+            for freq, frac in self._bagging_combinations
+        ]
 
         self.best_score = None
         self.best_params_ = None
         self.fit_params = None
         self.n_iterations = 0
 
         # parameters for bandit
@@ -383,15 +430,15 @@
 
     @kernel_bagging.setter
     def kernel_bagging(self, value):
         self._kernel_bagging = value
         self.gaussian_bagging = GaussianProcessRegressor(kernel=value)
 
     @property
-    def gec_iter(self):
+    def gec_iter(self) -> int:
         return len(self.hyperparameter_scores["output"])
 
     @classmethod
     def _cast_to_type(cls, value, type_):
         if type_ == np.float64:
             return float(value)
         elif type_ == np.int64:
@@ -461,28 +508,45 @@
         """
         representation = self._get_representation()
 
         with open(path, "w") as f:
             f.write(json.dumps(representation))
 
     @classmethod
-    def _convert_gaussian_process_data_for_serialisation(cls, data_dict):
+    def _convert_gaussian_process_data_for_serialisation(
+        cls,
+        data_dict: Dict[
+            str,
+            Union[
+                List[Union[List[float], float64, int, ndarray]],
+                List[Union[List[Union[float, float64]], float64, int, ndarray]],
+            ],
+        ],
+    ) -> Dict[
+        str,
+        Union[
+            List[Union[List[Union[float, float64]], float64, int, List[float64]]],
+            List[Union[List[float], float64, int, List[float64]]],
+        ],
+    ]:
         def process_value(key, value):
             if not isinstance(value, np.ndarray):
                 return value
             elif key != "inputs":
                 return list(value)
             else:
                 return list(value.astype(np.float64))
 
-        converted_dict = {k2: [process_value(k2, vv) for vv in v] for k2, v in data_dict.items()}
+        converted_dict = {
+            k2: [process_value(k2, vv) for vv in v] for k2, v in data_dict.items()
+        }
 
         return converted_dict
 
-    def _get_representation(self):
+    def _get_representation(self) -> Dict[str, Any]:
         hyperparameter_scores = self._convert_gaussian_process_data_for_serialisation(
             self.hyperparameter_scores
         )
         bagging_scores = self._convert_gaussian_process_data_for_serialisation(
             self.bagging_scores
         )
         representation = {
@@ -492,102 +556,111 @@
             "hyperparameter_scores": hyperparameter_scores,
             "bagging_scores": bagging_scores,
             "best_params_": self.best_params_,
             "best_score": self.best_score,
             "best_params_gec": self.best_params_gec,
             "best_scores_gec": self.best_scores_gec,
             "gec_iter": self.gec_iter,
-            "fit_params": self.fit_params
+            "fit_params": self.fit_params,
         }
         return representation
 
-
-    def _validate_parameter_maps(self):
+    def _validate_parameter_maps(self) -> None:
         real_to_linear_to_real = [
-            self._real_hyperparameters_map[hp][self._real_hyperparameters_map_reverse[hp][v]] == v
-            for hp, values in self._real_hyperparameters for v in values
+            self._real_hyperparameters_map[hp][
+                self._real_hyperparameters_map_reverse[hp][v]
+            ]
+            == v
+            for hp, values in self._real_hyperparameters
+            for v in values
         ]
 
         assert np.all(real_to_linear_to_real), real_to_linear_to_real
 
         linear_to_real_to_linear = [
-            self._real_hyperparameters_map_reverse[hp][self._real_hyperparameters_map[hp][v]] == v
-            for hp, values in self._real_hyperparameters_linear for v in values
+            self._real_hyperparameters_map_reverse[hp][
+                self._real_hyperparameters_map[hp][v]
+            ]
+            == v
+            for hp, values in self._real_hyperparameters_linear
+            for v in values
         ]
         assert np.all(linear_to_real_to_linear), linear_to_real_to_linear
 
-    def set_gec_hyperparameters(self, gec_hyperparameters):
+    def set_gec_hyperparameters(
+        self, gec_hyperparameters: Dict[str, Union[int, float, List[str]]]
+    ) -> None:
         """Set the hyperparameters of the GEC optimisation process
 
         Parameters
         ----------
             gec_hyperparameters : dict[str, float]
                 dictionary with keys that are in self.gec_hyperparameters
         """
         assert np.all(
-            np.array([hp in self.gec_hyperparameters for hp in gec_hyperparameters.keys()])
+            np.array(
+                [hp in self.gec_hyperparameters for hp in gec_hyperparameters.keys()]
+            )
         )
         self.gec_hyperparameters.update(gec_hyperparameters)
         self._set_gec_attributes()
 
-
     def freeze(self):
         self.frozen = True
-        return(self)
+        return self
 
     def unfreeze(self):
         self.frozen = False
-        return(self)
-    
+        return self
 
-    def set_params(self, **kwargs):
+    def set_params(self, **kwargs) -> None:
         if "frozen" in kwargs:
             self["frozen"] = kwargs.pop("frozen")
         super().set_params(**kwargs)
 
-
-    def get_params(self, deep=True):
+    def get_params(
+        self, deep: bool = True
+    ) -> Dict[str, Optional[Union[str, float, int, bool]]]:
         if hasattr(self, "best_params_") and self.best_params_ is not None:
             params = copy.deepcopy(self.best_params_)
         else:
             params = super().get_params(deep)
         params["frozen"] = self.frozen
-        
-        return(params)
+
+        return params
 
     def __sklearn_clone__(self):
         gec = GEC()
 
         for k, v in self.__dict__.items():
             gec.__dict__[k] = copy.deepcopy(v)
 
-        return(gec)
-
+        return gec
 
     def fit(
-            self,
-            X,
-            y,
-            n_iter=50,
-            fixed_hyperparameters=["n_estimators", "num_leaves"],
-            sample_weight=None,
-            init_score=None,
-            eval_set=None,
-            eval_names=None,
-            eval_sample_weight=None,
-            eval_class_weight=None,
-            eval_init_score=None,
-            eval_metric=None,
-            feature_name='auto',
-            categorical_feature='auto',
-            callbacks=None,
-            init_model=None
-        ):
+        self,
+        X: ndarray,
+        y: ndarray,
+        n_iter: int = 50,
+        fixed_hyperparameters: List[str] = ["n_estimators", "num_leaves"],
+        sample_weight=None,
+        init_score=None,
+        eval_set=None,
+        eval_names=None,
+        eval_sample_weight=None,
+        eval_class_weight=None,
+        eval_init_score=None,
+        eval_metric=None,
+        feature_name="auto",
+        categorical_feature="auto",
+        callbacks=None,
+        init_model=None,
+    ) -> "GEC":
         """Docstring is inherited from the LGBMClassifier.
-        
+
         Except for
 
         Parameters:
         ----------
             n_iter : int
                 number of optimization steps
             fixed_hyperparameters : list[str]
@@ -602,28 +675,30 @@
             "eval_sample_weight": eval_sample_weight,
             "eval_class_weight": eval_class_weight,
             "eval_init_score": eval_init_score,
             "eval_metric": eval_metric,
             "feature_name": feature_name,
             "categorical_feature": categorical_feature,
             "callbacks": callbacks,
-            "init_model": init_model
+            "init_model": init_model,
         }
         if not self.frozen:
-            filtered_hyperparameters = list(set(self.gec_hyperparameters["hyperparameters"]).difference(set(fixed_hyperparameters)))
-            self.set_gec_hyperparameters({"hyperparameters": filtered_hyperparameters })
+            filtered_hyperparameters = list(
+                set(self.gec_hyperparameters["hyperparameters"]).difference(
+                    set(fixed_hyperparameters)
+                )
+            )
+            self.set_gec_hyperparameters({"hyperparameters": filtered_hyperparameters})
 
             self.best_scores_gec = {}
             self.best_params_gec = {}
             (
                 self.best_params_gec["search"],
                 self.best_scores_gec["search"],
-            ) = self._optimise_hyperparameters(
-                n_iter, X, y, self.best_score, self.best_params_
-            )
+            ) = self._optimise_hyperparameters(n_iter, X, y)
             self.best_params_gec["grid"] = self._find_best_parameters()
             self.best_scores_gec["grid"] = self._calculate_cv_score(
                 X, y, self.best_params_gec["grid"]
             )
             best_params_prep = copy.deepcopy(self.best_params_gec["search"])
             self.best_params_gec[
                 "grid_from_search"
@@ -638,221 +713,277 @@
                     self.best_score = score
                     self.best_params_ = self.best_params_gec[source]
 
         self._fit_best_params(X, y)
 
         return self
 
-    def _calculate_cv_score(self, X, y, params):
+    def _calculate_cv_score(
+        self,
+        X: ndarray,
+        y: ndarray,
+        params: Dict[str, Optional[Union[str, float, int, float64]]],
+    ) -> float64:
         clf = LGBMClassifier(**params)
         try:
             with open(os.devnull, "w") as f, contextlib.redirect_stdout(f):
-                cross_val_scores = cross_val_score(clf, X, y, cv=5, fit_params=self.fit_params)
+                cross_val_scores = cross_val_score(
+                    clf, X, y, cv=5, fit_params=self.fit_params
+                )
                 score = np.mean(cross_val_scores)
         except:
-            warnings.warn(f"Could not calculate cross val scores for parameters: {params}")
+            warnings.warn(
+                f"Could not calculate cross val scores for parameters: {params}"
+            )
             score = 0.0
         return score
 
-
     def _optimise_hyperparameters(
         self,
-        n_iter,
-        X,
-        Y,
-        best_score,
-        best_params,
+        n_iter: int,
+        X: ndarray,
+        Y: ndarray,
         **kwargs,
-    ):
+    ) -> Tuple[Dict[str, Optional[Union[int, float, str]]], float64]:
 
         if self.gec_hyperparameters["randomize"]:
             np.random.seed(int(datetime.now().timestamp() % 1 * 1e7))
 
-        for i in tqdm(list(range(n_iter))):
-            if (i + self.gec_iter) < min(
-                self.gec_hyperparameters["n_random_exploration"], int(n_iter / 2)
-            ):
-                selected_arm = np.random.choice(
-                    self._categorical_hyperparameter_combinations
-                )
-                random_combination = np.array(
-                    [
-                        np.random.choice(range_)
-                        for real_hyperparameter, range_ in self._real_hyperparameters_linear
-                    ]
-                )
-                arguments = self._build_arguments(
-                    selected_arm.split("-"), random_combination
-                )
-                selected_combination = random_combination
-                random_combination_bagging = self._bagging_combinations[
-                    np.random.choice(range(len(self._bagging_combinations)))
-                ]
+        n_random_exploration = min(
+            self.gec_hyperparameters["n_random_exploration"], int(n_iter / 2)
+        )
 
+        for i in tqdm(list(range(n_iter))):
+            if (i + self.gec_iter) < n_random_exploration:
                 (
-                    arguments["bagging_freq"],
-                    arguments["bagging_fraction"],
-                ) = random_combination_bagging
-                selected_combination_bagging = random_combination_bagging
+                    selected_arm,
+                    selected_combination,
+                    selected_combination_bagging,
+                    arguments,
+                ) = self._get_random_hyperparameter_configuration()
 
-                mean, sigma, mean_bagging, sigma_bagging = 0, 0, 0, 0
+                mean, sigma, mean_bagging, sigma_bagging = None, None, None, None
             else:
-                sampled_reward = np.array(
-                    [
-                        beta.rvs(reward["a"], reward["b"])
-                        for _, reward in self.rewards.items()
-                    ]
-                )
-                selected_arm_index = sampled_reward.argmax()
-                selected_arm = self._categorical_hyperparameter_combinations[
-                    selected_arm_index
-                ]
-
-
-                sets = np.array(
-                    [
-                        np.random.choice(
-                            range_, self.gec_hyperparameters["n_sample_initial"]
-                        )
-                        for _, range_ in self._real_hyperparameters_linear
-                    ]
-                )
-
-                if len(self.hyperparameter_scores["inputs"]):
-                    n_best = max(
-                        3, int(self.gec_iter * self.gec_hyperparameters["best_share"])
-                    )
-                    best_interactions = np.argsort(
-                        np.array(self.hyperparameter_scores["output"])
-                    )[::-1][:n_best]
-
-                    best_hyperparameters = np.array(
-                        self.hyperparameter_scores["inputs"]
-                    )[best_interactions, :]
-
-                    closest_hyperparameters = best_hyperparameters.dot(sets).argsort(1)[
-                        :, : self.gec_hyperparameters["n_sample"]
-                    ]
-                    selected_hyperparameter_indices = np.unique(
-                        closest_hyperparameters.flatten()
-                    )
-
-                    combinations = list(sets[:, selected_hyperparameter_indices].T)
-                else:
-                    combinations = list(sets[:, :self.gec_hyperparameters["n_sample"]].T)
-
-                assert len(combinations), sets
-
-                if len(self.hyperparameter_scores["inputs"]) > 0:
-                    self._fit_gaussian()
-
-                mean, sigma = self.gaussian.predict(combinations, return_std=True)
-
-                predicted_rewards = np.array(
-                    [
-                        scipy.stats.norm.ppf(
-                            self.gec_hyperparameters[
-                                "hyperparams_acquisition_percentile"
-                            ],
-                            loc=m,
-                            scale=s,
-                        )
-                        for m, s in zip(mean, sigma)
-                    ]
-                )
-
-                best_predicted_combination = combinations[np.argmax(predicted_rewards)]
-                selected_combination = best_predicted_combination
+                (
+                    selected_arm,
+                    selected_combination,
+                    mean,
+                    sigma,
+                ) = self._select_parameters()
                 arguments = self._build_arguments(
                     selected_arm.split("-"), selected_combination
                 )
 
                 if "yes_bagging" in selected_arm:
-                    if len(self.bagging_scores["inputs"]) > 0:
-                        self._fit_gaussian_bagging()
-                    mean_bagging, sigma_bagging = self.gaussian_bagging.predict(
-                        self._bagging_combinations_rescaled, return_std=True
-                    )
+                    (
+                        selected_combination_bagging,
+                        mean_bagging,
+                        sigma_bagging,
+                    ) = self._select_bagging_parameters()
 
-                    predicted_rewards_bagging = np.array(
-                        [
-                            scipy.stats.norm.ppf(
-                                self.gec_hyperparameters[
-                                    "bagging_acquisition_percentile"
-                                ],
-                                loc=m,
-                                scale=s,
-                            )
-                            for m, s in zip(mean_bagging, sigma_bagging)
-                        ]
-                    )
-                    best_predicted_combination_bagging = self._bagging_combinations[
-                        np.argmax(predicted_rewards_bagging)
-                    ]
-                    selected_combination_bagging = best_predicted_combination_bagging
                     (
                         arguments["bagging_freq"],
                         arguments["bagging_fraction"],
-                    ) = best_predicted_combination_bagging
+                    ) = selected_combination_bagging
 
             del arguments["bagging"]
             arguments["verbosity"] = -1
 
-            try:
-                score = self._calculate_cv_score(X, Y, arguments)
-                if np.isnan(score):
-                    score = 0
-
-                if best_score is None or score > best_score:
-                    best_score = score
-                    best_params = arguments
-
-                self.selected_arms.append(selected_arm)
-                self.hyperparameter_scores["inputs"].append(
-                    [float(f) for f in selected_combination]
+            score = self._calculate_cv_score(X, Y, arguments)
+
+            self._update_gec_fields(
+                score, arguments, selected_arm, selected_combination, mean, sigma
+            )
+
+            if "bagging_freq" in arguments:
+                self._update_gec_fields_bagging(
+                    score, selected_combination_bagging, mean_bagging, sigma_bagging
                 )
-                self.hyperparameter_scores["output"].append(score)
-                self.hyperparameter_scores["means"].append(mean)
-                self.hyperparameter_scores["sigmas"].append(sigma)
-
-                if "bagging_freq" in arguments:
-                    self.bagging_scores["inputs"].append(
-                        list(self._rescale_bagging_combination(*selected_combination_bagging))
-                    )
-                    self.bagging_scores["output"].append(score)
-                    self.bagging_scores["means"].append(mean_bagging)
-                    self.bagging_scores["sigmas"].append(sigma_bagging)
-
-                if self.best_score is not None:
-                    score_delta = score - self.best_score
-                    weighted_score_delta = (
-                        score_delta * self.gec_hyperparameters["bandit_greediness"]
-                    )
-                    if score_delta > 0:
-                        self.rewards[selected_arm]["a"] = (
-                            self.rewards[selected_arm]["a"] + weighted_score_delta
-                        )
-                        self.best_params_ = arguments
-                        self.best_score = score
-                    else:
-                        self.rewards[selected_arm]["b"] = (
-                            self.rewards[selected_arm]["b"] - weighted_score_delta
-                        )
-                else:
-                    self.best_score = score
-                    self.best_params_ = arguments
 
-            except Exception as e:
-                warnings.warn(f"These arguments led to an Error: {arguments}: {e}")
+        return (self.best_params_, self.best_score)
+
+    def _get_random_hyperparameter_configuration(
+        self,
+    ) -> Tuple[
+        str_,
+        ndarray,
+        Tuple[int, float64],
+        Dict[str, Optional[Union[str, float, int, float64]]],
+    ]:
+
+        selected_arm = np.random.choice(self._categorical_hyperparameter_combinations)
+        random_combination = np.array(
+            [
+                np.random.choice(range_)
+                for real_hyperparameter, range_ in self._real_hyperparameters_linear
+            ]
+        )
+        arguments = self._build_arguments(selected_arm.split("-"), random_combination)
+        selected_combination = random_combination
+        random_combination_bagging = self._bagging_combinations[
+            np.random.choice(range(len(self._bagging_combinations)))
+        ]
+
+        (
+            arguments["bagging_freq"],
+            arguments["bagging_fraction"],
+        ) = random_combination_bagging
+        selected_combination_bagging = random_combination_bagging
+
+        return (
+            selected_arm,
+            selected_combination,
+            selected_combination_bagging,
+            arguments,
+        )
+
+    def _select_parameters(self) -> Tuple[str, ndarray, ndarray, ndarray]:
+
+        sampled_reward = np.array(
+            [beta.rvs(reward["a"], reward["b"]) for _, reward in self.rewards.items()]
+        )
+        selected_arm_index = sampled_reward.argmax()
+        selected_arm = self._categorical_hyperparameter_combinations[selected_arm_index]
+
+        sets = np.array(
+            [
+                np.random.choice(range_, self.gec_hyperparameters["n_sample_initial"])
+                for _, range_ in self._real_hyperparameters_linear
+            ]
+        )
+
+        combinations = self._get_combinations_to_score(sets)
+
+        assert len(combinations), sets
+
+        if len(self.hyperparameter_scores["inputs"]) > 0:
+            self._fit_gaussian()
 
-        best_score = self._calculate_cv_score(X, Y, best_params)
+        mean, sigma = self.gaussian.predict(combinations, return_std=True)
+
+        predicted_rewards = np.array(
+            [
+                scipy.stats.norm.ppf(
+                    self.gec_hyperparameters["hyperparams_acquisition_percentile"],
+                    loc=m,
+                    scale=s,
+                )
+                for m, s in zip(mean, sigma)
+            ]
+        )
 
-        return (best_params, best_score)
+        selected_combination = combinations[np.argmax(predicted_rewards)]
 
-    def _build_arguments(self, categorical_combination, real_combination_linear):
+        return (selected_arm, selected_combination, mean, sigma)
+
+    def _get_combinations_to_score(self, sets: ndarray) -> List[ndarray]:
+        if len(self.hyperparameter_scores["inputs"]):
+            n_best = max(3, int(self.gec_iter * self.gec_hyperparameters["best_share"]))
+            best_interactions = np.argsort(
+                np.array(self.hyperparameter_scores["output"])
+            )[::-1][:n_best]
+
+            best_hyperparameters = np.array(self.hyperparameter_scores["inputs"])[
+                best_interactions, :
+            ]
+
+            closest_hyperparameters = best_hyperparameters.dot(sets).argsort(1)[
+                :, : self.gec_hyperparameters["n_sample"]
+            ]
+            selected_hyperparameter_indices = np.unique(
+                closest_hyperparameters.flatten()
+            )
+
+            combinations = list(sets[:, selected_hyperparameter_indices].T)
+        else:
+            combinations = list(sets[:, : self.gec_hyperparameters["n_sample"]].T)
+
+        return combinations
+
+    def _select_bagging_parameters(
+        self,
+    ) -> Tuple[Tuple[int, float64], ndarray, ndarray]:
+        if len(self.bagging_scores["inputs"]) > 0:
+            self._fit_gaussian_bagging()
+        mean_bagging, sigma_bagging = self.gaussian_bagging.predict(
+            self._bagging_combinations_rescaled, return_std=True
+        )
+
+        predicted_rewards_bagging = np.array(
+            [
+                scipy.stats.norm.ppf(
+                    self.gec_hyperparameters["bagging_acquisition_percentile"],
+                    loc=m,
+                    scale=s,
+                )
+                for m, s in zip(mean_bagging, sigma_bagging)
+            ]
+        )
+        best_predicted_combination_bagging = self._bagging_combinations[
+            np.argmax(predicted_rewards_bagging)
+        ]
+        return (best_predicted_combination_bagging, mean_bagging, sigma_bagging)
+
+    def _update_gec_fields(
+        self,
+        score: float64,
+        arguments: Dict[str, Optional[Union[str, float, int, float64]]],
+        selected_arm: Union[str, str_],
+        selected_combination: ndarray,
+        mean: Optional[ndarray],
+        sigma: Optional[ndarray],
+    ) -> None:
+
+        self.selected_arms.append(selected_arm)
+        self.hyperparameter_scores["inputs"].append(
+            [float(f) for f in selected_combination]
+        )
+        self.hyperparameter_scores["output"].append(score)
+
+        if mean is not None:
+            self.hyperparameter_scores["means"].append(mean)
+            self.hyperparameter_scores["sigmas"].append(sigma)
+
+        if self.best_score is not None:
+            score_delta = score - self.best_score
+            weighted_score_delta = (
+                score_delta * self.gec_hyperparameters["bandit_greediness"]
+            )
+            if score_delta > 0:
+                self.rewards[selected_arm]["a"] = (
+                    self.rewards[selected_arm]["a"] + weighted_score_delta
+                )
+                self.best_params_ = arguments
+                self.best_score = score
+            else:
+                self.rewards[selected_arm]["b"] = (
+                    self.rewards[selected_arm]["b"] - weighted_score_delta
+                )
+        else:
+            self.best_score = score
+            self.best_params_ = arguments
+
+    def _update_gec_fields_bagging(
+        self,
+        score: float64,
+        selected_combination_bagging: Tuple[int, float64],
+        mean_bagging: Optional[ndarray],
+        sigma_bagging: Optional[ndarray],
+    ) -> None:
+        self.bagging_scores["inputs"].append(
+            list(self._rescale_bagging_combination(*selected_combination_bagging))
+        )
+        self.bagging_scores["output"].append(score)
+        if mean_bagging is not None:
+            self.bagging_scores["means"].append(mean_bagging)
+            self.bagging_scores["sigmas"].append(sigma_bagging)
+
+    def _build_arguments(
+        self, categorical_combination: List[str], real_combination_linear: ndarray
+    ) -> Dict[str, Optional[Union[int, float, str]]]:
         best_predicted_combination_converted = [
             self._real_hyperparameters_map[name][value]
             for name, value in zip(
                 self._real_hyperparameter_names,
                 real_combination_linear,
             )
         ]
@@ -868,49 +999,57 @@
         arguments = dict(
             zip(
                 self._categorical_hyperparameter_names
                 + self._real_hyperparameter_names,
                 hyperparameter_values,
             )
         )
-        return {**arguments, **self.fixed_params,  **self._init_args, **self._init_kwargs}
+        return {
+            **arguments,
+            **self.fixed_params,
+            **self._init_args,
+            **self._init_kwargs,
+        }
 
-    def _fit_best_params(self, X, y):
+    def _fit_best_params(self, X: ndarray, y: ndarray) -> None:
 
         if hasattr(self, "best_params_") and self.best_params_ is not None:
             for k, v in self.best_params_.items():
                 setattr(self, k, v)
             setattr(self, "random_state", 101)
 
         super().fit(X, y, **self.fit_params)
 
-    def _fit_gaussian(self):
+    def _fit_gaussian(self) -> None:
         self.gaussian.fit(
             np.array(self.hyperparameter_scores["inputs"]),
-            np.array(self.hyperparameter_scores["output"]) - np.mean(self.hyperparameter_scores["output"]),
+            np.array(self.hyperparameter_scores["output"])
+            - np.mean(self.hyperparameter_scores["output"]),
         )
 
-    def _fit_gaussian_bagging(self):
+    def _fit_gaussian_bagging(self) -> None:
         self.gaussian_bagging.fit(
             np.array(self.bagging_scores["inputs"]),
-            np.array(self.bagging_scores["output"]) - np.mean(self.bagging_scores["output"]),
+            np.array(self.bagging_scores["output"])
+            - np.mean(self.bagging_scores["output"]),
         )
 
-    def _get_best_arm(self):
+    def _get_best_arm(self) -> str:
         mean_reward = np.array(
             [
-                reward["a"]/ ( reward["a"] + reward["b"])
+                reward["a"] / (reward["a"] + reward["b"])
                 for _, reward in self.rewards.items()
             ]
         )
         best_arm = self._categorical_hyperparameter_combinations[mean_reward.argmax()]
-        return(best_arm)
-
+        return best_arm
 
-    def _find_best_parameters(self, step_sizes=[16, 8, 4, 2, 1]):
+    def _find_best_parameters(
+        self, step_sizes: List[int] = [16, 8, 4, 2, 1]
+    ) -> Dict[str, Optional[Union[int, float, str]]]:
 
         best_arm = self._get_best_arm()
 
         self._fit_gaussian()
         sets = [
             list(range_[:: step_sizes[0]]) + [range_[-1]]
             for range_ in self._real_hyperparameter_ranges
@@ -921,15 +1060,17 @@
 
         best_params = self._find_best_parameters_from_initial_parameters(
             best_arm, best_combination, step_sizes
         )
 
         return best_params
 
-    def _find_best_parameters_from_search(self, params):
+    def _find_best_parameters_from_search(
+        self, params: Dict[str, Optional[Union[int, float, str]]]
+    ) -> Dict[str, Optional[Union[int, float, str]]]:
         self._fit_gaussian()
 
         if "bagging_freq" in params:
             del params["bagging_freq"]
             del params["bagging_fraction"]
             bagging = "yes_bagging"
         else:
@@ -942,71 +1083,77 @@
             for name in self._real_hyperparameter_names
         ]
         best_params = self._find_best_parameters_from_initial_parameters(
             best_arm,
             best_params_linear_values,
             step_sizes=[4, 2, 1],
         )
-        
+
         return best_params
 
-    def _find_best_parameters_iter(self, combinations):
+    def _find_best_parameters_iter(
+        self, combinations: ndarray
+    ) -> Tuple[ndarray, float64]:
 
         mean = self.gaussian.predict(combinations)
         best_score = np.max(mean)
         best_combination = combinations[np.argmax(mean)]
 
         return best_combination, best_score
 
     def _find_best_parameters_from_initial_parameters(
-        self, best_arm, best_combination, step_sizes
-    ):
+        self,
+        best_arm: str,
+        best_combination: Union[List[float16], ndarray],
+        step_sizes: List[int],
+    ) -> Dict[str, Optional[Union[int, float, str]]]:
         for step_size, previous_step_size in zip(step_sizes[1:], step_sizes[:-1]):
 
             neighbouring_combinations = self._get_neighbouring_combinations(
                 best_combination, step_size, previous_step_size
             )
 
             new_ranges = [
-                (name, min(r), max(r)) for name, r in
-                zip(
-                    self._real_hyperparameter_names,
-                    neighbouring_combinations
+                (name, min(r), max(r))
+                for name, r in zip(
+                    self._real_hyperparameter_names, neighbouring_combinations
                 )
             ]
-            #log.info(new_ranges)
+            # log.info(new_ranges)
 
             best_combination, best_score = self._find_best_parameters_iter(
                 neighbouring_combinations
             )
 
-
-        arguments = self._build_arguments(
-            best_arm.split("-"), best_combination
-        )
+        arguments = self._build_arguments(best_arm.split("-"), best_combination)
 
         if "yes_bagging" in best_arm:
             self._fit_gaussian_bagging()
-            mean_bagging = self.gaussian_bagging.predict(self._bagging_combinations_rescaled)
+            mean_bagging = self.gaussian_bagging.predict(
+                self._bagging_combinations_rescaled
+            )
             best_predicted_combination_bagging = self._bagging_combinations[
                 np.argmax(mean_bagging)
             ]
 
             (
                 arguments["bagging_freq"],
                 arguments["bagging_fraction"],
             ) = best_predicted_combination_bagging
 
         del arguments["bagging"]
 
         return arguments
 
     def _get_neighbouring_combinations(
-        self, best_combination, step_size, previous_step_size
-    ):
+        self,
+        best_combination: Union[List[float16], ndarray],
+        step_size: int,
+        previous_step_size: int,
+    ) -> ndarray:
         new_sets = []
         for real_value, range_ in zip(
             best_combination, self._real_hyperparameter_ranges
         ):
             real_value_index = np.argmax(range_ == real_value)
 
             start_index = real_value_index - previous_step_size
@@ -1016,15 +1163,15 @@
             adjusted_step_size = min(int(len(range_) / 2), step_size)
             new_set = list(range_[start_index:end_index:adjusted_step_size])
             if np.max(new_set) < real_value:
                 new_set.append(real_value)
 
             new_sets.append(new_set)
         neighbouring_combinations = np.array(list(itertools.product(*new_sets)))
-    
+
         return neighbouring_combinations
 
     def save_plots(self, path_stem):
         """Create and save plots that summarise GEC trajectory
 
         Parameters
         ----------
@@ -1034,15 +1181,15 @@
         figs = self.plot_gec()
         self._write_figures(figs, path_stem)
 
     def _write_figures(self, figs, path_stem):
         for plot_name, fig in figs.items():
             fig.savefig(f"{path_stem}_{plot_name}.png")
 
-    def plot_gec(self):
+    def plot_gec(self) -> Dict[str, Figure]:
         """Create figures to summarise GEC trajectory
 
         Returns
         -------
             figs : dict[str, fig]
                 a dictionary of figures
         """
@@ -1050,52 +1197,46 @@
         figs = {}
 
         fig, axes = plt.subplots(
             nrows=2, ncols=2, sharex=True, sharey=False, figsize=(12, 12)
         )
         ax1, ax2, ax3, ax4 = axes.flatten()
 
-        x = np.arange(
-            len(self.hyperparameter_scores["means"])
-        )
+        x = np.arange(len(self.hyperparameter_scores["means"]))
         self._plot_mean_prediction_and_mean_variance(ax1, x)
         self._plot_prediction_std_and_variance_std(ax2, x)
         self._plot_prediction_mean_variance_correlation(ax3, x)
-        self._plot_linear_scaled_parameter_samples(ax4, x)
+        self._plot_linear_scaled_parameter_samples(ax4)
 
         figs["parameters"] = fig
 
         fig2 = self._plot_boosting_parameter_surface()
         figs["bagging"] = fig2
 
         return figs
 
-    def _plot_mean_prediction_and_mean_variance(self, ax, x):
-        gp_mean_prediction = [
-            np.mean(x) for x in self.hyperparameter_scores["means"]
-        ]
+    def _plot_mean_prediction_and_mean_variance(self, ax: Axes, x: ndarray) -> None:
+        gp_mean_prediction = [np.mean(x) for x in self.hyperparameter_scores["means"]]
         gp_mean_sigma = [np.mean(x) for x in self.hyperparameter_scores["sigmas"]]
 
         ax.plot(x, gp_mean_prediction, label="mean_prediction")
         ax.plot(x, gp_mean_sigma, label="mean_sigma")
         ax.legend(loc="upper right")
 
-    def _plot_prediction_std_and_variance_std(self, ax, x):
+    def _plot_prediction_std_and_variance_std(self, ax: Axes, x: ndarray) -> None:
         gp_prediction_variance = [
             np.std(x) for x in self.hyperparameter_scores["means"]
         ]
-        gp_sigma_variance = [
-            np.std(x) for x in self.hyperparameter_scores["sigmas"]
-        ]
+        gp_sigma_variance = [np.std(x) for x in self.hyperparameter_scores["sigmas"]]
 
         ax.plot(x, gp_prediction_variance, label="prediction_variance")
         ax.plot(x, gp_sigma_variance, label="sigma_variance")
         ax.legend(loc="lower right")
 
-    def _plot_prediction_mean_variance_correlation(self, ax, x):
+    def _plot_prediction_mean_variance_correlation(self, ax: Axes, x: ndarray) -> None:
         correlation = [
             np.corrcoef(
                 self.hyperparameter_scores["means"][i],
                 self.hyperparameter_scores["sigmas"][i],
             )[0, 1]
             for i in x
         ]
@@ -1103,31 +1244,32 @@
         ax.plot(
             x,
             correlation,
             label="corr(preds mean, preds variance)",
         )
         ax.legend(loc="lower right")
 
-    def _plot_linear_scaled_parameter_samples(self, ax, x):
+    def _plot_linear_scaled_parameter_samples(self, ax: Axes) -> None:
         inputs_ = np.array(self.hyperparameter_scores["inputs"])
+        x = np.arange(inputs_.shape[0])
         assert (
-            (len(self._real_hyperparameter_names) == inputs_.shape[1]), 
-            f"{len(self._real_hyperparameter_names)}!={inputs_.shape[1]}"
+            (len(self._real_hyperparameter_names) == inputs_.shape[1]),
+            f"{len(self._real_hyperparameter_names)}!={inputs_.shape[1]}",
         )
         for i in range(inputs_.shape[1]):
             ax.plot(x, inputs_[:, i], label=self._real_hyperparameter_names[i])
 
     def _plot_boosting_parameter_surface(
         self,
-        plot_bounds=True,
-    ):
+        plot_bounds: bool = True,
+    ) -> Figure:
         self._fit_gaussian_bagging()
 
-        X_range = np.array(self._bagging_combinations_rescaled)[0,:]
-        Y_range = np.array(self._bagging_combinations_rescaled)[1,:]
+        X_range = np.array(self._bagging_combinations_rescaled)[0, :]
+        Y_range = np.array(self._bagging_combinations_rescaled)[1, :]
         Z_range = np.arange(-0.5, 1.5, 0.1)
 
         fig, ax = plt.subplots(subplot_kw={"projection": "3d"}, figsize=(12, 12))
 
         # Make data.
         X = np.arange(
             np.min(X_range), np.max(X_range), (np.max(X_range) - np.min(X_range)) / 100
```

### Comparing `gecs-0.28.3/src/gecs/utils/gaussian_process_visualisation.py` & `gecs-0.29.0/src/gecs/utils/gaussian_process_visualisation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,67 @@
 import matplotlib.pyplot as plt
+import numpy as np
 from matplotlib import cm
 from matplotlib.ticker import LinearLocator
 from sklearn.utils.extmath import cartesian
-import numpy as np
+
 
 def visualise_1D_gaussian_process(gaussian):
     x = np.atleast_2d(np.linspace(0, 10, 100)).T
     y_pred, sigma = gaussian.predict(x, return_std=True)
     plt.figure(figsize=(15, 15))
-    plt.plot(x, y_pred, 'b-', label='Prediction')
+    plt.plot(x, y_pred, "b-", label="Prediction")
 
-    plt.fill(np.concatenate([x, x[::-1]]),
-             np.concatenate([y_pred - 1.9600 * sigma,
-                            (y_pred + 1.9600 * sigma)[::-1]]),
-             alpha=.5, fc='b', ec='None', label='95% confidence interval')
+    plt.fill(
+        np.concatenate([x, x[::-1]]),
+        np.concatenate([y_pred - 1.9600 * sigma, (y_pred + 1.9600 * sigma)[::-1]]),
+        alpha=0.5,
+        fc="b",
+        ec="None",
+        label="95% confidence interval",
+    )
     plt.show()
 
 
-def visualise_2D_gaussian_process(gaussian, X_range=np.arange(0, 10, 0.1), Y_range=np.arange(0, 10, 0.1), Z_range=np.arange(-3, 3, 1), plot_bounds=True):
+def visualise_2D_gaussian_process(
+    gaussian,
+    X_range=np.arange(0, 10, 0.1),
+    Y_range=np.arange(0, 10, 0.1),
+    Z_range=np.arange(-3, 3, 1),
+    plot_bounds=True,
+):
     fig, ax = plt.subplots(subplot_kw={"projection": "3d"}, figsize=(15, 15))
 
     # Make data.
-    X = np.arange(np.min(X_range), np.max(X_range), (np.max(X_range)-np.min(X_range))/100)
-    Y = np.arange(np.min(Y_range), np.max(Y_range), (np.max(Y_range)-np.min(Y_range))/100)
-    Z = np.arange(np.min(Z_range), np.max(Z_range), (np.max(Z_range)-np.min(Z_range))/100)
+    X = np.arange(
+        np.min(X_range), np.max(X_range), (np.max(X_range) - np.min(X_range)) / 100
+    )
+    Y = np.arange(
+        np.min(Y_range), np.max(Y_range), (np.max(Y_range) - np.min(Y_range)) / 100
+    )
+    Z = np.arange(
+        np.min(Z_range), np.max(Z_range), (np.max(Z_range) - np.min(Z_range)) / 100
+    )
     R = cartesian(np.array([X, Y]))
     X, Y = np.meshgrid(X, Y)
     Z, sigma = gaussian.predict(R, return_std=True)
     Z = Z.reshape((100, 100))
     sigma = sigma.reshape((100, 100))
 
     # Plot the surface.
-    surf = ax.plot_surface(X, Y, Z, cmap=cm.coolwarm,
-                           linewidth=0, antialiased=False)
+    surf = ax.plot_surface(X, Y, Z, cmap=cm.coolwarm, linewidth=0, antialiased=False)
     if plot_bounds:
-        surf2 = ax.plot_surface(X, Y, Z + 1.9600*sigma, alpha=0.2,
-                               linewidth=0, antialiased=False)
-        surf3 = ax.plot_surface(X, Y, Z - 1.9600*sigma, alpha=0.2,
-                               linewidth=0, antialiased=False)
+        surf2 = ax.plot_surface(
+            X, Y, Z + 1.9600 * sigma, alpha=0.2, linewidth=0, antialiased=False
+        )
+        surf3 = ax.plot_surface(
+            X, Y, Z - 1.9600 * sigma, alpha=0.2, linewidth=0, antialiased=False
+        )
     # Customize the z axis.
     ax.set_zlim(np.min(Z_range), np.max(Z_range))
     ax.zaxis.set_major_locator(LinearLocator(10))
     # A StrMethodFormatter is used automatically
-    ax.zaxis.set_major_formatter('{x:.02f}')
+    ax.zaxis.set_major_formatter("{x:.02f}")
     # Add a color bar which maps values to colors.
     fig.colorbar(surf, shrink=0.5, aspect=5)
 
-    plt.show()
+    plt.show()
```

### Comparing `gecs-0.28.3/setup.py` & `gecs-0.29.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'scikit-learn==1.2.2',
  'scipy==1.10.1',
  'tqdm==4.65.0',
  'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'gecs',
-    'version': '0.28.3',
+    'version': '0.29.0',
     'description': 'LightGBM Classifier with integrated bayesian hyperparameter optimization',
     'long_description': "![a gecko looking at the camera with bayesian math in white on a pink and green background](documentation/assets/header.png)\n\n\n# (100)gecs\n\nBayesian hyperparameter tuning for LGBMClassifier with a scikit-learn API\n\n## Table of Contents\n\n- [Project Overview](#project-overview)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Project Overview\n\nThe package `gecs` provides the class `GEC`, which is a child class of the class `LGBMClassifier` from the package `lightgbm`. It can be imported from `gecs.gec` and then used in place of `LGBMClassifier`, with the same API. The difference to `LGBMClassifier` lies in the fact that `GEC`automatically does bayesian hyperparameter optimization of the parameters `learning_rate`, `reg_alpha`, `reg_lambda`, `min_child_samples`, `min_child_weight`, `colsample_bytree` and optionally also of `num_leaves` and `n_estimators`.\n\nThe fit method has two new parameters: `n_iter`, which sets the number of hyperparameter combinations that will be tried (the higher `n_iter` the higher the expected accuracy, but at a cost of compute) and `fixed_hyperparameters`, which determines which hyperparameters of the LGBM classifier won't get optimized. By default, these are `n_estimators` and `num_leaves`, as the highest possible value for these hyperparameters is almost always optimal. The idea then is to set these as high as makes sense in a specific context and then optimize the other hyperparameters.\n\n\n## Installation\n\n    pip install gecs\n\n## Usage\n\n    from gecs.gec import GEC\n\n    gec.fit(X, y)\n\n    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes\n\n    gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier\n\n    yhat = gec.predict(X)\n\n    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier\n    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation\n\n\n    \n\n\n\n## Contributing\n\nIf you want to contribute, please reach out and I'll design a process around it.\n\n## License\n\nMIT\n\n## Contact Information\n\nYou can find my contact information on my website: [https://leonluithlen.eu](https://leonluithlen.eu)",
     'author': 'Leon Luithlen',
     'author_email': 'leontimnaluithlen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xideas/sequifier',
```

### Comparing `gecs-0.28.3/PKG-INFO` & `gecs-0.29.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecs
-Version: 0.28.3
+Version: 0.29.0
 Summary: LightGBM Classifier with integrated bayesian hyperparameter optimization
 Home-page: https://github.com/0xideas/sequifier
 License: MIT
 Keywords: lightgbm,classification,machine learning,hyperparameter optimization,classifier
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.10.0,<3.11.0
```

