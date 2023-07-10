# Comparing `tmp/easyfrenchtax-0.0.6.tar.gz` & `tmp/easyfrenchtax-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfrenchtax-0.0.6.tar", last modified: Tue Jul  4 20:10:10 2023, max compression
+gzip compressed data, was "easyfrenchtax-0.0.7.tar", last modified: Mon Jul 10 22:03:01 2023, max compression
```

## Comparing `easyfrenchtax-0.0.6.tar` & `easyfrenchtax-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-04 20:10:10.513974 easyfrenchtax-0.0.6/
--rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.6/LICENSE
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-04 20:10:10.514038 easyfrenchtax-0.0.6/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.6/README.md
--rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.6/pyproject.toml
--rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-07-04 20:10:10.514293 easyfrenchtax-0.0.6/setup.cfg
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-04 20:10:10.510055 easyfrenchtax-0.0.6/src/
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-04 20:10:10.511287 easyfrenchtax-0.0.6/src/easyfrenchtax/
--rw-r--r--   0 hadrien    (501) staff       (20)      100 2022-06-09 10:23:03.000000 easyfrenchtax-0.0.6/src/easyfrenchtax/__init__.py
--rw-r--r--   0 hadrien    (501) staff       (20)    19593 2023-07-04 20:10:04.000000 easyfrenchtax-0.0.6/src/easyfrenchtax/stock_helper.py
--rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-06-02 20:57:34.000000 easyfrenchtax-0.0.6/src/easyfrenchtax/tax_simulator.py
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-04 20:10:10.512241 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/
--rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-04 20:10:10.000000 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-07-04 20:10:10.000000 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/SOURCES.txt
--rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-07-04 20:10:10.000000 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/dependency_links.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-07-04 20:10:10.000000 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/requires.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-07-04 20:10:10.000000 easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/top_level.txt
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-04 20:10:10.513731 easyfrenchtax-0.0.6/tests/
--rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.6/tests/test_capital_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.6/tests/test_fiscal_advantages.py
--rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.6/tests/test_income_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.6/tests/test_rental_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    12885 2023-07-04 20:09:13.000000 easyfrenchtax-0.0.6/tests/test_stock_helper.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-10 22:03:01.370544 easyfrenchtax-0.0.7/
+-rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.7/LICENSE
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-10 22:03:01.370637 easyfrenchtax-0.0.7/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)     1824 2022-06-07 08:55:19.000000 easyfrenchtax-0.0.7/README.md
+-rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.7/pyproject.toml
+-rw-r--r--   0 hadrien    (501) staff       (20)      853 2023-07-10 22:03:01.370939 easyfrenchtax-0.0.7/setup.cfg
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-10 22:03:01.365499 easyfrenchtax-0.0.7/src/
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-10 22:03:01.367038 easyfrenchtax-0.0.7/src/easyfrenchtax/
+-rw-r--r--   0 hadrien    (501) staff       (20)      100 2022-06-09 10:23:03.000000 easyfrenchtax-0.0.7/src/easyfrenchtax/__init__.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    21251 2023-07-10 22:00:39.000000 easyfrenchtax-0.0.7/src/easyfrenchtax/stock_helper.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    27735 2023-06-02 20:57:34.000000 easyfrenchtax-0.0.7/src/easyfrenchtax/tax_simulator.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-10 22:03:01.368043 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/
+-rw-r--r--   0 hadrien    (501) staff       (20)     2557 2023-07-10 22:03:01.000000 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)      480 2023-07-10 22:03:01.000000 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/SOURCES.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)        1 2023-07-10 22:03:01.000000 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/dependency_links.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       18 2023-07-10 22:03:01.000000 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/requires.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       14 2023-07-10 22:03:01.000000 easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/top_level.txt
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2023-07-10 22:03:01.370280 easyfrenchtax-0.0.7/tests/
+-rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.7/tests/test_capital_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.7/tests/test_fiscal_advantages.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.7/tests/test_income_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.7/tests/test_rental_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    12964 2023-07-10 21:59:44.000000 easyfrenchtax-0.0.7/tests/test_stock_helper.py
```

### Comparing `easyfrenchtax-0.0.6/LICENSE` & `easyfrenchtax-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.6/PKG-INFO` & `easyfrenchtax-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfrenchtax-0.0.6/README.md` & `easyfrenchtax-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.6/setup.cfg` & `easyfrenchtax-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easyfrenchtax
-version = 0.0.6
+version = 0.0.7
 author = Hadrien Hamel
 author_email = hadrien.hamel@gmail.com
 license = MIT
 description = A simulator of French taxes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/had/easyfrenchtax
