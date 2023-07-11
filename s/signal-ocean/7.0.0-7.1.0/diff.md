# Comparing `tmp/signal-ocean-7.0.0.tar.gz` & `tmp/signal-ocean-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal-ocean-7.0.0.tar", last modified: Wed Jul  5 07:32:00 2023, max compression
+gzip compressed data, was "signal-ocean-7.1.0.tar", last modified: Tue Jul 11 15:10:05 2023, max compression
```

## Comparing `signal-ocean-7.0.0.tar` & `signal-ocean-7.1.0.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.052950 signal-ocean-7.0.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2175 2023-07-05 07:32:00.052950 signal-ocean-7.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1184 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 07:32:00.056950 signal-ocean-7.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1524 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.040950 signal-ocean-7.0.0/signal_ocean/
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/_internals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.040950 signal-ocean-7.0.0/signal_ocean/companies/
--rw-r--r--   0 root         (0) root         (0)      236 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/companies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/companies/companies_api.py
--rw-r--r--   0 root         (0) root         (0)     3020 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/companies/models.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.040950 signal-ocean-7.0.0/signal_ocean/distances/
--rw-r--r--   0 root         (0) root         (0)     1210 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/distances/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2523 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/distances/_distances_json.py
--rw-r--r--   0 root         (0) root         (0)    11714 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/distances/distances_api.py
--rw-r--r--   0 root         (0) root         (0)      287 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/distances/loading_condition.py
--rw-r--r--   0 root         (0) root         (0)     4589 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/distances/models.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/distances/port.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/distances/port_filter.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/distances/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/distances/vessel_class_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.044950 signal-ocean-7.0.0/signal_ocean/freight_pricing/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/_freight_pricing_json.py
--rw-r--r--   0 root         (0) root         (0)     4766 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/freight_pricing_api.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/models.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/port.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/port_filter.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/vessel_class_filter.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/vessel_subclass.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/vessel_type.py
--rw-r--r--   0 root         (0) root         (0)      877 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_pricing/vessel_type_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.044950 signal-ocean-7.0.0/signal_ocean/freight_rates/
--rw-r--r--   0 root         (0) root         (0)      565 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_rates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2145 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_rates/_freight_rates_json.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_rates/enums.py
--rw-r--r--   0 root         (0) root         (0)     3750 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_rates/freight_rates_api.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_rates/models.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_rates/port_filter.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/freight_rates/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.044950 signal-ocean-7.0.0/signal_ocean/geos/
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/geos/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4338 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/geos/geos_api.py
--rw-r--r--   0 root         (0) root         (0)     6299 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/geos/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.044950 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/
--rw-r--r--   0 root         (0) root         (0)     2261 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py
--rw-r--r--   0 root         (0) root         (0)      331 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/area.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/column.py
--rw-r--r--   0 root         (0) root         (0)      675 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/commercial_status.py
--rw-r--r--   0 root         (0) root         (0)      235 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/fixture_type.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/historical_tonnage_list.py
--rw-r--r--   0 root         (0) root         (0)     4968 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/index_level.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/location_taxonomy.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/market_deployment.py
--rw-r--r--   0 root         (0) root         (0)     1292 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/operational_status.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/push_type.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/tonnage_list.py
--rw-r--r--   0 root         (0) root         (0)     5517 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/vessel.py
--rw-r--r--   0 root         (0) root         (0)     6831 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/vessel_filter.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/vessel_subclass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.048950 signal-ocean-7.0.0/signal_ocean/market_rates/
--rw-r--r--   0 root         (0) root         (0)      536 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/market_rates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/market_rates/_market_rates_json.py
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/market_rates/enums.py
--rw-r--r--   0 root         (0) root         (0)     4006 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/market_rates/market_rates_api.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/market_rates/models.py
--rw-r--r--   0 root         (0) root         (0)      773 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/market_rates/utils.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/market_rates/vessel_classes.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/plots.py
--rw-r--r--   0 root         (0) root         (0)      578 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.048950 signal-ocean-7.0.0/signal_ocean/port_congestion/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_congestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4274 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_congestion/models.py
--rw-r--r--   0 root         (0) root         (0)    19251 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_congestion/port_congestion.py
--rw-r--r--   0 root         (0) root         (0)     4670 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_congestion/port_congestion_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.048950 signal-ocean-7.0.0/signal_ocean/port_expenses/
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_expenses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1433 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_expenses/_port_expenses_json.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_expenses/enums.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_expenses/models.py
--rw-r--r--   0 root         (0) root         (0)     8527 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_expenses/port_expenses_api.py
--rw-r--r--   0 root         (0) root         (0)      779 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_expenses/port_filter.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/port_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.048950 signal-ocean-7.0.0/signal_ocean/scraped_cargoes/
--rw-r--r--   0 root         (0) root         (0)      277 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_cargoes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26586 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_cargoes/models.py
--rw-r--r--   0 root         (0) root         (0)     5363 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_cargoes/scraped_cargoes_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.048950 signal-ocean-7.0.0/signal_ocean/scraped_data/
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4560 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_data/scraped_data_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.048950 signal-ocean-7.0.0/signal_ocean/scraped_fixtures/
--rw-r--r--   0 root         (0) root         (0)      291 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32666 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_fixtures/models.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_fixtures/scraped_fixtures_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.048950 signal-ocean-7.0.0/signal_ocean/scraped_lineups/
--rw-r--r--   0 root         (0) root         (0)      281 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_lineups/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21114 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_lineups/models.py
--rw-r--r--   0 root         (0) root         (0)     5968 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_lineups/scraped_lineups_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.048950 signal-ocean-7.0.0/signal_ocean/scraped_positions/
--rw-r--r--   0 root         (0) root         (0)      301 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_positions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16973 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_positions/models.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/scraped_positions/scraped_positions_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.048950 signal-ocean-7.0.0/signal_ocean/tonnage_list/
--rw-r--r--   0 root         (0) root         (0)      879 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/tonnage_list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/tonnage_list/_json.py
--rw-r--r--   0 root         (0) root         (0)     6084 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/tonnage_list/api.py
--rw-r--r--   0 root         (0) root         (0)     7229 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/tonnage_list/data_frame.py
--rw-r--r--   0 root         (0) root         (0)    26447 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/tonnage_list/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.048950 signal-ocean-7.0.0/signal_ocean/util/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6505 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/util/parsing_helpers.py
--rw-r--r--   0 root         (0) root         (0)     6529 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/util/request_helpers.py
--rw-r--r--   0 root         (0) root         (0)      647 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessel_class_api.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessel_class_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.052950 signal-ocean-7.0.0/signal_ocean/vessel_emissions/
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessel_emissions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14765 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessel_emissions/models.py
--rw-r--r--   0 root         (0) root         (0)    13047 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessel_emissions/vessel_emissions_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.052950 signal-ocean-7.0.0/signal_ocean/vessel_valuations/
--rw-r--r--   0 root         (0) root         (0)      298 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessel_valuations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessel_valuations/_valuation_json.py
--rw-r--r--   0 root         (0) root         (0)      608 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessel_valuations/models.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessel_valuations/vessel_valuations_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.052950 signal-ocean-7.0.0/signal_ocean/vessels/
--rw-r--r--   0 root         (0) root         (0)      378 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessels/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16693 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessels/models.py
--rw-r--r--   0 root         (0) root         (0)     3207 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/vessels/vessels_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.052950 signal-ocean-7.0.0/signal_ocean/voyages/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/voyages/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46003 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/voyages/models.py
--rw-r--r--   0 root         (0) root         (0)    44702 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/voyages/voyages_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.052950 signal-ocean-7.0.0/signal_ocean/voyages_market_data/
--rw-r--r--   0 root         (0) root         (0)      539 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/voyages_market_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15350 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/voyages_market_data/models.py
--rw-r--r--   0 root         (0) root         (0)    15865 2023-07-05 07:30:40.000000 signal-ocean-7.0.0/signal_ocean/voyages_market_data/voyages_market_data_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:32:00.040950 signal-ocean-7.0.0/signal_ocean.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2175 2023-07-05 07:31:59.000000 signal-ocean-7.0.0/signal_ocean.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5081 2023-07-05 07:31:59.000000 signal-ocean-7.0.0/signal_ocean.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:31:59.000000 signal-ocean-7.0.0/signal_ocean.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-07-05 07:31:59.000000 signal-ocean-7.0.0/signal_ocean.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 07:31:59.000000 signal-ocean-7.0.0/signal_ocean.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-11 15:10:05.677616 signal-ocean-7.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.661617 signal-ocean-7.1.0/signal_ocean/
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/_internals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean/companies/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/companies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/companies/companies_api.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/companies/models.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean/distances/
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/_distances_json.py
+-rw-r--r--   0 root         (0) root         (0)    11714 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/distances_api.py
+-rw-r--r--   0 root         (0) root         (0)      287 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/loading_condition.py
+-rw-r--r--   0 root         (0) root         (0)     4589 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/models.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/port.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/vessel_class_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean/freight_pricing/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/_freight_pricing_json.py
+-rw-r--r--   0 root         (0) root         (0)     4766 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/freight_pricing_api.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/models.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/port.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_class_filter.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_subclass.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_type.py
+-rw-r--r--   0 root         (0) root         (0)      877 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_type_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean/freight_rates/
+-rw-r--r--   0 root         (0) root         (0)      565 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/_freight_rates_json.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/enums.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/freight_rates_api.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/models.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean/geos/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/geos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4338 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/geos/geos_api.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/geos/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py
+-rw-r--r--   0 root         (0) root         (0)      331 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/area.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/column.py
+-rw-r--r--   0 root         (0) root         (0)      675 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/commercial_status.py
+-rw-r--r--   0 root         (0) root         (0)      235 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/fixture_type.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list.py
+-rw-r--r--   0 root         (0) root         (0)     4968 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/index_level.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/location_taxonomy.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/market_deployment.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/operational_status.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/push_type.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/tonnage_list.py
+-rw-r--r--   0 root         (0) root         (0)     5517 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel.py
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel_filter.py
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel_subclass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/market_rates/
+-rw-r--r--   0 root         (0) root         (0)      536 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/_market_rates_json.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/enums.py
+-rw-r--r--   0 root         (0) root         (0)     4006 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/market_rates_api.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/models.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/vessel_classes.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/plots.py
+-rw-r--r--   0 root         (0) root         (0)      578 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/port.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/port_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/port_congestion/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/port_congestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_congestion/models.py
+-rw-r--r--   0 root         (0) root         (0)    19251 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_congestion/port_congestion.py
+-rw-r--r--   0 root         (0) root         (0)     4670 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_congestion/port_congestion_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/port_expenses/
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/_port_expenses_json.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/models.py
+-rw-r--r--   0 root         (0) root         (0)     8527 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/port_expenses_api.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/scraped_cargoes/
+-rw-r--r--   0 root         (0) root         (0)      277 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_cargoes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26586 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_cargoes/models.py
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_cargoes/scraped_cargoes_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/scraped_data/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_data/scraped_data_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/scraped_fixtures/
+-rw-r--r--   0 root         (0) root         (0)      291 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32666 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_fixtures/models.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_fixtures/scraped_fixtures_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/scraped_lineups/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_lineups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21114 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_lineups/models.py
+-rw-r--r--   0 root         (0) root         (0)     5968 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_lineups/scraped_lineups_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/scraped_positions/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_positions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16973 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_positions/models.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_positions/scraped_positions_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/tonnage_list/
+-rw-r--r--   0 root         (0) root         (0)      879 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/tonnage_list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/tonnage_list/_json.py
+-rw-r--r--   0 root         (0) root         (0)     6084 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/tonnage_list/api.py
+-rw-r--r--   0 root         (0) root         (0)     7229 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/tonnage_list/data_frame.py
+-rw-r--r--   0 root         (0) root         (0)    26447 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/tonnage_list/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/util/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6505 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/util/parsing_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     6529 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/util/request_helpers.py
+-rw-r--r--   0 root         (0) root         (0)      647 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_class_api.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_class_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/vessel_emissions/
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_emissions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14765 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_emissions/models.py
+-rw-r--r--   0 root         (0) root         (0)    13047 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_emissions/vessel_emissions_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/vessel_valuations/
+-rw-r--r--   0 root         (0) root         (0)      298 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_valuations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_valuations/_valuation_json.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_valuations/models.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_valuations/vessel_valuations_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/vessels/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17416 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessels/models.py
+-rw-r--r--   0 root         (0) root         (0)     3539 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessels/vessels_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/voyages/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46003 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages/models.py
+-rw-r--r--   0 root         (0) root         (0)    44702 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages/voyages_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/voyages_market_data/
+-rw-r--r--   0 root         (0) root         (0)      539 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages_market_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15350 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages_market_data/models.py
+-rw-r--r--   0 root         (0) root         (0)    15865 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages_market_data/voyages_market_data_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-07-11 15:10:05.000000 signal-ocean-7.1.0/signal_ocean.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5081 2023-07-11 15:10:05.000000 signal-ocean-7.1.0/signal_ocean.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:10:05.000000 signal-ocean-7.1.0/signal_ocean.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2023-07-11 15:10:05.000000 signal-ocean-7.1.0/signal_ocean.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 15:10:05.000000 signal-ocean-7.1.0/signal_ocean.egg-info/top_level.txt
```

### Comparing `signal-ocean-7.0.0/LICENSE` & `signal-ocean-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/PKG-INFO` & `signal-ocean-7.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-ocean
-Version: 7.0.0
+Version: 7.1.0
 Summary: Access Signal Ocean Platform data using Python.
 Home-page: https://apis.signalocean.com/
 Author: Signal Ocean Developers
 Author-email: signaloceandevelopers@thesignalgroup.com
 License: Apache 2.0
 Project-URL: The Signal Group, https://www.thesignalgroup.com/
 Project-URL: Signal Ocean, https://www.signalocean.com/
