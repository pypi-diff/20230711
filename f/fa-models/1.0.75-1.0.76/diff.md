# Comparing `tmp/fa-models-1.0.75.tar.gz` & `tmp/fa-models-1.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.75.tar", last modified: Mon Jul 10 06:14:47 2023, max compression
+gzip compressed data, was "fa-models-1.0.76.tar", last modified: Tue Jul 11 09:56:36 2023, max compression
```

## Comparing `fa-models-1.0.75.tar` & `fa-models-1.0.76.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.211431 fa-models-1.0.75/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-10 06:14:47.211431 fa-models-1.0.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-10 06:14:11.000000 fa-models-1.0.75/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.207431 fa-models-1.0.75/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-10 06:14:47.000000 fa-models-1.0.75/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-10 06:14:47.000000 fa-models-1.0.75/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:14:47.000000 fa-models-1.0.75/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 06:14:47.000000 fa-models-1.0.75/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 06:14:47.000000 fa-models-1.0.75/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.207431 fa-models-1.0.75/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.211431 fa-models-1.0.75/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/investor_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.211431 fa-models-1.0.75/famodels/models/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/market/public_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/signal_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-10 06:14:11.000000 fa-models-1.0.75/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-10 06:14:37.000000 fa-models-1.0.75/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 06:14:47.211431 fa-models-1.0.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-10 06:14:11.000000 fa-models-1.0.75/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:14:47.211431 fa-models-1.0.75/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-10 06:14:11.000000 fa-models-1.0.75/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-10 06:14:11.000000 fa-models-1.0.75/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.237990 fa-models-1.0.76/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-11 09:56:36.237990 fa-models-1.0.76/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-11 09:56:06.000000 fa-models-1.0.76/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.233989 fa-models-1.0.76/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-11 09:56:36.000000 fa-models-1.0.76/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-11 09:56:36.000000 fa-models-1.0.76/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:56:36.000000 fa-models-1.0.76/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 09:56:36.000000 fa-models-1.0.76/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 09:56:36.000000 fa-models-1.0.76/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.233989 fa-models-1.0.76/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.233989 fa-models-1.0.76/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/investor_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.233989 fa-models-1.0.76/famodels/models/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/market/public_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/signal_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-11 09:56:27.000000 fa-models-1.0.76/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:56:36.237990 fa-models-1.0.76/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-11 09:56:06.000000 fa-models-1.0.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.233989 fa-models-1.0.76/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-11 09:56:06.000000 fa-models-1.0.76/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-11 09:56:06.000000 fa-models-1.0.76/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.75/PKG-INFO` & `fa-models-1.0.76/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.75
+Version: 1.0.76
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.75/README.md` & `fa-models-1.0.76/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.76/fa_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.75
+Version: 1.0.76
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.75/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.76/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/famodels/models/algorithm.py` & `fa-models-1.0.76/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/famodels/models/investor.py` & `fa-models-1.0.76/famodels/models/investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/famodels/models/investor_statement.py` & `fa-models-1.0.76/famodels/models/investor_statement.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/famodels/models/market/public_trade.py` & `fa-models-1.0.76/famodels/models/market/public_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/famodels/models/order.py` & `fa-models-1.0.76/famodels/models/order.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,41 @@
+from enum import Enum
 from typing import List, Set, Optional
 from famodels.models.direction import Direction
 from famodels.models.order_type import OrderType
 from famodels.models.side import Side
 from redis_om import (Field, JsonModel)
 from redis_om.connections import get_redis_connection
 import os
 
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
 print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
 