```

### Comparing `easyfrenchtax-0.0.6/src/easyfrenchtax/stock_helper.py` & `easyfrenchtax-0.0.7/src/easyfrenchtax/stock_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 from dataclasses import dataclass
 from datetime import date, datetime
+from enum import Enum
 from typing import Optional
 
 from dateutil.relativedelta import relativedelta
 from currency_converter import CurrencyConverter
 from collections import defaultdict
 import csv
 import glob
 
+class RsuTaxScheme(Enum):
+    NONQUALIFIED_RSU = 1
+    QUALIFIED_RSU = 2
+    MACRON_1_RSU = 3
+    MACRON_2_RSU = 4
+    MACRON_3_RSU = 5
+
+class StockType(Enum):
+    RSU = 1
+    ESPP = 2
+    STOCKOPTIONS = 3
 
 @dataclass
 class StockGroup:
     count: int
     available: int
     acq_price: float
     acq_price_eur: float
@@ -19,34 +31,32 @@
     plan_name: str
 
 
 @dataclass
 class RsuPlan:
     name: str
     approval_date: date
-    taxation_scheme: str
+    taxation_scheme: RsuTaxScheme
     stock_symbol: str
     currency: str
 
 
 @dataclass
 class SaleEvent:
     symbol: str
-    stock_type: str  # TODO change to enum
+    stock_type: StockType
     nb_stocks_sold: int
     unit_acquisition_price: float # in Euros
     sell_date: date
     sell_price_eur: float
     selling_fees: float
     owner: Optional[int] = None
-    plan_name: Optional[str] = None
+    rsu_tax_scheme: Optional[RsuTaxScheme] = None
     acq_date: Optional[date] = None
 
-
-
 # currency converter (USD/EUR in particular)
 cc = CurrencyConverter(fallback_on_wrong_date=True, fallback_on_missing_rate=True)
 
 
 class StockHelper:
     rsu_plans: dict[str, RsuPlan]
     rsus: dict[str, list[StockGroup]]  # TODO integrate list of RSUs to RsuPlan
@@ -57,22 +67,23 @@
         self.rsu_plans = {}
         self.rsus = defaultdict(list)
         self.espp_stocks = defaultdict(list)
         self.stock_options = defaultdict(list)
         self.stock_sales = defaultdict(list)
 
     # TODO: this seems unused, consider removing
-    def reset(self, stock_types: list[str] = ("espp", "stockoption", "rsu"), symbols: list[str] = None) -> None:
+    def reset(self, stock_types: list[StockType] = (StockType.RSU, StockType.ESPP, StockType.STOCKOPTIONS),
+              symbols: list[str] = None) -> None:
         for sales in self.stock_sales.values():
             sales[:] = [s for s in sales if
                         (symbols and s.symbol not in symbols) or (s.stock_type not in stock_types)]
         stock_types_mapping = {
-            "espp": self.espp_stocks,
-            "stockoption": self.stock_options,
-            "rsu": self.rsus
+            StockType.ESPP: self.espp_stocks,
+            StockType.STOCKOPTIONS: self.stock_options,
+            StockType.RSU: self.rsus
         }
         for stock_type in [stock_types_mapping[st] for st in stock_types]:
             if not symbols:
                 stocks_subset = stock_type.values()
             else:
                 stocks_subset = [stock_type[symbol] for symbol in symbols]
             for stocks in stocks_subset:
@@ -91,25 +102,25 @@
         for symbol, stockoptions in self.stock_options.items():
             for stockoption in stockoptions:
                 summary[symbol]["StockOption"] += stockoption.count
         return summary
 
     # ----- RSU related load functions ------
     @staticmethod
-    def _determine_rsu_plans_type(approval_date: date) -> str:
+    def _determine_rsu_plans_type(approval_date: date) -> RsuTaxScheme:
         if approval_date <= date(2012, 9, 27):
-            return "2007"  # TODO replace with an enum
+            return RsuTaxScheme.NONQUALIFIED_RSU
         elif approval_date <= date(2015, 8, 8):
