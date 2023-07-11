# Comparing `tmp/autora-theorist-bms-1.0.1.tar.gz` & `tmp/autora-theorist-bms-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-bms-1.0.1.tar", last modified: Mon Jul  3 18:48:39 2023, max compression
+gzip compressed data, was "autora-theorist-bms-1.0.2.tar", last modified: Tue Jul 11 16:15:39 2023, max compression
```

## Comparing `autora-theorist-bms-1.0.1.tar` & `autora-theorist-bms-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.852536 autora-theorist-bms-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.840536 autora-theorist-bms-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.844536 autora-theorist-bms-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 18:48:39.848536 autora-theorist-bms-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.844536 autora-theorist-bms-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    34190 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/how-it-works.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.844536 autora-theorist-bms-1.0.1/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   191653 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/img/BMSEquationTreeOps.png
--rw-r--r--   0 runner    (1001) docker     (123)   503083 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/img/BMSTempering.png
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.844536 autora-theorist-bms-1.0.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/meta-parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/search-space.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.844536 autora-theorist-bms-1.0.1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 18:48:39.852536 autora-theorist-bms-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.840536 autora-theorist-bms-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.840536 autora-theorist-bms-1.0.1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.840536 autora-theorist-bms-1.0.1/src/autora/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.848536 autora-theorist-bms-1.0.1/src/autora/theorist/bms/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/fit_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)    60423 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/regressor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2860 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.848536 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 18:48:39.000000 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 18:48:39.000000 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:48:39.000000 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-03 18:48:39.000000 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 18:48:39.000000 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.848536 autora-theorist-bms-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/tests/test_sklearn_bms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    34190 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/how-it-works.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   191653 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/img/BMSEquationTreeOps.png
+-rw-r--r--   0 runner    (1001) docker     (123)   503083 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/img/BMSTempering.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/meta-parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/search-space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/src/autora/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/src/autora/theorist/bms/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/fit_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60697 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/regressor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2124 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-11 16:15:39.000000 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-11 16:15:39.000000 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:15:39.000000 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 16:15:39.000000 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 16:15:39.000000 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/tests/test_sklearn_bms.py
```

### Comparing `autora-theorist-bms-1.0.1/.github/workflows/python-publish.yml` & `autora-theorist-bms-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/.gitignore` & `autora-theorist-bms-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/.pre-commit-config.yaml` & `autora-theorist-bms-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/PKG-INFO` & `autora-theorist-bms-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-bms
-Version: 1.0.1
+Version: 1.0.2
 Summary: Bayesian Machine Scientist theorist for AutoRA
 Author-email: Joshua Hewson <joshua_hewson@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-bms
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-bms-1.0.1/README.md` & `autora-theorist-bms-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/docs/Basic Usage.ipynb` & `autora-theorist-bms-1.0.2/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/docs/how-it-works.md` & `autora-theorist-bms-1.0.2/docs/how-it-works.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/docs/img/BMSEquationTreeOps.png` & `autora-theorist-bms-1.0.2/docs/img/BMSEquationTreeOps.png`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/docs/img/BMSTempering.png` & `autora-theorist-bms-1.0.2/docs/img/BMSTempering.png`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/docs/index.md` & `autora-theorist-bms-1.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/docs/meta-parameters.md` & `autora-theorist-bms-1.0.2/docs/meta-parameters.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/docs/search-space.md` & `autora-theorist-bms-1.0.2/docs/search-space.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/mkdocs/base.yml` & `autora-theorist-bms-1.0.2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/pyproject.toml` & `autora-theorist-bms-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "tqdm",
     "sympy",
 ]
 
 [project.optional-dependencies]
 dev = [
     "autora-core[dev]",
-    "autora-synthetic-data"
+    "autora-synthetic"
 ]
 
 [project.urls]
 homepage = "http://www.empiricalresearch.ai"
 repository = "https://github.com/AutoResearch/autora-theorist-bms"
 documentation = "https://autoresearch.github.io/autora/"
```

### Comparing `autora-theorist-bms-1.0.1/src/autora/theorist/bms/fit_prior.py` & `autora-theorist-bms-1.0.2/src/autora/theorist/bms/fit_prior.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/src/autora/theorist/bms/mcmc.py` & `autora-theorist-bms-1.0.2/src/autora/theorist/bms/mcmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -697,14 +697,18 @@
                     raise ValueError
                 else:
                     self.sse[ds] = np.sum(se)
             except ValueError:
                 if verbose:
                     print("> Cannot calculate SSE for %s: inf" % self, file=sys.stderr)
                 self.sse[ds] = np.inf
+            except TypeError:
+                if verbose:
+                    print("Complex-valued parameters are invalid")
+                self.sse[ds] = np.inf
 
         # Done
         return self.sse
 
     # -------------------------------------------------------------------------
     def get_bic(self, reset=True, fit=False, verbose=False):
         """
@@ -721,19 +725,20 @@
         # Get the sum of squared errors (fitting, if required)
         sse = self.get_sse(fit=fit, verbose=verbose)
         # Calculate the BIC
         parameters = set([p.value for p in self.ets[0] if p.value in self.parameters])
         k = 1 + len(parameters)
         BIC = 0.0
         for ds in self.y:
-            n = len(self.y[ds])
-            BIC += (k - n) * np.log(n) + n * (np.log(2.0 * np.pi) + log(sse[ds]) + 1)
-        for ds in self.y:
             if sse[ds] == 0.0:
                 BIC = -np.inf
+                break
+            else:
+                n = len(self.y[ds])
+                BIC += (k - n) * np.log(n) + n * (np.log(2.0 * np.pi) + log(sse[ds]) + 1)
         if reset:
             self.bic = BIC
         return BIC
 
     # -------------------------------------------------------------------------
     def get_energy(self, bic=False, reset=False, verbose=False):
         """
