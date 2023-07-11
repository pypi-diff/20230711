# Comparing `tmp/statease-0.2.8.tar.gz` & `tmp/statease-0.2.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statease-0.2.8.tar", last modified: Thu Feb  9 16:37:08 2023, max compression
+gzip compressed data, was "statease-0.2.9.dev2.tar", last modified: Tue Jul 11 15:52:16 2023, max compression
```

## Comparing `statease-0.2.8.tar` & `statease-0.2.9.dev2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 handerson   (501) staff       (20)        0 2023-02-09 16:37:08.879621 statease-0.2.8/
--rw-r--r--   0 handerson   (501) staff       (20)     5896 2022-03-02 15:06:20.000000 statease-0.2.8/LICENSE
--rw-r--r--   0 handerson   (501) staff       (20)     1376 2023-02-09 16:37:08.879493 statease-0.2.8/PKG-INFO
--rw-r--r--   0 handerson   (501) staff       (20)      406 2022-03-02 15:06:20.000000 statease-0.2.8/README.md
--rw-r--r--   0 handerson   (501) staff       (20)       38 2023-02-09 16:37:08.879668 statease-0.2.8/setup.cfg
--rw-r--r--   0 handerson   (501) staff       (20)     1498 2023-02-09 16:36:39.000000 statease-0.2.8/setup.py
-drwxr-xr-x   0 handerson   (501) staff       (20)        0 2023-02-09 16:37:08.878837 statease-0.2.8/statease/
--rw-r--r--   0 handerson   (501) staff       (20)      348 2022-03-02 15:06:20.000000 statease-0.2.8/statease/__init__.py
--rw-r--r--   0 handerson   (501) staff       (20)    11118 2023-02-09 16:35:54.000000 statease-0.2.8/statease/analysis.py
--rw-r--r--   0 handerson   (501) staff       (20)    14902 2023-02-09 16:35:54.000000 statease-0.2.8/statease/client.py
--rw-r--r--   0 handerson   (501) staff       (20)     5391 2023-02-01 19:32:31.000000 statease-0.2.8/statease/factor.py
--rw-r--r--   0 handerson   (501) staff       (20)      468 2022-11-07 16:02:15.000000 statease-0.2.8/statease/graph.py
--rw-r--r--   0 handerson   (501) staff       (20)     2548 2023-02-01 19:32:31.000000 statease-0.2.8/statease/information.py
--rw-r--r--   0 handerson   (501) staff       (20)     1330 2022-03-02 15:06:20.000000 statease-0.2.8/statease/node.py
--rw-r--r--   0 handerson   (501) staff       (20)     5445 2022-11-08 17:26:49.000000 statease-0.2.8/statease/optimizer.py
--rw-r--r--   0 handerson   (501) staff       (20)     4721 2023-02-01 19:32:31.000000 statease-0.2.8/statease/response.py
--rw-r--r--   0 handerson   (501) staff       (20)      271 2022-03-02 15:06:20.000000 statease-0.2.8/statease/row_status.py
--rw-r--r--   0 handerson   (501) staff       (20)      482 2023-02-09 16:35:54.000000 statease-0.2.8/statease/transform.py
-drwxr-xr-x   0 handerson   (501) staff       (20)        0 2023-02-09 16:37:08.879343 statease-0.2.8/statease.egg-info/
--rw-r--r--   0 handerson   (501) staff       (20)     1376 2023-02-09 16:37:08.000000 statease-0.2.8/statease.egg-info/PKG-INFO
--rw-r--r--   0 handerson   (501) staff       (20)      412 2023-02-09 16:37:08.000000 statease-0.2.8/statease.egg-info/SOURCES.txt
--rw-r--r--   0 handerson   (501) staff       (20)        1 2023-02-09 16:37:08.000000 statease-0.2.8/statease.egg-info/dependency_links.txt
--rw-r--r--   0 handerson   (501) staff       (20)        6 2023-02-09 16:37:08.000000 statease-0.2.8/statease.egg-info/requires.txt
--rw-r--r--   0 handerson   (501) staff       (20)        9 2023-02-09 16:37:08.000000 statease-0.2.8/statease.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:52:16.060333 statease-0.2.9.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-11 15:52:16.060333 statease-0.2.9.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:52:16.060333 statease-0.2.9.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:52:16.060333 statease-0.2.9.dev2/statease/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11168 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/row_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-11 15:51:50.000000 statease-0.2.9.dev2/statease/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:52:16.060333 statease-0.2.9.dev2/statease.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-11 15:52:16.000000 statease-0.2.9.dev2/statease.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-11 15:52:16.000000 statease-0.2.9.dev2/statease.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:52:16.000000 statease-0.2.9.dev2/statease.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 15:52:16.000000 statease-0.2.9.dev2/statease.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 15:52:16.000000 statease-0.2.9.dev2/statease.egg-info/top_level.txt
```

### Comparing `statease-0.2.8/LICENSE` & `statease-0.2.9.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `statease-0.2.8/PKG-INFO` & `statease-0.2.9.dev2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: statease
-Version: 0.2.8
+Version: 0.2.9.dev2
 Summary:  Python interface to Stat-Ease 360.
 Home-page: https://statease.com/docs/se360/python-integration/
 Author: Stat-Ease, Inc.
 Author-email: support@statease.com
 License: Other/Proprietary License
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
@@ -37,9 +36,7 @@
 ## Documentation
 
 See https://statease.com/docs/se360/python-integration/.
 
 ## License
 
 **statease** is licensed under a proprietary license. Details can be found in the `LICENSE` file.
-
-
```