-            return "2012"
-        elif approval_date <= date(2016, 12, 30):
-            return "2015"
-        elif approval_date <= date(2017, 12, 31):
-            return "2017"
+            return RsuTaxScheme.QUALIFIED_RSU
+        elif approval_date <= date(2017, 1, 1):
+            return RsuTaxScheme.MACRON_1_RSU
+        elif approval_date <= date(2018, 1, 1):
+            return RsuTaxScheme.MACRON_2_RSU
         else:
-            return "2018"
+            return RsuTaxScheme.MACRON_3_RSU
 
     ## IMPORTANT! approval_date here is used to determine the taxation scheme
     # (Macron I, Macron II, etc.) so it needs to be the date where the plan was
     # approved by the shareholders, NOT the grant date.
     def rsu_plan(self, name: str, approval_date: date, symbol: str, currency: str) -> None:
         if name not in self.rsu_plans:
             self.rsu_plans[name] = RsuPlan(
@@ -189,73 +200,93 @@
                         self.add_espp(symbol, acq_count, acq_date, acq_price, currency)
                     elif stock_type == "StockOption":
                         self.add_stockoptions(symbol, plan_name, acq_count, acq_date, acq_price, currency)
 
     ####### stock selling related load functions #######
 
     def sell_stockoptions(self, owner: int, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
-                          currency: str = "EUR"):
+                          currency: str = "EUR") -> int:
         if nb_stocks == 0:
-            return
+            return 0
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
         stocks_before_sell_date = [r for r in self.stock_options[symbol] if r.acq_date < sell_date]
         for i, acq in enumerate(stocks_before_sell_date):
             if acq.available == 0:
                 continue
             sell_from_acq = min(to_sell, acq.available)
             strike_price_eur = acq.acq_price_eur if acq.acq_price_eur else cc.convert(acq.acq_price, currency, "EUR",
                                                                                       date=sell_date)
-            self.stock_sales[sell_date.year].append(SaleEvent(
+            self.sell_stockoptions_2(
                 symbol=symbol,
-                stock_type="stockoption",
                 nb_stocks_sold=sell_from_acq,
                 unit_acquisition_price=strike_price_eur,  # re-using this field to store the strike price
                 sell_date=sell_date,
                 sell_price_eur=sell_price_eur,
-                selling_fees=round(cc.convert(fees, currency, "EUR", date=sell_date), 2),
                 owner=owner
-            ))
+            )
             # update the stock options data with new availability
             self.stock_options[symbol][i].available = acq.available - sell_from_acq
             to_sell -= sell_from_acq
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have ({to_sell})")
         return nb_stocks - to_sell
 
+    def sell_stockoptions_2(self, symbol: str, nb_stocks_sold: int, unit_acquisition_price: float,
+                sell_date: date, sell_price_eur: float, owner: int):
+        self.stock_sales[sell_date.year].append(SaleEvent(
+            symbol=symbol,
+            stock_type=StockType.STOCKOPTIONS,
+            nb_stocks_sold=nb_stocks_sold,
+            unit_acquisition_price=round(unit_acquisition_price, 2),
+            sell_date=sell_date,
+            sell_price_eur=sell_price_eur,
+            selling_fees=0,
+            owner=owner,
+        ))
     def sell_espp(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
-                  currency: str = "EUR"):
+                  currency: str = "EUR") -> int:
         if nb_stocks == 0:
-            return
+            return 0
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
         stocks_before_sell_date = [r for r in self.espp_stocks[symbol] if r.acq_date < sell_date]
         for i, acq in enumerate(stocks_before_sell_date):
             if acq.available == 0:
                 continue
             sell_from_acq = min(to_sell, acq.available)
             self.espp_stocks[symbol][i].available = acq.available - sell_from_acq
             to_sell -= sell_from_acq
-            self.stock_sales[sell_date.year].append(SaleEvent(
+            self.sell_espp_2(
                 symbol=symbol,
-                stock_type="espp",
                 nb_stocks_sold=sell_from_acq,
-                unit_acquisition_price=round(acq.acq_price_eur, 2),
+                unit_acquisition_price=acq.acq_price_eur,
                 sell_date=sell_date,
-                sell_price_eur=sell_price_eur,
-                selling_fees=0  # not sure how to handle this
-            ))
+                sell_price_eur=sell_price_eur
+            )
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have")
-            return (0, 0, [])
-        return (nb_stocks - to_sell)
+        return nb_stocks - to_sell
+
+    def sell_espp_2(self, symbol: str, nb_stocks_sold: int, unit_acquisition_price: float,
+                sell_date: date, sell_price_eur: float):
+        self.stock_sales[sell_date.year].append(SaleEvent(
+            symbol=symbol,
+            stock_type=StockType.ESPP,
+            nb_stocks_sold=nb_stocks_sold,
+            unit_acquisition_price=round(unit_acquisition_price, 2),
+            sell_date=sell_date,
+            sell_price_eur=sell_price_eur,
+            selling_fees=0,
+        ))
+
 
     def sell_rsus(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
                   currency: str = "EUR") -> int:
         if nb_stocks == 0:
             return 0
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
@@ -267,82 +298,95 @@
         if not rsu_before_sell_date:
             # no rsu for that date
             return 0
         for i, acq in enumerate(rsu_before_sell_date):
             if acq.available == 0:
                 continue
             sell_from_acq = min(to_sell, acq.available)