```

### Comparing `signal-ocean-7.0.0/README.md` & `signal-ocean-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/setup.py` & `signal-ocean-7.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/__init__.py` & `signal-ocean-7.1.0/signal_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/_internals.py` & `signal-ocean-7.1.0/signal_ocean/_internals.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/companies/companies_api.py` & `signal-ocean-7.1.0/signal_ocean/companies/companies_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/companies/models.py` & `signal-ocean-7.1.0/signal_ocean/companies/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/connection.py` & `signal-ocean-7.1.0/signal_ocean/connection.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/distances/__init__.py` & `signal-ocean-7.1.0/signal_ocean/distances/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/distances/_distances_json.py` & `signal-ocean-7.1.0/signal_ocean/distances/_distances_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/distances/distances_api.py` & `signal-ocean-7.1.0/signal_ocean/distances/distances_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/distances/models.py` & `signal-ocean-7.1.0/signal_ocean/distances/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/distances/port_filter.py` & `signal-ocean-7.1.0/signal_ocean/distances/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/distances/vessel_class_filter.py` & `signal-ocean-7.1.0/signal_ocean/distances/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_pricing/__init__.py` & `signal-ocean-7.1.0/signal_ocean/freight_pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_pricing/_freight_pricing_json.py` & `signal-ocean-7.1.0/signal_ocean/freight_pricing/_freight_pricing_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_pricing/freight_pricing_api.py` & `signal-ocean-7.1.0/signal_ocean/freight_pricing/freight_pricing_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_pricing/models.py` & `signal-ocean-7.1.0/signal_ocean/freight_pricing/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_pricing/port_filter.py` & `signal-ocean-7.1.0/signal_ocean/freight_pricing/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_pricing/vessel_class_filter.py` & `signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_pricing/vessel_type_filter.py` & `signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_type_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_rates/__init__.py` & `signal-ocean-7.1.0/signal_ocean/freight_rates/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_rates/_freight_rates_json.py` & `signal-ocean-7.1.0/signal_ocean/freight_rates/_freight_rates_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_rates/enums.py` & `signal-ocean-7.1.0/signal_ocean/freight_rates/enums.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_rates/freight_rates_api.py` & `signal-ocean-7.1.0/signal_ocean/freight_rates/freight_rates_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_rates/models.py` & `signal-ocean-7.1.0/signal_ocean/freight_rates/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_rates/port_filter.py` & `signal-ocean-7.1.0/signal_ocean/freight_rates/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/freight_rates/utils.py` & `signal-ocean-7.1.0/signal_ocean/freight_rates/utils.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/geos/geos_api.py` & `signal-ocean-7.1.0/signal_ocean/geos/geos_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/geos/models.py` & `signal-ocean-7.1.0/signal_ocean/geos/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/__init__.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/column.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/column.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/commercial_status.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/commercial_status.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/historical_tonnage_list.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/market_deployment.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/market_deployment.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/operational_status.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/operational_status.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/tonnage_list.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/tonnage_list.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/vessel.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/vessel_filter.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/historical_tonnage_list/vessel_subclass.py` & `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel_subclass.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/market_rates/__init__.py` & `signal-ocean-7.1.0/signal_ocean/market_rates/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/market_rates/_market_rates_json.py` & `signal-ocean-7.1.0/signal_ocean/market_rates/_market_rates_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/market_rates/market_rates_api.py` & `signal-ocean-7.1.0/signal_ocean/market_rates/market_rates_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/market_rates/models.py` & `signal-ocean-7.1.0/signal_ocean/market_rates/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/market_rates/utils.py` & `signal-ocean-7.1.0/signal_ocean/market_rates/utils.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/market_rates/vessel_classes.py` & `signal-ocean-7.1.0/signal_ocean/market_rates/vessel_classes.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/plots.py` & `signal-ocean-7.1.0/signal_ocean/plots.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port.py` & `signal-ocean-7.1.0/signal_ocean/port.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_api.py` & `signal-ocean-7.1.0/signal_ocean/port_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_congestion/models.py` & `signal-ocean-7.1.0/signal_ocean/port_congestion/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_congestion/port_congestion.py` & `signal-ocean-7.1.0/signal_ocean/port_congestion/port_congestion.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_congestion/port_congestion_api.py` & `signal-ocean-7.1.0/signal_ocean/port_congestion/port_congestion_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_expenses/__init__.py` & `signal-ocean-7.1.0/signal_ocean/port_expenses/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_expenses/_port_expenses_json.py` & `signal-ocean-7.1.0/signal_ocean/port_expenses/_port_expenses_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_expenses/enums.py` & `signal-ocean-7.1.0/signal_ocean/port_expenses/enums.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_expenses/models.py` & `signal-ocean-7.1.0/signal_ocean/port_expenses/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_expenses/port_expenses_api.py` & `signal-ocean-7.1.0/signal_ocean/port_expenses/port_expenses_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_expenses/port_filter.py` & `signal-ocean-7.1.0/signal_ocean/port_expenses/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/port_filter.py` & `signal-ocean-7.1.0/signal_ocean/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/scraped_cargoes/models.py` & `signal-ocean-7.1.0/signal_ocean/scraped_cargoes/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/scraped_cargoes/scraped_cargoes_api.py` & `signal-ocean-7.1.0/signal_ocean/scraped_cargoes/scraped_cargoes_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/scraped_data/scraped_data_api.py` & `signal-ocean-7.1.0/signal_ocean/scraped_data/scraped_data_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/scraped_fixtures/models.py` & `signal-ocean-7.1.0/signal_ocean/scraped_fixtures/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/scraped_fixtures/scraped_fixtures_api.py` & `signal-ocean-7.1.0/signal_ocean/scraped_fixtures/scraped_fixtures_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/scraped_lineups/models.py` & `signal-ocean-7.1.0/signal_ocean/scraped_lineups/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/scraped_lineups/scraped_lineups_api.py` & `signal-ocean-7.1.0/signal_ocean/scraped_lineups/scraped_lineups_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/scraped_positions/models.py` & `signal-ocean-7.1.0/signal_ocean/scraped_positions/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/scraped_positions/scraped_positions_api.py` & `signal-ocean-7.1.0/signal_ocean/scraped_positions/scraped_positions_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/tonnage_list/__init__.py` & `signal-ocean-7.1.0/signal_ocean/tonnage_list/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/tonnage_list/_json.py` & `signal-ocean-7.1.0/signal_ocean/tonnage_list/_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/tonnage_list/api.py` & `signal-ocean-7.1.0/signal_ocean/tonnage_list/api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/tonnage_list/data_frame.py` & `signal-ocean-7.1.0/signal_ocean/tonnage_list/data_frame.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/tonnage_list/models.py` & `signal-ocean-7.1.0/signal_ocean/tonnage_list/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/util/parsing_helpers.py` & `signal-ocean-7.1.0/signal_ocean/util/parsing_helpers.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/util/request_helpers.py` & `signal-ocean-7.1.0/signal_ocean/util/request_helpers.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/vessel_class.py` & `signal-ocean-7.1.0/signal_ocean/vessel_class.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/vessel_class_api.py` & `signal-ocean-7.1.0/signal_ocean/vessel_class_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/vessel_class_filter.py` & `signal-ocean-7.1.0/signal_ocean/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/vessel_emissions/__init__.py` & `signal-ocean-7.1.0/signal_ocean/vessel_emissions/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/vessel_emissions/models.py` & `signal-ocean-7.1.0/signal_ocean/vessel_emissions/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/vessel_emissions/vessel_emissions_api.py` & `signal-ocean-7.1.0/signal_ocean/vessel_emissions/vessel_emissions_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/vessel_valuations/_valuation_json.py` & `signal-ocean-7.1.0/signal_ocean/vessel_valuations/_valuation_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/vessel_valuations/models.py` & `signal-ocean-7.1.0/signal_ocean/vessel_valuations/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/vessel_valuations/vessel_valuations_api.py` & `signal-ocean-7.1.0/signal_ocean/vessel_valuations/vessel_valuations_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/vessels/models.py` & `signal-ocean-7.1.0/signal_ocean/vessels/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,23 @@
             of the vessel
         beneficial_owner: Name of the beneficial owner of the vessel
         parallel_body_length: The Parallel Body Length of the vessel
         heating_coils_fitted: Boolean, denotes whether the vessel is equipped
             with a heating coils system. Tanker vessels may be fitted with
             heating coils in order to maintain the required temperature of
             the cargo for pumping.
