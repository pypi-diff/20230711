# Comparing `tmp/morningstar_data-1.3.0.tar.gz` & `tmp/morningstar_data-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morningstar_data-1.3.0.tar", max compression
+gzip compressed data, was "morningstar_data-1.3.1.tar", max compression
```

## Comparing `morningstar_data-1.3.0.tar` & `morningstar_data-1.3.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      558 2023-06-22 23:57:19.310138 morningstar_data-1.3.0/LICENSE
--rw-r--r--   0        0        0    11361 2023-06-22 23:57:19.310422 morningstar_data-1.3.0/README.md
--rw-r--r--   0        0        0      207 2023-06-22 17:07:28.074097 morningstar_data-1.3.0/morningstar_data/__init__.py
--rw-r--r--   0        0        0      599 2023-06-22 17:07:28.074722 morningstar_data-1.3.0/morningstar_data/_base.py
--rw-r--r--   0        0        0     3056 2023-06-14 19:10:47.534369 morningstar_data-1.3.0/morningstar_data/_utils.py
--rw-r--r--   0        0        0       82 2023-06-22 17:07:28.075331 morningstar_data-1.3.0/morningstar_data/_version.py
--rw-r--r--   0        0        0       61 2023-03-23 20:56:12.199461 morningstar_data-1.3.0/morningstar_data/datalake/__init__.py
--rw-r--r--   0        0        0       62 2023-03-23 20:56:12.199647 morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/__init__.py
--rw-r--r--   0        0        0      556 2023-03-23 20:56:12.199811 morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/_file.py
--rw-r--r--   0        0        0      762 2023-03-23 20:56:12.200012 morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/_table.py
--rw-r--r--   0        0        0      996 2023-03-23 20:56:12.200274 morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/csvfile.py
--rw-r--r--   0        0        0     2163 2023-06-14 19:10:47.534854 morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/temptable.py
--rw-r--r--   0        0        0      552 2023-06-22 17:07:28.075659 morningstar_data-1.3.0/morningstar_data/datalake/_error_messages.py
--rw-r--r--   0        0        0      936 2023-06-14 19:10:47.535372 morningstar_data-1.3.0/morningstar_data/datalake/_exceptions.py
--rw-r--r--   0        0        0     5620 2023-06-22 17:07:28.076042 morningstar_data-1.3.0/morningstar_data/datalake/base.py
--rw-r--r--   0        0        0      939 2023-06-14 19:10:47.536605 morningstar_data-1.3.0/morningstar_data/direct/__init__.py
--rw-r--r--   0        0        0     2433 2023-06-14 19:10:47.537161 morningstar_data-1.3.0/morningstar_data/direct/_api.py
--rw-r--r--   0        0        0      179 2023-06-14 19:10:47.537414 morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/__init__.py
--rw-r--r--   0        0        0     1831 2023-06-22 17:07:28.076775 morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_delivery_backend.py
--rw-r--r--   0        0        0     5148 2023-06-14 19:10:47.537772 morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_holdings_backend.py
--rw-r--r--   0        0        0     3355 2023-06-14 19:10:47.537906 morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py
--rw-r--r--   0        0        0     3751 2023-06-14 19:10:47.538259 morningstar_data-1.3.0/morningstar_data/direct/_base_api.py
--rw-r--r--   0        0        0     5241 2023-06-22 23:57:19.312478 morningstar_data-1.3.0/morningstar_data/direct/_config.py
--rw-r--r--   0        0        0     1999 2022-07-19 18:10:19.834957 morningstar_data-1.3.0/morningstar_data/direct/_config_key.py
--rw-r--r--   0        0        0     7434 2023-06-22 17:07:28.077965 morningstar_data-1.3.0/morningstar_data/direct/_core_api.py
--rw-r--r--   0        0        0      197 2022-07-19 18:10:19.835284 morningstar_data-1.3.0/morningstar_data/direct/_data_objects/__init__.py
--rw-r--r--   0        0        0     2298 2022-07-19 18:10:19.835489 morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py
--rw-r--r--   0        0        0    26357 2023-06-22 17:07:28.078754 morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_data_points_object.py
--rw-r--r--   0        0        0     7532 2023-03-23 20:56:12.207196 morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_investments_object.py
--rw-r--r--   0        0        0     2572 2023-06-22 17:07:28.079551 morningstar_data-1.3.0/morningstar_data/direct/_data_point.py
--rw-r--r--   0        0        0     1051 2022-07-19 18:10:19.836661 morningstar_data-1.3.0/morningstar_data/direct/_data_type.py
--rw-r--r--   0        0        0     1593 2023-06-22 17:07:28.080200 morningstar_data-1.3.0/morningstar_data/direct/_decorator.py
--rw-r--r--   0        0        0    13892 2023-06-22 17:07:28.080827 morningstar_data-1.3.0/morningstar_data/direct/_error_messages.py
--rw-r--r--   0        0        0     3463 2023-06-22 17:07:28.081496 morningstar_data-1.3.0/morningstar_data/direct/_exceptions.py
--rw-r--r--   0        0        0        0 2022-07-19 18:10:19.837832 morningstar_data-1.3.0/morningstar_data/direct/_investment/__init__.py
--rw-r--r--   0        0        0     4288 2023-06-14 19:10:47.544214 morningstar_data-1.3.0/morningstar_data/direct/_investment/_asset_flow_data.py
--rw-r--r--   0        0        0     1546 2023-06-14 19:10:47.544648 morningstar_data-1.3.0/morningstar_data/direct/_investment/_common.py
--rw-r--r--   0        0        0     6085 2023-06-14 19:10:47.545176 morningstar_data-1.3.0/morningstar_data/direct/_investment/_data.py
--rw-r--r--   0        0        0     8369 2023-06-22 17:07:28.082117 morningstar_data-1.3.0/morningstar_data/direct/_investment/_normal_data.py
--rw-r--r--   0        0        0     5023 2023-06-14 19:10:47.546410 morningstar_data-1.3.0/morningstar_data/direct/_investment/_peer_group_data.py
--rw-r--r--   0        0        0      162 2023-03-23 20:56:12.208683 morningstar_data-1.3.0/morningstar_data/direct/_portfolio/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-14 19:10:47.546903 morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_common.py
--rw-r--r--   0        0        0     7859 2023-06-20 16:42:44.590672 morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
--rw-r--r--   0        0        0     7913 2023-06-20 16:42:44.590988 morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_settings.py
--rw-r--r--   0        0        0      955 2023-03-23 20:56:12.210194 morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_type.py
--rw-r--r--   0        0        0    10975 2023-06-14 19:10:47.548557 morningstar_data-1.3.0/morningstar_data/direct/_portfolio_data_set.py
--rw-r--r--   0        0        0     3357 2023-06-14 19:10:47.548933 morningstar_data-1.3.0/morningstar_data/direct/_utils.py
--rw-r--r--   0        0        0    13061 2023-06-22 17:07:28.082813 morningstar_data-1.3.0/morningstar_data/direct/asset_flow.py
--rw-r--r--   0        0        0    16274 2023-06-22 17:07:28.083438 morningstar_data-1.3.0/morningstar_data/direct/custom_database.py
--rw-r--r--   0        0        0     1236 2022-07-19 18:10:19.841830 morningstar_data-1.3.0/morningstar_data/direct/data_type.py
--rw-r--r--   0        0        0    42528 2023-06-22 17:07:28.084133 morningstar_data-1.3.0/morningstar_data/direct/holdings.py
--rw-r--r--   0        0        0    13577 2023-06-22 17:07:28.084678 morningstar_data-1.3.0/morningstar_data/direct/investment.py
--rw-r--r--   0        0        0    32223 2023-06-22 17:07:28.085565 morningstar_data-1.3.0/morningstar_data/direct/lookup.py
--rw-r--r--   0        0        0     6040 2023-06-22 17:07:28.086336 morningstar_data-1.3.0/morningstar_data/direct/peer_group.py
--rw-r--r--   0        0        0    19389 2023-06-22 17:07:28.087121 morningstar_data-1.3.0/morningstar_data/direct/performance_report.py
--rw-r--r--   0        0        0    37181 2023-06-22 17:07:28.087827 morningstar_data-1.3.0/morningstar_data/direct/portfolio.py
--rw-r--r--   0        0        0    12562 2023-06-22 17:07:28.088426 morningstar_data-1.3.0/morningstar_data/direct/returns.py
--rw-r--r--   0        0        0      413 2023-03-23 20:56:12.218181 morningstar_data-1.3.0/morningstar_data/direct/user_items/__init__.py
--rw-r--r--   0        0        0      742 2022-07-19 18:10:19.845539 morningstar_data-1.3.0/morningstar_data/direct/user_items/_utils.py
--rw-r--r--   0        0        0     7888 2023-06-22 17:07:28.088937 morningstar_data-1.3.0/morningstar_data/direct/user_items/data_set.py
--rw-r--r--   0        0        0    12981 2023-06-22 17:07:28.089417 morningstar_data-1.3.0/morningstar_data/direct/user_items/investment_lists.py
--rw-r--r--   0        0        0    11145 2023-06-20 16:42:44.598186 morningstar_data-1.3.0/morningstar_data/direct/user_items/portfolio.py
--rw-r--r--   0        0        0    10308 2023-06-22 17:07:28.089811 morningstar_data-1.3.0/morningstar_data/direct/user_items/search_criteria.py
--rw-r--r--   0        0        0     4752 2023-06-22 17:07:28.090463 morningstar_data-1.3.0/morningstar_data/lookup.py
--rw-r--r--   0        0        0      157 2023-06-14 19:10:47.555441 morningstar_data-1.3.0/morningstar_data/utils/__init__.py
--rw-r--r--   0        0        0     6359 2023-06-14 19:10:47.555845 morningstar_data-1.3.0/morningstar_data/utils/_delivery_config.py
--rw-r--r--   0        0        0     7752 2023-06-22 23:57:19.313230 morningstar_data-1.3.0/morningstar_data/utils/_helpers.py
--rw-r--r--   0        0        0    10435 2023-06-22 17:07:28.091516 morningstar_data-1.3.0/morningstar_data/utils/delivery.py
--rw-r--r--   0        0        0     2452 2023-06-23 00:21:47.576159 morningstar_data-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    12382 1970-01-01 00:00:00.000000 morningstar_data-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-07-11 19:45:18.025249 morningstar_data-1.3.1/LICENSE
+-rw-r--r--   0        0        0    11379 2023-07-11 19:45:18.029249 morningstar_data-1.3.1/README.md
+-rw-r--r--   0        0        0      207 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/__init__.py
+-rw-r--r--   0        0        0      599 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/_base.py
+-rw-r--r--   0        0        0     3056 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/_utils.py
+-rw-r--r--   0        0        0       82 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/_version.py
+-rw-r--r--   0        0        0       61 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/__init__.py
+-rw-r--r--   0        0        0      556 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/_file.py
+-rw-r--r--   0        0        0      762 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/_table.py
+-rw-r--r--   0        0        0      996 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/csvfile.py
+-rw-r--r--   0        0        0     2163 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/temptable.py
+-rw-r--r--   0        0        0      552 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_error_messages.py
+-rw-r--r--   0        0        0      936 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_exceptions.py
+-rw-r--r--   0        0        0     5620 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/base.py
+-rw-r--r--   0        0        0      939 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/__init__.py
+-rw-r--r--   0        0        0     2433 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_api.py
+-rw-r--r--   0        0        0      179 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/__init__.py
+-rw-r--r--   0        0        0     1845 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_delivery_backend.py
+-rw-r--r--   0        0        0     4801 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_holdings_backend.py
+-rw-r--r--   0        0        0     3361 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_signed_url_backend.py
+-rw-r--r--   0        0        0     3762 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_base_api.py
+-rw-r--r--   0        0        0     4947 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_config.py
+-rw-r--r--   0        0        0     1999 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_config_key.py
+-rw-r--r--   0        0        0     7434 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_core_api.py
+-rw-r--r--   0        0        0      197 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_objects/__init__.py
+-rw-r--r--   0        0        0     2298 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_custom_data_points_types.py
+-rw-r--r--   0        0        0    26357 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_data_points_object.py
+-rw-r--r--   0        0        0     7532 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_investments_object.py
+-rw-r--r--   0        0        0     2572 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_point.py
+-rw-r--r--   0        0        0     1051 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_type.py
+-rw-r--r--   0        0        0     1593 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_decorator.py
+-rw-r--r--   0        0        0    13892 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_error_messages.py
+-rw-r--r--   0        0        0     3463 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/__init__.py
+-rw-r--r--   0        0        0     4288 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/_asset_flow_data.py
+-rw-r--r--   0        0        0     1546 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/_common.py
+-rw-r--r--   0        0        0     6085 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/_data.py
+-rw-r--r--   0        0        0     8369 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/_normal_data.py
+-rw-r--r--   0        0        0     5023 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/_peer_group_data.py
+-rw-r--r--   0        0        0      162 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_common.py
+-rw-r--r--   0        0        0     7859 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
+-rw-r--r--   0        0        0     7913 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_settings.py
+-rw-r--r--   0        0        0      955 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_type.py
+-rw-r--r--   0        0        0    10975 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio_data_set.py
+-rw-r--r--   0        0        0     3357 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_utils.py
+-rw-r--r--   0        0        0    13061 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/asset_flow.py
+-rw-r--r--   0        0        0    16274 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/custom_database.py
+-rw-r--r--   0        0        0     1236 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/data_type.py
+-rw-r--r--   0        0        0    42528 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/holdings.py
+-rw-r--r--   0        0        0    13577 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/investment.py
+-rw-r--r--   0        0        0    32223 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/lookup.py
+-rw-r--r--   0        0        0     6040 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/peer_group.py
+-rw-r--r--   0        0        0    19389 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/performance_report.py
+-rw-r--r--   0        0        0    37181 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/portfolio.py
+-rw-r--r--   0        0        0    12562 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/returns.py
+-rw-r--r--   0        0        0      413 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/__init__.py
+-rw-r--r--   0        0        0      742 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/_utils.py
+-rw-r--r--   0        0        0     7888 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/data_set.py
+-rw-r--r--   0        0        0    12981 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/investment_lists.py
+-rw-r--r--   0        0        0    11145 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/portfolio.py
+-rw-r--r--   0        0        0    10308 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/search_criteria.py
+-rw-r--r--   0        0        0     4752 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/lookup.py
+-rw-r--r--   0        0        0      157 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/utils/__init__.py
+-rw-r--r--   0        0        0     6359 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/utils/_delivery_config.py
+-rw-r--r--   0        0        0     7752 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/utils/_helpers.py
+-rw-r--r--   0        0        0    10435 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/utils/delivery.py
+-rw-r--r--   0        0        0     2530 2023-07-11 19:46:06.420424 morningstar_data-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    12488 1970-01-01 00:00:00.000000 morningstar_data-1.3.1/PKG-INFO
```

### Comparing `morningstar_data-1.3.0/LICENSE` & `morningstar_data-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/README.md` & `morningstar_data-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,45 +2,50 @@
 
 The morningstar_data Python package provides users quick programmatic access to Morningstar data. It is a building block for doing practical investment data analysis in Python.
 
 # Getting Started
 
 ## Installation
 