-            self.stock_sales[sell_date.year].append(SaleEvent(
+            tax_scheme = self.rsu_plans[acq.plan_name].taxation_scheme
+            self.sell_rsus_2(
                 symbol=symbol,
-                stock_type="rsu",
                 nb_stocks_sold=sell_from_acq,
-                unit_acquisition_price=round(acq.acq_price_eur, 2),
-                sell_date=sell_date,
+                acq_date=acq.acq_date,
+                unit_acquisition_price=acq.acq_price_eur,
+                sell_date = sell_date,
                 sell_price_eur=sell_price_eur,
-                selling_fees=0,  # not sure how to handle this
-                owner=None,
-                plan_name=acq.plan_name,
-                acq_date=acq.acq_date
-            ))
+                tax_scheme=tax_scheme
+            )
             # update the rsu data with new availability (tuples are immutable, so replace with new one)
             self.rsus[symbol][i].available = acq.available - sell_from_acq
             to_sell -= sell_from_acq
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have ({to_sell})")
         return (nb_stocks - to_sell)
 
+    def sell_rsus_2(self, symbol: str, nb_stocks_sold: int, acq_date: date, unit_acquisition_price: float,
+                sell_date: date, sell_price_eur: float, tax_scheme: RsuTaxScheme):
+        self.stock_sales[sell_date.year].append(SaleEvent(
+            symbol=symbol,
+            stock_type=StockType.RSU,
+            nb_stocks_sold=nb_stocks_sold,
+            unit_acquisition_price=round(unit_acquisition_price, 2),
+            sell_date=sell_date,
+            sell_price_eur=sell_price_eur,
+            selling_fees=0,
+            owner=None,
+            rsu_tax_scheme=tax_scheme,
+            acq_date=acq_date
+        ))
+
+
     ####### tax computation functions #######
 
     # the bible of acquisition and capital gain tax (version 2021):
     # https://www.impots.gouv.fr/portail/www2/fichiers/documentation/brochure/ir_2021/pdf_som/09-plus_values_141a158.pdf
     def compute_acquisition_gain_tax(self, year: int):
         sell_events = self.stock_sales[year]
         taxable_gain = 0  # this would contribute to box 1TZ
         rebates = 0  # this would contribute to box 1UZ
         rebates_50p = 0  # this would contribute to box 1WZ
         other_taxable_gain_1 = 0  # this would contribute to box 1TT
         other_taxable_gain_2 = 0  # this would contribute to box 1UT
 
         for sale in sell_events:
-            if sale.stock_type == "stockoption":
+            if sale.stock_type == StockType.STOCKOPTIONS:
                 # exercise gain only applies to Stock Options
                 # /!\ only stock options attributed after 28/09/2012 are supported
 
                 # Note: strike price is stored in unit_acquisition_price
                 exercise_gain_eur = sale.nb_stocks_sold * (sale.sell_price_eur - sale.unit_acquisition_price)
                 if sale.owner == 1:
                     other_taxable_gain_1 += exercise_gain_eur
                 elif sale.owner == 2:
                     other_taxable_gain_2 += exercise_gain_eur
                 else:
                     raise Exception(
                         f"Owner must be 1 or 2, not {sale.owner} (type={type(sale.owner)}")
-            elif sale.stock_type == "rsu":
+            elif sale.stock_type == StockType.RSU:
                 # acquisition gain only applies to RSU
                 sell_date = sale.sell_date
                 sell_date_minus_2y = sell_date + relativedelta(years=-2)
                 sell_date_minus_8y = sell_date + relativedelta(years=-8)