+class StateOfOrder(str, Enum):    
+    """Describing the possible states of an Order. Keep it simple. Also, we added the str to inherit from, so that the ENUM is serializable.         """
+    NEW = "new"
+    """It's new order, when the order is to be picked up by a fa-dex/cex-exchange-adapter. """
+    SUBMITTED = "submitted"
+    """The order is submitted and accepted but nothing was filled so far."""
+    FILLING = "filling"
+    """The order is about to be filled."""
+    CANCELED = "canceled"
+    """The order was canceled e.g. due to 'too long alive and not filled'."""
+    FILLED = "filled"
+    """Filled means the order filled completely and is thus closed."""
+
 class Order(JsonModel):
     """This model is for hot orders ONLY! Use ColdOrder for paper trading.
     """
     id: str = Field(index=True)
     signal_id: str = Field(index=True)
     algo_id: str = Field(index=True)
+    trade_id: str = Field(index=True)
+    state: StateOfOrder = Field(index=True, default=StateOfOrder.NEW)
     order_type: OrderType = Field(index=True, default=OrderType.LIMIT)        
     market: str = Field(index=True)
     exchange: str = Field(index=True)
     direction: Direction = Field(index=True)
     side: Side = Field(index=True)
     price: float
     amount: float
```

### Comparing `fa-models-1.0.75/famodels/models/person.py` & `fa-models-1.0.76/famodels/models/person.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/famodels/models/processed_signal.py` & `fa-models-1.0.76/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/famodels/models/signal_provider.py` & `fa-models-1.0.76/famodels/models/signal_provider.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/famodels/models/trade.py` & `fa-models-1.0.76/famodels/models/trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # sort_index:int = field(init=False, repr=False)
     #trade_id: Optional[str] = Field(default=uuid.uuid4(), primary_key=True)
     """The trade id is the reference that keeps the state updates correlated. It will generate a UUID by default.
         Use this for the first record you insert. Inserting updated records (new records should then have the trade_id
         provided to create the correlation.)"""
     investor_id: str = Field(index=True)
     fund_id: str = Field(index=True)
-    pos_idx:int
+    fund_pos_idx:int
     market:str = Field(index=True)    
     state:StateOfTrade = Field(index=True, default=StateOfTrade.NEW)
     direction:Direction
     amount: float
     time_of_initiation:datetime = Field(index=True, default=int(time.time() * 1000))
     """When we decided to start this trade."""
     buy_order_id: Optional[str] = None
```

### Comparing `fa-models-1.0.75/famodels/models/trading_signal.py` & `fa-models-1.0.76/famodels/models/trading_signal.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,16 +47,19 @@
     """Simply BUY (open trade) or SELL (close trade)."""
     price: float
     """The price to buy use for the limit-order or limit-stop-order"""
     tp: float
     """Take-profit in absolute price."""
     sl: float
     """Stop-loss in absolute price."""
-    position_size_of_investment: float = 100
-    """Percentage of the investment position this algortihm is allowed to trade. Default is 100%, which is 1 position."""  
+    position_size_in_percentage: float = 100
+    """Percentage of the trade position this algortihm is allowed to trade. 
+    Default is 100%, which is 1 position of your fund's positions.
+    Another number than 100, will assume this provider-trade has multiple positions. 
+    If a signal provider has one partial position open and then closes it, it will also regard the trade as fully closed."""  
     # datatime.datetime would be fully serializable in REDIS. 
     # https://www.youtube.com/watch?v=ZP2j7bmWfmU
     timestamp_of_creation: int = Field(index=True)
     """The timestamp in milliseconds when the signal was created by the signal supplier."""
     timestamp_of_registration: Optional[int]
     """The timestamp in milliseconds when the signal was entering our interface. This will be overridden."""
```

### Comparing `fa-models-1.0.75/famodels/models/virtual_order.py` & `fa-models-1.0.76/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/pyproject.toml` & `fa-models-1.0.76/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.75"
+version = "1.0.76"
 description = "A simple library of trading models."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.75"
+current_version = "1.0.76"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.75/setup.py` & `fa-models-1.0.76/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/tests/test_investor.py` & `fa-models-1.0.76/tests/test_investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.75/tests/test_processed_trading_signal.py` & `fa-models-1.0.76/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