### Comparing `statease-0.2.8/setup.py` & `statease-0.2.9.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.2.8'
+VERSION = '0.2.9.dev2'
 DOCLINES = (__doc__ or '').split("\n")
 
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Manufacturing",
     "Intended Audience :: End Users/Desktop",
```

### Comparing `statease-0.2.8/statease/analysis.py` & `statease-0.2.9.dev2/statease/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,21 +276,23 @@
                 for term_dict in v:
                     term = namedtuple('Term', iter(term_dict.keys()))(**term_dict)
                     self.terms.append(term)
             else:
                 setattr(self, k, v)
 
     def __str__(self):
-        return """R2: {r2}
+        return """{transform}
+R2: {r2}
 Adj R2: {adjr2}
 Pred R2: {predr2}
 PRESS: {press}
 BIC: {bic}
 AICc: {aicc}
 Terms: {terms}""".format(
+            transform=self.transform,
             r2=self.r2,
             adjr2=self.adj_r2,
             predr2=self.pred_r2,
             press=self.press,
             bic=self.bic,
             aicc=self.aicc,
             terms=self.terms,
```

### Comparing `statease-0.2.8/statease/client.py` & `statease-0.2.9.dev2/statease/client.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.8/statease/factor.py` & `statease-0.2.9.dev2/statease/factor.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.8/statease/node.py` & `statease-0.2.9.dev2/statease/node.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.8/statease/optimizer.py` & `statease-0.2.9.dev2/statease/optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self._solutions = tuple(solutions)
 
 class Criteria:
     """The Criteria class is used by the optimizer to calculate a desirability score
     for a given point in the design space, which is then used to search for an optimal point.
 
     Each Analysis and Factor can have a Criteria (e.g. you might maximize the output of an Analysis,
-    and target a certian value of a Factor).
+    and target a certain value of a Factor).
     """
 
     def __init__(self, factor=None, analysis=None):
         """ Create a Criteria for a Factor or Analysis. """
 
         if (not analysis and not factor) or (analysis and factor):
             raise ValueError("You must pass in either an analysis or factor.")
@@ -90,30 +90,32 @@
         self._goal = Goal.NONE
         self._target = 0
         self._lower_limit = 0
         self._upper_limit = 0
         self._lower_weight = 1
         self._upper_weight = 1
         self._importance = 3
+        self._restrict_discrete = False
 
     def __str__(self):
         name = ''
         if self._analysis:
             name += self._analysis.name
         if self._factor:
             name += self._factor.name
-        return "Criteria for {} -> Goal: {} Target: {} Lower Limit: {} Upper Limit: {} Lower Weight: {} Upper Weight: {} Importance: {}".format(
+        return "Criteria for {} -> Goal: {} Target: {} Lower Limit: {} Upper Limit: {} Lower Weight: {} Upper Weight: {} Importance: {} Restrict discrete: {}".format(
             name,
             self._goal,
             self._target,
             self._lower_limit,
             self. _upper_limit,
             self._lower_weight,
             self._upper_weight,
             self._importance,
+            self._restrict_discrete,
         )
 
     @property
     def goal(self):
         """ The goal of this Criteria (e.g. Goal.MAXIMIZE). """
         return self._goal
 
@@ -171,14 +173,23 @@
         """ The importance of this Criteria, relative to other Criteria. """
         return self._importance
 
     @importance.setter
     def importance(self, importance):
         self._importance = importance
 
+    @property
+    def restrict_discrete(self):
+        """ The restrict discrete for this Criteria. """
+        return self._restrict_discrete
+
+    @restrict_discrete.setter
+    def restrict_discrete(self, restrict_discrete):
+        self._restrict_discrete = restrict_discrete
+
     def to_json(self):
         out_dict = {
             'analysis': self._analysis.name if self._analysis else None,
             'factor': self._factor.name if self._factor else None,
             'goal': str(self._goal),
         }
```

### Comparing `statease-0.2.8/statease/response.py` & `statease-0.2.9.dev2/statease/response.py`

 * *Files identical despite different names*

### Comparing `statease-0.2.8/statease.egg-info/PKG-INFO` & `statease-0.2.9.dev2/statease.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: statease
-Version: 0.2.8
+Version: 0.2.9.dev2
 Summary:  Python interface to Stat-Ease 360.
 Home-page: https://statease.com/docs/se360/python-integration/
 Author: Stat-Ease, Inc.
 Author-email: support@statease.com
 License: Other/Proprietary License
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
@@ -37,9 +36,7 @@
 ## Documentation
 
 See https://statease.com/docs/se360/python-integration/.
 
 ## License
 
 **statease** is licensed under a proprietary license. Details can be found in the `LICENSE` file.
-
-
```