-                rsu_plan = self.rsu_plans[sale.plan_name]
-                taxation_scheme = rsu_plan.taxation_scheme
+                taxation_scheme = sale.rsu_tax_scheme
                 acq_date = sale.acq_date
                 gain_eur = sale.nb_stocks_sold * sale.unit_acquisition_price
                 # gain tax
-                if taxation_scheme == "2015" or taxation_scheme == "2017":
+                if taxation_scheme in (RsuTaxScheme.MACRON_1_RSU, RsuTaxScheme.MACRON_2_RSU):
                     # 50% rebates btw 2 and 8y retention, 65% above 8y
                     if acq_date <= sell_date_minus_8y:
                         taxable_gain += gain_eur * 0.35
                         rebates += gain_eur * 0.65
                     elif acq_date <= sell_date_minus_2y:
                         taxable_gain += gain_eur * 0.5
                         rebates += gain_eur * 0.5
                     else:
                         taxable_gain += gain_eur  # too recent to have a rebate
-                elif taxation_scheme == "2018":
+                elif taxation_scheme == RsuTaxScheme.MACRON_3_RSU:
                     # 50% rebate
                     taxable_gain += gain_eur * 0.5
                     rebates_50p += gain_eur * 0.5
                 else:
                     raise Exception(f"Unsupported tax scheme: {taxation_scheme}")
 
         return {
@@ -359,15 +403,15 @@
         tax_report = {
             "2074": [],
             "2042C": {}
         }
         sell_events = self.stock_sales[year]
         total_capital_gain = 0
         for sale in sell_events:
-            if sale.stock_type == "stockoption":
+            if sale.stock_type == StockType.STOCKOPTIONS:
                 # stock option is "exercise and sold" immediately so there is no capital gain
                 continue
             sell_event_report = {}
             sell_event_report["selling_date_512"] = sale.sell_date
             sell_event_report["sell_price_514"] = sale.sell_price_eur
             sell_event_report["sold_stock_units_515"] = sale.nb_stocks_sold
             global_selling_proceeds = sale.sell_price_eur * sale.nb_stocks_sold
```

### Comparing `easyfrenchtax-0.0.6/src/easyfrenchtax/tax_simulator.py` & `easyfrenchtax-0.0.7/src/easyfrenchtax/tax_simulator.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.6/src/easyfrenchtax.egg-info/PKG-INFO` & `easyfrenchtax-0.0.7/src/easyfrenchtax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfrenchtax-0.0.6/tests/test_capital_tax.py` & `easyfrenchtax-0.0.7/tests/test_capital_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.6/tests/test_fiscal_advantages.py` & `easyfrenchtax-0.0.7/tests/test_fiscal_advantages.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.6/tests/test_income_tax.py` & `easyfrenchtax-0.0.7/tests/test_income_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.6/tests/test_rental_tax.py` & `easyfrenchtax-0.0.7/tests/test_rental_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.6/tests/test_stock_helper.py` & `easyfrenchtax-0.0.7/tests/test_stock_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from collections.abc import Callable
 
 import pytest
 from src.easyfrenchtax import StockHelper
 from datetime import date
 from currency_converter import CurrencyConverter
 
+from src.easyfrenchtax.stock_helper import StockType
+
 
 @pytest.fixture
 def stock_helper_with_plan():
     stock_helper = StockHelper()
     stock_helper.rsu_plan("Cake1", date(2016, 6, 28), "CAKE", "USD")
     stock_helper.rsu_vesting("CAKE", "Cake1", 240, date(2018, 6, 29), 20)
     stock_helper.rsu_vesting("CAKE", "Cake1", 10, date(2018, 7, 30), 18)
@@ -204,23 +206,23 @@
     # CAKE=240 ; BUD=200 ; PZZA=150
     stock_helper_with_plan.sell_rsus("CAKE", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_espp("BUD", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     stock_helper_with_plan.sell_stockoptions(1, "PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
-    stock_helper_with_plan.reset(stock_types=["espp"])
+    stock_helper_with_plan.reset(stock_types=[StockType.ESPP])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
-    stock_helper_with_plan.reset(stock_types=["stockoption"])
+    stock_helper_with_plan.reset(stock_types=[StockType.STOCKOPTIONS])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
-    stock_helper_with_plan.reset(stock_types=["rsu"])
+    stock_helper_with_plan.reset(stock_types=[StockType.RSU])
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
     assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
     assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
 
 
 def test_reset_by_symbol(stock_helper_with_plan):
     # CAKE=240 ; BUD=200 ; PZZA=150
```