+### Installing via pip
 ```
 pip install morningstar-data
 ```
 
+### Installing via conda
+```
+conda install -c conda-forge morningstar-data
+```
+
 **Warning**: Importing the package before authenticating will produce an error. See below for authentication steps.
 
 ## Authentication
 ### Retrieve Authentication Token
 1. Open [Analytics Lab](https://analyticslab.morningstar.com/) in your browser
 2. Login with your Morningstar Direct credentials
 3. On the top ribbon in the "Analytics Lab" dropdown menu select "Copy Authentication Token". This will copy your token to the clipboard.
 
 ![copy auth token](https://al-morningstar-readme-images-temp.s3.amazonaws.com/copy_auth_token.png)
 
 ### Set Authentication Token
-Set the environment variable `MD_AUTH_TOKEN`using the token you retrieved previously
+Set the environment variable `MD_AUTH_TOKEN` using the token you retrieved previously
 #### Bash
 
 `export MD_AUTH_TOKEN="paste copied token here"`
 
 #### Within a Python (.py) File
 
 ```
 # testing_morningstar_data.py
 import os
 
 os.environ['MD_AUTH_TOKEN']="paste copied token here"
 
 import morningstar_data as md
 ```
-**Note:** importing morningstar_data comes **after** setting the authentication token
 
 ## Requirements
 
 The morningstar_data package is tested with
 
 |             | Main version (latest)
 |-------------|------------------------------|
```

### Comparing `morningstar_data-1.3.0/morningstar_data/_base.py` & `morningstar_data-1.3.1/morningstar_data/_base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/_utils.py` & `morningstar_data-1.3.1/morningstar_data/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/_file.py` & `morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/_file.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/_table.py` & `morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/_table.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/csvfile.py` & `morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/csvfile.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/temptable.py` & `morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/temptable.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/datalake/_error_messages.py` & `morningstar_data-1.3.1/morningstar_data/datalake/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/datalake/_exceptions.py` & `morningstar_data-1.3.1/morningstar_data/datalake/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/datalake/base.py` & `morningstar_data-1.3.1/morningstar_data/datalake/base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/__init__.py` & `morningstar_data-1.3.1/morningstar_data/direct/__init__.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_api.py` & `morningstar_data-1.3.1/morningstar_data/direct/_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_delivery_backend.py` & `morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_delivery_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         request_id = os.getenv("REQUEST_ID", str(uuid.uuid4()))
         _logger.info(f"RequestId: {request_id} passed to POST requests")
         return request_id
 
     def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
         _logger.info(f"Requesting: {method} {url}")
         try:
-            self.headers["X-API-RequestId"] = self._get_request_id()
-            res = make_request(method, url, headers=self.headers, verify=False, data=data)
+            headers = {**self.get_headers(), "X-API-RequestId": self._get_request_id()}
+            res = make_request(method, url, headers=headers, verify=False, data=data)
             res.raise_for_status()
             return res.json()
         except requests.ConnectionError:
             raise NetworkExceptionError from None
         except requests.HTTPError:
             self._handle_custom_http_errors(res)
             self._handle_default_http_errors(res)
```

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_holdings_backend.py` & `morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_holdings_backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
         """
         Request and handle OK (status_code = 200) and network error responses.
         """
         _logger.info(f"Requesting: {method} {url}")
         try:
-            res = make_request(method, url, headers=self.headers, verify=True, data=data)
+            res = make_request(method, url, headers=self.get_headers(), verify=True, data=data)
             res.raise_for_status()
             # We have asked FOF team to return JSON object in the API, so we don't have to implement this class completely like this.
             # https://mswiki.morningstar.com/display/DWH/AL+FOF+Lookthrough+Holding?focusedCommentId=645255358#comment-645255358
             return res.json()
         except requests.ConnectionError:
             raise NetworkExceptionError from None
         except requests.HTTPError:
@@ -114,21 +114,15 @@
 
     def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
         """
         Request and handle OK (status_code = 200) and network error responses.
         """
         _logger.info(f"Requesting: {method} {url}")
         try:
-            # We will remove this after testing
-
-            self.headers["authorization"] = f"Bearer {_config.get_uim_token()}"  # Because we don't have  PROD FOF API, and dont' have custom user data in the NON PROD DO APIs
-            self.headers["x-api-requestid"] = str(uuid.uuid4())
-            self.headers["x-api-userid"] = os.environ["UIM_USER_ID"]
-
-            res = make_request(method, url, headers=self.headers, verify=True, data=data)
+            res = make_request(method, url, headers=self.get_headers(), verify=True, data=data)
             res.raise_for_status()
             return res.json()
         except requests.ConnectionError:
             raise NetworkExceptionError from None
         except requests.HTTPError:
             self._handle_custom_http_errors(res)
             self._handle_default_http_errors(res)
```

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py` & `morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_signed_url_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
         """
         Request and handle OK (status_code = 200) and network error responses.
         """
         _logger.info(f"Requesting: {method} {url}")
         try:
-            res = make_request(method=method, url=url, headers=self.headers, verify=False, data=json.dumps(data))
+            res = make_request(method=method, url=url, headers=self.get_headers(), verify=False, data=json.dumps(data))
             res.raise_for_status()
             return res.text
         except requests.ConnectionError:
             raise NetworkExceptionError from None
         except requests.HTTPError:
             self._handle_custom_http_errors(res)
             self._handle_default_http_errors(res)
```

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_base_api.py` & `morningstar_data-1.3.1/morningstar_data/direct/_base_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,14 @@
 
 
 class APIBackend(ABC):
     """
     Abstract class for all API requests
     """
 
-    def __init__(self) -> None:
-        self.headers = _config.get_headers()
-
     def do_get_request(self, url: str) -> Any:
         """
         Makes a GET request
         """
         return self._make_request(url, "GET")
 
     def do_post_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
@@ -42,21 +39,24 @@
 
     def do_put_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
         """
         Makes a PUT request
         """
         return self._make_request(url, "PUT", data)
 
+    def get_headers(self) -> Dict[str, str]:
+        return _config.get_headers()
+
     def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
         """
         Request and handle OK (status_code = 200) and network error responses.
         """
         _logger.info(f"Requesting: {method} {url}")
         try:
-            res = make_request(method, url, headers=self.headers, verify=False, data=data)
+            res = make_request(method, url, headers=self.get_headers(), verify=False, data=data)
             res.raise_for_status()
             return res.json()
         except requests.ConnectionError as e:
             raise NetworkExceptionError from None
         except requests.HTTPError as e:
             self._handle_custom_http_errors(res)
             self._handle_default_http_errors(res)
```

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_config.py` & `morningstar_data-1.3.1/morningstar_data/direct/_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,31 +9,22 @@
 from ._exceptions import EAMSTokenDoesNotExistError, MalformedJWTError, CredentialsException
 
 
 @dataclass
 class _Config:
     def __init__(self) -> None:
         self._MD_API: str = os.getenv("MD_API", "https://www.us-api.morningstar.com/md-api/")
-        md_auth_token = md_auth_token = os.getenv("MD_AUTH_TOKEN", os.getenv("UIM_JWT", ""))
-        self.token = md_auth_token
-        if self.token == "":
-            raise CredentialsException("Please set up MD_AUTH_TOKEN environment variable to access the morningstar_data package")
 
-    @property
-    def token(self) -> str:
-        # TODO: Test the token
-        return self._JWT
-
-    @token.setter
-    def token(self, new_token: str) -> None:
-        fixed_token = self._filter_invalid_jwt(new_token)
-        self._JWT = fixed_token
 
     def get_uim_token(self) -> str:
-        return self.token
+        token = os.getenv("MD_AUTH_TOKEN", os.getenv("UIM_JWT", ""))
+        if token == "":
+            raise CredentialsException("Please set up MD_AUTH_TOKEN environment variable to access the morningstar_data package")
+        return self._filter_invalid_jwt(token)
+
 
     def get_headers(self, add_headers: Dict[str, str] = {}) -> Dict[str, str]:
         headers = {
             "X-API-ComponentId": os.getenv("DO_API_REQUEST_ORIGIN", "analyticslab"),
             "X-API-Sourceapp": os.getenv("DO_API_REQUEST_ORIGIN", "morningstar-data"),
             "X-API-ProductId": "Direct",
             "Content-Type": "application/json",
```

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_config_key.py` & `morningstar_data-1.3.1/morningstar_data/direct/_config_key.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_core_api.py` & `morningstar_data-1.3.1/morningstar_data/direct/_core_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py` & `morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_custom_data_points_types.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_data_points_object.py` & `morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_data_points_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_investments_object.py` & `morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_investments_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_data_point.py` & `morningstar_data-1.3.1/morningstar_data/direct/_data_point.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_data_type.py` & `morningstar_data-1.3.1/morningstar_data/direct/_data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_decorator.py` & `morningstar_data-1.3.1/morningstar_data/direct/_decorator.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_error_messages.py` & `morningstar_data-1.3.1/morningstar_data/direct/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_exceptions.py` & `morningstar_data-1.3.1/morningstar_data/direct/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_investment/_asset_flow_data.py` & `morningstar_data-1.3.1/morningstar_data/direct/_investment/_asset_flow_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_investment/_common.py` & `morningstar_data-1.3.1/morningstar_data/direct/_investment/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_investment/_data.py` & `morningstar_data-1.3.1/morningstar_data/direct/_investment/_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_investment/_normal_data.py` & `morningstar_data-1.3.1/morningstar_data/direct/_investment/_normal_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_investment/_peer_group_data.py` & `morningstar_data-1.3.1/morningstar_data/direct/_investment/_peer_group_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_common.py` & `morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py` & `morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_settings.py` & `morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_settings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_type.py` & `morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_portfolio_data_set.py` & `morningstar_data-1.3.1/morningstar_data/direct/_portfolio_data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/_utils.py` & `morningstar_data-1.3.1/morningstar_data/direct/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/asset_flow.py` & `morningstar_data-1.3.1/morningstar_data/direct/asset_flow.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/custom_database.py` & `morningstar_data-1.3.1/morningstar_data/direct/custom_database.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/data_type.py` & `morningstar_data-1.3.1/morningstar_data/direct/data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/holdings.py` & `morningstar_data-1.3.1/morningstar_data/direct/holdings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/investment.py` & `morningstar_data-1.3.1/morningstar_data/direct/investment.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/lookup.py` & `morningstar_data-1.3.1/morningstar_data/direct/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/peer_group.py` & `morningstar_data-1.3.1/morningstar_data/direct/peer_group.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/performance_report.py` & `morningstar_data-1.3.1/morningstar_data/direct/performance_report.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/portfolio.py` & `morningstar_data-1.3.1/morningstar_data/direct/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/returns.py` & `morningstar_data-1.3.1/morningstar_data/direct/returns.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/user_items/_utils.py` & `morningstar_data-1.3.1/morningstar_data/direct/user_items/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/user_items/data_set.py` & `morningstar_data-1.3.1/morningstar_data/direct/user_items/data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/user_items/investment_lists.py` & `morningstar_data-1.3.1/morningstar_data/direct/user_items/investment_lists.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/user_items/portfolio.py` & `morningstar_data-1.3.1/morningstar_data/direct/user_items/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/direct/user_items/search_criteria.py` & `morningstar_data-1.3.1/morningstar_data/direct/user_items/search_criteria.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/lookup.py` & `morningstar_data-1.3.1/morningstar_data/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/utils/_delivery_config.py` & `morningstar_data-1.3.1/morningstar_data/utils/_delivery_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/utils/_helpers.py` & `morningstar_data-1.3.1/morningstar_data/utils/_helpers.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/morningstar_data/utils/delivery.py` & `morningstar_data-1.3.1/morningstar_data/utils/delivery.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.0/pyproject.toml` & `morningstar_data-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "morningstar_data"
-version = "1.3.0"
+version = "1.3.1"
 description = "Morningstar Data"
 authors = ["Morningstar, Inc."]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.morningstar.com/products/md-python-package"
+documentation = "https://docs-analyticslab.morningstar.com/latest/index.html"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "~1.5.3"
 typeguard = "^2.13.3"
 PyJWT = "^2.4.0"
 boto3 = "^1.20.1"
```

### Comparing `morningstar_data-1.3.0/PKG-INFO` & `morningstar_data-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morningstar-data
-Version: 1.3.0
+Version: 1.3.1
 Summary: Morningstar Data
 Home-page: https://www.morningstar.com/products/md-python-package
 License: Apache-2.0
 Author: Morningstar, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -19,55 +19,61 @@
 Requires-Dist: polling2 (==0.5.0)
 Requires-Dist: pyopenssl (>=23.1.1,<24.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: simplejson (>=3.18.4,<4.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: typeguard (>=2.13.3,<3.0.0)
 Requires-Dist: urllib3 (>=1.26,<2.0)
+Project-URL: Documentation, https://docs-analyticslab.morningstar.com/latest/index.html
 Description-Content-Type: text/markdown
 
 # Morningstar Data Package
 
 The morningstar_data Python package provides users quick programmatic access to Morningstar data. It is a building block for doing practical investment data analysis in Python.
 
 # Getting Started
 
 ## Installation
 
+### Installing via pip
 ```
 pip install morningstar-data
 ```
 
+### Installing via conda
+```
+conda install -c conda-forge morningstar-data
+```
+
 **Warning**: Importing the package before authenticating will produce an error. See below for authentication steps.
 
 ## Authentication
 ### Retrieve Authentication Token
 1. Open [Analytics Lab](https://analyticslab.morningstar.com/) in your browser
 2. Login with your Morningstar Direct credentials
 3. On the top ribbon in the "Analytics Lab" dropdown menu select "Copy Authentication Token". This will copy your token to the clipboard.
 
 ![copy auth token](https://al-morningstar-readme-images-temp.s3.amazonaws.com/copy_auth_token.png)
 
 ### Set Authentication Token
-Set the environment variable `MD_AUTH_TOKEN`using the token you retrieved previously
+Set the environment variable `MD_AUTH_TOKEN` using the token you retrieved previously
 #### Bash
 
 `export MD_AUTH_TOKEN="paste copied token here"`
 
 #### Within a Python (.py) File
 
 ```
 # testing_morningstar_data.py
 import os
 
 os.environ['MD_AUTH_TOKEN']="paste copied token here"
 
 import morningstar_data as md
 ```
-**Note:** importing morningstar_data comes **after** setting the authentication token
 
 ## Requirements
 
 The morningstar_data package is tested with
 
 |             | Main version (latest)
 |-------------|------------------------------|
```

