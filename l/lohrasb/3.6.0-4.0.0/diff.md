# Comparing `tmp/lohrasb-3.6.0.tar.gz` & `tmp/lohrasb-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lohrasb-3.6.0.tar", max compression
+gzip compressed data, was "lohrasb-4.0.0.tar", max compression
```

## Comparing `lohrasb-3.6.0.tar` & `lohrasb-4.0.0.tar`

### file list

```diff
@@ -1,34 +1,42 @@
--rw-r--r--   0        0        0     1323 2023-04-26 04:35:26.907410 lohrasb-3.6.0/LICENSE
--rw-r--r--   0        0        0    19279 2023-04-26 04:35:26.907777 lohrasb-3.6.0/README.md
--rw-r--r--   0        0        0       67 2023-04-26 04:35:26.929046 lohrasb-3.6.0/lohrasb/.env
--rw-r--r--   0        0        0     1373 2023-05-16 18:52:18.222362 lohrasb-3.6.0/lohrasb/__init__.py
--rw-r--r--   0        0        0      326 2023-04-26 04:35:26.929622 lohrasb-3.6.0/lohrasb/abstracts/estimators.py
--rw-r--r--   0        0        0      784 2023-04-26 04:35:26.929877 lohrasb-3.6.0/lohrasb/abstracts/optimizers.py
--rw-r--r--   0        0        0    69902 2023-05-03 16:37:24.354889 lohrasb-3.6.0/lohrasb/base_classes/optimizer_bases.py
--rw-r--r--   0        0        0   108969 2023-05-03 16:37:24.356088 lohrasb-3.6.0/lohrasb/best_estimator.py
--rw-r--r--   0        0        0      695 2023-04-26 04:35:26.931894 lohrasb-3.6.0/lohrasb/config.yaml
--rw-r--r--   0        0        0      405 2023-04-26 04:35:26.932370 lohrasb-3.6.0/lohrasb/decorators/decorators.py
--rw-r--r--   0        0        0        0 2023-04-26 04:35:26.932782 lohrasb-3.6.0/lohrasb/examples/__init__.py
--rw-r--r--   0        0        0    44737 2023-05-16 18:43:38.063534 lohrasb-3.6.0/lohrasb/examples/classification_gridsearch.ipynb
--rw-r--r--   0        0        0  4719592 2023-05-16 18:43:38.089872 lohrasb-3.6.0/lohrasb/examples/classification_gridsearch_interpretml_shapkernel.ipynb
--rw-r--r--   0        0        0    72836 2023-05-03 16:37:24.387040 lohrasb-3.6.0/lohrasb/examples/classification_optuna.ipynb
--rw-r--r--   0        0        0    54881 2023-04-26 04:35:26.999939 lohrasb-3.6.0/lohrasb/examples/classification_optuna_interpretml.ipynb
--rw-r--r--   0        0        0    36142 2023-05-03 16:37:24.388135 lohrasb-3.6.0/lohrasb/examples/classification_randomsearch.ipynb
--rw-r--r--   0        0        0    16972 2023-04-26 04:35:27.000539 lohrasb-3.6.0/lohrasb/examples/classification_randomsearch_multi_class.ipynb
--rw-r--r--   0        0        0    72830 2023-04-26 04:35:27.001019 lohrasb-3.6.0/lohrasb/examples/classification_ray_tunegridsearch.ipynb
--rw-r--r--   0        0        0    80165 2023-04-26 04:35:27.001245 lohrasb-3.6.0/lohrasb/examples/classification_ray_tunesearch.ipynb
--rw-r--r--   0        0        0    34631 2023-05-16 18:43:38.091286 lohrasb-3.6.0/lohrasb/examples/lohrasb.log
--rw-r--r--   0        0        0    40666 2023-05-03 16:37:24.389472 lohrasb-3.6.0/lohrasb/examples/regression_optuna.ipynb
--rw-r--r--   0        0        0   561335 2023-04-26 04:35:27.022424 lohrasb-3.6.0/lohrasb/examples/regression_optuna_interpretml.ipynb
--rw-r--r--   0        0        0    16470 2023-04-26 04:35:27.023516 lohrasb-3.6.0/lohrasb/examples/xgboost_survival_embeddings.ipynb
--rw-r--r--   0        0        0      414 2023-04-26 04:35:27.024016 lohrasb-3.6.0/lohrasb/factories/factories.py
--rw-r--r--   0        0        0        0 2023-04-26 04:35:27.024865 lohrasb-3.6.0/lohrasb/mediators/mediators.py
--rw-r--r--   0        0        0       96 2023-04-26 04:35:27.044004 lohrasb-3.6.0/lohrasb/model_conf.py
--rw-r--r--   0        0        0       95 2023-04-26 04:35:27.044679 lohrasb-3.6.0/lohrasb/project_conf.py
--rw-r--r--   0        0        0        0 2023-04-26 04:35:27.044969 lohrasb-3.6.0/lohrasb/utils/__init__.py
--rw-r--r--   0        0        0     4652 2023-04-26 04:35:27.045282 lohrasb-3.6.0/lohrasb/utils/helper_funcs.py
--rw-r--r--   0        0        0    18032 2023-04-26 04:35:27.045756 lohrasb-3.6.0/lohrasb/utils/metrics.py
--rw-r--r--   0        0        0       40 2023-05-16 18:52:18.222362 lohrasb-3.6.0/lohrasb/version.py
--rw-r--r--   0        0        0     1255 2023-05-16 18:52:18.223362 lohrasb-3.6.0/pyproject.toml
--rw-r--r--   0        0        0    21527 1970-01-01 00:00:00.000000 lohrasb-3.6.0/setup.py
--rw-r--r--   0        0        0    20786 1970-01-01 00:00:00.000000 lohrasb-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1323 2023-07-11 17:00:37.562579 lohrasb-4.0.0/LICENSE
+-rw-r--r--   0        0        0    38999 2023-07-11 17:00:37.563042 lohrasb-4.0.0/README.md
+-rw-r--r--   0        0        0       67 2023-07-11 17:00:37.564140 lohrasb-4.0.0/lohrasb/.env
+-rw-r--r--   0        0        0     1391 2023-07-11 17:00:37.564289 lohrasb-4.0.0/lohrasb/__init__.py
+-rw-r--r--   0        0        0      326 2023-07-11 17:00:37.564654 lohrasb-4.0.0/lohrasb/abstracts/estimators.py
+-rw-r--r--   0        0        0     2019 2023-07-11 17:00:37.564886 lohrasb-4.0.0/lohrasb/abstracts/optimizers.py
+-rw-r--r--   0        0        0    51341 2023-07-11 17:00:37.566268 lohrasb-4.0.0/lohrasb/base_classes/optimizer_bases.py
+-rw-r--r--   0        0        0    39131 2023-07-11 17:00:37.567093 lohrasb-4.0.0/lohrasb/best_estimator.py
+-rw-r--r--   0        0        0      695 2023-07-11 17:00:37.567331 lohrasb-4.0.0/lohrasb/config.yaml
+-rw-r--r--   0        0        0      405 2023-07-11 17:00:37.567581 lohrasb-4.0.0/lohrasb/decorators/decorators.py
+-rw-r--r--   0        0        0        0 2023-07-11 17:00:37.567709 lohrasb-4.0.0/lohrasb/examples/__init__.py
+-rw-r--r--   0        0        0    71027 2023-07-11 17:00:37.568596 lohrasb-4.0.0/lohrasb/examples/classification_gridsearch.ipynb
+-rw-r--r--   0        0        0   314630 2023-07-11 17:00:37.589575 lohrasb-4.0.0/lohrasb/examples/classification_gridsearch_interpretml_shapkernel.ipynb
+-rw-r--r--   0        0        0    45593 2023-07-11 17:00:37.590288 lohrasb-4.0.0/lohrasb/examples/classification_optuna.ipynb
+-rw-r--r--   0        0        0    44110 2023-07-11 17:00:37.590663 lohrasb-4.0.0/lohrasb/examples/classification_optuna_interpretml.ipynb
+-rw-r--r--   0        0        0    55844 2023-07-11 17:00:37.590856 lohrasb-4.0.0/lohrasb/examples/classification_optunacvsearch.ipynb
+-rw-r--r--   0        0        0    47551 2023-07-11 17:00:37.591134 lohrasb-4.0.0/lohrasb/examples/classification_randomsearch.ipynb
+-rw-r--r--   0        0        0  1209066 2023-07-11 17:00:37.597961 lohrasb-4.0.0/lohrasb/examples/classification_randomsearch_multi_class.ipynb
+-rw-r--r--   0        0        0    41991 2023-07-11 17:00:37.598523 lohrasb-4.0.0/lohrasb/examples/classification_ray_tunegridsearch.ipynb
+-rw-r--r--   0        0        0    43147 2023-07-11 17:00:37.598722 lohrasb-4.0.0/lohrasb/examples/classification_ray_tunesearch.ipynb
+-rw-r--r--   0        0        0    46101 2023-07-11 17:00:37.598892 lohrasb-4.0.0/lohrasb/examples/classification_tune.ipynb
+-rw-r--r--   0        0        0    41677 2023-07-11 17:00:37.599107 lohrasb-4.0.0/lohrasb/examples/lohrasb.log
+-rw-r--r--   0        0        0     2899 2023-07-11 17:00:37.599269 lohrasb-4.0.0/lohrasb/examples/optimize_by_gridsearchcv_examples.py
+-rw-r--r--   0        0        0     4414 2023-07-11 17:00:37.599419 lohrasb-4.0.0/lohrasb/examples/optimize_by_optunasearch_examples.py
+-rw-r--r--   0        0        0     2964 2023-07-11 17:00:37.599580 lohrasb-4.0.0/lohrasb/examples/optimize_by_optunasearchcv_examples.py
+-rw-r--r--   0        0        0     2881 2023-07-11 17:00:37.599696 lohrasb-4.0.0/lohrasb/examples/optimize_by_randomsearchcv_examples.py
+-rw-r--r--   0        0        0     4911 2023-07-11 17:00:37.599971 lohrasb-4.0.0/lohrasb/examples/optimize_by_tune_examples.py
+-rw-r--r--   0        0        0     2816 2023-07-11 17:00:37.600182 lohrasb-4.0.0/lohrasb/examples/optimize_by_tunegridsearchcv_examples.py
+-rw-r--r--   0        0        0     3547 2023-07-11 17:00:37.600373 lohrasb-4.0.0/lohrasb/examples/optimize_by_tunesearchcv_examples.py
+-rw-r--r--   0        0        0    39209 2023-07-11 17:00:37.600656 lohrasb-4.0.0/lohrasb/examples/regression_optuna.ipynb
+-rw-r--r--   0        0        0    99015 2023-07-11 17:00:37.601005 lohrasb-4.0.0/lohrasb/examples/regression_optuna_interpretml.ipynb
+-rw-r--r--   0        0        0    19224 2023-07-11 17:00:37.601370 lohrasb-4.0.0/lohrasb/examples/xgboost_survival_embeddings.ipynb
+-rw-r--r--   0        0        0      414 2023-07-11 17:00:37.601665 lohrasb-4.0.0/lohrasb/factories/factories.py
+-rw-r--r--   0        0        0       26 2023-07-11 17:00:37.602762 lohrasb-4.0.0/lohrasb/mediators/mediators.py
+-rw-r--r--   0        0        0       95 2023-07-11 17:00:37.602956 lohrasb-4.0.0/lohrasb/project_conf.py
+-rw-r--r--   0        0        0    25512 2023-07-11 17:00:37.603156 lohrasb-4.0.0/lohrasb/tests_conf.py
+-rw-r--r--   0        0        0        0 2023-07-11 17:00:37.603292 lohrasb-4.0.0/lohrasb/utils/__init__.py
+-rw-r--r--   0        0        0     5924 2023-07-11 17:00:37.603433 lohrasb-4.0.0/lohrasb/utils/helper_funcs.py
+-rw-r--r--   0        0        0    23061 2023-07-11 17:00:37.603702 lohrasb-4.0.0/lohrasb/utils/metrics.py
+-rw-r--r--   0        0        0       40 2023-07-11 17:00:37.603865 lohrasb-4.0.0/lohrasb/version.py
+-rw-r--r--   0        0        0     1615 2023-07-11 17:00:37.607413 lohrasb-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    40905 1970-01-01 00:00:00.000000 lohrasb-4.0.0/PKG-INFO
```

### Comparing `lohrasb-3.6.0/LICENSE` & `lohrasb-4.0.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2022, fuzzylearning
+Copyright (c) 2022, TorkamaniLab 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `lohrasb-3.6.0/lohrasb/__init__.py` & `lohrasb-4.0.0/lohrasb/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.6.0"
+__version__ = "4.0.0"
 
 import logging
 import logging.config
 import os
 from pathlib import Path, PurePath
 
 import ray
@@ -40,16 +40,16 @@
 
 else:
     print("default logger setting is applied !")
     logging.basicConfig(level=DEFAULT_LEVEL)
     logger = logging.getLogger()
 
 
-# Use Ray to accelerate computing
-try:
-    # Try to connect to Ray cluster.
-    ray.init(address="auto", ignore_reinit_error=True)
-    logger.info("Connected to Ray cluster!")
-except Exception as e:
-    # If connection fails, start Ray locally.
-    ray.init()
-    logger.warning("This error happened {e}. So Ray Started locally.")
+# # Use Ray to accelerate computing
+# try:
+#     # Try to connect to Ray cluster.
+#     ray.init(address="auto", ignore_reinit_error=True)
+#     logger.info("Connected to Ray cluster!")
+# except Exception as e:
+#     # If connection fails, start Ray locally.
+#     ray.init()
+#     logger.warning("This error happened {e}. So Ray Started locally.")
```

### Comparing `lohrasb-3.6.0/lohrasb/config.yaml` & `lohrasb-4.0.0/lohrasb/config.yaml`

 * *Files identical despite different names*

