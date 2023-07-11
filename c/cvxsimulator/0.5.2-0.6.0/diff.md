# Comparing `tmp/cvxsimulator-0.5.2.tar.gz` & `tmp/cvxsimulator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.5.2.tar", max compression
+gzip compressed data, was "cvxsimulator-0.6.0.tar", max compression
```

## Comparing `cvxsimulator-0.5.2.tar` & `cvxsimulator-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11375 2023-07-10 14:46:35.394627 cvxsimulator-0.5.2/LICENSE
--rw-r--r--   0        0        0     5166 2023-07-10 14:46:35.394627 cvxsimulator-0.5.2/README.md
--rw-r--r--   0        0        0        0 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    16257 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1613 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1209 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1457 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/month.py
--rw-r--r--   0        0        0    19303 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      795 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      726 2023-07-10 14:47:10.598803 cvxsimulator-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     5784 1970-01-01 00:00:00.000000 cvxsimulator-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-07-11 01:01:47.570381 cvxsimulator-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5166 2023-07-11 01:01:47.570381 cvxsimulator-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    16257 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1613 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1457 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/month.py
+-rw-r--r--   0        0        0    20589 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      795 2023-07-11 01:01:47.650382 cvxsimulator-0.6.0/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      726 2023-07-11 01:02:17.119008 cvxsimulator-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5784 1970-01-01 00:00:00.000000 cvxsimulator-0.6.0/PKG-INFO
```

### Comparing `cvxsimulator-0.5.2/LICENSE` & `cvxsimulator-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.2/README.md` & `cvxsimulator-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.2/cvx/simulator/builder.py` & `cvxsimulator-0.6.0/cvx/simulator/builder.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.2/cvx/simulator/grid.py` & `cvxsimulator-0.6.0/cvx/simulator/grid.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.2/cvx/simulator/month.py` & `cvxsimulator-0.6.0/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.2/cvx/simulator/portfolio.py` & `cvxsimulator-0.6.0/cvx/simulator/portfolio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,50 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from dataclasses import dataclass
+from enum import Enum
 
 import pandas as pd
+import quantstats as qs
 
 from cvx.simulator.grid import iron_frame
 from cvx.simulator.trading_costs import TradingCostModel
 
+qs.extend_pandas()
+
+
+class Plot(Enum):
+    DAILY_RETURNS = 1
+    DISTRIBUTION = 2
+    DRAWDOWN = 3
+    DRAWDOWNS_PERIODS = 4
+    EARNINGS = 5
+    HISTOGRAM = 6
+    LOG_RETURNS = 7
+    MONTHLY_HEATMAP = 8
+    # see issue: https://github.com/ranaroussi/quantstats/issues/276
+    MONTHLY_RETURNS = 9
+    RETURNS = 10
+    ROLLING_BETA = 11
+    ROLLING_SHARPE = 12
+    ROLLING_SORTINO = 13
+    ROLLING_VOLATILITY = 14
+    YEARLY_RETURNS = 15
+
+    # def __call__(self, *args, **kwargs):
+    #    return self.func(*args, **kwargs)
+
+    @property
+    def func(self):
+        return getattr(qs.plots, self.name.lower())
+
+    def plot(self, *args, **kwargs):
+        return self.func(*args, **kwargs)
+
 
 def diff(portfolio1, portfolio2, initial_cash=1e6, trading_cost_model=None):
     # check both portfolios are on the same price grid
     pd.testing.assert_frame_equal(portfolio1.prices, portfolio2.prices)
 
     stocks = portfolio1.stocks - portfolio2.stocks
 
@@ -432,7 +465,22 @@
 
         return EquityPortfolio(
             prices=self.prices,
             stocks=stocks,
             trading_cost_model=self.trading_cost_model,
             initial_cash=self.initial_cash,
         )
+
+    def metrics(self, **kwargs):
+        return qs.reports.metrics(self.nav.pct_change().dropna(), **kwargs)
+
+    def plots(self, **kwargs):
+        return qs.reports.plots(self.nav.pct_change().dropna(), **kwargs)
+
+    def plot(self, kind: Plot, **kwargs):
+        return kind.plot(returns=self.nav.pct_change().dropna(), **kwargs)
+
+    def html(self, **kwargs):
+        return qs.reports.html(self.nav.pct_change().dropna(), **kwargs)
+
+    def snapshot(self, **kwargs):
+        return qs.plots.snapshot(self.nav.pct_change().dropna(), **kwargs)
```

### Comparing `cvxsimulator-0.5.2/cvx/simulator/trading_costs.py` & `cvxsimulator-0.6.0/cvx/simulator/trading_costs.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.2/pyproject.toml` & `cvxsimulator-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.5.2"
+version = "v0.6.0"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.5.2/PKG-INFO` & `cvxsimulator-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.5.2
+Version: 0.6.0
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

