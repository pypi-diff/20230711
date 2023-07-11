# Comparing `tmp/autora-synthetic-1.0.2.tar.gz` & `tmp/autora-synthetic-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-synthetic-1.0.2.tar", last modified: Thu Jun  1 22:55:46 2023, max compression
+gzip compressed data, was "autora-synthetic-1.0.3.tar", last modified: Tue Jul 11 16:14:40 2023, max compression
```

## Comparing `autora-synthetic-1.0.2.tar` & `autora-synthetic-1.0.3.tar`

### file list

```diff
@@ -1,48 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.642861 autora-synthetic-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.638861 autora-synthetic-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.638861 autora-synthetic-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.638861 autora-synthetic-1.0.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/.idea/autora-synthetic.iml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-01 22:55:46.642861 autora-synthetic-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.638861 autora-synthetic-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   171038 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/docs/Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.638861 autora-synthetic-1.0.2/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.638861 autora-synthetic-1.0.2/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 22:55:46.642861 autora-synthetic-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.638861 autora-synthetic-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.638861 autora-synthetic-1.0.2/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.638861 autora-synthetic-1.0.2/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.642861 autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.642861 autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/abstract/template_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.642861 autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/economics/
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/economics/expected_value_theory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/economics/prospect_theory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.642861 autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/psychophysics/
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.642861 autora-synthetic-1.0.2/src/autora_synthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-01 22:55:46.000000 autora-synthetic-1.0.2/src/autora_synthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-01 22:55:46.000000 autora-synthetic-1.0.2/src/autora_synthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 22:55:46.000000 autora-synthetic-1.0.2/src/autora_synthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 22:55:46.000000 autora-synthetic-1.0.2/src/autora_synthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 22:55:46.000000 autora-synthetic-1.0.2/src/autora_synthetic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:55:46.642861 autora-synthetic-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/tests/test_bundled_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-01 22:55:35.000000 autora-synthetic-1.0.2/tests/test_synthetic_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.612998 autora-synthetic-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.600997 autora-synthetic-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.608997 autora-synthetic-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-11 16:14:40.612998 autora-synthetic-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.608997 autora-synthetic-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   171036 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/docs/Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.608997 autora-synthetic-1.0.3/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.608997 autora-synthetic-1.0.3/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:14:40.612998 autora-synthetic-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.604997 autora-synthetic-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.600997 autora-synthetic-1.0.3/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.600997 autora-synthetic-1.0.3/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.608997 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.608997 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/abstract/template_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.608997 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/economics/
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/economics/expected_value_theory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/economics/prospect_theory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.612998 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/psychology/
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/psychology/luce_choice_ratio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.612998 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/psychophysics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.612998 autora-synthetic-1.0.3/src/autora_synthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-11 16:14:40.000000 autora-synthetic-1.0.3/src/autora_synthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-11 16:14:40.000000 autora-synthetic-1.0.3/src/autora_synthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:14:40.000000 autora-synthetic-1.0.3/src/autora_synthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 16:14:40.000000 autora-synthetic-1.0.3/src/autora_synthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 16:14:40.000000 autora-synthetic-1.0.3/src/autora_synthetic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:14:40.612998 autora-synthetic-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/tests/test_bundled_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-11 16:14:29.000000 autora-synthetic-1.0.3/tests/test_synthetic_inventory.py
```

### Comparing `autora-synthetic-1.0.2/.github/workflows/python-publish.yml` & `autora-synthetic-1.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/.github/workflows/test-pytest.yml` & `autora-synthetic-1.0.3/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/.gitignore` & `autora-synthetic-1.0.3/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -63,7 +63,10 @@
 
 # Material for MkDocs
 site/
 docs/reference/
 
 # Jupyter Notebook load data
 .ipynb_checkpoints
+# IDE-specific directories
+.idea
+
```

### Comparing `autora-synthetic-1.0.2/.pre-commit-config.yaml` & `autora-synthetic-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/CONTRIBUTING.md` & `autora-synthetic-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/PKG-INFO` & `autora-synthetic-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-synthetic
-Version: 1.0.2
+Version: 1.0.3
 Summary: AutoRA Synthetic Experiments
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-synthetic
 Project-URL: documentation, https://autoresearch.github.io/autora-synthetic/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `autora-synthetic-1.0.2/README.md` & `autora-synthetic-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/docs/Example.ipynb` & `autora-synthetic-1.0.3/docs/Example.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999250374812594%*

 * *Differences: {"'cells'": "{21: {'source': {insert: [(3, 'from autora.experimentalist.sampler.random_sampler "*

 * *            "import random_sample\\n'), (9, 'sampler = partial(random_sample, n=20)\\n')], delete: "*

 * *            '[9, 3]}}}'}*

