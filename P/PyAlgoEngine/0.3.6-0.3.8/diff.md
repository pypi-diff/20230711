# Comparing `tmp/PyAlgoEngine-0.3.6.tar.gz` & `tmp/PyAlgoEngine-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAlgoEngine-0.3.6.tar", last modified: Sun Jul  9 05:29:43 2023, max compression
+gzip compressed data, was "PyAlgoEngine-0.3.8.tar", last modified: Tue Jul 11 07:46:16 2023, max compression
```

## Comparing `PyAlgoEngine-0.3.6.tar` & `PyAlgoEngine-0.3.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2023-07-09 05:29:43.305027 PyAlgoEngine-0.3.6/
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2023-07-09 05:29:43.301026 PyAlgoEngine-0.3.6/AlgoEngine/
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2023-07-09 05:29:43.301026 PyAlgoEngine-0.3.6/AlgoEngine/Engine/
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    31104 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Engine/AlgoEngine.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     1465 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Engine/EventEngine.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    31699 2023-07-09 05:24:08.000000 PyAlgoEngine-0.3.6/AlgoEngine/Engine/MarketEngine.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    79235 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Engine/TradeEngine.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     3653 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Engine/__init__.py
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2023-07-09 05:29:43.301026 PyAlgoEngine-0.3.6/AlgoEngine/Strategies/
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     1814 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Strategies/BackTest.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    12359 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Strategies/_StrategyEngine.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     1738 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Strategies/__init__.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)      426 2023-07-09 05:27:54.000000 PyAlgoEngine-0.3.6/AlgoEngine/__init__.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     1066 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/LICENSE
--rw-rw-r--   0 bolun     (1000) bolun     (1000)      515 2023-07-09 05:29:43.305027 PyAlgoEngine-0.3.6/PKG-INFO
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2023-07-09 05:29:43.305027 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/
--rw-rw-r--   0 bolun     (1000) bolun     (1000)      515 2023-07-09 05:29:43.000000 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/PKG-INFO
--rw-rw-r--   0 bolun     (1000) bolun     (1000)      499 2023-07-09 05:29:43.000000 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/SOURCES.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)        1 2023-07-09 05:29:43.000000 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/dependency_links.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       57 2023-07-09 05:29:43.000000 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/requires.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       11 2023-07-09 05:29:43.000000 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/top_level.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       42 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/README.md
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       38 2023-07-09 05:29:43.305027 PyAlgoEngine-0.3.6/setup.cfg
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     1528 2023-07-09 05:26:34.000000 PyAlgoEngine-0.3.6/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-11 07:46:16.644967 PyAlgoEngine-0.3.8/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-11 07:46:11.814647 PyAlgoEngine-0.3.8/AlgoEngine/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-11 07:46:13.912082 PyAlgoEngine-0.3.8/AlgoEngine/Engine/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31104 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8/AlgoEngine/Engine/AlgoEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1465 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8/AlgoEngine/Engine/EventEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    32307 2023-07-11 05:55:16.000000 PyAlgoEngine-0.3.8/AlgoEngine/Engine/MarketEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    79235 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8/AlgoEngine/Engine/TradeEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3653 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8/AlgoEngine/Engine/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-11 07:46:15.045077 PyAlgoEngine-0.3.8/AlgoEngine/Strategies/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1814 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8/AlgoEngine/Strategies/BackTest.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    15559 2023-07-11 06:11:38.000000 PyAlgoEngine-0.3.8/AlgoEngine/Strategies/_StrategyEngine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1738 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8/AlgoEngine/Strategies/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      426 2023-07-11 06:11:38.000000 PyAlgoEngine-0.3.8/AlgoEngine/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      515 2023-07-11 07:46:16.616318 PyAlgoEngine-0.3.8/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-07-11 07:46:16.361557 PyAlgoEngine-0.3.8/PyAlgoEngine.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      515 2023-07-11 07:45:36.000000 PyAlgoEngine-0.3.8/PyAlgoEngine.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      499 2023-07-11 07:45:51.000000 PyAlgoEngine-0.3.8/PyAlgoEngine.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-07-11 07:45:36.000000 PyAlgoEngine-0.3.8/PyAlgoEngine.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       57 2023-07-11 07:45:36.000000 PyAlgoEngine-0.3.8/PyAlgoEngine.egg-info/requires.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2023-07-11 07:45:36.000000 PyAlgoEngine-0.3.8/PyAlgoEngine.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       42 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8/README.md
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2023-07-11 07:46:16.670220 PyAlgoEngine-0.3.8/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1528 2023-07-11 05:27:47.000000 PyAlgoEngine-0.3.8/setup.py
```

### Comparing `PyAlgoEngine-0.3.6/AlgoEngine/Engine/AlgoEngine.py` & `PyAlgoEngine-0.3.8/AlgoEngine/Engine/AlgoEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.6/AlgoEngine/Engine/EventEngine.py` & `PyAlgoEngine-0.3.8/AlgoEngine/Engine/EventEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.6/AlgoEngine/Engine/MarketEngine.py` & `PyAlgoEngine-0.3.8/AlgoEngine/Engine/MarketEngine.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,14 +482,27 @@
 
     def __getitem__(self, monitor_id: str) -> MarketDataMonitor:
         return self._monitor[monitor_id]
 
     def add_monitor(self, monitor: MarketDataMonitor):
         self._monitor[monitor.monitor_id] = monitor
 
+    def pop_monitor(self, monitor: MarketDataMonitor = None, monitor_id: str = None, monitor_name: str = None):
+        if monitor_id is not None:
+            return self._monitor.pop(monitor_id)
+        elif monitor_name is not None:
+            for _ in list(self._monitor.values()):
+                if _.name == monitor_name:
+                    return self._monitor.pop(_.monitor_id)
+        elif monitor is not None:
+            return self._monitor.pop(monitor.monitor_id)
+        else:
+            LOGGER.error('must assign a monitor, or monitor_id, or monitor_name to pop.')
+            return None
+
     def init_cn_override(self):
         self.profile = CN_Profile()
 
     def _on_trade_data(self, trade_data: TradeData):
         ticker = trade_data.ticker
 
         if ticker not in self._trade_data:
```

### Comparing `PyAlgoEngine-0.3.6/AlgoEngine/Engine/TradeEngine.py` & `PyAlgoEngine-0.3.8/AlgoEngine/Engine/TradeEngine.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.6/AlgoEngine/Engine/__init__.py` & `PyAlgoEngine-0.3.8/AlgoEngine/Engine/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.6/AlgoEngine/Strategies/BackTest.py` & `PyAlgoEngine-0.3.8/AlgoEngine/Strategies/BackTest.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.6/AlgoEngine/Strategies/__init__.py` & `PyAlgoEngine-0.3.8/AlgoEngine/Strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.6/LICENSE` & `PyAlgoEngine-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.6/PKG-INFO` & `PyAlgoEngine-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.6
+Version: 0.3.8
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/PKG-INFO` & `PyAlgoEngine-0.3.8/PyAlgoEngine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.6
+Version: 0.3.8
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `PyAlgoEngine-0.3.6/setup.py` & `PyAlgoEngine-0.3.8/setup.py`

 * *Files identical despite different names*