@@ -786,14 +791,16 @@
             1: we haven't seen this canonical form before
             -1: we have seen this equation's canonical form before but it isn't in that form yet
         """
         # Check for canonical representative
         canonical = self.canonical(verbose=verbose)
         try:  # We've seen this canonical before!
             rep, rep_energy, rep_par_values = self.representative[canonical]
+        except TypeError:
+            return -1  # Complex-valued parameters are invalid
         except KeyError:  # Never seen this canonical formula before:
             # save it and return 1
             self.get_bic(reset=True, fit=True, verbose=verbose)
             new_energy = self.get_energy(bic=False, verbose=verbose)
             self.representative[canonical] = (
                 str(self),
                 new_energy,
```

### Comparing `autora-theorist-bms-1.0.1/src/autora/theorist/bms/parallel.py` & `autora-theorist-bms-1.0.2/src/autora/theorist/bms/parallel.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/src/autora/theorist/bms/prior.py` & `autora-theorist-bms-1.0.2/src/autora/theorist/bms/prior.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/src/autora/theorist/bms/regressor.py` & `autora-theorist-bms-1.0.2/src/autora/theorist/bms/regressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     and a pre-defined number of parameters
 
     This class is intended to be compatible with the
     [Scikit-Learn Estimator API](https://scikit-learn.org/stable/developers/develop.html).
 
     Examples:
 
-        >>> from autora.theorist.bms import Parallel, utils
+        >>> from autora.theorist.bms import Parallel
         >>> import numpy as np
         >>> num_samples = 1000
         >>> X = np.linspace(start=0, stop=1, num=num_samples).reshape(-1, 1)
         >>> y = 15. * np.ones(num_samples)
         >>> estimator = BMSRegressor()
         >>> estimator = estimator.fit(X, y)
         >>> estimator.predict([[15.]])
@@ -170,16 +170,25 @@
         check_is_fitted(self, attributes=["model_", "loss_", "cache_"])
         assert self.model_ is not None
         assert self.loss_ is not None
         assert self.cache_ is not None
 
         utils.present_results(self.model_, self.loss_, self.cache_)
 
-    def repr(self):
-        return self.model_.__repr__()
+    def __repr__(self):
+        return self.repr()
+
+    def repr(self, decimals=2):
+        model_str = self.model_.__repr__()
+        parameter_names = self.model_.parameters
+        parameter_values = self.model_.par_values
+        for name in parameter_names:
+            value = parameter_values["d0"][name]
+            model_str = model_str.replace(name, str(np.round(value, decimals=decimals)))
+        return model_str
 
     def latex(self):
         return self.model_.latex()
 
     def add_primitive(self, op: Callable):
         self.custom_ops.update({op.__name__: op})
         self.ops.update({op.__name__: len(signature(op).parameters)})
```

### Comparing `autora-theorist-bms-1.0.1/src/autora/theorist/bms/utils.py` & `autora-theorist-bms-1.0.2/src/autora/theorist/bms/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -59,31 +59,7 @@
     print("Desc. length:\t", model_len)
     plt.figure(figsize=(15, 5))
     plt.plot(desc_len)
     plt.xlabel("MCMC step", fontsize=14)
     plt.ylabel("Description length", fontsize=14)
     plt.title("MDL model: $%s$" % model.latex())
     plt.show()
-
-
-def predict(model: Tree, x: pd.DataFrame, y: pd.DataFrame) -> dict:
-    """
-    Maps independent variable data onto expected dependent variable data
-
-    Args:
-        model: The equation / function that best maps x onto y
-        x: The independent variables of the data
-        y: The dependent variable of the data
-
-    Returns: Predicted values for y given x and the model as trained
-    """
-    plt.figure(figsize=(6, 6))
-    plt.scatter(model.predict(x), y)
-
-    all_y = np.append(y, model.predict(x))
-    y_range = all_y.min().item(), all_y.max().item()
-    plt.plot(y_range, y_range)
-
-    plt.xlabel("MDL model predictions", fontsize=14)
-    plt.ylabel("Actual values", fontsize=14)
-    plt.show()
-    return model.predict(x)
```

### Comparing `autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/PKG-INFO` & `autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-bms
-Version: 1.0.1
+Version: 1.0.2
 Summary: Bayesian Machine Scientist theorist for AutoRA
 Author-email: Joshua Hewson <joshua_hewson@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-bms
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/SOURCES.txt` & `autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/tests/README.md` & `autora-theorist-bms-1.0.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.1/tests/test_sklearn_bms.py` & `autora-theorist-bms-1.0.2/tests/test_sklearn_bms.py`

 * *Files identical despite different names*

