# Comparing `tmp/coinmetrics_api_client-2023.6.8.20.tar.gz` & `tmp/coinmetrics_api_client-2023.7.11.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinmetrics_api_client-2023.6.8.20.tar", max compression
+gzip compressed data, was "coinmetrics_api_client-2023.7.11.17.tar", max compression
```

## Comparing `coinmetrics_api_client-2023.6.8.20.tar` & `coinmetrics_api_client-2023.7.11.17.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1088 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/LICENSE
--rw-r--r--   0        0        0    20460 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/README.md
--rw-r--r--   0        0        0       28 2023-06-08 20:26:54.999797 coinmetrics_api_client-2023.6.8.20/coinmetrics/__init__.py
--rw-r--r--   0        0        0    20960 2023-06-08 16:41:39.966788 coinmetrics_api_client-2023.6.8.20/coinmetrics/_catalogs.py
--rw-r--r--   0        0        0     9947 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/_data_collection.py
--rw-r--r--   0        0        0     2328 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/_exceptions.py
--rw-r--r--   0        0        0     1286 2023-06-07 14:08:45.748120 coinmetrics_api_client-2023.6.8.20/coinmetrics/_models.py
--rw-r--r--   0        0        0      699 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/_typing.py
--rw-r--r--   0        0        0     3951 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/_utils.py
--rw-r--r--   0        0        0   233688 2023-06-07 14:08:45.748120 coinmetrics_api_client-2023.6.8.20/coinmetrics/api_client.py
--rw-r--r--   0        0        0        0 2023-06-08 20:34:37.623456 coinmetrics_api_client-2023.6.8.20/coinmetrics/build.py
--rw-r--r--   0        0        0      148 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/constants.py
--rw-r--r--   0        0        0    20520 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/data_exporter.py
--rw-r--r--   0        0        0     8669 2023-05-12 17:43:51.950025 coinmetrics_api_client-2023.6.8.20/coinmetrics/typer_cli.py
--rw-r--r--   0        0        0     1236 2023-06-08 20:26:54.999797 coinmetrics_api_client-2023.6.8.20/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 20:34:37.627456 coinmetrics_api_client-2023.6.8.20/test/__init__.py
--rw-r--r--   0        0        0     1640 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_asset_pair_candles.csv
--rw-r--r--   0        0        0      412 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_asset_pairs.csv
--rw-r--r--   0        0        0     2097 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_assets_markets.csv
--rw-r--r--   0        0        0      605 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_assets_metrics.csv
--rw-r--r--   0        0        0      436 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_exchange_assets.csv
--rw-r--r--   0        0        0     3595 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_exchanges_markets.csv
--rw-r--r--   0        0        0      822 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_exchanges_metrics.csv
--rw-r--r--   0        0        0      556 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_indexes.csv
--rw-r--r--   0        0        0      223 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_institutions.csv
--rw-r--r--   0        0        0      178 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_market_orderbooks.csv
--rw-r--r--   0        0        0      254 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_market_quotes.csv
--rw-r--r--   0        0        0      297 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_market_trades.csv
--rw-r--r--   0        0        0      579 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_markets.csv
--rw-r--r--   0        0        0     2557 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/data/catalog_metrics.csv
--rw-r--r--   0        0        0    28915 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_api_client.py
--rw-r--r--   0        0        0    10311 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_api_methods.py
--rw-r--r--   0        0        0     2910 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_as_list.py
--rw-r--r--   0        0        0     1788 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_blockchain_methods.py
--rw-r--r--   0        0        0     2273 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_custom_exceptions.py
--rw-r--r--   0        0        0    13462 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_data_exporter.py
--rw-r--r--   0        0        0     1015 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_debugging.py
--rw-r--r--   0        0        0     2142 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_models.py
--rw-r--r--   0        0        0     1193 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_rate_limits.py
--rw-r--r--   0        0        0    14793 2023-06-08 16:41:39.966788 coinmetrics_api_client-2023.6.8.20/test/test_to_dataframe.py
--rw-r--r--   0        0        0     5829 2023-05-12 17:43:51.994026 coinmetrics_api_client-2023.6.8.20/test/test_websocket_methods.py
--rw-r--r--   0        0        0    21648 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.6.8.20/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/LICENSE
+-rw-r--r--   0        0        0    20461 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/README.md
+-rw-r--r--   0        0        0       29 2023-07-11 17:23:23.700383 coinmetrics_api_client-2023.7.11.17/coinmetrics/__init__.py
+-rw-r--r--   0        0        0    21023 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_catalogs.py
+-rw-r--r--   0        0        0     9947 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_data_collection.py
+-rw-r--r--   0        0        0     2328 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_exceptions.py
+-rw-r--r--   0        0        0     1286 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_models.py
+-rw-r--r--   0        0        0      699 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_typing.py
+-rw-r--r--   0        0        0     3951 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_utils.py
+-rw-r--r--   0        0        0   233688 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/api_client.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:05:55.696998 coinmetrics_api_client-2023.7.11.17/coinmetrics/build.py
+-rw-r--r--   0        0        0      148 2023-07-11 17:15:41.006507 coinmetrics_api_client-2023.7.11.17/coinmetrics/constants.py
+-rw-r--r--   0        0        0    20520 2023-07-11 17:15:41.006507 coinmetrics_api_client-2023.7.11.17/coinmetrics/data_exporter.py
+-rw-r--r--   0        0        0     8669 2023-07-11 17:15:41.006507 coinmetrics_api_client-2023.7.11.17/coinmetrics/typer_cli.py
+-rw-r--r--   0        0        0     1237 2023-07-11 17:23:23.700383 coinmetrics_api_client-2023.7.11.17/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 20:05:55.700998 coinmetrics_api_client-2023.7.11.17/test/__init__.py
+-rw-r--r--   0        0        0     1640 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_asset_pair_candles.csv
+-rw-r--r--   0        0        0      412 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_asset_pairs.csv
+-rw-r--r--   0        0        0     2097 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_assets_markets.csv
+-rw-r--r--   0        0        0      605 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_assets_metrics.csv
+-rw-r--r--   0        0        0      436 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_exchange_assets.csv
+-rw-r--r--   0        0        0     3595 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_exchanges_markets.csv
+-rw-r--r--   0        0        0      822 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_exchanges_metrics.csv
+-rw-r--r--   0        0        0      556 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_indexes.csv
+-rw-r--r--   0        0        0      223 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_institutions.csv
+-rw-r--r--   0        0        0      178 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_market_orderbooks.csv
+-rw-r--r--   0        0        0      254 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_market_quotes.csv
+-rw-r--r--   0        0        0      297 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_market_trades.csv
+-rw-r--r--   0        0        0      582 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_markets.csv
+-rw-r--r--   0        0        0     2557 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_metrics.csv
+-rw-r--r--   0        0        0    28630 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_api_client.py
+-rw-r--r--   0        0        0    10311 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_api_methods.py
+-rw-r--r--   0        0        0     2910 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_as_list.py
+-rw-r--r--   0        0        0     1788 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_blockchain_methods.py
+-rw-r--r--   0        0        0     2273 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_custom_exceptions.py
+-rw-r--r--   0        0        0    13462 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_data_exporter.py
+-rw-r--r--   0        0        0     1015 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_debugging.py
+-rw-r--r--   0        0        0     2142 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_models.py
+-rw-r--r--   0        0        0     1193 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_rate_limits.py
+-rw-r--r--   0        0        0    15850 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_to_dataframe.py
+-rw-r--r--   0        0        0     5829 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_websocket_methods.py
+-rw-r--r--   0        0        0    21650 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.7.11.17/PKG-INFO
```

### Comparing `coinmetrics_api_client-2023.6.8.20/LICENSE` & `coinmetrics_api_client-2023.7.11.17/LICENSE`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/README.md` & `coinmetrics_api_client-2023.7.11.17/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -389,9 +389,10 @@
 For proxies that require auth, you should be able to specify username and password similar to this example:
 ```python
 
 client = CoinMetricsClient(proxy_url=f'http://<username>:<password>@<hostname>:<port>')
 ```
 
 ## Extended documentation
+
 For more information about the available methods in the client please reference [API Client Spec](https://coinmetrics.github.io/api-client-python/site/api_client.html)
```