+        bwts: Boolean, denotes whether the vessel has any Ballast Water
+            Treatment System. This system is designed to remove and
+            destroy/inactive biological organisms (zooplankton, algae,
+            bacteria) from ballast water.
+        grabs_fitted: Boolean, denotes whether the vessel is fitted with
+            grabs. Grabs are fitted on cranes to allow the handling of cargo.
+        ghg: String, denotes the vessel’s GHG (Greenhouse Gas) Emissions
+            Rating. Developed by RightShip, GHG compares a ship's
+            design efficiency with peer vessels using a simple A–G scale.
     """
 
     imo: int
     vessel_type_id: int
     built_for_trade_id: int
     trade_id: int
     vessel_class_id: int
@@ -313,7 +322,10 @@
     zinc_coating: Optional[int] = None
     marineline_coating: Optional[int] = None
     crude_oil_washing: Optional[str] = None
     beneficial_owner_id: Optional[int] = None
     beneficial_owner: Optional[str] = None
     parallel_body_length: Optional[float] = None
     heating_coils_fitted: Optional[bool] = None
+    bwts: Optional[bool] = None
+    grabs_fitted: Optional[bool] = None
+    ghg: Optional[str] = None
```

### Comparing `signal-ocean-7.0.0/signal_ocean/vessels/vessels_api.py` & `signal-ocean-7.1.0/signal_ocean/vessels/vessels_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,17 @@
 
         Returns:
             A vessel or None if no vessel with the specified IMO has
                 been found.
         """
         url = urljoin(VesselsAPI.relative_url, f"vessels/{imo}")
         return get_single(self.__connection, url, Vessel,
-                          rename_keys={"STSTCoating": "stst_coating"})
+                          rename_keys={"STSTCoating": "stst_coating",
+                                       "BWTS": "bwts",
+                                       "GHG": "ghg"})
 
     def get_vessels(self, name: Optional[str] = None) -> Tuple[Vessel, ...]:
         """Retrieves all available vessels.
 
         Args:
                 name: String to filter and return only companies the name
                         of which contains the provided string. If None, all
@@ -66,15 +68,17 @@
             A tuple of all available vessels.
         """
         endpoint = (
             "vessels/all" if name is None else f"vessels/searchByName/{name}"
         )
         url = urljoin(VesselsAPI.relative_url, endpoint)
         return get_multiple(self.__connection, url, Vessel,
-                            rename_keys={"STSTCoating": "stst_coating"})
+                            rename_keys={"STSTCoating": "stst_coating",
+                                         "BWTS": "bwts",
+                                         "GHG": "ghg"})
 
     def get_vessels_by_vessel_class(
         self, vesselClass: int, point_in_time: Optional[str] = default_pit
     ) -> Tuple[Vessel, ...]:
         """Retrieves all vessels of a specific vessel class.
 
         Args:
@@ -82,8 +86,10 @@
 
         Returns:
             A tuple of all available vessels.
         """
         endpoint = f"pointInTime/{point_in_time}/byVesselClass/{vesselClass}"
         url = urljoin(VesselsAPI.relative_url, endpoint)
         return get_multiple(self.__connection, url, Vessel,
-                            rename_keys={"STSTCoating": "stst_coating"})
+                            rename_keys={"STSTCoating": "stst_coating",
+                                         "BWTS": "bwts",
+                                         "GHG": "ghg"})
```

### Comparing `signal-ocean-7.0.0/signal_ocean/voyages/__init__.py` & `signal-ocean-7.1.0/signal_ocean/voyages/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/voyages/models.py` & `signal-ocean-7.1.0/signal_ocean/voyages/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/voyages/voyages_api.py` & `signal-ocean-7.1.0/signal_ocean/voyages/voyages_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/voyages_market_data/__init__.py` & `signal-ocean-7.1.0/signal_ocean/voyages_market_data/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/voyages_market_data/models.py` & `signal-ocean-7.1.0/signal_ocean/voyages_market_data/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean/voyages_market_data/voyages_market_data_api.py` & `signal-ocean-7.1.0/signal_ocean/voyages_market_data/voyages_market_data_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.0.0/signal_ocean.egg-info/PKG-INFO` & `signal-ocean-7.1.0/signal_ocean.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-ocean
-Version: 7.0.0
+Version: 7.1.0
 Summary: Access Signal Ocean Platform data using Python.
 Home-page: https://apis.signalocean.com/
 Author: Signal Ocean Developers
 Author-email: signaloceandevelopers@thesignalgroup.com
 License: Apache 2.0
 Project-URL: The Signal Group, https://www.thesignalgroup.com/
 Project-URL: Signal Ocean, https://www.signalocean.com/
```

### Comparing `signal-ocean-7.0.0/signal_ocean.egg-info/SOURCES.txt` & `signal-ocean-7.1.0/signal_ocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