### Comparing `lohrasb-3.6.0/lohrasb/examples/classification_gridsearch.ipynb` & `lohrasb-4.0.0/lohrasb/examples/classification_ray_tunegridsearch.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9902856671701386%*

 * *Differences: {"'cells'": "{0: {'outputs': {0: {'text': ['2023-07-07 13:43:35,845 :: matplotlib :: matplotlib "*

 * *            'data path: '*

 * *            "/Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\\n', "*

 * *            "'2023-07-07 13:43:35,850 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\\n', "*

 * *            "'2023-07-07 13:43:35,853 :: matplotlib :: interactive is False\\n', '2023-07-07 "*

 * *            '13:43:35,854 :: matplotlib :: platform is darwin\\n\', "2023-07-07 13 […]*

```diff
@@ -5,22 +5,40 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2023-05-16 10:27:21,069 :: dev :: Connected to Ray cluster!\n",
-                        "2023-05-16 10:27:21,069 :: dev :: Connected to Ray cluster!\n",
-                        "2023-05-16 10:27:21,341 :: matplotlib :: matplotlib data path: /Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\n",
-                        "2023-05-16 10:27:21,347 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\n",
-                        "2023-05-16 10:27:21,350 :: matplotlib :: interactive is False\n",
-                        "2023-05-16 10:27:21,351 :: matplotlib :: platform is darwin\n",
-                        "2023-05-16 10:27:22,101 :: matplotlib :: CACHEDIR=/Users/hjavedani/.matplotlib\n",
-                        "2023-05-16 10:27:22,105 :: matplotlib.font_manager :: Using fontManager instance from /Users/hjavedani/.matplotlib/fontlist-v330.json\n"
+                        "2023-07-07 13:43:35,845 :: matplotlib :: matplotlib data path: /Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\n",
+                        "2023-07-07 13:43:35,850 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\n",
+                        "2023-07-07 13:43:35,853 :: matplotlib :: interactive is False\n",
+                        "2023-07-07 13:43:35,854 :: matplotlib :: platform is darwin\n",
+                        "2023-07-07 13:43:35,868 :: graphviz._tools :: deprecate positional args: graphviz.backend.piping.pipe(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-07 13:43:35,869 :: graphviz._tools :: deprecate positional args: graphviz.backend.rendering.render(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-07 13:43:35,871 :: graphviz._tools :: deprecate positional args: graphviz.backend.unflattening.unflatten(['stagger', 'fanout', 'chain', 'encoding'])\n",
+                        "2023-07-07 13:43:35,873 :: graphviz._tools :: deprecate positional args: graphviz.backend.viewing.view(['quiet'])\n",
+                        "2023-07-07 13:43:35,877 :: graphviz._tools :: deprecate positional args: graphviz.quoting.quote(['is_html_string', 'is_valid_id', 'dot_keywords', 'endswith_odd_number_of_backslashes', 'escape_unescaped_quotes'])\n",
+                        "2023-07-07 13:43:35,878 :: graphviz._tools :: deprecate positional args: graphviz.quoting.a_list(['kwargs', 'attributes'])\n",
+                        "2023-07-07 13:43:35,878 :: graphviz._tools :: deprecate positional args: graphviz.quoting.attr_list(['kwargs', 'attributes'])\n",
+                        "2023-07-07 13:43:35,879 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.clear(['keep_attrs'])\n",
+                        "2023-07-07 13:43:35,880 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.__iter__(['subgraph'])\n",
+                        "2023-07-07 13:43:35,880 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.node(['_attributes'])\n",
+                        "2023-07-07 13:43:35,881 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.edge(['_attributes'])\n",
+                        "2023-07-07 13:43:35,882 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.attr(['_attributes'])\n",
+                        "2023-07-07 13:43:35,883 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.subgraph(['name', 'comment', 'graph_attr', 'node_attr', 'edge_attr', 'body'])\n",
+                        "2023-07-07 13:43:35,886 :: graphviz._tools :: deprecate positional args: graphviz.piping.Pipe._pipe_legacy(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-07 13:43:35,889 :: graphviz._tools :: deprecate positional args: graphviz.saving.Save.save(['directory'])\n",
+                        "2023-07-07 13:43:35,890 :: graphviz._tools :: deprecate positional args: graphviz.rendering.Render.render(['directory', 'view', 'cleanup', 'format', 'renderer', 'formatter', 'neato_no_op', 'quiet', 'quiet_view'])\n",
+                        "2023-07-07 13:43:35,891 :: graphviz._tools :: deprecate positional args: graphviz.rendering.Render.view(['directory', 'cleanup', 'quiet', 'quiet_view'])\n",
+                        "2023-07-07 13:43:35,892 :: graphviz._tools :: deprecate positional args: graphviz.unflattening.Unflatten.unflatten(['stagger', 'fanout', 'chain'])\n",
+                        "2023-07-07 13:43:35,893 :: graphviz._tools :: deprecate positional args: graphviz.graphs.BaseGraph.__init__(['comment', 'filename', 'directory', 'format', 'engine', 'encoding', 'graph_attr', 'node_attr', 'edge_attr', 'body', 'strict'])\n",
+                        "2023-07-07 13:43:35,895 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.from_file(['directory', 'format', 'engine', 'encoding', 'renderer', 'formatter'])\n",
+                        "2023-07-07 13:43:35,896 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.__init__(['filename', 'directory', 'format', 'engine', 'encoding'])\n",
+                        "2023-07-07 13:43:35,897 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.save(['directory'])\n"
                     ]
                 }
             ],
             "source": [
                 "import pandas as pd\n",
                 "from sklearn.model_selection import KFold, train_test_split\n",
                 "from lohrasb.best_estimator import BaseModel\n",
@@ -329,39 +347,65 @@
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "obj = BaseModel().optimize_by_gridsearchcv(\n",
-                "            estimator=estimator,\n",
-                "            estimator_params=estimator_params,\n",
-                "            fit_params = None,\n",
-                "            measure_of_accuracy=None,\n",
-                "            # if scoring is not None, it will be applied instead of measure_of_accuracy\n",
-                "            scoring = 'f1',\n",
-                "            verbose=3,\n",
-                "            n_jobs=-1,\n",
-                "            random_state=42,\n",
-                "            cv=KFold(2),\n",
-                "        )"
+                "kwargs = { # extra params for model if any\n",
+                "            'main_tunegrid_kwargs':{}, \n",
+                "            # params for fit method or fit_params \n",
+                "            'fit_tunegrid_kwargs' :{\n",
+                "            'sample_weight':None,\n",
+                "            },\n",
+                "            # params for RandomSearchCV \n",
+                "            'tunegrid_search_kwargs' : {\n",
+                "            'estimator':estimator,\n",
+                "            'param_grid':estimator_params,\n",
+                "            'n_jobs':None,\n",
+                "            'cv':KFold(3),\n",
+                "            'early_stopping':None, \n",
+                "            'scoring':None, \n",
+                "            'refit':True, \n",
+                "            'error_score':'raise', \n",
+                "            'return_train_score':False, \n",
+                "            'local_dir':'~/ray_results', \n",
+                "            'name':None, \n",
+                "            'max_iters':1, \n",
+                "            'use_gpu':False, \n",
+                "            'loggers':None, \n",
+                "            'pipeline_auto_early_stop':True, \n",
+                "            'stopper':None, \n",
+                "            'time_budget_s':None, \n",
+                "            'mode':None,\n",
+                "                }\n",
+                "            }\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "\n",
+                "obj = BaseModel().optimize_by_tunegridsearchcv(kwargs=kwargs)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Build sklearn pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "\n",
                 "pipeline =Pipeline([\n",
                 "            # int missing values imputers\n",
@@ -383,44 +427,33 @@
             "metadata": {},
             "source": [
                 "#### Run Pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
+                    "data": {
+                        "text/html": [],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[2m\u001b[36m(pid=95759)\u001b[0m 2023-05-16 10:27:24,462 :: dev :: Connected to Ray cluster!\n",
-                        "\u001b[2m\u001b[36m(pid=95759)\u001b[0m 2023-05-16 10:27:24,462 :: dev :: Connected to Ray cluster!\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m 2023-05-16 10:27:25,724 :: dev :: The optimization will be based on f1 metric!\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m 2023-05-16 10:27:25,724 :: dev :: The optimization will be based on f1 metric!\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m Fitting 2 folds for each of 8 candidates, totalling 16 fits\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 1/2] END booster=gbtree, eval_metric=auc, gamma=0.1, max_depth=4, subsample=0.8;, score=0.695 total time=   0.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 2/2] END booster=gbtree, eval_metric=auc, gamma=0.1, max_depth=4, subsample=0.8;, score=0.701 total time=   0.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 1/2] END booster=gbtree, eval_metric=auc, gamma=0.1, max_depth=5, subsample=0.8;, score=0.692 total time=   1.1s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 2/2] END booster=gbtree, eval_metric=auc, gamma=0.1, max_depth=5, subsample=0.8;, score=0.686 total time=   1.1s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 1/2] END booster=gbtree, eval_metric=auc, gamma=1.2, max_depth=4, subsample=0.8;, score=0.691 total time=   0.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 2/2] END booster=gbtree, eval_metric=auc, gamma=1.2, max_depth=4, subsample=0.8;, score=0.696 total time=   0.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 1/2] END booster=gbtree, eval_metric=auc, gamma=1.2, max_depth=5, subsample=0.8;, score=0.687 total time=   1.0s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 2/2] END booster=gbtree, eval_metric=auc, gamma=1.2, max_depth=5, subsample=0.8;, score=0.697 total time=   1.0s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 1/2] END booster=dart, eval_metric=auc, gamma=0.1, max_depth=4, subsample=0.8;, score=0.698 total time=   3.4s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 2/2] END booster=dart, eval_metric=auc, gamma=0.1, max_depth=4, subsample=0.8;, score=0.698 total time=   3.5s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 1/2] END booster=dart, eval_metric=auc, gamma=0.1, max_depth=5, subsample=0.8;, score=0.692 total time=   3.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 2/2] END booster=dart, eval_metric=auc, gamma=0.1, max_depth=5, subsample=0.8;, score=0.696 total time=   3.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 1/2] END booster=dart, eval_metric=auc, gamma=1.2, max_depth=4, subsample=0.8;, score=0.698 total time=   3.4s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 2/2] END booster=dart, eval_metric=auc, gamma=1.2, max_depth=4, subsample=0.8;, score=0.700 total time=   3.5s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 1/2] END booster=dart, eval_metric=auc, gamma=1.2, max_depth=5, subsample=0.8;, score=0.696 total time=   3.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95759)\u001b[0m [CV 2/2] END booster=dart, eval_metric=auc, gamma=1.2, max_depth=5, subsample=0.8;, score=0.694 total time=   3.8s\n",
-                        "2023-05-16 10:28:07,762 :: dev :: The optimization will be based on f1 metric!\n",
-                        "2023-05-16 10:28:07,762 :: dev :: The optimization will be based on f1 metric!\n"
+                        "2023-07-07 13:44:29,834 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n",
+                        "2023-07-07 13:44:29,834 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n"
                     ]
                 }
             ],
             "source": [
                 "pipeline.fit(X_train,y_train)\n",
                 "y_pred = pipeline.predict(X_test)\n"
             ]
@@ -431,36 +464,36 @@
             "metadata": {},
             "source": [
                 "#### Check performance of the pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "F1 score : \n",
-                        "0.709435534263695\n",
+                        "0.7138089278264498\n",
                         "Classification report : \n",
                         "              precision    recall  f1-score   support\n",
                         "\n",
                         "           0       0.90      0.94      0.92      8158\n",
-                        "           1       0.77      0.66      0.71      2588\n",
+                        "           1       0.78      0.66      0.71      2588\n",
                         "\n",
                         "    accuracy                           0.87     10746\n",
-                        "   macro avg       0.83      0.80      0.81     10746\n",
+                        "   macro avg       0.84      0.80      0.82     10746\n",
                         "weighted avg       0.87      0.87      0.87     10746\n",
                         "\n",
                         "Confusion matrix : \n",
-                        "[[7648  510]\n",
-                        " [ 885 1703]]\n"
+                        "[[7663  495]\n",
+                        " [ 877 1711]]\n"
                     ]
                 }
             ],
             "source": [
                 "print('F1 score : ')\n",
                 "print(f1_score(y_test,y_pred))\n",
                 "print('Classification report : ')\n",
@@ -470,20 +503,20 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Part 2:  Use BestModel as a standalone estimator "
+                "#### Part 2: Another way of using it "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "X_train, X_test, y_train, y_test =train_test_split(X, y, \\\n",
                 "     test_size=0.33, stratify=y['label'], random_state=42)"
             ]
         },
@@ -493,15 +526,15 @@
             "metadata": {},
             "source": [
                 "#### Transform features to make them ready for model input"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "transform_pipeline =Pipeline([\n",
                 "            # int missing values imputers\n",
                 "            ('intimputer', MeanMedianImputer(\n",
                 "                imputation_method='median', variables=int_cols)),\n",
@@ -520,15 +553,15 @@
             "metadata": {},
             "source": [
                 "#### Transform X_train and X_test"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
                 "X_train=transform_pipeline.fit_transform(X_train,y_train)\n",
                 "X_test=transform_pipeline.transform(X_test)\n"
             ]
         },
@@ -538,44 +571,33 @@
             "metadata": {},
             "source": [
                 "#### Train model and predict"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
+                    "data": {
+                        "text/html": [],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[2m\u001b[36m(pid=95764)\u001b[0m 2023-05-16 10:28:09,265 :: dev :: Connected to Ray cluster!\n",
-                        "\u001b[2m\u001b[36m(pid=95764)\u001b[0m 2023-05-16 10:28:09,265 :: dev :: Connected to Ray cluster!\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m 2023-05-16 10:28:10,607 :: dev :: The optimization will be based on f1 metric!\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m 2023-05-16 10:28:10,607 :: dev :: The optimization will be based on f1 metric!\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m Fitting 2 folds for each of 8 candidates, totalling 16 fits\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 1/2] END booster=gbtree, eval_metric=auc, gamma=0.1, max_depth=4, subsample=0.8;, score=0.695 total time=   0.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 2/2] END booster=gbtree, eval_metric=auc, gamma=0.1, max_depth=4, subsample=0.8;, score=0.701 total time=   0.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 1/2] END booster=gbtree, eval_metric=auc, gamma=0.1, max_depth=5, subsample=0.8;, score=0.692 total time=   1.0s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 2/2] END booster=gbtree, eval_metric=auc, gamma=0.1, max_depth=5, subsample=0.8;, score=0.686 total time=   1.0s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 1/2] END booster=gbtree, eval_metric=auc, gamma=1.2, max_depth=4, subsample=0.8;, score=0.691 total time=   0.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 2/2] END booster=gbtree, eval_metric=auc, gamma=1.2, max_depth=4, subsample=0.8;, score=0.696 total time=   0.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 1/2] END booster=gbtree, eval_metric=auc, gamma=1.2, max_depth=5, subsample=0.8;, score=0.687 total time=   1.0s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 2/2] END booster=gbtree, eval_metric=auc, gamma=1.2, max_depth=5, subsample=0.8;, score=0.697 total time=   1.0s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 1/2] END booster=dart, eval_metric=auc, gamma=0.1, max_depth=4, subsample=0.8;, score=0.698 total time=   3.5s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 2/2] END booster=dart, eval_metric=auc, gamma=0.1, max_depth=4, subsample=0.8;, score=0.698 total time=   3.5s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 1/2] END booster=dart, eval_metric=auc, gamma=0.1, max_depth=5, subsample=0.8;, score=0.692 total time=   3.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 2/2] END booster=dart, eval_metric=auc, gamma=0.1, max_depth=5, subsample=0.8;, score=0.696 total time=   4.5s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 1/2] END booster=dart, eval_metric=auc, gamma=1.2, max_depth=4, subsample=0.8;, score=0.698 total time=   4.0s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 2/2] END booster=dart, eval_metric=auc, gamma=1.2, max_depth=4, subsample=0.8;, score=0.700 total time=   3.6s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 1/2] END booster=dart, eval_metric=auc, gamma=1.2, max_depth=5, subsample=0.8;, score=0.696 total time=   3.8s\n",
-                        "\u001b[2m\u001b[36m(GridSearch pid=95764)\u001b[0m [CV 2/2] END booster=dart, eval_metric=auc, gamma=1.2, max_depth=5, subsample=0.8;, score=0.694 total time=   3.9s\n",
-                        "2023-05-16 10:28:53,860 :: dev :: The optimization will be based on f1 metric!\n",
-                        "2023-05-16 10:28:53,860 :: dev :: The optimization will be based on f1 metric!\n"
+                        "2023-07-07 13:45:23,494 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n",
+                        "2023-07-07 13:45:23,494 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n"
                     ]
                 }
             ],
             "source": [
                 "obj.fit(X_train,y_train)\n",
                 "y_pred = obj.predict(X_test)"
             ]
@@ -586,245 +608,242 @@
             "metadata": {},
             "source": [
                 "#### Check performance of the pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "F1 score : \n",
-                        "0.709435534263695\n",
+                        "0.7138089278264498\n",
                         "Classification report : \n",
                         "              precision    recall  f1-score   support\n",
                         "\n",
                         "           0       0.90      0.94      0.92      8158\n",
-                        "           1       0.77      0.66      0.71      2588\n",
+                        "           1       0.78      0.66      0.71      2588\n",
                         "\n",
                         "    accuracy                           0.87     10746\n",
-                        "   macro avg       0.83      0.80      0.81     10746\n",
+                        "   macro avg       0.84      0.80      0.82     10746\n",
                         "weighted avg       0.87      0.87      0.87     10746\n",
                         "\n",
                         "Confusion matrix : \n",
-                        "[[7648  510]\n",
-                        " [ 885 1703]]\n"
+                        "[[7663  495]\n",
+                        " [ 877 1711]]\n"
                     ]
                 }
             ],
             "source": [
                 "print('F1 score : ')\n",
                 "print(f1_score(y_test,y_pred))\n",
                 "print('Classification report : ')\n",
                 "print(classification_report(y_test,y_pred))\n",
                 "print('Confusion matrix : ')\n",
                 "print(confusion_matrix(y_test,y_pred))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;dart&#x27;, callbacks=None,\n",
+                            "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;gbtree&#x27;, callbacks=None,\n",
                             "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
                             "              early_stopping_rounds=None, enable_categorical=False,\n",
                             "              eval_metric=&#x27;auc&#x27;, feature_types=None, gamma=1.2, gpu_id=-1,\n",
                             "              grow_policy=&#x27;depthwise&#x27;, importance_type=None,\n",
                             "              interaction_constraints=&#x27;&#x27;, learning_rate=0.300000012,\n",
                             "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
                             "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
                             "              missing=nan, monotone_constraints=&#x27;()&#x27;, n_estimators=100,\n",
-                            "              n_jobs=0, num_parallel_tree=1, predictor=&#x27;auto&#x27;, random_state=0, ...)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">XGBClassifier</label><div class=\"sk-toggleable__content\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;dart&#x27;, callbacks=None,\n",
+                            "              n_jobs=0, num_parallel_tree=1, predictor=&#x27;auto&#x27;, random_state=0, ...)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">XGBClassifier</label><div class=\"sk-toggleable__content\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;gbtree&#x27;, callbacks=None,\n",
                             "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
                             "              early_stopping_rounds=None, enable_categorical=False,\n",
                             "              eval_metric=&#x27;auc&#x27;, feature_types=None, gamma=1.2, gpu_id=-1,\n",
                             "              grow_policy=&#x27;depthwise&#x27;, importance_type=None,\n",
                             "              interaction_constraints=&#x27;&#x27;, learning_rate=0.300000012,\n",
                             "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
                             "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
                             "              missing=nan, monotone_constraints=&#x27;()&#x27;, n_estimators=100,\n",
                             "              n_jobs=0, num_parallel_tree=1, predictor=&#x27;auto&#x27;, random_state=0, ...)</pre></div></div></div></div></div>"
                         ],
                         "text/plain": [
-                            "XGBClassifier(base_score=0.5, booster='dart', callbacks=None,\n",
+                            "XGBClassifier(base_score=0.5, booster='gbtree', callbacks=None,\n",
                             "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
                             "              early_stopping_rounds=None, enable_categorical=False,\n",
                             "              eval_metric='auc', feature_types=None, gamma=1.2, gpu_id=-1,\n",
                             "              grow_policy='depthwise', importance_type=None,\n",
                             "              interaction_constraints='', learning_rate=0.300000012,\n",
                             "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
                             "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
                             "              missing=nan, monotone_constraints='()', n_estimators=100,\n",
                             "              n_jobs=0, num_parallel_tree=1, predictor='auto', random_state=0, ...)"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "obj.get_best_estimator()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<style>#sk-container-id-2 {color: black;background-color: white;}#sk-container-id-2 pre{padding: 0;}#sk-container-id-2 div.sk-toggleable {background-color: white;}#sk-container-id-2 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-2 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-2 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-2 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-2 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-2 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-2 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-2 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-2 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-2 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-2 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-2 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-2 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-2 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-2 div.sk-item {position: relative;z-index: 1;}#sk-container-id-2 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-2 div.sk-item::before, #sk-container-id-2 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-2 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-2 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-2 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-2 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-2 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-2 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-2 div.sk-label-container {text-align: center;}#sk-container-id-2 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-2 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-2\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;dart&#x27;, callbacks=None,\n",
+                            "<style>#sk-container-id-2 {color: black;background-color: white;}#sk-container-id-2 pre{padding: 0;}#sk-container-id-2 div.sk-toggleable {background-color: white;}#sk-container-id-2 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-2 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-2 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-2 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-2 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-2 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-2 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-2 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-2 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-2 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-2 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-2 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-2 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-2 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-2 div.sk-item {position: relative;z-index: 1;}#sk-container-id-2 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-2 div.sk-item::before, #sk-container-id-2 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-2 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-2 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-2 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-2 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-2 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-2 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-2 div.sk-label-container {text-align: center;}#sk-container-id-2 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-2 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-2\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;gbtree&#x27;, callbacks=None,\n",
                             "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
                             "              early_stopping_rounds=None, enable_categorical=False,\n",
                             "              eval_metric=&#x27;auc&#x27;, feature_types=None, gamma=1.2, gpu_id=-1,\n",
                             "              grow_policy=&#x27;depthwise&#x27;, importance_type=None,\n",
                             "              interaction_constraints=&#x27;&#x27;, learning_rate=0.300000012,\n",
                             "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
                             "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
                             "              missing=nan, monotone_constraints=&#x27;()&#x27;, n_estimators=100,\n",
-                            "              n_jobs=0, num_parallel_tree=1, predictor=&#x27;auto&#x27;, random_state=0, ...)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-2\" type=\"checkbox\" checked><label for=\"sk-estimator-id-2\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">XGBClassifier</label><div class=\"sk-toggleable__content\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;dart&#x27;, callbacks=None,\n",
+                            "              n_jobs=0, num_parallel_tree=1, predictor=&#x27;auto&#x27;, random_state=0, ...)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-2\" type=\"checkbox\" checked><label for=\"sk-estimator-id-2\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">XGBClassifier</label><div class=\"sk-toggleable__content\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;gbtree&#x27;, callbacks=None,\n",
                             "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
                             "              early_stopping_rounds=None, enable_categorical=False,\n",
                             "              eval_metric=&#x27;auc&#x27;, feature_types=None, gamma=1.2, gpu_id=-1,\n",
                             "              grow_policy=&#x27;depthwise&#x27;, importance_type=None,\n",
                             "              interaction_constraints=&#x27;&#x27;, learning_rate=0.300000012,\n",
                             "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
                             "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
                             "              missing=nan, monotone_constraints=&#x27;()&#x27;, n_estimators=100,\n",
                             "              n_jobs=0, num_parallel_tree=1, predictor=&#x27;auto&#x27;, random_state=0, ...)</pre></div></div></div></div></div>"
                         ],
                         "text/plain": [
-                            "XGBClassifier(base_score=0.5, booster='dart', callbacks=None,\n",
+                            "XGBClassifier(base_score=0.5, booster='gbtree', callbacks=None,\n",
                             "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
                             "              early_stopping_rounds=None, enable_categorical=False,\n",
                             "              eval_metric='auc', feature_types=None, gamma=1.2, gpu_id=-1,\n",
                             "              grow_policy='depthwise', importance_type=None,\n",
                             "              interaction_constraints='', learning_rate=0.300000012,\n",
                             "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
                             "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
                             "              missing=nan, monotone_constraints='()', n_estimators=100,\n",
                             "              n_jobs=0, num_parallel_tree=1, predictor='auto', random_state=0, ...)"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "obj.best_estimator"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Get fitted grid search object and its attributes"
+                "#### Get fitted search object and its attributes"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'mean_fit_time': array([0.74981165, 0.93834686, 0.73568881, 0.94974899, 2.91844547,\n",
-                            "        3.53780055, 3.22567642, 3.23812008]),\n",
-                            " 'std_fit_time': array([1.23004913e-02, 8.75592232e-03, 1.34110451e-04, 4.29892540e-03,\n",
-                            "        3.28305960e-02, 3.04844379e-01, 1.53799653e-01, 4.13870811e-02]),\n",
-                            " 'mean_score_time': array([0.02147448, 0.02464116, 0.02131498, 0.02656698, 0.57403207,\n",
-                            "        0.61339986, 0.5957005 , 0.58104408]),\n",
-                            " 'std_score_time': array([1.56164169e-05, 5.19871712e-04, 2.70962715e-04, 2.50005722e-03,\n",
-                            "        7.04050064e-04, 1.20294094e-03, 1.90415382e-02, 2.76386738e-03]),\n",
-                            " 'param_booster': masked_array(data=['gbtree', 'gbtree', 'gbtree', 'gbtree', 'dart', 'dart',\n",
-                            "                    'dart', 'dart'],\n",
-                            "              mask=[False, False, False, False, False, False, False, False],\n",
-                            "        fill_value='?',\n",
-                            "             dtype=object),\n",
-                            " 'param_eval_metric': masked_array(data=['auc', 'auc', 'auc', 'auc', 'auc', 'auc', 'auc', 'auc'],\n",
-                            "              mask=[False, False, False, False, False, False, False, False],\n",
-                            "        fill_value='?',\n",
-                            "             dtype=object),\n",
-                            " 'param_gamma': masked_array(data=[0.1, 0.1, 1.2, 1.2, 0.1, 0.1, 1.2, 1.2],\n",
-                            "              mask=[False, False, False, False, False, False, False, False],\n",
-                            "        fill_value='?',\n",
-                            "             dtype=object),\n",
-                            " 'param_max_depth': masked_array(data=[4, 5, 4, 5, 4, 5, 4, 5],\n",
-                            "              mask=[False, False, False, False, False, False, False, False],\n",
-                            "        fill_value='?',\n",
-                            "             dtype=object),\n",
-                            " 'param_subsample': masked_array(data=[0.8, 0.8, 0.8, 0.8, 0.8, 0.8, 0.8, 0.8],\n",
-                            "              mask=[False, False, False, False, False, False, False, False],\n",
-                            "        fill_value='?',\n",
-                            "             dtype=object),\n",
-                            " 'params': [{'booster': 'gbtree',\n",
+                            "{'params': [{'booster': 'gbtree',\n",
                             "   'eval_metric': 'auc',\n",
-                            "   'gamma': 0.1,\n",
                             "   'max_depth': 4,\n",
+                            "   'gamma': 0.1,\n",
                             "   'subsample': 0.8},\n",
-                            "  {'booster': 'gbtree',\n",
+                            "  {'booster': 'dart',\n",
                             "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 4,\n",
                             "   'gamma': 0.1,\n",
-                            "   'max_depth': 5,\n",
                             "   'subsample': 0.8},\n",
                             "  {'booster': 'gbtree',\n",
                             "   'eval_metric': 'auc',\n",
-                            "   'gamma': 1.2,\n",
                             "   'max_depth': 4,\n",
+                            "   'gamma': 1.2,\n",
                             "   'subsample': 0.8},\n",
-                            "  {'booster': 'gbtree',\n",
+                            "  {'booster': 'dart',\n",
                             "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 4,\n",
                             "   'gamma': 1.2,\n",
-                            "   'max_depth': 5,\n",
                             "   'subsample': 0.8},\n",
-                            "  {'booster': 'dart',\n",
+                            "  {'booster': 'gbtree',\n",
                             "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 5,\n",
                             "   'gamma': 0.1,\n",
-                            "   'max_depth': 4,\n",
                             "   'subsample': 0.8},\n",
                             "  {'booster': 'dart',\n",
                             "   'eval_metric': 'auc',\n",
-                            "   'gamma': 0.1,\n",
                             "   'max_depth': 5,\n",
+                            "   'gamma': 0.1,\n",
                             "   'subsample': 0.8},\n",
-                            "  {'booster': 'dart',\n",
+                            "  {'booster': 'gbtree',\n",
                             "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 5,\n",
                             "   'gamma': 1.2,\n",
-                            "   'max_depth': 4,\n",
                             "   'subsample': 0.8},\n",
                             "  {'booster': 'dart',\n",
                             "   'eval_metric': 'auc',\n",
-                            "   'gamma': 1.2,\n",
                             "   'max_depth': 5,\n",
+                            "   'gamma': 1.2,\n",
                             "   'subsample': 0.8}],\n",
-                            " 'split0_test_score': array([0.6949855 , 0.69180058, 0.69103676, 0.68661027, 0.6984127 ,\n",
-                            "        0.69229196, 0.6975398 , 0.69581281]),\n",
-                            " 'split1_test_score': array([0.70081967, 0.68641471, 0.69609856, 0.6973336 , 0.69798105,\n",
-                            "        0.69641046, 0.70045511, 0.69439348]),\n",
-                            " 'mean_test_score': array([0.69790258, 0.68910764, 0.69356766, 0.69197194, 0.69819687,\n",
-                            "        0.69435121, 0.69899745, 0.69510314]),\n",
-                            " 'std_test_score': array([0.00291709, 0.00269293, 0.0025309 , 0.00536167, 0.00021583,\n",
-                            "        0.00205925, 0.00145766, 0.00070967]),\n",
-                            " 'rank_test_score': array([3, 8, 6, 7, 2, 5, 1, 4], dtype=int32)}"
+                            " 'split0_test_score': array([0.86207371, 0.86386139, 0.86193619, 0.86234873, 0.86331133,\n",
+                            "        0.86111111, 0.86248625, 0.86138614]),\n",
+                            " 'split1_test_score': array([0.8719747 , 0.87252475, 0.87142464, 0.87252475, 0.87046205,\n",
+                            "        0.86647415, 0.87059956, 0.86977448]),\n",
+                            " 'split2_test_score': array([0.86673085, 0.86480539, 0.86838124, 0.86618072, 0.86343006,\n",
+                            "        0.86191721, 0.86343006, 0.86411773]),\n",
+                            " 'mean_test_score': array([0.86692642, 0.86706384, 0.86724736, 0.86701807, 0.86573448,\n",
+                            "        0.86316749, 0.86550529, 0.86509278]),\n",
+                            " 'std_test_score': array([0.00404443, 0.00388063, 0.00395575, 0.00419632, 0.00334325,\n",
+                            "        0.00236121, 0.00362274, 0.00349324]),\n",
+                            " 'rank_test_score': array([4, 2, 1, 3, 5, 8, 6, 7], dtype=int32),\n",
+                            " 'time_total_s': array([ 5.402529  , 15.62350202,  5.36826706, 15.67608404,  6.36941504,\n",
+                            "        16.71763706,  6.36367917, 16.56950927]),\n",
+                            " 'training_iteration': array([1, 1, 1, 1, 1, 1, 1, 1]),\n",
+                            " 'param_booster': masked_array(data=['gbtree', 'dart', 'gbtree', 'dart', 'gbtree', 'dart',\n",
+                            "                    'gbtree', 'dart'],\n",
+                            "              mask=[False, False, False, False, False, False, False, False],\n",
+                            "        fill_value='?',\n",
+                            "             dtype=object),\n",
+                            " 'param_eval_metric': masked_array(data=['auc', 'auc', 'auc', 'auc', 'auc', 'auc', 'auc', 'auc'],\n",
+                            "              mask=[False, False, False, False, False, False, False, False],\n",
+                            "        fill_value='?',\n",
+                            "             dtype=object),\n",
+                            " 'param_max_depth': masked_array(data=[4, 4, 4, 4, 5, 5, 5, 5],\n",
+                            "              mask=[False, False, False, False, False, False, False, False],\n",
+                            "        fill_value='?',\n",
+                            "             dtype=object),\n",
+                            " 'param_gamma': masked_array(data=[0.1, 0.1, 1.2, 1.2, 0.1, 0.1, 1.2, 1.2],\n",
+                            "              mask=[False, False, False, False, False, False, False, False],\n",
+                            "        fill_value='?',\n",
+                            "             dtype=object),\n",
+                            " 'param_subsample': masked_array(data=[0.8, 0.8, 0.8, 0.8, 0.8, 0.8, 0.8, 0.8],\n",
+                            "              mask=[False, False, False, False, False, False, False, False],\n",
+                            "        fill_value='?',\n",
+                            "             dtype=object)}"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "GridSearchObj = obj.get_optimized_object()\n",
                 "GridSearchObj.cv_results_"
```

### Comparing `lohrasb-3.6.0/lohrasb/examples/classification_randomsearch.ipynb` & `lohrasb-4.0.0/lohrasb/examples/regression_optuna.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9667680978738459%*

 * *Differences: {"'cells'": "{0: {'outputs': {0: {'text': ['2023-07-03 17:15:40,392 :: matplotlib :: matplotlib "*

 * *            'data path: '*

 * *            "/Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\\n', "*

 * *            "'2023-07-03 17:15:40,398 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\\n', "*

 * *            "'2023-07-03 17:15:40,401 :: matplotlib :: interactive is False\\n', '2023-07-03 "*

 * *            '17:15:40,402 :: matplotlib :: platform is darwin\\n\', "2023-07-03 17 […]*

```diff
@@ -5,57 +5,78 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2023-05-02 21:48:34,990 :: dev :: Connected to Ray cluster!\n",
-                        "2023-05-02 21:48:34,990 :: dev :: Connected to Ray cluster!\n",
-                        "2023-05-02 21:48:35,409 :: matplotlib :: matplotlib data path: /Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\n",
-                        "2023-05-02 21:48:35,415 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\n",
-                        "2023-05-02 21:48:35,419 :: matplotlib :: interactive is False\n",
-                        "2023-05-02 21:48:35,420 :: matplotlib :: platform is darwin\n",
-                        "2023-05-02 21:48:36,705 :: matplotlib :: CACHEDIR=/Users/hjavedani/.matplotlib\n",
-                        "2023-05-02 21:48:36,708 :: matplotlib.font_manager :: Using fontManager instance from /Users/hjavedani/.matplotlib/fontlist-v330.json\n"
+                        "2023-07-03 17:15:40,392 :: matplotlib :: matplotlib data path: /Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\n",
+                        "2023-07-03 17:15:40,398 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\n",
+                        "2023-07-03 17:15:40,401 :: matplotlib :: interactive is False\n",
+                        "2023-07-03 17:15:40,402 :: matplotlib :: platform is darwin\n",
+                        "2023-07-03 17:15:40,416 :: graphviz._tools :: deprecate positional args: graphviz.backend.piping.pipe(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-03 17:15:40,418 :: graphviz._tools :: deprecate positional args: graphviz.backend.rendering.render(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-03 17:15:40,420 :: graphviz._tools :: deprecate positional args: graphviz.backend.unflattening.unflatten(['stagger', 'fanout', 'chain', 'encoding'])\n",
+                        "2023-07-03 17:15:40,421 :: graphviz._tools :: deprecate positional args: graphviz.backend.viewing.view(['quiet'])\n",
+                        "2023-07-03 17:15:40,425 :: graphviz._tools :: deprecate positional args: graphviz.quoting.quote(['is_html_string', 'is_valid_id', 'dot_keywords', 'endswith_odd_number_of_backslashes', 'escape_unescaped_quotes'])\n",
+                        "2023-07-03 17:15:40,425 :: graphviz._tools :: deprecate positional args: graphviz.quoting.a_list(['kwargs', 'attributes'])\n",
+                        "2023-07-03 17:15:40,426 :: graphviz._tools :: deprecate positional args: graphviz.quoting.attr_list(['kwargs', 'attributes'])\n",
+                        "2023-07-03 17:15:40,427 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.clear(['keep_attrs'])\n",
+                        "2023-07-03 17:15:40,431 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.__iter__(['subgraph'])\n",
+                        "2023-07-03 17:15:40,433 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.node(['_attributes'])\n",
+                        "2023-07-03 17:15:40,434 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.edge(['_attributes'])\n",
+                        "2023-07-03 17:15:40,435 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.attr(['_attributes'])\n",
+                        "2023-07-03 17:15:40,435 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.subgraph(['name', 'comment', 'graph_attr', 'node_attr', 'edge_attr', 'body'])\n",
+                        "2023-07-03 17:15:40,438 :: graphviz._tools :: deprecate positional args: graphviz.piping.Pipe._pipe_legacy(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-03 17:15:40,441 :: graphviz._tools :: deprecate positional args: graphviz.saving.Save.save(['directory'])\n",
+                        "2023-07-03 17:15:40,441 :: graphviz._tools :: deprecate positional args: graphviz.rendering.Render.render(['directory', 'view', 'cleanup', 'format', 'renderer', 'formatter', 'neato_no_op', 'quiet', 'quiet_view'])\n",
+                        "2023-07-03 17:15:40,442 :: graphviz._tools :: deprecate positional args: graphviz.rendering.Render.view(['directory', 'cleanup', 'quiet', 'quiet_view'])\n",
+                        "2023-07-03 17:15:40,444 :: graphviz._tools :: deprecate positional args: graphviz.unflattening.Unflatten.unflatten(['stagger', 'fanout', 'chain'])\n",
+                        "2023-07-03 17:15:40,445 :: graphviz._tools :: deprecate positional args: graphviz.graphs.BaseGraph.__init__(['comment', 'filename', 'directory', 'format', 'engine', 'encoding', 'graph_attr', 'node_attr', 'edge_attr', 'body', 'strict'])\n",
+                        "2023-07-03 17:15:40,447 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.from_file(['directory', 'format', 'engine', 'encoding', 'renderer', 'formatter'])\n",
+                        "2023-07-03 17:15:40,447 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.__init__(['filename', 'directory', 'format', 'engine', 'encoding'])\n",
+                        "2023-07-03 17:15:40,448 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.save(['directory'])\n"
                     ]
                 }
             ],
             "source": [
-                "import pandas as pd\n",
-                "from sklearn.model_selection import KFold, train_test_split\n",
                 "from lohrasb.best_estimator import BaseModel\n",
+                "from optuna.pruners import HyperbandPruner\n",
+                "from optuna.samplers._tpe.sampler import TPESampler\n",
+                "from sklearn.model_selection import KFold,train_test_split\n",
+                "import pandas as pd\n",
+                "import optuna\n",
                 "from sklearn.pipeline import Pipeline\n",
                 "from feature_engine.imputation import (\n",
                 "    CategoricalImputer,\n",
                 "    MeanMedianImputer\n",
                 "    )\n",
                 "from category_encoders import OrdinalEncoder\n",
                 "from sklearn.metrics import (\n",
-                "    classification_report,\n",
-                "    confusion_matrix,\n",
-                "    f1_score)\n",
-                "from sklearn.metrics import f1_score, accuracy_score, make_scorer\n",
-                "from lightgbm import *\n"
+                "    make_scorer)\n",
+                "from sklearn.metrics import mean_absolute_error,r2_score\n",
+                "from sklearn.linear_model import *\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Example: Use Adult Data Set (a classification problem)\n",
+                "#### Example 2 :Computer Hardware Data Set (a regression problem)\n",
                 "  \n",
-                "https://archive.ics.uci.edu/ml/datasets/Adult"
+                "https://archive.ics.uci.edu/ml/datasets/Computer+Hardware"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Part 1: Use BestModel in sklearn pipeline\n"
+                "#### Part 1: Use BestModel in sklearn pipeline\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
@@ -76,417 +97,452 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>age</th>\n",
-                            "      <th>workclass</th>\n",
-                            "      <th>fnlwgt</th>\n",
-                            "      <th>education</th>\n",
-                            "      <th>education-num</th>\n",
-                            "      <th>marital-status</th>\n",
-                            "      <th>occupation</th>\n",
-                            "      <th>relationship</th>\n",
-                            "      <th>race</th>\n",
-                            "      <th>sex</th>\n",
-                            "      <th>capital-gain</th>\n",
-                            "      <th>capital-loss</th>\n",
-                            "      <th>hours-per-week</th>\n",
-                            "      <th>native-country</th>\n",
-                            "      <th>label</th>\n",
+                            "      <th>vendor name</th>\n",
+                            "      <th>Model Name</th>\n",
+                            "      <th>MYCT</th>\n",
+                            "      <th>MMIN</th>\n",
+                            "      <th>MMAX</th>\n",
+                            "      <th>CACH</th>\n",
+                            "      <th>CHMIN</th>\n",
+                            "      <th>CHMAX</th>\n",
+                            "      <th>PRP</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>39</td>\n",
-                            "      <td>State-gov</td>\n",
-                            "      <td>77516</td>\n",
-                            "      <td>Bachelors</td>\n",
-                            "      <td>13</td>\n",
-                            "      <td>Never-married</td>\n",
-                            "      <td>Adm-clerical</td>\n",
-                            "      <td>Not-in-family</td>\n",
-                            "      <td>White</td>\n",
-                            "      <td>Male</td>\n",
-                            "      <td>2174</td>\n",
+                            "      <th>adviser</th>\n",
+                            "      <td>32/60</td>\n",
+                            "      <td>125</td>\n",
+                            "      <td>256</td>\n",
+                            "      <td>6000</td>\n",
+                            "      <td>256</td>\n",
+                            "      <td>16</td>\n",
+                            "      <td>128</td>\n",
+                            "      <td>198</td>\n",
+                            "      <td>199</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>amdahl</th>\n",
+                            "      <td>470v/7</td>\n",
+                            "      <td>29</td>\n",
+                            "      <td>8000</td>\n",
+                            "      <td>32000</td>\n",
+                            "      <td>32</td>\n",
+                            "      <td>8</td>\n",
+                            "      <td>32</td>\n",
+                            "      <td>269</td>\n",
+                            "      <td>253</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>amdahl</th>\n",
+                            "      <td>470v/7a</td>\n",
+                            "      <td>29</td>\n",
+                            "      <td>8000</td>\n",
+                            "      <td>32000</td>\n",
+                            "      <td>32</td>\n",
+                            "      <td>8</td>\n",
+                            "      <td>32</td>\n",
+                            "      <td>220</td>\n",
+                            "      <td>253</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>amdahl</th>\n",
+                            "      <td>470v/7b</td>\n",
+                            "      <td>29</td>\n",
+                            "      <td>8000</td>\n",
+                            "      <td>32000</td>\n",
+                            "      <td>32</td>\n",
+                            "      <td>8</td>\n",
+                            "      <td>32</td>\n",
+                            "      <td>172</td>\n",
+                            "      <td>253</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>amdahl</th>\n",
+                            "      <td>470v/7c</td>\n",
+                            "      <td>29</td>\n",
+                            "      <td>8000</td>\n",
+                            "      <td>16000</td>\n",
+                            "      <td>32</td>\n",
+                            "      <td>8</td>\n",
+                            "      <td>16</td>\n",
+                            "      <td>132</td>\n",
+                            "      <td>132</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>...</th>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>sperry</th>\n",
+                            "      <td>80/8</td>\n",
+                            "      <td>124</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>8000</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>40</td>\n",
-                            "      <td>United-States</td>\n",
-                            "      <td>&lt;=50K</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>8</td>\n",
+                            "      <td>42</td>\n",
+                            "      <td>37</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1</th>\n",
+                            "      <th>sperry</th>\n",
+                            "      <td>90/80-model-3</td>\n",
+                            "      <td>98</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>8000</td>\n",
+                            "      <td>32</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>8</td>\n",
+                            "      <td>46</td>\n",
                             "      <td>50</td>\n",
-                            "      <td>Self-emp-not-inc</td>\n",
-                            "      <td>83311</td>\n",
-                            "      <td>Bachelors</td>\n",
-                            "      <td>13</td>\n",
-                            "      <td>Married-civ-spouse</td>\n",
-                            "      <td>Exec-managerial</td>\n",
-                            "      <td>Husband</td>\n",
-                            "      <td>White</td>\n",
-                            "      <td>Male</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>13</td>\n",
-                            "      <td>United-States</td>\n",
-                            "      <td>&lt;=50K</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>38</td>\n",
-                            "      <td>Private</td>\n",
-                            "      <td>215646</td>\n",
-                            "      <td>HS-grad</td>\n",
-                            "      <td>9</td>\n",
-                            "      <td>Divorced</td>\n",
-                            "      <td>Handlers-cleaners</td>\n",
-                            "      <td>Not-in-family</td>\n",
-                            "      <td>White</td>\n",
-                            "      <td>Male</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>sratus</th>\n",
+                            "      <td>32</td>\n",
+                            "      <td>125</td>\n",
+                            "      <td>2000</td>\n",
+                            "      <td>8000</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>14</td>\n",
+                            "      <td>52</td>\n",
+                            "      <td>41</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>wang</th>\n",
+                            "      <td>vs-100</td>\n",
+                            "      <td>480</td>\n",
+                            "      <td>512</td>\n",
+                            "      <td>8000</td>\n",
+                            "      <td>32</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>40</td>\n",
-                            "      <td>United-States</td>\n",
-                            "      <td>&lt;=50K</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>53</td>\n",
-                            "      <td>Private</td>\n",
-                            "      <td>234721</td>\n",
-                            "      <td>11th</td>\n",
-                            "      <td>7</td>\n",
-                            "      <td>Married-civ-spouse</td>\n",
-                            "      <td>Handlers-cleaners</td>\n",
-                            "      <td>Husband</td>\n",
-                            "      <td>Black</td>\n",
-                            "      <td>Male</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>67</td>\n",
+                            "      <td>47</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>wang</th>\n",
+                            "      <td>vs-90</td>\n",
+                            "      <td>480</td>\n",
+                            "      <td>1000</td>\n",
+                            "      <td>4000</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>40</td>\n",
-                            "      <td>United-States</td>\n",
-                            "      <td>&lt;=50K</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>28</td>\n",
-                            "      <td>Private</td>\n",
-                            "      <td>338409</td>\n",
-                            "      <td>Bachelors</td>\n",
-                            "      <td>13</td>\n",
-                            "      <td>Married-civ-spouse</td>\n",
-                            "      <td>Prof-specialty</td>\n",
-                            "      <td>Wife</td>\n",
-                            "      <td>Black</td>\n",
-                            "      <td>Female</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>40</td>\n",
-                            "      <td>Cuba</td>\n",
-                            "      <td>&lt;=50K</td>\n",
+                            "      <td>45</td>\n",
+                            "      <td>25</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
+                            "<p>209 rows \u00d7 9 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "   age          workclass  fnlwgt   education  education-num  \\\n",
-                            "0   39          State-gov   77516   Bachelors             13   \n",
-                            "1   50   Self-emp-not-inc   83311   Bachelors             13   \n",
-                            "2   38            Private  215646     HS-grad              9   \n",
-                            "3   53            Private  234721        11th              7   \n",
-                            "4   28            Private  338409   Bachelors             13   \n",
-                            "\n",
-                            "        marital-status          occupation    relationship    race      sex  \\\n",
-                            "0        Never-married        Adm-clerical   Not-in-family   White     Male   \n",
-                            "1   Married-civ-spouse     Exec-managerial         Husband   White     Male   \n",
-                            "2             Divorced   Handlers-cleaners   Not-in-family   White     Male   \n",
-                            "3   Married-civ-spouse   Handlers-cleaners         Husband   Black     Male   \n",
-                            "4   Married-civ-spouse      Prof-specialty            Wife   Black   Female   \n",
+                            "           vendor name  Model Name  MYCT   MMIN  MMAX  CACH  CHMIN  CHMAX  PRP\n",
+                            "adviser          32/60         125   256   6000   256    16    128    198  199\n",
+                            "amdahl          470v/7          29  8000  32000    32     8     32    269  253\n",
+                            "amdahl         470v/7a          29  8000  32000    32     8     32    220  253\n",
+                            "amdahl         470v/7b          29  8000  32000    32     8     32    172  253\n",
+                            "amdahl         470v/7c          29  8000  16000    32     8     16    132  132\n",
+                            "...                ...         ...   ...    ...   ...   ...    ...    ...  ...\n",
+                            "sperry            80/8         124  1000   8000     0     1      8     42   37\n",
+                            "sperry   90/80-model-3          98  1000   8000    32     2      8     46   50\n",
+                            "sratus              32         125  2000   8000     0     2     14     52   41\n",
+                            "wang            vs-100         480   512   8000    32     0      0     67   47\n",
+                            "wang             vs-90         480  1000   4000     0     0      0     45   25\n",
                             "\n",
-                            "   capital-gain  capital-loss  hours-per-week  native-country   label  \n",
-                            "0          2174             0              40   United-States   <=50K  \n",
-                            "1             0             0              13   United-States   <=50K  \n",
-                            "2             0             0              40   United-States   <=50K  \n",
-                            "3             0             0              40   United-States   <=50K  \n",
-                            "4             0             0              40            Cuba   <=50K  "
+                            "[209 rows x 9 columns]"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "urldata= \"https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data\"\n",
+                "urldata= \"https://archive.ics.uci.edu/ml/machine-learning-databases/cpu-performance/machine.data\"\n",
                 "# column names\n",
-                "col_names=[\"age\", \"workclass\", \"fnlwgt\" , \"education\" ,\"education-num\",\n",
-                "\"marital-status\",\"occupation\",\"relationship\",\"race\",\"sex\",\"capital-gain\",\"capital-loss\",\"hours-per-week\",\n",
-                "\"native-country\",\"label\"\n",
+                "col_names=[\n",
+                "    \"vendor name\",\n",
+                "    \"Model Name\",\n",
+                "    \"MYCT\",\n",
+                "    \"MMIN\",\n",
+                "    \"MMAX\",\n",
+                "    \"CACH\",\n",
+                "    \"CHMIN\",\n",
+                "    \"CHMAX\",\n",
+                "    \"PRP\"\n",
                 "]\n",
                 "# read data\n",
                 "data = pd.read_csv(urldata,header=None,names=col_names,sep=',')\n",
-                "data.head()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "#### Define labels\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "data.loc[data['label']=='<=50K','label']=0\n",
-                "data.loc[data['label']==' <=50K','label']=0\n",
-                "\n",
-                "data.loc[data['label']=='>50K','label']=1\n",
-                "data.loc[data['label']==' >50K','label']=1\n",
-                "\n",
-                "data['label']=data['label'].astype(int)"
+                "data"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Train test split"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
-                "X = data.loc[:, data.columns != \"label\"]\n",
-                "y = data.loc[:, data.columns == \"label\"]\n",
+                "X = data.loc[:, data.columns != \"PRP\"]\n",
+                "y = data.loc[:, data.columns == \"PRP\"]\n",
+                "y = y.values.ravel()\n",
                 "\n",
                 "\n",
-                "X_train, X_test, y_train, y_test =train_test_split(X, y, \\\n",
-                "     test_size=0.33, stratify=y['label'], random_state=42)\n"
+                "X_train, X_test, y_train, y_test =train_test_split(X, y, test_size=0.33, random_state=42)\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Find feature types for later use"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "int_cols =  X_train.select_dtypes(include=['int']).columns.tolist()\n",
                 "float_cols =  X_train.select_dtypes(include=['float']).columns.tolist()\n",
                 "cat_cols =  X_train.select_dtypes(include=['object']).columns.tolist()\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Define estimator and set its arguments \n"
+                "####  Define estimator and set its arguments  "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
-                "estimator = LGBMClassifier()\n",
-                "estimator_params = {\n",
-                "        \"max_depth\": [6],\n",
-                "        \"learning_rate\": [0.01, 0.1],\n",
-                "        \"n_estimators\": [100,200],\n",
-                "        \"boosting_type\": [\"gbdt\"],\n",
-                "\n",
+                "estimator = LinearRegression()\n",
+                "estimator_params= {\n",
+                "        \"fit_intercept\": [True, False],\n",
                 "    }\n",
-                "    "
+                "\n",
+                "kwargs = {  # params for fit method  \n",
+                "            'fit_optuna_kwargs' :{\n",
+                "            'sample_weight':None,\n",
+                "            },\n",
+                "            # params for OptunaSearch\n",
+                "            'main_optuna_kwargs' : {\n",
+                "            'estimator':estimator,\n",
+                "            'estimator_params':estimator_params,\n",
+                "            'refit':True,\n",
+                "            'measure_of_accuracy' :\"mean_absolute_error(y_true, y_pred, multioutput='uniform_average')\"\n",
+                "\n",
+                "            },\n",
+                "            'train_test_split_kwargs':{\n",
+                "                'test_size':.3,\n",
+                "                            \n",
+                "            },\n",
+                "            'study_search_kwargs':{\n",
+                "                'storage':None,\n",
+                "                'sampler':TPESampler(),\n",
+                "                'pruner':HyperbandPruner(),\n",
+                "                'study_name':\"example of optuna optimizer\",\n",
+                "                'direction':\"maximize\",\n",
+                "                'load_if_exists':False,\n",
+                "            },\n",
+                "            'optimize_kwargs':{\n",
+                "                # optuna optimization params\n",
+                "                'n_trials':20,\n",
+                "                'timeout':600,\n",
+                "                'catch':(),\n",
+                "                'callbacks':None,\n",
+                "                'gc_after_trial':False,\n",
+                "                'show_progress_bar':False,\n",
+                "            }\n",
+                "}\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
-                "\n",
-                "obj = BaseModel().optimize_by_randomsearchcv(\n",
-                "            estimator=estimator,\n",
-                "            estimator_params=estimator_params,\n",
-                "            fit_params={\n",
-                "                'sample_weight':None\n",
-                "            },\n",
-                "            measure_of_accuracy=make_scorer(accuracy_score, normalize=False, greater_is_better=True),\n",
-                "            # or scoring='accuracy'\n",
-                "            scoring='f1',\n",
-                "            verbose=3,\n",
-                "            n_jobs=-1,\n",
-                "            random_state=42,\n",
-                "            cv=KFold(2),\n",
-                "            n_iter=4,\n",
-                "        )"
+                "obj = BaseModel().optimize_by_optuna(\n",
+                "        kwargs=kwargs\n",
+                "        )\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Build sklearn pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "\n",
                 "pipeline =Pipeline([\n",
                 "            # int missing values imputers\n",
                 "            ('intimputer', MeanMedianImputer(\n",
                 "                imputation_method='median', variables=int_cols)),\n",
                 "            # category missing values imputers\n",
                 "            ('catimputer', CategoricalImputer(variables=cat_cols)),\n",
                 "            #\n",
                 "            ('catencoder', OrdinalEncoder()),\n",
-                "            # classification model\n",
-                "            ('obj', obj)\n",
+                "            # regression model \n",
+                "            ('obj', obj),\n",
+                "\n",
                 "\n",
-                " ])\n"
+                " ])\n",
+                "\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Run Pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[I 2023-07-03 17:15:41,499] A new study created in memory with name: example of optuna optimizer\n",
+                        "[I 2023-07-03 17:15:41,504] Trial 0 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,509] Trial 1 finished with value: 15.746844270792897 and parameters: {'fit_intercept': 1}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,516] Trial 2 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,521] Trial 3 finished with value: 15.746844270792897 and parameters: {'fit_intercept': 1}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,526] Trial 4 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,530] Trial 5 finished with value: 15.746844270792897 and parameters: {'fit_intercept': 1}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,535] Trial 6 finished with value: 15.746844270792897 and parameters: {'fit_intercept': 1}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,540] Trial 7 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,545] Trial 8 finished with value: 15.746844270792897 and parameters: {'fit_intercept': 1}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,550] Trial 9 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,560] Trial 10 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,569] Trial 11 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,580] Trial 12 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,589] Trial 13 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,598] Trial 14 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,608] Trial 15 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,619] Trial 16 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,629] Trial 17 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,639] Trial 18 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n",
+                        "[I 2023-07-03 17:15:41,648] Trial 19 finished with value: 17.224204194190605 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 17.224204194190605.\n"
+                    ]
+                },
+                {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[2m\u001b[36m(pid=9796)\u001b[0m 2023-05-02 21:48:40,518 :: dev :: Connected to Ray cluster!\n",
-                        "\u001b[2m\u001b[36m(pid=9796)\u001b[0m 2023-05-02 21:48:40,518 :: dev :: Connected to Ray cluster!\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m 2023-05-02 21:48:41,945 :: matplotlib :: matplotlib data path: /Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m 2023-05-02 21:48:41,949 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m 2023-05-02 21:48:41,951 :: matplotlib :: interactive is False\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m 2023-05-02 21:48:41,951 :: matplotlib :: platform is darwin\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m 2023-05-02 21:48:42,018 :: dev :: The optimization will be based on f1 metric!\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m 2023-05-02 21:48:42,018 :: dev :: The optimization will be based on f1 metric!\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m Fitting 2 folds for each of 4 candidates, totalling 8 fits\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m [CV 1/2] END boosting_type=gbdt, learning_rate=0.01, max_depth=6, n_estimators=100;, score=0.604 total time=   0.3s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m [CV 2/2] END boosting_type=gbdt, learning_rate=0.01, max_depth=6, n_estimators=100;, score=0.542 total time=   0.2s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m [CV 1/2] END boosting_type=gbdt, learning_rate=0.01, max_depth=6, n_estimators=200;, score=0.657 total time=   0.3s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m [CV 2/2] END boosting_type=gbdt, learning_rate=0.01, max_depth=6, n_estimators=200;, score=0.648 total time=   0.4s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m [CV 1/2] END boosting_type=gbdt, learning_rate=0.1, max_depth=6, n_estimators=100;, score=0.696 total time=   0.2s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m [CV 2/2] END boosting_type=gbdt, learning_rate=0.1, max_depth=6, n_estimators=100;, score=0.703 total time=   0.2s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m [CV 1/2] END boosting_type=gbdt, learning_rate=0.1, max_depth=6, n_estimators=200;, score=0.693 total time=   0.3s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9796)\u001b[0m [CV 2/2] END boosting_type=gbdt, learning_rate=0.1, max_depth=6, n_estimators=200;, score=0.705 total time=   0.3s\n",
-                        "2023-05-02 21:48:44,368 :: dev :: The optimization will be based on f1 metric!\n",
-                        "2023-05-02 21:48:44,368 :: dev :: The optimization will be based on f1 metric!\n"
+                        "2023-07-03 17:15:41,651 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset, i.e., X_train and y_train!\n",
+                        "2023-07-03 17:15:41,651 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset, i.e., X_train and y_train!\n"
                     ]
                 }
             ],
             "source": [
-                "pipeline.fit(X_train,y_train.values.ravel())\n",
+                "pipeline.fit(X_train,y_train)\n",
                 "y_pred = pipeline.predict(X_test)\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Check performance of the pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "F1 score : \n",
-                        "0.7127749576988157\n",
-                        "Classification report : \n",
-                        "              precision    recall  f1-score   support\n",
-                        "\n",
-                        "           0       0.90      0.94      0.92      8158\n",
-                        "           1       0.79      0.65      0.71      2588\n",
-                        "\n",
-                        "    accuracy                           0.87     10746\n",
-                        "   macro avg       0.84      0.80      0.82     10746\n",
-                        "weighted avg       0.87      0.87      0.87     10746\n",
-                        "\n",
-                        "Confusion matrix : \n",
-                        "[[7703  455]\n",
-                        " [ 903 1685]]\n"
+                        "r2 score : \n",
+                        "0.9192355855868294\n"
                     ]
                 }
             ],
             "source": [
-                "print('F1 score : ')\n",
-                "print(f1_score(y_test,y_pred))\n",
-                "print('Classification report : ')\n",
-                "print(classification_report(y_test,y_pred))\n",
-                "print('Confusion matrix : ')\n",
-                "print(confusion_matrix(y_test,y_pred))\n"
+                "print('r2 score : ')\n",
+                "print(r2_score(y_test,y_pred))\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Part 2:  Use BestModel as a standalone estimator "
+                "#### Part 2: Another way of using it"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
-                "X_train, X_test, y_train, y_test =train_test_split(X, y, \\\n",
-                "     test_size=0.33, stratify=y['label'], random_state=42)"
+                "X_train, X_test, y_train, y_test =train_test_split(X, y, test_size=0.33, random_state=42)\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Transform features to make them ready for model input"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "transform_pipeline =Pipeline([\n",
                 "            # int missing values imputers\n",
                 "            ('intimputer', MeanMedianImputer(\n",
                 "                imputation_method='median', variables=int_cols)),\n",
@@ -496,232 +552,189 @@
                 "            ('catencoder', OrdinalEncoder()),\n",
                 "            # classification model\n",
                 "\n",
                 " ])"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Transform X_train and X_test"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "X_train=transform_pipeline.fit_transform(X_train,y_train)\n",
                 "X_test=transform_pipeline.transform(X_test)\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Train model and predict"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[I 2023-07-03 17:15:41,725] A new study created in memory with name: example of optuna optimizer\n",
+                        "[I 2023-07-03 17:15:41,733] Trial 0 finished with value: 17.30868987281197 and parameters: {'fit_intercept': 1}. Best is trial 0 with value: 17.30868987281197.\n",
+                        "[I 2023-07-03 17:15:41,739] Trial 1 finished with value: 17.30868987281197 and parameters: {'fit_intercept': 1}. Best is trial 0 with value: 17.30868987281197.\n",
+                        "[I 2023-07-03 17:15:41,743] Trial 2 finished with value: 17.30868987281197 and parameters: {'fit_intercept': 1}. Best is trial 0 with value: 17.30868987281197.\n",
+                        "[I 2023-07-03 17:15:41,749] Trial 3 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,754] Trial 4 finished with value: 17.30868987281197 and parameters: {'fit_intercept': 1}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,758] Trial 5 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,763] Trial 6 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,767] Trial 7 finished with value: 17.30868987281197 and parameters: {'fit_intercept': 1}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,772] Trial 8 finished with value: 17.30868987281197 and parameters: {'fit_intercept': 1}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,778] Trial 9 finished with value: 17.30868987281197 and parameters: {'fit_intercept': 1}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,787] Trial 10 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,798] Trial 11 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,807] Trial 12 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,820] Trial 13 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,893] Trial 14 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,916] Trial 15 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,940] Trial 16 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,955] Trial 17 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,967] Trial 18 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n",
+                        "[I 2023-07-03 17:15:41,976] Trial 19 finished with value: 17.536991316420217 and parameters: {'fit_intercept': 0}. Best is trial 3 with value: 17.536991316420217.\n"
+                    ]
+                },
+                {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[2m\u001b[36m(pid=9797)\u001b[0m 2023-05-02 21:48:45,590 :: dev :: Connected to Ray cluster!\n",
-                        "\u001b[2m\u001b[36m(pid=9797)\u001b[0m 2023-05-02 21:48:45,590 :: dev :: Connected to Ray cluster!\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m 2023-05-02 21:48:46,782 :: matplotlib :: matplotlib data path: /Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m 2023-05-02 21:48:46,786 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m 2023-05-02 21:48:46,787 :: matplotlib :: interactive is False\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m 2023-05-02 21:48:46,787 :: matplotlib :: platform is darwin\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m 2023-05-02 21:48:46,837 :: dev :: The optimization will be based on f1 metric!\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m 2023-05-02 21:48:46,837 :: dev :: The optimization will be based on f1 metric!\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m Fitting 2 folds for each of 4 candidates, totalling 8 fits\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m [CV 1/2] END boosting_type=gbdt, learning_rate=0.01, max_depth=6, n_estimators=100;, score=0.604 total time=   0.2s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m [CV 2/2] END boosting_type=gbdt, learning_rate=0.01, max_depth=6, n_estimators=100;, score=0.542 total time=   0.2s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m [CV 1/2] END boosting_type=gbdt, learning_rate=0.01, max_depth=6, n_estimators=200;, score=0.657 total time=   0.3s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m [CV 2/2] END boosting_type=gbdt, learning_rate=0.01, max_depth=6, n_estimators=200;, score=0.648 total time=   0.3s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m [CV 1/2] END boosting_type=gbdt, learning_rate=0.1, max_depth=6, n_estimators=100;, score=0.696 total time=   0.2s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m [CV 2/2] END boosting_type=gbdt, learning_rate=0.1, max_depth=6, n_estimators=100;, score=0.703 total time=   0.2s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m [CV 1/2] END boosting_type=gbdt, learning_rate=0.1, max_depth=6, n_estimators=200;, score=0.693 total time=   0.3s\n",
-                        "\u001b[2m\u001b[36m(RandomSearch pid=9797)\u001b[0m [CV 2/2] END boosting_type=gbdt, learning_rate=0.1, max_depth=6, n_estimators=200;, score=0.705 total time=   0.3s\n",
-                        "2023-05-02 21:48:48,934 :: dev :: The optimization will be based on f1 metric!\n",
-                        "2023-05-02 21:48:48,934 :: dev :: The optimization will be based on f1 metric!\n"
+                        "2023-07-03 17:15:41,978 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset, i.e., X_train and y_train!\n",
+                        "2023-07-03 17:15:41,978 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset, i.e., X_train and y_train!\n"
                     ]
                 }
             ],
             "source": [
-                "obj.fit(X_train,y_train.values.ravel())\n",
+                "obj.fit(X_train,y_train)\n",
                 "y_pred = obj.predict(X_test)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Check performance of the model"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "accuracy score score : \n",
-                        "9388\n",
-                        "F1 score : \n",
-                        "0.7127749576988157\n",
-                        "Classification report : \n",
-                        "              precision    recall  f1-score   support\n",
-                        "\n",
-                        "           0       0.90      0.94      0.92      8158\n",
-                        "           1       0.79      0.65      0.71      2588\n",
-                        "\n",
-                        "    accuracy                           0.87     10746\n",
-                        "   macro avg       0.84      0.80      0.82     10746\n",
-                        "weighted avg       0.87      0.87      0.87     10746\n",
-                        "\n",
-                        "Confusion matrix : \n",
-                        "[[7703  455]\n",
-                        " [ 903 1685]]\n"
+                        "r2 score : \n",
+                        "0.9192355855868294\n",
+                        "mean_absolute_error : \n",
+                        "30.288069195735655\n"
                     ]
                 }
             ],
             "source": [
-                "print('accuracy score score : ')\n",
-                "print(accuracy_score(y_test,y_pred,normalize=False))\n",
-                "print('F1 score : ')\n",
-                "print(f1_score(y_test,y_pred))\n",
-                "print('Classification report : ')\n",
-                "print(classification_report(y_test,y_pred))\n",
-                "print('Confusion matrix : ')\n",
-                "print(confusion_matrix(y_test,y_pred))"
+                "print('r2 score : ')\n",
+                "print(r2_score(y_test,y_pred))\n",
+                "print('mean_absolute_error : ')\n",
+                "print(mean_absolute_error(y_test,y_pred))\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LGBMClassifier(max_depth=6)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LGBMClassifier</label><div class=\"sk-toggleable__content\"><pre>LGBMClassifier(max_depth=6)</pre></div></div></div></div></div>"
+                            "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LinearRegression(fit_intercept=0)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LinearRegression</label><div class=\"sk-toggleable__content\"><pre>LinearRegression(fit_intercept=0)</pre></div></div></div></div></div>"
                         ],
                         "text/plain": [
-                            "LGBMClassifier(max_depth=6)"
+                            "LinearRegression(fit_intercept=0)"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "obj.get_best_estimator()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<style>#sk-container-id-2 {color: black;background-color: white;}#sk-container-id-2 pre{padding: 0;}#sk-container-id-2 div.sk-toggleable {background-color: white;}#sk-container-id-2 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-2 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-2 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-2 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-2 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-2 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-2 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-2 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-2 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-2 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-2 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-2 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-2 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-2 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-2 div.sk-item {position: relative;z-index: 1;}#sk-container-id-2 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-2 div.sk-item::before, #sk-container-id-2 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-2 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-2 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-2 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-2 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-2 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-2 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-2 div.sk-label-container {text-align: center;}#sk-container-id-2 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-2 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-2\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LGBMClassifier(max_depth=6)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-2\" type=\"checkbox\" checked><label for=\"sk-estimator-id-2\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LGBMClassifier</label><div class=\"sk-toggleable__content\"><pre>LGBMClassifier(max_depth=6)</pre></div></div></div></div></div>"
+                            "<style>#sk-container-id-2 {color: black;background-color: white;}#sk-container-id-2 pre{padding: 0;}#sk-container-id-2 div.sk-toggleable {background-color: white;}#sk-container-id-2 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-2 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-2 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-2 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-2 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-2 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-2 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-2 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-2 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-2 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-2 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-2 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-2 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-2 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-2 div.sk-item {position: relative;z-index: 1;}#sk-container-id-2 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-2 div.sk-item::before, #sk-container-id-2 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-2 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-2 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-2 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-2 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-2 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-2 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-2 div.sk-label-container {text-align: center;}#sk-container-id-2 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-2 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-2\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LinearRegression(fit_intercept=0)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-2\" type=\"checkbox\" checked><label for=\"sk-estimator-id-2\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LinearRegression</label><div class=\"sk-toggleable__content\"><pre>LinearRegression(fit_intercept=0)</pre></div></div></div></div></div>"
                         ],
                         "text/plain": [
-                            "LGBMClassifier(max_depth=6)"
+                            "LinearRegression(fit_intercept=0)"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "obj.best_estimator"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Get fitted randomized search object and its attributes"
+                "#### Get fitted search object and its attributes"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'mean_fit_time': array([0.12175357, 0.21687698, 0.0990485 , 0.17422247]),\n",
-                            " 'std_fit_time': array([0.00492156, 0.005687  , 0.00100362, 0.0055666 ]),\n",
-                            " 'mean_score_time': array([0.05387998, 0.11204958, 0.05606008, 0.11344421]),\n",
-                            " 'std_score_time': array([0.00040674, 0.00518847, 0.00107503, 0.00354087]),\n",
-                            " 'param_n_estimators': masked_array(data=[100, 200, 100, 200],\n",
-                            "              mask=[False, False, False, False],\n",
-                            "        fill_value='?',\n",
-                            "             dtype=object),\n",
-                            " 'param_max_depth': masked_array(data=[6, 6, 6, 6],\n",
-                            "              mask=[False, False, False, False],\n",
-                            "        fill_value='?',\n",
-                            "             dtype=object),\n",
-                            " 'param_learning_rate': masked_array(data=[0.01, 0.01, 0.1, 0.1],\n",
-                            "              mask=[False, False, False, False],\n",
-                            "        fill_value='?',\n",
-                            "             dtype=object),\n",
-                            " 'param_boosting_type': masked_array(data=['gbdt', 'gbdt', 'gbdt', 'gbdt'],\n",
-                            "              mask=[False, False, False, False],\n",
-                            "        fill_value='?',\n",
-                            "             dtype=object),\n",
-                            " 'params': [{'n_estimators': 100,\n",
-                            "   'max_depth': 6,\n",
-                            "   'learning_rate': 0.01,\n",
-                            "   'boosting_type': 'gbdt'},\n",
-                            "  {'n_estimators': 200,\n",
-                            "   'max_depth': 6,\n",
-                            "   'learning_rate': 0.01,\n",
-                            "   'boosting_type': 'gbdt'},\n",
-                            "  {'n_estimators': 100,\n",
-                            "   'max_depth': 6,\n",
-                            "   'learning_rate': 0.1,\n",
-                            "   'boosting_type': 'gbdt'},\n",
-                            "  {'n_estimators': 200,\n",
-                            "   'max_depth': 6,\n",
-                            "   'learning_rate': 0.1,\n",
-                            "   'boosting_type': 'gbdt'}],\n",
-                            " 'split0_test_score': array([0.6038945 , 0.65738036, 0.69616027, 0.69338843]),\n",
-                            " 'split1_test_score': array([0.54229249, 0.64838931, 0.70332427, 0.70467174]),\n",
-                            " 'mean_test_score': array([0.5730935 , 0.65288484, 0.69974227, 0.69903009]),\n",
-                            " 'std_test_score': array([0.03080101, 0.00449553, 0.003582  , 0.00564166]),\n",
-                            " 'rank_test_score': array([4, 3, 1, 2], dtype=int32)}"
+                            "FrozenTrial(number=3, state=TrialState.COMPLETE, values=[17.536991316420217], datetime_start=datetime.datetime(2023, 7, 3, 17, 15, 41, 744969), datetime_complete=datetime.datetime(2023, 7, 3, 17, 15, 41, 749112), params={'fit_intercept': 0}, user_attrs={}, system_attrs={}, intermediate_values={}, distributions={'fit_intercept': IntDistribution(high=1, log=False, low=0, step=1)}, trial_id=3, value=None)"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "RandomSearchObj = obj.get_optimized_object()\n",
-                "RandomSearchObj.cv_results_"
+                "OptunaObj = obj.get_optimized_object()\n",
+                "OptunaObj"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.10.4 ('.venv': poetry)",
             "language": "python",
```

### Comparing `lohrasb-3.6.0/lohrasb/examples/regression_optuna.ipynb` & `lohrasb-4.0.0/lohrasb/examples/classification_ray_tunesearch.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9641155556155719%*

 * *Differences: {"'cells'": "{0: {'outputs': {0: {'text': ['2023-07-07 20:22:49,933 :: matplotlib :: matplotlib "*

 * *            'data path: '*

 * *            "/Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\\n', "*

 * *            "'2023-07-07 20:22:49,938 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\\n', "*

 * *            "'2023-07-07 20:22:49,941 :: matplotlib :: interactive is False\\n', '2023-07-07 "*

 * *            '20:22:49,942 :: matplotlib :: platform is darwin\\n\', "2023-07-07 20 […]*

```diff
@@ -5,54 +5,78 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2023-05-02 21:19:28,933 :: dev :: Connected to Ray cluster!\n",
-                        "2023-05-02 21:19:28,933 :: dev :: Connected to Ray cluster!\n",
-                        "2023-05-02 21:19:30,518 :: matplotlib :: matplotlib data path: /Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\n",
-                        "2023-05-02 21:19:30,524 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\n",
-                        "2023-05-02 21:19:30,526 :: matplotlib :: interactive is False\n",
-                        "2023-05-02 21:19:30,528 :: matplotlib :: platform is darwin\n",
-                        "2023-05-02 21:19:31,240 :: matplotlib :: CACHEDIR=/Users/hjavedani/.matplotlib\n",
-                        "2023-05-02 21:19:31,245 :: matplotlib.font_manager :: Using fontManager instance from /Users/hjavedani/.matplotlib/fontlist-v330.json\n"
+                        "2023-07-07 20:22:49,933 :: matplotlib :: matplotlib data path: /Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\n",
+                        "2023-07-07 20:22:49,938 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\n",
+                        "2023-07-07 20:22:49,941 :: matplotlib :: interactive is False\n",
+                        "2023-07-07 20:22:49,942 :: matplotlib :: platform is darwin\n",
+                        "2023-07-07 20:22:49,956 :: graphviz._tools :: deprecate positional args: graphviz.backend.piping.pipe(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-07 20:22:49,958 :: graphviz._tools :: deprecate positional args: graphviz.backend.rendering.render(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-07 20:22:49,960 :: graphviz._tools :: deprecate positional args: graphviz.backend.unflattening.unflatten(['stagger', 'fanout', 'chain', 'encoding'])\n",
+                        "2023-07-07 20:22:49,961 :: graphviz._tools :: deprecate positional args: graphviz.backend.viewing.view(['quiet'])\n",
+                        "2023-07-07 20:22:49,965 :: graphviz._tools :: deprecate positional args: graphviz.quoting.quote(['is_html_string', 'is_valid_id', 'dot_keywords', 'endswith_odd_number_of_backslashes', 'escape_unescaped_quotes'])\n",
+                        "2023-07-07 20:22:49,966 :: graphviz._tools :: deprecate positional args: graphviz.quoting.a_list(['kwargs', 'attributes'])\n",
+                        "2023-07-07 20:22:49,966 :: graphviz._tools :: deprecate positional args: graphviz.quoting.attr_list(['kwargs', 'attributes'])\n",
+                        "2023-07-07 20:22:49,967 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.clear(['keep_attrs'])\n",
+                        "2023-07-07 20:22:49,968 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.__iter__(['subgraph'])\n",
+                        "2023-07-07 20:22:49,969 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.node(['_attributes'])\n",
+                        "2023-07-07 20:22:49,969 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.edge(['_attributes'])\n",
+                        "2023-07-07 20:22:49,970 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.attr(['_attributes'])\n",
+                        "2023-07-07 20:22:49,971 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.subgraph(['name', 'comment', 'graph_attr', 'node_attr', 'edge_attr', 'body'])\n",
+                        "2023-07-07 20:22:49,986 :: graphviz._tools :: deprecate positional args: graphviz.piping.Pipe._pipe_legacy(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-07 20:22:50,019 :: graphviz._tools :: deprecate positional args: graphviz.saving.Save.save(['directory'])\n",
+                        "2023-07-07 20:22:50,021 :: graphviz._tools :: deprecate positional args: graphviz.rendering.Render.render(['directory', 'view', 'cleanup', 'format', 'renderer', 'formatter', 'neato_no_op', 'quiet', 'quiet_view'])\n",
+                        "2023-07-07 20:22:50,022 :: graphviz._tools :: deprecate positional args: graphviz.rendering.Render.view(['directory', 'cleanup', 'quiet', 'quiet_view'])\n",
+                        "2023-07-07 20:22:50,025 :: graphviz._tools :: deprecate positional args: graphviz.unflattening.Unflatten.unflatten(['stagger', 'fanout', 'chain'])\n",
+                        "2023-07-07 20:22:50,026 :: graphviz._tools :: deprecate positional args: graphviz.graphs.BaseGraph.__init__(['comment', 'filename', 'directory', 'format', 'engine', 'encoding', 'graph_attr', 'node_attr', 'edge_attr', 'body', 'strict'])\n",
+                        "2023-07-07 20:22:50,037 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.from_file(['directory', 'format', 'engine', 'encoding', 'renderer', 'formatter'])\n",
+                        "2023-07-07 20:22:50,040 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.__init__(['filename', 'directory', 'format', 'engine', 'encoding'])\n",
+                        "2023-07-07 20:22:50,041 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.save(['directory'])\n",
+                        "2023-07-07 20:22:50,898 :: dev :: Using Scikit-Learn API (tune-sklearn) for an example of classification\n",
+                        "2023-07-07 20:22:50,898 :: dev :: Using Scikit-Learn API (tune-sklearn) for an example of classification\n"
                     ]
                 }
             ],
             "source": [
-                "from lohrasb.best_estimator import BaseModel\n",
-                "from optuna.pruners import HyperbandPruner\n",
-                "from optuna.samplers._tpe.sampler import TPESampler\n",
-                "from sklearn.model_selection import KFold,train_test_split\n",
                 "import pandas as pd\n",
-                "import optuna\n",
+                "from sklearn.model_selection import KFold, train_test_split\n",
+                "from lohrasb.best_estimator import BaseModel\n",
                 "from sklearn.pipeline import Pipeline\n",
                 "from feature_engine.imputation import (\n",
                 "    CategoricalImputer,\n",
                 "    MeanMedianImputer\n",
                 "    )\n",
                 "from category_encoders import OrdinalEncoder\n",
                 "from sklearn.metrics import (\n",
-                "    make_scorer)\n",
-                "from sklearn.metrics import mean_absolute_error,r2_score\n",
-                "from sklearn.linear_model import *\n"
+                "    classification_report,\n",
+                "    confusion_matrix,\n",
+                "    f1_score)\n",
+                "from sklearn.metrics import f1_score, make_scorer\n",
+                "from xgboost import *\n",
+                "from lohrasb import logger\n",
+                "\n",
+                "logger.info(\"Using Scikit-Learn API (tune-sklearn) for an example of classification\")\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Example 2 :Computer Hardware Data Set (a regression problem)\n",
+                "#### Example: Use Adult Data Set (a classification problem)\n",
                 "  \n",
-                "https://archive.ics.uci.edu/ml/datasets/Computer+Hardware"
+                "https://archive.ics.uci.edu/ml/datasets/Adult"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Part 1: Use BestModel in sklearn pipeline\n"
             ]
         },
         {
@@ -77,427 +101,443 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>vendor name</th>\n",
-                            "      <th>Model Name</th>\n",
-                            "      <th>MYCT</th>\n",
-                            "      <th>MMIN</th>\n",
-                            "      <th>MMAX</th>\n",
-                            "      <th>CACH</th>\n",
-                            "      <th>CHMIN</th>\n",
-                            "      <th>CHMAX</th>\n",
-                            "      <th>PRP</th>\n",
+                            "      <th>age</th>\n",
+                            "      <th>workclass</th>\n",
+                            "      <th>fnlwgt</th>\n",
+                            "      <th>education</th>\n",
+                            "      <th>education-num</th>\n",
+                            "      <th>marital-status</th>\n",
+                            "      <th>occupation</th>\n",
+                            "      <th>relationship</th>\n",
+                            "      <th>race</th>\n",
+                            "      <th>sex</th>\n",
+                            "      <th>capital-gain</th>\n",
+                            "      <th>capital-loss</th>\n",
+                            "      <th>hours-per-week</th>\n",
+                            "      <th>native-country</th>\n",
+                            "      <th>label</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>adviser</th>\n",
-                            "      <td>32/60</td>\n",
-                            "      <td>125</td>\n",
-                            "      <td>256</td>\n",
-                            "      <td>6000</td>\n",
-                            "      <td>256</td>\n",
-                            "      <td>16</td>\n",
-                            "      <td>128</td>\n",
-                            "      <td>198</td>\n",
-                            "      <td>199</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>amdahl</th>\n",
-                            "      <td>470v/7</td>\n",
-                            "      <td>29</td>\n",
-                            "      <td>8000</td>\n",
-                            "      <td>32000</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>8</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>269</td>\n",
-                            "      <td>253</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>amdahl</th>\n",
-                            "      <td>470v/7a</td>\n",
-                            "      <td>29</td>\n",
-                            "      <td>8000</td>\n",
-                            "      <td>32000</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>8</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>220</td>\n",
-                            "      <td>253</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>amdahl</th>\n",
-                            "      <td>470v/7b</td>\n",
-                            "      <td>29</td>\n",
-                            "      <td>8000</td>\n",
-                            "      <td>32000</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>8</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>172</td>\n",
-                            "      <td>253</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>amdahl</th>\n",
-                            "      <td>470v/7c</td>\n",
-                            "      <td>29</td>\n",
-                            "      <td>8000</td>\n",
-                            "      <td>16000</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>8</td>\n",
-                            "      <td>16</td>\n",
-                            "      <td>132</td>\n",
-                            "      <td>132</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>...</th>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>sperry</th>\n",
-                            "      <td>80/8</td>\n",
-                            "      <td>124</td>\n",
-                            "      <td>1000</td>\n",
-                            "      <td>8000</td>\n",
+                            "      <th>0</th>\n",
+                            "      <td>39</td>\n",
+                            "      <td>State-gov</td>\n",
+                            "      <td>77516</td>\n",
+                            "      <td>Bachelors</td>\n",
+                            "      <td>13</td>\n",
+                            "      <td>Never-married</td>\n",
+                            "      <td>Adm-clerical</td>\n",
+                            "      <td>Not-in-family</td>\n",
+                            "      <td>White</td>\n",
+                            "      <td>Male</td>\n",
+                            "      <td>2174</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>8</td>\n",
-                            "      <td>42</td>\n",
-                            "      <td>37</td>\n",
+                            "      <td>40</td>\n",
+                            "      <td>United-States</td>\n",
+                            "      <td>&lt;=50K</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>sperry</th>\n",
-                            "      <td>90/80-model-3</td>\n",
-                            "      <td>98</td>\n",
-                            "      <td>1000</td>\n",
-                            "      <td>8000</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>8</td>\n",
-                            "      <td>46</td>\n",
+                            "      <th>1</th>\n",
                             "      <td>50</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>sratus</th>\n",
-                            "      <td>32</td>\n",
-                            "      <td>125</td>\n",
-                            "      <td>2000</td>\n",
-                            "      <td>8000</td>\n",
+                            "      <td>Self-emp-not-inc</td>\n",
+                            "      <td>83311</td>\n",
+                            "      <td>Bachelors</td>\n",
+                            "      <td>13</td>\n",
+                            "      <td>Married-civ-spouse</td>\n",
+                            "      <td>Exec-managerial</td>\n",
+                            "      <td>Husband</td>\n",
+                            "      <td>White</td>\n",
+                            "      <td>Male</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>14</td>\n",
-                            "      <td>52</td>\n",
-                            "      <td>41</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>wang</th>\n",
-                            "      <td>vs-100</td>\n",
-                            "      <td>480</td>\n",
-                            "      <td>512</td>\n",
-                            "      <td>8000</td>\n",
-                            "      <td>32</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>13</td>\n",
+                            "      <td>United-States</td>\n",
+                            "      <td>&lt;=50K</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>38</td>\n",
+                            "      <td>Private</td>\n",
+                            "      <td>215646</td>\n",
+                            "      <td>HS-grad</td>\n",
+                            "      <td>9</td>\n",
+                            "      <td>Divorced</td>\n",
+                            "      <td>Handlers-cleaners</td>\n",
+                            "      <td>Not-in-family</td>\n",
+                            "      <td>White</td>\n",
+                            "      <td>Male</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>67</td>\n",
-                            "      <td>47</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>wang</th>\n",
-                            "      <td>vs-90</td>\n",
-                            "      <td>480</td>\n",
-                            "      <td>1000</td>\n",
-                            "      <td>4000</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>40</td>\n",
+                            "      <td>United-States</td>\n",
+                            "      <td>&lt;=50K</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>53</td>\n",
+                            "      <td>Private</td>\n",
+                            "      <td>234721</td>\n",
+                            "      <td>11th</td>\n",
+                            "      <td>7</td>\n",
+                            "      <td>Married-civ-spouse</td>\n",
+                            "      <td>Handlers-cleaners</td>\n",
+                            "      <td>Husband</td>\n",
+                            "      <td>Black</td>\n",
+                            "      <td>Male</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>45</td>\n",
-                            "      <td>25</td>\n",
+                            "      <td>40</td>\n",
+                            "      <td>United-States</td>\n",
+                            "      <td>&lt;=50K</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>28</td>\n",
+                            "      <td>Private</td>\n",
+                            "      <td>338409</td>\n",
+                            "      <td>Bachelors</td>\n",
+                            "      <td>13</td>\n",
+                            "      <td>Married-civ-spouse</td>\n",
+                            "      <td>Prof-specialty</td>\n",
+                            "      <td>Wife</td>\n",
+                            "      <td>Black</td>\n",
+                            "      <td>Female</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>40</td>\n",
+                            "      <td>Cuba</td>\n",
+                            "      <td>&lt;=50K</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>209 rows \u00d7 9 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "           vendor name  Model Name  MYCT   MMIN  MMAX  CACH  CHMIN  CHMAX  PRP\n",
-                            "adviser          32/60         125   256   6000   256    16    128    198  199\n",
-                            "amdahl          470v/7          29  8000  32000    32     8     32    269  253\n",
-                            "amdahl         470v/7a          29  8000  32000    32     8     32    220  253\n",
-                            "amdahl         470v/7b          29  8000  32000    32     8     32    172  253\n",
-                            "amdahl         470v/7c          29  8000  16000    32     8     16    132  132\n",
-                            "...                ...         ...   ...    ...   ...   ...    ...    ...  ...\n",
-                            "sperry            80/8         124  1000   8000     0     1      8     42   37\n",
-                            "sperry   90/80-model-3          98  1000   8000    32     2      8     46   50\n",
-                            "sratus              32         125  2000   8000     0     2     14     52   41\n",
-                            "wang            vs-100         480   512   8000    32     0      0     67   47\n",
-                            "wang             vs-90         480  1000   4000     0     0      0     45   25\n",
+                            "   age          workclass  fnlwgt   education  education-num  \\\n",
+                            "0   39          State-gov   77516   Bachelors             13   \n",
+                            "1   50   Self-emp-not-inc   83311   Bachelors             13   \n",
+                            "2   38            Private  215646     HS-grad              9   \n",
+                            "3   53            Private  234721        11th              7   \n",
+                            "4   28            Private  338409   Bachelors             13   \n",
+                            "\n",
+                            "        marital-status          occupation    relationship    race      sex  \\\n",
+                            "0        Never-married        Adm-clerical   Not-in-family   White     Male   \n",
+                            "1   Married-civ-spouse     Exec-managerial         Husband   White     Male   \n",
+                            "2             Divorced   Handlers-cleaners   Not-in-family   White     Male   \n",
+                            "3   Married-civ-spouse   Handlers-cleaners         Husband   Black     Male   \n",
+                            "4   Married-civ-spouse      Prof-specialty            Wife   Black   Female   \n",
                             "\n",
-                            "[209 rows x 9 columns]"
+                            "   capital-gain  capital-loss  hours-per-week  native-country   label  \n",
+                            "0          2174             0              40   United-States   <=50K  \n",
+                            "1             0             0              13   United-States   <=50K  \n",
+                            "2             0             0              40   United-States   <=50K  \n",
+                            "3             0             0              40   United-States   <=50K  \n",
+                            "4             0             0              40            Cuba   <=50K  "
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "urldata= \"https://archive.ics.uci.edu/ml/machine-learning-databases/cpu-performance/machine.data\"\n",
+                "urldata= \"https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data\"\n",
                 "# column names\n",
-                "col_names=[\n",
-                "    \"vendor name\",\n",
-                "    \"Model Name\",\n",
-                "    \"MYCT\",\n",
-                "    \"MMIN\",\n",
-                "    \"MMAX\",\n",
-                "    \"CACH\",\n",
-                "    \"CHMIN\",\n",
-                "    \"CHMAX\",\n",
-                "    \"PRP\"\n",
+                "col_names=[\"age\", \"workclass\", \"fnlwgt\" , \"education\" ,\"education-num\",\n",
+                "\"marital-status\",\"occupation\",\"relationship\",\"race\",\"sex\",\"capital-gain\",\"capital-loss\",\"hours-per-week\",\n",
+                "\"native-country\",\"label\"\n",
                 "]\n",
                 "# read data\n",
                 "data = pd.read_csv(urldata,header=None,names=col_names,sep=',')\n",
-                "data"
+                "data.head()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Train test split"
+                "#### Define labels\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
-                "X = data.loc[:, data.columns != \"PRP\"]\n",
-                "y = data.loc[:, data.columns == \"PRP\"]\n",
-                "y = y.values.ravel()\n",
+                "data.loc[data['label']=='<=50K','label']=0\n",
+                "data.loc[data['label']==' <=50K','label']=0\n",
                 "\n",
+                "data.loc[data['label']=='>50K','label']=1\n",
+                "data.loc[data['label']==' >50K','label']=1\n",
                 "\n",
-                "X_train, X_test, y_train, y_test =train_test_split(X, y, test_size=0.33, random_state=42)\n"
+                "data['label']=data['label'].astype(int)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Find feature types for later use"
+                "#### Train test split"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
+                "X = data.loc[:, data.columns != \"label\"]\n",
+                "y = data.loc[:, data.columns == \"label\"]\n",
+                "\n",
+                "\n",
+                "X_train, X_test, y_train, y_test =train_test_split(X, y, \\\n",
+                "     test_size=0.33, stratify=y['label'], random_state=42)\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "#### Find feature types for later use"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "int_cols =  X_train.select_dtypes(include=['int']).columns.tolist()\n",
                 "float_cols =  X_train.select_dtypes(include=['float']).columns.tolist()\n",
                 "cat_cols =  X_train.select_dtypes(include=['object']).columns.tolist()\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "####  Define estimator and set its arguments  "
+                "#### Define estimator and set its arguments \n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
-                "estimator = LinearRegression()\n",
-                "estimator_params= {\n",
-                "        \"fit_intercept\": [True, False],\n",
-                "    }\n"
+                "estimator = XGBClassifier()\n",
+                "estimator_params = {\n",
+                "        \"booster\": [\"gbtree\",\"dart\"],\n",
+                "        \"eval_metric\": [\"auc\"],\n",
+                "        \"max_depth\": [4, 5],\n",
+                "        \"gamma\": [0.1, 1.2],\n",
+                "        \"subsample\": [0.5,0.8],\n",
+                "\n",
+                "    }\n",
+                "    "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "\u001b[32m[I 2023-05-02 21:19:32,037]\u001b[0m A new study created in memory with name: no-name-4fb713e4-dd44-4e9f-993e-1675997cb060\u001b[0m\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "obj = BaseModel().optimize_by_optuna(\n",
-                "            estimator=estimator,\n",
-                "            estimator_params=estimator_params,\n",
-                "            measure_of_accuracy=\"mean_absolute_error(y_true, y_pred, multioutput='uniform_average')\",\n",
-                "            with_stratified=False,\n",
-                "            test_size=.3,\n",
-                "            verbose=3,\n",
-                "            n_jobs=-1,\n",
-                "            random_state=42,\n",
-                "            # optuna params\n",
-                "            # optuna study init params\n",
-                "            study=optuna.create_study(\n",
-                "                storage=None,\n",
-                "                sampler=TPESampler(),\n",
-                "                pruner=HyperbandPruner(),\n",
-                "                study_name=None,\n",
-                "                direction=\"minimize\",\n",
-                "                load_if_exists=False,\n",
-                "                directions=None,\n",
-                "            ),\n",
-                "            # optuna optimization params\n",
-                "            study_optimize_objective=None,\n",
-                "            study_optimize_objective_n_trials=10,\n",
-                "            study_optimize_objective_timeout=600,\n",
-                "            study_optimize_n_jobs=-1,\n",
-                "            study_optimize_catch=(),\n",
-                "            study_optimize_callbacks=None,\n",
-                "            study_optimize_gc_after_trial=False,\n",
-                "            study_optimize_show_progress_bar=False,\n",
-                "        )"
+                "kwargs = { # some extra params for model if any\n",
+                "            'main_tune_kwargs':{},  \n",
+                "            # params for fit method or fit_params \n",
+                "            'fit_tune_kwargs' :{\n",
+                "            'sample_weight':None,\n",
+                "            },\n",
+                "            # params for RandomSearchCV \n",
+                "            'tune_search_kwargs' : {\n",
+                "            'estimator':estimator,\n",
+                "            'param_distributions':estimator_params,\n",
+                "            'n_jobs':None,\n",
+                "            'cv':KFold(2),\n",
+                "            'early_stopping':None, \n",
+                "            'scoring':'f1', \n",
+                "            'refit':True, \n",
+                "            'error_score':'raise', \n",
+                "            'return_train_score':False, \n",
+                "            'local_dir':'~/ray_results', \n",
+                "            'name':None, \n",
+                "            'max_iters':1, \n",
+                "            'use_gpu':False, \n",
+                "            'loggers':None, \n",
+                "            'pipeline_auto_early_stop':True, \n",
+                "            'stopper':None, \n",
+                "            'time_budget_s':None, \n",
+                "            'mode':None,\n",
+                "            'max_iters':1, \n",
+                "                }\n",
+                "            }\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "\n",
+                "obj = BaseModel().optimize_by_tunesearchcv(kwargs=kwargs)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Build sklearn pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "\n",
                 "pipeline =Pipeline([\n",
                 "            # int missing values imputers\n",
                 "            ('intimputer', MeanMedianImputer(\n",
                 "                imputation_method='median', variables=int_cols)),\n",
                 "            # category missing values imputers\n",
                 "            ('catimputer', CategoricalImputer(variables=cat_cols)),\n",
                 "            #\n",
                 "            ('catencoder', OrdinalEncoder()),\n",
-                "            # regression model \n",
-                "            ('obj', obj),\n",
-                "\n",
+                "            # classification model\n",
+                "            ('obj', obj)\n",
                 "\n",
-                " ])\n",
-                "\n"
+                " ])\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Run Pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
+                    "data": {
+                        "text/html": [],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "/Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/optuna/study/study.py:393: FutureWarning: `n_jobs` argument has been deprecated in v2.7.0. This feature will be removed in v4.0.0. See https://github.com/optuna/optuna/releases/tag/v2.7.0.\n",
-                        "  warnings.warn(\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,140]\u001b[0m Trial 0 finished with value: 14.770921159757803 and parameters: {'fit_intercept': 0}. Best is trial 0 with value: 14.770921159757803.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,143]\u001b[0m Trial 2 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,146]\u001b[0m Trial 1 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,154]\u001b[0m Trial 5 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,156]\u001b[0m Trial 4 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,160]\u001b[0m Trial 6 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,162]\u001b[0m Trial 3 finished with value: 14.770921159757803 and parameters: {'fit_intercept': 0}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,166]\u001b[0m Trial 8 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,168]\u001b[0m Trial 7 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,174]\u001b[0m Trial 9 finished with value: 14.770921159757803 and parameters: {'fit_intercept': 0}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n"
+                        "2023-07-07 20:23:54,522 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n",
+                        "2023-07-07 20:23:54,522 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n"
                     ]
                 }
             ],
             "source": [
                 "pipeline.fit(X_train,y_train)\n",
                 "y_pred = pipeline.predict(X_test)\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Check performance of the pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "r2 score : \n",
-                        "0.9401429300951223\n"
+                        "F1 score : \n",
+                        "0.7138089278264498\n",
+                        "Classification report : \n",
+                        "              precision    recall  f1-score   support\n",
+                        "\n",
+                        "           0       0.90      0.94      0.92      8158\n",
+                        "           1       0.78      0.66      0.71      2588\n",
+                        "\n",
+                        "    accuracy                           0.87     10746\n",
+                        "   macro avg       0.84      0.80      0.82     10746\n",
+                        "weighted avg       0.87      0.87      0.87     10746\n",
+                        "\n",
+                        "Confusion matrix : \n",
+                        "[[7663  495]\n",
+                        " [ 877 1711]]\n"
                     ]
                 }
             ],
             "source": [
-                "print('r2 score : ')\n",
-                "print(r2_score(y_test,y_pred))\n"
+                "print('F1 score : ')\n",
+                "print(f1_score(y_test,y_pred))\n",
+                "print('Classification report : ')\n",
+                "print(classification_report(y_test,y_pred))\n",
+                "print('Confusion matrix : ')\n",
+                "print(confusion_matrix(y_test,y_pred))\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Part 2:  Use BestModel as a standalone estimator "
+                "#### Part 2: Another way of using it "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
-                "X_train, X_test, y_train, y_test =train_test_split(X, y, test_size=0.33, random_state=42)\n"
+                "X_train, X_test, y_train, y_test =train_test_split(X, y, \\\n",
+                "     test_size=0.33, stratify=y['label'], random_state=42)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Transform features to make them ready for model input"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "transform_pipeline =Pipeline([\n",
                 "            # int missing values imputers\n",
                 "            ('intimputer', MeanMedianImputer(\n",
                 "                imputation_method='median', variables=int_cols)),\n",
@@ -507,187 +547,329 @@
                 "            ('catencoder', OrdinalEncoder()),\n",
                 "            # classification model\n",
                 "\n",
                 " ])"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Transform X_train and X_test"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
                 "X_train=transform_pipeline.fit_transform(X_train,y_train)\n",
                 "X_test=transform_pipeline.transform(X_test)\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Train model and predict"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
+                    "data": {
+                        "text/html": [],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "/Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/optuna/study/study.py:393: FutureWarning: `n_jobs` argument has been deprecated in v2.7.0. This feature will be removed in v4.0.0. See https://github.com/optuna/optuna/releases/tag/v2.7.0.\n",
-                        "  warnings.warn(\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,365]\u001b[0m Trial 11 finished with value: 14.770921159757803 and parameters: {'fit_intercept': 0}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,371]\u001b[0m Trial 12 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,375]\u001b[0m Trial 10 finished with value: 14.770921159757803 and parameters: {'fit_intercept': 0}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,387]\u001b[0m Trial 16 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,394]\u001b[0m Trial 15 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,394]\u001b[0m Trial 13 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,395]\u001b[0m Trial 14 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,400]\u001b[0m Trial 17 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,405]\u001b[0m Trial 18 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n",
-                        "\u001b[32m[I 2023-05-02 21:19:32,411]\u001b[0m Trial 19 finished with value: 13.714193910659512 and parameters: {'fit_intercept': 1}. Best is trial 2 with value: 13.714193910659512.\u001b[0m\n"
+                        "2023-07-07 20:25:06,284 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n",
+                        "2023-07-07 20:25:06,284 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n"
                     ]
                 }
             ],
             "source": [
                 "obj.fit(X_train,y_train)\n",
                 "y_pred = obj.predict(X_test)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Check performance of the model"
+                "#### Check performance of the pipeline"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "r2 score : \n",
-                        "0.9401429300951223\n",
-                        "mean_absolute_error : \n",
-                        "25.975645074588805\n"
+                        "F1 score : \n",
+                        "0.709435534263695\n",
+                        "Classification report : \n",
+                        "              precision    recall  f1-score   support\n",
+                        "\n",
+                        "           0       0.90      0.94      0.92      8158\n",
+                        "           1       0.77      0.66      0.71      2588\n",
+                        "\n",
+                        "    accuracy                           0.87     10746\n",
+                        "   macro avg       0.83      0.80      0.81     10746\n",
+                        "weighted avg       0.87      0.87      0.87     10746\n",
+                        "\n",
+                        "Confusion matrix : \n",
+                        "[[7648  510]\n",
+                        " [ 885 1703]]\n"
                     ]
                 }
             ],
             "source": [
-                "print('r2 score : ')\n",
-                "print(r2_score(y_test,y_pred))\n",
-                "print('mean_absolute_error : ')\n",
-                "print(mean_absolute_error(y_test,y_pred))\n"
+                "print('F1 score : ')\n",
+                "print(f1_score(y_test,y_pred))\n",
+                "print('Classification report : ')\n",
+                "print(classification_report(y_test,y_pred))\n",
+                "print('Confusion matrix : ')\n",
+                "print(confusion_matrix(y_test,y_pred))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LinearRegression(fit_intercept=1)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LinearRegression</label><div class=\"sk-toggleable__content\"><pre>LinearRegression(fit_intercept=1)</pre></div></div></div></div></div>"
+                            "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;dart&#x27;, callbacks=None,\n",
+                            "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
+                            "              early_stopping_rounds=None, enable_categorical=False,\n",
+                            "              eval_metric=&#x27;auc&#x27;, feature_types=None, gamma=1.2, gpu_id=-1,\n",
+                            "              grow_policy=&#x27;depthwise&#x27;, importance_type=None,\n",
+                            "              interaction_constraints=&#x27;&#x27;, learning_rate=0.300000012,\n",
+                            "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
+                            "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
+                            "              missing=nan, monotone_constraints=&#x27;()&#x27;, n_estimators=100,\n",
+                            "              n_jobs=0, num_parallel_tree=1, predictor=&#x27;auto&#x27;, random_state=0, ...)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">XGBClassifier</label><div class=\"sk-toggleable__content\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;dart&#x27;, callbacks=None,\n",
+                            "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
+                            "              early_stopping_rounds=None, enable_categorical=False,\n",
+                            "              eval_metric=&#x27;auc&#x27;, feature_types=None, gamma=1.2, gpu_id=-1,\n",
+                            "              grow_policy=&#x27;depthwise&#x27;, importance_type=None,\n",
+                            "              interaction_constraints=&#x27;&#x27;, learning_rate=0.300000012,\n",
+                            "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
+                            "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
+                            "              missing=nan, monotone_constraints=&#x27;()&#x27;, n_estimators=100,\n",
+                            "              n_jobs=0, num_parallel_tree=1, predictor=&#x27;auto&#x27;, random_state=0, ...)</pre></div></div></div></div></div>"
                         ],
                         "text/plain": [
-                            "LinearRegression(fit_intercept=1)"
+                            "XGBClassifier(base_score=0.5, booster='dart', callbacks=None,\n",
+                            "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
+                            "              early_stopping_rounds=None, enable_categorical=False,\n",
+                            "              eval_metric='auc', feature_types=None, gamma=1.2, gpu_id=-1,\n",
+                            "              grow_policy='depthwise', importance_type=None,\n",
+                            "              interaction_constraints='', learning_rate=0.300000012,\n",
+                            "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
+                            "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
+                            "              missing=nan, monotone_constraints='()', n_estimators=100,\n",
+                            "              n_jobs=0, num_parallel_tree=1, predictor='auto', random_state=0, ...)"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "obj.get_best_estimator()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<style>#sk-container-id-2 {color: black;background-color: white;}#sk-container-id-2 pre{padding: 0;}#sk-container-id-2 div.sk-toggleable {background-color: white;}#sk-container-id-2 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-2 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-2 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-2 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-2 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-2 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-2 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-2 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-2 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-2 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-2 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-2 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-2 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-2 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-2 div.sk-item {position: relative;z-index: 1;}#sk-container-id-2 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-2 div.sk-item::before, #sk-container-id-2 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-2 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-2 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-2 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-2 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-2 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-2 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-2 div.sk-label-container {text-align: center;}#sk-container-id-2 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-2 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-2\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LinearRegression(fit_intercept=1)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-2\" type=\"checkbox\" checked><label for=\"sk-estimator-id-2\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LinearRegression</label><div class=\"sk-toggleable__content\"><pre>LinearRegression(fit_intercept=1)</pre></div></div></div></div></div>"
+                            "<style>#sk-container-id-2 {color: black;background-color: white;}#sk-container-id-2 pre{padding: 0;}#sk-container-id-2 div.sk-toggleable {background-color: white;}#sk-container-id-2 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-2 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-2 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-2 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-2 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-2 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-2 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-2 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-2 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-2 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-2 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-2 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-2 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-2 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-2 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-2 div.sk-item {position: relative;z-index: 1;}#sk-container-id-2 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-2 div.sk-item::before, #sk-container-id-2 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-2 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-2 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-2 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-2 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-2 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-2 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-2 div.sk-label-container {text-align: center;}#sk-container-id-2 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-2 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-2\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;dart&#x27;, callbacks=None,\n",
+                            "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
+                            "              early_stopping_rounds=None, enable_categorical=False,\n",
+                            "              eval_metric=&#x27;auc&#x27;, feature_types=None, gamma=1.2, gpu_id=-1,\n",
+                            "              grow_policy=&#x27;depthwise&#x27;, importance_type=None,\n",
+                            "              interaction_constraints=&#x27;&#x27;, learning_rate=0.300000012,\n",
+                            "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
+                            "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
+                            "              missing=nan, monotone_constraints=&#x27;()&#x27;, n_estimators=100,\n",
+                            "              n_jobs=0, num_parallel_tree=1, predictor=&#x27;auto&#x27;, random_state=0, ...)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-2\" type=\"checkbox\" checked><label for=\"sk-estimator-id-2\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">XGBClassifier</label><div class=\"sk-toggleable__content\"><pre>XGBClassifier(base_score=0.5, booster=&#x27;dart&#x27;, callbacks=None,\n",
+                            "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
+                            "              early_stopping_rounds=None, enable_categorical=False,\n",
+                            "              eval_metric=&#x27;auc&#x27;, feature_types=None, gamma=1.2, gpu_id=-1,\n",
+                            "              grow_policy=&#x27;depthwise&#x27;, importance_type=None,\n",
+                            "              interaction_constraints=&#x27;&#x27;, learning_rate=0.300000012,\n",
+                            "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
+                            "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
+                            "              missing=nan, monotone_constraints=&#x27;()&#x27;, n_estimators=100,\n",
+                            "              n_jobs=0, num_parallel_tree=1, predictor=&#x27;auto&#x27;, random_state=0, ...)</pre></div></div></div></div></div>"
                         ],
                         "text/plain": [
-                            "LinearRegression(fit_intercept=1)"
+                            "XGBClassifier(base_score=0.5, booster='dart', callbacks=None,\n",
+                            "              colsample_bylevel=1, colsample_bynode=1, colsample_bytree=1,\n",
+                            "              early_stopping_rounds=None, enable_categorical=False,\n",
+                            "              eval_metric='auc', feature_types=None, gamma=1.2, gpu_id=-1,\n",
+                            "              grow_policy='depthwise', importance_type=None,\n",
+                            "              interaction_constraints='', learning_rate=0.300000012,\n",
+                            "              max_bin=256, max_cat_threshold=64, max_cat_to_onehot=4,\n",
+                            "              max_delta_step=0, max_depth=4, max_leaves=0, min_child_weight=1,\n",
+                            "              missing=nan, monotone_constraints='()', n_estimators=100,\n",
+                            "              n_jobs=0, num_parallel_tree=1, predictor='auto', random_state=0, ...)"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "obj.best_estimator"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Get fitted randomized search object and its attributes"
+                "#### Get fitted search object and its attributes"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[FrozenTrial(number=0, values=[14.770921159757803], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 116678), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 140702), params={'fit_intercept': 0}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=0, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=1, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 119864), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 146285), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=1, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=2, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 134888), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 142868), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=2, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=3, values=[14.770921159757803], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 144494), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 162128), params={'fit_intercept': 0}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=3, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=4, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 147332), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 156348), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=4, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=5, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 149389), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 154259), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=5, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=6, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 157268), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 160401), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=6, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=7, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 160931), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 168608), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=7, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=8, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 162491), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 165954), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=8, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=9, values=[14.770921159757803], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 170690), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 174582), params={'fit_intercept': 0}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=9, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=10, values=[14.770921159757803], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 356206), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 374896), params={'fit_intercept': 0}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=10, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=11, values=[14.770921159757803], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 360423), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 365532), params={'fit_intercept': 0}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=11, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=12, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 366613), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 371635), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=12, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=13, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 376681), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 394411), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=13, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=14, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 377459), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 395807), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=14, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=15, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 380198), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 393857), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=15, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=16, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 380733), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 387668), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=16, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=17, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 396260), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 400771), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=17, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=18, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 396986), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 405781), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=18, state=TrialState.COMPLETE, value=None),\n",
-                            " FrozenTrial(number=19, values=[13.714193910659512], datetime_start=datetime.datetime(2023, 5, 2, 21, 19, 32, 407201), datetime_complete=datetime.datetime(2023, 5, 2, 21, 19, 32, 411127), params={'fit_intercept': 1}, distributions={'fit_intercept': IntUniformDistribution(high=True, low=False, step=1)}, user_attrs={}, system_attrs={}, intermediate_values={}, trial_id=19, state=TrialState.COMPLETE, value=None)]"
+                            "{'params': [{'booster': 'dart',\n",
+                            "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 4,\n",
+                            "   'gamma': 1.2,\n",
+                            "   'subsample': 0.8},\n",
+                            "  {'booster': 'dart',\n",
+                            "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 4,\n",
+                            "   'gamma': 1.2,\n",
+                            "   'subsample': 0.8},\n",
+                            "  {'booster': 'dart',\n",
+                            "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 5,\n",
+                            "   'gamma': 1.2,\n",
+                            "   'subsample': 0.5},\n",
+                            "  {'booster': 'gbtree',\n",
+                            "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 5,\n",
+                            "   'gamma': 0.1,\n",
+                            "   'subsample': 0.5},\n",
+                            "  {'booster': 'gbtree',\n",
+                            "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 5,\n",
+                            "   'gamma': 0.1,\n",
+                            "   'subsample': 0.5},\n",
+                            "  {'booster': 'gbtree',\n",
+                            "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 5,\n",
+                            "   'gamma': 1.2,\n",
+                            "   'subsample': 0.8},\n",
+                            "  {'booster': 'dart',\n",
+                            "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 5,\n",
+                            "   'gamma': 0.1,\n",
+                            "   'subsample': 0.5},\n",
+                            "  {'booster': 'dart',\n",
+                            "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 5,\n",
+                            "   'gamma': 0.1,\n",
+                            "   'subsample': 0.5},\n",
+                            "  {'booster': 'gbtree',\n",
+                            "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 4,\n",
+                            "   'gamma': 0.1,\n",
+                            "   'subsample': 0.8},\n",
+                            "  {'booster': 'gbtree',\n",
+                            "   'eval_metric': 'auc',\n",
+                            "   'max_depth': 4,\n",
+                            "   'gamma': 0.1,\n",
+                            "   'subsample': 0.5}],\n",
+                            " 'split0_test_score': array([0.69076305, 0.69076305, 0.67712177, 0.67364532, 0.67364532,\n",
+                            "        0.69173859, 0.67792447, 0.67792447, 0.68899225, 0.68037383]),\n",
+                            " 'split1_test_score': array([0.71076443, 0.71076443, 0.70124355, 0.69400245, 0.69400245,\n",
+                            "        0.71126112, 0.70055113, 0.70055113, 0.709335  , 0.7053021 ]),\n",
+                            " 'split2_test_score': array([0.70344407, 0.70344407, 0.69254093, 0.6846247 , 0.6846247 ,\n",
+                            "        0.69549218, 0.68693558, 0.68693558, 0.70357908, 0.69815951]),\n",
+                            " 'mean_test_score': array([0.70165718, 0.70165718, 0.69030209, 0.68409082, 0.68409082,\n",
+                            "        0.6994973 , 0.68847039, 0.68847039, 0.70063544, 0.69461181]),\n",
+                            " 'std_test_score': array([0.00826271, 0.00826271, 0.00997411, 0.00831933, 0.00831933,\n",
+                            "        0.00845825, 0.00930083, 0.00930083, 0.00856176, 0.01048155]),\n",
+                            " 'rank_test_score': array([1, 1, 6, 9, 9, 4, 7, 7, 3, 5], dtype=int32),\n",
+                            " 'time_total_s': array([19.87035179, 19.93525195, 21.30324793,  7.15872407,  7.15159893,\n",
+                            "         7.15376496, 21.14884591, 21.14350796,  4.81208324,  4.88412595]),\n",
+                            " 'training_iteration': array([1, 1, 1, 1, 1, 1, 1, 1, 1, 1]),\n",
+                            " 'param_booster': masked_array(data=['dart', 'dart', 'dart', 'gbtree', 'gbtree', 'gbtree',\n",
+                            "                    'dart', 'dart', 'gbtree', 'gbtree'],\n",
+                            "              mask=[False, False, False, False, False, False, False, False,\n",
+                            "                    False, False],\n",
+                            "        fill_value='?',\n",
+                            "             dtype=object),\n",
+                            " 'param_eval_metric': masked_array(data=['auc', 'auc', 'auc', 'auc', 'auc', 'auc', 'auc', 'auc',\n",
+                            "                    'auc', 'auc'],\n",
+                            "              mask=[False, False, False, False, False, False, False, False,\n",
+                            "                    False, False],\n",
+                            "        fill_value='?',\n",
+                            "             dtype=object),\n",
+                            " 'param_max_depth': masked_array(data=[4, 4, 5, 5, 5, 5, 5, 5, 4, 4],\n",
+                            "              mask=[False, False, False, False, False, False, False, False,\n",
+                            "                    False, False],\n",
+                            "        fill_value='?',\n",
+                            "             dtype=object),\n",
+                            " 'param_gamma': masked_array(data=[1.2, 1.2, 1.2, 0.1, 0.1, 1.2, 0.1, 0.1, 0.1, 0.1],\n",
+                            "              mask=[False, False, False, False, False, False, False, False,\n",
+                            "                    False, False],\n",
+                            "        fill_value='?',\n",
+                            "             dtype=object),\n",
+                            " 'param_subsample': masked_array(data=[0.8, 0.8, 0.5, 0.5, 0.5, 0.8, 0.5, 0.5, 0.8, 0.5],\n",
+                            "              mask=[False, False, False, False, False, False, False, False,\n",
+                            "                    False, False],\n",
+                            "        fill_value='?',\n",
+                            "             dtype=object)}"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "OptunaObj = obj.get_optimized_object()\n",
-                "OptunaObj.trials"
+                "GridSearchObj = obj.get_optimized_object()\n",
+                "GridSearchObj.cv_results_"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.10.4 ('.venv': poetry)",
             "language": "python",
```

### Comparing `lohrasb-3.6.0/lohrasb/examples/xgboost_survival_embeddings.ipynb` & `lohrasb-4.0.0/lohrasb/examples/xgboost_survival_embeddings.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9811971509577326%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '### XGBoost Survival Embeddings\\n')], delete: [0]}, "*

 * *            "'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 2: {'outputs': {0: "*

 * *            "{'text': ['\\x1b[31mERROR: Could not find a version that satisfies the requirement "*

 * *            "torch==1.12.1 (from versions: 2.0.0, 2.0.1)\\x1b[0m\\x1b[31m\\n', "*

 * *            "'\\x1b[0m\\x1b[31mERROR: No matching distribution found for "*

 * *            "torch==1.12.1\\x1b[0m\\x1b[31m\\n', '\\x1b[0m\\ […]*

```diff
@@ -1,19 +1,21 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## XGBoost Survival Embeddings\n",
+                "### XGBoost Survival Embeddings\n",
                 "\n",
                 "examples from : https://github.com/loft-br/xgboost-survival-embeddings"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Install Pytorch  and other imports"
             ]
         },
         {
@@ -21,25 +23,45 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: torch==1.12.1 in /usr/local/lib/python3.10/site-packages (1.12.1)\n",
-                        "Requirement already satisfied: typing-extensions in /usr/local/lib/python3.10/site-packages (from torch==1.12.1) (4.4.0)\n",
-                        "\n",
-                        "\u001b[1m[\u001b[0m\u001b[34;49mnotice\u001b[0m\u001b[1;39;49m]\u001b[0m\u001b[39;49m A new release of pip available: \u001b[0m\u001b[31;49m22.3.1\u001b[0m\u001b[39;49m -> \u001b[0m\u001b[32;49m23.0.1\u001b[0m\n",
-                        "\u001b[1m[\u001b[0m\u001b[34;49mnotice\u001b[0m\u001b[1;39;49m]\u001b[0m\u001b[39;49m To update, run: \u001b[0m\u001b[32;49mpython3.10 -m pip install --upgrade pip\u001b[0m\n",
-                        "2023-02-21 20:45:32,287 :: matplotlib :: matplotlib data path: /Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\n",
-                        "2023-02-21 20:45:32,294 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\n",
-                        "2023-02-21 20:45:32,296 :: matplotlib :: interactive is False\n",
-                        "2023-02-21 20:45:32,297 :: matplotlib :: platform is darwin\n",
-                        "2023-02-21 20:45:33,387 :: matplotlib :: CACHEDIR=/Users/hjavedani/.matplotlib\n",
-                        "2023-02-21 20:45:33,391 :: matplotlib.font_manager :: Using fontManager instance from /Users/hjavedani/.matplotlib/fontlist-v330.json\n"
+                        "\u001b[31mERROR: Could not find a version that satisfies the requirement torch==1.12.1 (from versions: 2.0.0, 2.0.1)\u001b[0m\u001b[31m\n",
+                        "\u001b[0m\u001b[31mERROR: No matching distribution found for torch==1.12.1\u001b[0m\u001b[31m\n",
+                        "\u001b[0m\n",
+                        "\u001b[1m[\u001b[0m\u001b[34;49mnotice\u001b[0m\u001b[1;39;49m]\u001b[0m\u001b[39;49m A new release of pip is available: \u001b[0m\u001b[31;49m23.0.1\u001b[0m\u001b[39;49m -> \u001b[0m\u001b[32;49m23.1.2\u001b[0m\n",
+                        "\u001b[1m[\u001b[0m\u001b[34;49mnotice\u001b[0m\u001b[1;39;49m]\u001b[0m\u001b[39;49m To update, run: \u001b[0m\u001b[32;49mpython3.11 -m pip install --upgrade pip\u001b[0m\n",
+                        "2023-07-11 08:42:21,736 :: matplotlib :: matplotlib data path: /Users/hjavedani/Documents/Lohrasb/.venv/lib/python3.10/site-packages/matplotlib/mpl-data\n",
+                        "2023-07-11 08:42:21,742 :: matplotlib :: CONFIGDIR=/Users/hjavedani/.matplotlib\n",
+                        "2023-07-11 08:42:21,745 :: matplotlib :: interactive is False\n",
+                        "2023-07-11 08:42:21,746 :: matplotlib :: platform is darwin\n",
+                        "2023-07-11 08:42:21,761 :: graphviz._tools :: deprecate positional args: graphviz.backend.piping.pipe(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-11 08:42:21,763 :: graphviz._tools :: deprecate positional args: graphviz.backend.rendering.render(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-11 08:42:21,765 :: graphviz._tools :: deprecate positional args: graphviz.backend.unflattening.unflatten(['stagger', 'fanout', 'chain', 'encoding'])\n",
+                        "2023-07-11 08:42:21,767 :: graphviz._tools :: deprecate positional args: graphviz.backend.viewing.view(['quiet'])\n",
+                        "2023-07-11 08:42:21,770 :: graphviz._tools :: deprecate positional args: graphviz.quoting.quote(['is_html_string', 'is_valid_id', 'dot_keywords', 'endswith_odd_number_of_backslashes', 'escape_unescaped_quotes'])\n",
+                        "2023-07-11 08:42:21,771 :: graphviz._tools :: deprecate positional args: graphviz.quoting.a_list(['kwargs', 'attributes'])\n",
+                        "2023-07-11 08:42:21,772 :: graphviz._tools :: deprecate positional args: graphviz.quoting.attr_list(['kwargs', 'attributes'])\n",
+                        "2023-07-11 08:42:21,772 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.clear(['keep_attrs'])\n",
+                        "2023-07-11 08:42:21,773 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.__iter__(['subgraph'])\n",
+                        "2023-07-11 08:42:21,774 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.node(['_attributes'])\n",
+                        "2023-07-11 08:42:21,777 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.edge(['_attributes'])\n",
+                        "2023-07-11 08:42:21,779 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.attr(['_attributes'])\n",
+                        "2023-07-11 08:42:21,782 :: graphviz._tools :: deprecate positional args: graphviz.dot.Dot.subgraph(['name', 'comment', 'graph_attr', 'node_attr', 'edge_attr', 'body'])\n",
+                        "2023-07-11 08:42:21,785 :: graphviz._tools :: deprecate positional args: graphviz.piping.Pipe._pipe_legacy(['renderer', 'formatter', 'neato_no_op', 'quiet'])\n",
+                        "2023-07-11 08:42:21,789 :: graphviz._tools :: deprecate positional args: graphviz.saving.Save.save(['directory'])\n",
+                        "2023-07-11 08:42:21,790 :: graphviz._tools :: deprecate positional args: graphviz.rendering.Render.render(['directory', 'view', 'cleanup', 'format', 'renderer', 'formatter', 'neato_no_op', 'quiet', 'quiet_view'])\n",
+                        "2023-07-11 08:42:21,791 :: graphviz._tools :: deprecate positional args: graphviz.rendering.Render.view(['directory', 'cleanup', 'quiet', 'quiet_view'])\n",
+                        "2023-07-11 08:42:21,793 :: graphviz._tools :: deprecate positional args: graphviz.unflattening.Unflatten.unflatten(['stagger', 'fanout', 'chain'])\n",
+                        "2023-07-11 08:42:21,794 :: graphviz._tools :: deprecate positional args: graphviz.graphs.BaseGraph.__init__(['comment', 'filename', 'directory', 'format', 'engine', 'encoding', 'graph_attr', 'node_attr', 'edge_attr', 'body', 'strict'])\n",
+                        "2023-07-11 08:42:21,796 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.from_file(['directory', 'format', 'engine', 'encoding', 'renderer', 'formatter'])\n",
+                        "2023-07-11 08:42:21,797 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.__init__(['filename', 'directory', 'format', 'engine', 'encoding'])\n",
+                        "2023-07-11 08:42:21,797 :: graphviz._tools :: deprecate positional args: graphviz.sources.Source.save(['directory'])\n"
                     ]
                 }
             ],
             "source": [
                 "\n",
                 "! pip3 install torch==1.12.1\n",
                 "import sys\n",
@@ -59,22 +81,24 @@
                 "    XGBSEKaplanNeighbors,\n",
                 "    XGBSEKaplanTree,\n",
                 "    XGBSEBootstrapEstimator\n",
                 ")\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Example : XGBoost Survival Embeddings (XGBSEKaplanNeighbors)\n",
                 "  \n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For more information refer to this link : https://loft-br.github.io/xgboost-survival-embeddings/examples/confidence_interval.html\n",
                 "\n"
             ]
         },
@@ -83,18 +107,18 @@
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2023-02-21 20:45:34,011 :: h5py._conv :: Creating converter from 7 to 5\n",
-                        "2023-02-21 20:45:34,011 :: h5py._conv :: Creating converter from 5 to 7\n",
-                        "2023-02-21 20:45:34,012 :: h5py._conv :: Creating converter from 7 to 5\n",
-                        "2023-02-21 20:45:34,013 :: h5py._conv :: Creating converter from 5 to 7\n"
+                        "2023-07-11 08:42:22,753 :: h5py._conv :: Creating converter from 7 to 5\n",
+                        "2023-07-11 08:42:22,754 :: h5py._conv :: Creating converter from 5 to 7\n",
+                        "2023-07-11 08:42:22,755 :: h5py._conv :: Creating converter from 7 to 5\n",
+                        "2023-07-11 08:42:22,755 :: h5py._conv :: Creating converter from 5 to 7\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -227,14 +251,15 @@
                 "from pycox.datasets import metabric\n",
                 "# read data metabric\n",
                 "df = metabric.read_df()\n",
                 "df.head()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Define labels and train-test split \n"
             ]
         },
         {
@@ -250,14 +275,15 @@
                 "# splitting between train, and validation \n",
                 "(X_train, X_test,\n",
                 " y_train, y_test) = \\\n",
                 "train_test_split(X, y, test_size=0.2, random_state=42)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Example 1: Basic usage\n"
             ]
         },
         {
@@ -273,44 +299,54 @@
                 "estimator_params ={\n",
                 "     'n_neighbors': [50,70],\n",
                 "}\n",
                 "#xgbse_model.fit(X, y)\n",
                 "\n",
                 "# predicting\n",
                 "#event_probs = xgbse_model.predict(X)\n",
-                "# event_probs.head()"
+                "# event_probs.head()\n",
+                "\n",
+                "kwargs = {  # extra params for model if any\n",
+                "            'main_random_kwargs':{},\n",
+                "            # params for RandomSearchCV \n",
+                "            'random_search_kwargs' : {\n",
+                "            'estimator':estimator,\n",
+                "            'param_distributions':estimator_params,\n",
+                "            'scoring': make_scorer(concordance_index, greater_is_better=True),\n",
+                "            'n_jobs':-1,\n",
+                "            'cv':KFold(2),\n",
+                "            'n_iter':2,\n",
+                "            'random_state' : 42,\n",
+                "            'refit':True,\n",
+                "            }\n",
+                "            }\n",
+                "\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Define BestModel optimzed by random search"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "obj = BaseModel().optimize_by_randomsearchcv(\n",
-                "            estimator=estimator,\n",
-                "            fit_params = fit_params,\n",
-                "            estimator_params=estimator_params,\n",
-                "            measure_of_accuracy=make_scorer(concordance_index, greater_is_better=True),\n",
-                "            verbose=3,\n",
-                "            n_jobs=-1,\n",
-                "            n_iter=2,\n",
-                "            random_state=42,\n",
-                "            cv=KFold(2),\n",
+                " kwargs=kwargs\n",
                 "        )\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Define Pipeline and predict"
             ]
         },
         {
@@ -318,37 +354,31 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2023-02-21 20:45:34,909 :: dev :: The optimization will be based on make_scorer(concordance_index) metric!\n",
-                        "2023-02-21 20:45:34,909 :: dev :: The optimization will be based on make_scorer(concordance_index) metric!\n",
-                        "Fitting 2 folds for each of 2 candidates, totalling 4 fits\n",
-                        "[CV 1/2] END ....................n_neighbors=50;, score=0.631 total time= 4.1min\n",
-                        "[CV 2/2] END ....................n_neighbors=50;, score=0.622 total time=  43.7s\n",
-                        "[CV 1/2] END ....................n_neighbors=70;, score=0.632 total time=  48.6s\n",
-                        "[CV 2/2] END ....................n_neighbors=70;, score=0.619 total time=  52.4s\n",
-                        "2023-02-21 20:52:56,014 :: dev :: The optimization will be based on make_scorer(concordance_index) metric!\n",
-                        "2023-02-21 20:52:56,014 :: dev :: The optimization will be based on make_scorer(concordance_index) metric!\n"
+                        "2023-07-11 08:44:28,015 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n",
+                        "2023-07-11 08:44:28,015 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n"
                     ]
                 }
             ],
             "source": [
                 "pipeline =Pipeline([\n",
                 "            ('obj', obj)\n",
                 "\n",
                 " ])\n",
                 "\n",
                 "pipeline.fit(X_train,y_train)\n",
                 "y_pred = pipeline.predict(X_test)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Metrics"
             ]
         },
         {
@@ -369,14 +399,15 @@
                 "\n",
                 "\n",
                 "print(f'C-index: {concordance_index(y_test, y_pred)}')\n",
                 "print(f'Avg. Brier Score: {approx_brier_score(y_test, y_pred)}')\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Example 2: Define estimator and set its arguments \n"
             ]
         },
         {
@@ -409,14 +440,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "TIME_BINS = np.arange(15, 315, 15)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Define estimator and fit params\n"
             ]
         },
         {
@@ -426,42 +458,53 @@
             "outputs": [],
             "source": [
                 "estimator=XGBSEBootstrapEstimator(base_model)\n",
                 "fit_params = {\"time_bins\":TIME_BINS}\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Define BaseModel estimator using random search CV"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
+                "kwargs = {  \n",
+                "            # params for RandomSearchCV \n",
+                "            'main_random_kwargs':{},\n",
+                "            'fit_random_kwargs' : fit_params,\n",
+                "            'random_search_kwargs' : {\n",
+                "            'estimator':estimator,\n",
+                "            'param_distributions':estimator_params,\n",
+                "            'scoring': make_scorer(approx_brier_score, greater_is_better=False),\n",
+                "            'n_jobs':-1,\n",
+                "            'cv':KFold(2),\n",
+                "            'n_iter':2,\n",
+                "            'random_state' : 42,\n",
+                "            'refit':True,\n",
+                "            }\n",
+                "            }\n",
+                "\n",
                 "\n",
                 "obj = BaseModel().optimize_by_randomsearchcv(\n",
-                "            estimator=estimator,\n",
-                "            fit_params = fit_params,\n",
-                "            estimator_params=estimator_params,\n",
-                "            measure_of_accuracy=make_scorer(approx_brier_score, greater_is_better=False),\n",
-                "            verbose=3,\n",
-                "            n_jobs=-1,\n",
-                "            n_iter=2,\n",
-                "            random_state=42,\n",
-                "            cv=KFold(2),\n",
+                "        kwargs=kwargs\n",
                 "        )\n",
+                "\n",
                 "\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Build sklearn pipeline"
             ]
         },
         {
@@ -475,14 +518,15 @@
                 "pipeline =Pipeline([\n",
                 "            ('obj', obj)\n",
                 "\n",
                 " ])\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Run Pipeline"
             ]
         },
         {
@@ -490,32 +534,26 @@
             "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2023-02-21 20:52:56,942 :: dev :: The optimization will be based on make_scorer(approx_brier_score, greater_is_better=False) metric!\n",
-                        "2023-02-21 20:52:56,942 :: dev :: The optimization will be based on make_scorer(approx_brier_score, greater_is_better=False) metric!\n",
-                        "Fitting 2 folds for each of 2 candidates, totalling 4 fits\n",
-                        "[CV 1/2] END .................n_estimators=100;, score=-0.173 total time=   3.1s\n",
-                        "[CV 2/2] END .................n_estimators=100;, score=-0.179 total time=   2.8s\n",
-                        "[CV 1/2] END .................n_estimators=200;, score=-0.173 total time=   5.4s\n",
-                        "[CV 2/2] END .................n_estimators=200;, score=-0.179 total time=   5.2s\n",
-                        "2023-02-21 20:53:20,125 :: dev :: The optimization will be based on make_scorer(approx_brier_score, greater_is_better=False) metric!\n",
-                        "2023-02-21 20:53:20,125 :: dev :: The optimization will be based on make_scorer(approx_brier_score, greater_is_better=False) metric!\n"
+                        "2023-07-11 08:44:45,880 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n",
+                        "2023-07-11 08:44:45,880 :: dev :: If refit is set to True, the optimal model will be refit on the entire dataset again!\n"
                     ]
                 }
             ],
             "source": [
                 "pipeline.fit(X_train,y_train)\n",
                 "y_pred = pipeline.predict(X_test)\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Check performance of the pipeline"
             ]
         },
         {
@@ -550,15 +588,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.10.11"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "7ced68e88e9060e5bcf2eaa5b2d4f8fc97e4d610a52d347137abf879072ffb6d"
             }
         }
```

### Comparing `lohrasb-3.6.0/pyproject.toml` & `lohrasb-4.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # project configuration, use poetry
 [tool.poetry]
 name = "lohrasb"
-version = "3.6.0"
-description = "A scalable estimator optimization tool compatible with scikit-learn APIs"
+version = "4.0.0"
+description = "This versatile tool streamlines hyperparameter optimization in machine learning workflows. It supports a wide range of search methods, from GridSearchCV and RandomizedSearchCV to advanced techniques like OptunaSearchCV, Ray Tune, and Scikit-Learn Tune. Designed to enhance model performance and efficiency, it's suitable for tasks of any scale."
 authors = ["drhosseinjavedani <h.javedani@gmail.com>"]
 homepage = "https://github.com/drhosseinjavedani/lohrasb"
 license = "BSD-3-Clause license"
 
 readme = "README.md"
 keywords = [
     "Auto ML",
@@ -15,15 +15,15 @@
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 numpy = "^1.20"
 scipy = "^1.5"
-optuna = "^2.10.1"
+optuna = "^3.2.0"
 xgboost = "^1.6.1"
 imblearn = "^0.0"
 lightgbm = "^3.3.2"
 nox = "^2022.1.7"
 feature-engine = "^1.4.1"
 category-encoders = "^2.5.0"
 pandas = "^1.4"
@@ -34,24 +34,28 @@
 interpret = "^0.3.0"
 python-dotenv = "^0.21.1"
 ray = {extras = ["tune"], version = "^2.2.0"}
 tune-sklearn = "^0.4.5"
 protobuf = "3.20"
 hyperopt = "^0.2.7"
 scikit-optimize = "^0.9.0"
+bayesian-optimization = "^1.4.3"
+catboost = "^1.2"
+dill = "^0.3.6"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 black = "^22.6.0"
 nox = "^2022.1.7"
 bump2version = "^1.0.1"
 isort = "^5.10.1"
 pytest = "^7.1.2"
 ipykernel = "^6.15.2"
 
 [tool.poetry.group.dev.dependencies]
 IProgress = "^0.4"
 jupyter = "^1.0.0"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

