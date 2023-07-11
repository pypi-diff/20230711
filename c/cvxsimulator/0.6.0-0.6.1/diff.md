# Comparing `tmp/cvxsimulator-0.6.0.tar.gz` & `tmp/cvxsimulator-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.6.0.tar", max compression
+gzip compressed data, was "cvxsimulator-0.6.1.tar", max compression
```

## Comparing `cvxsimulator-0.6.0.tar` & `cvxsimulator-0.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11375 2023-07-11 01:01:47.570381 cvxsimulator-0.6.0/LICENSE
--rw-r--r--   0        0        0     5166 2023-07-11 01:01:47.570381 cvxsimulator-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    16257 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1613 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1457 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/month.py
--rw-r--r--   0        0        0    20589 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      795 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      726 2023-07-11 01:02:17.119008 cvxsimulator-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5784 1970-01-01 00:00:00.000000 cvxsimulator-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-07-11 06:54:48.576622 cvxsimulator-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5166 2023-07-11 06:54:48.576622 cvxsimulator-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    16756 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1613 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1457 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/month.py
+-rw-r--r--   0        0        0    20589 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      795 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      726 2023-07-11 06:55:14.244555 cvxsimulator-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5784 1970-01-01 00:00:00.000000 cvxsimulator-0.6.1/PKG-INFO
```

### Comparing `cvxsimulator-0.6.0/LICENSE` & `cvxsimulator-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.0/README.md` & `cvxsimulator-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.0/cvx/simulator/builder.py` & `cvxsimulator-0.6.1/cvx/simulator/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -263,14 +263,27 @@
 
         Notes: The function extracts the column names of the prices dataframe,
         which correspond to the assets held by the portfolio.
         The resulting list will contain the names of all assets
         held by the portfolio, without any duplicates."""
         return self.prices.columns
 
+    @property
+    def returns(self):
+        return self.prices.pct_change().dropna(axis=0, how="all")
+
+    def cov(self, **kwargs):
+        # You can do much better using volatility adjusted returns rather than returns
+        cov = self.returns.ewm(**kwargs).cov()
+        cov = cov.dropna(how="all", axis=0)
+        for t in cov.index.get_level_values(level=0).unique():
+            yield t, cov.loc[t, :, :]
+
+        # {t: cov.loc[t, :, :] for t in cov.index.get_level_values('date').unique()}
+
     def set_weights(self, time, weights):
         """
         Set the position via weights (e.g. fractions of the nav)
 
         :param time: time
         :param weights: series of weights
         """
```

### Comparing `cvxsimulator-0.6.0/cvx/simulator/grid.py` & `cvxsimulator-0.6.1/cvx/simulator/grid.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.0/cvx/simulator/month.py` & `cvxsimulator-0.6.1/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.0/cvx/simulator/portfolio.py` & `cvxsimulator-0.6.1/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.0/cvx/simulator/trading_costs.py` & `cvxsimulator-0.6.1/cvx/simulator/trading_costs.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.0/pyproject.toml` & `cvxsimulator-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.6.0"
+version = "v0.6.1"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.6.0/PKG-INFO` & `cvxsimulator-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.6.0
+Version: 0.6.1
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