### Comparing `coinmetrics_api_client-2023.6.8.20/coinmetrics/_catalogs.py` & `coinmetrics_api_client-2023.7.11.17/coinmetrics/_catalogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
     return list(map(_assign_value, iterable))
 
 
 def convert_catalog_dtypes(df: DataFrameType) -> DataFrameType:
     df = df.convert_dtypes()
     columns = df.columns
-    datetime_cols = [c for c in columns if c.endswith("_time") or c == "time"]
+    date_cols = {"expiration", "listing"}
+    datetime_cols = [c for c in columns if "time" in c.split("_") or c == "time" or c in date_cols]
     for col in datetime_cols:
         df[col] = df[col].apply(_convert_utc)
     return df
 
 
 class CatalogAssetsData(List[Any]):
     def to_dataframe(self, secondary_level: Optional[str] = None) -> DataFrameType:
```

### Comparing `coinmetrics_api_client-2023.6.8.20/coinmetrics/_data_collection.py` & `coinmetrics_api_client-2023.7.11.17/coinmetrics/_data_collection.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/coinmetrics/_exceptions.py` & `coinmetrics_api_client-2023.7.11.17/coinmetrics/_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/coinmetrics/_models.py` & `coinmetrics_api_client-2023.7.11.17/coinmetrics/_models.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/coinmetrics/_typing.py` & `coinmetrics_api_client-2023.7.11.17/coinmetrics/_typing.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/coinmetrics/_utils.py` & `coinmetrics_api_client-2023.7.11.17/coinmetrics/_utils.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/coinmetrics/api_client.py` & `coinmetrics_api_client-2023.7.11.17/coinmetrics/api_client.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/coinmetrics/data_exporter.py` & `coinmetrics_api_client-2023.7.11.17/coinmetrics/data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/coinmetrics/typer_cli.py` & `coinmetrics_api_client-2023.7.11.17/coinmetrics/typer_cli.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/pyproject.toml` & `coinmetrics_api_client-2023.7.11.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coinmetrics-api-client"
-version = "2023.6.8.20"
+version = "2023.7.11.17"
 description = "Python client for Coin Metrics API v4."
 authors = ["Coin Metrics <info@coinmetrics.io>", "Oleksandr Buchkovskyi <oleksandr@coinmetrics.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://coinmetrics.github.io/api-client-python/site/index.html"
 repository = "https://github.com/coinmetrics/api-client-python"
 packages = [{include = "coinmetrics"}]
```

### Comparing `coinmetrics_api_client-2023.6.8.20/test/data/catalog_asset_pair_candles.csv` & `coinmetrics_api_client-2023.7.11.17/test/data/catalog_asset_pair_candles.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/data/catalog_assets_markets.csv` & `coinmetrics_api_client-2023.7.11.17/test/data/catalog_assets_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/data/catalog_assets_metrics.csv` & `coinmetrics_api_client-2023.7.11.17/test/data/catalog_assets_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/data/catalog_exchanges_markets.csv` & `coinmetrics_api_client-2023.7.11.17/test/data/catalog_exchanges_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/data/catalog_exchanges_metrics.csv` & `coinmetrics_api_client-2023.7.11.17/test/data/catalog_exchanges_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/data/catalog_indexes.csv` & `coinmetrics_api_client-2023.7.11.17/test/data/catalog_indexes.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/data/catalog_markets.csv` & `coinmetrics_api_client-2023.7.11.17/test/data/catalog_markets.csv`

 * *Files 19% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 market,min_time,max_time,exchange,type,symbol,base,quote,size_asset,margin_asset,contract_size,tick_size,listing,expiration,min_time_trades,max_time_trades
-0,bitmex-XBTF15-future,2014-11-24 13:05:32.850000+00:00,2015-01-30 12:00:00+00:00,bitmex,future,XBTF15,btc,usd,XBT,USD,1,0.1,2014-11-24T13:05:32.850000000Z,2015-01-30T12:00:00.000000000Z,2014-11-24T13:05:32.850000000Z,2015-01-30T12:00:00.000000000Z
+0,bitmex-XBTF15-future,2014-11-24 13:05:32.850000+00:00,2015-01-30 12:00:00+00:00,bitmex,future,XBTF15,btc,usd,XBT,USD,1,0.1,'2014-11-24 13:05:32.850000+00:00','2015-01-30 12:00:00+00:00','2014-11-24 13:05:32.850000+00:00', '2015-01-30 12:00:00+00:00'
 1,bitfinex-agi-btc-spot,2018-04-07 16:25:55+00:00,2020-03-25 20:12:09.639000+00:00,bitfinex,spot,,agi,btc,,,,,,,2018-04-07T16:25:55.000000000Z,2020-03-25T20:12:09.639000000Z
```

### Comparing `coinmetrics_api_client-2023.6.8.20/test/data/catalog_metrics.csv` & `coinmetrics_api_client-2023.7.11.17/test/data/catalog_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_api_client.py` & `coinmetrics_api_client-2023.7.11.17/test/test_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -656,21 +656,14 @@
 def test_catalog_metrics_dataframe() -> None:
     data = CatalogMetricsData(catalog_metrics_test_data)
     df = data.to_dataframe().fillna("")
     df_test = pd.read_csv("test/data/catalog_metrics.csv", dtype=str).fillna("")
     assert (df.values == df_test.values).all()
 
 
-def test_catalog_markets_dataframe() -> None:
-    data = CatalogMarketsData(catalog_markets_test_data)
-    df = data.to_dataframe().fillna("").astype(str)
-    df_test = pd.read_csv("test/data/catalog_markets.csv", dtype=str).fillna("")
-    assert (df.values == df_test.values).all()
-
-
 def test_catalog_exchanges_dataframe() -> None:
     data = CatalogExchangesData(catalog_exchanges_test_data)
     df = data.to_dataframe()
     assert len(df) == df.exchange.nunique()
     df_markets = data.to_dataframe(secondary_level="markets")
     df_markets = df_markets.fillna("").astype(str)
     df_markets_test = pd.read_csv(
```

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_api_methods.py` & `coinmetrics_api_client-2023.7.11.17/test/test_api_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_as_list.py` & `coinmetrics_api_client-2023.7.11.17/test/test_as_list.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_blockchain_methods.py` & `coinmetrics_api_client-2023.7.11.17/test/test_blockchain_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_custom_exceptions.py` & `coinmetrics_api_client-2023.7.11.17/test/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_data_exporter.py` & `coinmetrics_api_client-2023.7.11.17/test/test_data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_debugging.py` & `coinmetrics_api_client-2023.7.11.17/test/test_debugging.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_models.py` & `coinmetrics_api_client-2023.7.11.17/test/test_models.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_rate_limits.py` & `coinmetrics_api_client-2023.7.11.17/test/test_rate_limits.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_to_dataframe.py` & `coinmetrics_api_client-2023.7.11.17/test/test_to_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd  # type: ignore
 import pytest
 from coinmetrics.api_client import CoinMetricsClient
 import os
+import numpy as np
 
 CM_API_KEY = os.environ.get("CM_API_KEY")
 client = CoinMetricsClient(str(CM_API_KEY))
 cm_api_key_set = CM_API_KEY is not None
 REASON_TO_SKIP = "Need to set CM_API_KEY as an env var in order to run this test"
 
 
@@ -392,10 +393,32 @@
     for catalog_data in list_data:
         for metric_data in catalog_data['metrics']:
             count_markets_and_frequencies += len(metric_data['frequencies'])
     as_data_frame = list_data.to_dataframe()
     count_df_rows = len(as_data_frame)
     assert count_df_rows == count_markets_and_frequencies
 
+@pytest.mark.skipif(not cm_api_key_set, reason=REASON_TO_SKIP)
+def test_catalog_markets_dtypes() -> None:
+    """
+    Tests catalog markets return data types as expected for new time cols
+    """
+    markets: pd.DataFrame = client.catalog_markets(exchange="binance").to_dataframe()
+    expected_dtype_cols = {"min_time_trades",
+                             "max_time_trades",
+                             "min_time_funding_rates",
+                             "max_time_funding_rates",
+                             "min_time_openinterest",
+                             "max_time_openinterest",
+                             "min_time_liquidations",
+                             "max_time_liquidations",
+                             "listing",
+                             "expiration"}
+    for type_name, dtype in markets.dtypes.items():
+        if type_name in expected_dtype_cols:
+            assert type(dtype == pd.core.dtypes.dtypes.DatetimeTZDtype)
+    spot_check = markets['listing'][0]
+    assert type(spot_check) == pd.Timestamp
+
 
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `coinmetrics_api_client-2023.6.8.20/test/test_websocket_methods.py` & `coinmetrics_api_client-2023.7.11.17/test/test_websocket_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.6.8.20/PKG-INFO` & `coinmetrics_api_client-2023.7.11.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinmetrics-api-client
-Version: 2023.6.8.20
+Version: 2023.7.11.17
 Summary: Python client for Coin Metrics API v4.
 Home-page: https://coinmetrics.github.io/api-client-python/site/index.html
 License: MIT
 Keywords: coin metrics,coin,metrics,crypto,bitcoin,network-data,market-data,api,handy
 Author: Coin Metrics
 Author-email: info@coinmetrics.io
 Requires-Python: >=3.7.1,<4.0.0
@@ -416,10 +416,11 @@
 For proxies that require auth, you should be able to specify username and password similar to this example:
 ```python
 
 client = CoinMetricsClient(proxy_url=f'http://<username>:<password>@<hostname>:<port>')
 ```
 
 ## Extended documentation
+
 For more information about the available methods in the client please reference [API Client Spec](https://coinmetrics.github.io/api-client-python/site/api_client.html)
```