```diff
@@ -348,21 +348,21 @@
                     ]
                 }
             ],
             "source": [
                 "from autora.workflow.protocol import ResultKind\n",
                 "from autora.experimentalist.pipeline import make_pipeline\n",
                 "from autora.experimentalist.pooler.grid import grid_pool\n",
-                "from autora.experimentalist.sampler.random_sampler import random_sampler\n",
+                "from autora.experimentalist.sampler.random_sampler import random_sample\n",
                 "from functools import partial\n",
                 "import random\n",
                 "variables = s.variables\n",
                 "pool = partial(grid_pool, ivs=variables.independent_variables)\n",
                 "random.seed(181) # set the seed for the random sampler\n",
-                "sampler = partial(random_sampler, n=20)\n",
+                "sampler = partial(random_sample, n=20)\n",
                 "experimentalist_pipeline = make_pipeline([pool, sampler])\n",
                 "\n",
                 "from autora.workflow import Controller\n",
                 "theorist = LinearRegression()\n",
                 "\n",
                 "cycle = Controller(\n",
                 "    variables=variables, experimentalist=experimentalist_pipeline,\n",
```

### Comparing `autora-synthetic-1.0.2/docs/index.md` & `autora-synthetic-1.0.3/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
 Install the synthetic data package:
 
 ```shell
-pip install -U "autora
+pip install -U "autora"
 ```
 
 !!! success
     It is recommended to use a `python` environment manager like `virtualenv`.
 
 Print a description of the prospect theory model by Kahneman and Tversky by running:
 ```shell
```

### Comparing `autora-synthetic-1.0.2/mkdocs/base.yml` & `autora-synthetic-1.0.3/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/pyproject.toml` & `autora-synthetic-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/abstract/template_experiment.py` & `autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/abstract/template_experiment.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/economics/expected_value_theory.py` & `autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/economics/expected_value_theory.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/economics/prospect_theory.py` & `autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/economics/prospect_theory.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py` & `autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/src/autora/experiment_runner/synthetic/utilities.py` & `autora-synthetic-1.0.3/src/autora/experiment_runner/synthetic/utilities.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.2/src/autora_synthetic.egg-info/PKG-INFO` & `autora-synthetic-1.0.3/src/autora_synthetic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-synthetic
-Version: 1.0.2
+Version: 1.0.3
 Summary: AutoRA Synthetic Experiments
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-synthetic
 Project-URL: documentation, https://autoresearch.github.io/autora-synthetic/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `autora-synthetic-1.0.2/src/autora_synthetic.egg-info/SOURCES.txt` & `autora-synthetic-1.0.3/src/autora_synthetic.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,27 +3,23 @@
 CONTRIBUTING.md
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/docs-publish.yml
 .github/workflows/python-publish.yml
 .github/workflows/test-pytest.yml
-.idea/.gitignore
-.idea/autora-synthetic.iml
-.idea/misc.xml
-.idea/modules.xml
-.idea/vcs.xml
 docs/Example.ipynb
 docs/index.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
 src/autora/experiment_runner/synthetic/utilities.py
 src/autora/experiment_runner/synthetic/abstract/template_experiment.py
 src/autora/experiment_runner/synthetic/economics/expected_value_theory.py
 src/autora/experiment_runner/synthetic/economics/prospect_theory.py
+src/autora/experiment_runner/synthetic/psychology/luce_choice_ratio.py
 src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py
 src/autora_synthetic.egg-info/PKG-INFO
 src/autora_synthetic.egg-info/SOURCES.txt
 src/autora_synthetic.egg-info/dependency_links.txt
 src/autora_synthetic.egg-info/requires.txt
 src/autora_synthetic.egg-info/top_level.txt
 tests/test_bundled_models.py
```

### Comparing `autora-synthetic-1.0.2/tests/test_bundled_models.py` & `autora-synthetic-1.0.3/tests/test_bundled_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 from autora.experiment_runner.synthetic.abstract.template_experiment import (
     template_experiment,
 )
 from autora.experiment_runner.synthetic.economics.expected_value_theory import (
     expected_value_theory,
 )
 from autora.experiment_runner.synthetic.economics.prospect_theory import prospect_theory
+from autora.experiment_runner.synthetic.psychology.luce_choice_ratio import (
+    luce_choice_ratio,
+)
 from autora.experiment_runner.synthetic.psychophysics.weber_fechner_law import (
     weber_fechner_law,
 )
 from autora.experiment_runner.synthetic.utilities import describe, register, retrieve
 
 all_bundled_models = [
     ("expected_value_theory", expected_value_theory),
     ("prospect_theory", prospect_theory),
+    ("luce_choice_ratio", luce_choice_ratio),
     ("template_experiment", template_experiment),
     ("weber_fechner_law", weber_fechner_law),
 ]
 
 all_bundled_model_names = [b[0] for b in all_bundled_models]
 
 for name, func in all_bundled_models:
```

### Comparing `autora-synthetic-1.0.2/tests/test_synthetic_inventory.py` & `autora-synthetic-1.0.3/tests/test_synthetic_inventory.py`

 * *Files identical despite different names*

